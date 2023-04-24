# Comparing `tmp/k8s_audit_filter-0.0.4-py3-none-any.whl.zip` & `tmp/k8s_audit_filter-0.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 17401 bytes, number of entries: 8
+Zip file size: 17695 bytes, number of entries: 9
+-rw-r--r--  2.0 unx       22 b- defN 20-Feb-02 00:00 k8s_audit_filter/__about__.py
 -rw-r--r--  2.0 unx       81 b- defN 20-Feb-02 00:00 k8s_audit_filter/__init__.py
 -rw-r--r--  2.0 unx     1564 b- defN 20-Feb-02 00:00 k8s_audit_filter/audit_filter.py
--rw-r--r--  2.0 unx     1512 b- defN 20-Feb-02 00:00 k8s_audit_filter/fields.py
+-rw-r--r--  2.0 unx     2197 b- defN 20-Feb-02 00:00 k8s_audit_filter/fields.py
 -rw-r--r--  2.0 unx     1356 b- defN 20-Feb-02 00:00 k8s_audit_filter/rules.py
-?rw-r--r--  2.0 unx     4878 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.0.4.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.0.4.dist-info/WHEEL
-?rw-r--r--  2.0 unx    35149 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.0.4.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      677 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.0.4.dist-info/RECORD
-8 files, 45304 bytes uncompressed, 16215 bytes compressed:  64.2%
+?rw-r--r--  2.0 unx     4848 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.1.0.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.1.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx    35149 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.1.0.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      761 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.1.0.dist-info/RECORD
+9 files, 46065 bytes uncompressed, 16375 bytes compressed:  64.5%
```

## zipnote {}

```diff
@@ -1,25 +1,28 @@
+Filename: k8s_audit_filter/__about__.py
+Comment: 
+
 Filename: k8s_audit_filter/__init__.py
 Comment: 
 
 Filename: k8s_audit_filter/audit_filter.py
 Comment: 
 
 Filename: k8s_audit_filter/fields.py
 Comment: 
 
 Filename: k8s_audit_filter/rules.py
 Comment: 
 
-Filename: k8s_audit_filter-0.0.4.dist-info/METADATA
+Filename: k8s_audit_filter-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: k8s_audit_filter-0.0.4.dist-info/WHEEL
+Filename: k8s_audit_filter-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: k8s_audit_filter-0.0.4.dist-info/licenses/LICENSE
+Filename: k8s_audit_filter-0.1.0.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: k8s_audit_filter-0.0.4.dist-info/RECORD
+Filename: k8s_audit_filter-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## k8s_audit_filter/fields.py

```diff
@@ -33,22 +33,47 @@
 
     def check_match(self, target: dict) -> bool:
         if target[self.name] in self.value:
             return True
         return False
 
 
+class UsersField(BaseField):
+    def __init__(self, value: List[str]):
+        self.name = "user"
+        self.value: List[str] = value
+
+    def check_match(self, target: dict) -> bool:
+        if target[self.name]["username"] in self.value:
+            return True
+        return False
+
+
+class UserGroupsField(BaseField):
+    def __init__(self, value: List[str]):
+        self.name = "user"
+        self.value: List[str] = value
+
+    def check_match(self, target: dict) -> bool:
+        for group in target[self.name]["groups"]:
+            if group in self.value:
+                return True
+        return False
+
+
 class FieldException(Exception):
     pass
 
 
 class FieldFactory:
     field_mapping = {
         "level": LevelField,
         "verbs": VerbsField,
+        "users": UsersField,
+        "userGroups": UserGroupsField,
     }
 
     @classmethod
     def create(cls, fields: dict):
         result = []
         for key, vale in fields.items():
             if key in cls.field_mapping:
```

## Comparing `k8s_audit_filter-0.0.4.dist-info/METADATA` & `k8s_audit_filter-0.1.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k8s-audit-filter
-Version: 0.0.4
+Version: 0.1.0
 Summary: A tool to filter k8s audit logs
 Project-URL: Homepage, https://github.com/petrishutin/k8s-audit-filter
 Project-URL: Tracker, https://github.com/petrishutin/k8s-audit-filter/issues
 Author-email: Petr Ishutinr <ishutinpetrdev@gmail.com>
 License-File: LICENSE
 Keywords: audit,filter,k8s
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
@@ -117,35 +117,33 @@
   # Exclude line in the audit log which contains verb "create"
   - level: None
     verbs:
       - "create"
 
 ```
 
-
-
 ## Supported Rules
 
-The library supports the following rules:
-
-- ```level```
-- ```verbs```
-
 Please note, that ```level``` is required field for every rule, and should have of one of next values:
 
-- ```None``` - do not log events that match this rule
+- ```None``` - do not log events that match this rule (this is ExcludeRule)
 - ```Metadata``` - log line marked as "Metadata"
 - ```Request``` - log line marked as "Request"
 - ```RequestResponse``` - log line marked as "RequestResponse"
 
+The library supports the following rules k8s audit PolicyRules:
+
+- ```level```
+- ```verbs```
+- ```users```
+- ```userGroups```
+
 ## Limitations
 
-Currently, the library does not support the following rules:
+Currently, the library does not support following rules:
 
-- ```users``` - will be supported in the future
-- ```userGroups``` - will be supported in the future
 - ```nonResourceURLs``` - will be supported in the future
 - ```resources``` - will be supported in the future
 - ```namespaces``` - will be supported in the future
 - ```omitStages``` - now it does not distinguish any stages, and filter any string provided
   to ```AuditFilter.filter()```
 - ```omitManagedFields```
```

## Comparing `k8s_audit_filter-0.0.4.dist-info/licenses/LICENSE` & `k8s_audit_filter-0.1.0.dist-info/licenses/LICENSE`

 * *Files identical despite different names*


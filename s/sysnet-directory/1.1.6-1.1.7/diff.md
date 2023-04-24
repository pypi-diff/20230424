# Comparing `tmp/sysnet-directory-1.1.6.tar.gz` & `tmp/sysnet-directory-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysnet-directory-1.1.6.tar", last modified: Wed Apr 12 14:47:27 2023, max compression
+gzip compressed data, was "sysnet-directory-1.1.7.tar", last modified: Mon Apr 24 16:24:54 2023, max compression
```

## Comparing `sysnet-directory-1.1.6.tar` & `sysnet-directory-1.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 14:47:27.419129 sysnet-directory-1.1.6/
--rw-rw-rw-   0        0        0    12425 2022-12-10 17:50:43.000000 sysnet-directory-1.1.6/LICENSE.md
--rw-rw-rw-   0        0        0    19125 2023-04-12 14:47:27.419129 sysnet-directory-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     4443 2023-03-28 11:33:39.000000 sysnet-directory-1.1.6/README.md
--rw-rw-rw-   0        0        0      761 2023-04-12 14:46:27.000000 sysnet-directory-1.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-12 14:47:27.419129 sysnet-directory-1.1.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-12 14:47:27.408621 sysnet-directory-1.1.6/sysnet_directory/
--rw-rw-rw-   0        0        0        0 2022-12-07 11:26:06.000000 sysnet-directory-1.1.6/sysnet_directory/__init__.py
--rw-rw-rw-   0        0        0    15648 2023-04-12 14:46:27.000000 sysnet-directory-1.1.6/sysnet_directory/factory.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:47:27.408621 sysnet-directory-1.1.6/sysnet_directory.egg-info/
--rw-rw-rw-   0        0        0    19125 2023-04-12 14:47:27.000000 sysnet-directory-1.1.6/sysnet_directory.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-04-12 14:47:27.000000 sysnet-directory-1.1.6/sysnet_directory.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 14:47:27.000000 sysnet-directory-1.1.6/sysnet_directory.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-12 14:47:27.000000 sysnet-directory-1.1.6/sysnet_directory.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 16:24:54.190482 sysnet-directory-1.1.7/
+-rw-rw-rw-   0        0        0    12425 2022-12-10 17:50:43.000000 sysnet-directory-1.1.7/LICENSE.md
+-rw-rw-rw-   0        0        0    19125 2023-04-24 16:24:54.189482 sysnet-directory-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4443 2023-03-28 11:33:39.000000 sysnet-directory-1.1.7/README.md
+-rw-rw-rw-   0        0        0      761 2023-04-24 16:24:01.000000 sysnet-directory-1.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-24 16:24:54.190482 sysnet-directory-1.1.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-24 16:24:54.165235 sysnet-directory-1.1.7/sysnet_directory/
+-rw-rw-rw-   0        0        0        0 2022-12-07 11:26:06.000000 sysnet-directory-1.1.7/sysnet_directory/__init__.py
+-rw-rw-rw-   0        0        0    15728 2023-04-24 16:16:12.000000 sysnet-directory-1.1.7/sysnet_directory/factory.py
+drwxrwxrwx   0        0        0        0 2023-04-24 16:24:54.171235 sysnet-directory-1.1.7/sysnet_directory.egg-info/
+-rw-rw-rw-   0        0        0    19125 2023-04-24 16:24:54.000000 sysnet-directory-1.1.7/sysnet_directory.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-04-24 16:24:54.000000 sysnet-directory-1.1.7/sysnet_directory.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 16:24:54.000000 sysnet-directory-1.1.7/sysnet_directory.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-24 16:24:54.000000 sysnet-directory-1.1.7/sysnet_directory.egg-info/top_level.txt
```

### Comparing `sysnet-directory-1.1.6/LICENSE.md` & `sysnet-directory-1.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sysnet-directory-1.1.6/PKG-INFO` & `sysnet-directory-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysnet-directory
-Version: 1.1.6
+Version: 1.1.7
 Summary: Directory client library
 Author-email: Data Developer <info@sysnet.cz>
 License: # LICENCE PRO DOMÁCÍ POUŽITÍ (SYSNET Home Use License) v 1.0
         
         ## SHUL © SYSNET s.r.o. 2022
         
         <h4 style="text-align: center;">Tato komerční licence SYSNET s.r.o. se vztahuje na dílo (ve smyslu níže uvedených
```

### Comparing `sysnet-directory-1.1.6/README.md` & `sysnet-directory-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `sysnet-directory-1.1.6/pyproject.toml` & `sysnet-directory-1.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sysnet-directory"
-version = "1.1.6"
+version = "1.1.7"
 authors = [
   { name="Data Developer", email="info@sysnet.cz" },
 ]
 description = "Directory client library"
 readme = "README.md"
 license = { file="LICENSE.md" }
 requires-python = ">=3.9"
```

### Comparing `sysnet-directory-1.1.6/sysnet_directory/factory.py` & `sysnet-directory-1.1.7/sysnet_directory/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,19 +125,19 @@
         """
         if not self.ready:
             raise DirectoryException('LDAP Factory not ready')
         search_filter = 'objectClass~=person'
         sf = []
         if key is not None:
             # search_filter = '(&({0})(|(mail={1})(cn={1})(userPrincipalName={1})(title={1})))'.format(search_filter, key)
-            sf.append('(|(mail={0})(cn={0})(userPrincipalName={0})(title={0})(employeeNumber={0}))'.format(key))
+            sf.append('(|(mail={0})(cn={0})(userPrincipalName={0})(title={0})(employeeNumber={0})(sAMAccountName={0}))'.format(key))
         if ou is not None:
             # search_filter = '(&({})(departmentNumber~={}))'.format(search_filter, ou)
             # extensionAttribute4
-            sf.append('(|(departmentNumber={0})(extensionAttribute4={0})(extensionAttribute5={0}))'.format(ou))
+            sf.append('(|(departmentNumber={0})(extensionAttribute4={0})(extensionAttribute5={0})(company={0}))'.format(ou))
         if head:
             # search_filter = '(&({})(extensionAttribute2=1))'.format(search_filter)
             sf.append('(extensionAttribute2=1)')
         if sf:
             k = ''.join(sf)
             search_filter = '(&({0}){1})'.format(search_filter, k)
         search_scope = ldap.SCOPE_SUBTREE
@@ -198,18 +198,18 @@
     def get_all_users(self):
         return self.get_user()
 
     def get_user_map(self):
         ulist = self.get_user()
         out = {}
         for u in ulist:
-            id = u['employee_id']
-            if id not in [None, '']:
-                if id not in out:
-                    out[id] = u
+            eid = u['employee_id']
+            if eid not in [None, '']:
+                if eid not in out:
+                    out[eid] = u
         return out
 
     def get_all_groups(self):
         return self.get_group()
 
     def get_org_structure(self):
         """Vrátí organizační strukturu
@@ -269,14 +269,15 @@
     head_ou = None
     division = []
     # organizace
     organization_level_0 = {
         'code': 'MZP',
         'value': _get_item_value_string(user_item[1], 'company')
     }
+    head_ou = organization_level_0['code']
     division.append(organization_level_0)
     # sekce
     organization_level_1 = {
         'code': _get_item_value_string(user_item[1], 'extensionAttribute5'),
         'value': _get_item_value_string(user_item[1], 'extensionAttribute7')
     }
     if organization_level_1['code'] != '':
```

### Comparing `sysnet-directory-1.1.6/sysnet_directory.egg-info/PKG-INFO` & `sysnet-directory-1.1.7/sysnet_directory.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysnet-directory
-Version: 1.1.6
+Version: 1.1.7
 Summary: Directory client library
 Author-email: Data Developer <info@sysnet.cz>
 License: # LICENCE PRO DOMÁCÍ POUŽITÍ (SYSNET Home Use License) v 1.0
         
         ## SHUL © SYSNET s.r.o. 2022
         
         <h4 style="text-align: center;">Tato komerční licence SYSNET s.r.o. se vztahuje na dílo (ve smyslu níže uvedených
```


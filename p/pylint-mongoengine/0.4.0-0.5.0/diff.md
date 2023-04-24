# Comparing `tmp/pylint-mongoengine-0.4.0.tar.gz` & `tmp/pylint-mongoengine-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pylint-mongoengine-0.4.0.tar", last modified: Sat Sep 28 07:36:52 2019, max compression
+gzip compressed data, was "pylint-mongoengine-0.5.0.tar", last modified: Mon Apr 24 10:13:45 2023, max compression
```

## Comparing `pylint-mongoengine-0.4.0.tar` & `pylint-mongoengine-0.5.0.tar`

### file list

```diff
@@ -1,31 +1,20 @@
-drwxr-xr-x   0 juca      (1000) juca      (1000)        0 2019-09-28 07:36:52.000000 pylint-mongoengine-0.4.0/
--rw-r--r--   0 juca      (1000) juca      (1000)      790 2019-09-28 07:36:52.000000 pylint-mongoengine-0.4.0/PKG-INFO
--rw-r--r--   0 juca      (1000) juca      (1000)      402 2018-09-12 09:27:22.000000 pylint-mongoengine-0.4.0/README.md
-drwxr-xr-x   0 juca      (1000) juca      (1000)        0 2019-09-28 07:36:52.000000 pylint-mongoengine-0.4.0/pylint_mongoengine/
--rw-r--r--   0 juca      (1000) juca      (1000)     1433 2019-09-28 07:36:10.000000 pylint-mongoengine-0.4.0/pylint_mongoengine/__init__.py
-drwxr-xr-x   0 juca      (1000) juca      (1000)        0 2019-09-28 07:36:52.000000 pylint-mongoengine-0.4.0/pylint_mongoengine/checkers/
--rw-r--r--   0 juca      (1000) juca      (1000)       24 2018-09-12 14:17:16.000000 pylint-mongoengine-0.4.0/pylint_mongoengine/checkers/__init__.py
--rw-r--r--   0 juca      (1000) juca      (1000)     2097 2019-09-28 07:36:10.000000 pylint-mongoengine-0.4.0/pylint_mongoengine/checkers/mongoengine.py
--rw-r--r--   0 juca      (1000) juca      (1000)     5760 2019-09-28 07:36:10.000000 pylint-mongoengine-0.4.0/pylint_mongoengine/suppression.py
--rw-r--r--   0 juca      (1000) juca      (1000)     5536 2019-09-28 07:36:10.000000 pylint-mongoengine-0.4.0/pylint_mongoengine/utils.py
-drwxr-xr-x   0 juca      (1000) juca      (1000)        0 2019-09-28 07:36:52.000000 pylint-mongoengine-0.4.0/pylint_mongoengine.egg-info/
--rw-r--r--   0 juca      (1000) juca      (1000)      790 2019-09-28 07:36:52.000000 pylint-mongoengine-0.4.0/pylint_mongoengine.egg-info/PKG-INFO
--rw-r--r--   0 juca      (1000) juca      (1000)      671 2019-09-28 07:36:52.000000 pylint-mongoengine-0.4.0/pylint_mongoengine.egg-info/SOURCES.txt
--rw-r--r--   0 juca      (1000) juca      (1000)        1 2019-09-28 07:36:52.000000 pylint-mongoengine-0.4.0/pylint_mongoengine.egg-info/dependency_links.txt
--rw-r--r--   0 juca      (1000) juca      (1000)        1 2018-09-12 09:35:09.000000 pylint-mongoengine-0.4.0/pylint_mongoengine.egg-info/not-zip-safe
--rw-r--r--   0 juca      (1000) juca      (1000)       37 2019-09-28 07:36:52.000000 pylint-mongoengine-0.4.0/pylint_mongoengine.egg-info/requires.txt
--rw-r--r--   0 juca      (1000) juca      (1000)       25 2019-09-28 07:36:52.000000 pylint-mongoengine-0.4.0/pylint_mongoengine.egg-info/top_level.txt
--rw-r--r--   0 juca      (1000) juca      (1000)       38 2019-09-28 07:36:52.000000 pylint-mongoengine-0.4.0/setup.cfg
--rw-r--r--   0 juca      (1000) juca      (1000)     1058 2019-09-28 07:36:10.000000 pylint-mongoengine-0.4.0/setup.py
-drwxr-xr-x   0 juca      (1000) juca      (1000)        0 2019-09-28 07:36:52.000000 pylint-mongoengine-0.4.0/tests/
--rw-r--r--   0 juca      (1000) juca      (1000)        0 2018-09-13 20:36:21.000000 pylint-mongoengine-0.4.0/tests/__init__.py
-drwxr-xr-x   0 juca      (1000) juca      (1000)        0 2019-09-28 07:36:52.000000 pylint-mongoengine-0.4.0/tests/functional/
--rw-r--r--   0 juca      (1000) juca      (1000)        0 2018-09-13 20:36:32.000000 pylint-mongoengine-0.4.0/tests/functional/__init__.py
--rw-r--r--   0 juca      (1000) juca      (1000)     1218 2019-09-28 07:36:10.000000 pylint-mongoengine-0.4.0/tests/functional/test_func.py
-drwxr-xr-x   0 juca      (1000) juca      (1000)        0 2019-09-28 07:36:52.000000 pylint-mongoengine-0.4.0/tests/unit/
--rw-r--r--   0 juca      (1000) juca      (1000)        0 2018-09-13 20:36:25.000000 pylint-mongoengine-0.4.0/tests/unit/__init__.py
-drwxr-xr-x   0 juca      (1000) juca      (1000)        0 2019-09-28 07:36:52.000000 pylint-mongoengine-0.4.0/tests/unit/checkers/
--rw-r--r--   0 juca      (1000) juca      (1000)       24 2018-09-13 20:36:44.000000 pylint-mongoengine-0.4.0/tests/unit/checkers/__init__.py
--rw-r--r--   0 juca      (1000) juca      (1000)     3373 2019-09-28 07:36:10.000000 pylint-mongoengine-0.4.0/tests/unit/checkers/test_mongoengine.py
--rw-r--r--   0 juca      (1000) juca      (1000)     3130 2019-09-28 07:36:10.000000 pylint-mongoengine-0.4.0/tests/unit/test_suppresion.py
--rw-r--r--   0 juca      (1000) juca      (1000)     8604 2019-09-28 07:36:10.000000 pylint-mongoengine-0.4.0/tests/unit/test_utils.py
+drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-04-24 10:13:45.323529 pylint-mongoengine-0.5.0/
+-rw-rw-r--   0 juca      (1001) juca      (1001)    35147 2023-04-24 01:16:16.000000 pylint-mongoengine-0.5.0/LICENSE
+-rw-rw-r--   0 juca      (1001) juca      (1001)       11 2023-04-24 10:05:59.000000 pylint-mongoengine-0.5.0/MANIFEST.in
+-rw-rw-r--   0 juca      (1001) juca      (1001)     1131 2023-04-24 10:13:45.323529 pylint-mongoengine-0.5.0/PKG-INFO
+-rw-rw-r--   0 juca      (1001) juca      (1001)      656 2023-04-24 01:16:16.000000 pylint-mongoengine-0.5.0/README.md
+drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-04-24 10:13:45.323529 pylint-mongoengine-0.5.0/pylint_mongoengine/
+-rw-rw-r--   0 juca      (1001) juca      (1001)     1433 2023-04-24 01:16:16.000000 pylint-mongoengine-0.5.0/pylint_mongoengine/__init__.py
+drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-04-24 10:13:45.323529 pylint-mongoengine-0.5.0/pylint_mongoengine/checkers/
+-rw-rw-r--   0 juca      (1001) juca      (1001)       24 2023-04-24 01:16:16.000000 pylint-mongoengine-0.5.0/pylint_mongoengine/checkers/__init__.py
+-rw-rw-r--   0 juca      (1001) juca      (1001)     2097 2023-04-24 01:16:16.000000 pylint-mongoengine-0.5.0/pylint_mongoengine/checkers/mongoengine.py
+-rw-rw-r--   0 juca      (1001) juca      (1001)     5634 2023-04-24 08:39:35.000000 pylint-mongoengine-0.5.0/pylint_mongoengine/suppression.py
+-rw-rw-r--   0 juca      (1001) juca      (1001)     5027 2023-04-24 09:35:20.000000 pylint-mongoengine-0.5.0/pylint_mongoengine/utils.py
+drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-04-24 10:13:45.323529 pylint-mongoengine-0.5.0/pylint_mongoengine.egg-info/
+-rw-rw-r--   0 juca      (1001) juca      (1001)     1131 2023-04-24 10:13:45.000000 pylint-mongoengine-0.5.0/pylint_mongoengine.egg-info/PKG-INFO
+-rw-rw-r--   0 juca      (1001) juca      (1001)      429 2023-04-24 10:13:45.000000 pylint-mongoengine-0.5.0/pylint_mongoengine.egg-info/SOURCES.txt
+-rw-rw-r--   0 juca      (1001) juca      (1001)        1 2023-04-24 10:13:45.000000 pylint-mongoengine-0.5.0/pylint_mongoengine.egg-info/dependency_links.txt
+-rw-rw-r--   0 juca      (1001) juca      (1001)       39 2023-04-24 10:13:45.000000 pylint-mongoengine-0.5.0/pylint_mongoengine.egg-info/requires.txt
+-rw-rw-r--   0 juca      (1001) juca      (1001)       57 2023-04-24 10:13:45.000000 pylint-mongoengine-0.5.0/pylint_mongoengine.egg-info/top_level.txt
+-rw-rw-r--   0 juca      (1001) juca      (1001)      684 2023-04-24 10:02:41.000000 pylint-mongoengine-0.5.0/pyproject.toml
+-rw-rw-r--   0 juca      (1001) juca      (1001)       38 2023-04-24 10:13:45.323529 pylint-mongoengine-0.5.0/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pylint-mongoengine-0.4.0/pylint_mongoengine/__init__.py` & `pylint-mongoengine-0.5.0/pylint_mongoengine/__init__.py`

 * *Files identical despite different names*

### Comparing `pylint-mongoengine-0.4.0/pylint_mongoengine/checkers/mongoengine.py` & `pylint-mongoengine-0.5.0/pylint_mongoengine/checkers/mongoengine.py`

 * *Files identical despite different names*

### Comparing `pylint-mongoengine-0.4.0/pylint_mongoengine/suppression.py` & `pylint-mongoengine-0.5.0/pylint_mongoengine/suppression.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # You should have received a copy of the GNU General Public License
 # along with pylint-mongoengine. If not, see <http://www.gnu.org/licenses/>.
 
 from astroid.exceptions import InferenceError
 from pylint.checkers.typecheck import TypeChecker, IterableChecker
 from pylint.checkers.utils import safe_infer
 from pylint_plugin_utils import suppress_message
-from pylint_mongoengine.utils import (name_is_from_qs, is_field_method,
+from pylint_mongoengine.utils import (name_is_from_qs,
                                       node_is_embedded_doc,
                                       node_is_embedded_doc_attr,
                                       node_is_complex_field,
                                       node_is_document,
                                       name_is_from_model,
                                       node_is_default_qs,
                                       name_is_doc_callable)
@@ -136,16 +136,14 @@
                      _is_call2custom_manager)
     suppress_message(linter, TypeChecker.visit_attribute, 'no-member',
                      _is_custom_manager_attribute)
 
 
 def suppress_fields_attrs_messages(linter):
     suppress_message(linter, TypeChecker.visit_attribute, 'no-member',
-                     is_field_method)
-    suppress_message(linter, TypeChecker.visit_attribute, 'no-member',
                      _is_embedded_doc_attr)
 
 
 def suppress_fields_messages(linter):
     suppress_message(linter, IterableChecker.visit_for,
                      'not-an-iterable', _is_complex_field_for)
```

### Comparing `pylint-mongoengine-0.4.0/pylint_mongoengine/utils.py` & `pylint-mongoengine-0.5.0/pylint_mongoengine/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -108,37 +108,21 @@
 def node_is_default_qs(node):
     # the default qs manager is called 'objects', we check for it here
     attrname = getattr(node, 'attrname', None)
     if attrname != 'objects':
         return False
 
     base_cls = node.last_child()
-    for cls in base_cls.inferred():
-        if node_is_document(cls):
-            return True
-
-    return False
-
-
-def is_field_method(node):
-    """Checks if a call to a field instance method is valid. A call is
-    valid if the call is a method of the underlying type. So, in a StringField
-    the methods from str are valid, in a ListField the methods from list are
-    valid and so on..."""
-    name = node.attrname
-    parent = node.last_child()
-    inferred = safe_infer(parent)
-
-    if not inferred:
+    try:
+        for cls in base_cls.inferred():
+            if node_is_document(cls):
+                return True
+    except InferenceError:
         return False
 
-    for cls_name, inst in FIELD_TYPES.items():
-        if node_is_instance(inferred, cls_name) and hasattr(inst, name):
-            return True
-
     return False
 
 
 def get_node_parent_class(node):
     """Supposes that node is a mongoengine field in a class and tries to
     get its parent class"""
```


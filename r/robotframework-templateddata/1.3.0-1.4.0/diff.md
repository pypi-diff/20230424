# Comparing `tmp/robotframework-templateddata-1.3.0.tar.gz` & `tmp/robotframework-templateddata-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-templateddata-1.3.0.tar", last modified: Fri Mar  4 11:23:27 2022, max compression
+gzip compressed data, was "robotframework-templateddata-1.4.0.tar", last modified: Mon Apr 24 18:24:46 2023, max compression
```

## Comparing `robotframework-templateddata-1.3.0.tar` & `robotframework-templateddata-1.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 11:23:27.278876 robotframework-templateddata-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-03-04 11:23:17.000000 robotframework-templateddata-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2772 2022-03-04 11:23:27.278876 robotframework-templateddata-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1992 2022-03-04 11:23:17.000000 robotframework-templateddata-1.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 11:23:27.278876 robotframework-templateddata-1.3.0/TemplatedData/
--rw-r--r--   0 runner    (1001) docker     (121)     5374 2022-03-04 11:23:17.000000 robotframework-templateddata-1.3.0/TemplatedData/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-03-04 11:23:17.000000 robotframework-templateddata-1.3.0/TemplatedData/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-04 11:23:27.278876 robotframework-templateddata-1.3.0/robotframework_templateddata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2772 2022-03-04 11:23:27.000000 robotframework-templateddata-1.3.0/robotframework_templateddata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-03-04 11:23:27.000000 robotframework-templateddata-1.3.0/robotframework_templateddata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-04 11:23:27.000000 robotframework-templateddata-1.3.0/robotframework_templateddata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-03-04 11:23:27.000000 robotframework-templateddata-1.3.0/robotframework_templateddata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-03-04 11:23:27.000000 robotframework-templateddata-1.3.0/robotframework_templateddata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-04 11:23:27.278876 robotframework-templateddata-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1107 2022-03-04 11:23:17.000000 robotframework-templateddata-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:24:46.526337 robotframework-templateddata-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-24 18:24:34.000000 robotframework-templateddata-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-04-24 18:24:46.526337 robotframework-templateddata-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-04-24 18:24:34.000000 robotframework-templateddata-1.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:24:46.526337 robotframework-templateddata-1.4.0/TemplatedData/
+-rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-04-24 18:24:34.000000 robotframework-templateddata-1.4.0/TemplatedData/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-24 18:24:34.000000 robotframework-templateddata-1.4.0/TemplatedData/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:24:46.526337 robotframework-templateddata-1.4.0/robotframework_templateddata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-04-24 18:24:46.000000 robotframework-templateddata-1.4.0/robotframework_templateddata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-24 18:24:46.000000 robotframework-templateddata-1.4.0/robotframework_templateddata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 18:24:46.000000 robotframework-templateddata-1.4.0/robotframework_templateddata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-24 18:24:46.000000 robotframework-templateddata-1.4.0/robotframework_templateddata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-24 18:24:46.000000 robotframework-templateddata-1.4.0/robotframework_templateddata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 18:24:46.526337 robotframework-templateddata-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-24 18:24:34.000000 robotframework-templateddata-1.4.0/setup.py
```

### Comparing `robotframework-templateddata-1.3.0/LICENSE` & `robotframework-templateddata-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-templateddata-1.3.0/README.rst` & `robotframework-templateddata-1.4.0/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -39,14 +39,17 @@
 
 Robot code::
 
     ${var}     Set Variable    ${10}
     ${data}    Get Templated Data From Path    test_data.txt
     Log    ${data} # it should print `my variable is 10`
 
+Default values
+~~~~~~~~~~~~~~~~~~
+
 If the variable is not found it will be replaced with empty string. You can override that behaviour::
 
     ${data}    Get Templated Data From Path    test_data.txt    default_empty=${5}
     Log    ${data} # it should print `my variable is 5`
 
 You can also set default value of variable with `:` symbol.
 
@@ -56,23 +59,85 @@
 
 Robot code::
 
     ${var}     Set Variable    ${10}
     ${data}    Get Templated Data From Path    test_data.txt
     Log    ${data} # it should print `my variable is 10 and some string`
 
+Return value type
+~~~~~~~~~~~~~~~~~~
+
 Return value can be either text/string (default) or json.
 
 Test data::
 
     { "key": "${var}" }
 
 Robot code::
 
     ${data}    Get Templated Data From Path    test_data.txt    var=value    return_type=json
     Log    ${data} # it should print `{ "key": "value" }` and ${data} will be of type json
    
+Jinja templating
+~~~~~~~~~~~~~~~~~~
+
+TemplatedData can also render the Jinja templates using Robot Framework variables. To enable Jinja template pass ``jinja_template`` as argument to 
+library import or method call::
+
+    *** Settings ***
+   Library    TemplatedData  jinja_template=${True}
+   
+   OR
+   
+   *** Keywords ***
+   Load Data
+       ${data}    Get Templated Data From Path    data.template    jinja_template=${True}
+
+Test data (Jinja template)::
+
+   {
+       "accounts": [
+           { "id": {{ ${account_id:5} }} },
+           { "id2": "{{ ${account_id2} }}" }
+           ],
+       "users": [
+   {%- for user, amount in ${users.items()} %}
+         {
+           "name": "{{ user }}",
+           "amount": {{ amount }}
+         }{{ "," if not loop.last }}
+   {%- endfor %}
+       ]
+   }
+
+Robot code::
+ 
+    ${data}    Get Templated Data From Path    data.template    jinja_template=${True}
+    
+Example data output::
+ 
+    {
+       "accounts": [
+           { "id": 10 },
+           { "id2": "10" }
+           ],
+       "users": [
+         {
+           "name": "bartek",
+           "amount": 5
+         },
+         {
+           "name": "tymoteusz",
+           "amount": 10
+         },
+         {
+           "name": "pawel",
+           "amount": -1
+         }
+       ]
+   }
+
 .. Badges links
 
 .. |License|
    image:: https://img.shields.io/pypi/l/robotframework-robocop
    :alt: PyPI - License
```

### Comparing `robotframework-templateddata-1.3.0/TemplatedData/__init__.py` & `robotframework-templateddata-1.4.0/TemplatedData/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 
-from jinja2 import Environment, BaseLoader
+from jinja2 import Environment, BaseLoader, select_autoescape
 from robot.api import logger
 from robot.errors import VariableError
 from robot.libraries.BuiltIn import BuiltIn
 
 
 class TemplatedData:
     def __init__(
@@ -30,15 +30,15 @@
         ignore_missing = kwargs.pop("ignore_missing", self.ignore_missing)
         logger.debug(f"Template:\n{template}")
         overwrite_values = {self.normalize(arg): value for arg, value in kwargs.items()}
         templated_vars = {}
         elements = _search_variables(template, default_empty, ignore_missing)
         template = resolve(elements, overwrite_values, jinja_template, templated_vars)
         if jinja_template:
-            r_template = Environment(loader=BaseLoader()).from_string(template)
+            r_template = Environment(loader=BaseLoader(), autoescape=select_autoescape(['html', 'htm', 'xml'])).from_string(template)
             replaced_data = r_template.render(templated_vars=templated_vars)
         else:
             replaced_data = template
         logger.debug(f"Rendered template:\n{replaced_data}")
         return self.return_data_with_type(replaced_data, return_type)
 
     def get_templated_data_from_path(self, path, encoding="utf-8", **kwargs):
```

### Comparing `robotframework-templateddata-1.3.0/setup.py` & `robotframework-templateddata-1.4.0/setup.py`

 * *Files identical despite different names*


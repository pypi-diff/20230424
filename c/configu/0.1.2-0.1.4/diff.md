# Comparing `tmp/configu-0.1.2.tar.gz` & `tmp/configu-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configu-0.1.2.tar", max compression
+gzip compressed data, was "configu-0.1.4.tar", max compression
```

## Comparing `configu-0.1.2.tar` & `configu-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      680 2023-04-03 16:06:01.107296 configu-0.1.2/README.md
--rw-r--r--   0        0        0      555 2023-04-03 16:06:01.107296 configu-0.1.2/configu/__init__.py
--rw-r--r--   0        0        0      123 2023-04-03 16:06:01.107296 configu-0.1.2/configu/commands/__init__.py
--rw-r--r--   0        0        0    13861 2023-04-03 16:06:01.107296 configu-0.1.2/configu/commands/eval_command.py
--rw-r--r--   0        0        0     2695 2023-04-03 16:06:01.107296 configu-0.1.2/configu/commands/upsert_command.py
--rw-r--r--   0        0        0      423 2023-04-03 16:06:01.107296 configu-0.1.2/configu/core/__init__.py
--rw-r--r--   0        0        0      354 2023-04-03 16:06:01.107296 configu-0.1.2/configu/core/command.py
--rw-r--r--   0        0        0     6442 2023-04-03 16:06:01.107296 configu-0.1.2/configu/core/config_schema.py
--rw-r--r--   0        0        0     1383 2023-04-03 16:06:01.107296 configu-0.1.2/configu/core/config_set.py
--rw-r--r--   0        0        0      457 2023-04-03 16:06:01.107296 configu-0.1.2/configu/core/config_store.py
--rw-r--r--   0        0        0    11311 2023-04-03 16:06:26.311746 configu-0.1.2/configu/core/generated.py
--rw-r--r--   0        0        0      187 2023-04-03 16:06:01.107296 configu-0.1.2/configu/stores/__init__.py
--rw-r--r--   0        0        0     2507 2023-04-03 16:06:01.107296 configu-0.1.2/configu/stores/configu_store.py
--rw-r--r--   0        0        0     1320 2023-04-03 16:06:01.107296 configu-0.1.2/configu/stores/in_memory_store.py
--rw-r--r--   0        0        0     2482 2023-04-03 16:06:01.107296 configu-0.1.2/configu/stores/json_file_store.py
--rw-r--r--   0        0        0     1234 2023-04-03 16:06:01.107296 configu-0.1.2/configu/utils.py
--rw-r--r--   0        0        0     1807 2023-04-03 16:06:39.959981 configu-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1823 1970-01-01 00:00:00.000000 configu-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      759 2023-04-24 16:42:15.764914 configu-0.1.4/README.md
+-rw-r--r--   0        0        0      555 2023-04-24 16:42:15.764914 configu-0.1.4/configu/__init__.py
+-rw-r--r--   0        0        0      123 2023-04-24 16:42:15.764914 configu-0.1.4/configu/commands/__init__.py
+-rw-r--r--   0        0        0    13948 2023-04-24 16:42:15.764914 configu-0.1.4/configu/commands/eval_command.py
+-rw-r--r--   0        0        0     2695 2023-04-24 16:42:15.764914 configu-0.1.4/configu/commands/upsert_command.py
+-rw-r--r--   0        0        0      423 2023-04-24 16:42:15.764914 configu-0.1.4/configu/core/__init__.py
+-rw-r--r--   0        0        0      354 2023-04-24 16:42:15.764914 configu-0.1.4/configu/core/command.py
+-rw-r--r--   0        0        0     6442 2023-04-24 16:42:15.764914 configu-0.1.4/configu/core/config_schema.py
+-rw-r--r--   0        0        0     1383 2023-04-24 16:42:15.764914 configu-0.1.4/configu/core/config_set.py
+-rw-r--r--   0        0        0      457 2023-04-24 16:42:15.764914 configu-0.1.4/configu/core/config_store.py
+-rw-r--r--   0        0        0    11311 2023-04-24 16:42:45.559380 configu-0.1.4/configu/core/generated.py
+-rw-r--r--   0        0        0      187 2023-04-24 16:42:15.764914 configu-0.1.4/configu/stores/__init__.py
+-rw-r--r--   0        0        0     2507 2023-04-24 16:42:15.764914 configu-0.1.4/configu/stores/configu_store.py
+-rw-r--r--   0        0        0     1320 2023-04-24 16:42:15.764914 configu-0.1.4/configu/stores/in_memory_store.py
+-rw-r--r--   0        0        0     2482 2023-04-24 16:42:15.764914 configu-0.1.4/configu/stores/json_file_store.py
+-rw-r--r--   0        0        0     1234 2023-04-24 16:42:15.764914 configu-0.1.4/configu/utils.py
+-rw-r--r--   0        0        0     1815 2023-04-24 16:43:09.861249 configu-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1914 1970-01-01 00:00:00.000000 configu-0.1.4/PKG-INFO
```

### Comparing `configu-0.1.2/configu/__init__.py` & `configu-0.1.4/configu/__init__.py`

 * *Files identical despite different names*

### Comparing `configu-0.1.2/configu/commands/eval_command.py` & `configu-0.1.4/configu/commands/eval_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -322,35 +322,35 @@
             {
                 key: scope
                 for key, scope in eval_scope.items()
                 if scope.result.from_.source == "schema-template"
             }.keys()
         )
 
-        render_context = {
-            key: value.result.value for key, value in eval_scope.items()
-        }
-
         run_again = True
         while len(template_keys) > 0 and run_again:
             has_rendered = False
+            render_context = {
+                key: value.result.value for key, value in eval_scope.items()
+            }
             for key in deepcopy(template_keys):
                 current: ConfigEvalScope = eval_scope[key]
                 template: str = current.cfgu.template
                 expressions = parse_template(template)
                 if any([True for exp in expressions if exp in template_keys]):
                     continue
 
                 eval_scope[key].result.value = render_template(
                     template,
                     {
                         **render_context,
                         **{
                             "CONFIGU_SET": {
                                 "path": current.context.set.path,
+                                "hierarchy": current.context.set.hierarchy,
                                 "first": current.context.set.hierarchy[0],
                                 "last": current.context.set.hierarchy[-1],
                                 **{
                                     str(index): path
                                     for index, path in enumerate(
                                         current.context.set.hierarchy
                                     )
```

### Comparing `configu-0.1.2/configu/commands/upsert_command.py` & `configu-0.1.4/configu/commands/upsert_command.py`

 * *Files identical despite different names*

### Comparing `configu-0.1.2/configu/core/config_schema.py` & `configu-0.1.4/configu/core/config_schema.py`

 * *Files identical despite different names*

### Comparing `configu-0.1.2/configu/core/config_set.py` & `configu-0.1.4/configu/core/config_set.py`

 * *Files identical despite different names*

### Comparing `configu-0.1.2/configu/core/generated.py` & `configu-0.1.4/configu/core/generated.py`

 * *Files identical despite different names*

### Comparing `configu-0.1.2/configu/stores/configu_store.py` & `configu-0.1.4/configu/stores/configu_store.py`

 * *Files identical despite different names*

### Comparing `configu-0.1.2/configu/stores/in_memory_store.py` & `configu-0.1.4/configu/stores/in_memory_store.py`

 * *Files identical despite different names*

### Comparing `configu-0.1.2/configu/stores/json_file_store.py` & `configu-0.1.4/configu/stores/json_file_store.py`

 * *Files identical despite different names*

### Comparing `configu-0.1.2/configu/utils.py` & `configu-0.1.4/configu/utils.py`

 * *Files identical despite different names*

### Comparing `configu-0.1.2/pyproject.toml` & `configu-0.1.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configu"
-version = "0.1.2"
+version = "0.1.4"
 description = "Configu Python SDK"
 authors = ["Configu <info@configu.com>"]
 maintainers = [
   "Ron Roditi <ron@configu.com>",
   "Or Levi <orlevi128@gmail.com>"
 ]
 license = "Apache-2.0"
@@ -16,15 +16,15 @@
   "cfgu",
   "configu",
   "configu-sdk",
   "configu-python-sdk"
 ]
 # https://pypi.org/classifiers/
 classifiers = [
-  "Development Status :: 3 - Alpha", # Development Status :: 5 - Production/Stable after CR
+  "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3 :: Only",
   "Topic :: Software Development"
 ]
 packages = [{ include = "configu" }]
 
@@ -34,14 +34,15 @@
 py-validator = "^0.17.0"
 pydantic = "^1.10.6"
 chevron = "^0.14.0"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0" # configs at .flake8
 black = { extras = ["d"], version = "^23.1.0" }
+pdoc = "^13.1.0" # https://pdoc.dev/docs/pdoc.html
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 
 # https://black.readthedocs.io/en/stable/usage_and_configuration/the_basics.html#
 [tool.black]
```

### Comparing `configu-0.1.2/PKG-INFO` & `configu-0.1.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: configu
-Version: 0.1.2
+Version: 0.1.4
 Summary: Configu Python SDK
 Home-page: https://configu.com/
 License: Apache-2.0
 Keywords: cfgu,configu,configu-sdk,configu-python-sdk
 Author: Configu
 Author-email: info@configu.com
 Maintainer: Ron Roditi
 Maintainer-email: ron@configu.com
 Requires-Python: >=3.9,<3.12
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -26,48 +26,51 @@
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Project-URL: Documentation, https://configu.com/docs/
 Project-URL: Repository, https://github.com/configu/configu
 Description-Content-Type: text/markdown
 
 # @configu/py
 
+> configu python sdk
+
 ## Install
 
 ```bash
 pip install configu
 ```
 
 ## Usage
 See example in the examples folder
 
 ## CONTRIBUTING
 
 ### Requirements
 
 1. Follow the instructions on the main [CONTRIBUTING.md](https://github.com/configu/configu/blob/main/CONTRIBUTING.md)
-   to set up node and npm. This is necessary for lint-staged workflow
-2. Install [pyenv](https://github.com/pyenv/pyenv)
-3. Install [poetry](https://python-poetry.org/)
+   to set up node and npm. This is necessary for lint-staged workflow.
+2. Install [pyenv](https://github.com/pyenv/pyenv) | [Homebrew](https://formulae.brew.sh/formula/pyenv)
+3. Install [poetry](https://python-poetry.org/) | [Homebrew](https://formulae.brew.sh/formula/poetry)
 
 ### Setup
 
->  <span style="color:#FF392B">**Make sure you're in configu/py directory**</span>
-
 #### Run these commands in order
 
+```bash
+cd py
+```
 
 ```bash
 pyenv install
 ```
 
 ```bash
 pyenv local 3.9.16
 ```
 
 ```bash
-poetry env use python
+poetry env use $(pyenv which python)
 ```
 
 ```bash
 poetry install
 ```
```


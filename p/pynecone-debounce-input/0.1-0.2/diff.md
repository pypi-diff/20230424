# Comparing `tmp/pynecone-debounce-input-0.1.tar.gz` & `tmp/pynecone-debounce-input-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynecone-debounce-input-0.1.tar", last modified: Sat Apr 22 15:41:44 2023, max compression
+gzip compressed data, was "pynecone-debounce-input-0.2.tar", last modified: Mon Apr 24 18:31:26 2023, max compression
```

## Comparing `pynecone-debounce-input-0.1.tar` & `pynecone-debounce-input-0.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:41:44.395717 pynecone-debounce-input-0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:41:44.387717 pynecone-debounce-input-0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:41:44.391717 pynecone-debounce-input-0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-22 15:40:48.000000 pynecone-debounce-input-0.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-22 15:40:48.000000 pynecone-debounce-input-0.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-22 15:40:48.000000 pynecone-debounce-input-0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-22 15:40:48.000000 pynecone-debounce-input-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-04-22 15:41:44.395717 pynecone-debounce-input-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-04-22 15:40:48.000000 pynecone-debounce-input-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:41:44.391717 pynecone-debounce-input-0.1/example/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-22 15:40:48.000000 pynecone-debounce-input-0.1/example/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:41:44.391717 pynecone-debounce-input-0.1/example/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-04-22 15:40:48.000000 pynecone-debounce-input-0.1/example/assets/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:41:44.391717 pynecone-debounce-input-0.1/example/example/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 15:40:48.000000 pynecone-debounce-input-0.1/example/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-22 15:40:48.000000 pynecone-debounce-input-0.1/example/example/example.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-22 15:40:48.000000 pynecone-debounce-input-0.1/example/pcconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-22 15:40:48.000000 pynecone-debounce-input-0.1/example/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-22 15:40:48.000000 pynecone-debounce-input-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 15:41:44.395717 pynecone-debounce-input-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-22 15:40:48.000000 pynecone-debounce-input-0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:41:44.391717 pynecone-debounce-input-0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:41:44.395717 pynecone-debounce-input-0.1/src/pynecone_debounce_input.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-04-22 15:41:44.000000 pynecone-debounce-input-0.1/src/pynecone_debounce_input.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-22 15:41:44.000000 pynecone-debounce-input-0.1/src/pynecone_debounce_input.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 15:41:44.000000 pynecone-debounce-input-0.1/src/pynecone_debounce_input.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-22 15:41:44.000000 pynecone-debounce-input-0.1/src/pynecone_debounce_input.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-22 15:41:44.000000 pynecone-debounce-input-0.1/src/pynecone_debounce_input.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-22 15:40:48.000000 pynecone-debounce-input-0.1/src/pynecone_debounce_input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 15:41:44.395717 pynecone-debounce-input-0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-22 15:40:48.000000 pynecone-debounce-input-0.1/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-22 15:40:48.000000 pynecone-debounce-input-0.1/tests/test_render.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-22 15:40:48.000000 pynecone-debounce-input-0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:31:26.433489 pynecone-debounce-input-0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:31:26.429489 pynecone-debounce-input-0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:31:26.429489 pynecone-debounce-input-0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-24 18:30:42.000000 pynecone-debounce-input-0.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-24 18:30:42.000000 pynecone-debounce-input-0.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-24 18:30:42.000000 pynecone-debounce-input-0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-24 18:30:42.000000 pynecone-debounce-input-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-04-24 18:31:26.433489 pynecone-debounce-input-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-04-24 18:30:42.000000 pynecone-debounce-input-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:31:26.429489 pynecone-debounce-input-0.2/example/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-24 18:30:42.000000 pynecone-debounce-input-0.2/example/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:31:26.429489 pynecone-debounce-input-0.2/example/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-04-24 18:30:42.000000 pynecone-debounce-input-0.2/example/assets/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:31:26.429489 pynecone-debounce-input-0.2/example/example/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 18:30:42.000000 pynecone-debounce-input-0.2/example/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-24 18:30:42.000000 pynecone-debounce-input-0.2/example/example/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-24 18:30:42.000000 pynecone-debounce-input-0.2/example/pcconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-24 18:30:42.000000 pynecone-debounce-input-0.2/example/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-24 18:30:42.000000 pynecone-debounce-input-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 18:31:26.433489 pynecone-debounce-input-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-24 18:30:42.000000 pynecone-debounce-input-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:31:26.429489 pynecone-debounce-input-0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:31:26.433489 pynecone-debounce-input-0.2/src/pynecone_debounce_input.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-04-24 18:31:26.000000 pynecone-debounce-input-0.2/src/pynecone_debounce_input.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-24 18:31:26.000000 pynecone-debounce-input-0.2/src/pynecone_debounce_input.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 18:31:26.000000 pynecone-debounce-input-0.2/src/pynecone_debounce_input.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-24 18:31:26.000000 pynecone-debounce-input-0.2/src/pynecone_debounce_input.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-24 18:31:26.000000 pynecone-debounce-input-0.2/src/pynecone_debounce_input.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-24 18:30:42.000000 pynecone-debounce-input-0.2/src/pynecone_debounce_input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:31:26.433489 pynecone-debounce-input-0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-24 18:30:42.000000 pynecone-debounce-input-0.2/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-24 18:30:42.000000 pynecone-debounce-input-0.2/tests/test_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-24 18:30:42.000000 pynecone-debounce-input-0.2/tox.ini
```

### Comparing `pynecone-debounce-input-0.1/.github/workflows/publish.yml` & `pynecone-debounce-input-0.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pynecone-debounce-input-0.1/.github/workflows/test.yml` & `pynecone-debounce-input-0.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pynecone-debounce-input-0.1/LICENSE` & `pynecone-debounce-input-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pynecone-debounce-input-0.1/PKG-INFO` & `pynecone-debounce-input-0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynecone-debounce-input
-Version: 0.1
+Version: 0.2
 Summary: Pynecone full-stack framework wrapper around react-debounce-input
 Author-email: Masen Furer <m_github@0x26.net>
 License: MIT License
         
         Copyright (c) 2023 Masen Furer
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -72,15 +72,15 @@
 
 @app.add_page
 def index():
     return pc.center(
         pc.hstack(
             debounce_input(
                 pc.input(
-                    placeholder="Query"
+                    placeholder="Query",
                     value=State.query,
                     on_change=State.set_query,
                 ),
             ),
             pc.text(State.query),
         )
     )
@@ -132,10 +132,16 @@
 
 #### `force_notify_on_blur: bool = True`
 
 Same as `force_notify_by_enter`, but notification will be sent when focus leaves the input field.
 
 ## Changelog
 
+### v0.2 - 2023-04-24
+
+* `import pynecone_debounce_input` automatically adds `react-debounce-input` to `Config.frontend_packages`
+* fix example in README, missing comma
+* improve test assertions when exporting example project
+
 ### v0.1 - 2023-04-21
 
 Initial Release
```

### Comparing `pynecone-debounce-input-0.1/README.md` & `pynecone-debounce-input-0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 @app.add_page
 def index():
     return pc.center(
         pc.hstack(
             debounce_input(
                 pc.input(
-                    placeholder="Query"
+                    placeholder="Query",
                     value=State.query,
                     on_change=State.set_query,
                 ),
             ),
             pc.text(State.query),
         )
     )
@@ -85,10 +85,16 @@
 
 #### `force_notify_on_blur: bool = True`
 
 Same as `force_notify_by_enter`, but notification will be sent when focus leaves the input field.
 
 ## Changelog
 
+### v0.2 - 2023-04-24
+
+* `import pynecone_debounce_input` automatically adds `react-debounce-input` to `Config.frontend_packages`
+* fix example in README, missing comma
+* improve test assertions when exporting example project
+
 ### v0.1 - 2023-04-21
 
 Initial Release
```

### Comparing `pynecone-debounce-input-0.1/example/assets/favicon.ico` & `pynecone-debounce-input-0.2/example/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `pynecone-debounce-input-0.1/example/example/example.py` & `pynecone-debounce-input-0.2/example/example/example.py`

 * *Files identical despite different names*

### Comparing `pynecone-debounce-input-0.1/pyproject.toml` & `pynecone-debounce-input-0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynecone-debounce-input-0.1/src/pynecone_debounce_input.egg-info/PKG-INFO` & `pynecone-debounce-input-0.2/src/pynecone_debounce_input.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynecone-debounce-input
-Version: 0.1
+Version: 0.2
 Summary: Pynecone full-stack framework wrapper around react-debounce-input
 Author-email: Masen Furer <m_github@0x26.net>
 License: MIT License
         
         Copyright (c) 2023 Masen Furer
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -72,15 +72,15 @@
 
 @app.add_page
 def index():
     return pc.center(
         pc.hstack(
             debounce_input(
                 pc.input(
-                    placeholder="Query"
+                    placeholder="Query",
                     value=State.query,
                     on_change=State.set_query,
                 ),
             ),
             pc.text(State.query),
         )
     )
@@ -132,10 +132,16 @@
 
 #### `force_notify_on_blur: bool = True`
 
 Same as `force_notify_by_enter`, but notification will be sent when focus leaves the input field.
 
 ## Changelog
 
+### v0.2 - 2023-04-24
+
+* `import pynecone_debounce_input` automatically adds `react-debounce-input` to `Config.frontend_packages`
+* fix example in README, missing comma
+* improve test assertions when exporting example project
+
 ### v0.1 - 2023-04-21
 
 Initial Release
```

### Comparing `pynecone-debounce-input-0.1/src/pynecone_debounce_input.egg-info/SOURCES.txt` & `pynecone-debounce-input-0.2/src/pynecone_debounce_input.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynecone-debounce-input-0.1/tests/test_render.py` & `pynecone-debounce-input-0.2/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `pynecone-debounce-input-0.1/tox.ini` & `pynecone-debounce-input-0.2/tox.ini`

 * *Files identical despite different names*


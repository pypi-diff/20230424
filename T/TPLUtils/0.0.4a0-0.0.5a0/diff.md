# Comparing `tmp/TPLUtils-0.0.4a-.tar.gz` & `tmp/TPLUtils-0.0.5a-.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TPLUtils-0.0.4a-.tar", last modified: Mon Apr 24 00:43:25 2023, max compression
+gzip compressed data, was "TPLUtils-0.0.5a-.tar", last modified: Mon Apr 24 01:08:26 2023, max compression
```

## Comparing `TPLUtils-0.0.4a-.tar` & `TPLUtils-0.0.5a-.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:43:25.436811 TPLUtils-0.0.4a-/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-24 00:43:25.432811 TPLUtils-0.0.4a-/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-24 00:43:13.000000 TPLUtils-0.0.4a-/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 00:43:25.436811 TPLUtils-0.0.4a-/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-24 00:43:13.000000 TPLUtils-0.0.4a-/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:43:25.432811 TPLUtils-0.0.4a-/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:43:25.432811 TPLUtils-0.0.4a-/src/TPL/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 00:43:13.000000 TPLUtils-0.0.4a-/src/TPL/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:43:25.432811 TPLUtils-0.0.4a-/src/TPL/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 00:43:13.000000 TPLUtils-0.0.4a-/src/TPL/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-24 00:43:13.000000 TPLUtils-0.0.4a-/src/TPL/db/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-24 00:43:13.000000 TPLUtils-0.0.4a-/src/TPL/db/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-24 00:43:13.000000 TPLUtils-0.0.4a-/src/TPL/db/website.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:43:25.432811 TPLUtils-0.0.4a-/src/TPL/utility/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 00:43:13.000000 TPLUtils-0.0.4a-/src/TPL/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-24 00:43:13.000000 TPLUtils-0.0.4a-/src/TPL/utility/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-24 00:43:13.000000 TPLUtils-0.0.4a-/src/TPL/utility/security.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 00:43:25.432811 TPLUtils-0.0.4a-/src/TPLUtils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-24 00:43:25.000000 TPLUtils-0.0.4a-/src/TPLUtils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-24 00:43:25.000000 TPLUtils-0.0.4a-/src/TPLUtils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 00:43:25.000000 TPLUtils-0.0.4a-/src/TPLUtils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-24 00:43:25.000000 TPLUtils-0.0.4a-/src/TPLUtils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-24 00:43:25.000000 TPLUtils-0.0.4a-/src/TPLUtils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:08:26.640181 TPLUtils-0.0.5a-/
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-04-24 01:08:26.640181 TPLUtils-0.0.5a-/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-04-24 01:08:11.000000 TPLUtils-0.0.5a-/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 01:08:26.640181 TPLUtils-0.0.5a-/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-24 01:08:11.000000 TPLUtils-0.0.5a-/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:08:26.636181 TPLUtils-0.0.5a-/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:08:26.636181 TPLUtils-0.0.5a-/src/TPL/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:08:11.000000 TPLUtils-0.0.5a-/src/TPL/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:08:26.640181 TPLUtils-0.0.5a-/src/TPL/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:08:11.000000 TPLUtils-0.0.5a-/src/TPL/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-24 01:08:11.000000 TPLUtils-0.0.5a-/src/TPL/db/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-24 01:08:11.000000 TPLUtils-0.0.5a-/src/TPL/db/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-24 01:08:11.000000 TPLUtils-0.0.5a-/src/TPL/db/website.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:08:26.640181 TPLUtils-0.0.5a-/src/TPL/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:08:11.000000 TPLUtils-0.0.5a-/src/TPL/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-24 01:08:11.000000 TPLUtils-0.0.5a-/src/TPL/utility/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-24 01:08:11.000000 TPLUtils-0.0.5a-/src/TPL/utility/security.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:08:26.640181 TPLUtils-0.0.5a-/src/TPLUtils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-04-24 01:08:26.000000 TPLUtils-0.0.5a-/src/TPLUtils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-24 01:08:26.000000 TPLUtils-0.0.5a-/src/TPLUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 01:08:26.000000 TPLUtils-0.0.5a-/src/TPLUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-24 01:08:26.000000 TPLUtils-0.0.5a-/src/TPLUtils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-24 01:08:26.000000 TPLUtils-0.0.5a-/src/TPLUtils.egg-info/top_level.txt
```

### Comparing `TPLUtils-0.0.4a-/setup.py` & `TPLUtils-0.0.5a-/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
     
 setup(
     name="TPLUtils",
-    version="0.0.4a'",
+    version="0.0.5a'",
     packages=find_packages(where="src"),
     description='A package used for the TPL project',
     license='MIT',
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         "fastapi",
```

### Comparing `TPLUtils-0.0.4a-/src/TPL/db/config.py` & `TPLUtils-0.0.5a-/src/TPL/db/config.py`

 * *Files identical despite different names*

### Comparing `TPLUtils-0.0.4a-/src/TPL/db/user.py` & `TPLUtils-0.0.5a-/src/TPL/db/user.py`

 * *Files identical despite different names*

### Comparing `TPLUtils-0.0.4a-/src/TPL/db/website.py` & `TPLUtils-0.0.5a-/src/TPL/db/website.py`

 * *Files identical despite different names*

### Comparing `TPLUtils-0.0.4a-/src/TPL/utility/security.py` & `TPLUtils-0.0.5a-/src/TPL/utility/security.py`

 * *Files identical despite different names*


# Comparing `tmp/ez_yaml-1.3.0.tar.gz` & `tmp/ez_yaml-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez_yaml-1.3.0.tar", last modified: Sun Apr  9 03:55:54 2023, max compression
+gzip compressed data, was "ez_yaml-1.3.2.tar", last modified: Mon Apr 24 15:17:35 2023, max compression
```

## Comparing `ez_yaml-1.3.0.tar` & `ez_yaml-1.3.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-09 03:55:54.806225 ez_yaml-1.3.0/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      718 2023-04-09 03:55:54.806084 ez_yaml-1.3.0/PKG-INFO
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-09 03:55:54.805158 ez_yaml-1.3.0/ez_yaml/
--rw-r--r--   0 jeffhykin   (501) staff       (20)       30 2022-12-02 18:23:22.000000 ez_yaml-1.3.0/ez_yaml/__init__.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6984 2023-04-09 03:54:41.000000 ez_yaml-1.3.0/ez_yaml/ez_yaml.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-09 03:55:54.805880 ez_yaml-1.3.0/ez_yaml.egg-info/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      718 2023-04-09 03:55:54.000000 ez_yaml-1.3.0/ez_yaml.egg-info/PKG-INFO
--rw-r--r--   0 jeffhykin   (501) staff       (20)      171 2023-04-09 03:55:54.000000 ez_yaml-1.3.0/ez_yaml.egg-info/SOURCES.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-04-09 03:55:54.000000 ez_yaml-1.3.0/ez_yaml.egg-info/dependency_links.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)        8 2023-04-09 03:55:54.000000 ez_yaml-1.3.0/ez_yaml.egg-info/top_level.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-04-09 03:55:54.806269 ez_yaml-1.3.0/setup.cfg
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1158 2023-04-09 03:44:06.000000 ez_yaml-1.3.0/setup.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-24 15:17:35.146455 ez_yaml-1.3.2/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      718 2023-04-24 15:17:35.146309 ez_yaml-1.3.2/PKG-INFO
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-24 15:17:35.145440 ez_yaml-1.3.2/ez_yaml/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       30 2022-12-02 18:23:22.000000 ez_yaml-1.3.2/ez_yaml/__init__.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6984 2023-04-09 03:54:41.000000 ez_yaml-1.3.2/ez_yaml/ez_yaml.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-24 15:17:35.146140 ez_yaml-1.3.2/ez_yaml.egg-info/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      718 2023-04-24 15:17:34.000000 ez_yaml-1.3.2/ez_yaml.egg-info/PKG-INFO
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      171 2023-04-24 15:17:35.000000 ez_yaml-1.3.2/ez_yaml.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-04-24 15:17:34.000000 ez_yaml-1.3.2/ez_yaml.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        8 2023-04-24 15:17:35.000000 ez_yaml-1.3.2/ez_yaml.egg-info/top_level.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-04-24 15:17:35.146498 ez_yaml-1.3.2/setup.cfg
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1158 2023-04-09 03:44:06.000000 ez_yaml-1.3.2/setup.py
```

### Comparing `ez_yaml-1.3.0/PKG-INFO` & `ez_yaml-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez_yaml
-Version: 1.3.0
+Version: 1.3.2
 Summary: Straighforward wrapper around Ruamel Yaml
 Home-page: https://github.com/jeff-hykin/ez_yaml
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `ez_yaml-1.3.0/ez_yaml/ez_yaml.py` & `ez_yaml-1.3.2/ez_yaml/ez_yaml.py`

 * *Files identical despite different names*

### Comparing `ez_yaml-1.3.0/ez_yaml.egg-info/PKG-INFO` & `ez_yaml-1.3.2/ez_yaml.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez-yaml
-Version: 1.3.0
+Version: 1.3.2
 Summary: Straighforward wrapper around Ruamel Yaml
 Home-page: https://github.com/jeff-hykin/ez_yaml
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `ez_yaml-1.3.0/setup.py` & `ez_yaml-1.3.2/setup.py`

 * *Files identical despite different names*


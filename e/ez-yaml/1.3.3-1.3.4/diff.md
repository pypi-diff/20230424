# Comparing `tmp/ez_yaml-1.3.3.tar.gz` & `tmp/ez_yaml-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez_yaml-1.3.3.tar", last modified: Mon Apr 24 16:32:21 2023, max compression
+gzip compressed data, was "ez_yaml-1.3.4.tar", last modified: Mon Apr 24 16:37:14 2023, max compression
```

## Comparing `ez_yaml-1.3.3.tar` & `ez_yaml-1.3.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-24 16:32:21.809105 ez_yaml-1.3.3/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      718 2023-04-24 16:32:21.808964 ez_yaml-1.3.3/PKG-INFO
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-24 16:32:21.808058 ez_yaml-1.3.3/ez_yaml/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6984 2023-04-24 16:29:01.000000 ez_yaml-1.3.3/ez_yaml/__init__.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-24 16:32:21.808771 ez_yaml-1.3.3/ez_yaml.egg-info/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      718 2023-04-24 16:32:21.000000 ez_yaml-1.3.3/ez_yaml.egg-info/PKG-INFO
--rw-r--r--   0 jeffhykin   (501) staff       (20)      152 2023-04-24 16:32:21.000000 ez_yaml-1.3.3/ez_yaml.egg-info/SOURCES.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-04-24 16:32:21.000000 ez_yaml-1.3.3/ez_yaml.egg-info/dependency_links.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)        8 2023-04-24 16:32:21.000000 ez_yaml-1.3.3/ez_yaml.egg-info/top_level.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-04-24 16:32:21.809155 ez_yaml-1.3.3/setup.cfg
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1158 2023-04-09 03:44:06.000000 ez_yaml-1.3.3/setup.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-24 16:37:14.081274 ez_yaml-1.3.4/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      718 2023-04-24 16:37:14.081119 ez_yaml-1.3.4/PKG-INFO
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-24 16:37:14.080049 ez_yaml-1.3.4/ez_yaml/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6984 2023-04-24 16:29:01.000000 ez_yaml-1.3.4/ez_yaml/__init__.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-24 16:37:14.080934 ez_yaml-1.3.4/ez_yaml.egg-info/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      718 2023-04-24 16:37:13.000000 ez_yaml-1.3.4/ez_yaml.egg-info/PKG-INFO
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      152 2023-04-24 16:37:13.000000 ez_yaml-1.3.4/ez_yaml.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-04-24 16:37:13.000000 ez_yaml-1.3.4/ez_yaml.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        8 2023-04-24 16:37:13.000000 ez_yaml-1.3.4/ez_yaml.egg-info/top_level.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-04-24 16:37:14.081317 ez_yaml-1.3.4/setup.cfg
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1158 2023-04-09 03:44:06.000000 ez_yaml-1.3.4/setup.py
```

### Comparing `ez_yaml-1.3.3/PKG-INFO` & `ez_yaml-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez_yaml
-Version: 1.3.3
+Version: 1.3.4
 Summary: Straighforward wrapper around Ruamel Yaml
 Home-page: https://github.com/jeff-hykin/ez_yaml
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `ez_yaml-1.3.3/ez_yaml/__init__.py` & `ez_yaml-1.3.4/ez_yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `ez_yaml-1.3.3/ez_yaml.egg-info/PKG-INFO` & `ez_yaml-1.3.4/ez_yaml.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez-yaml
-Version: 1.3.3
+Version: 1.3.4
 Summary: Straighforward wrapper around Ruamel Yaml
 Home-page: https://github.com/jeff-hykin/ez_yaml
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `ez_yaml-1.3.3/setup.py` & `ez_yaml-1.3.4/setup.py`

 * *Files identical despite different names*


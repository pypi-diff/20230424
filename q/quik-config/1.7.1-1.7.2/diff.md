# Comparing `tmp/quik_config-1.7.1.tar.gz` & `tmp/quik_config-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quik_config-1.7.1.tar", last modified: Mon Apr 24 15:40:29 2023, max compression
+gzip compressed data, was "quik_config-1.7.2.tar", last modified: Mon Apr 24 16:30:56 2023, max compression
```

## Comparing `quik_config-1.7.1.tar` & `quik_config-1.7.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-24 15:40:29.298634 quik_config-1.7.1/
--rw-r--r--   0 jeffhykin   (501) staff       (20)    11766 2023-04-24 15:40:29.298454 quik_config-1.7.1/PKG-INFO
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-24 15:40:29.297783 quik_config-1.7.1/quik_config/
--rw-r--r--   0 jeffhykin   (501) staff       (20)    33411 2023-04-24 15:37:27.000000 quik_config-1.7.1/quik_config/__init__.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-24 15:40:29.298276 quik_config-1.7.1/quik_config.egg-info/
--rw-r--r--   0 jeffhykin   (501) staff       (20)    11766 2023-04-24 15:40:28.000000 quik_config-1.7.1/quik_config.egg-info/PKG-INFO
--rw-r--r--   0 jeffhykin   (501) staff       (20)      172 2023-04-24 15:40:29.000000 quik_config-1.7.1/quik_config.egg-info/SOURCES.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-04-24 15:40:29.000000 quik_config-1.7.1/quik_config.egg-info/dependency_links.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       12 2023-04-24 15:40:29.000000 quik_config-1.7.1/quik_config.egg-info/top_level.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-04-24 15:40:29.298680 quik_config-1.7.1/setup.cfg
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1232 2023-04-20 16:40:30.000000 quik_config-1.7.1/setup.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-24 16:30:56.689983 quik_config-1.7.2/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    11766 2023-04-24 16:30:56.689758 quik_config-1.7.2/PKG-INFO
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-24 16:30:56.688910 quik_config-1.7.2/quik_config/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    33411 2023-04-24 16:27:22.000000 quik_config-1.7.2/quik_config/__init__.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-24 16:30:56.689439 quik_config-1.7.2/quik_config.egg-info/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    11766 2023-04-24 16:30:56.000000 quik_config-1.7.2/quik_config.egg-info/PKG-INFO
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      172 2023-04-24 16:30:56.000000 quik_config-1.7.2/quik_config.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-04-24 16:30:56.000000 quik_config-1.7.2/quik_config.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       12 2023-04-24 16:30:56.000000 quik_config-1.7.2/quik_config.egg-info/top_level.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-04-24 16:30:56.690047 quik_config-1.7.2/setup.cfg
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1232 2023-04-20 16:40:30.000000 quik_config-1.7.2/setup.py
```

### Comparing `quik_config-1.7.1/PKG-INFO` & `quik_config-1.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quik_config
-Version: 1.7.1
+Version: 1.7.2
 Summary: Project config files
 Home-page: https://github.com/jeff-hykin/quik_config_python.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `quik_config-1.7.1/quik_config/__init__.py` & `quik_config-1.7.2/quik_config/__init__.py`

 * *Files identical despite different names*

### Comparing `quik_config-1.7.1/quik_config.egg-info/PKG-INFO` & `quik_config-1.7.2/quik_config.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quik-config
-Version: 1.7.1
+Version: 1.7.2
 Summary: Project config files
 Home-page: https://github.com/jeff-hykin/quik_config_python.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `quik_config-1.7.1/setup.py` & `quik_config-1.7.2/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/OpenAccess-0.1.0.tar.gz` & `tmp/OpenAccess-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenAccess-0.1.0.tar", last modified: Mon Apr 24 21:22:56 2023, max compression
+gzip compressed data, was "OpenAccess-0.1.1.tar", last modified: Mon Apr 24 21:25:40 2023, max compression
```

## Comparing `OpenAccess-0.1.0.tar` & `OpenAccess-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 jaiber    (1000) jaiber    (1000)        0 2023-04-24 21:22:56.441590 OpenAccess-0.1.0/
-drwxrwxr-x   0 jaiber    (1000) jaiber    (1000)        0 2023-04-24 21:22:56.437590 OpenAccess-0.1.0/OpenAccess/
--rw-r--r--   0 jaiber    (1000) jaiber    (1000)      105 2023-04-24 21:21:59.000000 OpenAccess-0.1.0/OpenAccess/__init__.py
--rw-r--r--   0 jaiber    (1000) jaiber    (1000)    10381 2023-04-24 21:17:53.000000 OpenAccess-0.1.0/OpenAccess/openaccess.py
-drwxrwxr-x   0 jaiber    (1000) jaiber    (1000)        0 2023-04-24 21:22:56.437590 OpenAccess-0.1.0/OpenAccess.egg-info/
--rw-r--r--   0 jaiber    (1000) jaiber    (1000)     1581 2023-04-24 21:22:56.000000 OpenAccess-0.1.0/OpenAccess.egg-info/PKG-INFO
--rw-r--r--   0 jaiber    (1000) jaiber    (1000)      235 2023-04-24 21:22:56.000000 OpenAccess-0.1.0/OpenAccess.egg-info/SOURCES.txt
--rw-r--r--   0 jaiber    (1000) jaiber    (1000)        1 2023-04-24 21:22:56.000000 OpenAccess-0.1.0/OpenAccess.egg-info/dependency_links.txt
--rw-r--r--   0 jaiber    (1000) jaiber    (1000)        9 2023-04-24 21:22:56.000000 OpenAccess-0.1.0/OpenAccess.egg-info/requires.txt
--rw-r--r--   0 jaiber    (1000) jaiber    (1000)       11 2023-04-24 21:22:56.000000 OpenAccess-0.1.0/OpenAccess.egg-info/top_level.txt
--rw-rw-r--   0 jaiber    (1000) jaiber    (1000)     1581 2023-04-24 21:22:56.441590 OpenAccess-0.1.0/PKG-INFO
--rw-r--r--   0 jaiber    (1000) jaiber    (1000)     1249 2023-04-24 21:19:05.000000 OpenAccess-0.1.0/README.md
--rw-rw-r--   0 jaiber    (1000) jaiber    (1000)       38 2023-04-24 21:22:56.441590 OpenAccess-0.1.0/setup.cfg
--rw-r--r--   0 jaiber    (1000) jaiber    (1000)     1392 2023-04-03 16:58:33.000000 OpenAccess-0.1.0/setup.py
+drwxrwxr-x   0 jaiber    (1000) jaiber    (1000)        0 2023-04-24 21:25:40.693531 OpenAccess-0.1.1/
+drwxrwxr-x   0 jaiber    (1000) jaiber    (1000)        0 2023-04-24 21:25:40.689531 OpenAccess-0.1.1/OpenAccess/
+-rw-r--r--   0 jaiber    (1000) jaiber    (1000)      105 2023-04-24 21:25:34.000000 OpenAccess-0.1.1/OpenAccess/__init__.py
+-rw-r--r--   0 jaiber    (1000) jaiber    (1000)    10381 2023-04-24 21:17:53.000000 OpenAccess-0.1.1/OpenAccess/openaccess.py
+drwxrwxr-x   0 jaiber    (1000) jaiber    (1000)        0 2023-04-24 21:25:40.693531 OpenAccess-0.1.1/OpenAccess.egg-info/
+-rw-r--r--   0 jaiber    (1000) jaiber    (1000)     1581 2023-04-24 21:25:40.000000 OpenAccess-0.1.1/OpenAccess.egg-info/PKG-INFO
+-rw-r--r--   0 jaiber    (1000) jaiber    (1000)      235 2023-04-24 21:25:40.000000 OpenAccess-0.1.1/OpenAccess.egg-info/SOURCES.txt
+-rw-r--r--   0 jaiber    (1000) jaiber    (1000)        1 2023-04-24 21:25:40.000000 OpenAccess-0.1.1/OpenAccess.egg-info/dependency_links.txt
+-rw-r--r--   0 jaiber    (1000) jaiber    (1000)        9 2023-04-24 21:25:40.000000 OpenAccess-0.1.1/OpenAccess.egg-info/requires.txt
+-rw-r--r--   0 jaiber    (1000) jaiber    (1000)       11 2023-04-24 21:25:40.000000 OpenAccess-0.1.1/OpenAccess.egg-info/top_level.txt
+-rw-rw-r--   0 jaiber    (1000) jaiber    (1000)     1581 2023-04-24 21:25:40.693531 OpenAccess-0.1.1/PKG-INFO
+-rw-r--r--   0 jaiber    (1000) jaiber    (1000)     1249 2023-04-24 21:19:05.000000 OpenAccess-0.1.1/README.md
+-rw-rw-r--   0 jaiber    (1000) jaiber    (1000)       38 2023-04-24 21:25:40.693531 OpenAccess-0.1.1/setup.cfg
+-rw-r--r--   0 jaiber    (1000) jaiber    (1000)     1392 2023-04-03 16:58:33.000000 OpenAccess-0.1.1/setup.py
```

### Comparing `OpenAccess-0.1.0/OpenAccess/openaccess.py` & `OpenAccess-0.1.1/OpenAccess/openaccess.py`

 * *Files identical despite different names*

### Comparing `OpenAccess-0.1.0/OpenAccess.egg-info/PKG-INFO` & `OpenAccess-0.1.1/OpenAccess.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenAccess
-Version: 0.1.0
+Version: 0.1.1
 Summary: Librería no oficial para leer comunicarse con un servidor de LENEL OpenAccess 
 Home-page: https://github.com/alejomejia1
 Author: Alejandro Mejia Ayala, Jaiber Camacho
 Author-email: alejandromejia@qaingenieros.com
 License: GNU
 Description-Content-Type: text/markdown
```

### Comparing `OpenAccess-0.1.0/PKG-INFO` & `OpenAccess-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenAccess
-Version: 0.1.0
+Version: 0.1.1
 Summary: Librería no oficial para leer comunicarse con un servidor de LENEL OpenAccess 
 Home-page: https://github.com/alejomejia1
 Author: Alejandro Mejia Ayala, Jaiber Camacho
 Author-email: alejandromejia@qaingenieros.com
 License: GNU
 Description-Content-Type: text/markdown
```

### Comparing `OpenAccess-0.1.0/README.md` & `OpenAccess-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `OpenAccess-0.1.0/setup.py` & `OpenAccess-0.1.1/setup.py`

 * *Files identical despite different names*


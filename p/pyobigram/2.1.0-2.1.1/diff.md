# Comparing `tmp/pyobigram-2.1.0.tar.gz` & `tmp/pyobigram-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobigram-2.1.0.tar", last modified: Mon Apr 24 07:19:40 2023, max compression
+gzip compressed data, was "pyobigram-2.1.1.tar", last modified: Mon Apr 24 09:18:38 2023, max compression
```

## Comparing `pyobigram-2.1.0.tar` & `pyobigram-2.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 07:19:40.468398 pyobigram-2.1.0/
--rw-rw-rw-   0        0        0     1235 2023-04-13 20:26:37.000000 pyobigram-2.1.0/LICENSE
--rw-rw-rw-   0        0        0     1009 2023-04-24 07:19:40.458398 pyobigram-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1131 2023-04-13 20:26:37.000000 pyobigram-2.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 07:19:40.328398 pyobigram-2.1.0/pyobigram/
--rw-rw-rw-   0        0        0    18932 2023-04-13 20:26:37.000000 pyobigram-2.1.0/pyobigram/client.py
--rw-rw-rw-   0        0        0     1939 2023-04-13 20:26:37.000000 pyobigram-2.1.0/pyobigram/inline.py
--rw-rw-rw-   0        0        0    13252 2023-04-13 20:26:37.000000 pyobigram-2.1.0/pyobigram/paralleltransfer.py
--rw-rw-rw-   0        0        0     5512 2023-04-13 20:26:37.000000 pyobigram-2.1.0/pyobigram/readers.py
--rw-rw-rw-   0        0        0      932 2023-04-13 20:26:37.000000 pyobigram-2.1.0/pyobigram/threads.py
--rw-rw-rw-   0        0        0     9573 2023-04-13 20:26:37.000000 pyobigram-2.1.0/pyobigram/ttui.py
--rw-rw-rw-   0        0        0     3186 2023-04-13 20:26:37.000000 pyobigram-2.1.0/pyobigram/utils.py
--rw-rw-rw-   0        0        0       75 2023-04-13 20:26:37.000000 pyobigram-2.1.0/pyobigram/version.py
-drwxrwxrwx   0        0        0        0 2023-04-24 07:19:40.438398 pyobigram-2.1.0/pyobigram.egg-info/
--rw-rw-rw-   0        0        0     1009 2023-04-24 07:19:35.000000 pyobigram-2.1.0/pyobigram.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2023-04-24 07:19:37.000000 pyobigram-2.1.0/pyobigram.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 07:19:35.000000 pyobigram-2.1.0/pyobigram.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-04-24 07:19:35.000000 pyobigram-2.1.0/pyobigram.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-24 07:19:35.000000 pyobigram-2.1.0/pyobigram.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-24 07:19:35.000000 pyobigram-2.1.0/pyobigram.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-04-24 07:19:40.478398 pyobigram-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1632 2023-04-13 20:26:37.000000 pyobigram-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:18:38.387185 pyobigram-2.1.1/
+-rw-rw-rw-   0        0        0     1235 2023-04-13 20:26:37.000000 pyobigram-2.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1009 2023-04-24 09:18:38.377185 pyobigram-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1131 2023-04-13 20:26:37.000000 pyobigram-2.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 09:18:38.232177 pyobigram-2.1.1/pyobigram/
+-rw-rw-rw-   0        0        0    18932 2023-04-13 20:26:37.000000 pyobigram-2.1.1/pyobigram/client.py
+-rw-rw-rw-   0        0        0     1939 2023-04-13 20:26:37.000000 pyobigram-2.1.1/pyobigram/inline.py
+-rw-rw-rw-   0        0        0    13252 2023-04-13 20:26:37.000000 pyobigram-2.1.1/pyobigram/paralleltransfer.py
+-rw-rw-rw-   0        0        0     5512 2023-04-13 20:26:37.000000 pyobigram-2.1.1/pyobigram/readers.py
+-rw-rw-rw-   0        0        0      932 2023-04-13 20:26:37.000000 pyobigram-2.1.1/pyobigram/threads.py
+-rw-rw-rw-   0        0        0     9573 2023-04-13 20:26:37.000000 pyobigram-2.1.1/pyobigram/ttui.py
+-rw-rw-rw-   0        0        0     3186 2023-04-13 20:26:37.000000 pyobigram-2.1.1/pyobigram/utils.py
+-rw-rw-rw-   0        0        0       75 2023-04-24 09:18:16.000000 pyobigram-2.1.1/pyobigram/version.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:18:38.367185 pyobigram-2.1.1/pyobigram.egg-info/
+-rw-rw-rw-   0        0        0     1009 2023-04-24 09:18:35.000000 pyobigram-2.1.1/pyobigram.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2023-04-24 09:18:36.000000 pyobigram-2.1.1/pyobigram.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 09:18:35.000000 pyobigram-2.1.1/pyobigram.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-04-24 09:18:35.000000 pyobigram-2.1.1/pyobigram.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-24 09:18:35.000000 pyobigram-2.1.1/pyobigram.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-24 09:18:35.000000 pyobigram-2.1.1/pyobigram.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-04-24 09:18:38.397185 pyobigram-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1632 2023-04-13 20:26:37.000000 pyobigram-2.1.1/setup.py
```

### Comparing `pyobigram-2.1.0/LICENSE` & `pyobigram-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyobigram-2.1.0/PKG-INFO` & `pyobigram-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobigram
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python 3 library for telegram bots
 Home-page: https://github.com/ObisoftDev/pyobigram
 Author: ObisoftDev
 Author-email: obysoftt@gmail.com
 License: The Unlicense (Unlicense)
 Keywords: telegram,download,stream,bots
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyobigram-2.1.0/README.md` & `pyobigram-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyobigram-2.1.0/pyobigram/client.py` & `pyobigram-2.1.1/pyobigram/client.py`

 * *Files identical despite different names*

### Comparing `pyobigram-2.1.0/pyobigram/inline.py` & `pyobigram-2.1.1/pyobigram/inline.py`

 * *Files identical despite different names*

### Comparing `pyobigram-2.1.0/pyobigram/paralleltransfer.py` & `pyobigram-2.1.1/pyobigram/paralleltransfer.py`

 * *Files identical despite different names*

### Comparing `pyobigram-2.1.0/pyobigram/readers.py` & `pyobigram-2.1.1/pyobigram/readers.py`

 * *Files identical despite different names*

### Comparing `pyobigram-2.1.0/pyobigram/threads.py` & `pyobigram-2.1.1/pyobigram/threads.py`

 * *Files identical despite different names*

### Comparing `pyobigram-2.1.0/pyobigram/ttui.py` & `pyobigram-2.1.1/pyobigram/ttui.py`

 * *Files identical despite different names*

### Comparing `pyobigram-2.1.0/pyobigram/utils.py` & `pyobigram-2.1.1/pyobigram/utils.py`

 * *Files identical despite different names*

### Comparing `pyobigram-2.1.0/pyobigram.egg-info/PKG-INFO` & `pyobigram-2.1.1/pyobigram.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobigram
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python 3 library for telegram bots
 Home-page: https://github.com/ObisoftDev/pyobigram
 Author: ObisoftDev
 Author-email: obysoftt@gmail.com
 License: The Unlicense (Unlicense)
 Keywords: telegram,download,stream,bots
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyobigram-2.1.0/setup.py` & `pyobigram-2.1.1/setup.py`

 * *Files identical despite different names*


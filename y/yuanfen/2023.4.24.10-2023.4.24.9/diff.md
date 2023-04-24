# Comparing `tmp/yuanfen-2023.4.24.10.tar.gz` & `tmp/yuanfen-2023.4.24.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yuanfen-2023.4.24.10.tar", last modified: Mon Apr 24 12:58:29 2023, max compression
+gzip compressed data, was "yuanfen-2023.4.24.9.tar", last modified: Mon Apr 24 12:57:02 2023, max compression
```

## Comparing `yuanfen-2023.4.24.10.tar` & `yuanfen-2023.4.24.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:58:29.322533 yuanfen-2023.4.24.10/
--rw-r--r--   0 root         (0) root         (0)     1020 2023-04-24 12:58:29.321534 yuanfen-2023.4.24.10/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      686 2023-04-23 10:54:21.000000 yuanfen-2023.4.24.10/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 12:58:29.322533 yuanfen-2023.4.24.10/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      647 2023-04-23 08:36:40.000000 yuanfen-2023.4.24.10/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:58:29.321534 yuanfen-2023.4.24.10/yuanfen/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-24 12:58:28.000000 yuanfen-2023.4.24.10/yuanfen/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1881 2023-04-24 11:13:41.000000 yuanfen-2023.4.24.10/yuanfen/config.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2023-04-23 09:27:44.000000 yuanfen-2023.4.24.10/yuanfen/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:58:29.321534 yuanfen-2023.4.24.10/yuanfen.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1020 2023-04-24 12:58:29.000000 yuanfen-2023.4.24.10/yuanfen.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      228 2023-04-24 12:58:29.000000 yuanfen-2023.4.24.10/yuanfen.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 12:58:29.000000 yuanfen-2023.4.24.10/yuanfen.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-24 12:58:29.000000 yuanfen-2023.4.24.10/yuanfen.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-24 12:58:29.000000 yuanfen-2023.4.24.10/yuanfen.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:57:02.919557 yuanfen-2023.4.24.9/
+-rw-r--r--   0 root         (0) root         (0)     1019 2023-04-24 12:57:02.919557 yuanfen-2023.4.24.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      686 2023-04-23 10:54:21.000000 yuanfen-2023.4.24.9/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 12:57:02.919557 yuanfen-2023.4.24.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      647 2023-04-23 08:36:40.000000 yuanfen-2023.4.24.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:57:02.918557 yuanfen-2023.4.24.9/yuanfen/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-24 12:57:01.000000 yuanfen-2023.4.24.9/yuanfen/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1881 2023-04-24 11:13:41.000000 yuanfen-2023.4.24.9/yuanfen/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-04-23 09:27:44.000000 yuanfen-2023.4.24.9/yuanfen/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:57:02.918557 yuanfen-2023.4.24.9/yuanfen.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1019 2023-04-24 12:57:02.000000 yuanfen-2023.4.24.9/yuanfen.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      228 2023-04-24 12:57:02.000000 yuanfen-2023.4.24.9/yuanfen.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 12:57:02.000000 yuanfen-2023.4.24.9/yuanfen.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-24 12:57:02.000000 yuanfen-2023.4.24.9/yuanfen.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-24 12:57:02.000000 yuanfen-2023.4.24.9/yuanfen.egg-info/top_level.txt
```

### Comparing `yuanfen-2023.4.24.10/PKG-INFO` & `yuanfen-2023.4.24.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yuanfen
-Version: 2023.4.24.10
+Version: 2023.4.24.9
 Summary: Yuanfen Python Library
 Home-page: 
 Author: Bean
 Author-email: bean@yuanfen.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yuanfen-2023.4.24.10/README.md` & `yuanfen-2023.4.24.9/README.md`

 * *Files identical despite different names*

### Comparing `yuanfen-2023.4.24.10/setup.py` & `yuanfen-2023.4.24.9/setup.py`

 * *Files identical despite different names*

### Comparing `yuanfen-2023.4.24.10/yuanfen/config.py` & `yuanfen-2023.4.24.9/yuanfen/config.py`

 * *Files identical despite different names*

### Comparing `yuanfen-2023.4.24.10/yuanfen/logger.py` & `yuanfen-2023.4.24.9/yuanfen/logger.py`

 * *Files identical despite different names*

### Comparing `yuanfen-2023.4.24.10/yuanfen.egg-info/PKG-INFO` & `yuanfen-2023.4.24.9/yuanfen.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yuanfen
-Version: 2023.4.24.10
+Version: 2023.4.24.9
 Summary: Yuanfen Python Library
 Home-page: 
 Author: Bean
 Author-email: bean@yuanfen.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


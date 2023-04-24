# Comparing `tmp/ablerConfig-0.0.6.tar.gz` & `tmp/ablerConfig-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ablerConfig-0.0.6.tar", last modified: Mon Apr 24 09:26:48 2023, max compression
+gzip compressed data, was "ablerConfig-0.0.7.tar", last modified: Mon Apr 24 09:58:29 2023, max compression
```

## Comparing `ablerConfig-0.0.6.tar` & `ablerConfig-0.0.7.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:48.364877 ablerConfig-0.0.6/
--rw-rw-rw-   0        0        0     2004 2023-04-24 09:26:48.363877 ablerConfig-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1236 2023-04-23 22:28:12.000000 ablerConfig-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 09:26:48.361876 ablerConfig-0.0.6/ablerConfig.egg-info/
--rw-rw-rw-   0        0        0     2004 2023-04-24 09:26:48.000000 ablerConfig-0.0.6/ablerConfig.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-04-24 09:26:48.000000 ablerConfig-0.0.6/ablerConfig.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 09:26:48.000000 ablerConfig-0.0.6/ablerConfig.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-24 09:26:48.000000 ablerConfig-0.0.6/ablerConfig.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 09:26:48.000000 ablerConfig-0.0.6/ablerConfig.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 09:26:48.364877 ablerConfig-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1044 2023-04-24 09:24:45.000000 ablerConfig-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:58:29.795379 ablerConfig-0.0.7/
+-rw-rw-rw-   0        0        0     2004 2023-04-24 09:58:29.794379 ablerConfig-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1236 2023-04-23 22:28:12.000000 ablerConfig-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 09:58:29.785380 ablerConfig-0.0.7/ablerConfig/
+-rw-rw-rw-   0        0        0        0 2023-04-24 09:58:00.000000 ablerConfig-0.0.7/ablerConfig/__init__.py
+-rw-rw-rw-   0        0        0    12706 2023-04-22 20:35:47.000000 ablerConfig-0.0.7/ablerConfig/config.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:58:29.793379 ablerConfig-0.0.7/ablerConfig.egg-info/
+-rw-rw-rw-   0        0        0     2004 2023-04-24 09:58:29.000000 ablerConfig-0.0.7/ablerConfig.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-04-24 09:58:29.000000 ablerConfig-0.0.7/ablerConfig.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 09:58:29.000000 ablerConfig-0.0.7/ablerConfig.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-24 09:58:29.000000 ablerConfig-0.0.7/ablerConfig.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-24 09:58:29.000000 ablerConfig-0.0.7/ablerConfig.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 09:58:29.795379 ablerConfig-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1044 2023-04-24 09:58:12.000000 ablerConfig-0.0.7/setup.py
```

### Comparing `ablerConfig-0.0.6/PKG-INFO` & `ablerConfig-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ablerConfig
-Version: 0.0.6
+Version: 0.0.7
 Summary: 配置信息处理包
 Home-page: https://github.com/hanlaohan/abler-config
 Author: 憨老汉
 Author-email: hh28642257@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ablerConfig-0.0.6/README.md` & `ablerConfig-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ablerConfig-0.0.6/ablerConfig.egg-info/PKG-INFO` & `ablerConfig-0.0.7/ablerConfig.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ablerConfig
-Version: 0.0.6
+Version: 0.0.7
 Summary: 配置信息处理包
 Home-page: https://github.com/hanlaohan/abler-config
 Author: 憨老汉
 Author-email: hh28642257@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ablerConfig-0.0.6/setup.py` & `ablerConfig-0.0.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="ablerConfig",
-    version="0.0.6",
+    version="0.0.7",
     author="憨老汉",
     author_email="hh28642257@gmail.com",
     description="配置信息处理包",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hanlaohan/abler-config",
     packages=find_packages(),
```


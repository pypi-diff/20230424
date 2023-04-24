# Comparing `tmp/getRoutersConfig-0.0.1.tar.gz` & `tmp/getRoutersConfig-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getRoutersConfig-0.0.1.tar", last modified: Mon Apr 24 18:45:59 2023, max compression
+gzip compressed data, was "getRoutersConfig-0.0.2.tar", last modified: Mon Apr 24 18:51:36 2023, max compression
```

## Comparing `getRoutersConfig-0.0.1.tar` & `getRoutersConfig-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 18:45:59.985865 getRoutersConfig-0.0.1/
--rw-rw-rw-   0        0        0     1092 2023-04-22 13:23:07.000000 getRoutersConfig-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     4234 2023-04-24 18:45:59.985865 getRoutersConfig-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      150 2023-04-24 17:58:07.000000 getRoutersConfig-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 18:45:59.967993 getRoutersConfig-0.0.1/app/
-drwxrwxrwx   0        0        0        0 2023-04-24 18:45:59.973293 getRoutersConfig-0.0.1/app/getRoutersConfig/
--rw-rw-rw-   0        0        0       48 2023-04-22 20:51:53.000000 getRoutersConfig-0.0.1/app/getRoutersConfig/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 18:45:59.983864 getRoutersConfig-0.0.1/app/getRoutersConfig/src/
--rw-rw-rw-   0        0        0     9535 2023-04-24 18:18:52.000000 getRoutersConfig-0.0.1/app/getRoutersConfig/src/CiscoClass.py
--rw-rw-rw-   0        0        0     4106 2023-04-20 14:25:04.000000 getRoutersConfig-0.0.1/app/getRoutersConfig/src/HuaweiClass.py
--rw-rw-rw-   0        0        0     1028 2023-04-24 17:47:13.000000 getRoutersConfig-0.0.1/app/getRoutersConfig/src/RouterClass.py
--rw-rw-rw-   0        0        0        0 2023-04-22 18:35:47.000000 getRoutersConfig-0.0.1/app/getRoutersConfig/src/__init__.py
--rw-rw-rw-   0        0        0     2307 2023-04-23 13:29:05.000000 getRoutersConfig-0.0.1/app/getRoutersConfig/src/main.py
-drwxrwxrwx   0        0        0        0 2023-04-24 18:45:59.978297 getRoutersConfig-0.0.1/app/getRoutersConfig.egg-info/
--rw-rw-rw-   0        0        0     4234 2023-04-24 18:45:59.000000 getRoutersConfig-0.0.1/app/getRoutersConfig.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      467 2023-04-24 18:45:59.000000 getRoutersConfig-0.0.1/app/getRoutersConfig.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 18:45:59.000000 getRoutersConfig-0.0.1/app/getRoutersConfig.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-04-24 18:45:59.000000 getRoutersConfig-0.0.1/app/getRoutersConfig.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-24 18:45:59.000000 getRoutersConfig-0.0.1/app/getRoutersConfig.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 18:45:59.985865 getRoutersConfig-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1046 2023-04-23 22:32:25.000000 getRoutersConfig-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 18:51:36.061946 getRoutersConfig-0.0.2/
+-rw-rw-rw-   0        0        0     1092 2023-04-22 13:23:07.000000 getRoutersConfig-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4221 2023-04-24 18:51:36.061946 getRoutersConfig-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      150 2023-04-24 17:58:07.000000 getRoutersConfig-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 18:51:36.045362 getRoutersConfig-0.0.2/app/
+drwxrwxrwx   0        0        0        0 2023-04-24 18:51:36.049871 getRoutersConfig-0.0.2/app/getRoutersConfig/
+-rw-rw-rw-   0        0        0       48 2023-04-22 20:51:53.000000 getRoutersConfig-0.0.2/app/getRoutersConfig/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 18:51:36.059841 getRoutersConfig-0.0.2/app/getRoutersConfig/src/
+-rw-rw-rw-   0        0        0     9535 2023-04-24 18:18:52.000000 getRoutersConfig-0.0.2/app/getRoutersConfig/src/CiscoClass.py
+-rw-rw-rw-   0        0        0     4106 2023-04-20 14:25:04.000000 getRoutersConfig-0.0.2/app/getRoutersConfig/src/HuaweiClass.py
+-rw-rw-rw-   0        0        0     1028 2023-04-24 17:47:13.000000 getRoutersConfig-0.0.2/app/getRoutersConfig/src/RouterClass.py
+-rw-rw-rw-   0        0        0        0 2023-04-22 18:35:47.000000 getRoutersConfig-0.0.2/app/getRoutersConfig/src/__init__.py
+-rw-rw-rw-   0        0        0     2307 2023-04-23 13:29:05.000000 getRoutersConfig-0.0.2/app/getRoutersConfig/src/main.py
+drwxrwxrwx   0        0        0        0 2023-04-24 18:51:36.055835 getRoutersConfig-0.0.2/app/getRoutersConfig.egg-info/
+-rw-rw-rw-   0        0        0     4221 2023-04-24 18:51:35.000000 getRoutersConfig-0.0.2/app/getRoutersConfig.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      467 2023-04-24 18:51:35.000000 getRoutersConfig-0.0.2/app/getRoutersConfig.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 18:51:35.000000 getRoutersConfig-0.0.2/app/getRoutersConfig.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-04-24 18:51:35.000000 getRoutersConfig-0.0.2/app/getRoutersConfig.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-24 18:51:35.000000 getRoutersConfig-0.0.2/app/getRoutersConfig.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 18:51:36.061946 getRoutersConfig-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1033 2023-04-24 18:51:28.000000 getRoutersConfig-0.0.2/setup.py
```

### Comparing `getRoutersConfig-0.0.1/LICENSE` & `getRoutersConfig-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `getRoutersConfig-0.0.1/PKG-INFO` & `getRoutersConfig-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: getRoutersConfig
-Version: 0.0.1
-Summary: get routers (Cisco and Huawei) configuration as Json
+Version: 0.0.2
+Summary: get Cisco routers configuration as Json
 Home-page: https://github.com/DanielRicklin/getRoutersConfig
 Author: DanielRicklin
 Author-email: ricklin.daniel@outlook.fr
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

### Comparing `getRoutersConfig-0.0.1/app/getRoutersConfig/src/CiscoClass.py` & `getRoutersConfig-0.0.2/app/getRoutersConfig/src/CiscoClass.py`

 * *Files identical despite different names*

### Comparing `getRoutersConfig-0.0.1/app/getRoutersConfig/src/HuaweiClass.py` & `getRoutersConfig-0.0.2/app/getRoutersConfig/src/HuaweiClass.py`

 * *Files identical despite different names*

### Comparing `getRoutersConfig-0.0.1/app/getRoutersConfig/src/RouterClass.py` & `getRoutersConfig-0.0.2/app/getRoutersConfig/src/RouterClass.py`

 * *Files identical despite different names*

### Comparing `getRoutersConfig-0.0.1/app/getRoutersConfig/src/main.py` & `getRoutersConfig-0.0.2/app/getRoutersConfig/src/main.py`

 * *Files identical despite different names*

### Comparing `getRoutersConfig-0.0.1/app/getRoutersConfig.egg-info/PKG-INFO` & `getRoutersConfig-0.0.2/app/getRoutersConfig.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: getRoutersConfig
-Version: 0.0.1
-Summary: get routers (Cisco and Huawei) configuration as Json
+Version: 0.0.2
+Summary: get Cisco routers configuration as Json
 Home-page: https://github.com/DanielRicklin/getRoutersConfig
 Author: DanielRicklin
 Author-email: ricklin.daniel@outlook.fr
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

### Comparing `getRoutersConfig-0.0.1/setup.py` & `getRoutersConfig-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import find_packages, setup
 
 with open("app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="getRoutersConfig",
-    version="0.0.1",
-    description="get routers (Cisco and Huawei) configuration as Json",
+    version="0.0.2",
+    description="get Cisco routers configuration as Json",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/DanielRicklin/getRoutersConfig",
     author="DanielRicklin",
     author_email="ricklin.daniel@outlook.fr",
```


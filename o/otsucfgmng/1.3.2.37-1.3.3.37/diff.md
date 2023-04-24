# Comparing `tmp/otsucfgmng-1.3.2.37.tar.gz` & `tmp/otsucfgmng-1.3.3.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otsucfgmng-1.3.2.37.tar", last modified: Fri Jan 20 22:10:55 2023, max compression
+gzip compressed data, was "otsucfgmng-1.3.3.37.tar", last modified: Mon Apr 24 16:22:14 2023, max compression
```

## Comparing `otsucfgmng-1.3.2.37.tar` & `otsucfgmng-1.3.3.37.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-01-20 22:10:55.197662 otsucfgmng-1.3.2.37/
--rw-rw-rw-   0        0        0     1087 2021-09-12 16:41:27.000000 otsucfgmng-1.3.2.37/LICENSE.txt
--rw-rw-rw-   0        0        0    20207 2023-01-20 22:10:55.196155 otsucfgmng-1.3.2.37/PKG-INFO
--rw-rw-rw-   0        0        0    18508 2023-01-20 22:09:26.000000 otsucfgmng-1.3.2.37/README.md
-drwxrwxrwx   0        0        0        0 2023-01-20 22:10:55.181006 otsucfgmng-1.3.2.37/otsucfgmng/
--rw-rw-rw-   0        0        0      282 2023-01-15 01:49:53.000000 otsucfgmng-1.3.2.37/otsucfgmng/__init__.py
--rw-rw-rw-   0        0        0    10483 2023-01-20 22:09:43.000000 otsucfgmng-1.3.2.37/otsucfgmng/configuration_manager.py
--rw-rw-rw-   0        0        0     2110 2023-01-20 22:09:26.000000 otsucfgmng-1.3.2.37/otsucfgmng/funcs.py
-drwxrwxrwx   0        0        0        0 2023-01-20 22:10:55.195156 otsucfgmng-1.3.2.37/otsucfgmng.egg-info/
--rw-rw-rw-   0        0        0    20207 2023-01-20 22:10:55.000000 otsucfgmng-1.3.2.37/otsucfgmng.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-01-20 22:10:55.000000 otsucfgmng-1.3.2.37/otsucfgmng.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-20 22:10:55.000000 otsucfgmng-1.3.2.37/otsucfgmng.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-01-20 22:10:55.000000 otsucfgmng-1.3.2.37/otsucfgmng.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-01-20 22:10:55.000000 otsucfgmng-1.3.2.37/otsucfgmng.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-20 22:10:55.197662 otsucfgmng-1.3.2.37/setup.cfg
--rw-rw-rw-   0        0        0      867 2023-01-20 22:09:30.000000 otsucfgmng-1.3.2.37/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 16:22:14.404012 otsucfgmng-1.3.3.37/
+-rw-rw-rw-   0        0        0     1087 2021-09-12 16:41:27.000000 otsucfgmng-1.3.3.37/LICENSE.txt
+-rw-rw-rw-   0        0        0    20207 2023-04-24 16:22:14.402440 otsucfgmng-1.3.3.37/PKG-INFO
+-rw-rw-rw-   0        0        0    18508 2023-01-20 22:09:26.000000 otsucfgmng-1.3.3.37/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 16:22:14.380250 otsucfgmng-1.3.3.37/otsucfgmng/
+-rw-rw-rw-   0        0        0      282 2023-01-15 01:49:53.000000 otsucfgmng-1.3.3.37/otsucfgmng/__init__.py
+-rw-rw-rw-   0        0        0    10517 2023-04-24 16:17:59.000000 otsucfgmng-1.3.3.37/otsucfgmng/configuration_manager.py
+-rw-rw-rw-   0        0        0     2110 2023-01-20 22:09:26.000000 otsucfgmng-1.3.3.37/otsucfgmng/funcs.py
+drwxrwxrwx   0        0        0        0 2023-04-24 16:22:14.401436 otsucfgmng-1.3.3.37/otsucfgmng.egg-info/
+-rw-rw-rw-   0        0        0    20207 2023-04-24 16:22:14.000000 otsucfgmng-1.3.3.37/otsucfgmng.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-04-24 16:22:14.000000 otsucfgmng-1.3.3.37/otsucfgmng.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 16:22:14.000000 otsucfgmng-1.3.3.37/otsucfgmng.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-04-24 16:22:14.000000 otsucfgmng-1.3.3.37/otsucfgmng.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-24 16:22:14.000000 otsucfgmng-1.3.3.37/otsucfgmng.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 16:22:14.404961 otsucfgmng-1.3.3.37/setup.cfg
+-rw-rw-rw-   0        0        0      867 2023-04-24 16:18:40.000000 otsucfgmng-1.3.3.37/setup.py
```

### Comparing `otsucfgmng-1.3.2.37/LICENSE.txt` & `otsucfgmng-1.3.3.37/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `otsucfgmng-1.3.2.37/PKG-INFO` & `otsucfgmng-1.3.3.37/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otsucfgmng
-Version: 1.3.2.37
+Version: 1.3.3.37
 Summary: 設定ファイルを扱うクラスを生成するライブラリです。
 Home-page: https://github.com/Otsuhachi/OtsuConfigurationManager.git
 Author: Otsuhachi
 Author-email: agequodagis.tufuiegoeris@gmail.com
 License: MIT License
         
         Copyright (c) 2021 Otsuhachi
```

### Comparing `otsucfgmng-1.3.2.37/README.md` & `otsucfgmng-1.3.3.37/README.md`

 * *Files identical despite different names*

### Comparing `otsucfgmng-1.3.2.37/otsucfgmng/configuration_manager.py` & `otsucfgmng-1.3.3.37/otsucfgmng/configuration_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,15 +243,15 @@
             uv = getattr(self, k)
             dv = getattr(self, f"default_{k}_cm")
             position = place[k]
             u = user
             if position is not None:
                 for p in position:
                     u = u[p]
-            if not include_default_config and uv == dv:
+            if (not include_default_config or k in self.__hidden_options__) and uv == dv:
                 if u.get(k, OtsuNone) is not OtsuNone:
                     del u[k]
             else:
                 u[k] = uv
         return user
 
     @property
```

### Comparing `otsucfgmng-1.3.2.37/otsucfgmng/funcs.py` & `otsucfgmng-1.3.3.37/otsucfgmng/funcs.py`

 * *Files identical despite different names*

### Comparing `otsucfgmng-1.3.2.37/otsucfgmng.egg-info/PKG-INFO` & `otsucfgmng-1.3.3.37/otsucfgmng.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otsucfgmng
-Version: 1.3.2.37
+Version: 1.3.3.37
 Summary: 設定ファイルを扱うクラスを生成するライブラリです。
 Home-page: https://github.com/Otsuhachi/OtsuConfigurationManager.git
 Author: Otsuhachi
 Author-email: agequodagis.tufuiegoeris@gmail.com
 License: MIT License
         
         Copyright (c) 2021 Otsuhachi
```

### Comparing `otsucfgmng-1.3.2.37/setup.py` & `otsucfgmng-1.3.3.37/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     readme = f.read()
 with open("LICENSE.txt", "r", encoding="utf-8") as f:
     lcs = f.read()
 
-__VERSION__ = "1.3.2.37"
+__VERSION__ = "1.3.3.37"
 
 setup(
     name="otsucfgmng",
     version=__VERSION__,
     url="https://github.com/Otsuhachi/OtsuConfigurationManager.git",
     description="設定ファイルを扱うクラスを生成するライブラリです。",
     long_description_content_type="text/markdown",
```


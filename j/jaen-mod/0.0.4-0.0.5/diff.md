# Comparing `tmp/jaen_mod-0.0.4.tar.gz` & `tmp/jaen_mod-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaen_mod-0.0.4.tar", last modified: Mon Apr 24 07:42:44 2023, max compression
+gzip compressed data, was "jaen_mod-0.0.5.tar", last modified: Mon Apr 24 07:49:35 2023, max compression
```

## Comparing `jaen_mod-0.0.4.tar` & `jaen_mod-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 07:42:44.393880 jaen_mod-0.0.4/
--rw-rw-rw-   0        0        0      522 2023-04-24 07:42:44.393880 jaen_mod-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       73 2023-04-24 07:13:55.000000 jaen_mod-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 07:42:44.369880 jaen_mod-0.0.4/jaen_mod/
--rw-rw-rw-   0        0        0       44 2023-04-24 07:42:34.000000 jaen_mod-0.0.4/jaen_mod/__init__.py
--rw-rw-rw-   0        0        0     6841 2023-04-24 07:08:47.000000 jaen_mod-0.0.4/jaen_mod/jaen.py
-drwxrwxrwx   0        0        0        0 2023-04-24 07:42:44.391879 jaen_mod-0.0.4/jaen_mod.egg-info/
--rw-rw-rw-   0        0        0      522 2023-04-24 07:42:44.000000 jaen_mod-0.0.4/jaen_mod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-04-24 07:42:44.000000 jaen_mod-0.0.4/jaen_mod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 07:42:44.000000 jaen_mod-0.0.4/jaen_mod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-24 07:09:10.000000 jaen_mod-0.0.4/jaen_mod.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-04-24 07:42:44.000000 jaen_mod-0.0.4/jaen_mod.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-24 07:42:44.000000 jaen_mod-0.0.4/jaen_mod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 07:42:44.394881 jaen_mod-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      700 2023-04-24 07:42:35.000000 jaen_mod-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 07:49:35.272027 jaen_mod-0.0.5/
+-rw-rw-rw-   0        0        0      522 2023-04-24 07:49:35.272027 jaen_mod-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       73 2023-04-24 07:48:51.000000 jaen_mod-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 07:49:35.259029 jaen_mod-0.0.5/jaen_mod/
+-rw-rw-rw-   0        0        0       44 2023-04-24 07:48:41.000000 jaen_mod-0.0.5/jaen_mod/__init__.py
+-rw-rw-rw-   0        0        0     6841 2023-04-24 07:08:47.000000 jaen_mod-0.0.5/jaen_mod/jaen.py
+drwxrwxrwx   0        0        0        0 2023-04-24 07:49:35.270028 jaen_mod-0.0.5/jaen_mod.egg-info/
+-rw-rw-rw-   0        0        0      522 2023-04-24 07:49:35.000000 jaen_mod-0.0.5/jaen_mod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-04-24 07:49:35.000000 jaen_mod-0.0.5/jaen_mod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 07:49:35.000000 jaen_mod-0.0.5/jaen_mod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-24 07:09:10.000000 jaen_mod-0.0.5/jaen_mod.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-04-24 07:49:35.000000 jaen_mod-0.0.5/jaen_mod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-24 07:49:35.000000 jaen_mod-0.0.5/jaen_mod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 07:49:35.272027 jaen_mod-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      700 2023-04-24 07:48:37.000000 jaen_mod-0.0.5/setup.py
```

### Comparing `jaen_mod-0.0.4/PKG-INFO` & `jaen_mod-0.0.5/jaen_mod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: jaen_mod
-Version: 0.0.4
+Name: jaen-mod
+Version: 0.0.5
 Summary: Module for assisting JAEN project system written by ssim
 Home-page: http://git.jaen.kr/ssim/jaen_mod
 Author: ssim
 Author-email: sjk3037@gmail.com
 License: UNKNOWN
-Keywords: ssim,jaen,jaen-mod
+Keywords: ssim,jaen,jaen_mod
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
```

### Comparing `jaen_mod-0.0.4/jaen_mod/jaen.py` & `jaen_mod-0.0.5/jaen_mod/jaen.py`

 * *Files identical despite different names*

### Comparing `jaen_mod-0.0.4/jaen_mod.egg-info/PKG-INFO` & `jaen_mod-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: jaen-mod
-Version: 0.0.4
+Name: jaen_mod
+Version: 0.0.5
 Summary: Module for assisting JAEN project system written by ssim
 Home-page: http://git.jaen.kr/ssim/jaen_mod
 Author: ssim
 Author-email: sjk3037@gmail.com
 License: UNKNOWN
-Keywords: ssim,jaen,jaen-mod
+Keywords: ssim,jaen,jaen_mod
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
```

### Comparing `jaen_mod-0.0.4/setup.py` & `jaen_mod-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jaen_mod',
-    version='0.0.4',
+    version='0.0.5',
     description='Module for assisting JAEN project system written by ssim',
     author='ssim',
     author_email='sjk3037@gmail.com',
     url='http://git.jaen.kr/ssim/jaen_mod',
     install_requires=['pandas'],
     packages=find_packages(exclude=[]),
-    keywords=['ssim', 'jaen', 'jaen-mod'],
+    keywords=['ssim', 'jaen', 'jaen_mod'],
     python_requires='>=3.6',
     package_data={},
     zip_safe=False,
     classifiers=[
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
```


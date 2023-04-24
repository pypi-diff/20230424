# Comparing `tmp/ifastapi-0.0.2.tar.gz` & `tmp/ifastapi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifastapi-0.0.2.tar", last modified: Mon Apr 17 07:35:33 2023, max compression
+gzip compressed data, was "ifastapi-0.0.3.tar", last modified: Mon Apr 24 08:56:54 2023, max compression
```

## Comparing `ifastapi-0.0.2.tar` & `ifastapi-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 07:35:33.245016 ifastapi-0.0.2/
--rw-rw-rw-   0        0        0      231 2023-04-17 07:35:33.243928 ifastapi-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-17 07:35:33.233324 ifastapi-0.0.2/iFastApi/
--rw-rw-rw-   0        0        0       40 2023-04-17 04:17:29.000000 ifastapi-0.0.2/iFastApi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:35:33.234326 ifastapi-0.0.2/iFastApi/api/
--rw-rw-rw-   0        0        0       40 2023-04-17 07:25:09.000000 ifastapi-0.0.2/iFastApi/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:35:33.243928 ifastapi-0.0.2/ifastapi.egg-info/
--rw-rw-rw-   0        0        0      231 2023-04-17 07:35:33.000000 ifastapi-0.0.2/ifastapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-04-17 07:35:33.000000 ifastapi-0.0.2/ifastapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 07:35:33.000000 ifastapi-0.0.2/ifastapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-17 03:23:50.000000 ifastapi-0.0.2/ifastapi.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2023-04-17 07:35:33.000000 ifastapi-0.0.2/ifastapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-17 07:35:33.000000 ifastapi-0.0.2/ifastapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 07:35:33.245016 ifastapi-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      538 2023-04-17 07:35:29.000000 ifastapi-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:56:54.074232 ifastapi-0.0.3/
+-rw-rw-rw-   0        0        0      231 2023-04-24 08:56:54.073235 ifastapi-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       53 2023-04-24 08:55:07.000000 ifastapi-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 08:56:54.058235 ifastapi-0.0.3/iFastApi/
+-rw-rw-rw-   0        0        0     1068 2023-04-24 08:35:40.000000 ifastapi-0.0.3/iFastApi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:56:54.058235 ifastapi-0.0.3/iFastApi/api/
+-rw-rw-rw-   0        0        0       66 2023-04-23 07:25:56.000000 ifastapi-0.0.3/iFastApi/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:56:54.059234 ifastapi-0.0.3/iFastApi/db/
+-rw-rw-rw-   0        0        0      802 2023-04-23 10:00:35.000000 ifastapi-0.0.3/iFastApi/db/BaseQuery.py
+-rw-rw-rw-   0        0        0     1435 2023-04-24 08:35:40.000000 ifastapi-0.0.3/iFastApi/db/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:56:54.061232 ifastapi-0.0.3/iFastApi/utils/
+-rw-rw-rw-   0        0        0       40 2023-04-23 10:13:32.000000 ifastapi-0.0.3/iFastApi/utils/__init__.py
+-rw-rw-rw-   0        0        0      394 2023-04-24 08:01:17.000000 ifastapi-0.0.3/iFastApi/utils/singleton.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:56:54.072231 ifastapi-0.0.3/ifastapi.egg-info/
+-rw-rw-rw-   0        0        0      231 2023-04-24 08:56:53.000000 ifastapi-0.0.3/ifastapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2023-04-24 08:56:54.000000 ifastapi-0.0.3/ifastapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 08:56:53.000000 ifastapi-0.0.3/ifastapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-17 03:23:50.000000 ifastapi-0.0.3/ifastapi.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2023-04-24 08:56:53.000000 ifastapi-0.0.3/ifastapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-24 08:56:53.000000 ifastapi-0.0.3/ifastapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 08:56:54.074232 ifastapi-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      571 2023-04-24 08:56:47.000000 ifastapi-0.0.3/setup.py
```

### Comparing `ifastapi-0.0.2/setup.py` & `ifastapi-0.0.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(name='ifastapi',
-                 version='0.0.2',
+                 version='0.0.3',
                  description='基于fastapi二次优化 旨在更便捷、快速的搭建API',
                  url='https://github.com/ifczt/iFastApi',
                  author='IFCZT',
                  author_email='ifczt@qq.com',
                  license='MIT',
                  packages=setuptools.find_packages(),
                  password='aa83896389',
-                 install_requires=["fastapi"],
+                 install_requires=["fastapi","sqlalchemy","uvicorn","pymysql"],
                  zip_safe=False)
```


# Comparing `tmp/ifastapi-0.0.3.tar.gz` & `tmp/ifastapi-0.0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifastapi-0.0.3.tar", last modified: Mon Apr 24 08:56:54 2023, max compression
+gzip compressed data, was "ifastapi-0.0.3.1.tar", last modified: Mon Apr 24 09:14:04 2023, max compression
```

## Comparing `ifastapi-0.0.3.tar` & `ifastapi-0.0.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 08:56:54.074232 ifastapi-0.0.3/
--rw-rw-rw-   0        0        0      231 2023-04-24 08:56:54.073235 ifastapi-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       53 2023-04-24 08:55:07.000000 ifastapi-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 08:56:54.058235 ifastapi-0.0.3/iFastApi/
--rw-rw-rw-   0        0        0     1068 2023-04-24 08:35:40.000000 ifastapi-0.0.3/iFastApi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:56:54.058235 ifastapi-0.0.3/iFastApi/api/
--rw-rw-rw-   0        0        0       66 2023-04-23 07:25:56.000000 ifastapi-0.0.3/iFastApi/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:56:54.059234 ifastapi-0.0.3/iFastApi/db/
--rw-rw-rw-   0        0        0      802 2023-04-23 10:00:35.000000 ifastapi-0.0.3/iFastApi/db/BaseQuery.py
--rw-rw-rw-   0        0        0     1435 2023-04-24 08:35:40.000000 ifastapi-0.0.3/iFastApi/db/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:56:54.061232 ifastapi-0.0.3/iFastApi/utils/
--rw-rw-rw-   0        0        0       40 2023-04-23 10:13:32.000000 ifastapi-0.0.3/iFastApi/utils/__init__.py
--rw-rw-rw-   0        0        0      394 2023-04-24 08:01:17.000000 ifastapi-0.0.3/iFastApi/utils/singleton.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:56:54.072231 ifastapi-0.0.3/ifastapi.egg-info/
--rw-rw-rw-   0        0        0      231 2023-04-24 08:56:53.000000 ifastapi-0.0.3/ifastapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2023-04-24 08:56:54.000000 ifastapi-0.0.3/ifastapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 08:56:53.000000 ifastapi-0.0.3/ifastapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-17 03:23:50.000000 ifastapi-0.0.3/ifastapi.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2023-04-24 08:56:53.000000 ifastapi-0.0.3/ifastapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-24 08:56:53.000000 ifastapi-0.0.3/ifastapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 08:56:54.074232 ifastapi-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      571 2023-04-24 08:56:47.000000 ifastapi-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:14:04.102568 ifastapi-0.0.3.1/
+-rw-rw-rw-   0        0        0      233 2023-04-24 09:14:04.101568 ifastapi-0.0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0       53 2023-04-24 08:55:07.000000 ifastapi-0.0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 09:14:04.080568 ifastapi-0.0.3.1/iFastApi/
+-rw-rw-rw-   0        0        0     1069 2023-04-24 09:09:29.000000 ifastapi-0.0.3.1/iFastApi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:14:04.080568 ifastapi-0.0.3.1/iFastApi/api/
+-rw-rw-rw-   0        0        0       66 2023-04-23 07:25:56.000000 ifastapi-0.0.3.1/iFastApi/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:14:04.082567 ifastapi-0.0.3.1/iFastApi/db/
+-rw-rw-rw-   0        0        0      802 2023-04-23 10:00:35.000000 ifastapi-0.0.3.1/iFastApi/db/BaseQuery.py
+-rw-rw-rw-   0        0        0     1435 2023-04-24 09:12:58.000000 ifastapi-0.0.3.1/iFastApi/db/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:14:04.083569 ifastapi-0.0.3.1/iFastApi/utils/
+-rw-rw-rw-   0        0        0       40 2023-04-23 10:13:32.000000 ifastapi-0.0.3.1/iFastApi/utils/__init__.py
+-rw-rw-rw-   0        0        0      394 2023-04-24 08:01:17.000000 ifastapi-0.0.3.1/iFastApi/utils/singleton.py
+drwxrwxrwx   0        0        0        0 2023-04-24 09:14:04.100568 ifastapi-0.0.3.1/ifastapi.egg-info/
+-rw-rw-rw-   0        0        0      233 2023-04-24 09:14:04.000000 ifastapi-0.0.3.1/ifastapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2023-04-24 09:14:04.000000 ifastapi-0.0.3.1/ifastapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 09:14:04.000000 ifastapi-0.0.3.1/ifastapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-17 03:23:50.000000 ifastapi-0.0.3.1/ifastapi.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2023-04-24 09:14:04.000000 ifastapi-0.0.3.1/ifastapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-24 09:14:04.000000 ifastapi-0.0.3.1/ifastapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 09:14:04.102568 ifastapi-0.0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      573 2023-04-24 09:14:00.000000 ifastapi-0.0.3.1/setup.py
```

### Comparing `ifastapi-0.0.3/iFastApi/__init__.py` & `ifastapi-0.0.3.1/iFastApi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Author: IFCZT
 # Email: ifczt@qq.com
 import uvicorn
 from fastapi import FastAPI
 from starlette.middleware.cors import CORSMiddleware
 
-from db import DBManager
+from .db import DBManager
 
 
 class IFastAPI:
     """
     config: 配置文件
         - ORIGINS: 允许跨域的域名 默认为'*'
     """
```

### Comparing `ifastapi-0.0.3/iFastApi/db/BaseQuery.py` & `ifastapi-0.0.3.1/iFastApi/db/BaseQuery.py`

 * *Files identical despite different names*

### Comparing `ifastapi-0.0.3/iFastApi/db/__init__.py` & `ifastapi-0.0.3.1/iFastApi/db/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Author: IFCZT
 # Email: ifczt@qq.com
 from sqlalchemy import create_engine, Column, Integer, SmallInteger
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import sessionmaker
 
-from db.BaseQuery import BaseQuery
-from utils.singleton import Singleton
+from .BaseQuery import BaseQuery
+from ..utils.singleton import Singleton
 
 
 @Singleton
 class DBManager:
     base = declarative_base()
     def __init__(self):
         self._base = None
```

### Comparing `ifastapi-0.0.3/setup.py` & `ifastapi-0.0.3.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 setuptools.setup(name='ifastapi',
-                 version='0.0.3',
+                 version='0.0.3.1',
                  description='基于fastapi二次优化 旨在更便捷、快速的搭建API',
                  url='https://github.com/ifczt/iFastApi',
                  author='IFCZT',
                  author_email='ifczt@qq.com',
                  license='MIT',
                  packages=setuptools.find_packages(),
                  password='aa83896389',
```


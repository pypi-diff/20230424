# Comparing `tmp/graphdisplay-0.0.1.tar.gz` & `tmp/graphdisplay-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphdisplay-0.0.1.tar", last modified: Mon Apr 24 14:16:41 2023, max compression
+gzip compressed data, was "graphdisplay-0.0.2.tar", last modified: Mon Apr 24 14:35:36 2023, max compression
```

## Comparing `graphdisplay-0.0.1.tar` & `graphdisplay-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-04-24 14:16:41.173706 graphdisplay-0.0.1/
--rw-rw-r--   0 beto      (1000) beto      (1000)      420 2023-04-24 14:16:41.173706 graphdisplay-0.0.1/PKG-INFO
--rw-rw-r--   0 beto      (1000) beto      (1000)      124 2023-04-24 14:06:00.000000 graphdisplay-0.0.1/README.md
-drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-04-24 14:16:41.173706 graphdisplay-0.0.1/graphdisplay/
--rw-rw-r--   0 beto      (1000) beto      (1000)       34 2023-04-24 10:24:01.000000 graphdisplay-0.0.1/graphdisplay/__init__.py
--rw-rw-r--   0 beto      (1000) beto      (1000)     8277 2023-04-24 10:17:25.000000 graphdisplay-0.0.1/graphdisplay/graphdisplay.py
-drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-04-24 14:16:41.173706 graphdisplay-0.0.1/graphdisplay.egg-info/
--rw-rw-r--   0 beto      (1000) beto      (1000)      420 2023-04-24 14:16:41.000000 graphdisplay-0.0.1/graphdisplay.egg-info/PKG-INFO
--rw-rw-r--   0 beto      (1000) beto      (1000)      251 2023-04-24 14:16:41.000000 graphdisplay-0.0.1/graphdisplay.egg-info/SOURCES.txt
--rw-rw-r--   0 beto      (1000) beto      (1000)        1 2023-04-24 14:16:41.000000 graphdisplay-0.0.1/graphdisplay.egg-info/dependency_links.txt
--rw-rw-r--   0 beto      (1000) beto      (1000)       13 2023-04-24 14:16:41.000000 graphdisplay-0.0.1/graphdisplay.egg-info/requires.txt
--rw-rw-r--   0 beto      (1000) beto      (1000)       13 2023-04-24 14:16:41.000000 graphdisplay-0.0.1/graphdisplay.egg-info/top_level.txt
--rw-rw-r--   0 beto      (1000) beto      (1000)       38 2023-04-24 14:16:41.173706 graphdisplay-0.0.1/setup.cfg
--rw-rw-r--   0 beto      (1000) beto      (1000)     1335 2023-04-24 14:16:35.000000 graphdisplay-0.0.1/setup.py
+drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-04-24 14:35:36.785170 graphdisplay-0.0.2/
+-rw-rw-r--   0 beto      (1000) beto      (1000)      420 2023-04-24 14:35:36.785170 graphdisplay-0.0.2/PKG-INFO
+-rw-rw-r--   0 beto      (1000) beto      (1000)      124 2023-04-24 14:33:17.000000 graphdisplay-0.0.2/README.md
+drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-04-24 14:35:36.785170 graphdisplay-0.0.2/graphdisplay/
+-rw-rw-r--   0 beto      (1000) beto      (1000)       34 2023-04-24 14:33:17.000000 graphdisplay-0.0.2/graphdisplay/__init__.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)     8277 2023-04-24 14:33:17.000000 graphdisplay-0.0.2/graphdisplay/graphdisplay.py
+drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-04-24 14:35:36.785170 graphdisplay-0.0.2/graphdisplay.egg-info/
+-rw-rw-r--   0 beto      (1000) beto      (1000)      420 2023-04-24 14:35:36.000000 graphdisplay-0.0.2/graphdisplay.egg-info/PKG-INFO
+-rw-rw-r--   0 beto      (1000) beto      (1000)      251 2023-04-24 14:35:36.000000 graphdisplay-0.0.2/graphdisplay.egg-info/SOURCES.txt
+-rw-rw-r--   0 beto      (1000) beto      (1000)        1 2023-04-24 14:35:36.000000 graphdisplay-0.0.2/graphdisplay.egg-info/dependency_links.txt
+-rw-rw-r--   0 beto      (1000) beto      (1000)        8 2023-04-24 14:35:36.000000 graphdisplay-0.0.2/graphdisplay.egg-info/requires.txt
+-rw-rw-r--   0 beto      (1000) beto      (1000)       13 2023-04-24 14:35:36.000000 graphdisplay-0.0.2/graphdisplay.egg-info/top_level.txt
+-rw-rw-r--   0 beto      (1000) beto      (1000)       38 2023-04-24 14:35:36.785170 graphdisplay-0.0.2/setup.cfg
+-rw-rw-r--   0 beto      (1000) beto      (1000)     1321 2023-04-24 14:34:29.000000 graphdisplay-0.0.2/setup.py
```

### Comparing `graphdisplay-0.0.1/graphdisplay/graphdisplay.py` & `graphdisplay-0.0.2/graphdisplay/graphdisplay.py`

 * *Files identical despite different names*

### Comparing `graphdisplay-0.0.1/setup.py` & `graphdisplay-0.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.0.1' #Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
+VERSION = '0.0.2' #Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
 PACKAGE_NAME = 'graphdisplay' #Debe coincidir con el nombre de la carpeta
 AUTHOR = 'Alberto Penas Díaz' #Modificar con vuestros datos
 AUTHOR_EMAIL = 'albertopenasdiaz@gmail.com' #Modificar con vuestros datos
 URL = 'https://github.com/seniorbeto' #Modificar con vuestros datos
 
 LICENSE = 'MIT' #Tipo de licencia
 DESCRIPTION = 'Librería para representar visualmente grafos de tipo diccionario' #Descripción corta
 LONG_DESCRIPTION = (HERE / "README.md").read_text(encoding='utf-8') #Referencia al documento README con una descripción más elaborada
 LONG_DESC_TYPE = "text/markdown"
 
 
 #Paquetes necesarios para que funcione la libreía. Se instalarán a la vez si no lo tuvieras ya instalado
 INSTALL_REQUIRES = [
-      'tkinter',
-      'math'
+      'tkinter'
       ]
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
```


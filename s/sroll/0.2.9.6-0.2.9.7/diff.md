# Comparing `tmp/sroll-0.2.9.6.tar.gz` & `tmp/sroll-0.2.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sroll-0.2.9.6.tar", last modified: Wed Apr 12 13:38:23 2023, max compression
+gzip compressed data, was "dist/sroll-0.2.9.7.tar", last modified: Mon Apr 24 14:28:28 2023, max compression
```

## Comparing `sroll-0.2.9.6.tar` & `sroll-0.2.9.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 tfoulqui (205105) droos    (10042)        0 2023-04-12 13:38:23.000000 sroll-0.2.9.6/
--rw-r--r--   0 tfoulqui (205105) droos    (10042)       38 2023-04-12 13:38:23.000000 sroll-0.2.9.6/setup.cfg
--rw-r--r--   0 tfoulqui (205105) droos    (10042)       46 2023-01-26 14:13:59.000000 sroll-0.2.9.6/MANIFEST.in
--rw-r--r--   0 tfoulqui (205105) droos    (10042)      787 2023-04-12 13:38:13.000000 sroll-0.2.9.6/setup.py
-drwxr-xr-x   0 tfoulqui (205105) droos    (10042)        0 2023-04-12 13:38:23.000000 sroll-0.2.9.6/sroll.egg-info/
--rw-r--r--   0 tfoulqui (205105) droos    (10042)        1 2023-04-12 13:38:22.000000 sroll-0.2.9.6/sroll.egg-info/dependency_links.txt
--rw-r--r--   0 tfoulqui (205105) droos    (10042)      253 2023-04-12 13:38:23.000000 sroll-0.2.9.6/sroll.egg-info/SOURCES.txt
--rw-r--r--   0 tfoulqui (205105) droos    (10042)       21 2023-04-12 13:38:22.000000 sroll-0.2.9.6/sroll.egg-info/requires.txt
--rw-r--r--   0 tfoulqui (205105) droos    (10042)      506 2023-04-12 13:38:22.000000 sroll-0.2.9.6/sroll.egg-info/PKG-INFO
--rw-r--r--   0 tfoulqui (205105) droos    (10042)       14 2023-04-12 13:38:22.000000 sroll-0.2.9.6/sroll.egg-info/top_level.txt
-drwxr-xr-x   0 tfoulqui (205105) droos    (10042)        0 2023-04-12 13:38:23.000000 sroll-0.2.9.6/sroll_package/
--rw-r--r--   0 tfoulqui (205105) droos    (10042)     8266 2023-04-12 13:37:43.000000 sroll-0.2.9.6/sroll_package/set_env.py
--rw-r--r--   0 tfoulqui (205105) droos    (10042)      142 2023-01-26 14:13:59.000000 sroll-0.2.9.6/sroll_package/__init__.py
-drwxr-xr-x   0 tfoulqui (205105) droos    (10042)        0 2023-04-12 13:38:23.000000 sroll-0.2.9.6/sroll_package/static/
--rw-r--r--   0 tfoulqui (205105) droos    (10042)      793 2023-03-29 12:59:48.000000 sroll-0.2.9.6/sroll_package/static/requirements.txt
--rw-r--r--   0 tfoulqui (205105) droos    (10042)      506 2023-04-12 13:38:23.000000 sroll-0.2.9.6/PKG-INFO
+drwxr-xr-x   0 tfoulqui (205105) droos    (10042)        0 2023-04-24 14:28:28.000000 sroll-0.2.9.7/
+-rw-r--r--   0 tfoulqui (205105) droos    (10042)       38 2023-04-24 14:28:28.000000 sroll-0.2.9.7/setup.cfg
+-rw-r--r--   0 tfoulqui (205105) droos    (10042)       46 2023-01-26 14:13:59.000000 sroll-0.2.9.7/MANIFEST.in
+-rw-r--r--   0 tfoulqui (205105) droos    (10042)      787 2023-04-24 14:28:03.000000 sroll-0.2.9.7/setup.py
+drwxr-xr-x   0 tfoulqui (205105) droos    (10042)        0 2023-04-24 14:28:28.000000 sroll-0.2.9.7/sroll.egg-info/
+-rw-r--r--   0 tfoulqui (205105) droos    (10042)        1 2023-04-24 14:28:27.000000 sroll-0.2.9.7/sroll.egg-info/dependency_links.txt
+-rw-r--r--   0 tfoulqui (205105) droos    (10042)      253 2023-04-24 14:28:27.000000 sroll-0.2.9.7/sroll.egg-info/SOURCES.txt
+-rw-r--r--   0 tfoulqui (205105) droos    (10042)       21 2023-04-24 14:28:27.000000 sroll-0.2.9.7/sroll.egg-info/requires.txt
+-rw-r--r--   0 tfoulqui (205105) droos    (10042)      506 2023-04-24 14:28:27.000000 sroll-0.2.9.7/sroll.egg-info/PKG-INFO
+-rw-r--r--   0 tfoulqui (205105) droos    (10042)       14 2023-04-24 14:28:27.000000 sroll-0.2.9.7/sroll.egg-info/top_level.txt
+drwxr-xr-x   0 tfoulqui (205105) droos    (10042)        0 2023-04-24 14:28:28.000000 sroll-0.2.9.7/sroll_package/
+-rw-r--r--   0 tfoulqui (205105) droos    (10042)     8248 2023-04-24 14:27:31.000000 sroll-0.2.9.7/sroll_package/set_env.py
+-rw-r--r--   0 tfoulqui (205105) droos    (10042)      142 2023-01-26 14:13:59.000000 sroll-0.2.9.7/sroll_package/__init__.py
+drwxr-xr-x   0 tfoulqui (205105) droos    (10042)        0 2023-04-24 14:28:28.000000 sroll-0.2.9.7/sroll_package/static/
+-rw-r--r--   0 tfoulqui (205105) droos    (10042)      793 2023-03-29 12:59:48.000000 sroll-0.2.9.7/sroll_package/static/requirements.txt
+-rw-r--r--   0 tfoulqui (205105) droos    (10042)      506 2023-04-24 14:28:28.000000 sroll-0.2.9.7/PKG-INFO
```

### Comparing `sroll-0.2.9.6/setup.py` & `sroll-0.2.9.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 
 
 
 setuptools.setup(
     name='sroll',
-    version='0.2.9.6',    
+    version='0.2.9.7',    
     description='Python package for SRoll installation',    
     url='https://gitlab.ifremer.fr/iaocea/srollex.git',
     author='Theo Foulquier',
     author_email='tfoulqui@ifremer.fr',
     license='BSD 2-clause',
     include_package_data = True,
     packages=['sroll_package'],
```

### Comparing `sroll-0.2.9.6/sroll_package/set_env.py` & `sroll-0.2.9.7/sroll_package/set_env.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,14 @@
   """
   current_path = os.path.dirname(os.path.abspath(__file__))
   
   #os.system('virtualenv -p python3.6 ' +str(path)+'/py_sroll')
   try:
     #os.system('python3.6 -m venv ' +str(path)+'/py_sroll')
     os.system('virtualenv -p python3.6 ' +str(path)+'/py_sroll')
-    print("PASS")
     #os.system('virtualenv --python=3.6 ' +str(path)+'/py_sroll')
   except:
     try:
       os.system('virtualenv -p python3.6 ' +str(path)+'/py_sroll')
     except:
       #os.system('virtualenv -p python3 ' +str(path)+'/py_sroll')
       os.system('echo ERROR : failed to install python 3.6')
```

### Comparing `sroll-0.2.9.6/sroll_package/static/requirements.txt` & `sroll-0.2.9.7/sroll_package/static/requirements.txt`

 * *Files identical despite different names*


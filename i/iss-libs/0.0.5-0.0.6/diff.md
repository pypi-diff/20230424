# Comparing `tmp/iss-libs-0.0.5.tar.gz` & `tmp/iss-libs-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iss-libs-0.0.5.tar", last modified: Thu Jan  5 08:58:23 2023, max compression
+gzip compressed data, was "iss-libs-0.0.6.tar", last modified: Mon Apr 24 02:22:14 2023, max compression
```

## Comparing `iss-libs-0.0.5.tar` & `iss-libs-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 miniphoton  (1000) miniphoton  (1000)        0 2023-01-05 08:58:23.921608 iss-libs-0.0.5/
--rw-rw-r--   0 miniphoton  (1000) miniphoton  (1000)     1084 2022-12-28 09:04:32.000000 iss-libs-0.0.5/LICENSE
--rw-rw-r--   0 miniphoton  (1000) miniphoton  (1000)     1247 2023-01-05 08:58:23.921608 iss-libs-0.0.5/PKG-INFO
--rw-rw-r--   0 miniphoton  (1000) miniphoton  (1000)      688 2023-01-05 08:56:08.000000 iss-libs-0.0.5/README.md
-drwxrwxr-x   0 miniphoton  (1000) miniphoton  (1000)        0 2023-01-05 08:58:23.921608 iss-libs-0.0.5/iss_libs.egg-info/
--rw-rw-r--   0 miniphoton  (1000) miniphoton  (1000)     1247 2023-01-05 08:58:23.000000 iss-libs-0.0.5/iss_libs.egg-info/PKG-INFO
--rw-rw-r--   0 miniphoton  (1000) miniphoton  (1000)      195 2023-01-05 08:58:23.000000 iss-libs-0.0.5/iss_libs.egg-info/SOURCES.txt
--rw-rw-r--   0 miniphoton  (1000) miniphoton  (1000)        1 2023-01-05 08:58:23.000000 iss-libs-0.0.5/iss_libs.egg-info/dependency_links.txt
--rw-rw-r--   0 miniphoton  (1000) miniphoton  (1000)      197 2023-01-05 08:58:23.000000 iss-libs-0.0.5/iss_libs.egg-info/requires.txt
--rw-rw-r--   0 miniphoton  (1000) miniphoton  (1000)        1 2023-01-05 08:58:23.000000 iss-libs-0.0.5/iss_libs.egg-info/top_level.txt
--rw-rw-r--   0 miniphoton  (1000) miniphoton  (1000)       79 2023-01-05 08:58:23.925608 iss-libs-0.0.5/setup.cfg
--rw-rw-r--   0 miniphoton  (1000) miniphoton  (1000)     2057 2023-01-05 08:56:47.000000 iss-libs-0.0.5/setup.py
+drwxrwxr-x   0 minipack3  (1000) minipack3  (1000)        0 2023-04-24 02:22:14.421837 iss-libs-0.0.6/
+-rw-rw-r--   0 minipack3  (1000) minipack3  (1000)     1084 2023-04-24 02:13:12.000000 iss-libs-0.0.6/LICENSE
+-rw-rw-r--   0 minipack3  (1000) minipack3  (1000)     1167 2023-04-24 02:22:14.421837 iss-libs-0.0.6/PKG-INFO
+-rw-rw-r--   0 minipack3  (1000) minipack3  (1000)      605 2023-04-24 02:15:50.000000 iss-libs-0.0.6/README.md
+drwxrwxr-x   0 minipack3  (1000) minipack3  (1000)        0 2023-04-24 02:22:14.421837 iss-libs-0.0.6/iss_libs.egg-info/
+-rw-rw-r--   0 minipack3  (1000) minipack3  (1000)     1167 2023-04-24 02:22:14.000000 iss-libs-0.0.6/iss_libs.egg-info/PKG-INFO
+-rw-rw-r--   0 minipack3  (1000) minipack3  (1000)      195 2023-04-24 02:22:14.000000 iss-libs-0.0.6/iss_libs.egg-info/SOURCES.txt
+-rw-rw-r--   0 minipack3  (1000) minipack3  (1000)        1 2023-04-24 02:22:14.000000 iss-libs-0.0.6/iss_libs.egg-info/dependency_links.txt
+-rw-rw-r--   0 minipack3  (1000) minipack3  (1000)      232 2023-04-24 02:22:14.000000 iss-libs-0.0.6/iss_libs.egg-info/requires.txt
+-rw-rw-r--   0 minipack3  (1000) minipack3  (1000)        1 2023-04-24 02:22:14.000000 iss-libs-0.0.6/iss_libs.egg-info/top_level.txt
+-rw-rw-r--   0 minipack3  (1000) minipack3  (1000)       79 2023-04-24 02:22:14.421837 iss-libs-0.0.6/setup.cfg
+-rw-rw-r--   0 minipack3  (1000) minipack3  (1000)     2148 2023-04-24 02:17:04.000000 iss-libs-0.0.6/setup.py
```

### Comparing `iss-libs-0.0.5/LICENSE` & `iss-libs-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `iss-libs-0.0.5/PKG-INFO` & `iss-libs-0.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iss-libs
-Version: 0.0.5
+Version: 0.0.6
 Home-page: https://github.com/postersom/iss-libs
 Author: Somsak Binyaranee
 Author-email: poster.som@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -24,17 +24,14 @@
 ---------------
 
 To install iss_libs, simply run the following at your prompt:
 
 ```bash
   # from pypi
   pip3 install iss-libs
-  
-  # from source
-  pip3 install git+https://github.com/postersom/iss_libs.git
 
 ```
 ☤ Contributions
 ---------------
 - Somsak Binyaranee (@postersom) - Tests / CI / Uploads to Pypi
 
 ☤ License
```

### Comparing `iss-libs-0.0.5/README.md` & `iss-libs-0.0.6/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -7,17 +7,14 @@
 ---------------
 
 To install iss_libs, simply run the following at your prompt:
 
 ```bash
   # from pypi
   pip3 install iss-libs
-  
-  # from source
-  pip3 install git+https://github.com/postersom/iss_libs.git
 
 ```
 ☤ Contributions
 ---------------
 - Somsak Binyaranee (@postersom) - Tests / CI / Uploads to Pypi
 
 ☤ License
```

### Comparing `iss-libs-0.0.5/iss_libs.egg-info/PKG-INFO` & `iss-libs-0.0.6/iss_libs.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iss-libs
-Version: 0.0.5
+Version: 0.0.6
 Home-page: https://github.com/postersom/iss-libs
 Author: Somsak Binyaranee
 Author-email: poster.som@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -24,17 +24,14 @@
 ---------------
 
 To install iss_libs, simply run the following at your prompt:
 
 ```bash
   # from pypi
   pip3 install iss-libs
-  
-  # from source
-  pip3 install git+https://github.com/postersom/iss_libs.git
 
 ```
 ☤ Contributions
 ---------------
 - Somsak Binyaranee (@postersom) - Tests / CI / Uploads to Pypi
 
 ☤ License
```

### Comparing `iss-libs-0.0.5/setup.py` & `iss-libs-0.0.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='iss-libs',  # How you named your package folder (MyLib)
-    version='0.0.5',  # Start with a small number and increase it with every change you make
+    version='0.0.6',  # Start with a small number and increase it with every change you make
     author='Somsak Binyaranee',  # Type in your name
     author_email='poster.som@gmail.com',  # Type in your E-Mail
     description='',  # Give a short description about your library
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/postersom/iss-libs',  # Provide either the link to your github or to your website
     license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
@@ -20,24 +20,27 @@
                       'Flask-SocketIO',
                       'marshmallow',
                       'marshmallow_sqlalchemy',
                       'matplotlib',
                       'paramiko',
                       'prettytable',
                       'psutil',
+                      'pyserial',
                       'python-dotenv',
                       'python-gitlab',
                       'redis',
                       'robotframework',
+                      'robotframework-sshlibrary',
                       'six',
                       'sqlalchemy',
                       'swagger-ui-bundle',
                       'xmltodict'],
     classifiers=[
-        'Development Status :: 4 - Beta',   # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
+        'Development Status :: 4 - Beta',
+        # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         'Intended Audience :: Developers',  # Define that your audience are developers
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',  # Again, pick a license
         'Programming Language :: Python :: 3.9',  # Specify which pyhton versions that you want to support
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
```


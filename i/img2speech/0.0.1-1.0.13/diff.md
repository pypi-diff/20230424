# Comparing `tmp/img2speech-0.0.1.tar.gz` & `tmp/img2speech-1.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "img2speech-0.0.1.tar", last modified: Mon Apr 24 08:21:49 2023, max compression
+gzip compressed data, was "img2speech-1.0.13.tar", last modified: Mon Apr 24 08:07:57 2023, max compression
```

## Comparing `img2speech-0.0.1.tar` & `img2speech-1.0.13.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 08:21:49.502405 img2speech-0.0.1/
--rw-rw-rw-   0        0        0     1089 2023-03-15 09:28:29.000000 img2speech-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     3668 2023-04-24 08:21:49.499454 img2speech-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3284 2023-04-22 14:21:01.000000 img2speech-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 08:21:49.444557 img2speech-0.0.1/img2speech/
-drwxrwxrwx   0        0        0        0 2023-04-24 08:21:49.491465 img2speech-0.0.1/img2speech/src/
-drwxrwxrwx   0        0        0        0 2023-04-24 08:21:49.485483 img2speech-0.0.1/img2speech/src/img2speech.egg-info/
--rw-rw-rw-   0        0        0     3668 2023-04-24 08:21:48.000000 img2speech-0.0.1/img2speech/src/img2speech.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-04-24 08:21:49.000000 img2speech-0.0.1/img2speech/src/img2speech.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 08:21:48.000000 img2speech-0.0.1/img2speech/src/img2speech.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-04-24 08:21:48.000000 img2speech-0.0.1/img2speech/src/img2speech.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-24 08:21:48.000000 img2speech-0.0.1/img2speech/src/img2speech.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4495 2023-04-24 08:01:36.000000 img2speech-0.0.1/img2speech/src/img2speech.py
--rw-rw-rw-   0        0        0       42 2023-04-24 08:21:49.502405 img2speech-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1195 2023-04-24 08:17:48.000000 img2speech-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:07:57.258624 img2speech-1.0.13/
+-rw-rw-rw-   0        0        0     1089 2023-03-15 09:28:29.000000 img2speech-1.0.13/LICENSE
+-rw-rw-rw-   0        0        0     3669 2023-04-24 08:07:57.256776 img2speech-1.0.13/PKG-INFO
+-rw-rw-rw-   0        0        0     3284 2023-04-22 14:21:01.000000 img2speech-1.0.13/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 08:07:57.213981 img2speech-1.0.13/img2speech/
+drwxrwxrwx   0        0        0        0 2023-04-24 08:07:57.246451 img2speech-1.0.13/img2speech/src/
+drwxrwxrwx   0        0        0        0 2023-04-24 08:07:57.242471 img2speech-1.0.13/img2speech/src/img2speech.egg-info/
+-rw-rw-rw-   0        0        0     3669 2023-04-24 08:07:56.000000 img2speech-1.0.13/img2speech/src/img2speech.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      543 2023-04-24 08:07:57.000000 img2speech-1.0.13/img2speech/src/img2speech.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 08:07:56.000000 img2speech-1.0.13/img2speech/src/img2speech.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-04-24 08:07:56.000000 img2speech-1.0.13/img2speech/src/img2speech.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-24 08:07:56.000000 img2speech-1.0.13/img2speech/src/img2speech.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4495 2023-04-24 08:01:36.000000 img2speech-1.0.13/img2speech/src/img2speech.py
+-rw-rw-rw-   0        0        0       42 2023-04-24 08:07:57.258624 img2speech-1.0.13/setup.cfg
+-rw-rw-rw-   0        0        0     1196 2023-04-24 08:07:51.000000 img2speech-1.0.13/setup.py
```

### Comparing `img2speech-0.0.1/LICENSE` & `img2speech-1.0.13/LICENSE`

 * *Files identical despite different names*

### Comparing `img2speech-0.0.1/PKG-INFO` & `img2speech-1.0.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: img2speech
-Version: 0.0.1
+Version: 1.0.13
 Summary: Integrated Python package for converting Image to speech
 Author: Shreyas P J
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `img2speech-0.0.1/README.md` & `img2speech-1.0.13/README.md`

 * *Files identical despite different names*

### Comparing `img2speech-0.0.1/img2speech/src/img2speech.egg-info/PKG-INFO` & `img2speech-1.0.13/img2speech/src/img2speech.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: img2speech
-Version: 0.0.1
+Version: 1.0.13
 Summary: Integrated Python package for converting Image to speech
 Author: Shreyas P J
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `img2speech-0.0.1/img2speech/src/img2speech.py` & `img2speech-1.0.13/img2speech/src/img2speech.py`

 * *Files identical despite different names*

### Comparing `img2speech-0.0.1/setup.py` & `img2speech-1.0.13/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="img2speech",  # This is the name of the package
-    version="0.0.1",  # The initial release version
+    version="1.0.13",  # The initial release version
     author="Shreyas P J",  # Full name of the author
     description="Integrated Python package for converting Image to speech",
     long_description=long_description,  # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),  # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
```


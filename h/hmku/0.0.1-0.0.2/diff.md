# Comparing `tmp/hmku-0.0.1.tar.gz` & `tmp/hmku-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmku-0.0.1.tar", last modified: Mon Apr 24 15:58:19 2023, max compression
+gzip compressed data, was "hmku-0.0.2.tar", last modified: Mon Apr 24 16:19:02 2023, max compression
```

## Comparing `hmku-0.0.1.tar` & `hmku-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 15:58:19.629424 hmku-0.0.1/
--rw-rw-rw-   0        0        0      318 2023-04-24 15:58:19.628424 hmku-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-24 15:58:19.618429 hmku-0.0.1/example_pkg/
--rw-rw-rw-   0        0        0       22 2023-04-24 15:47:04.000000 hmku-0.0.1/example_pkg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:58:19.626423 hmku-0.0.1/hmku.egg-info/
--rw-rw-rw-   0        0        0      318 2023-04-24 15:58:19.000000 hmku-0.0.1/hmku.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      171 2023-04-24 15:58:19.000000 hmku-0.0.1/hmku.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 15:58:19.000000 hmku-0.0.1/hmku.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-04-24 15:58:19.000000 hmku-0.0.1/hmku.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-24 15:58:19.000000 hmku-0.0.1/hmku.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 15:58:19.629424 hmku-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      858 2023-04-24 15:56:15.000000 hmku-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 16:19:02.026263 hmku-0.0.2/
+-rw-rw-rw-   0        0        0      318 2023-04-24 16:19:02.025263 hmku-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-24 16:15:23.000000 hmku-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 16:19:02.016260 hmku-0.0.2/example_pkg/
+-rw-rw-rw-   0        0        0       15 2023-04-24 16:16:27.000000 hmku-0.0.2/example_pkg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 16:19:02.024263 hmku-0.0.2/hmku.egg-info/
+-rw-rw-rw-   0        0        0      318 2023-04-24 16:19:01.000000 hmku-0.0.2/hmku.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      181 2023-04-24 16:19:01.000000 hmku-0.0.2/hmku.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 16:19:01.000000 hmku-0.0.2/hmku.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-04-24 16:19:01.000000 hmku-0.0.2/hmku.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-24 16:19:01.000000 hmku-0.0.2/hmku.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 16:19:02.026263 hmku-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      875 2023-04-24 16:18:25.000000 hmku-0.0.2/setup.py
```

### Comparing `hmku-0.0.1/setup.py` & `hmku-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import setuptools
+from demo import main
 
-# with open("README.md", "r") as fh:
-#     long_description = fh.read()
+with open("README.md", "r") as fh:
+    long_description = fh.read()
 
 setuptools.setup(
     name="hmku",
-    version="0.0.1",
+    version="0.0.2",
     author="Yuki",
     author_email="3026408975@qq.com",
     description="Collect manga from the Korean Manga Library and download them locally",
-    # long_description=long_description,
+    long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         # "License :: OSI Approved :: MIT License",
         # "Operating System :: OS Independent",
```


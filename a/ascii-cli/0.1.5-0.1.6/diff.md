# Comparing `tmp/ascii-cli-0.1.5.tar.gz` & `tmp/ascii-cli-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ascii-cli-0.1.5.tar", last modified: Mon Apr 24 13:31:30 2023, max compression
+gzip compressed data, was "ascii-cli-0.1.6.tar", last modified: Mon Apr 24 13:39:03 2023, max compression
```

## Comparing `ascii-cli-0.1.5.tar` & `ascii-cli-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 13:31:30.130626 ascii-cli-0.1.5/
--rw-rw-rw-   0        0        0     1088 2023-04-19 10:43:59.000000 ascii-cli-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     2541 2023-04-24 13:31:30.128626 ascii-cli-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2044 2023-04-24 03:40:48.000000 ascii-cli-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 13:31:30.110628 ascii-cli-0.1.5/ascii_cli.egg-info/
--rw-rw-rw-   0        0        0     2541 2023-04-24 13:31:30.000000 ascii-cli-0.1.5/ascii_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2023-04-24 13:31:30.000000 ascii-cli-0.1.5/ascii_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 13:31:30.000000 ascii-cli-0.1.5/ascii_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-24 13:31:30.000000 ascii-cli-0.1.5/ascii_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-04-24 13:31:30.000000 ascii-cli-0.1.5/ascii_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-24 13:31:30.000000 ascii-cli-0.1.5/ascii_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 13:31:30.130626 ascii-cli-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      935 2023-04-24 13:30:46.000000 ascii-cli-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:31:30.117626 ascii-cli-0.1.5/src/
--rw-rw-rw-   0        0        0        0 2023-04-23 06:05:45.000000 ascii-cli-0.1.5/src/__init__.py
--rw-rw-rw-   0        0        0     1330 2023-04-24 05:53:28.000000 ascii-cli-0.1.5/src/__main__.py
--rw-rw-rw-   0        0        0     2960 2023-04-24 09:57:21.000000 ascii-cli-0.1.5/src/functions.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:31:30.126635 ascii-cli-0.1.5/tests/
--rw-rw-rw-   0        0        0        0 2023-04-24 06:31:01.000000 ascii-cli-0.1.5/tests/__init__.py
--rw-rw-rw-   0        0        0      602 2023-04-24 10:22:51.000000 ascii-cli-0.1.5/tests/random_test.py
--rw-rw-rw-   0        0        0      915 2023-04-24 10:22:43.000000 ascii-cli-0.1.5/tests/set_test.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:39:03.695766 ascii-cli-0.1.6/
+-rw-rw-rw-   0        0        0     1088 2023-04-19 10:43:59.000000 ascii-cli-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     2541 2023-04-24 13:39:03.692764 ascii-cli-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2044 2023-04-24 03:40:48.000000 ascii-cli-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 13:39:03.656767 ascii-cli-0.1.6/ascii_cli.egg-info/
+-rw-rw-rw-   0        0        0     2541 2023-04-24 13:39:03.000000 ascii-cli-0.1.6/ascii_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2023-04-24 13:39:03.000000 ascii-cli-0.1.6/ascii_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 13:39:03.000000 ascii-cli-0.1.6/ascii_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-24 13:39:03.000000 ascii-cli-0.1.6/ascii_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-04-24 13:39:03.000000 ascii-cli-0.1.6/ascii_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-24 13:39:03.000000 ascii-cli-0.1.6/ascii_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 13:39:03.695766 ascii-cli-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      935 2023-04-24 13:38:59.000000 ascii-cli-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:39:03.681764 ascii-cli-0.1.6/src/
+-rw-rw-rw-   0        0        0        0 2023-04-23 06:05:45.000000 ascii-cli-0.1.6/src/__init__.py
+-rw-rw-rw-   0        0        0     1338 2023-04-24 13:38:18.000000 ascii-cli-0.1.6/src/__main__.py
+-rw-rw-rw-   0        0        0     2960 2023-04-24 13:37:48.000000 ascii-cli-0.1.6/src/functions.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:39:03.689765 ascii-cli-0.1.6/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-24 06:31:01.000000 ascii-cli-0.1.6/tests/__init__.py
+-rw-rw-rw-   0        0        0      602 2023-04-24 10:22:51.000000 ascii-cli-0.1.6/tests/random_test.py
+-rw-rw-rw-   0        0        0      915 2023-04-24 10:22:43.000000 ascii-cli-0.1.6/tests/set_test.py
```

### Comparing `ascii-cli-0.1.5/LICENSE` & `ascii-cli-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ascii-cli-0.1.5/PKG-INFO` & `ascii-cli-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascii-cli
-Version: 0.1.5
+Version: 0.1.6
 Summary: A command-line tool that converts images to ASCII art.
 Home-page: https://github.com/mrq-andras/ascii-cli
 Author: mrq-andras
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ascii-cli-0.1.5/README.md` & `ascii-cli-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `ascii-cli-0.1.5/ascii_cli.egg-info/PKG-INFO` & `ascii-cli-0.1.6/ascii_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascii-cli
-Version: 0.1.5
+Version: 0.1.6
 Summary: A command-line tool that converts images to ASCII art.
 Home-page: https://github.com/mrq-andras/ascii-cli
 Author: mrq-andras
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ascii-cli-0.1.5/setup.py` & `ascii-cli-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="ascii-cli",
     author="mrq-andras",
-    version="0.1.5",
+    version="0.1.6",
     packages=find_packages(),
     package_data={'src': ['functions.py']},
     install_requires=["Pillow"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `ascii-cli-0.1.5/src/__main__.py` & `ascii-cli-0.1.6/src/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import argparse
-from functions import convert_to_ascii
-from functions import print_cmd
+from src.functions import convert_to_ascii
+from src.functions import print_cmd
 
 
 def arguments():
     # cmd arguments
     # define the command line arguments
     parser = argparse.ArgumentParser(
         description="Converts an image to ASCII art.")
```

### Comparing `ascii-cli-0.1.5/src/functions.py` & `ascii-cli-0.1.6/src/functions.py`

 * *Files identical despite different names*

### Comparing `ascii-cli-0.1.5/tests/random_test.py` & `ascii-cli-0.1.6/tests/random_test.py`

 * *Files identical despite different names*

### Comparing `ascii-cli-0.1.5/tests/set_test.py` & `ascii-cli-0.1.6/tests/set_test.py`

 * *Files identical despite different names*


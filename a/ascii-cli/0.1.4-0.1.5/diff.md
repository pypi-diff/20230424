# Comparing `tmp/ascii-cli-0.1.4.tar.gz` & `tmp/ascii-cli-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ascii-cli-0.1.4.tar", last modified: Mon Apr 24 02:56:17 2023, max compression
+gzip compressed data, was "ascii-cli-0.1.5.tar", last modified: Mon Apr 24 13:31:30 2023, max compression
```

## Comparing `ascii-cli-0.1.4.tar` & `ascii-cli-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 02:56:17.409306 ascii-cli-0.1.4/
--rw-rw-rw-   0        0        0     1088 2023-04-19 10:43:59.000000 ascii-cli-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     2541 2023-04-24 02:56:17.407318 ascii-cli-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2044 2023-04-24 02:50:58.000000 ascii-cli-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 02:56:17.395301 ascii-cli-0.1.4/ascii_cli.egg-info/
--rw-rw-rw-   0        0        0     2541 2023-04-24 02:56:17.000000 ascii-cli-0.1.4/ascii_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-04-24 02:56:17.000000 ascii-cli-0.1.4/ascii_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 02:56:17.000000 ascii-cli-0.1.4/ascii_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-24 02:56:17.000000 ascii-cli-0.1.4/ascii_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-04-24 02:56:17.000000 ascii-cli-0.1.4/ascii_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-24 02:56:17.000000 ascii-cli-0.1.4/ascii_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 02:56:17.409306 ascii-cli-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      930 2023-04-24 02:55:11.000000 ascii-cli-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 02:56:17.405334 ascii-cli-0.1.4/src/
--rw-rw-rw-   0        0        0        0 2023-04-23 06:05:45.000000 ascii-cli-0.1.4/src/__init__.py
--rw-rw-rw-   0        0        0     1320 2023-04-24 02:47:45.000000 ascii-cli-0.1.4/src/__main__.py
--rw-rw-rw-   0        0        0     3116 2023-04-24 02:42:00.000000 ascii-cli-0.1.4/src/func.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:31:30.130626 ascii-cli-0.1.5/
+-rw-rw-rw-   0        0        0     1088 2023-04-19 10:43:59.000000 ascii-cli-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     2541 2023-04-24 13:31:30.128626 ascii-cli-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2044 2023-04-24 03:40:48.000000 ascii-cli-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 13:31:30.110628 ascii-cli-0.1.5/ascii_cli.egg-info/
+-rw-rw-rw-   0        0        0     2541 2023-04-24 13:31:30.000000 ascii-cli-0.1.5/ascii_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2023-04-24 13:31:30.000000 ascii-cli-0.1.5/ascii_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 13:31:30.000000 ascii-cli-0.1.5/ascii_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-24 13:31:30.000000 ascii-cli-0.1.5/ascii_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-04-24 13:31:30.000000 ascii-cli-0.1.5/ascii_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-24 13:31:30.000000 ascii-cli-0.1.5/ascii_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 13:31:30.130626 ascii-cli-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      935 2023-04-24 13:30:46.000000 ascii-cli-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:31:30.117626 ascii-cli-0.1.5/src/
+-rw-rw-rw-   0        0        0        0 2023-04-23 06:05:45.000000 ascii-cli-0.1.5/src/__init__.py
+-rw-rw-rw-   0        0        0     1330 2023-04-24 05:53:28.000000 ascii-cli-0.1.5/src/__main__.py
+-rw-rw-rw-   0        0        0     2960 2023-04-24 09:57:21.000000 ascii-cli-0.1.5/src/functions.py
+drwxrwxrwx   0        0        0        0 2023-04-24 13:31:30.126635 ascii-cli-0.1.5/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-24 06:31:01.000000 ascii-cli-0.1.5/tests/__init__.py
+-rw-rw-rw-   0        0        0      602 2023-04-24 10:22:51.000000 ascii-cli-0.1.5/tests/random_test.py
+-rw-rw-rw-   0        0        0      915 2023-04-24 10:22:43.000000 ascii-cli-0.1.5/tests/set_test.py
```

### Comparing `ascii-cli-0.1.4/LICENSE` & `ascii-cli-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ascii-cli-0.1.4/PKG-INFO` & `ascii-cli-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascii-cli
-Version: 0.1.4
+Version: 0.1.5
 Summary: A command-line tool that converts images to ASCII art.
 Home-page: https://github.com/mrq-andras/ascii-cli
 Author: mrq-andras
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ascii-cli-0.1.4/README.md` & `ascii-cli-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ascii-cli-0.1.4/ascii_cli.egg-info/PKG-INFO` & `ascii-cli-0.1.5/ascii_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ascii-cli
-Version: 0.1.4
+Version: 0.1.5
 Summary: A command-line tool that converts images to ASCII art.
 Home-page: https://github.com/mrq-andras/ascii-cli
 Author: mrq-andras
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ascii-cli-0.1.4/setup.py` & `ascii-cli-0.1.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="ascii-cli",
     author="mrq-andras",
-    version="0.1.4",
+    version="0.1.5",
     packages=find_packages(),
-    package_data={'src': ['func.py']},
+    package_data={'src': ['functions.py']},
     install_requires=["Pillow"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: MIT License",
```

### Comparing `ascii-cli-0.1.4/src/__main__.py` & `ascii-cli-0.1.5/src/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import argparse
-from func import convert_to_ascii
-from func import print_cmd
+from functions import convert_to_ascii
+from functions import print_cmd
 
 
 def arguments():
     # cmd arguments
     # define the command line arguments
     parser = argparse.ArgumentParser(
         description="Converts an image to ASCII art.")
```

### Comparing `ascii-cli-0.1.4/src/func.py` & `ascii-cli-0.1.5/src/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,33 +6,27 @@
 SET1 = ['/', '!', '=', '+', '|', '#', '%', '@', '0', '1', '2', '3', '4', '5', '6', '7', '8', '9', '=', '?', '[', ']',
         '{', '}', 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z']
 SET2 = ["0", "O", "o", "8", "9", "6", "@", "&", ".", '"', ":"]
 SET3 = ["▀", "▄", "▌", "▐", "■", "◽", "◆", "►", "●", "░", "▒", "▓", "█"]
 
 
 def get_char_set(set_choice):
+
     # return character set
     if set_choice == "1":
         return SET1
     elif set_choice == "2":
         return SET2
     elif set_choice == "3":
         return SET3
     else:
-        print("Invalid character set. Please choose 1, 2, or 3.")
+        print("Error: Invalid character set. Please choose 1, 2, or 3.")
         exit()
 
 
-def pathcheck(args):
-    if not os.path.isfile(args.path):
-        print("Error: Invalid path to image.")
-    else:
-        print("Path to file is valid.")
-
-
 def randomize(args):
     CHAR_SET = get_char_set(args.set)
     # if the argument is random shuffle the character set
     if args.random:
         random.shuffle(CHAR_SET)
```


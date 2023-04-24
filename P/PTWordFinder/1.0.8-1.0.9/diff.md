# Comparing `tmp/PTWordFinder-1.0.8.tar.gz` & `tmp/PTWordFinder-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PTWordFinder-1.0.8.tar", last modified: Thu Mar 23 15:27:43 2023, max compression
+gzip compressed data, was "PTWordFinder-1.0.9.tar", last modified: Thu Mar 23 15:53:46 2023, max compression
```

## Comparing `PTWordFinder-1.0.8.tar` & `PTWordFinder-1.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:27:43.007758 PTWordFinder-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-03-23 15:27:31.000000 PTWordFinder-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-03-23 15:27:43.007758 PTWordFinder-1.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:27:43.007758 PTWordFinder-1.0.8/PTWordFinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-03-23 15:27:42.000000 PTWordFinder-1.0.8/PTWordFinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-23 15:27:43.000000 PTWordFinder-1.0.8/PTWordFinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 15:27:42.000000 PTWordFinder-1.0.8/PTWordFinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-23 15:27:42.000000 PTWordFinder-1.0.8/PTWordFinder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-23 15:27:42.000000 PTWordFinder-1.0.8/PTWordFinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-23 15:27:42.000000 PTWordFinder-1.0.8/PTWordFinder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-03-23 15:27:31.000000 PTWordFinder-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:27:43.007758 PTWordFinder-1.0.8/ptwordfinder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 15:27:31.000000 PTWordFinder-1.0.8/ptwordfinder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:27:43.007758 PTWordFinder-1.0.8/ptwordfinder/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-03-23 15:27:31.000000 PTWordFinder-1.0.8/ptwordfinder/commands/PTWordFinder.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-23 15:27:31.000000 PTWordFinder-1.0.8/ptwordfinder/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-23 15:27:31.000000 PTWordFinder-1.0.8/ptwordfinder/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-03-23 15:27:31.000000 PTWordFinder-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 15:27:43.007758 PTWordFinder-1.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:27:43.007758 PTWordFinder-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-03-23 15:27:31.000000 PTWordFinder-1.0.8/tests/test_PTWordFinder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:53:46.729593 PTWordFinder-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-03-23 15:53:28.000000 PTWordFinder-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-03-23 15:53:46.729593 PTWordFinder-1.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:53:46.725593 PTWordFinder-1.0.9/PTWordFinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-03-23 15:53:46.000000 PTWordFinder-1.0.9/PTWordFinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-23 15:53:46.000000 PTWordFinder-1.0.9/PTWordFinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 15:53:46.000000 PTWordFinder-1.0.9/PTWordFinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-23 15:53:46.000000 PTWordFinder-1.0.9/PTWordFinder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-23 15:53:46.000000 PTWordFinder-1.0.9/PTWordFinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-23 15:53:46.000000 PTWordFinder-1.0.9/PTWordFinder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-23 15:53:28.000000 PTWordFinder-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:53:46.725593 PTWordFinder-1.0.9/ptwordfinder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 15:53:28.000000 PTWordFinder-1.0.9/ptwordfinder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:53:46.725593 PTWordFinder-1.0.9/ptwordfinder/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-03-23 15:53:28.000000 PTWordFinder-1.0.9/ptwordfinder/commands/PTWordFinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-23 15:53:28.000000 PTWordFinder-1.0.9/ptwordfinder/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-23 15:53:28.000000 PTWordFinder-1.0.9/ptwordfinder/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-03-23 15:53:28.000000 PTWordFinder-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 15:53:46.729593 PTWordFinder-1.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 15:53:46.725593 PTWordFinder-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-03-23 15:53:28.000000 PTWordFinder-1.0.9/tests/test_PTWordFinder.py
```

### Comparing `PTWordFinder-1.0.8/LICENSE` & `PTWordFinder-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PTWordFinder-1.0.8/PKG-INFO` & `PTWordFinder-1.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PTWordFinder
-Version: 1.0.8
+Version: 1.0.9
 Summary: A command line tool that help to find specific words from a file  in any selected file.
 Author: DarekRepos
 License: MIT License
         
         Copyright (c) 2022 DarekRepos
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,22 +42,26 @@
 ## how to use
 you can installl this cmd tool from pip:.py
 ```
     pip install PTWordFinder
 ```
 Usage: ptwordf calculate-words WORDS_INPUT_FILE SEARCHED_FILE
 
-where:
+<strong>where:</strong>
+
 WORDS_INPUT_FILE - is path to input file (.txt) that contain searched words 
+
 SEARCHED_FILE - is path to file that program search for a specific word
 
 Try 'ptwordf --help' for help
 
-examples:
+<strong>examples:</strong>
+
  ptwordf calculate-words words-list.txt test-file.txt
+
  ptwordf calculate-words srcfolder/words-list.csv newfolder/test-file.csv
 
 ## Features
 - [x] lines counter
 - [x] a specific word counter
 - [x] tracking the script execution time
 - [x] support csv files
```

### Comparing `PTWordFinder-1.0.8/PTWordFinder.egg-info/PKG-INFO` & `PTWordFinder-1.0.9/PTWordFinder.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PTWordFinder
-Version: 1.0.8
+Version: 1.0.9
 Summary: A command line tool that help to find specific words from a file  in any selected file.
 Author: DarekRepos
 License: MIT License
         
         Copyright (c) 2022 DarekRepos
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,22 +42,26 @@
 ## how to use
 you can installl this cmd tool from pip:.py
 ```
     pip install PTWordFinder
 ```
 Usage: ptwordf calculate-words WORDS_INPUT_FILE SEARCHED_FILE
 
-where:
+<strong>where:</strong>
+
 WORDS_INPUT_FILE - is path to input file (.txt) that contain searched words 
+
 SEARCHED_FILE - is path to file that program search for a specific word
 
 Try 'ptwordf --help' for help
 
-examples:
+<strong>examples:</strong>
+
  ptwordf calculate-words words-list.txt test-file.txt
+
  ptwordf calculate-words srcfolder/words-list.csv newfolder/test-file.csv
 
 ## Features
 - [x] lines counter
 - [x] a specific word counter
 - [x] tracking the script execution time
 - [x] support csv files
```

### Comparing `PTWordFinder-1.0.8/README.md` & `PTWordFinder-1.0.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -11,22 +11,26 @@
 ## how to use
 you can installl this cmd tool from pip:.py
 ```
     pip install PTWordFinder
 ```
 Usage: ptwordf calculate-words WORDS_INPUT_FILE SEARCHED_FILE
 
-where:
+<strong>where:</strong>
+
 WORDS_INPUT_FILE - is path to input file (.txt) that contain searched words 
+
 SEARCHED_FILE - is path to file that program search for a specific word
 
 Try 'ptwordf --help' for help
 
-examples:
+<strong>examples:</strong>
+
  ptwordf calculate-words words-list.txt test-file.txt
+
  ptwordf calculate-words srcfolder/words-list.csv newfolder/test-file.csv
 
 ## Features
 - [x] lines counter
 - [x] a specific word counter
 - [x] tracking the script execution time
 - [x] support csv files
```

### Comparing `PTWordFinder-1.0.8/ptwordfinder/commands/PTWordFinder.py` & `PTWordFinder-1.0.9/ptwordfinder/commands/PTWordFinder.py`

 * *Files identical despite different names*

### Comparing `PTWordFinder-1.0.8/pyproject.toml` & `PTWordFinder-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "PTWordFinder"
-version = "1.0.8"
+version = "1.0.9"
 description = "A command line tool that help to find specific words from a file  in any selected file." 
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [
     { name = "DarekRepos" }
 ]
```

### Comparing `PTWordFinder-1.0.8/tests/test_PTWordFinder.py` & `PTWordFinder-1.0.9/tests/test_PTWordFinder.py`

 * *Files identical despite different names*


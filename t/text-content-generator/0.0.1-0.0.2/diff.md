# Comparing `tmp/text_content_generator-0.0.1.tar.gz` & `tmp/text_content_generator-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text_content_generator-0.0.1.tar", last modified: Mon Apr 24 08:10:16 2023, max compression
+gzip compressed data, was "text_content_generator-0.0.2.tar", last modified: Mon Apr 24 08:18:49 2023, max compression
```

## Comparing `text_content_generator-0.0.1.tar` & `text_content_generator-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 zerefhesh   (501) staff       (20)        0 2023-04-24 08:10:16.698219 text_content_generator-0.0.1/
--rw-r--r--   0 zerefhesh   (501) staff       (20)     1073 2023-04-24 06:11:14.000000 text_content_generator-0.0.1/LICENSE
--rw-r--r--   0 zerefhesh   (501) staff       (20)     1337 2023-04-24 08:10:16.698086 text_content_generator-0.0.1/PKG-INFO
--rw-r--r--   0 zerefhesh   (501) staff       (20)      852 2023-04-24 07:30:43.000000 text_content_generator-0.0.1/README.md
--rw-r--r--   0 zerefhesh   (501) staff       (20)      637 2023-04-24 08:10:09.000000 text_content_generator-0.0.1/pyproject.toml
--rw-r--r--   0 zerefhesh   (501) staff       (20)       38 2023-04-24 08:10:16.698258 text_content_generator-0.0.1/setup.cfg
-drwxr-xr-x   0 zerefhesh   (501) staff       (20)        0 2023-04-24 08:10:16.694838 text_content_generator-0.0.1/src/
-drwxr-xr-x   0 zerefhesh   (501) staff       (20)        0 2023-04-24 08:10:16.697332 text_content_generator-0.0.1/src/text_content_generator/
--rw-r--r--   0 zerefhesh   (501) staff       (20)        0 2023-04-24 08:01:24.000000 text_content_generator-0.0.1/src/text_content_generator/__init__.py
--rw-r--r--   0 zerefhesh   (501) staff       (20)      620 2023-04-24 06:26:41.000000 text_content_generator-0.0.1/src/text_content_generator/audio.py
--rw-r--r--   0 zerefhesh   (501) staff       (20)     2756 2023-04-24 07:56:44.000000 text_content_generator-0.0.1/src/text_content_generator/generate.py
--rw-r--r--   0 zerefhesh   (501) staff       (20)      513 2023-04-24 06:26:41.000000 text_content_generator-0.0.1/src/text_content_generator/pdf.py
--rw-r--r--   0 zerefhesh   (501) staff       (20)     1950 2023-04-24 06:30:20.000000 text_content_generator-0.0.1/src/text_content_generator/summarize.py
--rw-r--r--   0 zerefhesh   (501) staff       (20)      489 2023-04-24 06:26:41.000000 text_content_generator-0.0.1/src/text_content_generator/webpage.py
--rw-r--r--   0 zerefhesh   (501) staff       (20)     1456 2023-04-24 06:26:41.000000 text_content_generator-0.0.1/src/text_content_generator/youtube.py
-drwxr-xr-x   0 zerefhesh   (501) staff       (20)        0 2023-04-24 08:10:16.697898 text_content_generator-0.0.1/src/text_content_generator.egg-info/
--rw-r--r--   0 zerefhesh   (501) staff       (20)     1337 2023-04-24 08:10:16.000000 text_content_generator-0.0.1/src/text_content_generator.egg-info/PKG-INFO
--rw-r--r--   0 zerefhesh   (501) staff       (20)      496 2023-04-24 08:10:16.000000 text_content_generator-0.0.1/src/text_content_generator.egg-info/SOURCES.txt
--rw-r--r--   0 zerefhesh   (501) staff       (20)        1 2023-04-24 08:10:16.000000 text_content_generator-0.0.1/src/text_content_generator.egg-info/dependency_links.txt
--rw-r--r--   0 zerefhesh   (501) staff       (20)       23 2023-04-24 08:10:16.000000 text_content_generator-0.0.1/src/text_content_generator.egg-info/top_level.txt
+drwxr-xr-x   0 zerefhesh   (501) staff       (20)        0 2023-04-24 08:18:49.980648 text_content_generator-0.0.2/
+-rw-r--r--   0 zerefhesh   (501) staff       (20)     1073 2023-04-24 06:11:14.000000 text_content_generator-0.0.2/LICENSE
+-rw-r--r--   0 zerefhesh   (501) staff       (20)     1337 2023-04-24 08:18:49.980527 text_content_generator-0.0.2/PKG-INFO
+-rw-r--r--   0 zerefhesh   (501) staff       (20)      852 2023-04-24 07:30:43.000000 text_content_generator-0.0.2/README.md
+-rw-r--r--   0 zerefhesh   (501) staff       (20)      637 2023-04-24 08:18:45.000000 text_content_generator-0.0.2/pyproject.toml
+-rw-r--r--   0 zerefhesh   (501) staff       (20)       38 2023-04-24 08:18:49.980685 text_content_generator-0.0.2/setup.cfg
+drwxr-xr-x   0 zerefhesh   (501) staff       (20)        0 2023-04-24 08:18:49.977583 text_content_generator-0.0.2/src/
+drwxr-xr-x   0 zerefhesh   (501) staff       (20)        0 2023-04-24 08:18:49.979797 text_content_generator-0.0.2/src/text_content_generator/
+-rw-r--r--   0 zerefhesh   (501) staff       (20)        0 2023-04-24 08:01:24.000000 text_content_generator-0.0.2/src/text_content_generator/__init__.py
+-rw-r--r--   0 zerefhesh   (501) staff       (20)      620 2023-04-24 06:26:41.000000 text_content_generator-0.0.2/src/text_content_generator/audio.py
+-rw-r--r--   0 zerefhesh   (501) staff       (20)     2729 2023-04-24 08:18:17.000000 text_content_generator-0.0.2/src/text_content_generator/generate.py
+-rw-r--r--   0 zerefhesh   (501) staff       (20)      513 2023-04-24 06:26:41.000000 text_content_generator-0.0.2/src/text_content_generator/pdf.py
+-rw-r--r--   0 zerefhesh   (501) staff       (20)     1950 2023-04-24 06:30:20.000000 text_content_generator-0.0.2/src/text_content_generator/summarize.py
+-rw-r--r--   0 zerefhesh   (501) staff       (20)      489 2023-04-24 06:26:41.000000 text_content_generator-0.0.2/src/text_content_generator/webpage.py
+-rw-r--r--   0 zerefhesh   (501) staff       (20)     1456 2023-04-24 06:26:41.000000 text_content_generator-0.0.2/src/text_content_generator/youtube.py
+drwxr-xr-x   0 zerefhesh   (501) staff       (20)        0 2023-04-24 08:18:49.980371 text_content_generator-0.0.2/src/text_content_generator.egg-info/
+-rw-r--r--   0 zerefhesh   (501) staff       (20)     1337 2023-04-24 08:18:49.000000 text_content_generator-0.0.2/src/text_content_generator.egg-info/PKG-INFO
+-rw-r--r--   0 zerefhesh   (501) staff       (20)      496 2023-04-24 08:18:49.000000 text_content_generator-0.0.2/src/text_content_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 zerefhesh   (501) staff       (20)        1 2023-04-24 08:18:49.000000 text_content_generator-0.0.2/src/text_content_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 zerefhesh   (501) staff       (20)       23 2023-04-24 08:18:49.000000 text_content_generator-0.0.2/src/text_content_generator.egg-info/top_level.txt
```

### Comparing `text_content_generator-0.0.1/LICENSE` & `text_content_generator-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `text_content_generator-0.0.1/PKG-INFO` & `text_content_generator-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text_content_generator
-Version: 0.0.1
+Version: 0.0.2
 Summary: To scrape or collect text based content from media
 Author-email: mheshze <assassinmahesh@gmail.com>
 Project-URL: Homepage, https://github.com/mheshze/TextContentGeneration.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `text_content_generator-0.0.1/README.md` & `text_content_generator-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `text_content_generator-0.0.1/pyproject.toml` & `text_content_generator-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires=["setuptools >= 61.0","wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "text_content_generator"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="mheshze", email="assassinmahesh@gmail.com" },
 ]
 description = "To scrape or collect text based content from media"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `text_content_generator-0.0.1/src/text_content_generator/audio.py` & `text_content_generator-0.0.2/src/text_content_generator/audio.py`

 * *Files identical despite different names*

### Comparing `text_content_generator-0.0.1/src/text_content_generator/generate.py` & `text_content_generator-0.0.2/src/text_content_generator/generate.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,10 +69,8 @@
 
         elif i == 0:
             print("\n---QUITING!---\n")
             break
 
         else:
             print("\nPlease enter a VALID OPTION!\n")
-    return transcript
-
-print(generate_content())
+    return transcript
```

### Comparing `text_content_generator-0.0.1/src/text_content_generator/pdf.py` & `text_content_generator-0.0.2/src/text_content_generator/pdf.py`

 * *Files identical despite different names*

### Comparing `text_content_generator-0.0.1/src/text_content_generator/summarize.py` & `text_content_generator-0.0.2/src/text_content_generator/summarize.py`

 * *Files identical despite different names*

### Comparing `text_content_generator-0.0.1/src/text_content_generator/youtube.py` & `text_content_generator-0.0.2/src/text_content_generator/youtube.py`

 * *Files identical despite different names*

### Comparing `text_content_generator-0.0.1/src/text_content_generator.egg-info/PKG-INFO` & `text_content_generator-0.0.2/src/text_content_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text-content-generator
-Version: 0.0.1
+Version: 0.0.2
 Summary: To scrape or collect text based content from media
 Author-email: mheshze <assassinmahesh@gmail.com>
 Project-URL: Homepage, https://github.com/mheshze/TextContentGeneration.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```


# Comparing `tmp/text_content_generator-0.0.2.tar.gz` & `tmp/text_content_generator-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text_content_generator-0.0.2.tar", last modified: Mon Apr 24 08:18:49 2023, max compression
+gzip compressed data, was "text_content_generator-0.0.3.tar", last modified: Mon Apr 24 08:46:50 2023, max compression
```

## Comparing `text_content_generator-0.0.2.tar` & `text_content_generator-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 zerefhesh   (501) staff       (20)        0 2023-04-24 08:18:49.980648 text_content_generator-0.0.2/
--rw-r--r--   0 zerefhesh   (501) staff       (20)     1073 2023-04-24 06:11:14.000000 text_content_generator-0.0.2/LICENSE
--rw-r--r--   0 zerefhesh   (501) staff       (20)     1337 2023-04-24 08:18:49.980527 text_content_generator-0.0.2/PKG-INFO
--rw-r--r--   0 zerefhesh   (501) staff       (20)      852 2023-04-24 07:30:43.000000 text_content_generator-0.0.2/README.md
--rw-r--r--   0 zerefhesh   (501) staff       (20)      637 2023-04-24 08:18:45.000000 text_content_generator-0.0.2/pyproject.toml
--rw-r--r--   0 zerefhesh   (501) staff       (20)       38 2023-04-24 08:18:49.980685 text_content_generator-0.0.2/setup.cfg
-drwxr-xr-x   0 zerefhesh   (501) staff       (20)        0 2023-04-24 08:18:49.977583 text_content_generator-0.0.2/src/
-drwxr-xr-x   0 zerefhesh   (501) staff       (20)        0 2023-04-24 08:18:49.979797 text_content_generator-0.0.2/src/text_content_generator/
--rw-r--r--   0 zerefhesh   (501) staff       (20)        0 2023-04-24 08:01:24.000000 text_content_generator-0.0.2/src/text_content_generator/__init__.py
--rw-r--r--   0 zerefhesh   (501) staff       (20)      620 2023-04-24 06:26:41.000000 text_content_generator-0.0.2/src/text_content_generator/audio.py
--rw-r--r--   0 zerefhesh   (501) staff       (20)     2729 2023-04-24 08:18:17.000000 text_content_generator-0.0.2/src/text_content_generator/generate.py
--rw-r--r--   0 zerefhesh   (501) staff       (20)      513 2023-04-24 06:26:41.000000 text_content_generator-0.0.2/src/text_content_generator/pdf.py
--rw-r--r--   0 zerefhesh   (501) staff       (20)     1950 2023-04-24 06:30:20.000000 text_content_generator-0.0.2/src/text_content_generator/summarize.py
--rw-r--r--   0 zerefhesh   (501) staff       (20)      489 2023-04-24 06:26:41.000000 text_content_generator-0.0.2/src/text_content_generator/webpage.py
--rw-r--r--   0 zerefhesh   (501) staff       (20)     1456 2023-04-24 06:26:41.000000 text_content_generator-0.0.2/src/text_content_generator/youtube.py
-drwxr-xr-x   0 zerefhesh   (501) staff       (20)        0 2023-04-24 08:18:49.980371 text_content_generator-0.0.2/src/text_content_generator.egg-info/
--rw-r--r--   0 zerefhesh   (501) staff       (20)     1337 2023-04-24 08:18:49.000000 text_content_generator-0.0.2/src/text_content_generator.egg-info/PKG-INFO
--rw-r--r--   0 zerefhesh   (501) staff       (20)      496 2023-04-24 08:18:49.000000 text_content_generator-0.0.2/src/text_content_generator.egg-info/SOURCES.txt
--rw-r--r--   0 zerefhesh   (501) staff       (20)        1 2023-04-24 08:18:49.000000 text_content_generator-0.0.2/src/text_content_generator.egg-info/dependency_links.txt
--rw-r--r--   0 zerefhesh   (501) staff       (20)       23 2023-04-24 08:18:49.000000 text_content_generator-0.0.2/src/text_content_generator.egg-info/top_level.txt
+drwxr-xr-x   0 zerefhesh   (501) staff       (20)        0 2023-04-24 08:46:50.997700 text_content_generator-0.0.3/
+-rw-r--r--   0 zerefhesh   (501) staff       (20)     1073 2023-04-24 06:11:14.000000 text_content_generator-0.0.3/LICENSE
+-rw-r--r--   0 zerefhesh   (501) staff       (20)     1337 2023-04-24 08:46:50.997569 text_content_generator-0.0.3/PKG-INFO
+-rw-r--r--   0 zerefhesh   (501) staff       (20)      853 2023-04-24 08:24:10.000000 text_content_generator-0.0.3/README.md
+-rw-r--r--   0 zerefhesh   (501) staff       (20)      636 2023-04-24 08:35:20.000000 text_content_generator-0.0.3/pyproject.toml
+-rw-r--r--   0 zerefhesh   (501) staff       (20)       38 2023-04-24 08:46:50.997736 text_content_generator-0.0.3/setup.cfg
+drwxr-xr-x   0 zerefhesh   (501) staff       (20)        0 2023-04-24 08:46:50.994120 text_content_generator-0.0.3/src/
+drwxr-xr-x   0 zerefhesh   (501) staff       (20)        0 2023-04-24 08:46:50.996677 text_content_generator-0.0.3/src/text_content_generator/
+-rw-r--r--   0 zerefhesh   (501) staff       (20)        0 2023-04-24 08:01:24.000000 text_content_generator-0.0.3/src/text_content_generator/__init__.py
+-rw-r--r--   0 zerefhesh   (501) staff       (20)      620 2023-04-24 06:26:41.000000 text_content_generator-0.0.3/src/text_content_generator/audio.py
+-rw-r--r--   0 zerefhesh   (501) staff       (20)     2729 2023-04-24 08:18:17.000000 text_content_generator-0.0.3/src/text_content_generator/generate.py
+-rw-r--r--   0 zerefhesh   (501) staff       (20)      513 2023-04-24 06:26:41.000000 text_content_generator-0.0.3/src/text_content_generator/pdf.py
+-rw-r--r--   0 zerefhesh   (501) staff       (20)     1950 2023-04-24 06:30:20.000000 text_content_generator-0.0.3/src/text_content_generator/summarize.py
+-rw-r--r--   0 zerefhesh   (501) staff       (20)      489 2023-04-24 06:26:41.000000 text_content_generator-0.0.3/src/text_content_generator/webpage.py
+-rw-r--r--   0 zerefhesh   (501) staff       (20)     1456 2023-04-24 06:26:41.000000 text_content_generator-0.0.3/src/text_content_generator/youtube.py
+drwxr-xr-x   0 zerefhesh   (501) staff       (20)        0 2023-04-24 08:46:50.997372 text_content_generator-0.0.3/src/text_content_generator.egg-info/
+-rw-r--r--   0 zerefhesh   (501) staff       (20)     1337 2023-04-24 08:46:50.000000 text_content_generator-0.0.3/src/text_content_generator.egg-info/PKG-INFO
+-rw-r--r--   0 zerefhesh   (501) staff       (20)      496 2023-04-24 08:46:50.000000 text_content_generator-0.0.3/src/text_content_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 zerefhesh   (501) staff       (20)        1 2023-04-24 08:46:50.000000 text_content_generator-0.0.3/src/text_content_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 zerefhesh   (501) staff       (20)       23 2023-04-24 08:46:50.000000 text_content_generator-0.0.3/src/text_content_generator.egg-info/top_level.txt
```

### Comparing `text_content_generator-0.0.2/LICENSE` & `text_content_generator-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `text_content_generator-0.0.2/PKG-INFO` & `text_content_generator-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: text_content_generator
-Version: 0.0.2
+Version: 0.0.3
 Summary: To scrape or collect text based content from media
 Author-email: mheshze <assassinmahesh@gmail.com>
 Project-URL: Homepage, https://github.com/mheshze/TextContentGeneration.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TextContentGeneration
 Generates Text Content from various sources such as YouTube Videos, Local Audio/Video Files, Webpages and PDF's.
 
-Use the **_text_content_generation.generate()_** function to generate content from
+##  Imports
+
+Use the **_tcg.generate_content()_** function to generate content from
 four sources:
 1. PDFS
 2. Web Pages
 3. YouTube Video Transcripts
 4. Local Audio/Video Files
 
 You can also individual modules if you need only specific functionality.
```

### Comparing `text_content_generator-0.0.2/README.md` & `text_content_generator-0.0.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # TextContentGeneration
 Generates Text Content from various sources such as YouTube Videos, Local Audio/Video Files, Webpages and PDF's.
 
-Use the **_text_content_generation.generate()_** function to generate content from
+##  Imports
+
+Use the **_tcg.generate_content()_** function to generate content from
 four sources:
 1. PDFS
 2. Web Pages
 3. YouTube Video Transcripts
 4. Local Audio/Video Files
 
 You can also individual modules if you need only specific functionality.
```

### Comparing `text_content_generator-0.0.2/pyproject.toml` & `text_content_generator-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires=["setuptools >= 61.0","wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "text_content_generator"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="mheshze", email="assassinmahesh@gmail.com" },
 ]
 description = "To scrape or collect text based content from media"
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `text_content_generator-0.0.2/src/text_content_generator/audio.py` & `text_content_generator-0.0.3/src/text_content_generator/audio.py`

 * *Files identical despite different names*

### Comparing `text_content_generator-0.0.2/src/text_content_generator/generate.py` & `text_content_generator-0.0.3/src/text_content_generator/generate.py`

 * *Files identical despite different names*

### Comparing `text_content_generator-0.0.2/src/text_content_generator/pdf.py` & `text_content_generator-0.0.3/src/text_content_generator/pdf.py`

 * *Files identical despite different names*

### Comparing `text_content_generator-0.0.2/src/text_content_generator/summarize.py` & `text_content_generator-0.0.3/src/text_content_generator/summarize.py`

 * *Files identical despite different names*

### Comparing `text_content_generator-0.0.2/src/text_content_generator/youtube.py` & `text_content_generator-0.0.3/src/text_content_generator/youtube.py`

 * *Files identical despite different names*

### Comparing `text_content_generator-0.0.2/src/text_content_generator.egg-info/PKG-INFO` & `text_content_generator-0.0.3/src/text_content_generator.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: text-content-generator
-Version: 0.0.2
+Version: 0.0.3
 Summary: To scrape or collect text based content from media
 Author-email: mheshze <assassinmahesh@gmail.com>
 Project-URL: Homepage, https://github.com/mheshze/TextContentGeneration.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TextContentGeneration
 Generates Text Content from various sources such as YouTube Videos, Local Audio/Video Files, Webpages and PDF's.
 
-Use the **_text_content_generation.generate()_** function to generate content from
+##  Imports
+
+Use the **_tcg.generate_content()_** function to generate content from
 four sources:
 1. PDFS
 2. Web Pages
 3. YouTube Video Transcripts
 4. Local Audio/Video Files
 
 You can also individual modules if you need only specific functionality.
```


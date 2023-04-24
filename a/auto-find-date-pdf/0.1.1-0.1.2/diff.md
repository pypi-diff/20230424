# Comparing `tmp/auto_find_date_pdf-0.1.1.tar.gz` & `tmp/auto_find_date_pdf-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_find_date_pdf-0.1.1.tar", last modified: Mon Apr 24 01:29:26 2023, max compression
+gzip compressed data, was "auto_find_date_pdf-0.1.2.tar", last modified: Mon Apr 24 03:02:49 2023, max compression
```

## Comparing `auto_find_date_pdf-0.1.1.tar` & `auto_find_date_pdf-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 01:29:26.217960 auto_find_date_pdf-0.1.1/
--rw-rw-rw-   0        0        0     1092 2023-04-23 05:51:11.000000 auto_find_date_pdf-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      212 2023-04-24 01:29:26.217960 auto_find_date_pdf-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-24 01:29:26.217960 auto_find_date_pdf-0.1.1/auto_find_date_pdf.egg-info/
--rw-rw-rw-   0        0        0      212 2023-04-24 01:29:26.000000 auto_find_date_pdf-0.1.1/auto_find_date_pdf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-04-24 01:29:26.000000 auto_find_date_pdf-0.1.1/auto_find_date_pdf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 01:29:26.000000 auto_find_date_pdf-0.1.1/auto_find_date_pdf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-24 01:29:26.000000 auto_find_date_pdf-0.1.1/auto_find_date_pdf.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2023-04-24 01:29:26.000000 auto_find_date_pdf-0.1.1/auto_find_date_pdf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-24 01:29:26.000000 auto_find_date_pdf-0.1.1/auto_find_date_pdf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1320 2023-04-24 00:40:25.000000 auto_find_date_pdf-0.1.1/main.py
--rw-rw-rw-   0        0        0       42 2023-04-24 01:29:26.219463 auto_find_date_pdf-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      530 2023-04-24 01:29:15.000000 auto_find_date_pdf-0.1.1/setup.py
--rw-rw-rw-   0        0        0     5989 2023-04-24 00:48:27.000000 auto_find_date_pdf-0.1.1/text_search.py
+drwxrwxrwx   0        0        0        0 2023-04-24 03:02:49.817860 auto_find_date_pdf-0.1.2/
+-rw-rw-rw-   0        0        0     1092 2023-04-23 05:51:11.000000 auto_find_date_pdf-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      212 2023-04-24 03:02:49.817353 auto_find_date_pdf-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-24 03:02:49.816352 auto_find_date_pdf-0.1.2/auto_find_date_pdf.egg-info/
+-rw-rw-rw-   0        0        0      212 2023-04-24 03:02:49.000000 auto_find_date_pdf-0.1.2/auto_find_date_pdf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-04-24 03:02:49.000000 auto_find_date_pdf-0.1.2/auto_find_date_pdf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 03:02:49.000000 auto_find_date_pdf-0.1.2/auto_find_date_pdf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-24 03:02:49.000000 auto_find_date_pdf-0.1.2/auto_find_date_pdf.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2023-04-24 03:02:49.000000 auto_find_date_pdf-0.1.2/auto_find_date_pdf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-24 03:02:49.000000 auto_find_date_pdf-0.1.2/auto_find_date_pdf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1320 2023-04-24 00:40:25.000000 auto_find_date_pdf-0.1.2/main.py
+-rw-rw-rw-   0        0        0       42 2023-04-24 03:02:49.817860 auto_find_date_pdf-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      530 2023-04-24 03:02:35.000000 auto_find_date_pdf-0.1.2/setup.py
+-rw-rw-rw-   0        0        0     6400 2023-04-24 03:01:32.000000 auto_find_date_pdf-0.1.2/text_search.py
```

### Comparing `auto_find_date_pdf-0.1.1/LICENSE` & `auto_find_date_pdf-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_find_date_pdf-0.1.1/main.py` & `auto_find_date_pdf-0.1.2/main.py`

 * *Files identical despite different names*

### Comparing `auto_find_date_pdf-0.1.1/setup.py` & `auto_find_date_pdf-0.1.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='auto_find_date_pdf',
-    version='0.1.1',
+    version='0.1.2',
     description='A simple lib to find dates from any txt/ pdf/ rtf source',
     author='Your Name',
     packages=find_packages(),
     author_email='opensource@marvsai.com',
     py_modules=['text_search', 'main'],
     install_requires=[
         'pypdf',
```

### Comparing `auto_find_date_pdf-0.1.1/text_search.py` & `auto_find_date_pdf-0.1.2/text_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,27 @@
 import re
 from datetime import datetime, timedelta
 from re import Pattern
 from pypdf import PdfReader
 from typing import Callable
 
 
-def extract_rtf_pdf(name: str, get_ai_text:Callable=None):
+def supported_images(imgname:str)->bool:
+    strings = ["JPEG", "PNG8", "PNG24", "GIF", "GIF", "BMP", "WEBP",
+               "TIFF"]
+
+    endI = imgname.rfind('.')
+    if endI<0:
+        return False
+    if imgname[endI+1:].upper() in strings:
+        return True
+    return False
+
+
+def extract_rtf_pdf(name: str, get_ai_text:Callable=None)->str:
     text = ''
     if name[-3:].find('rt')>-1:
         from striprtf.striprtf import rtf_to_text
         with open(name, 'r') as doc:
             rtf_data = doc.read()
             text = rtf_to_text(rtf_data, errors='ignore')
     elif name[-3:].lower().find('pdf')>-1:
@@ -24,14 +36,18 @@
                 pdf_reader = PdfReader(f)
                 # Get the number of pages in the PDF document
                 num_pages = pdf_reader.pages
                 # Loop over each page in the PDF document
                 for page_num in num_pages:
                     # Extract the text from the page
                     text += page_num.extract_text()
+        elif supported_images(name):
+            if get_ai_text:
+                text = get_ai_text(name)
+
     return text
 
 
 date_dash_pattern = re.compile(r'\d{1,2}-\w{3}-\d{4}')
 date_pattern_gen = re.compile(r'\d{1,2}[/-]\d{1,2}[/-]\d{2,4}')
```


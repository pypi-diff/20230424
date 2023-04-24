# Comparing `tmp/auto_find_date_pdf-0.1.21.tar.gz` & `tmp/auto_find_date_pdf-0.1.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_find_date_pdf-0.1.21.tar", last modified: Mon Apr 24 03:08:58 2023, max compression
+gzip compressed data, was "auto_find_date_pdf-0.1.22.tar", last modified: Mon Apr 24 03:27:05 2023, max compression
```

## Comparing `auto_find_date_pdf-0.1.21.tar` & `auto_find_date_pdf-0.1.22.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 03:08:58.244335 auto_find_date_pdf-0.1.21/
--rw-rw-rw-   0        0        0     1092 2023-04-23 05:51:11.000000 auto_find_date_pdf-0.1.21/LICENSE
--rw-rw-rw-   0        0        0      213 2023-04-24 03:08:58.244335 auto_find_date_pdf-0.1.21/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-24 03:08:58.243330 auto_find_date_pdf-0.1.21/auto_find_date_pdf.egg-info/
--rw-rw-rw-   0        0        0      213 2023-04-24 03:08:58.000000 auto_find_date_pdf-0.1.21/auto_find_date_pdf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-04-24 03:08:58.000000 auto_find_date_pdf-0.1.21/auto_find_date_pdf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 03:08:58.000000 auto_find_date_pdf-0.1.21/auto_find_date_pdf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-24 03:08:58.000000 auto_find_date_pdf-0.1.21/auto_find_date_pdf.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2023-04-24 03:08:58.000000 auto_find_date_pdf-0.1.21/auto_find_date_pdf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-24 03:08:58.000000 auto_find_date_pdf-0.1.21/auto_find_date_pdf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1320 2023-04-24 00:40:25.000000 auto_find_date_pdf-0.1.21/main.py
--rw-rw-rw-   0        0        0       42 2023-04-24 03:08:58.244335 auto_find_date_pdf-0.1.21/setup.cfg
--rw-rw-rw-   0        0        0      531 2023-04-24 03:08:44.000000 auto_find_date_pdf-0.1.21/setup.py
--rw-rw-rw-   0        0        0     6413 2023-04-24 03:08:09.000000 auto_find_date_pdf-0.1.21/text_search.py
+drwxrwxrwx   0        0        0        0 2023-04-24 03:27:05.757635 auto_find_date_pdf-0.1.22/
+-rw-rw-rw-   0        0        0     1092 2023-04-23 05:51:11.000000 auto_find_date_pdf-0.1.22/LICENSE
+-rw-rw-rw-   0        0        0      236 2023-04-24 03:27:05.756637 auto_find_date_pdf-0.1.22/PKG-INFO
+-rw-rw-rw-   0        0        0      501 2023-04-24 03:26:39.000000 auto_find_date_pdf-0.1.22/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 03:27:05.756637 auto_find_date_pdf-0.1.22/auto_find_date_pdf.egg-info/
+-rw-rw-rw-   0        0        0      236 2023-04-24 03:27:05.000000 auto_find_date_pdf-0.1.22/auto_find_date_pdf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-04-24 03:27:05.000000 auto_find_date_pdf-0.1.22/auto_find_date_pdf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 03:27:05.000000 auto_find_date_pdf-0.1.22/auto_find_date_pdf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-24 03:27:05.000000 auto_find_date_pdf-0.1.22/auto_find_date_pdf.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2023-04-24 03:27:05.000000 auto_find_date_pdf-0.1.22/auto_find_date_pdf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-24 03:27:05.000000 auto_find_date_pdf-0.1.22/auto_find_date_pdf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      921 2023-04-24 03:26:48.000000 auto_find_date_pdf-0.1.22/main.py
+-rw-rw-rw-   0        0        0       42 2023-04-24 03:27:05.757635 auto_find_date_pdf-0.1.22/setup.cfg
+-rw-rw-rw-   0        0        0      554 2023-04-24 03:26:54.000000 auto_find_date_pdf-0.1.22/setup.py
+-rw-rw-rw-   0        0        0     6858 2023-04-24 03:24:11.000000 auto_find_date_pdf-0.1.22/text_search.py
```

### Comparing `auto_find_date_pdf-0.1.21/LICENSE` & `auto_find_date_pdf-0.1.22/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_find_date_pdf-0.1.21/text_search.py` & `auto_find_date_pdf-0.1.22/text_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,25 @@
         return False
     if imgname[endI+1:].upper() in strings:
         return True
     return False
 
 
 def extract_rtf_pdf(name: str, get_ai_text:Callable=None)->str:
+    """
+      Find text from pdf and rtf
+
+      Args:
+          name (str): The string in which to find any format of dates
+          get_ai_text: call back function that can call google vision api or AWS or Azure equivalents for text extraction
+          Called for images and image PDFs.
+
+      Returns:
+          List[datetime.datetime]: A list of datetime objects the latest can be found using max()
+      """
     text = ''
     if name[-3:].find('rt')>-1:
         from striprtf.striprtf import rtf_to_text
         with open(name, 'r') as doc:
             rtf_data = doc.read()
             text = rtf_to_text(rtf_data, errors='ignore')
     elif name[-3:].lower().find('pdf')>-1:
@@ -36,17 +47,17 @@
                 pdf_reader = PdfReader(f)
                 # Get the number of pages in the PDF document
                 num_pages = pdf_reader.pages
                 # Loop over each page in the PDF document
                 for page_num in num_pages:
                     # Extract the text from the page
                     text += page_num.extract_text()
-        elif supported_images(name):
-            if get_ai_text:
-                text = get_ai_text(name)
+    elif supported_images(name):
+        if get_ai_text:
+            text = get_ai_text(name)
 
     return text
 
 
 date_dash_pattern = re.compile(r'\d{1,2}-\w{3}-\d{4}')
 date_pattern_gen = re.compile(r'\d{1,2}[/-]\d{1,2}[/-]\d{2,4}')
 
@@ -76,21 +87,24 @@
                         except ValueError:
                             date = None
         if date is not None:
             dates.append(date)
 
 
 def find_dates(file_contents: str):
-    # Open the file asynchronously and read the contents
-    # async with aiofiles.open(file_path, 'r') as file:
-    #     file_contents = await file.read()
+    """
+      Find any dates in a large python string usually taken from a file or pdf
 
-    # Define a regular expression pattern to match dates
+      Args:
+          file_contents (str): The string in which to find any format of dates
 
-    # Find all matches of the pattern in the file contents
+
+      Returns:
+          List[datetime.datetime]: A list of datetime objects the latest can be found using max()
+      """
     matches = date_dash_pattern.findall(file_contents)
     # Convert the matches to datetime objects
     dates = []
     if matches:
         try:
             for match in matches:
                 date = datetime.strptime(match, '%d-%b-%Y')
```


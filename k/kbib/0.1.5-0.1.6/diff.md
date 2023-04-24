# Comparing `tmp/kbib-0.1.5.tar.gz` & `tmp/kbib-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kbib-0.1.5.tar", last modified: Wed Nov 30 08:50:51 2022, max compression
+gzip compressed data, was "kbib-0.1.6.tar", last modified: Mon Apr 24 05:27:00 2023, max compression
```

## Comparing `kbib-0.1.5.tar` & `kbib-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 08:50:51.451460 kbib-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-11-30 08:50:26.000000 kbib-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       42 2022-11-30 08:50:26.000000 kbib-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2022-11-30 08:50:51.451460 kbib-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2022-11-30 08:50:26.000000 kbib-0.1.5/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 08:50:51.447460 kbib-0.1.5/kbib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-11-30 08:50:26.000000 kbib-0.1.5/kbib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2022-11-30 08:50:26.000000 kbib-0.1.5/kbib/parseRefs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8548 2022-11-30 08:50:26.000000 kbib-0.1.5/kbib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-30 08:50:51.451460 kbib-0.1.5/kbib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2022-11-30 08:50:51.000000 kbib-0.1.5/kbib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      280 2022-11-30 08:50:51.000000 kbib-0.1.5/kbib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-30 08:50:51.000000 kbib-0.1.5/kbib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2022-11-30 08:50:51.000000 kbib-0.1.5/kbib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2022-11-30 08:50:51.000000 kbib-0.1.5/kbib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2022-11-30 08:50:51.000000 kbib-0.1.5/kbib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-30 08:50:51.000000 kbib-0.1.5/kbib.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-11-30 08:50:51.451460 kbib-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2022-11-30 08:50:26.000000 kbib-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:27:00.901289 kbib-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-24 05:26:43.000000 kbib-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-24 05:26:43.000000 kbib-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-04-24 05:27:00.901289 kbib-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-04-24 05:26:43.000000 kbib-0.1.6/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:27:00.901289 kbib-0.1.6/kbib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 05:26:43.000000 kbib-0.1.6/kbib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-24 05:26:43.000000 kbib-0.1.6/kbib/parseRefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-04-24 05:26:43.000000 kbib-0.1.6/kbib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:27:00.901289 kbib-0.1.6/kbib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-04-24 05:27:00.000000 kbib-0.1.6/kbib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-24 05:27:00.000000 kbib-0.1.6/kbib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 05:27:00.000000 kbib-0.1.6/kbib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-24 05:27:00.000000 kbib-0.1.6/kbib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-24 05:27:00.000000 kbib-0.1.6/kbib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-24 05:27:00.000000 kbib-0.1.6/kbib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 05:27:00.000000 kbib-0.1.6/kbib.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 05:27:00.901289 kbib-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-24 05:26:43.000000 kbib-0.1.6/setup.py
```

### Comparing `kbib-0.1.5/LICENSE` & `kbib-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kbib-0.1.5/PKG-INFO` & `kbib-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kbib
-Version: 0.1.5
+Version: 0.1.6
 Summary: A command line tool to get bibtex information from DOIs and PDFs
 Author: Koushik Naskar
 Author-email: koushik.naskar9@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/Koushikphy/kbib
 Keywords: bibtex references doi crossref
 Classifier: Development Status :: 5 - Production/Stable
@@ -32,14 +32,15 @@
 
 
 ### ⚡ Features
 1. Get bibtex information from DOI.
 2. Get bibtex information from article pdf.
 3. Get full list of references of an article as a .bib file.
 4. Directly rename pdf files with bibtex information.
+5. Find duplicate bib entries in bibtex files.
 
 ### 🛠️ Installation
 Download and install the latest package from the [release section](https://github.com/Koushikphy/kbib/releases/latest) or directly by pip
 ```bash
 pip install kbib
 ```
 For parsing bibtex information from PDF files, optional dependencies need to be installed
@@ -48,23 +49,24 @@
 pip install kbib['pdf']
 ```
 
 
 ### 🚀 Usage 
 Use the command line tool `kbib` as 
 ```bash
-kbib [-h] [-bib DOI] [-ref DOI] [-pdf [PDF [PDF ...]]] [-ren [PDF [PDF ...]]] [-o DOI]
+kbib [-h] [-bib DOI] [-ref DOI] [-pdf [PDF [PDF ...]]] [-ren [PDF [PDF ...]]] [-dup [BIB [BIB ...]]] [-o DOI]
 ```
 
 | Argument    |  Description|
 | ----------- | ----------- 
 |    `-bib`    | DOI to get bibtex entry |
 |    `-ref`    | DOI to get bibtex entries for all the references | 
 |    `-pdf`    | PDF file name(s) to get bibtex info | 
 |    `-ren`    | PDF file name(s) to rename with bibtex info | 
+|    `-dup`    | Bib file name(s) to find duplicates. | 
 |    `-o`      | Output bib file | 
 
 * Get bibtex from a DOI
     ```bash
     kbib -bib https://doi.org/10xxxxxx
     ```
 * Get bibtex from a DOI and store in a file 'ref.bib'
@@ -85,14 +87,18 @@
     ```
 * Rename pdf files with bibtex information
     ```bash
     kbib -ren article.pdf
     # or
     kbib -ren *.pdf
     ```
+* Find duplicate bib entries in bibtex files.
+    ```bash
+    kbib -dup article_1.bib article_2.bib
+    ```
 
 #### ⚓Limitation:
 - `kbib` parses DOI information from [Crossref API](https://github.com/CrossRef/rest-api-doc). So if the article is not indexed in Crossref database this tool will fail to get the necessary information. Also the API may temporarily block requests from an IP if a large number of queries are made within a short period of time.
 - Special/Latex characters in the title may gets messed up during the API call. One needs to be careful using title field for the bibtex created by `kbib`.
 - For bibtex keys and renaming files, `kbib` uses format as `<Short Journal Name>_<Volume>_<Year>_<Last name of first author>`, which is presently hardcoded in the tool. Therefore, one can not use any desired format through the command line.
```

### Comparing `kbib-0.1.5/Readme.md` & `kbib-0.1.6/Readme.md`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 
 ### ⚡ Features
 1. Get bibtex information from DOI.
 2. Get bibtex information from article pdf.
 3. Get full list of references of an article as a .bib file.
 4. Directly rename pdf files with bibtex information.
+5. Find duplicate bib entries in bibtex files.
 
 ### 🛠️ Installation
 Download and install the latest package from the [release section](https://github.com/Koushikphy/kbib/releases/latest) or directly by pip
 ```bash
 pip install kbib
 ```
 For parsing bibtex information from PDF files, optional dependencies need to be installed
@@ -25,23 +26,24 @@
 pip install kbib['pdf']
 ```
 
 
 ### 🚀 Usage 
 Use the command line tool `kbib` as 
 ```bash
-kbib [-h] [-bib DOI] [-ref DOI] [-pdf [PDF [PDF ...]]] [-ren [PDF [PDF ...]]] [-o DOI]
+kbib [-h] [-bib DOI] [-ref DOI] [-pdf [PDF [PDF ...]]] [-ren [PDF [PDF ...]]] [-dup [BIB [BIB ...]]] [-o DOI]
 ```
 
 | Argument    |  Description|
 | ----------- | ----------- 
 |    `-bib`    | DOI to get bibtex entry |
 |    `-ref`    | DOI to get bibtex entries for all the references | 
 |    `-pdf`    | PDF file name(s) to get bibtex info | 
 |    `-ren`    | PDF file name(s) to rename with bibtex info | 
+|    `-dup`    | Bib file name(s) to find duplicates. | 
 |    `-o`      | Output bib file | 
 
 * Get bibtex from a DOI
     ```bash
     kbib -bib https://doi.org/10xxxxxx
     ```
 * Get bibtex from a DOI and store in a file 'ref.bib'
@@ -62,14 +64,18 @@
     ```
 * Rename pdf files with bibtex information
     ```bash
     kbib -ren article.pdf
     # or
     kbib -ren *.pdf
     ```
+* Find duplicate bib entries in bibtex files.
+    ```bash
+    kbib -dup article_1.bib article_2.bib
+    ```
 
 #### ⚓Limitation:
 - `kbib` parses DOI information from [Crossref API](https://github.com/CrossRef/rest-api-doc). So if the article is not indexed in Crossref database this tool will fail to get the necessary information. Also the API may temporarily block requests from an IP if a large number of queries are made within a short period of time.
 - Special/Latex characters in the title may gets messed up during the API call. One needs to be careful using title field for the bibtex created by `kbib`.
 - For bibtex keys and renaming files, `kbib` uses format as `<Short Journal Name>_<Volume>_<Year>_<Last name of first author>`, which is presently hardcoded in the tool. Therefore, one can not use any desired format through the command line.
```

### Comparing `kbib-0.1.5/kbib/parseRefs.py` & `kbib-0.1.6/kbib/parseRefs.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from kbib.utils import (
     CustomParser,
     RawTextHelpFormatter,
     get_bib,
     reconfigureBibs,
     getFullRefList,
     pdftobib,
-    renamePDF
+    renamePDF,
+    listDuplicates
 )
 
 
 __all__ = []
 # version = '0.1.1'
 version= pkg_resources.require('kbib')[0].version
 
@@ -27,14 +28,15 @@
     )
 
     #adding options for numerical jobs
     parser.add_argument('-bib', type=str, help="DOI to get bibtex entry", metavar="DOI")
     parser.add_argument('-ref', type=str, help="DOI to get bibtex entries for all the references", metavar="DOI")
     parser.add_argument('-pdf', type=str, help="PDF file name(s) to get bibtex info", metavar="PDF", nargs='*')
     parser.add_argument('-ren', type=str, help="PDF file name(s) to rename with bibtex info", metavar="PDF", nargs='*')
+    parser.add_argument('-dup', type=str, help="Bib file name(s) to find duplicates.", metavar="BIB", nargs='*')
     parser.add_argument('-o',   type=str, help="Output bib file", metavar="FILE")
 
     return parser
 
 
 
 
@@ -79,14 +81,17 @@
 
         if args.pdf:
             bibs = pdftobib(args.pdf)
             writeBib(bibs,args.o)
 
         if args.ren:
             renamePDF(args.ren)
+        
+        if args.dup:
+            listDuplicates(args.dup)
 
     except AssertionError as e:
         print(e)
 
     except:
         print("Unable to parse bibtex information.")
         # raise
```

### Comparing `kbib-0.1.5/kbib/utils.py` & `kbib-0.1.6/kbib/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     TimeRemainingColumn,
     BarColumn,
     MofNCompleteColumn
 )
 from argparse import ArgumentParser, RawTextHelpFormatter
 from datetime import timedelta
 from rich import print as rprint
+from collections import Counter
 try:
     import pdf2doi
     PDF_AVAILABLE = True
     pdf2doi.config.set('verbose',False)
 except ImportError:
     PDF_AVAILABLE = False
 
@@ -271,14 +272,38 @@
             ch = input(f"Rename {file} -> {newName}? [y/n] ")
             if ch=='y':
                 os.rename(file,newName)
 
 
 
 
+def listDuplicates(bibFiles):
+    bib_db = bibtexparser.loads('\n'.join(open(f).read() for f in bibFiles))
+    entries = bib_db.entries
+
+    # decide duplicates based on year, volume and pages. Can we make it in more sophisticated way
+    test_en = [(en.get('year',''), en.get('volume',''),en.get('pages','')) for en in entries]
+
+    duplicates = []
+    for item, count in Counter(test_en).items():
+        if count>1:
+            dupTmp = []
+            for en in entries:
+                it = (en.get('year',''), en.get('volume',''),en.get('pages',''))
+                if it==item:
+                    dupTmp.append(en.get('ID'))
+            if len(dupTmp)>1:
+                duplicates.append(dupTmp)
+
+    if len(duplicates):
+        print("The following bib entries may be duplicate. Please check:")
+        for i, item in enumerate(duplicates, start=1):
+            print(f"{i}. {' '.join(item)}")
+
+
 # progress = Progress()
 
 # progress.start()
 # task = progress.add_task("Getting references-------------",total=124)
 
 # async def get(url, session):
 #     async with session.get(url=url) as response:
```

### Comparing `kbib-0.1.5/kbib.egg-info/PKG-INFO` & `kbib-0.1.6/kbib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kbib
-Version: 0.1.5
+Version: 0.1.6
 Summary: A command line tool to get bibtex information from DOIs and PDFs
 Author: Koushik Naskar
 Author-email: koushik.naskar9@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/Koushikphy/kbib
 Keywords: bibtex references doi crossref
 Classifier: Development Status :: 5 - Production/Stable
@@ -32,14 +32,15 @@
 
 
 ### ⚡ Features
 1. Get bibtex information from DOI.
 2. Get bibtex information from article pdf.
 3. Get full list of references of an article as a .bib file.
 4. Directly rename pdf files with bibtex information.
+5. Find duplicate bib entries in bibtex files.
 
 ### 🛠️ Installation
 Download and install the latest package from the [release section](https://github.com/Koushikphy/kbib/releases/latest) or directly by pip
 ```bash
 pip install kbib
 ```
 For parsing bibtex information from PDF files, optional dependencies need to be installed
@@ -48,23 +49,24 @@
 pip install kbib['pdf']
 ```
 
 
 ### 🚀 Usage 
 Use the command line tool `kbib` as 
 ```bash
-kbib [-h] [-bib DOI] [-ref DOI] [-pdf [PDF [PDF ...]]] [-ren [PDF [PDF ...]]] [-o DOI]
+kbib [-h] [-bib DOI] [-ref DOI] [-pdf [PDF [PDF ...]]] [-ren [PDF [PDF ...]]] [-dup [BIB [BIB ...]]] [-o DOI]
 ```
 
 | Argument    |  Description|
 | ----------- | ----------- 
 |    `-bib`    | DOI to get bibtex entry |
 |    `-ref`    | DOI to get bibtex entries for all the references | 
 |    `-pdf`    | PDF file name(s) to get bibtex info | 
 |    `-ren`    | PDF file name(s) to rename with bibtex info | 
+|    `-dup`    | Bib file name(s) to find duplicates. | 
 |    `-o`      | Output bib file | 
 
 * Get bibtex from a DOI
     ```bash
     kbib -bib https://doi.org/10xxxxxx
     ```
 * Get bibtex from a DOI and store in a file 'ref.bib'
@@ -85,14 +87,18 @@
     ```
 * Rename pdf files with bibtex information
     ```bash
     kbib -ren article.pdf
     # or
     kbib -ren *.pdf
     ```
+* Find duplicate bib entries in bibtex files.
+    ```bash
+    kbib -dup article_1.bib article_2.bib
+    ```
 
 #### ⚓Limitation:
 - `kbib` parses DOI information from [Crossref API](https://github.com/CrossRef/rest-api-doc). So if the article is not indexed in Crossref database this tool will fail to get the necessary information. Also the API may temporarily block requests from an IP if a large number of queries are made within a short period of time.
 - Special/Latex characters in the title may gets messed up during the API call. One needs to be careful using title field for the bibtex created by `kbib`.
 - For bibtex keys and renaming files, `kbib` uses format as `<Short Journal Name>_<Volume>_<Year>_<Last name of first author>`, which is presently hardcoded in the tool. Therefore, one can not use any desired format through the command line.
```

### Comparing `kbib-0.1.5/setup.py` & `kbib-0.1.6/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open('Readme.md') as f:
     txt = f.read()
 
 setup(name='kbib',
-    version='0.1.5',
+    version='0.1.6',
     description='A command line tool to get bibtex information from DOIs and PDFs',
     long_description=txt,
     long_description_content_type='text/markdown',
     author='Koushik Naskar',
     author_email='koushik.naskar9@gmail.com',
     license="MIT",
     classifiers=[
```


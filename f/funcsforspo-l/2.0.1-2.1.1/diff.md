# Comparing `tmp/funcsforspo_l-2.0.1.tar.gz` & `tmp/funcsforspo_l-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcsforspo_l-2.0.1.tar", last modified: Sat Mar 25 21:02:47 2023, max compression
+gzip compressed data, was "funcsforspo_l-2.1.1.tar", last modified: Mon Apr 24 15:27:36 2023, max compression
```

## Comparing `funcsforspo_l-2.0.1.tar` & `funcsforspo_l-2.1.1.tar`

### file list

```diff
@@ -1,57 +1,59 @@
-drwxrwxrwx   0        0        0        0 2023-03-25 21:02:47.586681 funcsforspo_l-2.0.1/
--rw-rw-rw-   0        0        0     1076 2023-02-03 19:05:17.000000 funcsforspo_l-2.0.1/LICENSE
--rw-rw-rw-   0        0        0     1374 2023-03-25 21:02:47.583958 funcsforspo_l-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      935 2023-02-03 19:05:17.000000 funcsforspo_l-2.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-25 21:02:47.350081 funcsforspo_l-2.0.1/funcsforspo_l/
-drwxrwxrwx   0        0        0        0 2023-03-25 21:02:47.419312 funcsforspo_l-2.0.1/funcsforspo_l/femails/
--rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 funcsforspo_l-2.0.1/funcsforspo_l/femails/__init__.py
--rw-rw-rw-   0        0        0     7604 2023-01-19 14:03:01.000000 funcsforspo_l-2.0.1/funcsforspo_l/femails/femails.py
-drwxrwxrwx   0        0        0        0 2023-03-25 21:02:47.456850 funcsforspo_l-2.0.1/funcsforspo_l/fexceptions/
--rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 funcsforspo_l-2.0.1/funcsforspo_l/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      638 2023-01-19 14:04:05.000000 funcsforspo_l-2.0.1/funcsforspo_l/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-03-25 21:02:47.465960 funcsforspo_l-2.0.1/funcsforspo_l/fftp/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 funcsforspo_l-2.0.1/funcsforspo_l/fftp/__init__.py
--rw-rw-rw-   0        0        0     6241 2023-01-19 14:03:52.000000 funcsforspo_l-2.0.1/funcsforspo_l/fftp/fftp.py
-drwxrwxrwx   0        0        0        0 2023-03-25 21:02:47.475835 funcsforspo_l-2.0.1/funcsforspo_l/fopenpyxl/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 funcsforspo_l-2.0.1/funcsforspo_l/fopenpyxl/__init__.py
--rw-rw-rw-   0        0        0    11086 2023-02-03 19:05:17.000000 funcsforspo_l-2.0.1/funcsforspo_l/fopenpyxl/openpyxl_funcs.py
-drwxrwxrwx   0        0        0        0 2023-03-25 21:02:47.343610 funcsforspo_l-2.0.1/funcsforspo_l/fpdf/
-drwxrwxrwx   0        0        0        0 2023-03-25 21:02:47.480846 funcsforspo_l-2.0.1/funcsforspo_l/fpdf/base/
--rw-rw-rw-   0        0        0     9129 2023-03-25 20:32:20.000000 funcsforspo_l-2.0.1/funcsforspo_l/fpdf/base/base.py
-drwxrwxrwx   0        0        0        0 2023-03-25 21:02:47.496059 funcsforspo_l-2.0.1/funcsforspo_l/fpdf/fcompress/
--rw-rw-rw-   0        0        0     7782 2023-01-19 14:04:21.000000 funcsforspo_l-2.0.1/funcsforspo_l/fpdf/fcompress/__compress_online.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 funcsforspo_l-2.0.1/funcsforspo_l/fpdf/fcompress/__init__.py
--rw-rw-rw-   0        0        0     1637 2023-02-03 19:05:17.000000 funcsforspo_l-2.0.1/funcsforspo_l/fpdf/fcompress/compress.py
-drwxrwxrwx   0        0        0        0 2023-03-25 21:02:47.511676 funcsforspo_l-2.0.1/funcsforspo_l/fpdf/fhtml_to_pdf/
--rw-rw-rw-   0        0        0     3198 2023-03-25 20:17:19.000000 funcsforspo_l-2.0.1/funcsforspo_l/fpdf/fhtml_to_pdf/__html_to_pdf.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 funcsforspo_l-2.0.1/funcsforspo_l/fpdf/fhtml_to_pdf/__init__.py
--rw-rw-rw-   0        0        0     1607 2023-02-03 21:27:39.000000 funcsforspo_l-2.0.1/funcsforspo_l/fpdf/fhtml_to_pdf/html_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-03-25 21:02:47.514676 funcsforspo_l-2.0.1/funcsforspo_l/fpdf/fimgpdf/
--rw-rw-rw-   0        0        0    11127 2023-01-19 14:04:42.000000 funcsforspo_l-2.0.1/funcsforspo_l/fpdf/fimgpdf/img_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-03-25 21:02:47.530964 funcsforspo_l-2.0.1/funcsforspo_l/fpdf/focr/
--rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 funcsforspo_l-2.0.1/funcsforspo_l/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0     3546 2023-03-25 20:46:53.000000 funcsforspo_l-2.0.1/funcsforspo_l/fpdf/focr/__ocr_online.py
--rw-rw-rw-   0        0        0     2715 2023-03-25 20:26:53.000000 funcsforspo_l-2.0.1/funcsforspo_l/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2023-03-25 21:02:47.539022 funcsforspo_l-2.0.1/funcsforspo_l/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 funcsforspo_l-2.0.1/funcsforspo_l/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4620 2023-01-19 14:04:54.000000 funcsforspo_l-2.0.1/funcsforspo_l/fpysimplegui/functions_for_sg.py
-drwxrwxrwx   0        0        0        0 2023-03-25 21:02:47.548216 funcsforspo_l-2.0.1/funcsforspo_l/fpython/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 funcsforspo_l-2.0.1/funcsforspo_l/fpython/__init__.py
--rw-rw-rw-   0        0        0    67709 2023-03-25 20:45:09.000000 funcsforspo_l-2.0.1/funcsforspo_l/fpython/functions_for_py.py
-drwxrwxrwx   0        0        0        0 2023-03-25 21:02:47.559497 funcsforspo_l-2.0.1/funcsforspo_l/fregex/
--rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 funcsforspo_l-2.0.1/funcsforspo_l/fregex/__init__.py
--rw-rw-rw-   0        0        0    10116 2023-02-03 19:05:17.000000 funcsforspo_l-2.0.1/funcsforspo_l/fregex/functions_re.py
-drwxrwxrwx   0        0        0        0 2023-03-25 21:02:47.568986 funcsforspo_l-2.0.1/funcsforspo_l/fselenium/
--rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 funcsforspo_l-2.0.1/funcsforspo_l/fselenium/__init__.py
--rw-rw-rw-   0        0        0    38910 2023-03-25 20:46:06.000000 funcsforspo_l-2.0.1/funcsforspo_l/fselenium/functions_selenium.py
-drwxrwxrwx   0        0        0        0 2023-03-25 21:02:47.579570 funcsforspo_l-2.0.1/funcsforspo_l/fsqlite/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 funcsforspo_l-2.0.1/funcsforspo_l/fsqlite/__init__.py
--rw-rw-rw-   0        0        0     1645 2023-02-03 19:02:23.000000 funcsforspo_l-2.0.1/funcsforspo_l/fsqlite/sqlite_functions.py
-drwxrwxrwx   0        0        0        0 2023-03-25 21:02:47.408450 funcsforspo_l-2.0.1/funcsforspo_l.egg-info/
--rw-rw-rw-   0        0        0     1374 2023-03-25 21:02:47.000000 funcsforspo_l-2.0.1/funcsforspo_l.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1333 2023-03-25 21:02:47.000000 funcsforspo_l-2.0.1/funcsforspo_l.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-25 21:02:47.000000 funcsforspo_l-2.0.1/funcsforspo_l.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      139 2023-03-25 21:02:47.000000 funcsforspo_l-2.0.1/funcsforspo_l.egg-info/requires.txt
--rw-rw-rw-   0        0        0      362 2023-03-25 21:02:47.000000 funcsforspo_l-2.0.1/funcsforspo_l.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-25 21:02:47.586681 funcsforspo_l-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2088 2023-03-25 21:02:43.000000 funcsforspo_l-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.343428 funcsforspo_l-2.1.1/
+-rw-rw-rw-   0        0        0     1076 2023-02-03 19:05:17.000000 funcsforspo_l-2.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1374 2023-04-24 15:27:36.338461 funcsforspo_l-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      935 2023-02-03 19:05:17.000000 funcsforspo_l-2.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.128252 funcsforspo_l-2.1.1/funcsforspo_l/
+drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.188733 funcsforspo_l-2.1.1/funcsforspo_l/femails/
+-rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 funcsforspo_l-2.1.1/funcsforspo_l/femails/__init__.py
+-rw-rw-rw-   0        0        0     7604 2023-01-19 14:03:01.000000 funcsforspo_l-2.1.1/funcsforspo_l/femails/femails.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.200789 funcsforspo_l-2.1.1/funcsforspo_l/fexceptions/
+-rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 funcsforspo_l-2.1.1/funcsforspo_l/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      638 2023-01-19 14:04:05.000000 funcsforspo_l-2.1.1/funcsforspo_l/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.208796 funcsforspo_l-2.1.1/funcsforspo_l/fftp/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 funcsforspo_l-2.1.1/funcsforspo_l/fftp/__init__.py
+-rw-rw-rw-   0        0        0     6241 2023-01-19 14:03:52.000000 funcsforspo_l-2.1.1/funcsforspo_l/fftp/fftp.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.218305 funcsforspo_l-2.1.1/funcsforspo_l/fopenpyxl/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 funcsforspo_l-2.1.1/funcsforspo_l/fopenpyxl/__init__.py
+-rw-rw-rw-   0        0        0    11086 2023-02-03 19:05:17.000000 funcsforspo_l-2.1.1/funcsforspo_l/fopenpyxl/openpyxl_funcs.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.121889 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/
+drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.224008 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/base/
+-rw-rw-rw-   0        0        0    10163 2023-04-14 13:50:03.000000 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/base/base.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.241009 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/fcompress/
+-rw-rw-rw-   0        0        0     7782 2023-01-19 14:04:21.000000 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/fcompress/__compress_online.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/fcompress/__init__.py
+-rw-rw-rw-   0        0        0     1637 2023-02-03 19:05:17.000000 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/fcompress/compress.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.257167 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/fhtml_to_pdf/
+-rw-rw-rw-   0        0        0     3198 2023-03-25 20:17:19.000000 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/fhtml_to_pdf/__html_to_pdf.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/fhtml_to_pdf/__init__.py
+-rw-rw-rw-   0        0        0     1607 2023-02-03 21:27:39.000000 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/fhtml_to_pdf/html_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.264387 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/fimgpdf/
+-rw-rw-rw-   0        0        0    11127 2023-01-19 14:04:42.000000 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/fimgpdf/img_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.280904 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/focr/
+-rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0     3546 2023-03-25 20:46:53.000000 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/focr/__ocr_online.py
+-rw-rw-rw-   0        0        0     2715 2023-03-25 20:26:53.000000 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.285386 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/pdftoxlsx/
+-rw-rw-rw-   0        0        0     4212 2023-04-13 21:48:05.000000 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/pdftoxlsx/pdftoxlsx.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.295128 funcsforspo_l-2.1.1/funcsforspo_l/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 funcsforspo_l-2.1.1/funcsforspo_l/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4620 2023-01-19 14:04:54.000000 funcsforspo_l-2.1.1/funcsforspo_l/fpysimplegui/functions_for_sg.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.304118 funcsforspo_l-2.1.1/funcsforspo_l/fpython/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 funcsforspo_l-2.1.1/funcsforspo_l/fpython/__init__.py
+-rw-rw-rw-   0        0        0    67709 2023-03-25 20:45:09.000000 funcsforspo_l-2.1.1/funcsforspo_l/fpython/functions_for_py.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.314461 funcsforspo_l-2.1.1/funcsforspo_l/fregex/
+-rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 funcsforspo_l-2.1.1/funcsforspo_l/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10116 2023-02-03 19:05:17.000000 funcsforspo_l-2.1.1/funcsforspo_l/fregex/functions_re.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.322914 funcsforspo_l-2.1.1/funcsforspo_l/fselenium/
+-rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 funcsforspo_l-2.1.1/funcsforspo_l/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    37863 2023-04-24 15:26:45.000000 funcsforspo_l-2.1.1/funcsforspo_l/fselenium/functions_selenium.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.334971 funcsforspo_l-2.1.1/funcsforspo_l/fsqlite/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 funcsforspo_l-2.1.1/funcsforspo_l/fsqlite/__init__.py
+-rw-rw-rw-   0        0        0     1645 2023-02-03 19:02:23.000000 funcsforspo_l-2.1.1/funcsforspo_l/fsqlite/sqlite_functions.py
+drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.178473 funcsforspo_l-2.1.1/funcsforspo_l.egg-info/
+-rw-rw-rw-   0        0        0     1374 2023-04-24 15:27:35.000000 funcsforspo_l-2.1.1/funcsforspo_l.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1375 2023-04-24 15:27:36.000000 funcsforspo_l-2.1.1/funcsforspo_l.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 15:27:35.000000 funcsforspo_l-2.1.1/funcsforspo_l.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      139 2023-04-24 15:27:35.000000 funcsforspo_l-2.1.1/funcsforspo_l.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      391 2023-04-24 15:27:35.000000 funcsforspo_l-2.1.1/funcsforspo_l.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 15:27:36.343934 funcsforspo_l-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     2153 2023-04-24 15:26:59.000000 funcsforspo_l-2.1.1/setup.py
```

### Comparing `funcsforspo_l-2.0.1/LICENSE` & `funcsforspo_l-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `funcsforspo_l-2.0.1/PKG-INFO` & `funcsforspo_l-2.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcsforspo_l
-Version: 2.0.1
+Version: 2.1.1
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium - Linux
 Home-page: https://github.com/githubpaycon/funcsforspo_l
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium - Linux
 Description-Content-Type: text/markdown
```

### Comparing `funcsforspo_l-2.0.1/README.md` & `funcsforspo_l-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `funcsforspo_l-2.0.1/funcsforspo_l/femails/femails.py` & `funcsforspo_l-2.1.1/funcsforspo_l/femails/femails.py`

 * *Files identical despite different names*

### Comparing `funcsforspo_l-2.0.1/funcsforspo_l/fexceptions/exceptions.py` & `funcsforspo_l-2.1.1/funcsforspo_l/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `funcsforspo_l-2.0.1/funcsforspo_l/fftp/fftp.py` & `funcsforspo_l-2.1.1/funcsforspo_l/fftp/fftp.py`

 * *Files identical despite different names*

### Comparing `funcsforspo_l-2.0.1/funcsforspo_l/fopenpyxl/openpyxl_funcs.py` & `funcsforspo_l-2.1.1/funcsforspo_l/fopenpyxl/openpyxl_funcs.py`

 * *Files identical despite different names*

### Comparing `funcsforspo_l-2.0.1/funcsforspo_l/fpdf/base/base.py` & `funcsforspo_l-2.1.1/funcsforspo_l/fpdf/base/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -97,14 +97,22 @@
         self.WDW10 = WebDriverWait(self.DRIVER, timeout=10)
         self.WDW30 = WebDriverWait(self.DRIVER, timeout=30)
         self.WDW60 = WebDriverWait(self.DRIVER, timeout=60)
         self.WDW120 = WebDriverWait(self.DRIVER, timeout=120)
         self.WDW180 = WebDriverWait(self.DRIVER, timeout=180)
         self.WDW = self.WDW7
 
+        """
+        O código adiciona suporte para o download automático de arquivos em um diretório especificado no Chrome com headless usando o Selenium WebDriver.
+        """
+        self.DRIVER.command_executor._commands["send_command"] = ("POST", '/session/$sessionId/chromium/send_command')
+
+        params = {'cmd': 'Page.setDownloadBehavior', 'params': {'behavior': 'allow', 'downloadPath': self._DOWNLOAD_DIR}}
+        command_result = self.DRIVER.execute("send_command", params)
+
         self.DRIVER.maximize_window()
         return self.DRIVER
 
     def quit_web(self):
         self.DRIVER.quit()
         
         
@@ -182,17 +190,28 @@
         self.WDW10 = WebDriverWait(self.DRIVER, timeout=10)
         self.WDW30 = WebDriverWait(self.DRIVER, timeout=30)
         self.WDW60 = WebDriverWait(self.DRIVER, timeout=60)
         self.WDW120 = WebDriverWait(self.DRIVER, timeout=120)
         self.WDW180 = WebDriverWait(self.DRIVER, timeout=180)
         self.WDW = self.WDW7
 
+        """
+        O código adiciona suporte para o download automático de arquivos em um diretório especificado no Chrome com headless usando o Selenium WebDriver.
+        """
+        self.DRIVER.command_executor._commands["send_command"] = ("POST", '/session/$sessionId/chromium/send_command')
+
+        params = {'cmd': 'Page.setDownloadBehavior', 'params': {'behavior': 'allow', 'downloadPath': self._DOWNLOAD_DIR}}
+        command_result = self.DRIVER.execute("send_command", params)
+
         self.DRIVER.maximize_window()
+        
+        
+        
         return self.DRIVER
 
     def quit_web(self):
         self.DRIVER.quit()
         
 # UTILS #
 def faz_log_st(info):
     st.markdown(f'*`{info}`*')
-# UTILS #
+# UTILS #
```

### Comparing `funcsforspo_l-2.0.1/funcsforspo_l/fpdf/fcompress/__compress_online.py` & `funcsforspo_l-2.1.1/funcsforspo_l/fpdf/fcompress/__compress_online.py`

 * *Files identical despite different names*

### Comparing `funcsforspo_l-2.0.1/funcsforspo_l/fpdf/fcompress/compress.py` & `funcsforspo_l-2.1.1/funcsforspo_l/fpdf/fcompress/compress.py`

 * *Files identical despite different names*

### Comparing `funcsforspo_l-2.0.1/funcsforspo_l/fpdf/fhtml_to_pdf/__html_to_pdf.py` & `funcsforspo_l-2.1.1/funcsforspo_l/fpdf/fhtml_to_pdf/__html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `funcsforspo_l-2.0.1/funcsforspo_l/fpdf/fhtml_to_pdf/html_to_pdf.py` & `funcsforspo_l-2.1.1/funcsforspo_l/fpdf/fhtml_to_pdf/html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `funcsforspo_l-2.0.1/funcsforspo_l/fpdf/fimgpdf/img_to_pdf.py` & `funcsforspo_l-2.1.1/funcsforspo_l/fpdf/fimgpdf/img_to_pdf.py`

 * *Files identical despite different names*

### Comparing `funcsforspo_l-2.0.1/funcsforspo_l/fpdf/focr/__ocr_online.py` & `funcsforspo_l-2.1.1/funcsforspo_l/fpdf/focr/__ocr_online.py`

 * *Files identical despite different names*

### Comparing `funcsforspo_l-2.0.1/funcsforspo_l/fpdf/focr/orc.py` & `funcsforspo_l-2.1.1/funcsforspo_l/fpdf/focr/orc.py`

 * *Files identical despite different names*

### Comparing `funcsforspo_l-2.0.1/funcsforspo_l/fpysimplegui/functions_for_sg.py` & `funcsforspo_l-2.1.1/funcsforspo_l/fpysimplegui/functions_for_sg.py`

 * *Files identical despite different names*

### Comparing `funcsforspo_l-2.0.1/funcsforspo_l/fpython/functions_for_py.py` & `funcsforspo_l-2.1.1/funcsforspo_l/fpython/functions_for_py.py`

 * *Files identical despite different names*

### Comparing `funcsforspo_l-2.0.1/funcsforspo_l/fregex/functions_re.py` & `funcsforspo_l-2.1.1/funcsforspo_l/fregex/functions_re.py`

 * *Files identical despite different names*

### Comparing `funcsforspo_l-2.0.1/funcsforspo_l/fselenium/functions_selenium.py` & `funcsforspo_l-2.1.1/funcsforspo_l/fselenium/functions_selenium.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from random_user_agent.user_agent import UserAgent
 from random_user_agent.params import SoftwareName, OperatingSystem
 from time import sleep
 from funcsforspo_l.fpython.functions_for_py import *
 from funcsforspo_l.fregex.functions_re import extrair_email
 from wget import download
 from subprocess import getoutput
+import re
 
 def url_atual(driver) -> str:
     """
     ### Função RETORNA a url atual
 
     Args:
         driver (WebDriver): Seu Webdriver (Chrome, Firefox, Opera...)
@@ -53,45 +54,16 @@
     else:
         wdw.until(EC.presence_of_all_elements_located(locator))
     elements = driver.find_elements(*locator)
     len_elements = len(elements)
 
     for i in range(len_elements):
         elements[i].click()
-        
-        
-def verifica_se_baixou_o_arquivo(diretorio_de_download, palavra_chave, sleep_time=2, return_file=False) -> bool|str:
-    _LOCAL_DE_DOWNLOAD = os.path.abspath(diretorio_de_download)
-    baixou = False
-    while not baixou:
-        lista_arquivos = os.listdir(_LOCAL_DE_DOWNLOAD)
-        if len(lista_arquivos) == 0:
-            sleep(sleep_time)
-            baixou = False
-            lista_arquivos = os.listdir(_LOCAL_DE_DOWNLOAD)
-        else:
-            for i in lista_arquivos:
-                if '.crdownload' in i:
-                    sleep(sleep_time)
-                    lista_arquivos = os.listdir(_LOCAL_DE_DOWNLOAD)
-                    baixou = False
-                    continue
-                if palavra_chave in i:
-                    baixou = True
-                    faz_log('Download concluido!')
-                    if return_file:
-                        return arquivo_com_caminho_absoluto(_LOCAL_DE_DOWNLOAD, i)
-                    else:
-                        return True
-                else:
-                    sleep(sleep_time)
-                    lista_arquivos = os.listdir(_LOCAL_DE_DOWNLOAD)
-                    baixou = False
 
-    
+
 def espera_elemento_disponivel_e_clica(wdw:WebDriverWait, locator: tuple, in_dom:bool=False) -> None:
     """Espera o elemento ficar disponível para clicar e clica
 
     Args:
         wdw (WebDriverWait): WebDriverWait
         locator (tuple): localização do elemento -> (By.CSS_SELECTOR, '.b')
     """
@@ -996,38 +968,38 @@
     soup = BeautifulSoup(r.content, 'html5lib')
     if no_escape_sequence:
         return soup.find(tag_name).text.replace('\n', '').replace(u'\xa0', u' ')
     else:
         return soup.find(tag_name).text.replace(u'\xa0', u' ')
 
 
-def verifica_se_baixou_o_arquivo(diretorio_de_download, palavra_chave, sleep_time=2, return_file=False) -> bool:
+def verifica_se_baixou_o_arquivo(diretorio_de_download, palavra_chave, sleep_time=2, return_file=False) -> str|bool:
+    """
+    Verifies if a file with the specified keyword was downloaded in the given directory.
+    :param diretorio_de_download: the directory where the download occurred.
+    :param palavra_chave: the keyword to search for in the downloaded files.
+    :param sleep_time: the time to wait before checking again if the file was downloaded.
+    :param return_file: whether or not to return the downloaded file.
+    :return: the downloaded file with absolute path if return_file=True or True if it was downloaded.
+    """
     _LOCAL_DE_DOWNLOAD = os.path.abspath(diretorio_de_download)
     baixou = False
     while not baixou:
         lista_arquivos = os.listdir(_LOCAL_DE_DOWNLOAD)
-        lista_arquivos = [x.lower() for x in lista_arquivos]
         if len(lista_arquivos) == 0:
             sleep(sleep_time)
             baixou = False
             lista_arquivos = os.listdir(_LOCAL_DE_DOWNLOAD)
-            lista_arquivos = [x.lower() for x in lista_arquivos]
         else:
             for i in lista_arquivos:
-                if '.crdownload' in i:
-                    sleep(sleep_time)
-                    lista_arquivos = os.listdir(_LOCAL_DE_DOWNLOAD)
-                    lista_arquivos = [x.lower() for x in lista_arquivos]
-                    baixou = False
-                    continue
-                if palavra_chave in i:
+                files = re.findall(palavra_chave, i, re.IGNORECASE)
+                if len(files) >= 1:                
                     baixou = True
                     faz_log('Download concluido!')
                     if return_file:
                         return arquivo_com_caminho_absoluto(_LOCAL_DE_DOWNLOAD, i)
                     else:
                         return True
                 else:
                     sleep(sleep_time)
                     lista_arquivos = os.listdir(_LOCAL_DE_DOWNLOAD)
-                    lista_arquivos = [x.lower() for x in lista_arquivos]
                     baixou = False
```

### Comparing `funcsforspo_l-2.0.1/funcsforspo_l/fsqlite/sqlite_functions.py` & `funcsforspo_l-2.1.1/funcsforspo_l/fsqlite/sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `funcsforspo_l-2.0.1/funcsforspo_l.egg-info/PKG-INFO` & `funcsforspo_l-2.1.1/funcsforspo_l.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcsforspo-l
-Version: 2.0.1
+Version: 2.1.1
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium - Linux
 Home-page: https://github.com/githubpaycon/funcsforspo_l
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium - Linux
 Description-Content-Type: text/markdown
```

### Comparing `funcsforspo_l-2.0.1/funcsforspo_l.egg-info/SOURCES.txt` & `funcsforspo_l-2.1.1/funcsforspo_l.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 funcsforspo_l/fpdf/fhtml_to_pdf/__html_to_pdf.py
 funcsforspo_l/fpdf/fhtml_to_pdf/__init__.py
 funcsforspo_l/fpdf/fhtml_to_pdf/html_to_pdf.py
 funcsforspo_l/fpdf/fimgpdf/img_to_pdf.py
 funcsforspo_l/fpdf/focr/__init__.py
 funcsforspo_l/fpdf/focr/__ocr_online.py
 funcsforspo_l/fpdf/focr/orc.py
+funcsforspo_l/fpdf/pdftoxlsx/pdftoxlsx.py
 funcsforspo_l/fpysimplegui/__init__.py
 funcsforspo_l/fpysimplegui/functions_for_sg.py
 funcsforspo_l/fpython/__init__.py
 funcsforspo_l/fpython/functions_for_py.py
 funcsforspo_l/fregex/__init__.py
 funcsforspo_l/fregex/functions_re.py
 funcsforspo_l/fselenium/__init__.py
```

### Comparing `funcsforspo_l-2.0.1/setup.py` & `funcsforspo_l-2.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 import os
 from setuptools import setup
 
-version = '2.0.1'
+version = '2.1.1'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='funcsforspo_l',
         version=version,
         url='https://github.com/githubpaycon/funcsforspo_l',
@@ -18,14 +18,15 @@
         keywords='Funções Para Melhorar Desenvolvimento de Robôs com Selenium - Linux',
         description=u'Funções Para Melhorar Desenvolvimento de Robôs com Selenium - Linux',
         
         packages= [
             os.path.join('funcsforspo_l', 'femails'),
             os.path.join('funcsforspo_l', 'fexceptions'),
             os.path.join('funcsforspo_l', 'fftp'),
+            os.path.join('funcsforspo_l', 'fpdf', 'pdftoxlsx'),
             os.path.join('funcsforspo_l', 'fpdf'),
             os.path.join('funcsforspo_l', 'fpdf', 'base'),
             os.path.join('funcsforspo_l', 'fpdf', 'focr'),
             os.path.join('funcsforspo_l', 'fpdf', 'fcompress'),
             os.path.join('funcsforspo_l', 'fpdf', 'fimgpdf'),
             os.path.join('funcsforspo_l', 'fpdf', 'fhtml_to_pdf'),
             os.path.join('funcsforspo_l', 'fopenpyxl'),
```


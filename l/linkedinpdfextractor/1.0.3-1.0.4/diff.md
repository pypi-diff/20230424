# Comparing `tmp/linkedinpdfextractor-1.0.3.tar.gz` & `tmp/linkedinpdfextractor-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkedinpdfextractor-1.0.3.tar", last modified: Fri Apr 21 08:38:20 2023, max compression
+gzip compressed data, was "linkedinpdfextractor-1.0.4.tar", last modified: Mon Apr 24 06:29:19 2023, max compression
```

## Comparing `linkedinpdfextractor-1.0.3.tar` & `linkedinpdfextractor-1.0.4.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-21 08:38:20.410487 linkedinpdfextractor-1.0.3/
--rw-r--r--   0 seshivitakula   (501) staff       (20)     8196 2023-04-21 07:18:22.000000 linkedinpdfextractor-1.0.3/.DS_Store
--rw-r--r--   0 seshivitakula   (501) staff       (20)     1809 2023-04-21 06:26:32.000000 linkedinpdfextractor-1.0.3/.gitignore
--rw-r--r--   0 seshivitakula   (501) staff       (20)       82 2023-04-21 07:18:22.000000 linkedinpdfextractor-1.0.3/AUTHORS.rst
--rw-r--r--   0 seshivitakula   (501) staff       (20)      128 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.3/CHANGELOG.rst
--rw-r--r--   0 seshivitakula   (501) staff       (20)    14010 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.3/CONTRIBUTING.rst
--rw-r--r--   0 seshivitakula   (501) staff       (20)     1078 2023-04-19 16:57:33.000000 linkedinpdfextractor-1.0.3/LICENSE.txt
--rw-r--r--   0 seshivitakula   (501) staff       (20)     2374 2023-04-21 08:38:20.410640 linkedinpdfextractor-1.0.3/PKG-INFO
--rw-r--r--   0 seshivitakula   (501) staff       (20)     1865 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.3/README.rst
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-21 08:38:20.389120 linkedinpdfextractor-1.0.3/docs/
--rw-r--r--   0 seshivitakula   (501) staff       (20)     1154 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.3/docs/Makefile
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-21 08:38:20.389422 linkedinpdfextractor-1.0.3/docs/_static/
--rw-r--r--   0 seshivitakula   (501) staff       (20)       18 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.3/docs/_static/.gitignore
--rw-r--r--   0 seshivitakula   (501) staff       (20)       41 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.3/docs/authors.rst
--rw-r--r--   0 seshivitakula   (501) staff       (20)       43 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.3/docs/changelog.rst
--rw-r--r--   0 seshivitakula   (501) staff       (20)     9807 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.3/docs/conf.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)       33 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.3/docs/contributing.rst
--rw-r--r--   0 seshivitakula   (501) staff       (20)     2373 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.3/docs/index.rst
--rw-r--r--   0 seshivitakula   (501) staff       (20)       67 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.3/docs/license.rst
--rw-r--r--   0 seshivitakula   (501) staff       (20)       39 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.3/docs/readme.rst
--rw-r--r--   0 seshivitakula   (501) staff       (20)      233 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.3/docs/requirements.txt
--rw-r--r--   0 seshivitakula   (501) staff       (20)      346 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.3/pyproject.toml
--rw-r--r--   0 seshivitakula   (501) staff       (20)       46 2023-04-21 06:26:32.000000 linkedinpdfextractor-1.0.3/requirements.txt
--rw-r--r--   0 seshivitakula   (501) staff       (20)     1233 2023-04-21 08:38:20.411808 linkedinpdfextractor-1.0.3/setup.cfg
--rw-r--r--   0 seshivitakula   (501) staff       (20)      719 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.3/setup.py
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-21 08:38:20.389719 linkedinpdfextractor-1.0.3/src/
--rw-r--r--   0 seshivitakula   (501) staff       (20)     6148 2023-04-19 11:25:51.000000 linkedinpdfextractor-1.0.3/src/.DS_Store
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-21 08:38:20.391293 linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/
--rw-r--r--   0 seshivitakula   (501) staff       (20)     6148 2023-04-19 11:27:25.000000 linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/.DS_Store
--rw-r--r--   0 seshivitakula   (501) staff       (20)      577 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/__init__.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     5517 2023-04-21 07:18:22.000000 linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/extractor.py
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-21 08:38:20.392807 linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/pdfstructure/
--rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/pdfstructure/__init__.py
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-21 08:38:20.394384 linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/pdfstructure/analysis/
--rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/pdfstructure/analysis/__init__.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     2801 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/pdfstructure/analysis/annotate.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     3645 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/pdfstructure/analysis/sizemapper.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     5473 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/pdfstructure/analysis/styledistribution.py
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-21 08:38:20.395866 linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/pdfstructure/hierarchy/
--rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/pdfstructure/hierarchy/__init__.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     1501 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/pdfstructure/hierarchy/detectheader.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     2939 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/pdfstructure/hierarchy/headercompare.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     7135 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/pdfstructure/hierarchy/parser.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     2585 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/pdfstructure/hierarchy/traversal.py
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-21 08:38:20.396642 linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/pdfstructure/model/
--rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/pdfstructure/model/__init__.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     4451 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/pdfstructure/model/document.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     2108 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/pdfstructure/model/style.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     4063 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/pdfstructure/printer.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     4983 2023-04-21 06:26:32.000000 linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/pdfstructure/source.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     4253 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/pdfstructure/utils.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     4310 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/skeleton.py
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-21 08:38:20.398391 linkedinpdfextractor-1.0.3/src/linkedinpdfextractor.egg-info/
--rw-r--r--   0 seshivitakula   (501) staff       (20)     2374 2023-04-21 08:38:20.000000 linkedinpdfextractor-1.0.3/src/linkedinpdfextractor.egg-info/PKG-INFO
--rw-r--r--   0 seshivitakula   (501) staff       (20)     2518 2023-04-21 08:38:20.000000 linkedinpdfextractor-1.0.3/src/linkedinpdfextractor.egg-info/SOURCES.txt
--rw-r--r--   0 seshivitakula   (501) staff       (20)        1 2023-04-21 08:38:20.000000 linkedinpdfextractor-1.0.3/src/linkedinpdfextractor.egg-info/dependency_links.txt
--rw-r--r--   0 seshivitakula   (501) staff       (20)        1 2023-04-21 07:55:27.000000 linkedinpdfextractor-1.0.3/src/linkedinpdfextractor.egg-info/not-zip-safe
--rw-r--r--   0 seshivitakula   (501) staff       (20)       87 2023-04-21 08:38:20.000000 linkedinpdfextractor-1.0.3/src/linkedinpdfextractor.egg-info/requires.txt
--rw-r--r--   0 seshivitakula   (501) staff       (20)       23 2023-04-21 08:38:20.000000 linkedinpdfextractor-1.0.3/src/linkedinpdfextractor.egg-info/top_level.txt
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-21 08:38:20.402375 linkedinpdfextractor-1.0.3/tests/
--rw-r--r--   0 seshivitakula   (501) staff       (20)     6148 2023-04-19 17:09:48.000000 linkedinpdfextractor-1.0.3/tests/.DS_Store
--rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.3/tests/__init__.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)      290 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.3/tests/conftest.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)      728 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.3/tests/helper.py
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-21 08:38:20.408430 linkedinpdfextractor-1.0.3/tests/resources/
--rw-r--r--   0 seshivitakula   (501) staff       (20)   143869 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.3/tests/resources/5648.pdf
--rw-r--r--   0 seshivitakula   (501) staff       (20)   401628 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.3/tests/resources/IE00BM67HT60-ATB-FS-DE-2020-2-28.pdf
--rw-r--r--   0 seshivitakula   (501) staff       (20)    18836 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.3/tests/resources/SameSize_BoldTitle.pdf
--rw-r--r--   0 seshivitakula   (501) staff       (20)    12108 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.3/tests/resources/SameSize_EnumeratedTitle.pdf
--rw-r--r--   0 seshivitakula   (501) staff       (20)    12178 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.3/tests/resources/SameStyleOnly.pdf
--rw-r--r--   0 seshivitakula   (501) staff       (20)    45965 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.3/tests/resources/interview_cheatsheet-excerpt.png
--rwxr-xr-x   0 seshivitakula   (501) staff       (20)   230787 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.3/tests/resources/interview_cheatsheet.pdf
--rw-r--r--   0 seshivitakula   (501) staff       (20)    32674 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.3/tests/resources/lorem.pdf
--rw-r--r--   0 seshivitakula   (501) staff       (20)   383508 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.3/tests/resources/paper.pdf
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-21 08:38:20.410207 linkedinpdfextractor-1.0.3/tests/resources/parsed/
--rw-r--r--   0 seshivitakula   (501) staff       (20)   215280 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.3/tests/resources/parsed/interview_cheatsheet.json
--rw-r--r--   0 seshivitakula   (501) staff       (20)    15753 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.3/tests/resources/parsed/interview_cheatsheet_pretty.txt
--rw-r--r--   0 seshivitakula   (501) staff       (20)    62812 2023-04-19 12:12:39.000000 linkedinpdfextractor-1.0.3/tests/resources/profile.pdf
--rw-r--r--   0 seshivitakula   (501) staff       (20)   251982 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.3/tests/resources/samplepptx.pdf
--rw-r--r--   0 seshivitakula   (501) staff       (20)     1306 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.3/tests/test_custom_use_cases.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)      633 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.3/tests/test_document.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     2235 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.3/tests/test_headercompare.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     4617 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.3/tests/test_hierarchy.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     3110 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.3/tests/test_printer.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)      597 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.3/tests/test_skeleton.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     4161 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.3/tests/test_style_analyser.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     3773 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.3/tests/test_traversal.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)      781 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.3/tests/test_utils.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     2690 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.3/tox.ini
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-24 06:29:19.702229 linkedinpdfextractor-1.0.4/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     8196 2023-04-21 07:18:22.000000 linkedinpdfextractor-1.0.4/.DS_Store
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     1809 2023-04-21 06:26:32.000000 linkedinpdfextractor-1.0.4/.gitignore
+-rw-r--r--   0 seshivitakula   (501) staff       (20)       82 2023-04-21 07:18:22.000000 linkedinpdfextractor-1.0.4/AUTHORS.rst
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      128 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.4/CHANGELOG.rst
+-rw-r--r--   0 seshivitakula   (501) staff       (20)    14010 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.4/CONTRIBUTING.rst
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     1078 2023-04-19 16:57:33.000000 linkedinpdfextractor-1.0.4/LICENSE.txt
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     2374 2023-04-24 06:29:19.702393 linkedinpdfextractor-1.0.4/PKG-INFO
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     1865 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.4/README.rst
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-24 06:29:19.679794 linkedinpdfextractor-1.0.4/docs/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     1154 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.4/docs/Makefile
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-24 06:29:19.680037 linkedinpdfextractor-1.0.4/docs/_static/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)       18 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.4/docs/_static/.gitignore
+-rw-r--r--   0 seshivitakula   (501) staff       (20)       41 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.4/docs/authors.rst
+-rw-r--r--   0 seshivitakula   (501) staff       (20)       43 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.4/docs/changelog.rst
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     9807 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.4/docs/conf.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)       33 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.4/docs/contributing.rst
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     2373 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.4/docs/index.rst
+-rw-r--r--   0 seshivitakula   (501) staff       (20)       67 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.4/docs/license.rst
+-rw-r--r--   0 seshivitakula   (501) staff       (20)       39 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.4/docs/readme.rst
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      233 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.4/docs/requirements.txt
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      346 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.4/pyproject.toml
+-rw-r--r--   0 seshivitakula   (501) staff       (20)       46 2023-04-21 06:26:32.000000 linkedinpdfextractor-1.0.4/requirements.txt
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     1233 2023-04-24 06:29:19.703167 linkedinpdfextractor-1.0.4/setup.cfg
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      719 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.4/setup.py
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-24 06:29:19.680323 linkedinpdfextractor-1.0.4/src/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     6148 2023-04-19 11:25:51.000000 linkedinpdfextractor-1.0.4/src/.DS_Store
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-24 06:29:19.681705 linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     6148 2023-04-19 11:27:25.000000 linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/.DS_Store
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      577 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/__init__.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     5609 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/extractor.py
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-24 06:29:19.682782 linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/pdfstructure/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/pdfstructure/__init__.py
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-24 06:29:19.684041 linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/pdfstructure/analysis/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/pdfstructure/analysis/__init__.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     2916 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/pdfstructure/analysis/annotate.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     3691 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/pdfstructure/analysis/sizemapper.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     5496 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/pdfstructure/analysis/styledistribution.py
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-24 06:29:19.685403 linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/pdfstructure/hierarchy/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/pdfstructure/hierarchy/__init__.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     1593 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/pdfstructure/hierarchy/detectheader.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     2985 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/pdfstructure/hierarchy/headercompare.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     7296 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/pdfstructure/hierarchy/parser.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     2608 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/pdfstructure/hierarchy/traversal.py
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-24 06:29:19.686068 linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/pdfstructure/model/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/pdfstructure/model/__init__.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     4497 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/pdfstructure/model/document.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     2108 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/pdfstructure/model/style.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     4155 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/pdfstructure/printer.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     4983 2023-04-21 06:26:32.000000 linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/pdfstructure/source.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     4253 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/pdfstructure/utils.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     4310 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/skeleton.py
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-24 06:29:19.688036 linkedinpdfextractor-1.0.4/src/linkedinpdfextractor.egg-info/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     2374 2023-04-24 06:29:19.000000 linkedinpdfextractor-1.0.4/src/linkedinpdfextractor.egg-info/PKG-INFO
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     2518 2023-04-24 06:29:19.000000 linkedinpdfextractor-1.0.4/src/linkedinpdfextractor.egg-info/SOURCES.txt
+-rw-r--r--   0 seshivitakula   (501) staff       (20)        1 2023-04-24 06:29:19.000000 linkedinpdfextractor-1.0.4/src/linkedinpdfextractor.egg-info/dependency_links.txt
+-rw-r--r--   0 seshivitakula   (501) staff       (20)        1 2023-04-21 07:55:27.000000 linkedinpdfextractor-1.0.4/src/linkedinpdfextractor.egg-info/not-zip-safe
+-rw-r--r--   0 seshivitakula   (501) staff       (20)       87 2023-04-24 06:29:19.000000 linkedinpdfextractor-1.0.4/src/linkedinpdfextractor.egg-info/requires.txt
+-rw-r--r--   0 seshivitakula   (501) staff       (20)       23 2023-04-24 06:29:19.000000 linkedinpdfextractor-1.0.4/src/linkedinpdfextractor.egg-info/top_level.txt
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-24 06:29:19.691486 linkedinpdfextractor-1.0.4/tests/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     6148 2023-04-19 17:09:48.000000 linkedinpdfextractor-1.0.4/tests/.DS_Store
+-rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.4/tests/__init__.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      290 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.4/tests/conftest.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      820 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.0.4/tests/helper.py
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-24 06:29:19.700228 linkedinpdfextractor-1.0.4/tests/resources/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)   143869 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.4/tests/resources/5648.pdf
+-rw-r--r--   0 seshivitakula   (501) staff       (20)   401628 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.4/tests/resources/IE00BM67HT60-ATB-FS-DE-2020-2-28.pdf
+-rw-r--r--   0 seshivitakula   (501) staff       (20)    18836 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.4/tests/resources/SameSize_BoldTitle.pdf
+-rw-r--r--   0 seshivitakula   (501) staff       (20)    12108 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.4/tests/resources/SameSize_EnumeratedTitle.pdf
+-rw-r--r--   0 seshivitakula   (501) staff       (20)    12178 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.4/tests/resources/SameStyleOnly.pdf
+-rw-r--r--   0 seshivitakula   (501) staff       (20)    45965 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.4/tests/resources/interview_cheatsheet-excerpt.png
+-rwxr-xr-x   0 seshivitakula   (501) staff       (20)   230787 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.4/tests/resources/interview_cheatsheet.pdf
+-rw-r--r--   0 seshivitakula   (501) staff       (20)    32674 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.4/tests/resources/lorem.pdf
+-rw-r--r--   0 seshivitakula   (501) staff       (20)   383508 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.4/tests/resources/paper.pdf
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-04-24 06:29:19.701920 linkedinpdfextractor-1.0.4/tests/resources/parsed/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)   215280 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.4/tests/resources/parsed/interview_cheatsheet.json
+-rw-r--r--   0 seshivitakula   (501) staff       (20)    15753 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.4/tests/resources/parsed/interview_cheatsheet_pretty.txt
+-rw-r--r--   0 seshivitakula   (501) staff       (20)    62812 2023-04-19 12:12:39.000000 linkedinpdfextractor-1.0.4/tests/resources/profile.pdf
+-rw-r--r--   0 seshivitakula   (501) staff       (20)   251982 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.0.4/tests/resources/samplepptx.pdf
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     1398 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.0.4/tests/test_custom_use_cases.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      656 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.0.4/tests/test_document.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     2304 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.0.4/tests/test_headercompare.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     4709 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.0.4/tests/test_hierarchy.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     3202 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.0.4/tests/test_printer.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      597 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.4/tests/test_skeleton.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     4276 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.0.4/tests/test_style_analyser.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     3865 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.0.4/tests/test_traversal.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      804 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.0.4/tests/test_utils.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     2690 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.0.4/tox.ini
```

### Comparing `linkedinpdfextractor-1.0.3/.DS_Store` & `linkedinpdfextractor-1.0.4/.DS_Store`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.0.3/.gitignore` & `linkedinpdfextractor-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.0.3/CONTRIBUTING.rst` & `linkedinpdfextractor-1.0.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.0.3/LICENSE.txt` & `linkedinpdfextractor-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.0.3/PKG-INFO` & `linkedinpdfextractor-1.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkedinpdfextractor
-Version: 1.0.3
+Version: 1.0.4
 Summary: Add a short description here!
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Ketan Prabhu
 Author-email: ketan.prabhu@gigvistas.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `linkedinpdfextractor-1.0.3/README.rst` & `linkedinpdfextractor-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.0.3/docs/Makefile` & `linkedinpdfextractor-1.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.0.3/docs/conf.py` & `linkedinpdfextractor-1.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.0.3/docs/index.rst` & `linkedinpdfextractor-1.0.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.0.3/setup.cfg` & `linkedinpdfextractor-1.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.0.3/setup.py` & `linkedinpdfextractor-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.0.3/src/.DS_Store` & `linkedinpdfextractor-1.0.4/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/.DS_Store` & `linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/.DS_Store`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/__init__.py` & `linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/__init__.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/extractor.py` & `linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from pdfstructure.hierarchy.parser import HierarchyParser
-from pdfstructure.source import FileSource
-from pdfstructure.printer import JsonFilePrinter
+from linkedin_pdf_extractor.pdfstructure.hierarchy.parser import HierarchyParser
+from linkedin_pdf_extractor.pdfstructure.source import FileSource
+from linkedin_pdf_extractor.pdfstructure.printer import JsonFilePrinter
 import json
-from pdfstructure.model.document import TextElement, Section, StructuredPdfDocument, DanglingTextSection
+from linkedin_pdf_extractor.pdfstructure.model.document import TextElement, Section, StructuredPdfDocument, DanglingTextSection
 from typing import List
 import pandas as pd
 import re
 import jsonpickle
 
 
 class Summary:
```

### Comparing `linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/pdfstructure/analysis/annotate.py` & `linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/pdfstructure/analysis/annotate.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import statistics
 from collections import Counter
 
 from pdfminer.layout import LTTextBoxHorizontal, LTChar
 
-from pdfstructure.analysis.sizemapper import SizeMapper
-from pdfstructure.analysis.styledistribution import StyleDistribution
-from pdfstructure.model.document import TextElement
-from pdfstructure.model.style import Style, TextSize
-from pdfstructure.utils import truncate
+from linkedin_pdf_extractor.pdfstructure.analysis.sizemapper import SizeMapper
+from linkedin_pdf_extractor.pdfstructure.analysis.styledistribution import StyleDistribution
+from linkedin_pdf_extractor.pdfstructure.model.document import TextElement
+from linkedin_pdf_extractor.pdfstructure.model.style import Style, TextSize
+from linkedin_pdf_extractor.pdfstructure.utils import truncate
 
 
 class StyleAnnotator:
     """
     creates a PdfElements from incoming pdf-paragraphs (raw LTTextContainer from pdfminer.six).
     - annotates paragraph with @Style(italic, bold, fontname, mapped_size, mean_size).
     - mapped_font_size: captures most dominant character size within paragraph & maps it to TextSize Enum.
```

### Comparing `linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/pdfstructure/analysis/sizemapper.py` & `linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/pdfstructure/analysis/sizemapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import math
 from enum import Enum
 from typing import Type
 
-from pdfstructure.analysis.styledistribution import StyleDistribution
-from pdfstructure.model.style import TextSize
+from linkedin_pdf_extractor.pdfstructure.analysis.styledistribution import StyleDistribution
+from linkedin_pdf_extractor.pdfstructure.model.style import TextSize
 
 
 class SizeMapper:
 
     def __init__(self):
         self._borders = None
```

### Comparing `linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/pdfstructure/analysis/styledistribution.py` & `linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/pdfstructure/analysis/styledistribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import itertools
 from collections import Counter, defaultdict
 
 from pdfminer.layout import LTTextContainer, LTTextLine, LTChar
 from sortedcontainers import SortedDict
 
-from pdfstructure.utils import truncate, closest_key
+from linkedin_pdf_extractor.pdfstructure.utils import truncate, closest_key
 
 
 class StyleDistribution:
     """
     Represents style information for one analysed element stream (typically one stream per document).
     """
```

### Comparing `linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/pdfstructure/hierarchy/detectheader.py` & `linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/pdfstructure/hierarchy/detectheader.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from collections import Counter
 
 from pdfminer.layout import LTTextBoxVertical
 
-from pdfstructure.analysis.styledistribution import StyleDistribution
-from pdfstructure.model.document import TextElement
-from pdfstructure.model.style import TextSize
-from pdfstructure.utils import word_generator
+from linkedin_pdf_extractor.pdfstructure.analysis.styledistribution import StyleDistribution
+from linkedin_pdf_extractor.pdfstructure.model.document import TextElement
+from linkedin_pdf_extractor.pdfstructure.model.style import TextSize
+from linkedin_pdf_extractor.pdfstructure.utils import word_generator
 
 
 def header_detector(element: TextElement, style_distribution: StyleDistribution):
     if isinstance(element._data, LTTextBoxVertical):
         return False
     stats = Counter()
     terms = element._data
```

### Comparing `linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/pdfstructure/hierarchy/headercompare.py` & `linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/pdfstructure/hierarchy/headercompare.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 
-from pdfstructure.model.document import Section
-from pdfstructure.utils import word_generator
+from linkedin_pdf_extractor.pdfstructure.model.document import Section
+from linkedin_pdf_extractor.pdfstructure.utils import word_generator
 
 numeration_pattern = re.compile("^(?=.*\d+)((?=.*\.)|(?=.*:)).*$")
 white_space_pattern = re.compile("\\s+")
 
 
 class SubHeaderPredicate:
     """
```

### Comparing `linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/pdfstructure/hierarchy/parser.py` & `linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/pdfstructure/hierarchy/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from pathlib import Path
 from typing import List, Generator
 
 from pdfminer.layout import LTTextContainer, LAParams
 
-from pdfstructure.analysis.annotate import StyleAnnotator
-from pdfstructure.analysis.sizemapper import PivotLogMapper
-from pdfstructure.analysis.styledistribution import count_sizes, StyleDistribution
-from pdfstructure.hierarchy.detectheader import header_detector
-from pdfstructure.hierarchy.headercompare import get_default_sub_header_conditions
-from pdfstructure.model.document import TextElement, Section, StructuredPdfDocument, DanglingTextSection
-from pdfstructure.source import Source
+from linkedin_pdf_extractor.pdfstructure.analysis.annotate import StyleAnnotator
+from linkedin_pdf_extractor.pdfstructure.analysis.sizemapper import PivotLogMapper
+from linkedin_pdf_extractor.pdfstructure.analysis.styledistribution import count_sizes, StyleDistribution
+from linkedin_pdf_extractor.pdfstructure.hierarchy.detectheader import header_detector
+from linkedin_pdf_extractor.pdfstructure.hierarchy.headercompare import get_default_sub_header_conditions
+from linkedin_pdf_extractor.pdfstructure.model.document import TextElement, Section, StructuredPdfDocument, DanglingTextSection
+from linkedin_pdf_extractor.pdfstructure.source import Source
 
 
 class HierarchyParser:
 
     def __init__(self, sub_header_conditions=get_default_sub_header_conditions()):
         self._isSubHeader = sub_header_conditions
```

### Comparing `linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/pdfstructure/hierarchy/traversal.py` & `linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/pdfstructure/hierarchy/traversal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 from collections import deque
 from typing import Generator
 
-from pdfstructure.model.document import StructuredPdfDocument, Section
+from linkedin_pdf_extractor.pdfstructure.model.document import StructuredPdfDocument, Section
 
 
 def get_document_depth(document: StructuredPdfDocument):
     """
     retrieves document depth found within tree structure, + 1 because the levels are 0 notated.
     """
     return max(set([section.level for section in traverse_in_order(document)])) + 1
```

### Comparing `linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/pdfstructure/model/document.py` & `linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/pdfstructure/model/document.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections import defaultdict
 from typing import List
 
 from pdfminer.layout import LTTextContainer
 
-from pdfstructure.analysis.styledistribution import StyleDistribution
-from pdfstructure.model.style import Style
+from linkedin_pdf_extractor.pdfstructure.analysis.styledistribution import StyleDistribution
+from linkedin_pdf_extractor.pdfstructure.model.style import Style
 
 
 class TextElement:
     """
     Represents one single TextContainer like a line of words.
     """
```

### Comparing `linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/pdfstructure/model/style.py` & `linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/pdfstructure/model/style.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/pdfstructure/printer.py` & `linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/pdfstructure/printer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 from typing import Iterator
 
-from pdfstructure.hierarchy.traversal import traverse_in_order
-from pdfstructure.model.document import Section, StructuredPdfDocument, TextElement
-from pdfstructure.model.style import Style
-from pdfstructure.utils import dict_subset
+from linkedin_pdf_extractor.pdfstructure.hierarchy.traversal import traverse_in_order
+from linkedin_pdf_extractor.pdfstructure.model.document import Section, StructuredPdfDocument, TextElement
+from linkedin_pdf_extractor.pdfstructure.model.style import Style
+from linkedin_pdf_extractor.pdfstructure.utils import dict_subset
 
 
 class Printer:
     def print(self, document: StructuredPdfDocument, *args, **kwargs):
         pass
```

### Comparing `linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/pdfstructure/source.py` & `linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/pdfstructure/source.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/pdfstructure/utils.py` & `linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/pdfstructure/utils.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.0.3/src/linkedin_pdf_extractor/skeleton.py` & `linkedinpdfextractor-1.0.4/src/linkedin_pdf_extractor/skeleton.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.0.3/src/linkedinpdfextractor.egg-info/PKG-INFO` & `linkedinpdfextractor-1.0.4/src/linkedinpdfextractor.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkedinpdfextractor
-Version: 1.0.3
+Version: 1.0.4
 Summary: Add a short description here!
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Ketan Prabhu
 Author-email: ketan.prabhu@gigvistas.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `linkedinpdfextractor-1.0.3/src/linkedinpdfextractor.egg-info/SOURCES.txt` & `linkedinpdfextractor-1.0.4/src/linkedinpdfextractor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.0.3/tests/.DS_Store` & `linkedinpdfextractor-1.0.4/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.0.3/tests/resources/5648.pdf` & `linkedinpdfextractor-1.0.4/tests/resources/5648.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.0.3/tests/resources/IE00BM67HT60-ATB-FS-DE-2020-2-28.pdf` & `linkedinpdfextractor-1.0.4/tests/resources/IE00BM67HT60-ATB-FS-DE-2020-2-28.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.0.3/tests/resources/SameSize_BoldTitle.pdf` & `linkedinpdfextractor-1.0.4/tests/resources/SameSize_BoldTitle.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.0.3/tests/resources/SameSize_EnumeratedTitle.pdf` & `linkedinpdfextractor-1.0.4/tests/resources/SameSize_EnumeratedTitle.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.0.3/tests/resources/SameStyleOnly.pdf` & `linkedinpdfextractor-1.0.4/tests/resources/SameStyleOnly.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.0.3/tests/resources/interview_cheatsheet-excerpt.png` & `linkedinpdfextractor-1.0.4/tests/resources/interview_cheatsheet-excerpt.png`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.0.3/tests/resources/interview_cheatsheet.pdf` & `linkedinpdfextractor-1.0.4/tests/resources/interview_cheatsheet.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.0.3/tests/resources/lorem.pdf` & `linkedinpdfextractor-1.0.4/tests/resources/lorem.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.0.3/tests/resources/paper.pdf` & `linkedinpdfextractor-1.0.4/tests/resources/paper.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.0.3/tests/resources/parsed/interview_cheatsheet.json` & `linkedinpdfextractor-1.0.4/tests/resources/parsed/interview_cheatsheet.json`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.0.3/tests/resources/parsed/interview_cheatsheet_pretty.txt` & `linkedinpdfextractor-1.0.4/tests/resources/parsed/interview_cheatsheet_pretty.txt`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.0.3/tests/resources/profile.pdf` & `linkedinpdfextractor-1.0.4/tests/resources/profile.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.0.3/tests/resources/samplepptx.pdf` & `linkedinpdfextractor-1.0.4/tests/resources/samplepptx.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.0.3/tests/test_custom_use_cases.py` & `linkedinpdfextractor-1.0.4/tests/test_custom_use_cases.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 from unittest import TestCase
 
-from pdfstructure.hierarchy.parser import HierarchyParser
-from pdfstructure.hierarchy.traversal import traverse_inorder_sections_with_content
-from pdfstructure.printer import PrettyStringPrinter as txtPrinter
-from pdfstructure.source import FileSource
+from linkedin_pdf_extractor.pdfstructure.hierarchy.parser import HierarchyParser
+from linkedin_pdf_extractor.pdfstructure.hierarchy.traversal import traverse_inorder_sections_with_content
+from linkedin_pdf_extractor.pdfstructure.printer import PrettyStringPrinter as txtPrinter
+from linkedin_pdf_extractor.pdfstructure.source import FileSource
 
 
 class TestExamples(TestCase):
     parser = HierarchyParser()
 
     def test_count_paragraph_words(self):
         test_file = str(Path("resources/lorem.pdf"))
```

### Comparing `linkedinpdfextractor-1.0.3/tests/test_document.py` & `linkedinpdfextractor-1.0.4/tests/test_document.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 from pathlib import Path
 from unittest import TestCase
 
-from pdfstructure.model.document import StructuredPdfDocument
+from linkedin_pdf_extractor.pdfstructure.model.document import StructuredPdfDocument
 
 
 class TestSection(TestCase):
 
     def test_full_content(self):
         with open(str(Path("resources/parsed/interview_cheatsheet.json").absolute()), "r") as fp:
             json_string = json.load(fp)
```

### Comparing `linkedinpdfextractor-1.0.3/tests/test_headercompare.py` & `linkedinpdfextractor-1.0.4/tests/test_headercompare.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from unittest import TestCase
 
 from pdfminer.layout import LTChar, LTTextBoxHorizontal, LTTextLineHorizontal
 
-from pdfstructure.hierarchy.headercompare import condition_h2_extends_h1, condition_h1_enum_h2_not
-from pdfstructure.model.document import TextElement, Section
-from pdfstructure.model.style import Style, TextSize
+from linkedin_pdf_extractor.pdfstructure.hierarchy.headercompare import condition_h2_extends_h1, condition_h1_enum_h2_not
+from linkedin_pdf_extractor.pdfstructure.model.document import TextElement, Section
+from linkedin_pdf_extractor.pdfstructure.model.style import Style, TextSize
 
 
 class TestSubHeaderConditions(TestCase):
     style_middle_bold = Style(bold=True, italic=True, font_name="test-font",
                               mapped_font_size=TextSize.middle,
                               mean_size=10, max_size=15)
```

### Comparing `linkedinpdfextractor-1.0.3/tests/test_hierarchy.py` & `linkedinpdfextractor-1.0.4/tests/test_hierarchy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from pathlib import Path
 from unittest import TestCase
 
 from pdfminer.high_level import extract_text
 
-from pdfstructure.hierarchy.parser import HierarchyParser
-from pdfstructure.model.document import DanglingTextSection
-from pdfstructure.printer import PrettyStringPrinter
-from pdfstructure.source import FileSource
+from linkedin_pdf_extractor.pdfstructure.hierarchy.parser import HierarchyParser
+from linkedin_pdf_extractor.pdfstructure.model.document import DanglingTextSection
+from linkedin_pdf_extractor.pdfstructure.printer import PrettyStringPrinter
+from linkedin_pdf_extractor.pdfstructure.source import FileSource
 
 
 class TestHierarchy(TestCase):
     doc_with_columns = str(Path("resources/IE00BM67HT60-ATB-FS-DE-2020-2-28.pdf").absolute())
     straight_forward_doc = str(Path("resources/interview_cheatsheet.pdf").absolute())
     nested_doc_bold_title = str(Path("resources/5648.pdf").absolute())
```

### Comparing `linkedinpdfextractor-1.0.3/tests/test_printer.py` & `linkedinpdfextractor-1.0.4/tests/test_printer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from pathlib import Path
 from unittest import TestCase
 
-from pdfstructure.hierarchy.parser import HierarchyParser
-from pdfstructure.model.document import StructuredPdfDocument
-from pdfstructure.printer import PrettyStringFilePrinter, PrettyStringPrinter, JsonFilePrinter, JsonStringPrinter
-from pdfstructure.source import FileSource
+from linkedin_pdf_extractor.pdfstructure.hierarchy.parser import HierarchyParser
+from linkedin_pdf_extractor.pdfstructure.model.document import StructuredPdfDocument
+from linkedin_pdf_extractor.pdfstructure.printer import PrettyStringFilePrinter, PrettyStringPrinter, JsonFilePrinter, JsonStringPrinter
+from linkedin_pdf_extractor.pdfstructure.source import FileSource
 
 
 class TestPrettyStringPrinter(TestCase):
     straight_forward_doc = str(Path("resources/interview_cheatsheet.pdf").absolute())
     column_doc = str(Path("resources/IE00BM67HT60-ATB-FS-DE-2020-2-28.pdf").absolute())
     correctFormattedText = "[Data Structure Basics]\n\n\t[Array]\n\n\t\t[Definition:]\n\t\t\tStores data elements" \
                            " based on an sequential, most commonly 0 based, index."
```

### Comparing `linkedinpdfextractor-1.0.3/tests/test_skeleton.py` & `linkedinpdfextractor-1.0.4/tests/test_skeleton.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.0.3/tests/test_style_analyser.py` & `linkedinpdfextractor-1.0.4/tests/test_style_analyser.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import itertools
 from collections import Counter
 from pathlib import Path
 from unittest import TestCase
 
 import pandas as pd
 
-from pdfstructure.analysis.annotate import StyleAnnotator
-from pdfstructure.analysis.sizemapper import PivotLogMapper, PivotLinearMapper
-from pdfstructure.analysis.styledistribution import count_sizes, StyleDistribution
-from pdfstructure.model.style import TextSize
-from pdfstructure.utils import element_generator, find_file, DocTypeFilter
+from linkedin_pdf_extractor.pdfstructure.analysis.annotate import StyleAnnotator
+from linkedin_pdf_extractor.pdfstructure.analysis.sizemapper import PivotLogMapper, PivotLinearMapper
+from linkedin_pdf_extractor.pdfstructure.analysis.styledistribution import count_sizes, StyleDistribution
+from linkedin_pdf_extractor.pdfstructure.model.style import TextSize
+from linkedin_pdf_extractor.pdfstructure.utils import element_generator, find_file, DocTypeFilter
 
 
 class TestSizeMapper(TestCase):
 
     def test_log_mapper(self):
         distribution = StyleDistribution(Counter((1, 5, 6, 10, 10, 10, 10, 20, 100)))
         scaler = PivotLogMapper(distribution)
```

### Comparing `linkedinpdfextractor-1.0.3/tests/test_traversal.py` & `linkedinpdfextractor-1.0.4/tests/test_traversal.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 from unittest import TestCase
 
-from pdfstructure.hierarchy.parser import HierarchyParser
-from pdfstructure.hierarchy.traversal import traverse_in_order, traverse_level_order, get_document_depth, \
+from linkedin_pdf_extractor.pdfstructure.hierarchy.parser import HierarchyParser
+from linkedin_pdf_extractor.pdfstructure.hierarchy.traversal import traverse_in_order, traverse_level_order, get_document_depth, \
     traverse_inorder_sections_with_content
-from pdfstructure.model.document import DanglingTextSection
-from pdfstructure.source import FileSource
+from linkedin_pdf_extractor.pdfstructure.model.document import DanglingTextSection
+from linkedin_pdf_extractor.pdfstructure.source import FileSource
 
 
 class TestDocumentTraversal(TestCase):
     straight_forward_doc = str(Path("resources/interview_cheatsheet.pdf").absolute())
     same_style_doc = str(Path("resources/SameStyleOnly.pdf").absolute())
     test_doc = None
     test_doc_same_style = None
```

### Comparing `linkedinpdfextractor-1.0.3/tests/test_utils.py` & `linkedinpdfextractor-1.0.4/tests/test_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 from unittest import TestCase
 
-from pdfstructure.utils import element_generator, word_generator
+from linkedin_pdf_extractor.pdfstructure.utils import element_generator, word_generator
 
 
 class Test(TestCase):
     test_path_1 = str(Path("resources/interview_cheatsheet.pdf").absolute())
     
     def test_word_generator(self):
         elements = element_generator(self.test_path_1)
```

### Comparing `linkedinpdfextractor-1.0.3/tox.ini` & `linkedinpdfextractor-1.0.4/tox.ini`

 * *Files identical despite different names*


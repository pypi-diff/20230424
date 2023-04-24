# Comparing `tmp/google-resumable-media-2.4.1.tar.gz` & `tmp/google-resumable-media-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-resumable-media-2.4.1.tar", last modified: Thu Jan 19 21:32:45 2023, max compression
+gzip compressed data, was "google-resumable-media-2.5.0.tar", last modified: Mon Apr 24 19:02:52 2023, max compression
```

## Comparing `google-resumable-media-2.4.1.tar` & `google-resumable-media-2.5.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-19 21:32:45.372634 google-resumable-media-2.4.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      111 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     1884 2023-01-19 21:32:45.372634 google-resumable-media-2.4.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003      964 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-19 21:32:45.360633 google-resumable-media-2.4.1/google/
--rw-rw-r--   0 root         (0)     1003      764 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/google/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-19 21:32:45.364633 google-resumable-media-2.4.1/google/_async_resumable_media/
--rw-rw-r--   0 root         (0)     1003     1736 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/google/_async_resumable_media/__init__.py
--rw-rw-r--   0 root         (0)     1003    20354 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/google/_async_resumable_media/_download.py
--rw-rw-r--   0 root         (0)     1003     6572 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/google/_async_resumable_media/_helpers.py
--rw-rw-r--   0 root         (0)     1003    37337 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/google/_async_resumable_media/_upload.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-19 21:32:45.364633 google-resumable-media-2.4.1/google/_async_resumable_media/requests/
--rw-rw-r--   0 root         (0)     1003    21652 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/google/_async_resumable_media/requests/__init__.py
--rw-rw-r--   0 root         (0)     1003     5117 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/google/_async_resumable_media/requests/_request_helpers.py
--rw-rw-r--   0 root         (0)     1003    18751 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/google/_async_resumable_media/requests/download.py
--rw-rw-r--   0 root         (0)     1003    19252 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/google/_async_resumable_media/requests/upload.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-19 21:32:45.364633 google-resumable-media-2.4.1/google/resumable_media/
--rw-rw-r--   0 root         (0)     1003     1736 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/google/resumable_media/__init__.py
--rw-rw-r--   0 root         (0)     1003    20656 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/google/resumable_media/_download.py
--rw-rw-r--   0 root         (0)     1003    13439 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/google/resumable_media/_helpers.py
--rw-rw-r--   0 root         (0)     1003    39465 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/google/resumable_media/_upload.py
--rw-rw-r--   0 root         (0)     1003     6191 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/google/resumable_media/common.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-19 21:32:45.364633 google-resumable-media-2.4.1/google/resumable_media/requests/
--rw-rw-r--   0 root         (0)     1003    21603 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/google/resumable_media/requests/__init__.py
--rw-rw-r--   0 root         (0)     1003     6151 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/google/resumable_media/requests/_request_helpers.py
--rw-rw-r--   0 root         (0)     1003    26433 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/google/resumable_media/requests/download.py
--rw-rw-r--   0 root         (0)     1003    20858 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/google/resumable_media/requests/upload.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-19 21:32:45.364633 google-resumable-media-2.4.1/google_resumable_media.egg-info/
--rw-r--r--   0 root         (0)     1003     1884 2023-01-19 21:32:45.000000 google-resumable-media-2.4.1/google_resumable_media.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1783 2023-01-19 21:32:45.000000 google-resumable-media-2.4.1/google_resumable_media.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-19 21:32:45.000000 google-resumable-media-2.4.1/google_resumable_media.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        7 2023-01-19 21:32:45.000000 google-resumable-media-2.4.1/google_resumable_media.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-19 21:32:45.000000 google-resumable-media-2.4.1/google_resumable_media.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      102 2023-01-19 21:32:45.000000 google-resumable-media-2.4.1/google_resumable_media.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-01-19 21:32:45.000000 google-resumable-media-2.4.1/google_resumable_media.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003      104 2023-01-19 21:32:45.372634 google-resumable-media-2.4.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2131 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-19 21:32:45.368633 google-resumable-media-2.4.1/tests/
--rw-rw-r--   0 root         (0)     1003      575 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-19 21:32:45.368633 google-resumable-media-2.4.1/tests/data/
--rw-rw-r--   0 root         (0)     1003      905 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/tests/data/favicon.ico
--rw-rw-r--   0 root         (0)     1003     2368 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/tests/data/file.txt
--rw-rw-r--   0 root         (0)     1003     2368 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/tests/data/gzipped.txt
--rw-rw-r--   0 root         (0)     1003       89 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/tests/data/gzipped.txt.gz
--rw-rw-r--   0 root         (0)     1003  1364156 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/tests/data/image1.jpg
--rw-rw-r--   0 root         (0)     1003   697286 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/tests/data/image2.jpg
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-19 21:32:45.368633 google-resumable-media-2.4.1/tests/system/
--rw-rw-r--   0 root         (0)     1003      575 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/tests/system/__init__.py
--rw-rw-r--   0 root         (0)     1003     3340 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/tests/system/credentials.json.enc
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-19 21:32:45.372634 google-resumable-media-2.4.1/tests/system/requests/
--rw-rw-r--   0 root         (0)     1003      575 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/tests/system/requests/__init__.py
--rw-rw-r--   0 root         (0)     1003     1966 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/tests/system/requests/conftest.py
--rw-rw-r--   0 root         (0)     1003    23241 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/tests/system/requests/test_download.py
--rw-rw-r--   0 root         (0)     1003    26788 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/tests/system/requests/test_upload.py
--rw-rw-r--   0 root         (0)     1003     2624 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/tests/system/utils.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-19 21:32:45.372634 google-resumable-media-2.4.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      575 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-19 21:32:45.372634 google-resumable-media-2.4.1/tests/unit/requests/
--rw-rw-r--   0 root         (0)     1003      575 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/tests/unit/requests/__init__.py
--rw-rw-r--   0 root         (0)     1003    14206 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/tests/unit/requests/test__helpers.py
--rw-rw-r--   0 root         (0)     1003    44281 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/tests/unit/requests/test_download.py
--rw-rw-r--   0 root         (0)     1003    12472 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/tests/unit/requests/test_upload.py
--rw-rw-r--   0 root         (0)     1003    27192 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/tests/unit/test__download.py
--rw-rw-r--   0 root         (0)     1003    17824 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/tests/unit/test__helpers.py
--rw-rw-r--   0 root         (0)     1003    48693 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/tests/unit/test__upload.py
--rw-rw-r--   0 root         (0)     1003     3425 2023-01-19 21:29:29.000000 google-resumable-media-2.4.1/tests/unit/test_common.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-24 19:02:52.186299 google-resumable-media-2.5.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      111 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     1884 2023-04-24 19:02:52.186299 google-resumable-media-2.5.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003      964 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-24 19:02:52.174298 google-resumable-media-2.5.0/google/
+-rw-rw-r--   0 root         (0)     1003      764 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/google/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-24 19:02:52.178299 google-resumable-media-2.5.0/google/_async_resumable_media/
+-rw-rw-r--   0 root         (0)     1003     1736 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/google/_async_resumable_media/__init__.py
+-rw-rw-r--   0 root         (0)     1003    20354 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/google/_async_resumable_media/_download.py
+-rw-rw-r--   0 root         (0)     1003     6572 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/google/_async_resumable_media/_helpers.py
+-rw-rw-r--   0 root         (0)     1003    37337 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/google/_async_resumable_media/_upload.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-24 19:02:52.178299 google-resumable-media-2.5.0/google/_async_resumable_media/requests/
+-rw-rw-r--   0 root         (0)     1003    21652 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/google/_async_resumable_media/requests/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5117 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/google/_async_resumable_media/requests/_request_helpers.py
+-rw-rw-r--   0 root         (0)     1003    18751 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/google/_async_resumable_media/requests/download.py
+-rw-rw-r--   0 root         (0)     1003    19252 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/google/_async_resumable_media/requests/upload.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-24 19:02:52.178299 google-resumable-media-2.5.0/google/resumable_media/
+-rw-rw-r--   0 root         (0)     1003     1736 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/google/resumable_media/__init__.py
+-rw-rw-r--   0 root         (0)     1003    20656 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/google/resumable_media/_download.py
+-rw-rw-r--   0 root         (0)     1003    13439 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/google/resumable_media/_helpers.py
+-rw-rw-r--   0 root         (0)     1003    39465 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/google/resumable_media/_upload.py
+-rw-rw-r--   0 root         (0)     1003     6191 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/google/resumable_media/common.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-24 19:02:52.178299 google-resumable-media-2.5.0/google/resumable_media/requests/
+-rw-rw-r--   0 root         (0)     1003    21603 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/google/resumable_media/requests/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6371 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/google/resumable_media/requests/_request_helpers.py
+-rw-rw-r--   0 root         (0)     1003    26433 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/google/resumable_media/requests/download.py
+-rw-rw-r--   0 root         (0)     1003    20858 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/google/resumable_media/requests/upload.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-24 19:02:52.182299 google-resumable-media-2.5.0/google_resumable_media.egg-info/
+-rw-r--r--   0 root         (0)     1003     1884 2023-04-24 19:02:52.000000 google-resumable-media-2.5.0/google_resumable_media.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1783 2023-04-24 19:02:52.000000 google-resumable-media-2.5.0/google_resumable_media.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-04-24 19:02:52.000000 google-resumable-media-2.5.0/google_resumable_media.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-04-24 19:02:52.000000 google-resumable-media-2.5.0/google_resumable_media.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-04-24 19:02:52.000000 google-resumable-media-2.5.0/google_resumable_media.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      102 2023-04-24 19:02:52.000000 google-resumable-media-2.5.0/google_resumable_media.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-04-24 19:02:52.000000 google-resumable-media-2.5.0/google_resumable_media.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003      104 2023-04-24 19:02:52.186299 google-resumable-media-2.5.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2131 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-24 19:02:52.182299 google-resumable-media-2.5.0/tests/
+-rw-rw-r--   0 root         (0)     1003      575 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-24 19:02:52.182299 google-resumable-media-2.5.0/tests/data/
+-rw-rw-r--   0 root         (0)     1003      905 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/tests/data/favicon.ico
+-rw-rw-r--   0 root         (0)     1003     2368 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/tests/data/file.txt
+-rw-rw-r--   0 root         (0)     1003     2368 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/tests/data/gzipped.txt
+-rw-rw-r--   0 root         (0)     1003       89 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/tests/data/gzipped.txt.gz
+-rw-rw-r--   0 root         (0)     1003  1364156 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/tests/data/image1.jpg
+-rw-rw-r--   0 root         (0)     1003   697286 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/tests/data/image2.jpg
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-24 19:02:52.186299 google-resumable-media-2.5.0/tests/system/
+-rw-rw-r--   0 root         (0)     1003      575 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/tests/system/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3340 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/tests/system/credentials.json.enc
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-24 19:02:52.186299 google-resumable-media-2.5.0/tests/system/requests/
+-rw-rw-r--   0 root         (0)     1003      575 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/tests/system/requests/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1966 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/tests/system/requests/conftest.py
+-rw-rw-r--   0 root         (0)     1003    23241 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/tests/system/requests/test_download.py
+-rw-rw-r--   0 root         (0)     1003    26788 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/tests/system/requests/test_upload.py
+-rw-rw-r--   0 root         (0)     1003     2624 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/tests/system/utils.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-24 19:02:52.186299 google-resumable-media-2.5.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      575 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-04-24 19:02:52.186299 google-resumable-media-2.5.0/tests/unit/requests/
+-rw-rw-r--   0 root         (0)     1003      575 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/tests/unit/requests/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14607 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/tests/unit/requests/test__helpers.py
+-rw-rw-r--   0 root         (0)     1003    44281 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/tests/unit/requests/test_download.py
+-rw-rw-r--   0 root         (0)     1003    12472 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/tests/unit/requests/test_upload.py
+-rw-rw-r--   0 root         (0)     1003    27192 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/tests/unit/test__download.py
+-rw-rw-r--   0 root         (0)     1003    17824 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/tests/unit/test__helpers.py
+-rw-rw-r--   0 root         (0)     1003    48693 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/tests/unit/test__upload.py
+-rw-rw-r--   0 root         (0)     1003     3425 2023-04-24 19:00:19.000000 google-resumable-media-2.5.0/tests/unit/test_common.py
```

### Comparing `google-resumable-media-2.4.1/LICENSE` & `google-resumable-media-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/PKG-INFO` & `google-resumable-media-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-resumable-media
-Version: 2.4.1
+Version: 2.5.0
 Summary: Utilities for Google Media Downloads and Resumable Uploads
 Home-page: https://github.com/googleapis/google-resumable-media-python
 Author: Google Cloud Platform
 Author-email: googleapis-publisher@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-resumable-media-2.4.1/README.rst` & `google-resumable-media-2.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/google/__init__.py` & `google-resumable-media-2.5.0/google/__init__.py`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/google/_async_resumable_media/__init__.py` & `google-resumable-media-2.5.0/google/_async_resumable_media/__init__.py`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/google/_async_resumable_media/_download.py` & `google-resumable-media-2.5.0/google/_async_resumable_media/_download.py`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/google/_async_resumable_media/_helpers.py` & `google-resumable-media-2.5.0/google/_async_resumable_media/_helpers.py`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/google/_async_resumable_media/_upload.py` & `google-resumable-media-2.5.0/google/_async_resumable_media/_upload.py`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/google/_async_resumable_media/requests/__init__.py` & `google-resumable-media-2.5.0/google/_async_resumable_media/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/google/_async_resumable_media/requests/_request_helpers.py` & `google-resumable-media-2.5.0/google/_async_resumable_media/requests/_request_helpers.py`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/google/_async_resumable_media/requests/download.py` & `google-resumable-media-2.5.0/google/_async_resumable_media/requests/download.py`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/google/_async_resumable_media/requests/upload.py` & `google-resumable-media-2.5.0/google/_async_resumable_media/requests/upload.py`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/google/resumable_media/__init__.py` & `google-resumable-media-2.5.0/google/resumable_media/__init__.py`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/google/resumable_media/_download.py` & `google-resumable-media-2.5.0/google/resumable_media/_download.py`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/google/resumable_media/_helpers.py` & `google-resumable-media-2.5.0/google/resumable_media/_helpers.py`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/google/resumable_media/_upload.py` & `google-resumable-media-2.5.0/google/resumable_media/_upload.py`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/google/resumable_media/common.py` & `google-resumable-media-2.5.0/google/resumable_media/common.py`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/google/resumable_media/requests/__init__.py` & `google-resumable-media-2.5.0/google/resumable_media/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/google/resumable_media/requests/_request_helpers.py` & `google-resumable-media-2.5.0/google/resumable_media/requests/_request_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 
 """Shared utilities used by both downloads and uploads.
 
 This utilities are explicitly catered to ``requests``-like transports.
 """
 
+import http.client
 import requests.exceptions
 import urllib3.exceptions  # type: ignore
 
 import time
 
 from google.resumable_media import common
 from google.resumable_media import _helpers
@@ -31,18 +32,24 @@
 # (connect() call on socket). Avoid setting this to a multiple of 3 to not
 # Align with TCP Retransmission timing. (typically 2.5-3s)
 _DEFAULT_CONNECT_TIMEOUT = 61
 # The number of seconds to wait between bytes sent from the server.
 _DEFAULT_READ_TIMEOUT = 60
 
 _CONNECTION_ERROR_CLASSES = (
+    http.client.BadStatusLine,
+    http.client.IncompleteRead,
+    http.client.ResponseNotReady,
     requests.exceptions.ConnectionError,
     requests.exceptions.ChunkedEncodingError,
     requests.exceptions.Timeout,
+    urllib3.exceptions.PoolError,
     urllib3.exceptions.ProtocolError,
+    urllib3.exceptions.SSLError,
+    urllib3.exceptions.TimeoutError,
     ConnectionError,  # Python 3.x only, superclass of ConnectionResetError.
 )
 
 
 class RequestsMixin(object):
     """Mix-in class implementing ``requests``-specific behavior.
```

### Comparing `google-resumable-media-2.4.1/google/resumable_media/requests/download.py` & `google-resumable-media-2.5.0/google/resumable_media/requests/download.py`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/google/resumable_media/requests/upload.py` & `google-resumable-media-2.5.0/google/resumable_media/requests/upload.py`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/google_resumable_media.egg-info/PKG-INFO` & `google-resumable-media-2.5.0/google_resumable_media.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-resumable-media
-Version: 2.4.1
+Version: 2.5.0
 Summary: Utilities for Google Media Downloads and Resumable Uploads
 Home-page: https://github.com/googleapis/google-resumable-media-python
 Author: Google Cloud Platform
 Author-email: googleapis-publisher@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-resumable-media-2.4.1/google_resumable_media.egg-info/SOURCES.txt` & `google-resumable-media-2.5.0/google_resumable_media.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/setup.py` & `google-resumable-media-2.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         'requests >= 2.18.0, < 3.0.0dev',
     ],
     'aiohttp': 'aiohttp >= 3.6.2, < 4.0.0dev'
 }
 
 setuptools.setup(
     name='google-resumable-media',
-    version = "2.4.1",
+    version = "2.5.0",
     description='Utilities for Google Media Downloads and Resumable Uploads',
     author='Google Cloud Platform',
     author_email='googleapis-publisher@google.com',
     long_description=README,
     namespace_packages=['google'],
     scripts=[],
     url='https://github.com/googleapis/google-resumable-media-python',
```

### Comparing `google-resumable-media-2.4.1/tests/__init__.py` & `google-resumable-media-2.5.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/tests/data/favicon.ico` & `google-resumable-media-2.5.0/tests/data/favicon.ico`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/tests/data/file.txt` & `google-resumable-media-2.5.0/tests/data/file.txt`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/tests/data/gzipped.txt` & `google-resumable-media-2.5.0/tests/data/gzipped.txt`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/tests/data/image1.jpg` & `google-resumable-media-2.5.0/tests/data/image1.jpg`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/tests/data/image2.jpg` & `google-resumable-media-2.5.0/tests/data/image2.jpg`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/tests/system/__init__.py` & `google-resumable-media-2.5.0/tests/system/__init__.py`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/tests/system/credentials.json.enc` & `google-resumable-media-2.5.0/tests/system/credentials.json.enc`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/tests/system/requests/__init__.py` & `google-resumable-media-2.5.0/tests/system/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/tests/system/requests/conftest.py` & `google-resumable-media-2.5.0/tests/system/requests/conftest.py`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/tests/system/requests/test_download.py` & `google-resumable-media-2.5.0/tests/system/requests/test_download.py`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/tests/system/requests/test_upload.py` & `google-resumable-media-2.5.0/tests/system/requests/test_upload.py`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/tests/system/utils.py` & `google-resumable-media-2.5.0/tests/system/utils.py`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/tests/unit/__init__.py` & `google-resumable-media-2.5.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/tests/unit/requests/__init__.py` & `google-resumable-media-2.5.0/tests/unit/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/tests/unit/requests/test__helpers.py` & `google-resumable-media-2.5.0/tests/unit/requests/test__helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -161,105 +161,109 @@
         )  # previous delay 3 * multiplier 4 + jitter 0.625
         sleep_mock.assert_any_call(
             48.375
         )  # previous delay 12 * multiplier 4 + jitter 0.375
 
     @mock.patch("time.sleep")
     @mock.patch("random.randint")
-    def test_success_with_retry_connection_error(self, randint_mock, sleep_mock):
-        randint_mock.side_effect = [125, 625, 375]
+    def test_retry_success_http_standard_lib_connection_errors(
+        self, randint_mock, sleep_mock
+    ):
+        randint_mock.side_effect = [125, 625, 500, 875, 375]
 
-        response = _make_response(http.client.NOT_FOUND)
+        status_code = int(http.client.OK)
+        response = _make_response(status_code)
         responses = [
-            ConnectionResetError,  # Subclass of ConnectionError
-            urllib3.exceptions.ConnectionError,
-            requests.exceptions.ConnectionError,
+            http.client.BadStatusLine(""),
+            http.client.IncompleteRead(""),
+            http.client.ResponseNotReady,
+            ConnectionError,
             response,
         ]
         func = mock.Mock(side_effect=responses, spec=[])
 
         retry_strategy = common.RetryStrategy()
         ret_val = _request_helpers.wait_and_retry(
             func, _get_status_code, retry_strategy
         )
 
         assert ret_val == responses[-1]
-
-        assert func.call_count == 4
-        assert func.mock_calls == [mock.call()] * 4
-
-        assert randint_mock.call_count == 3
-        assert randint_mock.mock_calls == [mock.call(0, 1000)] * 3
-
-        assert sleep_mock.call_count == 3
+        assert func.call_count == 5
+        assert func.mock_calls == [mock.call()] * 5
+        assert randint_mock.call_count == 4
+        assert randint_mock.mock_calls == [mock.call(0, 1000)] * 4
+        assert sleep_mock.call_count == 4
         sleep_mock.assert_any_call(1.125)
         sleep_mock.assert_any_call(2.625)
-        sleep_mock.assert_any_call(4.375)
+        sleep_mock.assert_any_call(4.500)
+        sleep_mock.assert_any_call(8.875)
 
     @mock.patch("time.sleep")
     @mock.patch("random.randint")
-    def test_success_with_retry_chunked_encoding_error(self, randint_mock, sleep_mock):
-        randint_mock.side_effect = [125, 625, 375]
+    def test_retry_success_requests_lib_connection_errors(
+        self, randint_mock, sleep_mock
+    ):
+        randint_mock.side_effect = [125, 625, 500, 875]
 
         status_code = int(http.client.OK)
         response = _make_response(status_code)
         responses = [
+            requests.exceptions.ConnectionError,
             requests.exceptions.ChunkedEncodingError,
-            requests.exceptions.ChunkedEncodingError,
+            requests.exceptions.Timeout,
             response,
         ]
         func = mock.Mock(side_effect=responses, spec=[])
 
         retry_strategy = common.RetryStrategy()
         ret_val = _request_helpers.wait_and_retry(
             func, _get_status_code, retry_strategy
         )
 
         assert ret_val == responses[-1]
-
-        assert func.call_count == 3
-        assert func.mock_calls == [mock.call()] * 3
-
-        assert randint_mock.call_count == 2
-        assert randint_mock.mock_calls == [mock.call(0, 1000)] * 2
-
-        assert sleep_mock.call_count == 2
+        assert func.call_count == 4
+        assert func.mock_calls == [mock.call()] * 4
+        assert randint_mock.call_count == 3
+        assert randint_mock.mock_calls == [mock.call(0, 1000)] * 3
+        assert sleep_mock.call_count == 3
         sleep_mock.assert_any_call(1.125)
         sleep_mock.assert_any_call(2.625)
+        sleep_mock.assert_any_call(4.500)
 
     @mock.patch("time.sleep")
     @mock.patch("random.randint")
-    def test_success_with_retry_client_timeout(self, randint_mock, sleep_mock):
-        randint_mock.side_effect = [125, 625, 375]
+    def test_retry_success_urllib3_connection_errors(self, randint_mock, sleep_mock):
+        randint_mock.side_effect = [125, 625, 500, 875, 375]
 
         status_code = int(http.client.OK)
         response = _make_response(status_code)
         responses = [
-            requests.exceptions.Timeout,
-            requests.exceptions.Timeout,
+            urllib3.exceptions.PoolError(None, ""),
+            urllib3.exceptions.ProtocolError,
+            urllib3.exceptions.SSLError,
+            urllib3.exceptions.TimeoutError,
             response,
         ]
         func = mock.Mock(side_effect=responses, spec=[])
 
         retry_strategy = common.RetryStrategy()
         ret_val = _request_helpers.wait_and_retry(
             func, _get_status_code, retry_strategy
         )
 
         assert ret_val == responses[-1]
-
-        assert func.call_count == 3
-        assert func.mock_calls == [mock.call()] * 3
-
-        assert randint_mock.call_count == 2
-        assert randint_mock.mock_calls == [mock.call(0, 1000)] * 2
-
-        assert sleep_mock.call_count == 2
+        assert func.call_count == 5
+        assert func.mock_calls == [mock.call()] * 5
+        assert randint_mock.call_count == 4
+        assert randint_mock.mock_calls == [mock.call(0, 1000)] * 4
+        assert sleep_mock.call_count == 4
         sleep_mock.assert_any_call(1.125)
         sleep_mock.assert_any_call(2.625)
+        sleep_mock.assert_any_call(4.500)
+        sleep_mock.assert_any_call(8.875)
 
     @mock.patch("time.sleep")
     @mock.patch("random.randint")
     def test_retry_exceeds_max_cumulative(self, randint_mock, sleep_mock):
         randint_mock.side_effect = [875, 0, 375, 500, 500, 250, 125]
 
         status_codes = (
```

### Comparing `google-resumable-media-2.4.1/tests/unit/requests/test_download.py` & `google-resumable-media-2.5.0/tests/unit/requests/test_download.py`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/tests/unit/requests/test_upload.py` & `google-resumable-media-2.5.0/tests/unit/requests/test_upload.py`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/tests/unit/test__download.py` & `google-resumable-media-2.5.0/tests/unit/test__download.py`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/tests/unit/test__helpers.py` & `google-resumable-media-2.5.0/tests/unit/test__helpers.py`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/tests/unit/test__upload.py` & `google-resumable-media-2.5.0/tests/unit/test__upload.py`

 * *Files identical despite different names*

### Comparing `google-resumable-media-2.4.1/tests/unit/test_common.py` & `google-resumable-media-2.5.0/tests/unit/test_common.py`

 * *Files identical despite different names*


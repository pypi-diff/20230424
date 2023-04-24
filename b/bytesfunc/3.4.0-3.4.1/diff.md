# Comparing `tmp/bytesfunc-3.4.0.tar.gz` & `tmp/bytesfunc-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytesfunc-3.4.0.tar", last modified: Mon Dec 12 04:23:13 2022, max compression
+gzip compressed data, was "bytesfunc-3.4.1.tar", last modified: Sun Apr 23 02:31:06 2023, max compression
```

## Comparing `bytesfunc-3.4.0.tar` & `bytesfunc-3.4.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2022-12-12 04:23:13.181922 bytesfunc-3.4.0/
--rw-rw-r--   0 me        (1000) me        (1000)       99 2019-10-29 23:53:37.000000 bytesfunc-3.4.0/COPYRIGHT
--rw-rw-r--   0 me        (1000) me        (1000)    11354 2015-05-15 01:35:41.000000 bytesfunc-3.4.0/LICENSE
--rw-rw-r--   0 me        (1000) me        (1000)      109 2022-12-06 06:27:06.000000 bytesfunc-3.4.0/MANIFEST.in
--rw-rw-r--   0 me        (1000) me        (1000)    12610 2022-12-12 04:23:13.181922 bytesfunc-3.4.0/PKG-INFO
--rw-rw-r--   0 me        (1000) me        (1000)    11997 2022-12-12 04:22:32.000000 bytesfunc-3.4.0/README.rst
--rw-rw-r--   0 me        (1000) me        (1000)        6 2022-12-06 05:42:40.000000 bytesfunc-3.4.0/VERSION.TXT
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2022-12-12 04:23:13.169922 bytesfunc-3.4.0/bytesfunc/
--rw-r--r--   0 me        (1000) me        (1000)      941 2022-12-12 04:23:08.000000 bytesfunc-3.4.0/bytesfunc/__init__.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2022-12-12 04:23:13.169922 bytesfunc-3.4.0/bytesfunc.egg-info/
--rw-rw-r--   0 me        (1000) me        (1000)    12610 2022-12-12 04:23:13.000000 bytesfunc-3.4.0/bytesfunc.egg-info/PKG-INFO
--rw-rw-r--   0 me        (1000) me        (1000)      887 2022-12-12 04:23:13.000000 bytesfunc-3.4.0/bytesfunc.egg-info/SOURCES.txt
--rw-rw-r--   0 me        (1000) me        (1000)        1 2022-12-12 04:23:13.000000 bytesfunc-3.4.0/bytesfunc.egg-info/dependency_links.txt
--rw-rw-r--   0 me        (1000) me        (1000)      109 2022-12-12 04:23:13.000000 bytesfunc-3.4.0/bytesfunc.egg-info/top_level.txt
--rw-rw-r--   0 me        (1000) me        (1000)       84 2022-11-08 08:03:58.000000 bytesfunc-3.4.0/pyproject.toml
--rw-rw-r--   0 me        (1000) me        (1000)       38 2022-12-12 04:23:13.181922 bytesfunc-3.4.0/setup.cfg
--rwxrwxr-x   0 me        (1000) me        (1000)     6501 2022-12-09 06:08:00.000000 bytesfunc-3.4.0/setup.py
--rw-rw-r--   0 me        (1000) me        (1000)     2186 2022-12-05 00:14:57.000000 bytesfunc-3.4.0/setupuser.bat
--rwxrwxr-x   0 me        (1000) me        (1000)      622 2022-12-09 06:33:37.000000 bytesfunc-3.4.0/setupuser.sh
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2022-12-12 04:23:13.181922 bytesfunc-3.4.0/src/
--rw-rw-r--   0 me        (1000) me        (1000)    35586 2022-07-11 04:42:32.000000 bytesfunc-3.4.0/src/and_.c
--rw-rw-r--   0 me        (1000) me        (1000)     2017 2019-07-06 20:56:44.000000 bytesfunc-3.4.0/src/arrayops.c
--rw-rw-r--   0 me        (1000) me        (1000)     1358 2019-07-06 20:56:52.000000 bytesfunc-3.4.0/src/arrayops.h
--rw-rw-r--   0 me        (1000) me        (1000)    53728 2022-07-11 04:42:32.000000 bytesfunc-3.4.0/src/ball.c
--rw-rw-r--   0 me        (1000) me        (1000)    52574 2022-07-11 04:42:32.000000 bytesfunc-3.4.0/src/bany.c
--rw-rw-r--   0 me        (1000) me        (1000)    10580 2022-07-11 04:42:32.000000 bytesfunc-3.4.0/src/bmax.c
--rw-rw-r--   0 me        (1000) me        (1000)    10580 2022-07-11 04:42:32.000000 bytesfunc-3.4.0/src/bmin.c
--rw-rw-r--   0 me        (1000) me        (1000)    14081 2022-07-11 04:42:32.000000 bytesfunc-3.4.0/src/bsum.c
--rw-r--r--   0 me        (1000) me        (1000)     2084 2020-01-29 05:32:56.000000 bytesfunc-3.4.0/src/byteserrs.c
--rw-r--r--   0 me        (1000) me        (1000)     1806 2020-02-17 05:55:52.000000 bytesfunc-3.4.0/src/byteserrs.h
--rw-rw-r--   0 me        (1000) me        (1000)     5666 2022-07-10 05:45:02.000000 bytesfunc-3.4.0/src/bytesparams_allany.c
--rw-rw-r--   0 me        (1000) me        (1000)     1867 2022-07-10 05:44:41.000000 bytesfunc-3.4.0/src/bytesparams_allany.h
--rw-r--r--   0 me        (1000) me        (1000)     7868 2022-07-10 06:40:16.000000 bytesfunc-3.4.0/src/bytesparams_base.c
--rw-r--r--   0 me        (1000) me        (1000)     2305 2022-07-10 04:21:09.000000 bytesfunc-3.4.0/src/bytesparams_base.h
--rw-rw-r--   0 me        (1000) me        (1000)     4646 2022-07-10 04:24:31.000000 bytesfunc-3.4.0/src/bytesparams_bsum.c
--rw-rw-r--   0 me        (1000) me        (1000)     1803 2022-07-10 04:20:29.000000 bytesfunc-3.4.0/src/bytesparams_bsum.h
--rw-r--r--   0 me        (1000) me        (1000)     7410 2022-07-10 07:11:10.000000 bytesfunc-3.4.0/src/bytesparams_comp.c
--rw-r--r--   0 me        (1000) me        (1000)     2010 2022-07-10 04:21:31.000000 bytesfunc-3.4.0/src/bytesparams_comp.h
--rw-rw-r--   0 me        (1000) me        (1000)     5973 2022-07-06 06:55:02.000000 bytesfunc-3.4.0/src/bytesparams_invert.c
--rw-rw-r--   0 me        (1000) me        (1000)     1872 2022-07-06 06:54:48.000000 bytesfunc-3.4.0/src/bytesparams_invert.h
--rw-rw-r--   0 me        (1000) me        (1000)     9701 2022-07-10 07:21:48.000000 bytesfunc-3.4.0/src/bytesparams_two.c
--rw-rw-r--   0 me        (1000) me        (1000)     2154 2022-07-11 00:07:16.000000 bytesfunc-3.4.0/src/bytesparams_two.h
--rw-r--r--   0 me        (1000) me        (1000)     4622 2022-07-10 04:23:17.000000 bytesfunc-3.4.0/src/bytesparams_valoutsimd.c
--rw-r--r--   0 me        (1000) me        (1000)     1806 2022-07-10 04:20:44.000000 bytesfunc-3.4.0/src/bytesparams_valoutsimd.h
--rw-rw-r--   0 me        (1000) me        (1000)    24280 2022-07-11 04:42:32.000000 bytesfunc-3.4.0/src/eq.c
--rw-rw-r--   0 me        (1000) me        (1000)    56103 2022-07-11 04:42:32.000000 bytesfunc-3.4.0/src/findindex.c
--rw-rw-r--   0 me        (1000) me        (1000)    24788 2022-07-11 04:42:32.000000 bytesfunc-3.4.0/src/ge.c
--rw-rw-r--   0 me        (1000) me        (1000)    25358 2022-07-11 04:42:32.000000 bytesfunc-3.4.0/src/gt.c
--rw-rw-r--   0 me        (1000) me        (1000)    14930 2022-07-11 04:42:32.000000 bytesfunc-3.4.0/src/invert.c
--rw-rw-r--   0 me        (1000) me        (1000)    24792 2022-07-11 04:42:32.000000 bytesfunc-3.4.0/src/le.c
--rw-rw-r--   0 me        (1000) me        (1000)    20329 2022-07-11 04:42:32.000000 bytesfunc-3.4.0/src/lshift.c
--rw-rw-r--   0 me        (1000) me        (1000)    25362 2022-07-11 04:42:32.000000 bytesfunc-3.4.0/src/lt.c
--rw-rw-r--   0 me        (1000) me        (1000)    24292 2022-07-11 04:42:32.000000 bytesfunc-3.4.0/src/ne.c
--rw-rw-r--   0 me        (1000) me        (1000)    35494 2022-07-11 04:42:32.000000 bytesfunc-3.4.0/src/or_.c
--rw-rw-r--   0 me        (1000) me        (1000)    20333 2022-07-11 04:42:32.000000 bytesfunc-3.4.0/src/rshift.c
--rw-rw-r--   0 me        (1000) me        (1000)     4366 2022-07-06 03:28:38.000000 bytesfunc-3.4.0/src/simddefs.h
--rw-rw-r--   0 me        (1000) me        (1000)     4915 2022-04-23 05:47:53.000000 bytesfunc-3.4.0/src/simdsupport.c
--rw-rw-r--   0 me        (1000) me        (1000)    35500 2022-07-11 04:42:32.000000 bytesfunc-3.4.0/src/xor.c
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-04-23 02:31:06.689328 bytesfunc-3.4.1/
+-rw-rw-r--   0 me        (1000) me        (1000)       99 2019-10-29 23:53:37.000000 bytesfunc-3.4.1/COPYRIGHT
+-rw-rw-r--   0 me        (1000) me        (1000)    11354 2015-05-15 01:35:41.000000 bytesfunc-3.4.1/LICENSE
+-rw-rw-r--   0 me        (1000) me        (1000)      109 2022-12-06 06:27:06.000000 bytesfunc-3.4.1/MANIFEST.in
+-rw-rw-r--   0 me        (1000) me        (1000)    14191 2023-04-23 02:31:06.689328 bytesfunc-3.4.1/PKG-INFO
+-rw-rw-r--   0 me        (1000) me        (1000)    13578 2023-04-23 02:23:29.000000 bytesfunc-3.4.1/README.rst
+-rw-rw-r--   0 me        (1000) me        (1000)        6 2023-04-23 01:36:42.000000 bytesfunc-3.4.1/VERSION.TXT
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-04-23 02:31:06.677328 bytesfunc-3.4.1/bytesfunc/
+-rw-r--r--   0 me        (1000) me        (1000)      941 2023-04-23 02:31:02.000000 bytesfunc-3.4.1/bytesfunc/__init__.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-04-23 02:31:06.677328 bytesfunc-3.4.1/bytesfunc.egg-info/
+-rw-rw-r--   0 me        (1000) me        (1000)    14191 2023-04-23 02:31:06.000000 bytesfunc-3.4.1/bytesfunc.egg-info/PKG-INFO
+-rw-rw-r--   0 me        (1000) me        (1000)      887 2023-04-23 02:31:06.000000 bytesfunc-3.4.1/bytesfunc.egg-info/SOURCES.txt
+-rw-rw-r--   0 me        (1000) me        (1000)        1 2023-04-23 02:31:06.000000 bytesfunc-3.4.1/bytesfunc.egg-info/dependency_links.txt
+-rw-rw-r--   0 me        (1000) me        (1000)      109 2023-04-23 02:31:06.000000 bytesfunc-3.4.1/bytesfunc.egg-info/top_level.txt
+-rw-rw-r--   0 me        (1000) me        (1000)       84 2022-11-08 08:03:58.000000 bytesfunc-3.4.1/pyproject.toml
+-rw-rw-r--   0 me        (1000) me        (1000)       38 2023-04-23 02:31:06.689328 bytesfunc-3.4.1/setup.cfg
+-rwxrwxr-x   0 me        (1000) me        (1000)     6501 2022-12-09 06:08:00.000000 bytesfunc-3.4.1/setup.py
+-rw-rw-r--   0 me        (1000) me        (1000)     2186 2022-12-05 00:14:57.000000 bytesfunc-3.4.1/setupuser.bat
+-rwxrwxr-x   0 me        (1000) me        (1000)      622 2022-12-09 06:33:37.000000 bytesfunc-3.4.1/setupuser.sh
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-04-23 02:31:06.689328 bytesfunc-3.4.1/src/
+-rw-rw-r--   0 me        (1000) me        (1000)    35586 2022-07-11 04:42:32.000000 bytesfunc-3.4.1/src/and_.c
+-rw-rw-r--   0 me        (1000) me        (1000)     2017 2019-07-06 20:56:44.000000 bytesfunc-3.4.1/src/arrayops.c
+-rw-rw-r--   0 me        (1000) me        (1000)     1358 2019-07-06 20:56:52.000000 bytesfunc-3.4.1/src/arrayops.h
+-rw-rw-r--   0 me        (1000) me        (1000)    53728 2022-07-11 04:42:32.000000 bytesfunc-3.4.1/src/ball.c
+-rw-rw-r--   0 me        (1000) me        (1000)    52574 2022-07-11 04:42:32.000000 bytesfunc-3.4.1/src/bany.c
+-rw-rw-r--   0 me        (1000) me        (1000)    10580 2022-07-11 04:42:32.000000 bytesfunc-3.4.1/src/bmax.c
+-rw-rw-r--   0 me        (1000) me        (1000)    10580 2022-07-11 04:42:32.000000 bytesfunc-3.4.1/src/bmin.c
+-rw-rw-r--   0 me        (1000) me        (1000)    14081 2022-07-11 04:42:32.000000 bytesfunc-3.4.1/src/bsum.c
+-rw-r--r--   0 me        (1000) me        (1000)     2084 2020-01-29 05:32:56.000000 bytesfunc-3.4.1/src/byteserrs.c
+-rw-r--r--   0 me        (1000) me        (1000)     1806 2020-02-17 05:55:52.000000 bytesfunc-3.4.1/src/byteserrs.h
+-rw-rw-r--   0 me        (1000) me        (1000)     5666 2022-07-10 05:45:02.000000 bytesfunc-3.4.1/src/bytesparams_allany.c
+-rw-rw-r--   0 me        (1000) me        (1000)     1867 2022-07-10 05:44:41.000000 bytesfunc-3.4.1/src/bytesparams_allany.h
+-rw-r--r--   0 me        (1000) me        (1000)     7868 2022-07-10 06:40:16.000000 bytesfunc-3.4.1/src/bytesparams_base.c
+-rw-r--r--   0 me        (1000) me        (1000)     2305 2022-07-10 04:21:09.000000 bytesfunc-3.4.1/src/bytesparams_base.h
+-rw-rw-r--   0 me        (1000) me        (1000)     4646 2022-07-10 04:24:31.000000 bytesfunc-3.4.1/src/bytesparams_bsum.c
+-rw-rw-r--   0 me        (1000) me        (1000)     1803 2022-07-10 04:20:29.000000 bytesfunc-3.4.1/src/bytesparams_bsum.h
+-rw-r--r--   0 me        (1000) me        (1000)     7410 2022-07-10 07:11:10.000000 bytesfunc-3.4.1/src/bytesparams_comp.c
+-rw-r--r--   0 me        (1000) me        (1000)     2010 2022-07-10 04:21:31.000000 bytesfunc-3.4.1/src/bytesparams_comp.h
+-rw-rw-r--   0 me        (1000) me        (1000)     5973 2022-07-06 06:55:02.000000 bytesfunc-3.4.1/src/bytesparams_invert.c
+-rw-rw-r--   0 me        (1000) me        (1000)     1872 2022-07-06 06:54:48.000000 bytesfunc-3.4.1/src/bytesparams_invert.h
+-rw-rw-r--   0 me        (1000) me        (1000)     9701 2022-07-10 07:21:48.000000 bytesfunc-3.4.1/src/bytesparams_two.c
+-rw-rw-r--   0 me        (1000) me        (1000)     2154 2022-07-11 00:07:16.000000 bytesfunc-3.4.1/src/bytesparams_two.h
+-rw-r--r--   0 me        (1000) me        (1000)     4622 2022-07-10 04:23:17.000000 bytesfunc-3.4.1/src/bytesparams_valoutsimd.c
+-rw-r--r--   0 me        (1000) me        (1000)     1806 2022-07-10 04:20:44.000000 bytesfunc-3.4.1/src/bytesparams_valoutsimd.h
+-rw-rw-r--   0 me        (1000) me        (1000)    24280 2022-07-11 04:42:32.000000 bytesfunc-3.4.1/src/eq.c
+-rw-rw-r--   0 me        (1000) me        (1000)    56103 2022-07-11 04:42:32.000000 bytesfunc-3.4.1/src/findindex.c
+-rw-rw-r--   0 me        (1000) me        (1000)    24788 2022-07-11 04:42:32.000000 bytesfunc-3.4.1/src/ge.c
+-rw-rw-r--   0 me        (1000) me        (1000)    25358 2022-07-11 04:42:32.000000 bytesfunc-3.4.1/src/gt.c
+-rw-rw-r--   0 me        (1000) me        (1000)    14930 2022-07-11 04:42:32.000000 bytesfunc-3.4.1/src/invert.c
+-rw-rw-r--   0 me        (1000) me        (1000)    24792 2022-07-11 04:42:32.000000 bytesfunc-3.4.1/src/le.c
+-rw-rw-r--   0 me        (1000) me        (1000)    20329 2022-07-11 04:42:32.000000 bytesfunc-3.4.1/src/lshift.c
+-rw-rw-r--   0 me        (1000) me        (1000)    25362 2022-07-11 04:42:32.000000 bytesfunc-3.4.1/src/lt.c
+-rw-rw-r--   0 me        (1000) me        (1000)    24292 2022-07-11 04:42:32.000000 bytesfunc-3.4.1/src/ne.c
+-rw-rw-r--   0 me        (1000) me        (1000)    35494 2022-07-11 04:42:32.000000 bytesfunc-3.4.1/src/or_.c
+-rw-rw-r--   0 me        (1000) me        (1000)    20333 2022-07-11 04:42:32.000000 bytesfunc-3.4.1/src/rshift.c
+-rw-rw-r--   0 me        (1000) me        (1000)     4366 2022-07-06 03:28:38.000000 bytesfunc-3.4.1/src/simddefs.h
+-rw-rw-r--   0 me        (1000) me        (1000)     4915 2022-04-23 05:47:53.000000 bytesfunc-3.4.1/src/simdsupport.c
+-rw-rw-r--   0 me        (1000) me        (1000)    35500 2022-07-11 04:42:32.000000 bytesfunc-3.4.1/src/xor.c
```

### Comparing `bytesfunc-3.4.0/LICENSE` & `bytesfunc-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/PKG-INFO` & `bytesfunc-3.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bytesfunc
-Version: 3.4.0
+Version: 3.4.1
 Summary: Fast bytes and bytearray processing functions
 Home-page: https://github.com/m1griffin/bytesfunc
 Author: M Griffin
 Author-email: m12.griffin@gmail.com
 License: Apache License V2.0
 Keywords: bytes and bytearray functions
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,16 +18,16 @@
 =========
 BytesFunc
 =========
 
 :Authors:
     Michael Griffin
 
-:Version:  3.4.0 for 2022-12-11
-:Copyright: 2014 - 2022
+:Version:  3.4.1 for 2023-04-22
+:Copyright: 2014 - 2023
 :License: This document may be distributed under the Apache 2.0 License.
 :Language: Python 3.6 or later
 
 ---------------------------------------------------------------------
 
 Introduction
 ============
@@ -149,20 +149,20 @@
 
 ======================= ========== ====== =============== ================
 OS                       Hardware   Bits   Compiler        Python Version
 ======================= ========== ====== =============== ================
 Debian 11                i686         32     GCC               3.9.2
 Debian 11                x86_64       64     GCC               3.9.2
 Ubuntu 22.04             x86_64       64     GCC               3.10.6
-Ubuntu 22.10             x86_64       64     GCC               3.10.7
+Ubuntu 23.04             x86_64       64     GCC               3.11.2
 opensuse-leap 15.4       x86_64       64     GCC               3.6.15
-almalinux 9.0            x86_64       64     GCC               3.9.10
-alpine 3.16.2            i686         32     GCC               3.10.5
-FreeBSD 13.1             amd64        64     Clang             3.9.15
-OpenBSD 7.2              amd64        64     Clang             3.9.15
+almalinux 9.1            x86_64       64     GCC               3.9.14
+alpine 3.17.3            i686         32     GCC               3.10.11
+FreeBSD 13.2             amd64        64     Clang             3.9.16
+OpenBSD 7.3              amd64        64     Clang             3.10.10
 MS Windows 10            AMD64        64     MSC               3.11.0
 MS Windows 11            AMD64        64     MSC               3.11.0
 Raspbian 11              armv7l       32     GCC               3.9.2
 Ubuntu 22.04             aarch64      64     GCC               3.10.6
 ======================= ========== ====== =============== ================
 
 amd64 is another name for x86_64 and does not indicate the CPU brand.
@@ -223,18 +223,55 @@
 The setup.py file has platform detection code which it uses to pass the 
 correct flags to the C compiler. For ARM, this includes the CPU type. If you
 are using an ARM CPU type which is not recognized then setup.py may not
 compile in SIMD features. You can experiment with modifying setup.py to add
 new ARM models, but be sure that anything you try is compatible with the 
 existing ones.
 
+
+Installing on Linux with PIP and PEP-668
+----------------------------------------
+PEP-668 (PEPs describe changes to Python) introduced a new feature which can
+affect how packages are installed with PIP. If PIP is configured to be 
+EXTERNALLY-MANAGED it will refuse to install a package outside of a virtual
+environment.
+
+The intention of this is to prevent conflicts between packages which are 
+installed using the system package manager, and ones which are installed using
+PIP.
+
+Linux distros which are affeced by this include the latest versions of Debian
+and Ubuntu.
+
+As this package is a library which is intended to be used by other 
+applications, there is no one right way to install it, whether inside or 
+outside of a virtual environment. Review the options available with PIP to see
+what is suitable for your application.
+
+For testing purposes this package was installed by setting the environment
+variable PIP_BREAK_SYSTEM_PACKAGES to "1", which effectively disables this
+feature in PIP. 
+
+example::
+
+	export PIP_BREAK_SYSTEM_PACKAGES=1
+
+
 ---------------------------------------------------------------------
 
 Release History
 ===============
+* 3.4.1 - Update to testing and support. There were no code. changes. 
+          Ubuntu version updated to 23.04. AlmaLinux updated to 9.1. 
+          Alpine Linux updated to 3.17.3. FreeBSD updated to 13.2. 
+          OpenBSD updated to 7.3. 
+          On Ubuntu 23.04, the installation method has changed due to how 
+          PEP-668 was implemented by Debian and how this affects "pip". 
+          Some other distros may experience the same problems if they made 
+          the same changes. See the README.TxT for details. 
 * 3.4.0 - Added pyproject.toml file to satisfy Python 3.11 requirements.
           Updated build scripts to use python3 -m build instead of calling
           setup.py directly. Test targets were updated, Ubuntu 20.04 was 
           dropped, Ubuntu 22.10 was added, FreeBSD python version upgraded 
           to 3.9, OpenBSD upgraded to 7.2, Windows 10 Python upgraded to 3.11,
           Windows 11 Python upgraded to 3.11. Added __version__ attribute to 
           allow checking package version number at run time. Added version
```

### Comparing `bytesfunc-3.4.0/README.rst` & `bytesfunc-3.4.1/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 =========
 BytesFunc
 =========
 
 :Authors:
     Michael Griffin
 
-:Version:  3.4.0 for 2022-12-11
-:Copyright: 2014 - 2022
+:Version:  3.4.1 for 2023-04-22
+:Copyright: 2014 - 2023
 :License: This document may be distributed under the Apache 2.0 License.
 :Language: Python 3.6 or later
 
 ---------------------------------------------------------------------
 
 Introduction
 ============
@@ -132,20 +132,20 @@
 
 ======================= ========== ====== =============== ================
 OS                       Hardware   Bits   Compiler        Python Version
 ======================= ========== ====== =============== ================
 Debian 11                i686         32     GCC               3.9.2
 Debian 11                x86_64       64     GCC               3.9.2
 Ubuntu 22.04             x86_64       64     GCC               3.10.6
-Ubuntu 22.10             x86_64       64     GCC               3.10.7
+Ubuntu 23.04             x86_64       64     GCC               3.11.2
 opensuse-leap 15.4       x86_64       64     GCC               3.6.15
-almalinux 9.0            x86_64       64     GCC               3.9.10
-alpine 3.16.2            i686         32     GCC               3.10.5
-FreeBSD 13.1             amd64        64     Clang             3.9.15
-OpenBSD 7.2              amd64        64     Clang             3.9.15
+almalinux 9.1            x86_64       64     GCC               3.9.14
+alpine 3.17.3            i686         32     GCC               3.10.11
+FreeBSD 13.2             amd64        64     Clang             3.9.16
+OpenBSD 7.3              amd64        64     Clang             3.10.10
 MS Windows 10            AMD64        64     MSC               3.11.0
 MS Windows 11            AMD64        64     MSC               3.11.0
 Raspbian 11              armv7l       32     GCC               3.9.2
 Ubuntu 22.04             aarch64      64     GCC               3.10.6
 ======================= ========== ====== =============== ================
 
 amd64 is another name for x86_64 and does not indicate the CPU brand.
@@ -206,18 +206,55 @@
 The setup.py file has platform detection code which it uses to pass the 
 correct flags to the C compiler. For ARM, this includes the CPU type. If you
 are using an ARM CPU type which is not recognized then setup.py may not
 compile in SIMD features. You can experiment with modifying setup.py to add
 new ARM models, but be sure that anything you try is compatible with the 
 existing ones.
 
+
+Installing on Linux with PIP and PEP-668
+----------------------------------------
+PEP-668 (PEPs describe changes to Python) introduced a new feature which can
+affect how packages are installed with PIP. If PIP is configured to be 
+EXTERNALLY-MANAGED it will refuse to install a package outside of a virtual
+environment.
+
+The intention of this is to prevent conflicts between packages which are 
+installed using the system package manager, and ones which are installed using
+PIP.
+
+Linux distros which are affeced by this include the latest versions of Debian
+and Ubuntu.
+
+As this package is a library which is intended to be used by other 
+applications, there is no one right way to install it, whether inside or 
+outside of a virtual environment. Review the options available with PIP to see
+what is suitable for your application.
+
+For testing purposes this package was installed by setting the environment
+variable PIP_BREAK_SYSTEM_PACKAGES to "1", which effectively disables this
+feature in PIP. 
+
+example::
+
+	export PIP_BREAK_SYSTEM_PACKAGES=1
+
+
 ---------------------------------------------------------------------
 
 Release History
 ===============
+* 3.4.1 - Update to testing and support. There were no code. changes. 
+          Ubuntu version updated to 23.04. AlmaLinux updated to 9.1. 
+          Alpine Linux updated to 3.17.3. FreeBSD updated to 13.2. 
+          OpenBSD updated to 7.3. 
+          On Ubuntu 23.04, the installation method has changed due to how 
+          PEP-668 was implemented by Debian and how this affects "pip". 
+          Some other distros may experience the same problems if they made 
+          the same changes. See the README.TxT for details. 
 * 3.4.0 - Added pyproject.toml file to satisfy Python 3.11 requirements.
           Updated build scripts to use python3 -m build instead of calling
           setup.py directly. Test targets were updated, Ubuntu 20.04 was 
           dropped, Ubuntu 22.10 was added, FreeBSD python version upgraded 
           to 3.9, OpenBSD upgraded to 7.2, Windows 10 Python upgraded to 3.11,
           Windows 11 Python upgraded to 3.11. Added __version__ attribute to 
           allow checking package version number at run time. Added version
```

### Comparing `bytesfunc-3.4.0/bytesfunc/__init__.py` & `bytesfunc-3.4.1/bytesfunc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """The BytesFunc module provides high speed bytes and bytearray processing 
 functions. These functions are patterned after the functions in the standard 
 Python Itertools module together with some additional ones import other sources.
 """
 
 # The version number should be updated automatically by the build script.
-__version__ = '3.4.0'
+__version__ = '3.4.1'
 
 from bytesfunc.bmax import bmax
 from bytesfunc.bmin import bmin
 from bytesfunc.bsum import bsum
 
 from bytesfunc.eq import eq
 from bytesfunc.ge import ge
```

### Comparing `bytesfunc-3.4.0/bytesfunc.egg-info/PKG-INFO` & `bytesfunc-3.4.1/bytesfunc.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bytesfunc
-Version: 3.4.0
+Version: 3.4.1
 Summary: Fast bytes and bytearray processing functions
 Home-page: https://github.com/m1griffin/bytesfunc
 Author: M Griffin
 Author-email: m12.griffin@gmail.com
 License: Apache License V2.0
 Keywords: bytes and bytearray functions
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,16 +18,16 @@
 =========
 BytesFunc
 =========
 
 :Authors:
     Michael Griffin
 
-:Version:  3.4.0 for 2022-12-11
-:Copyright: 2014 - 2022
+:Version:  3.4.1 for 2023-04-22
+:Copyright: 2014 - 2023
 :License: This document may be distributed under the Apache 2.0 License.
 :Language: Python 3.6 or later
 
 ---------------------------------------------------------------------
 
 Introduction
 ============
@@ -149,20 +149,20 @@
 
 ======================= ========== ====== =============== ================
 OS                       Hardware   Bits   Compiler        Python Version
 ======================= ========== ====== =============== ================
 Debian 11                i686         32     GCC               3.9.2
 Debian 11                x86_64       64     GCC               3.9.2
 Ubuntu 22.04             x86_64       64     GCC               3.10.6
-Ubuntu 22.10             x86_64       64     GCC               3.10.7
+Ubuntu 23.04             x86_64       64     GCC               3.11.2
 opensuse-leap 15.4       x86_64       64     GCC               3.6.15
-almalinux 9.0            x86_64       64     GCC               3.9.10
-alpine 3.16.2            i686         32     GCC               3.10.5
-FreeBSD 13.1             amd64        64     Clang             3.9.15
-OpenBSD 7.2              amd64        64     Clang             3.9.15
+almalinux 9.1            x86_64       64     GCC               3.9.14
+alpine 3.17.3            i686         32     GCC               3.10.11
+FreeBSD 13.2             amd64        64     Clang             3.9.16
+OpenBSD 7.3              amd64        64     Clang             3.10.10
 MS Windows 10            AMD64        64     MSC               3.11.0
 MS Windows 11            AMD64        64     MSC               3.11.0
 Raspbian 11              armv7l       32     GCC               3.9.2
 Ubuntu 22.04             aarch64      64     GCC               3.10.6
 ======================= ========== ====== =============== ================
 
 amd64 is another name for x86_64 and does not indicate the CPU brand.
@@ -223,18 +223,55 @@
 The setup.py file has platform detection code which it uses to pass the 
 correct flags to the C compiler. For ARM, this includes the CPU type. If you
 are using an ARM CPU type which is not recognized then setup.py may not
 compile in SIMD features. You can experiment with modifying setup.py to add
 new ARM models, but be sure that anything you try is compatible with the 
 existing ones.
 
+
+Installing on Linux with PIP and PEP-668
+----------------------------------------
+PEP-668 (PEPs describe changes to Python) introduced a new feature which can
+affect how packages are installed with PIP. If PIP is configured to be 
+EXTERNALLY-MANAGED it will refuse to install a package outside of a virtual
+environment.
+
+The intention of this is to prevent conflicts between packages which are 
+installed using the system package manager, and ones which are installed using
+PIP.
+
+Linux distros which are affeced by this include the latest versions of Debian
+and Ubuntu.
+
+As this package is a library which is intended to be used by other 
+applications, there is no one right way to install it, whether inside or 
+outside of a virtual environment. Review the options available with PIP to see
+what is suitable for your application.
+
+For testing purposes this package was installed by setting the environment
+variable PIP_BREAK_SYSTEM_PACKAGES to "1", which effectively disables this
+feature in PIP. 
+
+example::
+
+	export PIP_BREAK_SYSTEM_PACKAGES=1
+
+
 ---------------------------------------------------------------------
 
 Release History
 ===============
+* 3.4.1 - Update to testing and support. There were no code. changes. 
+          Ubuntu version updated to 23.04. AlmaLinux updated to 9.1. 
+          Alpine Linux updated to 3.17.3. FreeBSD updated to 13.2. 
+          OpenBSD updated to 7.3. 
+          On Ubuntu 23.04, the installation method has changed due to how 
+          PEP-668 was implemented by Debian and how this affects "pip". 
+          Some other distros may experience the same problems if they made 
+          the same changes. See the README.TxT for details. 
 * 3.4.0 - Added pyproject.toml file to satisfy Python 3.11 requirements.
           Updated build scripts to use python3 -m build instead of calling
           setup.py directly. Test targets were updated, Ubuntu 20.04 was 
           dropped, Ubuntu 22.10 was added, FreeBSD python version upgraded 
           to 3.9, OpenBSD upgraded to 7.2, Windows 10 Python upgraded to 3.11,
           Windows 11 Python upgraded to 3.11. Added __version__ attribute to 
           allow checking package version number at run time. Added version
```

### Comparing `bytesfunc-3.4.0/bytesfunc.egg-info/SOURCES.txt` & `bytesfunc-3.4.1/bytesfunc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/setup.py` & `bytesfunc-3.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/setupuser.bat` & `bytesfunc-3.4.1/setupuser.bat`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/setupuser.sh` & `bytesfunc-3.4.1/setupuser.sh`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/and_.c` & `bytesfunc-3.4.1/src/and_.c`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/arrayops.c` & `bytesfunc-3.4.1/src/arrayops.c`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/arrayops.h` & `bytesfunc-3.4.1/src/arrayops.h`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/ball.c` & `bytesfunc-3.4.1/src/ball.c`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/bany.c` & `bytesfunc-3.4.1/src/bany.c`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/bmax.c` & `bytesfunc-3.4.1/src/bmax.c`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/bmin.c` & `bytesfunc-3.4.1/src/bmin.c`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/bsum.c` & `bytesfunc-3.4.1/src/bsum.c`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/byteserrs.c` & `bytesfunc-3.4.1/src/byteserrs.c`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/byteserrs.h` & `bytesfunc-3.4.1/src/byteserrs.h`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/bytesparams_allany.c` & `bytesfunc-3.4.1/src/bytesparams_allany.c`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/bytesparams_allany.h` & `bytesfunc-3.4.1/src/bytesparams_allany.h`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/bytesparams_base.c` & `bytesfunc-3.4.1/src/bytesparams_base.c`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/bytesparams_base.h` & `bytesfunc-3.4.1/src/bytesparams_base.h`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/bytesparams_bsum.c` & `bytesfunc-3.4.1/src/bytesparams_bsum.c`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/bytesparams_bsum.h` & `bytesfunc-3.4.1/src/bytesparams_bsum.h`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/bytesparams_comp.c` & `bytesfunc-3.4.1/src/bytesparams_comp.c`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/bytesparams_comp.h` & `bytesfunc-3.4.1/src/bytesparams_comp.h`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/bytesparams_invert.c` & `bytesfunc-3.4.1/src/bytesparams_invert.c`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/bytesparams_invert.h` & `bytesfunc-3.4.1/src/bytesparams_invert.h`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/bytesparams_two.c` & `bytesfunc-3.4.1/src/bytesparams_two.c`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/bytesparams_two.h` & `bytesfunc-3.4.1/src/bytesparams_two.h`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/bytesparams_valoutsimd.c` & `bytesfunc-3.4.1/src/bytesparams_valoutsimd.c`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/bytesparams_valoutsimd.h` & `bytesfunc-3.4.1/src/bytesparams_valoutsimd.h`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/eq.c` & `bytesfunc-3.4.1/src/eq.c`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/findindex.c` & `bytesfunc-3.4.1/src/findindex.c`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/ge.c` & `bytesfunc-3.4.1/src/ge.c`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/gt.c` & `bytesfunc-3.4.1/src/gt.c`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/invert.c` & `bytesfunc-3.4.1/src/invert.c`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/le.c` & `bytesfunc-3.4.1/src/le.c`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/lshift.c` & `bytesfunc-3.4.1/src/lshift.c`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/lt.c` & `bytesfunc-3.4.1/src/lt.c`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/ne.c` & `bytesfunc-3.4.1/src/ne.c`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/or_.c` & `bytesfunc-3.4.1/src/or_.c`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/rshift.c` & `bytesfunc-3.4.1/src/rshift.c`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/simddefs.h` & `bytesfunc-3.4.1/src/simddefs.h`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/simdsupport.c` & `bytesfunc-3.4.1/src/simdsupport.c`

 * *Files identical despite different names*

### Comparing `bytesfunc-3.4.0/src/xor.c` & `bytesfunc-3.4.1/src/xor.c`

 * *Files identical despite different names*


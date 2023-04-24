# Comparing `tmp/boxx-0.9.7.tar.gz` & `tmp/boxx-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/boxx-0.9.7.tar", last modified: Fri Sep 10 13:20:29 2021, max compression
+gzip compressed data, was "dist/boxx-0.9.9.tar", last modified: Tue Oct 12 10:23:58 2021, max compression
```

## Comparing `boxx-0.9.7.tar` & `boxx-0.9.9.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2021-09-10 13:20:29.000000 boxx-0.9.7/
--rw-rw-r--   0 dl        (1000) dl        (1000)       83 2018-12-13 08:21:19.000000 boxx-0.9.7/MANIFEST.in
--rw-rw-r--   0 dl        (1000) dl        (1000)     1148 2021-09-10 13:20:29.000000 boxx-0.9.7/PKG-INFO
--rw-rw-r--   0 dl        (1000) dl        (1000)    11681 2018-12-13 08:21:19.000000 boxx-0.9.7/README.md
--rw-rw-r--   0 dl        (1000) dl        (1000)    11866 2019-05-08 14:14:09.000000 boxx-0.9.7/README_zh_cn.md
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2021-09-10 13:20:29.000000 boxx-0.9.7/boxx/
--rw-rw-r--   0 dl        (1000) dl        (1000)      975 2021-09-10 13:17:26.000000 boxx-0.9.7/boxx/__init__.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     3193 2019-11-03 03:04:28.000000 boxx-0.9.7/boxx/cp.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     1071 2018-12-13 08:21:19.000000 boxx-0.9.7/boxx/g.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     1067 2018-12-13 08:21:19.000000 boxx-0.9.7/boxx/gg.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     1005 2018-12-13 08:21:19.000000 boxx-0.9.7/boxx/p.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     1495 2021-08-27 10:39:23.000000 boxx-0.9.7/boxx/script.py
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2021-09-10 13:20:29.000000 boxx-0.9.7/boxx/tool/
--rw-rw-r--   0 dl        (1000) dl        (1000)     3009 2021-09-09 10:22:17.000000 boxx-0.9.7/boxx/tool/__init__.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     9739 2020-09-03 05:23:24.000000 boxx-0.9.7/boxx/tool/toolFunction.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     1286 2021-09-09 10:22:47.000000 boxx-0.9.7/boxx/tool/toolGui.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     6378 2020-04-15 17:50:30.000000 boxx-0.9.7/boxx/tool/toolIo.py
--rw-rw-r--   0 dl        (1000) dl        (1000)    37627 2020-03-30 08:42:16.000000 boxx-0.9.7/boxx/tool/toolLog.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     2737 2020-02-26 06:42:39.000000 boxx-0.9.7/boxx/tool/toolMarkdown.py
--rw-rw-r--   0 dl        (1000) dl        (1000)    15252 2020-01-03 09:03:51.000000 boxx-0.9.7/boxx/tool/toolStructObj.py
--rw-rw-r--   0 dl        (1000) dl        (1000)    16334 2021-09-10 13:17:10.000000 boxx-0.9.7/boxx/tool/toolSystem.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     6959 2020-05-06 10:03:04.000000 boxx-0.9.7/boxx/tool/toolTools.py
--rw-rw-r--   0 dl        (1000) dl        (1000)      109 2018-12-13 08:21:19.000000 boxx-0.9.7/boxx/undetermined.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     5342 2019-11-03 03:06:03.000000 boxx-0.9.7/boxx/ylcompat.py
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2021-09-10 13:20:29.000000 boxx-0.9.7/boxx/yldb/
--rw-rw-r--   0 dl        (1000) dl        (1000)      159 2018-12-13 11:04:33.000000 boxx-0.9.7/boxx/yldb/__init__.py
--rw-rw-r--   0 dl        (1000) dl        (1000)       68 2018-12-13 08:21:19.000000 boxx-0.9.7/boxx/yldb/dbPublicFuncation.py
--rw-rw-r--   0 dl        (1000) dl        (1000)      798 2018-12-13 10:51:11.000000 boxx-0.9.7/boxx/yldb/yldf.py
--rw-rw-r--   0 dl        (1000) dl        (1000)       67 2018-12-13 08:21:19.000000 boxx-0.9.7/boxx/yldb/ylmysql.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     2402 2019-11-03 03:04:59.000000 boxx-0.9.7/boxx/yldb/ylsqlite.py
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2021-09-10 13:20:29.000000 boxx-0.9.7/boxx/ylimg/
--rw-rw-r--   0 dl        (1000) dl        (1000)      750 2019-06-04 12:33:02.000000 boxx-0.9.7/boxx/ylimg/__init__.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     5554 2021-08-23 08:38:05.000000 boxx-0.9.7/boxx/ylimg/showImgsInBrowser.py
--rw-rw-r--   0 dl        (1000) dl        (1000)    44581 2021-03-22 16:23:49.000000 boxx-0.9.7/boxx/ylimg/ylimgTool.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     2794 2018-12-13 08:21:19.000000 boxx-0.9.7/boxx/ylimg/ylimgVideoAndGif.py
--rw-rw-r--   0 dl        (1000) dl        (1000)      226 2018-12-13 08:21:19.000000 boxx-0.9.7/boxx/yllab.py
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2021-09-10 13:20:29.000000 boxx-0.9.7/boxx/ylml/
--rw-rw-r--   0 dl        (1000) dl        (1000)      604 2019-04-26 09:25:16.000000 boxx-0.9.7/boxx/ylml/__init__.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     8886 2019-04-26 13:17:02.000000 boxx-0.9.7/boxx/ylml/ylDete.py
--rw-rw-r--   0 dl        (1000) dl        (1000)    13529 2019-11-03 03:05:44.000000 boxx-0.9.7/boxx/ylml/ylmlEvalu.py
--rw-rw-r--   0 dl        (1000) dl        (1000)    14562 2018-12-13 08:21:19.000000 boxx-0.9.7/boxx/ylml/ylmlTest.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     4961 2018-12-13 08:21:19.000000 boxx-0.9.7/boxx/ylml/ylmlTrain.py
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2021-09-10 13:20:29.000000 boxx-0.9.7/boxx/ylsci/
--rw-rw-r--   0 dl        (1000) dl        (1000)      484 2020-03-11 04:07:44.000000 boxx-0.9.7/boxx/ylsci/__init__.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     4709 2019-11-10 11:47:39.000000 boxx-0.9.7/boxx/ylsci/ylnp.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     2265 2020-02-14 10:12:06.000000 boxx-0.9.7/boxx/ylsci/ylstatistics.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     3328 2020-03-11 04:08:41.000000 boxx-0.9.7/boxx/ylsci/ylvector.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     4110 2021-03-25 07:28:50.000000 boxx-0.9.7/boxx/ylsys.py
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2021-09-10 13:20:29.000000 boxx-0.9.7/boxx/ylth/
--rw-rw-r--   0 dl        (1000) dl        (1000)    11960 2021-05-31 12:34:15.000000 boxx-0.9.7/boxx/ylth/__init__.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     1182 2021-05-31 12:31:27.000000 boxx-0.9.7/boxx/ylth/pthnan.py
--rw-rw-r--   0 dl        (1000) dl        (1000)      435 2018-12-13 08:21:19.000000 boxx-0.9.7/boxx/ylweb.py
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2021-09-10 13:20:29.000000 boxx-0.9.7/boxx.egg-info/
--rw-rw-r--   0 dl        (1000) dl        (1000)     1148 2021-09-10 13:20:29.000000 boxx-0.9.7/boxx.egg-info/PKG-INFO
--rw-rw-r--   0 dl        (1000) dl        (1000)     1059 2021-09-10 13:20:29.000000 boxx-0.9.7/boxx.egg-info/SOURCES.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)        1 2021-09-10 13:20:29.000000 boxx-0.9.7/boxx.egg-info/dependency_links.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       74 2021-09-10 13:20:29.000000 boxx-0.9.7/boxx.egg-info/requires.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)        5 2021-09-10 13:20:29.000000 boxx-0.9.7/boxx.egg-info/top_level.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       74 2021-09-10 13:15:50.000000 boxx-0.9.7/requirements.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       38 2021-09-10 13:20:29.000000 boxx-0.9.7/setup.cfg
--rw-rw-r--   0 dl        (1000) dl        (1000)     6834 2019-07-19 08:26:39.000000 boxx-0.9.7/setup.py
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2021-09-10 13:20:29.000000 boxx-0.9.7/test/
--rw-rw-r--   0 dl        (1000) dl        (1000)     1655 2018-12-13 08:21:19.000000 boxx-0.9.7/test/testAll.py
--rw-rw-r--   0 dl        (1000) dl        (1000)      475 2019-07-11 04:33:41.000000 boxx-0.9.7/yllab.py
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2021-10-12 10:23:58.000000 boxx-0.9.9/
+-rw-rw-r--   0 dl        (1000) dl        (1000)       83 2018-12-13 08:21:19.000000 boxx-0.9.9/MANIFEST.in
+-rw-rw-r--   0 dl        (1000) dl        (1000)     1148 2021-10-12 10:23:58.000000 boxx-0.9.9/PKG-INFO
+-rw-rw-r--   0 dl        (1000) dl        (1000)    11681 2018-12-13 08:21:19.000000 boxx-0.9.9/README.md
+-rw-rw-r--   0 dl        (1000) dl        (1000)    11866 2019-05-08 14:14:09.000000 boxx-0.9.9/README_zh_cn.md
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2021-10-12 10:23:58.000000 boxx-0.9.9/boxx/
+-rw-rw-r--   0 dl        (1000) dl        (1000)      975 2021-10-12 10:15:58.000000 boxx-0.9.9/boxx/__init__.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     3193 2019-11-03 03:04:28.000000 boxx-0.9.9/boxx/cp.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     1071 2018-12-13 08:21:19.000000 boxx-0.9.9/boxx/g.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     1067 2018-12-13 08:21:19.000000 boxx-0.9.9/boxx/gg.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     1005 2018-12-13 08:21:19.000000 boxx-0.9.9/boxx/p.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     1495 2021-08-27 10:39:23.000000 boxx-0.9.9/boxx/script.py
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2021-10-12 10:23:58.000000 boxx-0.9.9/boxx/tool/
+-rw-rw-r--   0 dl        (1000) dl        (1000)     3019 2021-09-18 05:27:19.000000 boxx-0.9.9/boxx/tool/__init__.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)    13704 2021-10-12 10:08:34.000000 boxx-0.9.9/boxx/tool/toolFunction.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     1286 2021-09-09 10:22:47.000000 boxx-0.9.9/boxx/tool/toolGui.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     6378 2020-04-15 17:50:30.000000 boxx-0.9.9/boxx/tool/toolIo.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)    37627 2020-03-30 08:42:16.000000 boxx-0.9.9/boxx/tool/toolLog.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     2737 2020-02-26 06:42:39.000000 boxx-0.9.9/boxx/tool/toolMarkdown.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)    15250 2021-09-23 09:28:31.000000 boxx-0.9.9/boxx/tool/toolStructObj.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)    16336 2021-09-28 08:21:36.000000 boxx-0.9.9/boxx/tool/toolSystem.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     6959 2020-05-06 10:03:04.000000 boxx-0.9.9/boxx/tool/toolTools.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)      109 2018-12-13 08:21:19.000000 boxx-0.9.9/boxx/undetermined.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     5342 2019-11-03 03:06:03.000000 boxx-0.9.9/boxx/ylcompat.py
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2021-10-12 10:23:58.000000 boxx-0.9.9/boxx/yldb/
+-rw-rw-r--   0 dl        (1000) dl        (1000)      163 2021-09-17 09:22:42.000000 boxx-0.9.9/boxx/yldb/__init__.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)       68 2018-12-13 08:21:19.000000 boxx-0.9.9/boxx/yldb/dbPublicFuncation.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)      794 2021-09-17 09:22:27.000000 boxx-0.9.9/boxx/yldb/yldf.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)       67 2018-12-13 08:21:19.000000 boxx-0.9.9/boxx/yldb/ylmysql.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     2402 2019-11-03 03:04:59.000000 boxx-0.9.9/boxx/yldb/ylsqlite.py
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2021-10-12 10:23:58.000000 boxx-0.9.9/boxx/ylimg/
+-rw-rw-r--   0 dl        (1000) dl        (1000)      750 2019-06-04 12:33:02.000000 boxx-0.9.9/boxx/ylimg/__init__.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     5554 2021-08-23 08:38:05.000000 boxx-0.9.9/boxx/ylimg/showImgsInBrowser.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)    44581 2021-03-22 16:23:49.000000 boxx-0.9.9/boxx/ylimg/ylimgTool.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     2794 2018-12-13 08:21:19.000000 boxx-0.9.9/boxx/ylimg/ylimgVideoAndGif.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)      226 2018-12-13 08:21:19.000000 boxx-0.9.9/boxx/yllab.py
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2021-10-12 10:23:58.000000 boxx-0.9.9/boxx/ylml/
+-rw-rw-r--   0 dl        (1000) dl        (1000)      616 2021-09-27 16:49:23.000000 boxx-0.9.9/boxx/ylml/__init__.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     8886 2019-04-26 13:17:02.000000 boxx-0.9.9/boxx/ylml/ylDete.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)    13529 2019-11-03 03:05:44.000000 boxx-0.9.9/boxx/ylml/ylmlEvalu.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)    14562 2018-12-13 08:21:19.000000 boxx-0.9.9/boxx/ylml/ylmlTest.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     4961 2018-12-13 08:21:19.000000 boxx-0.9.9/boxx/ylml/ylmlTrain.py
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2021-10-12 10:23:58.000000 boxx-0.9.9/boxx/ylsci/
+-rw-rw-r--   0 dl        (1000) dl        (1000)      484 2020-03-11 04:07:44.000000 boxx-0.9.9/boxx/ylsci/__init__.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     4710 2021-09-28 09:52:26.000000 boxx-0.9.9/boxx/ylsci/ylnp.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     2265 2020-02-14 10:12:06.000000 boxx-0.9.9/boxx/ylsci/ylstatistics.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     3328 2020-03-11 04:08:41.000000 boxx-0.9.9/boxx/ylsci/ylvector.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     4110 2021-03-25 07:28:50.000000 boxx-0.9.9/boxx/ylsys.py
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2021-10-12 10:23:58.000000 boxx-0.9.9/boxx/ylth/
+-rw-rw-r--   0 dl        (1000) dl        (1000)    11960 2021-09-28 08:15:38.000000 boxx-0.9.9/boxx/ylth/__init__.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     1182 2021-05-31 12:31:27.000000 boxx-0.9.9/boxx/ylth/pthnan.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)      435 2018-12-13 08:21:19.000000 boxx-0.9.9/boxx/ylweb.py
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2021-10-12 10:23:58.000000 boxx-0.9.9/boxx.egg-info/
+-rw-rw-r--   0 dl        (1000) dl        (1000)     1148 2021-10-12 10:23:58.000000 boxx-0.9.9/boxx.egg-info/PKG-INFO
+-rw-rw-r--   0 dl        (1000) dl        (1000)     1059 2021-10-12 10:23:58.000000 boxx-0.9.9/boxx.egg-info/SOURCES.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)        1 2021-10-12 10:23:58.000000 boxx-0.9.9/boxx.egg-info/dependency_links.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       74 2021-10-12 10:23:58.000000 boxx-0.9.9/boxx.egg-info/requires.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)        5 2021-10-12 10:23:58.000000 boxx-0.9.9/boxx.egg-info/top_level.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       74 2021-09-10 13:15:50.000000 boxx-0.9.9/requirements.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       38 2021-10-12 10:23:58.000000 boxx-0.9.9/setup.cfg
+-rw-rw-r--   0 dl        (1000) dl        (1000)     6834 2019-07-19 08:26:39.000000 boxx-0.9.9/setup.py
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2021-10-12 10:23:58.000000 boxx-0.9.9/test/
+-rw-rw-r--   0 dl        (1000) dl        (1000)     1655 2018-12-13 08:21:19.000000 boxx-0.9.9/test/testAll.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)      475 2019-07-11 04:33:41.000000 boxx-0.9.9/yllab.py
```

### Comparing `boxx-0.9.7/PKG-INFO` & `boxx-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: boxx
-Version: 0.9.7
+Version: 0.9.9
 Summary: Tool-box for efficient build and debug in Python. Especially for Scientific Computing and Computer Vision.
 Home-page: https://github.com/DIYer22/boxx
 Author: DIYer22
 Author-email: ylxx@live.com
 Maintainer: DIYer22
 Maintainer-email: ylxx@live.com
 License: MIT
```

### Comparing `boxx-0.9.7/README.md` & `boxx-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `boxx-0.9.7/README_zh_cn.md` & `boxx-0.9.9/README_zh_cn.md`

 * *Files identical despite different names*

### Comparing `boxx-0.9.7/boxx/__init__.py` & `boxx-0.9.9/boxx/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import unicode_literals
 
 '''
 Tool-box for efficient build and debug in Python. 
 Espacially for Scientific Computing and Computer Vision.
 '''
-__version__ = "0.9.7"
+__version__ = "0.9.9"
 __short_description__ = "Tool-box for efficient build and debug in Python. Especially for Scientific Computing and Computer Vision."
 __license__ = "MIT"
 __author__ = "DIYer22"
 __author_email__ = "ylxx@live.com"
 __maintainer__ = "DIYer22"
 __maintainer_email__ = "ylxx@live.com"
 __github_username__ = "DIYer22"
```

### Comparing `boxx-0.9.7/boxx/cp.py` & `boxx-0.9.9/boxx/cp.py`

 * *Files identical despite different names*

### Comparing `boxx-0.9.7/boxx/g.py` & `boxx-0.9.9/boxx/g.py`

 * *Files identical despite different names*

### Comparing `boxx-0.9.7/boxx/gg.py` & `boxx-0.9.9/boxx/gg.py`

 * *Files identical despite different names*

### Comparing `boxx-0.9.7/boxx/p.py` & `boxx-0.9.9/boxx/p.py`

 * *Files identical despite different names*

### Comparing `boxx-0.9.7/boxx/script.py` & `boxx-0.9.9/boxx/script.py`

 * *Files identical despite different names*

### Comparing `boxx-0.9.7/boxx/tool/__init__.py` & `boxx-0.9.9/boxx/tool/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 load_data = loadData
 
 from .toolSystem import (crun, performance, timeit, heatmap, getArgvDic, 
                          softInPath, makedirs, execmd, addPathToSys)
 from .toolSystem import importAllFunCode, impt, inpkg, importByPath, tryImport, FakeModule, removeImportSelf,  removeimp
 from .toolSystem import getMainFrame, getRootFrame, getFatherFrames#, exceptionHook
 
-from .toolFunction import (getFunName, SaveArguments, dynamicWraps, setTimeout, pipe,
+from .toolFunction import (getFunName, FuncArgs, SaveArguments, dynamicWraps, setTimeout, pipe,
                            setInterval, multiThread, mapmp, mapmt, maptry, retry)
 
 from .toolTools import (intround, increase, filterList, findints, randint, randfloat, randchoice,
                        listdirWithFun, replaceAllInRoot, findinRoot, iscn, zipTar,
                        camel2snake, snake2camel)
 
 from .toolMarkdown import Markdown
```

### Comparing `boxx-0.9.7/boxx/tool/toolFunction.py` & `boxx-0.9.9/boxx/tool/toolFunction.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import unicode_literals, print_function
+
 import time
+import inspect
 
 from ..ylsys import cpun, winYl
 from .toolStructObj import typestr
 
 from functools import reduce
 
 def getFunName(fun):
@@ -20,29 +22,159 @@
     """
     Save Arguments in funcation and apply those arguments to fun
     """
     def __init__(self, *l, **kv):
         self.l = l
         self.kv = kv
 
-    def apply(self, function):
+    def apply(self, func):
         """
         Apply the saved arguments to the function
         """
-        return function(*self.l, **self.kv)
-
+        return func(*self.l, **self.kv)
+        
+    __call__ = apply
     def __str__(self):
         ls = ", ".join(map(str, self.l))
         if len(self.l) and len(self.kv):
             ls += ", "
         kvs = ", ".join(["%s=%s" % (kv) for kv in self.kv.items()])
         return "SaveArguments(%s)" % (ls + kvs)
 
     __repr__ = __str__
 
+
+
+_NONE_TAG = []
+
+class FuncArgs:
+    """
+    Catch and manipulate function argments, for example::
+    
+        def func(a=None, b=None, c=None, *args, **kwargs):
+            print(a, b, c, args, kwargs)
+        fa = FuncArgs(func, "a1", b="b1", c=3.14,)
+        fa.apply(func)
+        fa.set_arg(0, 0)
+        fa.set_arg("b", "bb")
+        fa.set_arg(float, 2.71)
+        fa.apply(func)
+    """
+
+    class DummyBoundArguments:
+        def __init__(self, args, kwargs):
+            self.args = args
+            self.kwargs = kwargs
+
+        def find_argname(self, arg):
+            if isinstance(arg, (tuple, type)):
+                for idx, v in enumerate(self.args):
+                    if isinstance(v, arg):
+                        return idx
+                for k, v in self.kwargs.items():
+                    if isinstance(v, arg):
+                        return k
+            return arg
+
+        def op_arg(self, key, value=_NONE_TAG):
+            argname = self.find_argname(key)
+            if isinstance(argname, int):
+                if value is _NONE_TAG:
+                    return self.args[argname]
+                else:
+                    self.args = (
+                        self.args[:argname] + (value,) + self.args[argname + 1 :]
+                    )
+                    return
+            if isinstance(argname, str):
+                if value is _NONE_TAG:
+                    return self.kwargs[argname]
+                else:
+                    self.kwargs[argname] = value
+                    return
+
+        def __str__(self):
+            return "<DummyBoundArguments (args=%s, kwargs=%s)>" % (
+                self.args,
+                self.kwargs,
+            )
+
+    def __init__(self, func, *args, **kwargs):
+        if not callable(func):
+
+            def func(*args, **kwargs):
+                pass
+
+        self.func = func
+        try:
+            self.sig = inspect.signature(func)
+            # inspect.BoundArguments
+            self.ba = self.sig.bind(*args, **kwargs)
+            self.ba.apply_defaults()
+        except ValueError:
+            self.ba = self.DummyBoundArguments(args, kwargs)
+
+    def find_argname(self, arg):
+        if not hasattr(self, "sig"):
+            return self.ba.find_argname(arg)
+
+        if isinstance(arg, str):
+            argname = arg
+        elif isinstance(arg, int):
+            argname = list(self.sig.parameters.keys())[arg]
+        elif isinstance(arg, (tuple, type)):
+            # return first argname belong to arg type
+            for idx, _arg in enumerate(self.ba.args):
+                if isinstance(_arg, arg):
+                    argname = list(self.sig.parameters.keys())[idx]
+                    return argname
+            for k, _arg in self.ba.kwargs.items():
+                if isinstance(_arg, arg):
+                    return k
+        return argname
+
+    def set_arg(self, key, value):
+        if not hasattr(self, "sig"):
+            self.ba.op_arg(key, value)
+            return self
+        argname = self.find_argname(key)
+        self.ba.arguments[argname] = value
+        return self
+
+    def get_arg(self, key):
+        if not hasattr(self, "sig"):
+            return self.ba.op_arg(key)
+        argname = self.find_argname(key)
+        return self.ba.arguments[argname]
+
+    def apply(self, func=None):
+        if func is None:
+            func = self.func
+        return func(*self.ba.args, **self.ba.kwargs)
+
+    __call__ = apply
+
+    def __str__(self):
+        s = str(self.ba)
+        s = s.replace("BoundArguments ", "FuncArgs of " + self.func.__name__)
+        return s
+
+    __repr__ = __str__
+    @staticmethod
+    def test():
+        def func(a=None, b=None, c=None, *args, **kwargs):
+            print(a, b, c, args, kwargs)
+
+        fa = FuncArgs(func, "a1", b="b1", c=3.14,)
+        fa.apply(func)
+        fa.set_arg(0, 0)
+        fa.set_arg("b", "bb")
+        fa.set_arg(float, 2.71)
+        fa.apply(func)
+
 def dynamicWraps(func):
     '''
     decorator 动态规划 装饰器
     '''
     cache={}
     from functools import wraps
     @wraps(func)
```

### Comparing `boxx-0.9.7/boxx/tool/toolGui.py` & `boxx-0.9.9/boxx/tool/toolGui.py`

 * *Files identical despite different names*

### Comparing `boxx-0.9.7/boxx/tool/toolIo.py` & `boxx-0.9.9/boxx/tool/toolIo.py`

 * *Files identical despite different names*

### Comparing `boxx-0.9.7/boxx/tool/toolLog.py` & `boxx-0.9.9/boxx/tool/toolLog.py`

 * *Files identical despite different names*

### Comparing `boxx-0.9.7/boxx/tool/toolMarkdown.py` & `boxx-0.9.9/boxx/tool/toolMarkdown.py`

 * *Files identical despite different names*

### Comparing `boxx-0.9.7/boxx/tool/toolStructObj.py` & `boxx-0.9.9/boxx/tool/toolStructObj.py`

 * *Files 0% similar despite different names*

```diff
@@ -398,18 +398,18 @@
     
     Parameters
     ----------
     enterFun : function, default None
         No parameter function
     exitFun : function, default None
         No parameter function or parameter are (exc_type, exc_value, exc_traceback)
-    exception : bool, default False
+    exception : bool, default True
         Whether send (exc_type, exc_value, exc_traceback) to exitFun
     '''
-    def __init__(self, enterFun=None, exitFun=None, exception=False):
+    def __init__(self, enterFun=None, exitFun=None, exception=True):
         self.enterFun = enterFun
         self.exitFun = exitFun
         self.exception = exception
     def __enter__(self):
         if self.enterFun:
             return self.enterFun()
     def __exit__(self, exc_type, exc_value, exc_traceback):
```

### Comparing `boxx-0.9.7/boxx/tool/toolSystem.py` & `boxx-0.9.9/boxx/tool/toolSystem.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
     >>> module = importByPath('far/away.py')
     '''
     from boxx import os, dirname, sys, withfun
     pyFile = pyPath
     assert os.path.isfile(pyFile) or os.path.isdir(pyFile), pyFile
     dirr = dirname(pyFile)
     import importlib
-    def exitFun():
+    def exitFun(*l):
         assert sys.path.pop(0)==dirr
     with withfun(lambda :sys.path.insert(0, dirr), exitFun):
         module = importlib.import_module(os.path.basename(pyFile).replace('.py',''))
         return module
     
 def tryImport(moduleName):
     '''
```

### Comparing `boxx-0.9.7/boxx/tool/toolTools.py` & `boxx-0.9.9/boxx/tool/toolTools.py`

 * *Files identical despite different names*

### Comparing `boxx-0.9.7/boxx/ylcompat.py` & `boxx-0.9.9/boxx/ylcompat.py`

 * *Files identical despite different names*

### Comparing `boxx-0.9.7/boxx/yldb/yldf.py` & `boxx-0.9.9/boxx/yldb/yldf.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 """
 tools for pandas 
 
 @author: yl
 """
 
 from __future__ import unicode_literals
+import pandas as pd
 
 def df2dicts(df, inculdeIndex=False):
     '''
     input a df, return to a list of dict
     
     Parameters
     ----------
@@ -22,15 +23,14 @@
     if inculdeIndex:
         for index, dic in zip(df.index, dicts):
             dic['index'] = index
     return dicts
 
 if __name__ == '__main__':
     pass
-    import pandas as pd
     df = pd.DataFrame({
                        0:list(range(5)),
                        1:list(range(10,15)),
                        'a':list("abcde"),
                        })
     df.set_index(0,inplace=True)
```

### Comparing `boxx-0.9.7/boxx/yldb/ylsqlite.py` & `boxx-0.9.9/boxx/yldb/ylsqlite.py`

 * *Files identical despite different names*

### Comparing `boxx-0.9.7/boxx/ylimg/__init__.py` & `boxx-0.9.9/boxx/ylimg/__init__.py`

 * *Files identical despite different names*

### Comparing `boxx-0.9.7/boxx/ylimg/showImgsInBrowser.py` & `boxx-0.9.9/boxx/ylimg/showImgsInBrowser.py`

 * *Files identical despite different names*

### Comparing `boxx-0.9.7/boxx/ylimg/ylimgTool.py` & `boxx-0.9.9/boxx/ylimg/ylimgTool.py`

 * *Files identical despite different names*

### Comparing `boxx-0.9.7/boxx/ylimg/ylimgVideoAndGif.py` & `boxx-0.9.9/boxx/ylimg/ylimgVideoAndGif.py`

 * *Files identical despite different names*

### Comparing `boxx-0.9.7/boxx/ylml/ylDete.py` & `boxx-0.9.9/boxx/ylml/ylDete.py`

 * *Files identical despite different names*

### Comparing `boxx-0.9.7/boxx/ylml/ylmlEvalu.py` & `boxx-0.9.9/boxx/ylml/ylmlEvalu.py`

 * *Files identical despite different names*

### Comparing `boxx-0.9.7/boxx/ylml/ylmlTest.py` & `boxx-0.9.9/boxx/ylml/ylmlTest.py`

 * *Files identical despite different names*

### Comparing `boxx-0.9.7/boxx/ylml/ylmlTrain.py` & `boxx-0.9.9/boxx/ylml/ylmlTrain.py`

 * *Files identical despite different names*

### Comparing `boxx-0.9.7/boxx/ylsci/ylnp.py` & `boxx-0.9.9/boxx/ylsci/ylnp.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     X, Y = np.meshgrid(X, Y)
     __draw3dSurface(X,Y,Z)
 
 __numpyTypeCache = dict()
 def getNumpyType(typee='int'):
     if typee in __numpyTypeCache:
         return __numpyTypeCache[typee]
-    finds = eval('('+', '.join(['np.'+mu for mu in filterList(typee, dir(np))])+')')
+    finds = eval('('+', '.join(['np.'+mu for mu in filterList(typee, dir(np))])+',)')
     types = [x for x in finds if type(x)==type]
     if typee == "str":
         types = tuple(types) + getNumpyType('unicode')
     types = tuple(types)
     __numpyTypeCache[typee] = types
     return types
 def isNumpyType(array, typee='int'):
```

### Comparing `boxx-0.9.7/boxx/ylsci/ylstatistics.py` & `boxx-0.9.9/boxx/ylsci/ylstatistics.py`

 * *Files identical despite different names*

### Comparing `boxx-0.9.7/boxx/ylsci/ylvector.py` & `boxx-0.9.9/boxx/ylsci/ylvector.py`

 * *Files identical despite different names*

### Comparing `boxx-0.9.7/boxx/ylsys.py` & `boxx-0.9.9/boxx/ylsys.py`

 * *Files identical despite different names*

### Comparing `boxx-0.9.7/boxx/ylth/__init__.py` & `boxx-0.9.9/boxx/ylth/__init__.py`

 * *Files identical despite different names*

### Comparing `boxx-0.9.7/boxx/ylth/pthnan.py` & `boxx-0.9.9/boxx/ylth/pthnan.py`

 * *Files identical despite different names*

### Comparing `boxx-0.9.7/boxx.egg-info/PKG-INFO` & `boxx-0.9.9/boxx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: boxx
-Version: 0.9.7
+Version: 0.9.9
 Summary: Tool-box for efficient build and debug in Python. Especially for Scientific Computing and Computer Vision.
 Home-page: https://github.com/DIYer22/boxx
 Author: DIYer22
 Author-email: ylxx@live.com
 Maintainer: DIYer22
 Maintainer-email: ylxx@live.com
 License: MIT
```

### Comparing `boxx-0.9.7/boxx.egg-info/SOURCES.txt` & `boxx-0.9.9/boxx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `boxx-0.9.7/setup.py` & `boxx-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `boxx-0.9.7/test/testAll.py` & `boxx-0.9.9/test/testAll.py`

 * *Files identical despite different names*


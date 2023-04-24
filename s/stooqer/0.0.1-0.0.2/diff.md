# Comparing `tmp/stooqer-0.0.1.tar.gz` & `tmp/stooqer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stooqer-0.0.1.tar", last modified: Sat Apr 22 15:33:30 2023, max compression
+gzip compressed data, was "stooqer-0.0.2.tar", last modified: Mon Apr 24 14:12:40 2023, max compression
```

## Comparing `stooqer-0.0.1.tar` & `stooqer-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 15:33:30.610746 stooqer-0.0.1/
--rw-rw-rw-   0        0        0     1064 2023-04-22 15:29:40.000000 stooqer-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      536 2023-04-22 15:33:30.609749 stooqer-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1445 2023-04-22 15:29:40.000000 stooqer-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 15:33:30.604762 stooqer-0.0.1/Stooqer/
--rw-rw-rw-   0        0        0        0 2023-04-22 15:30:26.000000 stooqer-0.0.1/Stooqer/__init__.py
--rw-rw-rw-   0        0        0      474 2023-04-22 04:12:03.000000 stooqer-0.0.1/Stooqer/parsing.py
--rw-rw-rw-   0        0        0     1897 2023-04-22 15:30:37.000000 stooqer-0.0.1/Stooqer/stooqer.py
--rw-rw-rw-   0        0        0       42 2023-04-22 15:33:30.610746 stooqer-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      770 2023-04-22 15:30:29.000000 stooqer-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-22 15:33:30.609749 stooqer-0.0.1/stooqer.egg-info/
--rw-rw-rw-   0        0        0      536 2023-04-22 15:33:30.000000 stooqer-0.0.1/stooqer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-04-22 15:33:30.000000 stooqer-0.0.1/stooqer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 15:33:30.000000 stooqer-0.0.1/stooqer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-22 15:33:30.000000 stooqer-0.0.1/stooqer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-22 15:33:30.000000 stooqer-0.0.1/stooqer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 14:12:40.505399 stooqer-0.0.2/
+-rw-rw-rw-   0        0        0     1064 2023-04-22 15:29:40.000000 stooqer-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      536 2023-04-24 14:12:40.505399 stooqer-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1445 2023-04-22 15:29:40.000000 stooqer-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 14:12:40.490440 stooqer-0.0.2/Stooqer/
+-rw-rw-rw-   0        0        0       25 2023-04-24 14:11:57.000000 stooqer-0.0.2/Stooqer/__init__.py
+-rw-rw-rw-   0        0        0      474 2023-04-22 04:12:03.000000 stooqer-0.0.2/Stooqer/parsing.py
+-rw-rw-rw-   0        0        0     1897 2023-04-22 15:30:37.000000 stooqer-0.0.2/Stooqer/stooqer.py
+-rw-rw-rw-   0        0        0       42 2023-04-24 14:12:40.505399 stooqer-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      770 2023-04-24 14:11:58.000000 stooqer-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:12:40.504402 stooqer-0.0.2/stooqer.egg-info/
+-rw-rw-rw-   0        0        0      536 2023-04-24 14:12:40.000000 stooqer-0.0.2/stooqer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-04-24 14:12:40.000000 stooqer-0.0.2/stooqer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 14:12:40.000000 stooqer-0.0.2/stooqer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-24 14:12:40.000000 stooqer-0.0.2/stooqer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-24 14:12:40.000000 stooqer-0.0.2/stooqer.egg-info/top_level.txt
```

### Comparing `stooqer-0.0.1/LICENSE` & `stooqer-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stooqer-0.0.1/PKG-INFO` & `stooqer-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stooqer
-Version: 0.0.1
+Version: 0.0.2
 Summary: Stooq data download into pandas DataFrame
 Author: Septixu (Michał Lachowicz)
 Author-email: <michal.lachowicz@protnmail.com>
 Keywords: python,stock,stooq,finance
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `stooqer-0.0.1/README.md` & `stooqer-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `stooqer-0.0.1/Stooqer/stooqer.py` & `stooqer-0.0.2/Stooqer/stooqer.py`

 * *Files identical despite different names*

### Comparing `stooqer-0.0.1/stooqer.egg-info/PKG-INFO` & `stooqer-0.0.2/stooqer.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stooqer
-Version: 0.0.1
+Version: 0.0.2
 Summary: Stooq data download into pandas DataFrame
 Author: Septixu (Michał Lachowicz)
 Author-email: <michal.lachowicz@protnmail.com>
 Keywords: python,stock,stooq,finance
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```


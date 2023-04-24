# Comparing `tmp/sosin-1.0.2.tar.gz` & `tmp/sosin-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sosin-1.0.2.tar", last modified: Sat Apr 22 13:06:34 2023, max compression
+gzip compressed data, was "sosin-1.0.3.tar", last modified: Mon Apr 24 10:26:26 2023, max compression
```

## Comparing `sosin-1.0.2.tar` & `sosin-1.0.3.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 13:06:34.316430 sosin-1.0.2/
--rw-rw-rw-   0        0        0     1083 2023-04-17 11:46:46.000000 sosin-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     1268 2023-04-22 13:06:34.315329 sosin-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      863 2023-04-17 11:46:46.000000 sosin-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-22 13:06:34.316430 sosin-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      994 2023-04-22 13:05:48.000000 sosin-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-22 13:06:34.278792 sosin-1.0.2/sosin/
--rw-rw-rw-   0        0        0        0 2023-04-17 12:05:52.000000 sosin-1.0.2/sosin/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-22 13:06:34.304280 sosin-1.0.2/sosin/databases/
--rw-rw-rw-   0        0        0     6203 2023-04-19 13:20:07.000000 sosin-1.0.2/sosin/databases/rdb.py
-drwxrwxrwx   0        0        0        0 2023-04-22 13:06:34.305795 sosin-1.0.2/sosin/rpa/
--rw-rw-rw-   0        0        0    10828 2023-04-22 13:06:11.000000 sosin-1.0.2/sosin/rpa/email_mgr.py
-drwxrwxrwx   0        0        0        0 2023-04-22 13:06:34.310814 sosin-1.0.2/sosin/utils/
--rw-rw-rw-   0        0        0     1687 2023-04-17 11:46:46.000000 sosin-1.0.2/sosin/utils/currency.py
--rw-rw-rw-   0        0        0      304 2023-04-17 11:46:46.000000 sosin-1.0.2/sosin/utils/log.py
--rw-rw-rw-   0        0        0      527 2023-04-17 11:46:46.000000 sosin-1.0.2/sosin/utils/progress.py
--rw-rw-rw-   0        0        0      385 2023-04-17 11:46:46.000000 sosin-1.0.2/sosin/utils/secret.py
-drwxrwxrwx   0        0        0        0 2023-04-22 13:06:34.314321 sosin-1.0.2/sosin/web/
--rw-rw-rw-   0        0        0     1055 2023-04-18 14:49:45.000000 sosin-1.0.2/sosin/web/content.py
--rw-rw-rw-   0        0        0     1018 2023-04-17 11:46:46.000000 sosin-1.0.2/sosin/web/translate.py
--rw-rw-rw-   0        0        0     4796 2023-04-17 11:46:46.000000 sosin-1.0.2/sosin/web/virtual.py
-drwxrwxrwx   0        0        0        0 2023-04-22 13:06:34.302774 sosin-1.0.2/sosin.egg-info/
--rw-rw-rw-   0        0        0     1268 2023-04-22 13:06:33.000000 sosin-1.0.2/sosin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2023-04-22 13:06:34.000000 sosin-1.0.2/sosin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 13:06:34.000000 sosin-1.0.2/sosin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-04-22 13:06:34.000000 sosin-1.0.2/sosin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-22 13:06:34.000000 sosin-1.0.2/sosin.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 10:26:26.457757 sosin-1.0.3/
+-rw-rw-rw-   0        0        0     1083 2023-04-17 11:46:46.000000 sosin-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1268 2023-04-24 10:26:26.456733 sosin-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      863 2023-04-17 11:46:46.000000 sosin-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-24 10:26:26.459134 sosin-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      994 2023-04-24 10:12:17.000000 sosin-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 10:26:26.412730 sosin-1.0.3/sosin/
+-rw-rw-rw-   0        0        0        0 2023-04-17 12:05:52.000000 sosin-1.0.3/sosin/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 10:26:26.431728 sosin-1.0.3/sosin/databases/
+-rw-rw-rw-   0        0        0     9667 2023-04-24 02:18:48.000000 sosin-1.0.3/sosin/databases/rdb.py
+drwxrwxrwx   0        0        0        0 2023-04-24 10:26:26.434653 sosin-1.0.3/sosin/rpa/
+-rw-rw-rw-   0        0        0    10828 2023-04-22 13:06:11.000000 sosin-1.0.3/sosin/rpa/email_mgr.py
+-rw-rw-rw-   0        0        0     3698 2023-04-24 10:25:20.000000 sosin-1.0.3/sosin/rpa/sms_mgr.py
+drwxrwxrwx   0        0        0        0 2023-04-24 10:26:26.439798 sosin-1.0.3/sosin/utils/
+-rw-rw-rw-   0        0        0     1687 2023-04-17 11:46:46.000000 sosin-1.0.3/sosin/utils/currency.py
+-rw-rw-rw-   0        0        0      304 2023-04-17 11:46:46.000000 sosin-1.0.3/sosin/utils/log.py
+-rw-rw-rw-   0        0        0      527 2023-04-17 11:46:46.000000 sosin-1.0.3/sosin/utils/progress.py
+-rw-rw-rw-   0        0        0      385 2023-04-17 11:46:46.000000 sosin-1.0.3/sosin/utils/secret.py
+drwxrwxrwx   0        0        0        0 2023-04-24 10:26:26.454741 sosin-1.0.3/sosin/web/
+-rw-rw-rw-   0        0        0     1055 2023-04-18 14:49:45.000000 sosin-1.0.3/sosin/web/content.py
+-rw-rw-rw-   0        0        0     1018 2023-04-17 11:46:46.000000 sosin-1.0.3/sosin/web/translate.py
+-rw-rw-rw-   0        0        0     4796 2023-04-24 07:25:27.000000 sosin-1.0.3/sosin/web/virtual.py
+drwxrwxrwx   0        0        0        0 2023-04-24 10:26:26.430748 sosin-1.0.3/sosin.egg-info/
+-rw-rw-rw-   0        0        0     1268 2023-04-24 10:26:26.000000 sosin-1.0.3/sosin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2023-04-24 10:26:26.000000 sosin-1.0.3/sosin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 10:26:26.000000 sosin-1.0.3/sosin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-04-24 10:26:26.000000 sosin-1.0.3/sosin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-24 10:26:26.000000 sosin-1.0.3/sosin.egg-info/top_level.txt
```

### Comparing `sosin-1.0.2/LICENSE` & `sosin-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sosin-1.0.2/PKG-INFO` & `sosin-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosin
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python utils for general works
 Home-page: https://github.com/devsosin/sosin
 Author: Jason Choi
 Author-email: svstar94@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sosin-1.0.2/README.md` & `sosin-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `sosin-1.0.2/setup.py` & `sosin-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name                                = "sosin",
-    version                             = "1.0.2",
+    version                             = "1.0.3",
     license                             = 'MIT',
     author                              = "Jason Choi",
     author_email                        = "svstar94@gmail.com",
     description                         = "Python utils for general works",
     long_description                    = open('README.md').read(),
     url                                 = "https://github.com/devsosin/sosin",
     install_requires                    = ['requests', 'beautifulsoup4', 'PyMySQL',],
```

### Comparing `sosin-1.0.2/sosin/rpa/email_mgr.py` & `sosin-1.0.3/sosin/rpa/email_mgr.py`

 * *Files identical despite different names*

### Comparing `sosin-1.0.2/sosin/utils/currency.py` & `sosin-1.0.3/sosin/utils/currency.py`

 * *Files identical despite different names*

### Comparing `sosin-1.0.2/sosin/utils/progress.py` & `sosin-1.0.3/sosin/utils/progress.py`

 * *Files identical despite different names*

### Comparing `sosin-1.0.2/sosin/web/content.py` & `sosin-1.0.3/sosin/web/content.py`

 * *Files identical despite different names*

### Comparing `sosin-1.0.2/sosin/web/translate.py` & `sosin-1.0.3/sosin/web/translate.py`

 * *Files identical despite different names*

### Comparing `sosin-1.0.2/sosin/web/virtual.py` & `sosin-1.0.3/sosin/web/virtual.py`

 * *Files identical despite different names*

### Comparing `sosin-1.0.2/sosin.egg-info/PKG-INFO` & `sosin-1.0.3/sosin.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosin
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python utils for general works
 Home-page: https://github.com/devsosin/sosin
 Author: Jason Choi
 Author-email: svstar94@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```


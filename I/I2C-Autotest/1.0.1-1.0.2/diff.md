# Comparing `tmp/I2C_Autotest-1.0.1.tar.gz` & `tmp/I2C_Autotest-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\I2C_Autotest-1.0.1.tar", last modified: Mon Apr 24 02:43:22 2023, max compression
+gzip compressed data, was "dist\I2C_Autotest-1.0.2.tar", last modified: Mon Apr 24 03:32:48 2023, max compression
```

## Comparing `I2C_Autotest-1.0.1.tar` & `I2C_Autotest-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 02:43:22.000000 I2C_Autotest-1.0.1/
-drwxrwxrwx   0        0        0        0 2023-04-24 02:43:22.000000 I2C_Autotest-1.0.1/I2C_Autotest/
--rw-rw-rw-   0        0        0        0 2023-04-24 02:25:13.000000 I2C_Autotest-1.0.1/I2C_Autotest/__init__.py
--rw-rw-rw-   0        0        0    28813 2023-04-24 02:43:03.000000 I2C_Autotest-1.0.1/I2C_Autotest/analytics_core.py
-drwxrwxrwx   0        0        0        0 2023-04-24 02:43:22.000000 I2C_Autotest-1.0.1/I2C_Autotest.egg-info/
--rw-rw-rw-   0        0        0      617 2023-04-24 02:43:21.000000 I2C_Autotest-1.0.1/I2C_Autotest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-04-24 02:43:21.000000 I2C_Autotest-1.0.1/I2C_Autotest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 02:43:21.000000 I2C_Autotest-1.0.1/I2C_Autotest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-24 02:43:21.000000 I2C_Autotest-1.0.1/I2C_Autotest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-24 02:43:21.000000 I2C_Autotest-1.0.1/I2C_Autotest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      617 2023-04-24 02:43:22.000000 I2C_Autotest-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-24 02:43:22.000000 I2C_Autotest-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1359 2023-04-24 02:40:43.000000 I2C_Autotest-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 03:32:48.000000 I2C_Autotest-1.0.2/
+drwxrwxrwx   0        0        0        0 2023-04-24 03:32:48.000000 I2C_Autotest-1.0.2/I2C_Autotest/
+-rw-rw-rw-   0        0        0        0 2023-04-24 02:25:13.000000 I2C_Autotest-1.0.2/I2C_Autotest/__init__.py
+-rw-rw-rw-   0        0        0    28813 2023-04-24 02:43:03.000000 I2C_Autotest-1.0.2/I2C_Autotest/analytics_core.py
+drwxrwxrwx   0        0        0        0 2023-04-24 03:32:48.000000 I2C_Autotest-1.0.2/I2C_Autotest.egg-info/
+-rw-rw-rw-   0        0        0      617 2023-04-24 03:32:48.000000 I2C_Autotest-1.0.2/I2C_Autotest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-04-24 03:32:48.000000 I2C_Autotest-1.0.2/I2C_Autotest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 03:32:48.000000 I2C_Autotest-1.0.2/I2C_Autotest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-24 03:32:48.000000 I2C_Autotest-1.0.2/I2C_Autotest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-24 03:32:48.000000 I2C_Autotest-1.0.2/I2C_Autotest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      617 2023-04-24 03:32:48.000000 I2C_Autotest-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-24 03:32:48.000000 I2C_Autotest-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1359 2023-04-24 02:44:12.000000 I2C_Autotest-1.0.2/setup.py
```

### Comparing `I2C_Autotest-1.0.1/I2C_Autotest/analytics_core.py` & `I2C_Autotest-1.0.2/I2C_Autotest/analytics_core.py`

 * *Files identical despite different names*

### Comparing `I2C_Autotest-1.0.1/I2C_Autotest.egg-info/PKG-INFO` & `I2C_Autotest-1.0.2/I2C_Autotest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: I2C-Autotest
-Version: 1.0.1
+Version: 1.0.2
 Summary: A set of data tools in Python
 Home-page: https://github.com/
 Author: Tairong Chen
 Author-email: s321790@gmail.com
 License: MIT
 Download-URL: https://pypi.org/
 Description: UNKNOWN
```

### Comparing `I2C_Autotest-1.0.1/PKG-INFO` & `I2C_Autotest-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: I2C_Autotest
-Version: 1.0.1
+Version: 1.0.2
 Summary: A set of data tools in Python
 Home-page: https://github.com/
 Author: Tairong Chen
 Author-email: s321790@gmail.com
 License: MIT
 Download-URL: https://pypi.org/
 Description: UNKNOWN
```

### Comparing `I2C_Autotest-1.0.1/setup.py` & `I2C_Autotest-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 PACKAGE_NAME = "I2C_Autotest"
 AUTHOR = "Tairong Chen"
 AUTHOR_EMAIL = "s321790@gmail.com"
 URL = "https://github.com/"
 DOWNLOAD_URL = "https://pypi.org/"
  
 LICENSE = "MIT"
-VERSION = "1.0.1"
+VERSION = "1.0.2"
 DESCRIPTION = "A set of data tools in Python"
 LONG_DESCRIPTION = (HERE / "docs" / "README.md").read_text(encoding="utf8")
 LONG_DESC_TYPE = "text/markdown"
  
 requirements = (HERE / "requirements.txt").read_text(encoding="utf8")
 INSTALL_REQUIRES = [s.strip() for s in requirements.split("\n")]
```


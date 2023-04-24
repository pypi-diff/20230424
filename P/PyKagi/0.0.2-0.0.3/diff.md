# Comparing `tmp/PyKagi-0.0.2.tar.gz` & `tmp/PyKagi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyKagi-0.0.2.tar", last modified: Mon Apr 24 01:28:25 2023, max compression
+gzip compressed data, was "PyKagi-0.0.3.tar", last modified: Mon Apr 24 01:32:21 2023, max compression
```

## Comparing `PyKagi-0.0.2.tar` & `PyKagi-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 01:28:25.258896 PyKagi-0.0.2/
--rw-rw-rw-   0        0        0    11558 2023-03-29 23:46:55.000000 PyKagi-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     3194 2023-04-24 01:28:25.257900 PyKagi-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-24 01:28:25.239947 PyKagi-0.0.2/PyKagi/
--rw-rw-rw-   0        0        0      262 2023-03-30 01:22:53.000000 PyKagi-0.0.2/PyKagi/__init__.py
--rw-rw-rw-   0        0        0     2400 2023-04-24 01:04:11.000000 PyKagi-0.0.2/PyKagi/api.py
-drwxrwxrwx   0        0        0        0 2023-04-24 01:28:25.256901 PyKagi-0.0.2/PyKagi/config/
--rw-rw-rw-   0        0        0        0 2022-10-13 08:58:13.000000 PyKagi-0.0.2/PyKagi/config/__init__.py
--rw-rw-rw-   0        0        0      172 2023-04-24 01:13:34.000000 PyKagi-0.0.2/PyKagi/config/info.py
-drwxrwxrwx   0        0        0        0 2023-04-24 01:28:25.254907 PyKagi-0.0.2/PyKagi.egg-info/
--rw-rw-rw-   0        0        0     3194 2023-04-24 01:28:25.000000 PyKagi-0.0.2/PyKagi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2023-04-24 01:28:25.000000 PyKagi-0.0.2/PyKagi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 01:28:25.000000 PyKagi-0.0.2/PyKagi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-04-24 01:28:25.000000 PyKagi-0.0.2/PyKagi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-24 01:28:25.000000 PyKagi-0.0.2/PyKagi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2731 2023-04-24 01:22:21.000000 PyKagi-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-24 01:28:25.258896 PyKagi-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      903 2023-04-24 01:28:03.000000 PyKagi-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:32:21.149187 PyKagi-0.0.3/
+-rw-rw-rw-   0        0        0    11558 2023-03-29 23:46:55.000000 PyKagi-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3194 2023-04-24 01:32:21.148191 PyKagi-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-24 01:32:21.135064 PyKagi-0.0.3/PyKagi/
+-rw-rw-rw-   0        0        0      262 2023-03-30 01:22:53.000000 PyKagi-0.0.3/PyKagi/__init__.py
+-rw-rw-rw-   0        0        0     2367 2023-04-24 01:31:24.000000 PyKagi-0.0.3/PyKagi/api.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:32:21.148191 PyKagi-0.0.3/PyKagi/config/
+-rw-rw-rw-   0        0        0        0 2022-10-13 08:58:13.000000 PyKagi-0.0.3/PyKagi/config/__init__.py
+-rw-rw-rw-   0        0        0      172 2023-04-24 01:31:58.000000 PyKagi-0.0.3/PyKagi/config/info.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:32:21.146196 PyKagi-0.0.3/PyKagi.egg-info/
+-rw-rw-rw-   0        0        0     3194 2023-04-24 01:32:21.000000 PyKagi-0.0.3/PyKagi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2023-04-24 01:32:21.000000 PyKagi-0.0.3/PyKagi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 01:32:21.000000 PyKagi-0.0.3/PyKagi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-04-24 01:32:21.000000 PyKagi-0.0.3/PyKagi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-24 01:32:21.000000 PyKagi-0.0.3/PyKagi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2731 2023-04-24 01:22:21.000000 PyKagi-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-24 01:32:21.150186 PyKagi-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      903 2023-04-24 01:28:03.000000 PyKagi-0.0.3/setup.py
```

### Comparing `PyKagi-0.0.2/LICENSE` & `PyKagi-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PyKagi-0.0.2/PKG-INFO` & `PyKagi-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyKagi
-Version: 0.0.2
+Version: 0.0.3
 Summary: Kagi API Python Wrapper
 Home-page: https://github.com/WooilJeong/PyKagi
 Author: 정우일(Wooil Jeong)
 Author-email: wooil@kakao.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyKagi Version: 0.0.2 Summary: Kagi API Python
+Metadata-Version: 2.1 Name: PyKagi Version: 0.0.3 Summary: Kagi API Python
 Wrapper Home-page: https://github.com/WooilJeong/PyKagi Author: ì ì°ì¼(Wooil
 Jeong) Author-email: wooil@kakao.com License: MIT Platform: UNKNOWN Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE
                             Kagi API Python Wrapper
       ð`pip install PyKagi --upgrade` [![PyPI Latest Release](https://
```

### Comparing `PyKagi-0.0.2/PyKagi/api.py` & `PyKagi-0.0.3/PyKagi/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
                 "engine": engine,
                 "summary_type": summary_type,
                 "target_language": target_language,
                 "cache": str(cache).lower()
             }
             response = requests.get(
                 self.base_url, headers=headers, params=params)
-            print(response.url)
         else:
             headers["Content-Type"] = "application/json"
             data = {
                 "text": text,
                 "engine": engine,
                 "summary_type": summary_type,
                 "target_language": target_language,
```

### Comparing `PyKagi-0.0.2/PyKagi.egg-info/PKG-INFO` & `PyKagi-0.0.3/PyKagi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyKagi
-Version: 0.0.2
+Version: 0.0.3
 Summary: Kagi API Python Wrapper
 Home-page: https://github.com/WooilJeong/PyKagi
 Author: 정우일(Wooil Jeong)
 Author-email: wooil@kakao.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyKagi Version: 0.0.2 Summary: Kagi API Python
+Metadata-Version: 2.1 Name: PyKagi Version: 0.0.3 Summary: Kagi API Python
 Wrapper Home-page: https://github.com/WooilJeong/PyKagi Author: ì ì°ì¼(Wooil
 Jeong) Author-email: wooil@kakao.com License: MIT Platform: UNKNOWN Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE
                             Kagi API Python Wrapper
       ð`pip install PyKagi --upgrade` [![PyPI Latest Release](https://
```

### Comparing `PyKagi-0.0.2/README.md` & `PyKagi-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `PyKagi-0.0.2/setup.py` & `PyKagi-0.0.3/setup.py`

 * *Files identical despite different names*


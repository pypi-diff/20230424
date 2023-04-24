# Comparing `tmp/bingpython-0.0.19.tar.gz` & `tmp/bingpython-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bingpython-0.0.19.tar", last modified: Wed Mar 22 20:19:30 2023, max compression
+gzip compressed data, was "bingpython-0.0.21.tar", last modified: Mon Apr 24 14:45:19 2023, max compression
```

## Comparing `bingpython-0.0.19.tar` & `bingpython-0.0.21.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-03-22 20:19:30.628166 bingpython-0.0.19/
--rw-rw-rw-   0        0        0     1509 2023-03-22 20:19:30.628166 bingpython-0.0.19/PKG-INFO
--rw-rw-rw-   0        0        0      713 2023-03-22 20:04:30.000000 bingpython-0.0.19/README.md
--rw-rw-rw-   0        0        0      111 2023-03-22 20:19:30.629176 bingpython-0.0.19/setup.cfg
--rw-rw-rw-   0        0        0     1228 2023-03-22 20:07:17.000000 bingpython-0.0.19/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-22 20:19:30.614009 bingpython-0.0.19/src/
--rw-rw-rw-   0        0        0     7440 2023-03-22 20:19:16.000000 bingpython-0.0.19/src/BingPython.py
-drwxrwxrwx   0        0        0        0 2023-03-22 20:19:30.628166 bingpython-0.0.19/src/bingpython.egg-info/
--rw-rw-rw-   0        0        0     1509 2023-03-22 20:19:30.000000 bingpython-0.0.19/src/bingpython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-03-22 20:19:30.000000 bingpython-0.0.19/src/bingpython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-22 20:19:30.000000 bingpython-0.0.19/src/bingpython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-03-22 20:19:30.000000 bingpython-0.0.19/src/bingpython.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-03-22 20:19:30.000000 bingpython-0.0.19/src/bingpython.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 14:45:19.560889 bingpython-0.0.21/
+-rw-rw-rw-   0        0        0    16725 2023-04-05 08:00:45.000000 bingpython-0.0.21/LICENSE
+-rw-rw-rw-   0        0        0     1532 2023-04-24 14:45:19.561869 bingpython-0.0.21/PKG-INFO
+-rw-rw-rw-   0        0        0      713 2023-04-05 08:00:45.000000 bingpython-0.0.21/README.md
+-rw-rw-rw-   0        0        0      111 2023-04-24 14:45:19.568850 bingpython-0.0.21/setup.cfg
+-rw-rw-rw-   0        0        0     1194 2023-04-24 14:44:29.000000 bingpython-0.0.21/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:45:19.513003 bingpython-0.0.21/src/
+-rw-rw-rw-   0        0        0     9902 2023-04-24 14:43:07.000000 bingpython-0.0.21/src/BingPython.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:45:19.553905 bingpython-0.0.21/src/bingpython.egg-info/
+-rw-rw-rw-   0        0        0     1532 2023-04-24 14:45:19.000000 bingpython-0.0.21/src/bingpython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-04-24 14:45:19.000000 bingpython-0.0.21/src/bingpython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 14:45:19.000000 bingpython-0.0.21/src/bingpython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-24 14:45:19.000000 bingpython-0.0.21/src/bingpython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-24 14:45:19.000000 bingpython-0.0.21/src/bingpython.egg-info/top_level.txt
```

### Comparing `bingpython-0.0.19/PKG-INFO` & `bingpython-0.0.21/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: bingpython
-Version: 0.0.19
+Version: 0.0.21
 Summary: Bing AI Chat API
 Home-page: https://github.com/alicangnll/BingGPT-Python
 Author: Ali Can Gönüllü
 Author-email: alicangonullu@yahoo.com
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/alicangnll/BingGPT-Python/issues/new
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # BingGPT - Bing AI API on Python
 You can use BingGPT AI API on Python!
 # Requirements
 <ul>
   <li>Python 3.8+</li>
 </ul>
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: bingpython Version: 0.0.19 Summary: Bing AI Chat
+Metadata-Version: 2.1 Name: bingpython Version: 0.0.21 Summary: Bing AI Chat
 API Home-page: https://github.com/alicangnll/BingGPT-Python Author: Ali Can
 GÃ¶nÃ¼llÃ¼ Author-email: alicangonullu@yahoo.com License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/alicangnll/BingGPT-
 Python/issues/new Classifier: License :: OSI Approved :: GNU General Public
 License v2 (GPLv2) Classifier: Intended Audience :: Developers Classifier:
 Topic :: Software Development :: Libraries :: Python Modules Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Description-Content-Type: text/markdown
-# BingGPT - Bing AI API on Python You can use BingGPT AI API on Python! #
-Requirements
+License-File: LICENSE # BingGPT - Bing AI API on Python You can use BingGPT AI
+API on Python! # Requirements
     * Python 3.8+
 ****** Installation ******
     * pip install -r requirements.txt
     * pip install dist/binggpt-0.0.18-py3-none-any.whl OR pip install
       bingpython
 ****** Pictures ******
 [https://raw.githubusercontent.com/alicangnll/BingGPT-Python/main/pic/pic1.png]
```

### Comparing `bingpython-0.0.19/README.md` & `bingpython-0.0.21/README.md`

 * *Files identical despite different names*

### Comparing `bingpython-0.0.19/setup.py` & `bingpython-0.0.21/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from setuptools import find_packages
-from setuptools import setup
-
-setup(
-    name="bingpython",
-    version="0.0.19",
-    license="GNU General Public License v2.0",
-    author="Ali Can Gönüllü",
-    author_email="alicangonullu@yahoo.com",
-    description="Bing AI Chat API",
-    packages=find_packages("src"),
-    package_dir={"": "src"},
-    url="https://github.com/alicangnll/BingGPT-Python",
-    project_urls={"Bug Report": "https://github.com/alicangnll/BingGPT-Python/issues/new"},
-    install_requires=[
-        "asyncio",
-        "requests",
-        "websockets",
-        "rich",
-        "certifi",
-        "uuid"
-    ],
-    long_description=open("README.md", encoding="utf-8").read(),
-    long_description_content_type="text/markdown",
-    py_modules=["BingPython"],
-    classifiers=[
-        "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
-        "Intended Audience :: Developers",
-        "Topic :: Software Development :: Libraries :: Python Modules",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-    ],
+from setuptools import find_packages
+from setuptools import setup
+
+setup(
+    name="bingpython",
+    version="0.0.21",
+    license="GNU General Public License v2.0",
+    author="Ali Can Gönüllü",
+    author_email="alicangonullu@yahoo.com",
+    description="Bing AI Chat API",
+    packages=find_packages("src"),
+    package_dir={"": "src"},
+    url="https://github.com/alicangnll/BingGPT-Python",
+    project_urls={"Bug Report": "https://github.com/alicangnll/BingGPT-Python/issues/new"},
+    install_requires=[
+        "asyncio",
+        "requests",
+        "websockets",
+        "rich",
+        "certifi",
+        "uuid"
+    ],
+    long_description=open("README.md", encoding="utf-8").read(),
+    long_description_content_type="text/markdown",
+    py_modules=["BingPython"],
+    classifiers=[
+        "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
+        "Intended Audience :: Developers",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+    ],
 )
```

### Comparing `bingpython-0.0.19/src/bingpython.egg-info/PKG-INFO` & `bingpython-0.0.21/src/bingpython.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: bingpython
-Version: 0.0.19
+Version: 0.0.21
 Summary: Bing AI Chat API
 Home-page: https://github.com/alicangnll/BingGPT-Python
 Author: Ali Can Gönüllü
 Author-email: alicangonullu@yahoo.com
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/alicangnll/BingGPT-Python/issues/new
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # BingGPT - Bing AI API on Python
 You can use BingGPT AI API on Python!
 # Requirements
 <ul>
   <li>Python 3.8+</li>
 </ul>
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: bingpython Version: 0.0.19 Summary: Bing AI Chat
+Metadata-Version: 2.1 Name: bingpython Version: 0.0.21 Summary: Bing AI Chat
 API Home-page: https://github.com/alicangnll/BingGPT-Python Author: Ali Can
 GÃ¶nÃ¼llÃ¼ Author-email: alicangonullu@yahoo.com License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/alicangnll/BingGPT-
 Python/issues/new Classifier: License :: OSI Approved :: GNU General Public
 License v2 (GPLv2) Classifier: Intended Audience :: Developers Classifier:
 Topic :: Software Development :: Libraries :: Python Modules Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Description-Content-Type: text/markdown
-# BingGPT - Bing AI API on Python You can use BingGPT AI API on Python! #
-Requirements
+License-File: LICENSE # BingGPT - Bing AI API on Python You can use BingGPT AI
+API on Python! # Requirements
     * Python 3.8+
 ****** Installation ******
     * pip install -r requirements.txt
     * pip install dist/binggpt-0.0.18-py3-none-any.whl OR pip install
       bingpython
 ****** Pictures ******
 [https://raw.githubusercontent.com/alicangnll/BingGPT-Python/main/pic/pic1.png]
```


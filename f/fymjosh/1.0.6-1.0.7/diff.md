# Comparing `tmp/fymjosh-1.0.6.tar.gz` & `tmp/fymjosh-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fymjosh-1.0.6.tar", last modified: Sun Apr 23 22:36:42 2023, max compression
+gzip compressed data, was "fymjosh-1.0.7.tar", last modified: Sun Apr 23 23:04:50 2023, max compression
```

## Comparing `fymjosh-1.0.6.tar` & `fymjosh-1.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 22:36:41.916571 fymjosh-1.0.6/
--rw-rw-rw-   0        0        0       86 2023-02-26 01:07:18.000000 fymjosh-1.0.6/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1069 2023-02-26 01:11:20.000000 fymjosh-1.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-02-26 01:09:21.000000 fymjosh-1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      777 2023-04-23 22:36:41.910608 fymjosh-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      136 2023-02-26 01:21:48.000000 fymjosh-1.0.6/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-23 22:36:41.821921 fymjosh-1.0.6/fymjosh/
--rw-rw-rw-   0        0        0     2930 2023-04-23 22:25:09.000000 fymjosh-1.0.6/fymjosh/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 22:36:41.883528 fymjosh-1.0.6/fymjosh.egg-info/
--rw-rw-rw-   0        0        0      777 2023-04-23 22:36:40.000000 fymjosh-1.0.6/fymjosh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-04-23 22:36:40.000000 fymjosh-1.0.6/fymjosh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 22:36:40.000000 fymjosh-1.0.6/fymjosh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-04-23 22:36:40.000000 fymjosh-1.0.6/fymjosh.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-23 22:36:40.000000 fymjosh-1.0.6/fymjosh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4179 2023-03-21 14:19:07.000000 fymjosh-1.0.6/new 2.py
--rw-rw-rw-   0        0        0     4150 2023-03-21 14:56:05.000000 fymjosh-1.0.6/protect.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 22:36:41.956696 fymjosh-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      970 2023-04-23 22:27:56.000000 fymjosh-1.0.6/setup.py
--rw-rw-rw-   0        0        0     2449 2023-02-26 02:15:44.000000 fymjosh-1.0.6/vanity.py
+drwxrwxrwx   0        0        0        0 2023-04-23 23:04:50.925152 fymjosh-1.0.7/
+-rw-rw-rw-   0        0        0       86 2023-02-26 01:07:18.000000 fymjosh-1.0.7/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1069 2023-02-26 01:11:20.000000 fymjosh-1.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-02-26 01:09:21.000000 fymjosh-1.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      777 2023-04-23 23:04:50.924159 fymjosh-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      136 2023-02-26 01:21:48.000000 fymjosh-1.0.7/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 23:04:50.855204 fymjosh-1.0.7/fymjosh/
+-rw-rw-rw-   0        0        0     2912 2023-04-23 23:04:09.000000 fymjosh-1.0.7/fymjosh/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 23:04:50.920220 fymjosh-1.0.7/fymjosh.egg-info/
+-rw-rw-rw-   0        0        0      777 2023-04-23 23:04:50.000000 fymjosh-1.0.7/fymjosh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-04-23 23:04:50.000000 fymjosh-1.0.7/fymjosh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 23:04:50.000000 fymjosh-1.0.7/fymjosh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-23 23:04:50.000000 fymjosh-1.0.7/fymjosh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-23 23:04:50.000000 fymjosh-1.0.7/fymjosh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4179 2023-03-21 14:19:07.000000 fymjosh-1.0.7/new 2.py
+-rw-rw-rw-   0        0        0     4150 2023-03-21 14:56:05.000000 fymjosh-1.0.7/protect.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 23:04:50.926145 fymjosh-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      970 2023-04-23 23:04:17.000000 fymjosh-1.0.7/setup.py
+-rw-rw-rw-   0        0        0     2449 2023-02-26 02:15:44.000000 fymjosh-1.0.7/vanity.py
```

### Comparing `fymjosh-1.0.6/LICENSE.txt` & `fymjosh-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fymjosh-1.0.6/PKG-INFO` & `fymjosh-1.0.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fymjosh
-Version: 1.0.6
+Version: 1.0.7
 Summary: A library that focuses on customization of console and discord
 Home-page: UNKNOWN
 Author: fymjosh
 Author-email: lone.cord12@gmail.com
 License: MIT
 Keywords: discord,console
 Platform: UNKNOWN
```

### Comparing `fymjosh-1.0.6/fymjosh/__init__.py` & `fymjosh-1.0.7/fymjosh/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         
         faded += (f"\033[38;2;{self.red};0;220m{text}")
             
         
         return faded
         
         
-    def _write(self,datefmt=' %H:%M:%S.%f - ', text):
+    def _write(self,datefmt, text):
         
         print(self.purplepink(f"{datetime.utcnow().strftime(datefmt)}\033[37m{text}"))
         if not self.red == 255 and self.cycle == 0:
             self.red += 15
```

### Comparing `fymjosh-1.0.6/fymjosh.egg-info/PKG-INFO` & `fymjosh-1.0.7/fymjosh.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fymjosh
-Version: 1.0.6
+Version: 1.0.7
 Summary: A library that focuses on customization of console and discord
 Home-page: UNKNOWN
 Author: fymjosh
 Author-email: lone.cord12@gmail.com
 License: MIT
 Keywords: discord,console
 Platform: UNKNOWN
```

### Comparing `fymjosh-1.0.6/new 2.py` & `fymjosh-1.0.7/new 2.py`

 * *Files identical despite different names*

### Comparing `fymjosh-1.0.6/protect.txt` & `fymjosh-1.0.7/protect.txt`

 * *Files identical despite different names*

### Comparing `fymjosh-1.0.6/setup.py` & `fymjosh-1.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3',
     
 ]
 
 setup(
     name="fymjosh",
-    version="1.0.6",
+    version="1.0.7",
     description = 'A library that focuses on customization of console and discord',
     long_description ="fymjosh is a library that allows for your discord account to change statuses to like streaming, watching, listening, playing and helps to customize your discord account. Also has custom printing with rich features",
     url='',
     author='fymjosh',
     author_email='lone.cord12@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

### Comparing `fymjosh-1.0.6/vanity.py` & `fymjosh-1.0.7/vanity.py`

 * *Files identical despite different names*


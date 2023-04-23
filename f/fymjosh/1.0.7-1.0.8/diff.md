# Comparing `tmp/fymjosh-1.0.7.tar.gz` & `tmp/fymjosh-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fymjosh-1.0.7.tar", last modified: Sun Apr 23 23:04:50 2023, max compression
+gzip compressed data, was "fymjosh-1.0.8.tar", last modified: Sun Apr 23 23:15:29 2023, max compression
```

## Comparing `fymjosh-1.0.7.tar` & `fymjosh-1.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 23:04:50.925152 fymjosh-1.0.7/
--rw-rw-rw-   0        0        0       86 2023-02-26 01:07:18.000000 fymjosh-1.0.7/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1069 2023-02-26 01:11:20.000000 fymjosh-1.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-02-26 01:09:21.000000 fymjosh-1.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0      777 2023-04-23 23:04:50.924159 fymjosh-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      136 2023-02-26 01:21:48.000000 fymjosh-1.0.7/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-23 23:04:50.855204 fymjosh-1.0.7/fymjosh/
--rw-rw-rw-   0        0        0     2912 2023-04-23 23:04:09.000000 fymjosh-1.0.7/fymjosh/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 23:04:50.920220 fymjosh-1.0.7/fymjosh.egg-info/
--rw-rw-rw-   0        0        0      777 2023-04-23 23:04:50.000000 fymjosh-1.0.7/fymjosh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-04-23 23:04:50.000000 fymjosh-1.0.7/fymjosh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 23:04:50.000000 fymjosh-1.0.7/fymjosh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-04-23 23:04:50.000000 fymjosh-1.0.7/fymjosh.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-23 23:04:50.000000 fymjosh-1.0.7/fymjosh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4179 2023-03-21 14:19:07.000000 fymjosh-1.0.7/new 2.py
--rw-rw-rw-   0        0        0     4150 2023-03-21 14:56:05.000000 fymjosh-1.0.7/protect.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 23:04:50.926145 fymjosh-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      970 2023-04-23 23:04:17.000000 fymjosh-1.0.7/setup.py
--rw-rw-rw-   0        0        0     2449 2023-02-26 02:15:44.000000 fymjosh-1.0.7/vanity.py
+drwxrwxrwx   0        0        0        0 2023-04-23 23:15:29.243770 fymjosh-1.0.8/
+-rw-rw-rw-   0        0        0       86 2023-02-26 01:07:18.000000 fymjosh-1.0.8/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1069 2023-02-26 01:11:20.000000 fymjosh-1.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-02-26 01:09:21.000000 fymjosh-1.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      777 2023-04-23 23:15:29.242787 fymjosh-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      136 2023-02-26 01:21:48.000000 fymjosh-1.0.8/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 23:15:29.205033 fymjosh-1.0.8/fymjosh/
+-rw-rw-rw-   0        0        0     2921 2023-04-23 23:14:40.000000 fymjosh-1.0.8/fymjosh/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 23:15:29.238853 fymjosh-1.0.8/fymjosh.egg-info/
+-rw-rw-rw-   0        0        0      777 2023-04-23 23:15:28.000000 fymjosh-1.0.8/fymjosh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-04-23 23:15:28.000000 fymjosh-1.0.8/fymjosh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 23:15:28.000000 fymjosh-1.0.8/fymjosh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-23 23:15:28.000000 fymjosh-1.0.8/fymjosh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-23 23:15:28.000000 fymjosh-1.0.8/fymjosh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4179 2023-03-21 14:19:07.000000 fymjosh-1.0.8/new 2.py
+-rw-rw-rw-   0        0        0     4150 2023-03-21 14:56:05.000000 fymjosh-1.0.8/protect.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 23:15:29.244772 fymjosh-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      970 2023-04-23 23:14:48.000000 fymjosh-1.0.8/setup.py
+-rw-rw-rw-   0        0        0     2449 2023-02-26 02:15:44.000000 fymjosh-1.0.8/vanity.py
```

### Comparing `fymjosh-1.0.7/LICENSE.txt` & `fymjosh-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fymjosh-1.0.7/PKG-INFO` & `fymjosh-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fymjosh
-Version: 1.0.7
+Version: 1.0.8
 Summary: A library that focuses on customization of console and discord
 Home-page: UNKNOWN
 Author: fymjosh
 Author-email: lone.cord12@gmail.com
 License: MIT
 Keywords: discord,console
 Platform: UNKNOWN
```

### Comparing `fymjosh-1.0.7/fymjosh/__init__.py` & `fymjosh-1.0.8/fymjosh/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
             
         
         return faded
         
         
     def _write(self,datefmt, text):
         
-        print(self.purplepink(f"{datetime.utcnow().strftime(datefmt)}\033[37m{text}"))
+        print(self.purplepink(f"{datetime.datetime.utcnow().strftime(datefmt)}\033[37m{text}"))
         if not self.red == 255 and self.cycle == 0:
             self.red += 15
             
         
             
         if self.red > 255:
             self.cycle += 1
```

### Comparing `fymjosh-1.0.7/fymjosh.egg-info/PKG-INFO` & `fymjosh-1.0.8/fymjosh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fymjosh
-Version: 1.0.7
+Version: 1.0.8
 Summary: A library that focuses on customization of console and discord
 Home-page: UNKNOWN
 Author: fymjosh
 Author-email: lone.cord12@gmail.com
 License: MIT
 Keywords: discord,console
 Platform: UNKNOWN
```

### Comparing `fymjosh-1.0.7/new 2.py` & `fymjosh-1.0.8/new 2.py`

 * *Files identical despite different names*

### Comparing `fymjosh-1.0.7/protect.txt` & `fymjosh-1.0.8/protect.txt`

 * *Files identical despite different names*

### Comparing `fymjosh-1.0.7/setup.py` & `fymjosh-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3',
     
 ]
 
 setup(
     name="fymjosh",
-    version="1.0.7",
+    version="1.0.8",
     description = 'A library that focuses on customization of console and discord',
     long_description ="fymjosh is a library that allows for your discord account to change statuses to like streaming, watching, listening, playing and helps to customize your discord account. Also has custom printing with rich features",
     url='',
     author='fymjosh',
     author_email='lone.cord12@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

### Comparing `fymjosh-1.0.7/vanity.py` & `fymjosh-1.0.8/vanity.py`

 * *Files identical despite different names*


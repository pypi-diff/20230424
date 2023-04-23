# Comparing `tmp/fymjosh-0.0.6.tar.gz` & `tmp/fymjosh-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fymjosh-0.0.6.tar", last modified: Sun Feb 26 02:08:40 2023, max compression
+gzip compressed data, was "fymjosh-1.0.6.tar", last modified: Sun Apr 23 22:36:42 2023, max compression
```

## Comparing `fymjosh-0.0.6.tar` & `fymjosh-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-02-26 02:08:40.106948 fymjosh-0.0.6/
--rw-rw-rw-   0        0        0       86 2023-02-26 01:07:18.000000 fymjosh-0.0.6/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1069 2023-02-26 01:11:20.000000 fymjosh-0.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-02-26 01:09:21.000000 fymjosh-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      716 2023-02-26 02:08:40.103950 fymjosh-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      136 2023-02-26 01:21:48.000000 fymjosh-0.0.6/README.txt
-drwxrwxrwx   0        0        0        0 2023-02-26 02:08:39.995855 fymjosh-0.0.6/fymjosh/
--rw-rw-rw-   0        0        0     2043 2023-02-26 01:04:13.000000 fymjosh-0.0.6/fymjosh/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-26 02:08:40.098947 fymjosh-0.0.6/fymjosh.egg-info/
--rw-rw-rw-   0        0        0      716 2023-02-26 02:08:39.000000 fymjosh-0.0.6/fymjosh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-02-26 02:08:39.000000 fymjosh-0.0.6/fymjosh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-26 02:08:39.000000 fymjosh-0.0.6/fymjosh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-02-26 02:08:39.000000 fymjosh-0.0.6/fymjosh.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-02-26 02:08:39.000000 fymjosh-0.0.6/fymjosh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-26 02:08:40.106948 fymjosh-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      908 2023-02-26 02:08:20.000000 fymjosh-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 22:36:41.916571 fymjosh-1.0.6/
+-rw-rw-rw-   0        0        0       86 2023-02-26 01:07:18.000000 fymjosh-1.0.6/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1069 2023-02-26 01:11:20.000000 fymjosh-1.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-02-26 01:09:21.000000 fymjosh-1.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      777 2023-04-23 22:36:41.910608 fymjosh-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      136 2023-02-26 01:21:48.000000 fymjosh-1.0.6/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 22:36:41.821921 fymjosh-1.0.6/fymjosh/
+-rw-rw-rw-   0        0        0     2930 2023-04-23 22:25:09.000000 fymjosh-1.0.6/fymjosh/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-23 22:36:41.883528 fymjosh-1.0.6/fymjosh.egg-info/
+-rw-rw-rw-   0        0        0      777 2023-04-23 22:36:40.000000 fymjosh-1.0.6/fymjosh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-04-23 22:36:40.000000 fymjosh-1.0.6/fymjosh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 22:36:40.000000 fymjosh-1.0.6/fymjosh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-23 22:36:40.000000 fymjosh-1.0.6/fymjosh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-23 22:36:40.000000 fymjosh-1.0.6/fymjosh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4179 2023-03-21 14:19:07.000000 fymjosh-1.0.6/new 2.py
+-rw-rw-rw-   0        0        0     4150 2023-03-21 14:56:05.000000 fymjosh-1.0.6/protect.txt
+-rw-rw-rw-   0        0        0       42 2023-04-23 22:36:41.956696 fymjosh-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      970 2023-04-23 22:27:56.000000 fymjosh-1.0.6/setup.py
+-rw-rw-rw-   0        0        0     2449 2023-02-26 02:15:44.000000 fymjosh-1.0.6/vanity.py
```

### Comparing `fymjosh-0.0.6/LICENSE.txt` & `fymjosh-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fymjosh-0.0.6/fymjosh/__init__.py` & `fymjosh-1.0.6/fymjosh/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,44 @@
 
-import os, time, sys, websocket, requests, json, logging
-
+import os, time, sys, websocket, requests, json, logging, datetime
 
+class Colwrite:
+    def __init__(self):
+        self.red = 40
+        self.cycle = 0 
+    
+    def purplepink(self,text):
+        os.system("");faded = ""
+        
+        
+        faded += (f"\033[38;2;{self.red};0;220m{text}")
+            
+        
+        return faded
+        
+        
+    def _write(self,datefmt=' %H:%M:%S.%f - ', text):
+        
+        print(self.purplepink(f"{datetime.utcnow().strftime(datefmt)}\033[37m{text}"))
+        if not self.red == 255 and self.cycle == 0:
+            self.red += 15
+            
+        
+            
+        if self.red > 255:
+            self.cycle += 1
+            #self.red -= 15
+            
+                
+        if self.cycle > 0:    
+            if self.red > 40:
+                self.red -= 15
+                       
+            if self.red == 40:
+                self.cycle = 0
 
 
 
 class Status:
     
 
     def streaming(stream_name:str, atream_url:str):
```

### Comparing `fymjosh-0.0.6/setup.py` & `fymjosh-1.0.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,19 +7,19 @@
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3',
     
 ]
 
 setup(
     name="fymjosh",
-    version="0.0.6",
-    description = 'A StreamBot library to online your token with statuses',
-    long_description ="fymjosh is a library that allows for your discord account to change statuses to like streaming, watching, listening, playing and helps to customize your discord account",
+    version="1.0.6",
+    description = 'A library that focuses on customization of console and discord',
+    long_description ="fymjosh is a library that allows for your discord account to change statuses to like streaming, watching, listening, playing and helps to customize your discord account. Also has custom printing with rich features",
     url='',
     author='fymjosh',
     author_email='lone.cord12@gmail.com',
     license='MIT',
     classifiers=classifiers,
-    keywords='discord',
+    keywords='discord, console',
     packages=find_packages(),
     install_requires=['websocket', 'websocket-client', 'asyncio', 'requests']
 )
```


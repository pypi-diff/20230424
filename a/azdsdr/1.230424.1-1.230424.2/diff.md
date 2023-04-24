# Comparing `tmp/azdsdr-1.230424.1.tar.gz` & `tmp/azdsdr-1.230424.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azdsdr-1.230424.1.tar", last modified: Mon Apr 24 19:29:27 2023, max compression
+gzip compressed data, was "azdsdr-1.230424.2.tar", last modified: Mon Apr 24 19:31:37 2023, max compression
```

## Comparing `azdsdr-1.230424.1.tar` & `azdsdr-1.230424.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 19:29:27.172481 azdsdr-1.230424.1/
--rw-rw-rw-   0        0        0    12797 2023-04-24 19:29:27.172481 azdsdr-1.230424.1/PKG-INFO
--rw-rw-rw-   0        0        0    12457 2023-04-20 21:11:05.000000 azdsdr-1.230424.1/README.md
--rw-rw-rw-   0        0        0      198 2023-04-24 19:29:27.174476 azdsdr-1.230424.1/setup.cfg
--rw-rw-rw-   0        0        0      726 2023-04-24 19:27:00.000000 azdsdr-1.230424.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 19:29:27.143559 azdsdr-1.230424.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-24 19:29:27.152549 azdsdr-1.230424.1/src/azdsdr/
--rw-rw-rw-   0        0        0        0 2022-09-29 16:46:06.000000 azdsdr-1.230424.1/src/azdsdr/__init__.py
--rw-rw-rw-   0        0        0    35840 2023-03-04 19:26:54.000000 azdsdr-1.230424.1/src/azdsdr/readers.py
--rw-rw-rw-   0        0        0    10158 2023-04-24 19:23:53.000000 azdsdr-1.230424.1/src/azdsdr/tools.py
-drwxrwxrwx   0        0        0        0 2023-04-24 19:29:27.169489 azdsdr-1.230424.1/src/azdsdr.egg-info/
--rw-rw-rw-   0        0        0    12797 2023-04-24 19:29:26.000000 azdsdr-1.230424.1/src/azdsdr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-04-24 19:29:27.000000 azdsdr-1.230424.1/src/azdsdr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 19:29:26.000000 azdsdr-1.230424.1/src/azdsdr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      125 2023-04-24 19:29:26.000000 azdsdr-1.230424.1/src/azdsdr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-24 19:29:26.000000 azdsdr-1.230424.1/src/azdsdr.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-24 19:29:27.170486 azdsdr-1.230424.1/test/
--rw-rw-rw-   0        0        0    17848 2023-03-04 19:42:32.000000 azdsdr-1.230424.1/test/test.py
+drwxrwxrwx   0        0        0        0 2023-04-24 19:31:37.922356 azdsdr-1.230424.2/
+-rw-rw-rw-   0        0        0    12797 2023-04-24 19:31:37.922356 azdsdr-1.230424.2/PKG-INFO
+-rw-rw-rw-   0        0        0    12457 2023-04-20 21:11:05.000000 azdsdr-1.230424.2/README.md
+-rw-rw-rw-   0        0        0      198 2023-04-24 19:31:37.924381 azdsdr-1.230424.2/setup.cfg
+-rw-rw-rw-   0        0        0      726 2023-04-24 19:31:28.000000 azdsdr-1.230424.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 19:31:37.884299 azdsdr-1.230424.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-24 19:31:37.894793 azdsdr-1.230424.2/src/azdsdr/
+-rw-rw-rw-   0        0        0        0 2022-09-29 16:46:06.000000 azdsdr-1.230424.2/src/azdsdr/__init__.py
+-rw-rw-rw-   0        0        0    35840 2023-03-04 19:26:54.000000 azdsdr-1.230424.2/src/azdsdr/readers.py
+-rw-rw-rw-   0        0        0    10158 2023-04-24 19:30:58.000000 azdsdr-1.230424.2/src/azdsdr/tools.py
+drwxrwxrwx   0        0        0        0 2023-04-24 19:31:37.920359 azdsdr-1.230424.2/src/azdsdr.egg-info/
+-rw-rw-rw-   0        0        0    12797 2023-04-24 19:31:37.000000 azdsdr-1.230424.2/src/azdsdr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-04-24 19:31:37.000000 azdsdr-1.230424.2/src/azdsdr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 19:31:37.000000 azdsdr-1.230424.2/src/azdsdr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      125 2023-04-24 19:31:37.000000 azdsdr-1.230424.2/src/azdsdr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-24 19:31:37.000000 azdsdr-1.230424.2/src/azdsdr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 19:31:37.921356 azdsdr-1.230424.2/test/
+-rw-rw-rw-   0        0        0    17848 2023-03-04 19:42:32.000000 azdsdr-1.230424.2/test/test.py
```

### Comparing `azdsdr-1.230424.1/PKG-INFO` & `azdsdr-1.230424.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azdsdr
-Version: 1.230424.1
+Version: 1.230424.2
 Summary: This package provide functions and tools for accessing data in a easy way.
 Home-page: https://github.com/xhinker/azdsdr
 Author: Andrew Zhu
 Author-email: xhinker@hotmail.com
 License: Apache License
 Keywords: DS Data Reader
 Description-Content-Type: text/markdown
```

### Comparing `azdsdr-1.230424.1/README.md` & `azdsdr-1.230424.2/README.md`

 * *Files identical despite different names*

### Comparing `azdsdr-1.230424.1/setup.py` & `azdsdr-1.230424.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_packages
 
 setup(
     name='azdsdr',
-    version='1.230424.1',
+    version='1.230424.2',
     license='Apache License',
     author="Andrew Zhu",
     author_email='xhinker@hotmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://github.com/xhinker/azdsdr',
     keywords='DS Data Reader',
```

### Comparing `azdsdr-1.230424.1/src/azdsdr/readers.py` & `azdsdr-1.230424.2/src/azdsdr/readers.py`

 * *Files identical despite different names*

### Comparing `azdsdr-1.230424.1/src/azdsdr/tools.py` & `azdsdr-1.230424.2/src/azdsdr/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
     def human_format(self,num):
         magnitude = 0 
         while abs(num) >= 1000:
             magnitude += 1 
             num /= 1000.0 
         # add more suffixes if you need them 
-        return '%.0f%s' % (num, ['', 'K', 'M', 'B', 'T', 'P'][magnitude])
+        return '%.2f%s' % (num, ['', 'K', 'M', 'B', 'T', 'P'][magnitude])
 
     def single_bar_chart(
         self
         ,title
         ,x_list
         ,y_list
         ,rotate_x = 30
```

### Comparing `azdsdr-1.230424.1/src/azdsdr.egg-info/PKG-INFO` & `azdsdr-1.230424.2/src/azdsdr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azdsdr
-Version: 1.230424.1
+Version: 1.230424.2
 Summary: This package provide functions and tools for accessing data in a easy way.
 Home-page: https://github.com/xhinker/azdsdr
 Author: Andrew Zhu
 Author-email: xhinker@hotmail.com
 License: Apache License
 Keywords: DS Data Reader
 Description-Content-Type: text/markdown
```

### Comparing `azdsdr-1.230424.1/test/test.py` & `azdsdr-1.230424.2/test/test.py`

 * *Files identical despite different names*


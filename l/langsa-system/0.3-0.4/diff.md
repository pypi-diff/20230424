# Comparing `tmp/langsa_system-0.3.tar.gz` & `tmp/langsa_system-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langsa_system-0.3.tar", last modified: Mon Apr 24 14:45:43 2023, max compression
+gzip compressed data, was "langsa_system-0.4.tar", last modified: Mon Apr 24 14:47:15 2023, max compression
```

## Comparing `langsa_system-0.3.tar` & `langsa_system-0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 14:45:43.147114 langsa_system-0.3/
--rw-rw-rw-   0        0        0    35823 2023-04-04 10:37:11.000000 langsa_system-0.3/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-24 14:45:43.147114 langsa_system-0.3/PKG-INFO
--rw-rw-rw-   0        0        0    11534 2023-04-04 10:57:40.000000 langsa_system-0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 14:45:43.147114 langsa_system-0.3/langsa_system.egg-info/
--rw-rw-rw-   0        0        0      273 2023-04-24 14:45:43.000000 langsa_system-0.3/langsa_system.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-04-24 14:45:43.000000 langsa_system-0.3/langsa_system.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 14:45:43.000000 langsa_system-0.3/langsa_system.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 14:45:43.000000 langsa_system-0.3/langsa_system.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 14:45:43.147114 langsa_system-0.3/setup.cfg
--rw-rw-rw-   0        0        0      581 2023-04-24 14:44:54.000000 langsa_system-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 14:47:15.840348 langsa_system-0.4/
+-rw-rw-rw-   0        0        0    35823 2023-04-04 10:37:11.000000 langsa_system-0.4/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-24 14:47:15.840348 langsa_system-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    11534 2023-04-04 10:57:40.000000 langsa_system-0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 14:47:15.840348 langsa_system-0.4/langsa_system.egg-info/
+-rw-rw-rw-   0        0        0      273 2023-04-24 14:47:15.000000 langsa_system-0.4/langsa_system.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-04-24 14:47:15.000000 langsa_system-0.4/langsa_system.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 14:47:15.000000 langsa_system-0.4/langsa_system.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 14:47:15.000000 langsa_system-0.4/langsa_system.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 14:47:15.840348 langsa_system-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      581 2023-04-24 14:47:10.000000 langsa_system-0.4/setup.py
```

### Comparing `langsa_system-0.3/LICENSE` & `langsa_system-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `langsa_system-0.3/README.md` & `langsa_system-0.4/README.md`

 * *Files identical despite different names*

### Comparing `langsa_system-0.3/setup.py` & `langsa_system-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # @Software: PyCharm
 
 from setuptools import setup, find_packages
 
 
 setup(
     name='langsa_system',
-    version='0.3',
+    version='0.4',
     author="浪飒",
     url='https://github.com/langsasec/langsa-system',
     author_email="langsa-hy@qq.com",
     license="GPL",
     description='langsa-system：浪飒（langsa）进制，代表自己的进制',
     packages=find_packages(),
     package_data={
```


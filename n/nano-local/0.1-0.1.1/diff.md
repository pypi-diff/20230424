# Comparing `tmp/nano_local-0.1.tar.gz` & `tmp/nano_local-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nano_local-0.1.tar", last modified: Mon Apr 24 18:40:35 2023, max compression
+gzip compressed data, was "nano_local-0.1.1.tar", last modified: Mon Apr 24 18:58:57 2023, max compression
```

## Comparing `nano_local-0.1.tar` & `nano_local-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 bl         (501) staff       (20)        0 2023-04-24 18:40:35.000000 nano_local-0.1/
--rw-r--r--   0 bl         (501) staff       (20)      132 2023-04-24 18:40:35.000000 nano_local-0.1/PKG-INFO
--rw-r--r--   0 bl         (501) staff       (20)     5720 2023-04-24 07:12:26.000000 nano_local-0.1/README.md
-drwxr-xr-x   0 bl         (501) staff       (20)        0 2023-04-24 18:40:35.000000 nano_local-0.1/nano_local.egg-info/
--rw-r--r--   0 bl         (501) staff       (20)      132 2023-04-24 18:40:35.000000 nano_local-0.1/nano_local.egg-info/PKG-INFO
--rw-r--r--   0 bl         (501) staff       (20)      293 2023-04-24 18:40:35.000000 nano_local-0.1/nano_local.egg-info/SOURCES.txt
--rw-r--r--   0 bl         (501) staff       (20)        1 2023-04-24 18:40:35.000000 nano_local-0.1/nano_local.egg-info/dependency_links.txt
--rw-r--r--   0 bl         (501) staff       (20)      104 2023-04-24 18:40:35.000000 nano_local-0.1/nano_local.egg-info/requires.txt
--rw-r--r--   0 bl         (501) staff       (20)       10 2023-04-24 18:40:35.000000 nano_local-0.1/nano_local.egg-info/top_level.txt
-drwxr-xr-x   0 bl         (501) staff       (20)        0 2023-04-24 18:40:35.000000 nano_local-0.1/nanolocal/
--rw-r--r--   0 bl         (501) staff       (20)        0 2023-04-24 07:12:26.000000 nano_local-0.1/nanolocal/__init__.py
--rwxr-xr-x   0 bl         (501) staff       (20)    24546 2023-04-24 12:05:25.000000 nano_local-0.1/nanolocal/nl_module.py
-drwxr-xr-x   0 bl         (501) staff       (20)        0 2023-04-24 18:40:35.000000 nano_local-0.1/nanolocal/testcases/
--rw-r--r--   0 bl         (501) staff       (20)        0 2023-04-24 07:12:26.000000 nano_local-0.1/nanolocal/testcases/__init__.py
--rw-r--r--   0 bl         (501) staff       (20)     8865 2023-04-24 07:12:26.000000 nano_local-0.1/nanolocal/testcases/basic.py
--rw-r--r--   0 bl         (501) staff       (20)       38 2023-04-24 18:40:35.000000 nano_local-0.1/setup.cfg
--rw-r--r--   0 bl         (501) staff       (20)      403 2023-04-24 18:40:09.000000 nano_local-0.1/setup.py
+drwxr-xr-x   0 bl         (501) staff       (20)        0 2023-04-24 18:58:57.000000 nano_local-0.1.1/
+-rw-r--r--   0 bl         (501) staff       (20)      134 2023-04-24 18:58:57.000000 nano_local-0.1.1/PKG-INFO
+-rw-r--r--   0 bl         (501) staff       (20)     5720 2023-04-24 07:12:26.000000 nano_local-0.1.1/README.md
+drwxr-xr-x   0 bl         (501) staff       (20)        0 2023-04-24 18:58:57.000000 nano_local-0.1.1/nano_local.egg-info/
+-rw-r--r--   0 bl         (501) staff       (20)      134 2023-04-24 18:58:57.000000 nano_local-0.1.1/nano_local.egg-info/PKG-INFO
+-rw-r--r--   0 bl         (501) staff       (20)      293 2023-04-24 18:58:57.000000 nano_local-0.1.1/nano_local.egg-info/SOURCES.txt
+-rw-r--r--   0 bl         (501) staff       (20)        1 2023-04-24 18:58:57.000000 nano_local-0.1.1/nano_local.egg-info/dependency_links.txt
+-rw-r--r--   0 bl         (501) staff       (20)       96 2023-04-24 18:58:57.000000 nano_local-0.1.1/nano_local.egg-info/requires.txt
+-rw-r--r--   0 bl         (501) staff       (20)       10 2023-04-24 18:58:57.000000 nano_local-0.1.1/nano_local.egg-info/top_level.txt
+drwxr-xr-x   0 bl         (501) staff       (20)        0 2023-04-24 18:58:57.000000 nano_local-0.1.1/nanolocal/
+-rw-r--r--   0 bl         (501) staff       (20)        0 2023-04-24 07:12:26.000000 nano_local-0.1.1/nanolocal/__init__.py
+-rwxr-xr-x   0 bl         (501) staff       (20)    24546 2023-04-24 12:05:25.000000 nano_local-0.1.1/nanolocal/nl_module.py
+drwxr-xr-x   0 bl         (501) staff       (20)        0 2023-04-24 18:58:57.000000 nano_local-0.1.1/nanolocal/testcases/
+-rw-r--r--   0 bl         (501) staff       (20)        0 2023-04-24 07:12:26.000000 nano_local-0.1.1/nanolocal/testcases/__init__.py
+-rw-r--r--   0 bl         (501) staff       (20)     8865 2023-04-24 07:12:26.000000 nano_local-0.1.1/nanolocal/testcases/basic.py
+-rw-r--r--   0 bl         (501) staff       (20)       38 2023-04-24 18:58:57.000000 nano_local-0.1.1/setup.cfg
+-rw-r--r--   0 bl         (501) staff       (20)      397 2023-04-24 18:57:39.000000 nano_local-0.1.1/setup.py
```

### Comparing `nano_local-0.1/README.md` & `nano_local-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nano_local-0.1/nanolocal/nl_module.py` & `nano_local-0.1.1/nanolocal/nl_module.py`

 * *Files identical despite different names*

### Comparing `nano_local-0.1/nanolocal/testcases/basic.py` & `nano_local-0.1.1/nanolocal/testcases/basic.py`

 * *Files identical despite different names*


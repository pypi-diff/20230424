# Comparing `tmp/nano_local-0.1.2.tar.gz` & `tmp/nano_local-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nano_local-0.1.2.tar", last modified: Mon Apr 24 19:03:35 2023, max compression
+gzip compressed data, was "nano_local-0.1.3.tar", last modified: Mon Apr 24 19:49:52 2023, max compression
```

## Comparing `nano_local-0.1.2.tar` & `nano_local-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,23 @@
-drwxr-xr-x   0 bl         (501) staff       (20)        0 2023-04-24 19:03:35.000000 nano_local-0.1.2/
--rw-r--r--   0 bl         (501) staff       (20)      134 2023-04-24 19:03:35.000000 nano_local-0.1.2/PKG-INFO
--rw-r--r--   0 bl         (501) staff       (20)     5720 2023-04-24 07:12:26.000000 nano_local-0.1.2/README.md
-drwxr-xr-x   0 bl         (501) staff       (20)        0 2023-04-24 19:03:35.000000 nano_local-0.1.2/nano_local.egg-info/
--rw-r--r--   0 bl         (501) staff       (20)      134 2023-04-24 19:03:35.000000 nano_local-0.1.2/nano_local.egg-info/PKG-INFO
--rw-r--r--   0 bl         (501) staff       (20)      293 2023-04-24 19:03:35.000000 nano_local-0.1.2/nano_local.egg-info/SOURCES.txt
--rw-r--r--   0 bl         (501) staff       (20)        1 2023-04-24 19:03:35.000000 nano_local-0.1.2/nano_local.egg-info/dependency_links.txt
--rw-r--r--   0 bl         (501) staff       (20)       96 2023-04-24 19:03:35.000000 nano_local-0.1.2/nano_local.egg-info/requires.txt
--rw-r--r--   0 bl         (501) staff       (20)       10 2023-04-24 19:03:35.000000 nano_local-0.1.2/nano_local.egg-info/top_level.txt
-drwxr-xr-x   0 bl         (501) staff       (20)        0 2023-04-24 19:03:35.000000 nano_local-0.1.2/nanolocal/
--rw-r--r--   0 bl         (501) staff       (20)        0 2023-04-24 07:12:26.000000 nano_local-0.1.2/nanolocal/__init__.py
--rwxr-xr-x   0 bl         (501) staff       (20)    24546 2023-04-24 12:05:25.000000 nano_local-0.1.2/nanolocal/nl_module.py
-drwxr-xr-x   0 bl         (501) staff       (20)        0 2023-04-24 19:03:35.000000 nano_local-0.1.2/nanolocal/testcases/
--rw-r--r--   0 bl         (501) staff       (20)        0 2023-04-24 07:12:26.000000 nano_local-0.1.2/nanolocal/testcases/__init__.py
--rw-r--r--   0 bl         (501) staff       (20)     8865 2023-04-24 07:12:26.000000 nano_local-0.1.2/nanolocal/testcases/basic.py
--rw-r--r--   0 bl         (501) staff       (20)       38 2023-04-24 19:03:35.000000 nano_local-0.1.2/setup.cfg
--rw-r--r--   0 bl         (501) staff       (20)      397 2023-04-24 19:03:29.000000 nano_local-0.1.2/setup.py
+drwxr-xr-x   0 bl         (501) staff       (20)        0 2023-04-24 19:49:53.000000 nano_local-0.1.3/
+-rw-r--r--   0 bl         (501) staff       (20)      134 2023-04-24 19:49:53.000000 nano_local-0.1.3/PKG-INFO
+-rw-r--r--   0 bl         (501) staff       (20)     5720 2023-04-24 07:12:26.000000 nano_local-0.1.3/README.md
+drwxr-xr-x   0 bl         (501) staff       (20)        0 2023-04-24 19:49:53.000000 nano_local-0.1.3/nano_local.egg-info/
+-rw-r--r--   0 bl         (501) staff       (20)      134 2023-04-24 19:49:52.000000 nano_local-0.1.3/nano_local.egg-info/PKG-INFO
+-rw-r--r--   0 bl         (501) staff       (20)      453 2023-04-24 19:49:52.000000 nano_local-0.1.3/nano_local.egg-info/SOURCES.txt
+-rw-r--r--   0 bl         (501) staff       (20)        1 2023-04-24 19:49:52.000000 nano_local-0.1.3/nano_local.egg-info/dependency_links.txt
+-rw-r--r--   0 bl         (501) staff       (20)       96 2023-04-24 19:49:52.000000 nano_local-0.1.3/nano_local.egg-info/requires.txt
+-rw-r--r--   0 bl         (501) staff       (20)       10 2023-04-24 19:49:52.000000 nano_local-0.1.3/nano_local.egg-info/top_level.txt
+drwxr-xr-x   0 bl         (501) staff       (20)        0 2023-04-24 19:49:53.000000 nano_local-0.1.3/nanolocal/
+-rw-r--r--   0 bl         (501) staff       (20)        0 2023-04-24 07:12:26.000000 nano_local-0.1.3/nanolocal/__init__.py
+drwxr-xr-x   0 bl         (501) staff       (20)        0 2023-04-24 19:49:53.000000 nano_local-0.1.3/nanolocal/common/
+-rw-r--r--   0 bl         (501) staff       (20)        0 2023-04-24 19:49:11.000000 nano_local-0.1.3/nanolocal/common/__init__.py
+-rw-r--r--   0 bl         (501) staff       (20)    28068 2023-04-24 07:12:26.000000 nano_local-0.1.3/nanolocal/common/nl_block_tools.py
+-rw-r--r--   0 bl         (501) staff       (20)     6783 2023-04-24 07:12:26.000000 nano_local-0.1.3/nanolocal/common/nl_initialise.py
+-rw-r--r--   0 bl         (501) staff       (20)     2479 2023-04-24 07:12:26.000000 nano_local-0.1.3/nanolocal/common/nl_nanolib.py
+-rw-r--r--   0 bl         (501) staff       (20)    44314 2023-04-24 07:12:26.000000 nano_local-0.1.3/nanolocal/common/nl_parse_config.py
+-rw-r--r--   0 bl         (501) staff       (20)    37748 2023-04-24 07:12:26.000000 nano_local-0.1.3/nanolocal/common/nl_rpc.py
+-rwxr-xr-x   0 bl         (501) staff       (20)    24546 2023-04-24 19:48:13.000000 nano_local-0.1.3/nanolocal/nl_module.py
+drwxr-xr-x   0 bl         (501) staff       (20)        0 2023-04-24 19:49:53.000000 nano_local-0.1.3/nanolocal/testcases/
+-rw-r--r--   0 bl         (501) staff       (20)     8865 2023-04-24 07:12:26.000000 nano_local-0.1.3/nanolocal/testcases/basic.py
+-rw-r--r--   0 bl         (501) staff       (20)       38 2023-04-24 19:49:53.000000 nano_local-0.1.3/setup.cfg
+-rw-r--r--   0 bl         (501) staff       (20)      397 2023-04-24 19:49:50.000000 nano_local-0.1.3/setup.py
```

### Comparing `nano_local-0.1.2/README.md` & `nano_local-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nano_local-0.1.2/nanolocal/nl_module.py` & `nano_local-0.1.3/nanolocal/nl_module.py`

 * *Files identical despite different names*

### Comparing `nano_local-0.1.2/nanolocal/testcases/basic.py` & `nano_local-0.1.3/nanolocal/testcases/basic.py`

 * *Files identical despite different names*


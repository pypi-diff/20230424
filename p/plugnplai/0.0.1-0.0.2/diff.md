# Comparing `tmp/plugnplai-0.0.1.tar.gz` & `tmp/plugnplai-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plugnplai-0.0.1.tar", max compression
+gzip compressed data, was "plugnplai-0.0.2.tar", max compression
```

## Comparing `plugnplai-0.0.1.tar` & `plugnplai-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-04-12 16:29:06.408488 plugnplai-0.0.1/LICENSE
--rw-r--r--   0        0        0       52 2023-04-17 16:58:44.701622 plugnplai-0.0.1/README.md
--rw-r--r--   0        0        0      440 2023-04-23 15:54:14.397330 plugnplai-0.0.1/plugnplai/__init__.py
--rw-r--r--   0        0        0     4865 2023-04-23 15:21:03.489180 plugnplai-0.0.1/plugnplai/call_api.py
--rw-r--r--   0        0        0     4502 2023-04-23 15:53:08.170325 plugnplai-0.0.1/plugnplai/load.py
--rw-r--r--   0        0        0     6645 2023-04-23 15:23:07.446189 plugnplai-0.0.1/plugnplai/plugin.py
--rw-r--r--   0        0        0      400 2023-04-23 16:54:10.553601 plugnplai-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 plugnplai-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-12 16:29:06.408488 plugnplai-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1445 2023-04-23 23:39:08.792020 plugnplai-0.0.2/README.md
+-rw-r--r--   0        0        0      440 2023-04-23 23:39:08.829020 plugnplai-0.0.2/plugnplai/__init__.py
+-rw-r--r--   0        0        0     4865 2023-04-23 23:39:08.883020 plugnplai-0.0.2/plugnplai/call_api.py
+-rw-r--r--   0        0        0     4502 2023-04-23 23:39:08.885020 plugnplai-0.0.2/plugnplai/load.py
+-rw-r--r--   0        0        0     6645 2023-04-23 23:39:08.900020 plugnplai-0.0.2/plugnplai/plugin.py
+-rw-r--r--   0        0        0      400 2023-04-23 23:49:32.318067 plugnplai-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2022 1970-01-01 00:00:00.000000 plugnplai-0.0.2/PKG-INFO
```

### Comparing `plugnplai-0.0.1/LICENSE` & `plugnplai-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `plugnplai-0.0.1/plugnplai/call_api.py` & `plugnplai-0.0.2/plugnplai/call_api.py`

 * *Files identical despite different names*

### Comparing `plugnplai-0.0.1/plugnplai/load.py` & `plugnplai-0.0.2/plugnplai/load.py`

 * *Files identical despite different names*

### Comparing `plugnplai-0.0.1/plugnplai/plugin.py` & `plugnplai-0.0.2/plugnplai/plugin.py`

 * *Files identical despite different names*


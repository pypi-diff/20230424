# Comparing `tmp/caveclient-5.3.0.tar.gz` & `tmp/caveclient-5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caveclient-5.3.0.tar", last modified: Fri Apr 21 14:33:14 2023, max compression
+gzip compressed data, was "caveclient-5.3.1.tar", last modified: Mon Apr 24 02:26:14 2023, max compression
```

## Comparing `caveclient-5.3.0.tar` & `caveclient-5.3.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-21 14:33:14.838295 caveclient-5.3.0/
--rw-r--r--   0 forrestc   (503) staff       (20)       24 2020-02-28 17:30:55.000000 caveclient-5.3.0/MANIFEST.in
--rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-04-21 14:33:14.837802 caveclient-5.3.0/PKG-INFO
--rw-r--r--   0 forrestc   (503) staff       (20)      537 2023-03-24 04:01:05.000000 caveclient-5.3.0/README.rst
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-21 14:33:14.833866 caveclient-5.3.0/caveclient/
--rw-r--r--   0 forrestc   (503) staff       (20)       63 2023-04-21 14:33:11.000000 caveclient-5.3.0/caveclient/__init__.py
--rw-r--r--   0 forrestc   (503) staff       (20)    33307 2023-02-09 16:57:03.000000 caveclient-5.3.0/caveclient/annotationengine.py
--rw-r--r--   0 forrestc   (503) staff       (20)    11864 2023-01-27 00:36:02.000000 caveclient-5.3.0/caveclient/auth.py
--rw-r--r--   0 forrestc   (503) staff       (20)     8125 2023-02-09 16:57:03.000000 caveclient-5.3.0/caveclient/base.py
--rw-r--r--   0 forrestc   (503) staff       (20)    36523 2023-03-24 04:01:05.000000 caveclient-5.3.0/caveclient/chunkedgraph.py
--rw-r--r--   0 forrestc   (503) staff       (20)     2769 2023-03-29 00:16:05.000000 caveclient-5.3.0/caveclient/datastack_lookup.py
--rw-r--r--   0 forrestc   (503) staff       (20)     2784 2022-12-21 20:12:16.000000 caveclient-5.3.0/caveclient/emannotationschemas.py
--rw-r--r--   0 forrestc   (503) staff       (20)    10725 2023-04-21 14:33:06.000000 caveclient-5.3.0/caveclient/endpoints.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1810 2023-03-24 04:01:07.000000 caveclient-5.3.0/caveclient/format_utils.py
--rw-r--r--   0 forrestc   (503) staff       (20)    18573 2023-03-24 22:05:12.000000 caveclient-5.3.0/caveclient/frameworkclient.py
--rw-r--r--   0 forrestc   (503) staff       (20)    16395 2023-02-09 16:57:03.000000 caveclient-5.3.0/caveclient/infoservice.py
--rw-r--r--   0 forrestc   (503) staff       (20)     6256 2022-12-21 20:12:16.000000 caveclient-5.3.0/caveclient/jsonservice.py
--rw-r--r--   0 forrestc   (503) staff       (20)     3855 2023-03-24 04:01:07.000000 caveclient-5.3.0/caveclient/l2cache.py
--rw-r--r--   0 forrestc   (503) staff       (20)    85615 2023-04-21 14:33:06.000000 caveclient-5.3.0/caveclient/materializationengine.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1519 2021-09-20 22:23:45.000000 caveclient-5.3.0/caveclient/session_config.py
--rw-r--r--   0 forrestc   (503) staff       (20)      790 2022-12-21 20:12:16.000000 caveclient-5.3.0/caveclient/timeit.py
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-21 14:33:14.835595 caveclient-5.3.0/caveclient/tools/
--rw-r--r--   0 forrestc   (503) staff       (20)        0 2022-12-21 20:12:16.000000 caveclient-5.3.0/caveclient/tools/__init__.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1153 2022-12-21 20:12:16.000000 caveclient-5.3.0/caveclient/tools/caching.py
--rw-r--r--   0 forrestc   (503) staff       (20)     7893 2022-12-21 20:12:16.000000 caveclient-5.3.0/caveclient/tools/stage.py
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-21 14:33:14.834870 caveclient-5.3.0/caveclient.egg-info/
--rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-04-21 14:33:14.000000 caveclient-5.3.0/caveclient.egg-info/PKG-INFO
--rw-r--r--   0 forrestc   (503) staff       (20)      869 2023-04-21 14:33:14.000000 caveclient-5.3.0/caveclient.egg-info/SOURCES.txt
--rw-r--r--   0 forrestc   (503) staff       (20)        1 2023-04-21 14:33:14.000000 caveclient-5.3.0/caveclient.egg-info/dependency_links.txt
--rw-r--r--   0 forrestc   (503) staff       (20)      115 2023-04-21 14:33:14.000000 caveclient-5.3.0/caveclient.egg-info/requires.txt
--rw-r--r--   0 forrestc   (503) staff       (20)       17 2023-04-21 14:33:14.000000 caveclient-5.3.0/caveclient.egg-info/top_level.txt
--rw-r--r--   0 forrestc   (503) staff       (20)      114 2022-12-21 20:12:16.000000 caveclient-5.3.0/requirements.txt
--rw-r--r--   0 forrestc   (503) staff       (20)       38 2023-04-21 14:33:14.838394 caveclient-5.3.0/setup.cfg
--rw-r--r--   0 forrestc   (503) staff       (20)     1128 2022-12-21 20:12:16.000000 caveclient-5.3.0/setup.py
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-21 14:33:14.837473 caveclient-5.3.0/tests/
--rw-r--r--   0 forrestc   (503) staff       (20)        0 2021-04-20 22:19:21.000000 caveclient-5.3.0/tests/__init__.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1471 2023-03-24 22:05:12.000000 caveclient-5.3.0/tests/conftest.py
--rw-r--r--   0 forrestc   (503) staff       (20)     6627 2022-12-21 20:12:16.000000 caveclient-5.3.0/tests/test_annotation.py
--rw-r--r--   0 forrestc   (503) staff       (20)    30468 2022-12-21 20:12:16.000000 caveclient-5.3.0/tests/test_chunkedgraph.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1958 2022-12-21 20:12:16.000000 caveclient-5.3.0/tests/test_infoservice.py
--rw-r--r--   0 forrestc   (503) staff       (20)    18399 2023-02-09 16:57:03.000000 caveclient-5.3.0/tests/test_materialization.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-24 02:26:14.748138 caveclient-5.3.1/
+-rw-r--r--   0 forrestc   (503) staff       (20)       24 2020-02-28 17:30:55.000000 caveclient-5.3.1/MANIFEST.in
+-rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-04-24 02:26:14.747731 caveclient-5.3.1/PKG-INFO
+-rw-r--r--   0 forrestc   (503) staff       (20)      537 2023-04-23 20:02:55.000000 caveclient-5.3.1/README.rst
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-24 02:26:14.742015 caveclient-5.3.1/caveclient/
+-rw-r--r--   0 forrestc   (503) staff       (20)       63 2023-04-24 02:26:10.000000 caveclient-5.3.1/caveclient/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    33307 2023-02-09 16:57:03.000000 caveclient-5.3.1/caveclient/annotationengine.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    11864 2023-01-27 00:36:02.000000 caveclient-5.3.1/caveclient/auth.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     8125 2023-02-09 16:57:03.000000 caveclient-5.3.1/caveclient/base.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    36523 2023-04-23 20:02:55.000000 caveclient-5.3.1/caveclient/chunkedgraph.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     2769 2023-04-23 20:02:55.000000 caveclient-5.3.1/caveclient/datastack_lookup.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     2784 2022-12-21 20:12:16.000000 caveclient-5.3.1/caveclient/emannotationschemas.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    10725 2023-04-23 20:02:55.000000 caveclient-5.3.1/caveclient/endpoints.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1810 2023-04-23 20:02:55.000000 caveclient-5.3.1/caveclient/format_utils.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    18573 2023-04-23 20:02:55.000000 caveclient-5.3.1/caveclient/frameworkclient.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    16395 2023-02-09 16:57:03.000000 caveclient-5.3.1/caveclient/infoservice.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     6256 2022-12-21 20:12:16.000000 caveclient-5.3.1/caveclient/jsonservice.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     3855 2023-04-23 20:02:55.000000 caveclient-5.3.1/caveclient/l2cache.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    85649 2023-04-24 02:23:13.000000 caveclient-5.3.1/caveclient/materializationengine.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1519 2021-09-20 22:23:45.000000 caveclient-5.3.1/caveclient/session_config.py
+-rw-r--r--   0 forrestc   (503) staff       (20)      790 2022-12-21 20:12:16.000000 caveclient-5.3.1/caveclient/timeit.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-24 02:26:14.744580 caveclient-5.3.1/caveclient/tools/
+-rw-r--r--   0 forrestc   (503) staff       (20)        0 2022-12-21 20:12:16.000000 caveclient-5.3.1/caveclient/tools/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1153 2022-12-21 20:12:16.000000 caveclient-5.3.1/caveclient/tools/caching.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     7893 2022-12-21 20:12:16.000000 caveclient-5.3.1/caveclient/tools/stage.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-24 02:26:14.743719 caveclient-5.3.1/caveclient.egg-info/
+-rw-r--r--   0 forrestc   (503) staff       (20)      342 2023-04-24 02:26:14.000000 caveclient-5.3.1/caveclient.egg-info/PKG-INFO
+-rw-r--r--   0 forrestc   (503) staff       (20)      869 2023-04-24 02:26:14.000000 caveclient-5.3.1/caveclient.egg-info/SOURCES.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)        1 2023-04-24 02:26:14.000000 caveclient-5.3.1/caveclient.egg-info/dependency_links.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)      115 2023-04-24 02:26:14.000000 caveclient-5.3.1/caveclient.egg-info/requires.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)       17 2023-04-24 02:26:14.000000 caveclient-5.3.1/caveclient.egg-info/top_level.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)      114 2022-12-21 20:12:16.000000 caveclient-5.3.1/requirements.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)       38 2023-04-24 02:26:14.748217 caveclient-5.3.1/setup.cfg
+-rw-r--r--   0 forrestc   (503) staff       (20)     1128 2022-12-21 20:12:16.000000 caveclient-5.3.1/setup.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-24 02:26:14.747155 caveclient-5.3.1/tests/
+-rw-r--r--   0 forrestc   (503) staff       (20)        0 2021-04-20 22:19:21.000000 caveclient-5.3.1/tests/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1471 2023-04-23 20:02:55.000000 caveclient-5.3.1/tests/conftest.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     6627 2022-12-21 20:12:16.000000 caveclient-5.3.1/tests/test_annotation.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    30468 2022-12-21 20:12:16.000000 caveclient-5.3.1/tests/test_chunkedgraph.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1958 2022-12-21 20:12:16.000000 caveclient-5.3.1/tests/test_infoservice.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    18399 2023-02-09 16:57:03.000000 caveclient-5.3.1/tests/test_materialization.py
```

### Comparing `caveclient-5.3.0/README.rst` & `caveclient-5.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.0/caveclient/annotationengine.py` & `caveclient-5.3.1/caveclient/annotationengine.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.0/caveclient/auth.py` & `caveclient-5.3.1/caveclient/auth.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.0/caveclient/base.py` & `caveclient-5.3.1/caveclient/base.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.0/caveclient/chunkedgraph.py` & `caveclient-5.3.1/caveclient/chunkedgraph.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.0/caveclient/datastack_lookup.py` & `caveclient-5.3.1/caveclient/datastack_lookup.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.0/caveclient/emannotationschemas.py` & `caveclient-5.3.1/caveclient/emannotationschemas.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.0/caveclient/endpoints.py` & `caveclient-5.3.1/caveclient/endpoints.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.0/caveclient/format_utils.py` & `caveclient-5.3.1/caveclient/format_utils.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.0/caveclient/frameworkclient.py` & `caveclient-5.3.1/caveclient/frameworkclient.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.0/caveclient/infoservice.py` & `caveclient-5.3.1/caveclient/infoservice.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.0/caveclient/jsonservice.py` & `caveclient-5.3.1/caveclient/jsonservice.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.0/caveclient/l2cache.py` & `caveclient-5.3.1/caveclient/l2cache.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.0/caveclient/materializationengine.py` & `caveclient-5.3.1/caveclient/materializationengine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1994,14 +1994,15 @@
                 warnings.simplefilter(action="ignore", category=DeprecationWarning)
                 df = pa.deserialize(response.content)
                 df = df.copy()
 
             if metadata:
                 attrs = self._assemble_attributes(
                     [view_name],
+                    is_view=True,
                     filters={
                         "inclusive": filter_in_dict,
                         "exclusive": filter_out_dict,
                         "equal": filter_equal_dict,
                         "spatial": filter_spatial_dict,
                     },
                     select_columns=select_columns,
```

### Comparing `caveclient-5.3.0/caveclient/session_config.py` & `caveclient-5.3.1/caveclient/session_config.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.0/caveclient/timeit.py` & `caveclient-5.3.1/caveclient/timeit.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.0/caveclient/tools/caching.py` & `caveclient-5.3.1/caveclient/tools/caching.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.0/caveclient/tools/stage.py` & `caveclient-5.3.1/caveclient/tools/stage.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.0/caveclient.egg-info/SOURCES.txt` & `caveclient-5.3.1/caveclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.0/setup.py` & `caveclient-5.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.0/tests/conftest.py` & `caveclient-5.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.0/tests/test_annotation.py` & `caveclient-5.3.1/tests/test_annotation.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.0/tests/test_chunkedgraph.py` & `caveclient-5.3.1/tests/test_chunkedgraph.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.0/tests/test_infoservice.py` & `caveclient-5.3.1/tests/test_infoservice.py`

 * *Files identical despite different names*

### Comparing `caveclient-5.3.0/tests/test_materialization.py` & `caveclient-5.3.1/tests/test_materialization.py`

 * *Files identical despite different names*


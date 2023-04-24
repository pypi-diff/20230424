# Comparing `tmp/ccache_upload_redis-0.1.1a1.tar.gz` & `tmp/ccache_upload_redis-0.1.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccache_upload_redis-0.1.1a1.tar", max compression
+gzip compressed data, was "ccache_upload_redis-0.1.1a2.tar", max compression
```

## Comparing `ccache_upload_redis-0.1.1a1.tar` & `ccache_upload_redis-0.1.1a2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1097 2023-04-19 04:58:00.966726 ccache_upload_redis-0.1.1a1/LICENSE
--rw-r--r--   0        0        0     3170 2023-04-19 06:56:45.848803 ccache_upload_redis-0.1.1a1/README.md
--rwxr-xr-x   0        0        0     2244 2023-04-19 05:04:49.867881 ccache_upload_redis-0.1.1a1/ccache-download-redis
--rwxr-xr-x   0        0        0    10254 2023-04-19 06:30:07.099422 ccache_upload_redis-0.1.1a1/ccache-performance
--rwxr-xr-x   0        0        0     2532 2023-04-19 07:05:13.780841 ccache_upload_redis-0.1.1a1/ccache-upload-redis
--rw-r--r--   0        0        0     1045 2023-04-19 23:13:25.120012 ccache_upload_redis-0.1.1a1/pyproject.toml
--rw-r--r--   0        0        0     4155 1970-01-01 00:00:00.000000 ccache_upload_redis-0.1.1a1/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-04-19 04:58:00.966726 ccache_upload_redis-0.1.1a2/LICENSE
+-rw-r--r--   0        0        0     3170 2023-04-19 06:56:45.848803 ccache_upload_redis-0.1.1a2/README.md
+-rw-r--r--   0        0        0     2071 2023-04-24 09:05:19.214573 ccache_upload_redis-0.1.1a2/pyproject.toml
+-rwxr-xr-x   0        0        0     2244 2023-04-19 05:04:49.867881 ccache_upload_redis-0.1.1a2/src/ccache-download-redis.py
+-rwxr-xr-x   0        0        0    10254 2023-04-19 06:30:07.099422 ccache_upload_redis-0.1.1a2/src/ccache-performance.py
+-rwxr-xr-x   0        0        0     2532 2023-04-19 07:05:13.780841 ccache_upload_redis-0.1.1a2/src/ccache-upload-redis.py
+-rw-r--r--   0        0        0     4155 1970-01-01 00:00:00.000000 ccache_upload_redis-0.1.1a2/PKG-INFO
```

### Comparing `ccache_upload_redis-0.1.1a1/LICENSE` & `ccache_upload_redis-0.1.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `ccache_upload_redis-0.1.1a1/README.md` & `ccache_upload_redis-0.1.1a2/README.md`

 * *Files identical despite different names*

### Comparing `ccache_upload_redis-0.1.1a1/ccache-download-redis` & `ccache_upload_redis-0.1.1a2/src/ccache-download-redis.py`

 * *Files identical despite different names*

### Comparing `ccache_upload_redis-0.1.1a1/ccache-performance` & `ccache_upload_redis-0.1.1a2/src/ccache-performance.py`

 * *Files identical despite different names*

### Comparing `ccache_upload_redis-0.1.1a1/ccache-upload-redis` & `ccache_upload_redis-0.1.1a2/src/ccache-upload-redis.py`

 * *Files identical despite different names*

### Comparing `ccache_upload_redis-0.1.1a1/PKG-INFO` & `ccache_upload_redis-0.1.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccache-upload-redis
-Version: 0.1.1a1
+Version: 0.1.1a2
 Summary: A script to downloads the contents of the local ccache cache from a Redis remote storage.
 Home-page: https://github.com/berlin4apk/action-ccache-download-upload-redis
 License: GPL-3.0-or-later
 Keywords: ccache,redis,upload,download
 Author: berlin4apk
 Author-email: 83521068+berlin4apk@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
```


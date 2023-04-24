# Comparing `tmp/ccache_download_redis-0.1.1a12.tar.gz` & `tmp/ccache_download_redis-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccache_download_redis-0.1.1a12.tar", max compression
+gzip compressed data, was "ccache_download_redis-0.2.0.tar", max compression
```

## Comparing `ccache_download_redis-0.1.1a12.tar` & `ccache_download_redis-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1097 2023-04-24 10:39:24.533249 ccache_download_redis-0.1.1a12/LICENSE
--rw-r--r--   0        0        0     3170 2023-04-24 10:39:24.533249 ccache_download_redis-0.1.1a12/README.md
--rwxr-xr-x   0        0        0     2244 2023-04-19 05:04:49.867881 ccache_download_redis-0.1.1a12/ccache-download-redis
--rw-r--r--   0        0        0     2410 2023-04-24 11:04:51.599575 ccache_download_redis-0.1.1a12/pyproject.toml
--rw-r--r--   0        0        0     4151 1970-01-01 00:00:00.000000 ccache_download_redis-0.1.1a12/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-04-24 10:39:24.533249 ccache_download_redis-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3170 2023-04-24 10:39:24.533249 ccache_download_redis-0.2.0/README.md
+-rwxr-xr-x   0        0        0     2244 2023-04-19 05:04:49.867881 ccache_download_redis-0.2.0/ccache-download-redis
+-rw-r--r--   0        0        0     2407 2023-04-24 11:10:58.204879 ccache_download_redis-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4148 1970-01-01 00:00:00.000000 ccache_download_redis-0.2.0/PKG-INFO
```

### Comparing `ccache_download_redis-0.1.1a12/LICENSE` & `ccache_download_redis-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ccache_download_redis-0.1.1a12/README.md` & `ccache_download_redis-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ccache_download_redis-0.1.1a12/ccache-download-redis` & `ccache_download_redis-0.2.0/ccache-download-redis`

 * *Files identical despite different names*

### Comparing `ccache_download_redis-0.1.1a12/pyproject.toml` & `ccache_download_redis-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 #name = "ccache-download-upload-redis"
 #name = "ccache_upload_redis"
 name = "ccache-download-redis"
-version = "0.1.1a12"
+version = "0.2.0"
 description = "A script to downloads the contents of the local ccache cache from a Redis remote storage."
 authors = ["berlin4apk <83521068+berlin4apk@users.noreply.github.com>"]
 repository = "https://github.com/berlin4apk/action-ccache-download-upload-redis"
 keywords = ["ccache", "redis", "download"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 packages = [
```

### Comparing `ccache_download_redis-0.1.1a12/PKG-INFO` & `ccache_download_redis-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccache-download-redis
-Version: 0.1.1a12
+Version: 0.2.0
 Summary: A script to downloads the contents of the local ccache cache from a Redis remote storage.
 Home-page: https://github.com/berlin4apk/action-ccache-download-upload-redis
 License: GPL-3.0-or-later
 Keywords: ccache,redis,download
 Author: berlin4apk
 Author-email: 83521068+berlin4apk@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
```


# Comparing `tmp/ccache_upload_redis-0.1.1a8.tar.gz` & `tmp/ccache_upload_redis-0.1.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccache_upload_redis-0.1.1a8.tar", max compression
+gzip compressed data, was "ccache_upload_redis-0.1.1a9.tar", max compression
```

## Comparing `ccache_upload_redis-0.1.1a8.tar` & `ccache_upload_redis-0.1.1a9.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1097 2023-04-19 04:58:00.966726 ccache_upload_redis-0.1.1a8/LICENSE
--rw-r--r--   0        0        0     3170 2023-04-19 06:56:45.848803 ccache_upload_redis-0.1.1a8/README.md
--rw-r--r--   0        0        0     2275 2023-04-24 10:11:38.748418 ccache_upload_redis-0.1.1a8/pyproject.toml
--rwxr-xr-x   0        0        0     2244 2023-04-19 05:04:49.867881 ccache_upload_redis-0.1.1a8/src/ccache-download-redis
--rwxr-xr-x   0        0        0     2532 2023-04-19 07:05:13.780841 ccache_upload_redis-0.1.1a8/src/ccache-upload-redis
--rw-r--r--   0        0        0     4155 1970-01-01 00:00:00.000000 ccache_upload_redis-0.1.1a8/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-04-19 04:58:00.966726 ccache_upload_redis-0.1.1a9/LICENSE
+-rw-r--r--   0        0        0     3170 2023-04-19 06:56:45.848803 ccache_upload_redis-0.1.1a9/README.md
+-rw-r--r--   0        0        0     2281 2023-04-24 10:16:17.238344 ccache_upload_redis-0.1.1a9/pyproject.toml
+-rwxr-xr-x   0        0        0     2532 2023-04-19 07:05:13.780841 ccache_upload_redis-0.1.1a9/src/ccache-upload-redis
+-rw-r--r--   0        0        0     4155 1970-01-01 00:00:00.000000 ccache_upload_redis-0.1.1a9/PKG-INFO
```

### Comparing `ccache_upload_redis-0.1.1a8/LICENSE` & `ccache_upload_redis-0.1.1a9/LICENSE`

 * *Files identical despite different names*

### Comparing `ccache_upload_redis-0.1.1a8/README.md` & `ccache_upload_redis-0.1.1a9/README.md`

 * *Files identical despite different names*

### Comparing `ccache_upload_redis-0.1.1a8/pyproject.toml` & `ccache_upload_redis-0.1.1a9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 #name = "ccache-download-upload-redis"
 #name = "ccache_upload_redis"
 name = "ccache-upload-redis"
-version = "0.1.1a8"
+version = "0.1.1a9"
 description = "A script to downloads the contents of the local ccache cache from a Redis remote storage."
 authors = ["berlin4apk <83521068+berlin4apk@users.noreply.github.com>"]
 repository = "https://github.com/berlin4apk/action-ccache-download-upload-redis"
 keywords = ["ccache", "redis", "upload", "download"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 packages = [
@@ -24,15 +24,15 @@
 #my_package_cli = 'my_package.console:run'
 #ccache-download-redis = 'ccache-download-redis.console:run'
 ###ccache-performance-sh = { reference = "src/ccache-performance.py", type= "file" }
 #sample_script = { reference = "script-files/sample_script.sh", type= "file" }
 #extra-script-legacy = {callable = "my_package.extra_legacy:main", extras = ["time"]}
 #extra-script = {reference = "my_package.extra:main", extras = ["time"], type = "console"}
 #ccache-download-redis-sh = { reference = "src/ccache-download-redis.py", type = "file" }
-ccache-download-redis-sh = { reference = "src/ccache-download-redis", type = "file" }
+# # # ccache-download-redis-sh = { reference = "src/ccache-download-redis", type = "file" }
 #ccache-download-redis-sh = {reference = "ccache-download-redis.py", extras = ["time"], type = "file"}
 #sh-script = {reference = "bin/script1.sh", type = "file"}
 #sh-script1 = {reference = "ccache-upload-redis", type = "file"}
 #sh-script2 = {reference = "ccache-download-redis", type = "file"}
 #sh-script3 = {reference = "ccache-performance", type = "file"}
```

### Comparing `ccache_upload_redis-0.1.1a8/src/ccache-upload-redis` & `ccache_upload_redis-0.1.1a9/src/ccache-upload-redis`

 * *Files identical despite different names*

### Comparing `ccache_upload_redis-0.1.1a8/PKG-INFO` & `ccache_upload_redis-0.1.1a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccache-upload-redis
-Version: 0.1.1a8
+Version: 0.1.1a9
 Summary: A script to downloads the contents of the local ccache cache from a Redis remote storage.
 Home-page: https://github.com/berlin4apk/action-ccache-download-upload-redis
 License: GPL-3.0-or-later
 Keywords: ccache,redis,upload,download
 Author: berlin4apk
 Author-email: 83521068+berlin4apk@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
```


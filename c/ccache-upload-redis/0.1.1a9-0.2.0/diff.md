# Comparing `tmp/ccache_upload_redis-0.1.1a9.tar.gz` & `tmp/ccache_upload_redis-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccache_upload_redis-0.1.1a9.tar", max compression
+gzip compressed data, was "ccache_upload_redis-0.2.0.tar", max compression
```

## Comparing `ccache_upload_redis-0.1.1a9.tar` & `ccache_upload_redis-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1097 2023-04-19 04:58:00.966726 ccache_upload_redis-0.1.1a9/LICENSE
--rw-r--r--   0        0        0     3170 2023-04-19 06:56:45.848803 ccache_upload_redis-0.1.1a9/README.md
--rw-r--r--   0        0        0     2281 2023-04-24 10:16:17.238344 ccache_upload_redis-0.1.1a9/pyproject.toml
--rwxr-xr-x   0        0        0     2532 2023-04-19 07:05:13.780841 ccache_upload_redis-0.1.1a9/src/ccache-upload-redis
--rw-r--r--   0        0        0     4155 1970-01-01 00:00:00.000000 ccache_upload_redis-0.1.1a9/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-04-24 10:39:24.533249 ccache_upload_redis-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3170 2023-04-24 10:39:24.533249 ccache_upload_redis-0.2.0/README.md
+-rwxr-xr-x   0        0        0     2532 2023-04-19 07:05:13.780841 ccache_upload_redis-0.2.0/ccache-upload-redis
+-rw-r--r--   0        0        0     2377 2023-04-24 11:11:37.389418 ccache_upload_redis-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4142 1970-01-01 00:00:00.000000 ccache_upload_redis-0.2.0/PKG-INFO
```

### Comparing `ccache_upload_redis-0.1.1a9/LICENSE` & `ccache_upload_redis-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ccache_upload_redis-0.1.1a9/README.md` & `ccache_upload_redis-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ccache_upload_redis-0.1.1a9/pyproject.toml` & `ccache_upload_redis-0.2.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 [tool.poetry]
 #name = "ccache-download-upload-redis"
 #name = "ccache_upload_redis"
 name = "ccache-upload-redis"
-version = "0.1.1a9"
-description = "A script to downloads the contents of the local ccache cache from a Redis remote storage."
+version = "0.2.0"
+description = "A script to uploads the contents of the local ccache cache from a Redis remote storage."
 authors = ["berlin4apk <83521068+berlin4apk@users.noreply.github.com>"]
 repository = "https://github.com/berlin4apk/action-ccache-download-upload-redis"
-keywords = ["ccache", "redis", "upload", "download"]
+keywords = ["ccache", "redis", "upload"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 packages = [
-    { include = "src/ccache-upload-redis" },
+#    { include = "src/ccache-upload-redis" },
+    { include = "ccache-upload-redis" },
 ###    { include = "src/ccache-download-redis.py" },
 ###    { include = "src/ccache-performance" },
 ]
 
 [tool.poetry.scripts]
+#ccache-upload-redis-sh = { reference = "src/ccache-upload-redis", type= "file" }
+ccache-upload-redis-sh = { reference = "ccache-upload-redis", type= "file" }
 #ccache-upload-redis_cli = 'ccache-upload-redis.console:run'
 # https://github.com/python-poetry/poetry-core/pull/40/files
 ###ccache-upload-redis = 'ccache-upload-redis.console.py:run'
 #ccache-upload-redis-sh = { reference = "src/ccache-upload-redis.py", type= "file" }
-# # # # ccache-upload-redis-sh = { reference = "src/ccache-upload-redis", type= "file" }
 #my_package_cli = 'my_package.console:run'
 #ccache-download-redis = 'ccache-download-redis.console:run'
 ###ccache-performance-sh = { reference = "src/ccache-performance.py", type= "file" }
 #sample_script = { reference = "script-files/sample_script.sh", type= "file" }
 #extra-script-legacy = {callable = "my_package.extra_legacy:main", extras = ["time"]}
 #extra-script = {reference = "my_package.extra:main", extras = ["time"], type = "console"}
 #ccache-download-redis-sh = { reference = "src/ccache-download-redis.py", type = "file" }
```

### Comparing `ccache_upload_redis-0.1.1a9/src/ccache-upload-redis` & `ccache_upload_redis-0.2.0/ccache-upload-redis`

 * *Files identical despite different names*

### Comparing `ccache_upload_redis-0.1.1a9/PKG-INFO` & `ccache_upload_redis-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ccache-upload-redis
-Version: 0.1.1a9
-Summary: A script to downloads the contents of the local ccache cache from a Redis remote storage.
+Version: 0.2.0
+Summary: A script to uploads the contents of the local ccache cache from a Redis remote storage.
 Home-page: https://github.com/berlin4apk/action-ccache-download-upload-redis
 License: GPL-3.0-or-later
-Keywords: ccache,redis,upload,download
+Keywords: ccache,redis,upload
 Author: berlin4apk
 Author-email: 83521068+berlin4apk@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


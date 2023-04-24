# Comparing `tmp/ytpodgen-0.2.6.tar.gz` & `tmp/ytpodgen-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytpodgen-0.2.6.tar", max compression
+gzip compressed data, was "ytpodgen-0.3.0.tar", max compression
```

## Comparing `ytpodgen-0.2.6.tar` & `ytpodgen-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-04-17 03:41:08.602094 ytpodgen-0.2.6/LICENSE
--rw-r--r--   0        0        0     3336 2023-04-17 03:41:08.602094 ytpodgen-0.2.6/README.md
--rw-r--r--   0        0        0      616 2023-04-17 03:41:08.602094 ytpodgen-0.2.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-17 03:41:08.606094 ytpodgen-0.2.6/ytpodgen/__init__.py
--rw-r--r--   0        0        0     1193 2023-04-17 03:41:08.606094 ytpodgen-0.2.6/ytpodgen/downloader.py
--rw-r--r--   0        0        0     1225 2023-04-17 03:41:08.606094 ytpodgen-0.2.6/ytpodgen/feedgenerator.py
--rw-r--r--   0        0        0     1795 2023-04-17 03:41:08.606094 ytpodgen-0.2.6/ytpodgen/uploader.py
--rw-r--r--   0        0        0     2870 2023-04-17 03:41:08.606094 ytpodgen-0.2.6/ytpodgen/ytpodgen.py
--rw-r--r--   0        0        0     4126 1970-01-01 00:00:00.000000 ytpodgen-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-24 03:00:29.635292 ytpodgen-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3811 2023-04-24 03:00:29.635292 ytpodgen-0.3.0/README.md
+-rw-r--r--   0        0        0      616 2023-04-24 03:00:29.635292 ytpodgen-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-24 03:00:29.635292 ytpodgen-0.3.0/ytpodgen/__init__.py
+-rw-r--r--   0        0        0     1193 2023-04-24 03:00:29.635292 ytpodgen-0.3.0/ytpodgen/downloader.py
+-rw-r--r--   0        0        0     1227 2023-04-24 03:00:29.635292 ytpodgen-0.3.0/ytpodgen/feedgenerator.py
+-rw-r--r--   0        0        0     1791 2023-04-24 03:00:29.635292 ytpodgen-0.3.0/ytpodgen/uploader.py
+-rw-r--r--   0        0        0     3309 2023-04-24 03:00:29.635292 ytpodgen-0.3.0/ytpodgen/ytpodgen.py
+-rw-r--r--   0        0        0     4601 1970-01-01 00:00:00.000000 ytpodgen-0.3.0/PKG-INFO
```

### Comparing `ytpodgen-0.2.6/LICENSE` & `ytpodgen-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ytpodgen-0.2.6/README.md` & `ytpodgen-0.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-# ytpodgen - turns YouTube live streams into podcasts
+# ytpodgen
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
+command line tool to turn YouTube live streams into podcasts
+
 ## prerequisite
 - python3 and pip
 
 ## first time setup
 ```
 python3 -m pip install --user ytpodgen
 ```
@@ -64,15 +66,19 @@
 
 ## Why only Cloudflare R2, and not other S3-compatible cloud storage?
 Because:
 
 - It offers free tier for up to 10GB of storage space per month
 - With Cloudflare Worker, basic auth can be applied to the uploaded files that are made public
 
-## how I configured basic auth on Cloudflare R2 using Cloudflare Workers
+## "Private Podcasts" private url or basic auth?
+There are cases where you want to publish a podcast, but you don't want to make it public. In such cases, you can use two methods to make it private, "private url" or "basic auth".
+
+"basic auth" is more secure, but it requires additional setup. "private url" is easier to setup, but it is not as secure as "basic auth". You can create private url podcast by passing `--private-url` argument to `ytpodgen`.
+### how I configured basic auth on Cloudflare R2 using Cloudflare Workers
 1. connected a custom domain to my R2 bucket, to make the bucket public. [docs](https://developers.cloudflare.com/r2/buckets/public-buckets/)
 2. configured a basic auth worker by following steps described [here](https://qiita.com/AnaKutsu/items/1c8bd0eb938edd3c0e0a).
 3. replaced the plaintext declaration of password with worker env var. [docs](https://developers.cloudflare.com/workers/platform/environment-variables/#environment-variables-via-the-dashboard)
 4. added a trigger(custom domain route) to the basic auth worker. [docs](https://developers.cloudflare.com/workers/platform/triggers/routes/)
 
 ## TODO/IDEAS
 moved to [GitHub issues](https://github.com/harupong/ytpodgen/issues/)
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-# ytpodgen - turns YouTube live streams into podcasts [![Code style: black]
-(https://img.shields.io/badge/code%20style-black-000000.svg)](https://
-github.com/psf/black) ## prerequisite - python3 and pip ## first time setup ```
-python3 -m pip install --user ytpodgen ``` Set environment variable
-`SLACK_WEBHOOK_URL`, if you want Slack notification. If you want to upload
-files to Cloudflare R2 as well, don't forget to set three environment variables
-for Cloudflare R2. - R2_ENDPOINT_URL - R2_ACCESS_KEY_ID - R2_SECRET_ACCESS_KEY
-For now, R2 bucket name must be `podcast`. ## examples ### wait for new
-livestream, and once on the air, record it and generate podcast RSS in
-background ``` TITLE=
+# ytpodgen [![Code style: black](https://img.shields.io/badge/code%20style-
+black-000000.svg)](https://github.com/psf/black) command line tool to turn
+YouTube live streams into podcasts ## prerequisite - python3 and pip ## first
+time setup ``` python3 -m pip install --user ytpodgen ``` Set environment
+variable `SLACK_WEBHOOK_URL`, if you want Slack notification. If you want to
+upload files to Cloudflare R2 as well, don't forget to set three environment
+variables for Cloudflare R2. - R2_ENDPOINT_URL - R2_ACCESS_KEY_ID -
+R2_SECRET_ACCESS_KEY For now, R2 bucket name must be `podcast`. ## examples ###
+wait for new livestream, and once on the air, record it and generate podcast
+RSS in background ``` TITLE=
  ; #YouTube live URL that ends with "/live" HOSTNAME= ; #hostname to serve
 files from screen -dmS ${TITLE} ytpodgen --liveurl ${LIVEURL} --title ${TITLE}
 --hostname ${HOSTNAME} ``` When completed, `ytpodgen` will wait for another
 livestream. Since all the waiting might take a while, I prefer running this in
 background using `screen`. ### Why not upload them as well!? You can pass `--
 upload-r2` argument to enable file uploadig to Cloudflare R2. By enabling it,
 mp3s/RSS are uploaded to Cloudflare R2. For example, by running the commands
@@ -27,17 +27,23 @@
 exits. ## How to release Executing the commands below, and the GitHub Actions
 publishes new package to PyPI. ```bash poetry version
 inor/major> git add pyproject.toml && git commit -m $(poetry version -s) git
 push origin main gh release create --generate-notes "v$(poetry version -s)" git
 fetch --tags origin ``` ## Why only Cloudflare R2, and not other S3-compatible
 cloud storage? Because: - It offers free tier for up to 10GB of storage space
 per month - With Cloudflare Worker, basic auth can be applied to the uploaded
-files that are made public ## how I configured basic auth on Cloudflare R2
-using Cloudflare Workers 1. connected a custom domain to my R2 bucket, to make
-the bucket public. [docs](https://developers.cloudflare.com/r2/buckets/public-
+files that are made public ## "Private Podcasts" private url or basic auth?
+There are cases where you want to publish a podcast, but you don't want to make
+it public. In such cases, you can use two methods to make it private, "private
+url" or "basic auth". "basic auth" is more secure, but it requires additional
+setup. "private url" is easier to setup, but it is not as secure as "basic
+auth". You can create private url podcast by passing `--private-url` argument
+to `ytpodgen`. ### how I configured basic auth on Cloudflare R2 using
+Cloudflare Workers 1. connected a custom domain to my R2 bucket, to make the
+bucket public. [docs](https://developers.cloudflare.com/r2/buckets/public-
 buckets/) 2. configured a basic auth worker by following steps described [here]
 (https://qiita.com/AnaKutsu/items/1c8bd0eb938edd3c0e0a). 3. replaced the
 plaintext declaration of password with worker env var. [docs](https://
 developers.cloudflare.com/workers/platform/environment-variables/#environment-
 variables-via-the-dashboard) 4. added a trigger(custom domain route) to the
 basic auth worker. [docs](https://developers.cloudflare.com/workers/platform/
 triggers/routes/) ## TODO/IDEAS moved to [GitHub issues](https://github.com/
```

### Comparing `ytpodgen-0.2.6/pyproject.toml` & `ytpodgen-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ytpodgen"
-version = "0.2.6"
+version = "0.3.0"
 description = "turns YouTube live streams into podcasts"
 license = "MIT"
 authors = ["harupong <harupong@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/harupong/ytpodgen"
 
 [tool.poetry.dependencies]
```

### Comparing `ytpodgen-0.2.6/ytpodgen/downloader.py` & `ytpodgen-0.3.0/ytpodgen/downloader.py`

 * *Files identical despite different names*

### Comparing `ytpodgen-0.2.6/ytpodgen/feedgenerator.py` & `ytpodgen-0.3.0/ytpodgen/feedgenerator.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,32 +6,32 @@
 
 
 class FeedGenerator:
     def __init__(self):
         pass
 
     @staticmethod
-    def generate_rss(title, hostname):
+    def generate_rss(title, hostname, path):
         podcast = Podcast(
             name=title,
-            website=f"https://{hostname}/{title}/",
+            website=f"https://{hostname}/{path}/",
             description=title,
             explicit=False,
             withhold_from_itunes=True,
         )
 
-        FeedGenerator._add_episodes(title, hostname, podcast)
+        FeedGenerator._add_episodes(hostname, podcast, path)
         podcast.rss_file("index.rss")
 
     @staticmethod
-    def _add_episodes(title, hostname, podcast):
+    def _add_episodes(hostname, podcast, path):
         files = Path(".").glob("*.mp3")
         for file in sorted(files, reverse=True):
             media = Media(
-                url=f"https://{hostname}/{title}/{file.name}",
+                url=f"https://{hostname}/{path}/{file.name}",
                 size=file.stat().st_size,
             )
             media.populate_duration_from(file)
 
             podcast.add_episode(
                 Episode(
                     title=file.name,  # filename
```

### Comparing `ytpodgen-0.2.6/ytpodgen/uploader.py` & `ytpodgen-0.3.0/ytpodgen/uploader.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 
 
 class Uploader:
     def __init__(self):
         pass
 
     @staticmethod
-    def upload_to_r2(title, bucket="podcast"):
+    def upload_to_r2(path, bucket="podcast"):
         s3 = boto3.resource(
             "s3",
             endpoint_url=Uploader.get_env_var("R2_ENDPOINT_URL"),
             aws_access_key_id=Uploader.get_env_var("R2_ACCESS_KEY_ID"),
             aws_secret_access_key=Uploader.get_env_var("R2_SECRET_ACCESS_KEY"),
         )
 
         filetypes = r"(.+\.mp3|index.rss)"  # regex pattern in string
         files = Uploader.collect_files(filetypes)
         podcastbucket = Uploader.get_or_create_bucket(bucket, s3)
-        Uploader.upload(title, files, podcastbucket)
+        Uploader.upload(path, files, podcastbucket)
 
     @staticmethod
     def get_env_var(name):
         try:
             envvar = os.environ[name]
             return envvar
         except KeyError:
@@ -45,17 +45,17 @@
     def collect_files(pattern):
         files = [p for p in Path(".").glob("*") if re.search(pattern, str(p))]
         if not len(files):
             raise FileNotFoundError("required files not found.")
         return files
 
     @staticmethod
-    def upload(title, upload_files, podcastbucket):
+    def upload(path, upload_files, podcastbucket):
         for file in upload_files:
             try:
-                podcastbucket.upload_file(file, f"{title}/{file}")
+                podcastbucket.upload_file(file, f"{path}/{file}")
             except ClientError as e:
                 logger.error(e)
 
     @staticmethod
     def bucket_exists(s3bucket, s3) -> bool:
         return s3bucket in s3.buckets.all()
```

### Comparing `ytpodgen-0.2.6/ytpodgen/ytpodgen.py` & `ytpodgen-0.3.0/ytpodgen/ytpodgen.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import argparse
 import os
+import hashlib
 from importlib.metadata import version
 from pathlib import Path
 from textwrap import dedent
 
 
 from loguru import logger
 import requests
@@ -49,14 +50,24 @@
     )
     parser.add_argument(
         "--output",
         default=".",
         help="Output directory(default: current directory)"
     )
     parser.add_argument(
+        "--bucket",
+        default="podcast",
+        help="R2 Bucket name to upload files(default: podcast)"
+    )
+    parser.add_argument(
+        "--private",
+        action="store_true",
+        help="If specified, make the podcast private by generating hashed url."
+    )
+    parser.add_argument(
         "--version",
         action="version",
         version=get_version(),
         help="Show version and exit.",
     )
 
     args = parser.parse_args()
@@ -93,29 +104,33 @@
     except FileNotFoundError:
         create_logger(title)
         logger.error(f"Invalid argument {output} for --output option.")
         exit()
 
 
 def run(args):
+    path = args.title
+    if args.private:
+        path = hashlib.sha256(args.title.encode("utf-8")).hexdigest()
+
     if args.liveurl:
         logger.info("Running yt-dlp...")
         Downloader.download(args.title, args.liveurl)
 
     logger.info("Generating feeds...")
-    FeedGenerator.generate_rss(args.title, args.hostname)
+    FeedGenerator.generate_rss(args.title, args.hostname, path)
 
     if args.upload_r2:
         logger.info("Uploading files...")
-        Uploader.upload_to_r2(args.title)
+        Uploader.upload_to_r2(path, args.bucket)
         logger.success(
             dedent(
                 f"""
             Upload completed.  Podcast feed url:
-            https://{args.hostname}/{args.title}/index.rss
+            https://{args.hostname}/{path}/index.rss
             """
             ).strip("\n")
         )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ytpodgen-0.2.6/PKG-INFO` & `ytpodgen-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytpodgen
-Version: 0.2.6
+Version: 0.3.0
 Summary: turns YouTube live streams into podcasts
 Home-page: https://github.com/harupong/ytpodgen
 License: MIT
 Author: harupong
 Author-email: harupong@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -16,17 +16,19 @@
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: podgen (>=1.1.0,<2.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: yt-dlp (>=2023.3.4,<2024.0.0)
 Project-URL: Repository, https://github.com/harupong/ytpodgen
 Description-Content-Type: text/markdown
 
-# ytpodgen - turns YouTube live streams into podcasts
+# ytpodgen
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
+command line tool to turn YouTube live streams into podcasts
+
 ## prerequisite
 - python3 and pip
 
 ## first time setup
 ```
 python3 -m pip install --user ytpodgen
 ```
@@ -86,15 +88,19 @@
 
 ## Why only Cloudflare R2, and not other S3-compatible cloud storage?
 Because:
 
 - It offers free tier for up to 10GB of storage space per month
 - With Cloudflare Worker, basic auth can be applied to the uploaded files that are made public
 
-## how I configured basic auth on Cloudflare R2 using Cloudflare Workers
+## "Private Podcasts" private url or basic auth?
+There are cases where you want to publish a podcast, but you don't want to make it public. In such cases, you can use two methods to make it private, "private url" or "basic auth".
+
+"basic auth" is more secure, but it requires additional setup. "private url" is easier to setup, but it is not as secure as "basic auth". You can create private url podcast by passing `--private-url` argument to `ytpodgen`.
+### how I configured basic auth on Cloudflare R2 using Cloudflare Workers
 1. connected a custom domain to my R2 bucket, to make the bucket public. [docs](https://developers.cloudflare.com/r2/buckets/public-buckets/)
 2. configured a basic auth worker by following steps described [here](https://qiita.com/AnaKutsu/items/1c8bd0eb938edd3c0e0a).
 3. replaced the plaintext declaration of password with worker env var. [docs](https://developers.cloudflare.com/workers/platform/environment-variables/#environment-variables-via-the-dashboard)
 4. added a trigger(custom domain route) to the basic auth worker. [docs](https://developers.cloudflare.com/workers/platform/triggers/routes/)
 
 ## TODO/IDEAS
 moved to [GitHub issues](https://github.com/harupong/ytpodgen/issues/)
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1 Name: ytpodgen Version: 0.2.6 Summary: turns YouTube live
+Metadata-Version: 2.1 Name: ytpodgen Version: 0.3.0 Summary: turns YouTube live
 streams into podcasts Home-page: https://github.com/harupong/ytpodgen License:
 MIT Author: harupong Author-email: harupong@gmail.com Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: boto3
 (>=1.26.89,<2.0.0) Requires-Dist: click (>=8.1.3,<9.0.0) Requires-Dist: loguru
 (>=0.6.0,<0.7.0) Requires-Dist: podgen (>=1.1.0,<2.0.0) Requires-Dist: requests
 (>=2.28.2,<3.0.0) Requires-Dist: yt-dlp (>=2023.3.4,<2024.0.0) Project-URL:
 Repository, https://github.com/harupong/ytpodgen Description-Content-Type:
-text/markdown # ytpodgen - turns YouTube live streams into podcasts [![Code
-style: black](https://img.shields.io/badge/code%20style-black-000000.svg)]
-(https://github.com/psf/black) ## prerequisite - python3 and pip ## first time
-setup ``` python3 -m pip install --user ytpodgen ``` Set environment variable
-`SLACK_WEBHOOK_URL`, if you want Slack notification. If you want to upload
-files to Cloudflare R2 as well, don't forget to set three environment variables
-for Cloudflare R2. - R2_ENDPOINT_URL - R2_ACCESS_KEY_ID - R2_SECRET_ACCESS_KEY
-For now, R2 bucket name must be `podcast`. ## examples ### wait for new
-livestream, and once on the air, record it and generate podcast RSS in
-background ``` TITLE=
+text/markdown # ytpodgen [![Code style: black](https://img.shields.io/badge/
+code%20style-black-000000.svg)](https://github.com/psf/black) command line tool
+to turn YouTube live streams into podcasts ## prerequisite - python3 and pip ##
+first time setup ``` python3 -m pip install --user ytpodgen ``` Set environment
+variable `SLACK_WEBHOOK_URL`, if you want Slack notification. If you want to
+upload files to Cloudflare R2 as well, don't forget to set three environment
+variables for Cloudflare R2. - R2_ENDPOINT_URL - R2_ACCESS_KEY_ID -
+R2_SECRET_ACCESS_KEY For now, R2 bucket name must be `podcast`. ## examples ###
+wait for new livestream, and once on the air, record it and generate podcast
+RSS in background ``` TITLE=
  ; #YouTube live URL that ends with "/live" HOSTNAME= ; #hostname to serve
 files from screen -dmS ${TITLE} ytpodgen --liveurl ${LIVEURL} --title ${TITLE}
 --hostname ${HOSTNAME} ``` When completed, `ytpodgen` will wait for another
 livestream. Since all the waiting might take a while, I prefer running this in
 background using `screen`. ### Why not upload them as well!? You can pass `--
 upload-r2` argument to enable file uploadig to Cloudflare R2. By enabling it,
 mp3s/RSS are uploaded to Cloudflare R2. For example, by running the commands
@@ -37,17 +37,23 @@
 exits. ## How to release Executing the commands below, and the GitHub Actions
 publishes new package to PyPI. ```bash poetry version
 inor/major> git add pyproject.toml && git commit -m $(poetry version -s) git
 push origin main gh release create --generate-notes "v$(poetry version -s)" git
 fetch --tags origin ``` ## Why only Cloudflare R2, and not other S3-compatible
 cloud storage? Because: - It offers free tier for up to 10GB of storage space
 per month - With Cloudflare Worker, basic auth can be applied to the uploaded
-files that are made public ## how I configured basic auth on Cloudflare R2
-using Cloudflare Workers 1. connected a custom domain to my R2 bucket, to make
-the bucket public. [docs](https://developers.cloudflare.com/r2/buckets/public-
+files that are made public ## "Private Podcasts" private url or basic auth?
+There are cases where you want to publish a podcast, but you don't want to make
+it public. In such cases, you can use two methods to make it private, "private
+url" or "basic auth". "basic auth" is more secure, but it requires additional
+setup. "private url" is easier to setup, but it is not as secure as "basic
+auth". You can create private url podcast by passing `--private-url` argument
+to `ytpodgen`. ### how I configured basic auth on Cloudflare R2 using
+Cloudflare Workers 1. connected a custom domain to my R2 bucket, to make the
+bucket public. [docs](https://developers.cloudflare.com/r2/buckets/public-
 buckets/) 2. configured a basic auth worker by following steps described [here]
 (https://qiita.com/AnaKutsu/items/1c8bd0eb938edd3c0e0a). 3. replaced the
 plaintext declaration of password with worker env var. [docs](https://
 developers.cloudflare.com/workers/platform/environment-variables/#environment-
 variables-via-the-dashboard) 4. added a trigger(custom domain route) to the
 basic auth worker. [docs](https://developers.cloudflare.com/workers/platform/
 triggers/routes/) ## TODO/IDEAS moved to [GitHub issues](https://github.com/
```


# Comparing `tmp/isic-cli-5.1.0.tar.gz` & `tmp/isic-cli-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isic-cli-5.1.0.tar", last modified: Thu Apr 13 23:15:59 2023, max compression
+gzip compressed data, was "isic-cli-6.0.0.tar", last modified: Mon Apr 24 13:47:12 2023, max compression
```

## Comparing `isic-cli-5.1.0.tar` & `isic-cli-6.0.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:15:59.913542 isic-cli-5.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-13 23:15:37.000000 isic-cli-5.1.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-13 23:15:37.000000 isic-cli-5.1.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:15:59.897542 isic-cli-5.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:15:59.901542 isic-cli-5.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-13 23:15:37.000000 isic-cli-5.1.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-13 23:15:37.000000 isic-cli-5.1.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-13 23:15:37.000000 isic-cli-5.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-13 23:15:37.000000 isic-cli-5.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-13 23:15:59.913542 isic-cli-5.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-13 23:15:37.000000 isic-cli-5.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:15:59.905542 isic-cli-5.1.0/isic_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-13 23:15:37.000000 isic-cli-5.1.0/isic_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:15:59.913542 isic-cli-5.1.0/isic_cli/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     7979 2023-04-13 23:15:37.000000 isic-cli-5.1.0/isic_cli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-13 23:15:37.000000 isic-cli-5.1.0/isic_cli/cli/accession.py
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-04-13 23:15:37.000000 isic-cli-5.1.0/isic_cli/cli/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-13 23:15:37.000000 isic-cli-5.1.0/isic_cli/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-04-13 23:15:37.000000 isic-cli-5.1.0/isic_cli/cli/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-04-13 23:15:37.000000 isic-cli-5.1.0/isic_cli/cli/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-13 23:15:37.000000 isic-cli-5.1.0/isic_cli/cli/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-13 23:15:37.000000 isic-cli-5.1.0/isic_cli/cli/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-13 23:15:37.000000 isic-cli-5.1.0/isic_cli/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:15:59.913542 isic-cli-5.1.0/isic_cli/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 23:15:37.000000 isic-cli-5.1.0/isic_cli/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-04-13 23:15:37.000000 isic-cli-5.1.0/isic_cli/io/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-13 23:15:37.000000 isic-cli-5.1.0/isic_cli/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-13 23:15:37.000000 isic-cli-5.1.0/isic_cli/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:15:59.913542 isic-cli-5.1.0/isic_cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 23:15:37.000000 isic-cli-5.1.0/isic_cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-13 23:15:37.000000 isic-cli-5.1.0/isic_cli/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:15:59.913542 isic-cli-5.1.0/isic_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-13 23:15:59.000000 isic-cli-5.1.0/isic_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-13 23:15:59.000000 isic-cli-5.1.0/isic_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 23:15:59.000000 isic-cli-5.1.0/isic_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-13 23:15:59.000000 isic-cli-5.1.0/isic_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-13 23:15:59.000000 isic-cli-5.1.0/isic_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 23:15:59.000000 isic-cli-5.1.0/isic_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-13 23:15:37.000000 isic-cli-5.1.0/justfile
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-13 23:15:37.000000 isic-cli-5.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 23:15:59.913542 isic-cli-5.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-13 23:15:37.000000 isic-cli-5.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:15:59.913542 isic-cli-5.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-13 23:15:37.000000 isic-cli-5.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-13 23:15:37.000000 isic-cli-5.1.0/tests/test_cli_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-13 23:15:37.000000 isic-cli-5.1.0/tests/test_cli_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-13 23:15:37.000000 isic-cli-5.1.0/tests/test_cli_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-13 23:15:37.000000 isic-cli-5.1.0/tests/test_cli_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 23:15:37.000000 isic-cli-5.1.0/tests/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-13 23:15:37.000000 isic-cli-5.1.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-13 23:15:37.000000 isic-cli-5.1.0/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-13 23:15:37.000000 isic-cli-5.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:47:12.918415 isic-cli-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-24 13:46:51.000000 isic-cli-6.0.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-24 13:46:51.000000 isic-cli-6.0.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:47:12.914415 isic-cli-6.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:47:12.914415 isic-cli-6.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-24 13:46:51.000000 isic-cli-6.0.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-24 13:46:51.000000 isic-cli-6.0.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-24 13:46:51.000000 isic-cli-6.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-24 13:46:51.000000 isic-cli-6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-24 13:47:12.918415 isic-cli-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-24 13:46:51.000000 isic-cli-6.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:47:12.914415 isic-cli-6.0.0/isic_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-24 13:46:51.000000 isic-cli-6.0.0/isic_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:47:12.918415 isic-cli-6.0.0/isic_cli/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     7979 2023-04-24 13:46:51.000000 isic-cli-6.0.0/isic_cli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-24 13:46:51.000000 isic-cli-6.0.0/isic_cli/cli/accession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-04-24 13:46:51.000000 isic-cli-6.0.0/isic_cli/cli/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-24 13:46:51.000000 isic-cli-6.0.0/isic_cli/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-04-24 13:46:51.000000 isic-cli-6.0.0/isic_cli/cli/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-04-24 13:46:51.000000 isic-cli-6.0.0/isic_cli/cli/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-24 13:46:51.000000 isic-cli-6.0.0/isic_cli/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-24 13:46:51.000000 isic-cli-6.0.0/isic_cli/cli/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-24 13:46:51.000000 isic-cli-6.0.0/isic_cli/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:47:12.918415 isic-cli-6.0.0/isic_cli/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:46:51.000000 isic-cli-6.0.0/isic_cli/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-04-24 13:46:51.000000 isic-cli-6.0.0/isic_cli/io/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-24 13:46:51.000000 isic-cli-6.0.0/isic_cli/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-24 13:46:51.000000 isic-cli-6.0.0/isic_cli/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:47:12.918415 isic-cli-6.0.0/isic_cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:46:51.000000 isic-cli-6.0.0/isic_cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-24 13:46:51.000000 isic-cli-6.0.0/isic_cli/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:47:12.914415 isic-cli-6.0.0/isic_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-24 13:47:12.000000 isic-cli-6.0.0/isic_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-24 13:47:12.000000 isic-cli-6.0.0/isic_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:47:12.000000 isic-cli-6.0.0/isic_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-24 13:47:12.000000 isic-cli-6.0.0/isic_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-24 13:47:12.000000 isic-cli-6.0.0/isic_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-24 13:47:12.000000 isic-cli-6.0.0/isic_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-24 13:46:51.000000 isic-cli-6.0.0/justfile
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-24 13:46:51.000000 isic-cli-6.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 13:47:12.918415 isic-cli-6.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-24 13:46:51.000000 isic-cli-6.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:47:12.918415 isic-cli-6.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-24 13:46:51.000000 isic-cli-6.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-24 13:46:51.000000 isic-cli-6.0.0/tests/test_cli_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-24 13:46:51.000000 isic-cli-6.0.0/tests/test_cli_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-24 13:46:51.000000 isic-cli-6.0.0/tests/test_cli_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-24 13:46:51.000000 isic-cli-6.0.0/tests/test_cli_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 13:46:51.000000 isic-cli-6.0.0/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-24 13:46:51.000000 isic-cli-6.0.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-24 13:46:51.000000 isic-cli-6.0.0/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-24 13:46:51.000000 isic-cli-6.0.0/tox.ini
```

### Comparing `isic-cli-5.1.0/.github/workflows/ci.yml` & `isic-cli-6.0.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `isic-cli-5.1.0/.github/workflows/release.yml` & `isic-cli-6.0.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `isic-cli-5.1.0/.gitignore` & `isic-cli-6.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `isic-cli-5.1.0/LICENSE` & `isic-cli-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `isic-cli-5.1.0/PKG-INFO` & `isic-cli-6.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isic-cli
-Version: 5.1.0
+Version: 6.0.0
 Home-page: https://github.com/ImageMarkup/isic-cli
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/ImageMarkup/isic-cli/issues
 Project-URL: Source, https://github.com/ImageMarkup/isic-cli
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `isic-cli-5.1.0/README.md` & `isic-cli-6.0.0/README.md`

 * *Files identical despite different names*

### Comparing `isic-cli-5.1.0/isic_cli/cli/__init__.py` & `isic-cli-6.0.0/isic_cli/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `isic-cli-5.1.0/isic_cli/cli/accession.py` & `isic-cli-6.0.0/isic_cli/cli/accession.py`

 * *Files identical despite different names*

### Comparing `isic-cli-5.1.0/isic_cli/cli/collection.py` & `isic-cli-6.0.0/isic_cli/cli/collection.py`

 * *Files identical despite different names*

### Comparing `isic-cli-5.1.0/isic_cli/cli/image.py` & `isic-cli-6.0.0/isic_cli/cli/image.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import os
 from pathlib import Path
 import sys
 
 import click
 from click.types import IntRange
 from humanize import intcomma
+from more_itertools.more import chunked
 from rich.console import Console
 from rich.progress import Progress
 
 from isic_cli.cli.context import IsicContext
 from isic_cli.cli.types import CommaSeparatedIdentifiers, SearchString
 from isic_cli.cli.utils import _extract_metadata, get_attributions, suggest_guest_login
 from isic_cli.io.http import download_image, get_images, get_num_images
@@ -94,36 +95,30 @@
     # (crashes) where they may not have gotten cleaned up.
     cleanup_partially_downloaded_files(outdir)
 
     with Progress(console=Console(file=sys.stderr)) as progress:
         archive_num_images = get_num_images(ctx.session, search, collections)
         download_num_images = archive_num_images if limit == 0 else min(archive_num_images, limit)
         nice_num_images = intcomma(download_num_images)
-
-        task1 = progress.add_task(
-            f"Downloading image information ({nice_num_images} total)",
+        task = progress.add_task(
+            f"Downloading images (and metadata) ({nice_num_images} total)",
             total=download_num_images,
         )
-        task2 = progress.add_task(
-            f"Downloading image files ({nice_num_images} total)", total=download_num_images
-        )
+        # the futures ThreadPoolExecutor doesn't allow one to easily Ctrl-c
+        thread_pool = ThreadPool(max(10, os.cpu_count() or 10))
         images_iterator = itertools.islice(
             get_images(ctx.session, search, collections), download_num_images
         )
-        images = []
 
         # See comment above _extract_metadata for why this is necessary
-        for image in images_iterator:
-            images.append(image)
-            progress.update(task1, advance=1)
-
-        # the futures ThreadPoolExecutor doesn't allow one to easily Ctrl-c
-        thread_pool = ThreadPool(max(10, os.cpu_count() or 10))
-        func = functools.partial(download_image, to=outdir, progress=progress, task=task2)
-        thread_pool.map(func, images)
+        images = []
+        func = functools.partial(download_image, to=outdir, progress=progress, task=task)
+        for image_chunk in chunked(images_iterator, 100):
+            images.extend(image_chunk)
+            thread_pool.map(func, image_chunk)
 
         headers, records = _extract_metadata(images)
         with (outdir / "metadata.csv").open("w", encoding="utf8") as outfile:
             writer = csv.DictWriter(outfile, headers)
             writer.writeheader()
             writer.writerows(records)
```

### Comparing `isic-cli-5.1.0/isic_cli/cli/metadata.py` & `isic-cli-6.0.0/isic_cli/cli/metadata.py`

 * *Files identical despite different names*

### Comparing `isic-cli-5.1.0/isic_cli/cli/types.py` & `isic-cli-6.0.0/isic_cli/cli/types.py`

 * *Files identical despite different names*

### Comparing `isic-cli-5.1.0/isic_cli/cli/user.py` & `isic-cli-6.0.0/isic_cli/cli/user.py`

 * *Files identical despite different names*

### Comparing `isic-cli-5.1.0/isic_cli/cli/utils.py` & `isic-cli-6.0.0/isic_cli/cli/utils.py`

 * *Files identical despite different names*

### Comparing `isic-cli-5.1.0/isic_cli/io/http.py` & `isic-cli-6.0.0/isic_cli/io/http.py`

 * *Files identical despite different names*

### Comparing `isic-cli-5.1.0/isic_cli/session.py` & `isic-cli-6.0.0/isic_cli/session.py`

 * *Files identical despite different names*

### Comparing `isic-cli-5.1.0/isic_cli/utils/version.py` & `isic-cli-6.0.0/isic_cli/utils/version.py`

 * *Files identical despite different names*

### Comparing `isic-cli-5.1.0/isic_cli.egg-info/PKG-INFO` & `isic-cli-6.0.0/isic_cli.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isic-cli
-Version: 5.1.0
+Version: 6.0.0
 Home-page: https://github.com/ImageMarkup/isic-cli
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/ImageMarkup/isic-cli/issues
 Project-URL: Source, https://github.com/ImageMarkup/isic-cli
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `isic-cli-5.1.0/isic_cli.egg-info/SOURCES.txt` & `isic-cli-6.0.0/isic_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `isic-cli-5.1.0/pyproject.toml` & `isic-cli-6.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `isic-cli-5.1.0/setup.py` & `isic-cli-6.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `isic-cli-5.1.0/tests/conftest.py` & `isic-cli-6.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `isic-cli-5.1.0/tests/test_cli_base.py` & `isic-cli-6.0.0/tests/test_cli_base.py`

 * *Files identical despite different names*

### Comparing `isic-cli-5.1.0/tests/test_cli_collection.py` & `isic-cli-6.0.0/tests/test_cli_collection.py`

 * *Files identical despite different names*

### Comparing `isic-cli-5.1.0/tests/test_cli_image.py` & `isic-cli-6.0.0/tests/test_cli_image.py`

 * *Files identical despite different names*

### Comparing `isic-cli-5.1.0/tests/test_cli_metadata.py` & `isic-cli-6.0.0/tests/test_cli_metadata.py`

 * *Files identical despite different names*

### Comparing `isic-cli-5.1.0/tests/test_utils.py` & `isic-cli-6.0.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `isic-cli-5.1.0/tox.ini` & `isic-cli-6.0.0/tox.ini`

 * *Files identical despite different names*


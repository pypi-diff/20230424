# Comparing `tmp/lndb_storage-0.2rc5.tar.gz` & `tmp/lndb_storage-0.2rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lndb_storage-0.2rc5.tar", last modified: Tue Apr 18 11:37:12 2023, max compression
+gzip compressed data, was "lndb_storage-0.2rc6.tar", last modified: Mon Apr 24 16:54:33 2023, max compression
```

## Comparing `lndb_storage-0.2rc5.tar` & `lndb_storage-0.2rc6.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0     3181 2023-04-10 13:55:12.337864 lndb_storage-0.2rc5/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-03-29 20:45:21.388328 lndb_storage-0.2rc5/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-03-29 20:45:21.388401 lndb_storage-0.2rc5/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1199 2023-03-29 20:45:21.388463 lndb_storage-0.2rc5/.gitignore
--rw-r--r--   0        0        0     1758 2023-03-29 20:45:21.388537 lndb_storage-0.2rc5/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-03-29 20:45:21.388633 lndb_storage-0.2rc5/LICENSE
--rw-r--r--   0        0        0      124 2023-03-29 20:45:21.388936 lndb_storage-0.2rc5/README.md
--rw-r--r--   0        0        0     2314 2023-04-18 11:36:46.449362 lndb_storage-0.2rc5/docs/changelog.md
--rw-r--r--   0        0        0     4351 2023-04-16 20:58:33.197754 lndb_storage-0.2rc5/docs/guide/add-replace-stage.ipynb
--rw-r--r--   0        0        0       88 2023-04-09 22:14:23.875135 lndb_storage-0.2rc5/docs/guide/index.md
--rw-r--r--   0        0        0     3976 2023-04-08 09:43:17.308905 lndb_storage-0.2rc5/docs/guide/iris.csv
--rw-r--r--   0        0        0     4550 2023-04-08 09:43:17.309082 lndb_storage-0.2rc5/docs/guide/iris.data
--rw-r--r--   0        0        0     4615 2023-04-10 12:49:18.628116 lndb_storage-0.2rc5/docs/guide/serialize-cache.ipynb
--rw-r--r--   0        0        0     7032 2023-04-16 21:09:57.518313 lndb_storage-0.2rc5/docs/guide/stream.ipynb
--rw-r--r--   0        0        0     7566 2023-04-10 10:36:19.544617 lndb_storage-0.2rc5/docs/guide/upload.ipynb
--rw-r--r--   0        0        0      122 2023-04-10 13:20:18.123402 lndb_storage-0.2rc5/docs/index.md
--rw-r--r--   0        0        0       60 2023-04-09 20:42:44.949390 lndb_storage-0.2rc5/docs/reference.md
--rw-r--r--   0        0        0      160 2023-03-29 20:45:21.390164 lndb_storage-0.2rc5/lamin-project.yaml
--rw-r--r--   0        0        0      580 2023-04-18 11:36:25.922864 lndb_storage-0.2rc5/lndb_storage/__init__.py
--rw-r--r--   0        0        0     3337 2023-04-18 11:35:08.919567 lndb_storage-0.2rc5/lndb_storage/_file.py
--rw-r--r--   0        0        0      492 2023-04-16 20:58:33.198299 lndb_storage-0.2rc5/lndb_storage/_h5ad.py
--rw-r--r--   0        0        0      204 2023-03-29 20:45:21.390606 lndb_storage-0.2rc5/lndb_storage/_images.py
--rw-r--r--   0        0        0     2307 2023-03-29 20:45:21.390671 lndb_storage-0.2rc5/lndb_storage/_subset.py
--rw-r--r--   0        0        0     2764 2023-04-09 20:42:44.950408 lndb_storage-0.2rc5/lndb_storage/_zarr.py
--rw-r--r--   0        0        0      317 2023-03-29 20:45:21.390956 lndb_storage-0.2rc5/lndb_storage/object/__init__.py
--rw-r--r--   0        0        0      945 2023-04-16 20:58:33.198732 lndb_storage-0.2rc5/lndb_storage/object/_anndata.py
--rw-r--r--   0        0        0      730 2023-03-29 20:45:21.391077 lndb_storage-0.2rc5/lndb_storage/object/_anndata_sizes.py
--rw-r--r--   0        0        0      900 2023-03-29 20:45:21.391132 lndb_storage-0.2rc5/lndb_storage/object/_core.py
--rw-r--r--   0        0        0     4116 2023-03-29 20:45:21.391201 lndb_storage-0.2rc5/lndb_storage/object/_lazy_field.py
--rw-r--r--   0        0        0     3507 2023-04-09 20:42:44.950762 lndb_storage-0.2rc5/lndb_storage/object/_subset_anndata.py
--rw-r--r--   0        0        0      913 2023-04-09 22:16:03.478614 lndb_storage-0.2rc5/noxfile.py
--rw-r--r--   0        0        0     1064 2023-04-16 20:58:33.198898 lndb_storage-0.2rc5/pyproject.toml
--rw-r--r--   0        0        0      490 2023-03-29 20:45:21.391918 lndb_storage-0.2rc5/tests/test_notebooks.py
--rw-r--r--   0        0        0     1127 1970-01-01 00:00:00.000000 lndb_storage-0.2rc5/PKG-INFO
+-rw-r--r--   0        0        0     3181 2023-04-10 13:55:12.337864 lndb_storage-0.2rc6/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-03-29 20:45:21.388328 lndb_storage-0.2rc6/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-03-29 20:45:21.388401 lndb_storage-0.2rc6/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1199 2023-03-29 20:45:21.388463 lndb_storage-0.2rc6/.gitignore
+-rw-r--r--   0        0        0     1765 2023-04-24 16:53:24.500304 lndb_storage-0.2rc6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-03-29 20:45:21.388633 lndb_storage-0.2rc6/LICENSE
+-rw-r--r--   0        0        0      124 2023-03-29 20:45:21.388936 lndb_storage-0.2rc6/README.md
+-rw-r--r--   0        0        0     2770 2023-04-24 16:54:08.774433 lndb_storage-0.2rc6/docs/changelog.md
+-rw-r--r--   0        0        0     9684 2023-04-23 22:03:51.292643 lndb_storage-0.2rc6/docs/guide/add-replace-stage.ipynb
+-rw-r--r--   0        0        0       88 2023-04-09 22:14:23.875135 lndb_storage-0.2rc6/docs/guide/index.md
+-rw-r--r--   0        0        0     3976 2023-04-08 09:43:17.308905 lndb_storage-0.2rc6/docs/guide/iris.csv
+-rw-r--r--   0        0        0     4550 2023-04-08 09:43:17.309082 lndb_storage-0.2rc6/docs/guide/iris.data
+-rw-r--r--   0        0        0     4349 2023-04-23 22:03:51.292792 lndb_storage-0.2rc6/docs/guide/new_iris.csv
+-rw-r--r--   0        0        0     4615 2023-04-10 12:49:18.628116 lndb_storage-0.2rc6/docs/guide/serialize-cache.ipynb
+-rw-r--r--   0        0        0     4069 2023-04-24 16:53:24.501276 lndb_storage-0.2rc6/docs/guide/stream.ipynb
+-rw-r--r--   0        0        0     7566 2023-04-10 10:36:19.544617 lndb_storage-0.2rc6/docs/guide/upload.ipynb
+-rw-r--r--   0        0        0      122 2023-04-10 13:20:18.123402 lndb_storage-0.2rc6/docs/index.md
+-rw-r--r--   0        0        0       60 2023-04-09 20:42:44.949390 lndb_storage-0.2rc6/docs/reference.md
+-rw-r--r--   0        0        0      160 2023-03-29 20:45:21.390164 lndb_storage-0.2rc6/lamin-project.yaml
+-rw-r--r--   0        0        0      580 2023-04-24 16:53:45.180185 lndb_storage-0.2rc6/lndb_storage/__init__.py
+-rw-r--r--   0        0        0     3337 2023-04-18 11:35:08.919567 lndb_storage-0.2rc6/lndb_storage/_file.py
+-rw-r--r--   0        0        0      492 2023-04-16 20:58:33.198299 lndb_storage-0.2rc6/lndb_storage/_h5ad.py
+-rw-r--r--   0        0        0      204 2023-03-29 20:45:21.390606 lndb_storage-0.2rc6/lndb_storage/_images.py
+-rw-r--r--   0        0        0     2307 2023-03-29 20:45:21.390671 lndb_storage-0.2rc6/lndb_storage/_subset.py
+-rw-r--r--   0        0        0     2764 2023-04-09 20:42:44.950408 lndb_storage-0.2rc6/lndb_storage/_zarr.py
+-rw-r--r--   0        0        0      317 2023-03-29 20:45:21.390956 lndb_storage-0.2rc6/lndb_storage/object/__init__.py
+-rw-r--r--   0        0        0      945 2023-04-16 20:58:33.198732 lndb_storage-0.2rc6/lndb_storage/object/_anndata.py
+-rw-r--r--   0        0        0      730 2023-03-29 20:45:21.391077 lndb_storage-0.2rc6/lndb_storage/object/_anndata_sizes.py
+-rw-r--r--   0        0        0      900 2023-03-29 20:45:21.391132 lndb_storage-0.2rc6/lndb_storage/object/_core.py
+-rw-r--r--   0        0        0     4116 2023-03-29 20:45:21.391201 lndb_storage-0.2rc6/lndb_storage/object/_lazy_field.py
+-rw-r--r--   0        0        0     4937 2023-04-24 16:53:24.501473 lndb_storage-0.2rc6/lndb_storage/object/_subset_anndata.py
+-rw-r--r--   0        0        0      919 2023-04-24 16:53:24.501654 lndb_storage-0.2rc6/noxfile.py
+-rw-r--r--   0        0        0     1086 2023-04-24 02:04:57.542525 lndb_storage-0.2rc6/pyproject.toml
+-rw-r--r--   0        0        0      490 2023-03-29 20:45:21.391918 lndb_storage-0.2rc6/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1175 1970-01-01 00:00:00.000000 lndb_storage-0.2rc6/PKG-INFO
```

### Comparing `lndb_storage-0.2rc5/.github/workflows/build.yml` & `lndb_storage-0.2rc6/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc5/.github/workflows/latest-changes.yml` & `lndb_storage-0.2rc6/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc5/.gitignore` & `lndb_storage-0.2rc6/.gitignore`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc5/.pre-commit-config.yaml` & `lndb_storage-0.2rc6/.pre-commit-config.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
       - id: flake8
         additional_dependencies:
           - flake8-black==0.3.3
           - flake8-typing-imports==1.10.0
         language_version: python3
         args:
           - --max-line-length=88
-          - --ignore=E203
+          - --ignore=E203,TYP001
         exclude: |
           (?x)(
               __init__.py
           )
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: v2.6.2
     hooks:
```

### Comparing `lndb_storage-0.2rc5/LICENSE` & `lndb_storage-0.2rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc5/docs/changelog.md` & `lndb_storage-0.2rc6/docs/changelog.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+✨ Add `CloudAnnData` | [26](https://github.com/laminlabs/lndb-storage/pull/26) | [falexwolf](https://github.com/falexwolf) | 2023-04-24 | 0.2rc6
+📝 Drastically simplify streaming guide | [25](https://github.com/laminlabs/lndb-storage/pull/25) | [falexwolf](https://github.com/falexwolf) | 2023-04-24 |
+✅ Add additional tests for replace | [24](https://github.com/laminlabs/lndb-storage/pull/24) | [Koncopd](https://github.com/Koncopd) | 2023-04-23 |
 ✅ Check add with key | [20](https://github.com/laminlabs/lndb-storage/pull/20) | [Koncopd](https://github.com/Koncopd) | 2023-04-16 | 0.2rc5
 ♻️ Refactoring | [19](https://github.com/laminlabs/lndb-storage/pull/19) | [Koncopd](https://github.com/Koncopd) | 2023-04-16 |
 ♻️ Remove call to nbproject in progress bar | [18](https://github.com/laminlabs/lndb-storage/pull/18) | [falexwolf](https://github.com/falexwolf) | 2023-04-14 | 0.2rc4
 ✅ Introduce separate upload guide | [14](https://github.com/laminlabs/lndb-storage/pull/14) | [falexwolf](https://github.com/falexwolf) | 2023-04-09 | 0.2rc3
 💚 Attempt fix CI | [12](https://github.com/laminlabs/lndb-storage/pull/12) | [falexwolf](https://github.com/falexwolf) | 2023-04-09 |
 🚚 Move `UPath` back to `lndb` | [11](https://github.com/laminlabs/lndb-storage/pull/11) | [falexwolf](https://github.com/falexwolf) | 2023-04-08 |
 ✅ Add test for replace and stage | [10](https://github.com/laminlabs/lndb-storage/pull/10) | [Koncopd](https://github.com/Koncopd) | 2023-04-04 |
```

### Comparing `lndb_storage-0.2rc5/docs/guide/add-replace-stage.ipynb` & `lndb_storage-0.2rc6/docs/guide/stream.ipynb`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7839316716269842%*

 * *Differences: {"'cells'": "{0: {'source': ['# Stream data'], delete: ['id']}, 1: {'cell_type': 'markdown', "*

 * *            "'source': ['When working with large serialized objects, it is often inefficient to "*

 * *            "load entire files into memory.\\n', '\\n', 'Here, we show how to subset an `AnnData` "*

 * *            "stored in the cloud.'], delete: ['execution_count', 'id', 'outputs']}, 2: {'source': "*

 * *            "['import lamindb as ln'], delete: ['id']}, 3: {'source': ['ln.track()'], delete: "*

 * *            "['id']}, 4 […]*

```diff
@@ -1,214 +1,180 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "30fd690f",
             "metadata": {},
             "source": [
-                "# Add, replace, stage and delete files"
+                "# Stream data"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "dca2c05d",
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "import lamindb as ln\n",
-                "from lndb.dev.upath import UPath"
+                "When working with large serialized objects, it is often inefficient to load entire files into memory.\n",
+                "\n",
+                "Here, we show how to subset an `AnnData` stored in the cloud."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "1c5186af",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.track()"
+                "import lamindb as ln"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "21d11d75",
             "metadata": {},
             "outputs": [],
             "source": [
-                "file = ln.File(\"iris.csv\")"
+                "ln.track()"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "b780712e",
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "ln.add(file)"
+                "Check the configured storage:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "293eac7f",
             "metadata": {},
             "outputs": [],
             "source": [
-                "cache_csv_path = file.stage()"
+                "ln.setup.settings.storage.root"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "7372ea62",
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "cache_csv_path"
+                "Register a file:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "dfefd884",
             "metadata": {},
             "outputs": [],
             "source": [
-                "assert cache_csv_path.suffix == \".csv\""
+                "file = ln.File(\"s3://lamindb-ci/lndb-storage/pbmc68k.h5ad\")\n",
+                "file = ln.add(file)"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "a8492c68",
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "file.replace(\"iris.data\")"
+                "Get its backed cloud representation:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "f36159d9",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.add(file)"
+                "adata = file.backed()"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "3b695dde",
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "cache_data_path = file.stage()"
+                "Inspect its metadata:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "f71f4a3c",
             "metadata": {},
             "outputs": [],
             "source": [
-                "cache_data_path"
+                "adata.obs.head()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "8edba44a",
             "metadata": {},
             "outputs": [],
             "source": [
-                "assert cache_data_path.suffix == \".data\""
+                "adata.obs.cell_type.value_counts()"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "c75115b2",
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "assert cache_data_path.stat().st_mtime >= cache_csv_path.stat().st_mtime"
+                "Construct a subsetter based on the metadata:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "7273324a",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.delete(file, delete_data_from_storage=True)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "bff43702",
-            "metadata": {},
-            "source": [
-                "## Add with `key`"
+                "obs = file.subsetter()\n",
+                "subset_obs = obs.cell_type.isin([\"Dendritic cells\", \"CD14+ Monocytes\"]) & (\n",
+                "    obs.percent_mito <= 0.05\n",
+                ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "48d77993",
             "metadata": {},
             "outputs": [],
             "source": [
-                "file = ln.File(\"iris.csv\", key=\"iris.csv\")"
+                "adata_subset = file.stream(subset_obs=subset_obs)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "4249829f",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.add(file)"
+                "adata_subset"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "7d7f97fe",
             "metadata": {},
             "outputs": [],
             "source": [
-                "key_path = UPath(\"s3://lamindb-ci/iris.csv\")"
+                "adata_subset.obs.cell_type.value_counts()"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "fb8790e5",
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "assert key_path.exists()"
+                "You can do the same with a zarr object:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "ced86160",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.delete(file, delete_data_from_storage=True)"
+                "file = ln.add(ln.File(\"s3://lamindb-ci/lndb-storage/pbmc68k.zarr\"))\n",
+                "print(file.backed().obs.head())\n",
+                "adata_subset = file.stream(subset_obs=subset_obs)\n",
+                "adata_subset.obs.cell_type.value_counts()"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -220,23 +186,28 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.12"
+            "version": "3.9.15"
         },
         "nbproject": {
-            "id": "uBQMCcdYwEjA",
+            "id": "YVUCtH4GfQOy",
             "parent": null,
             "pypackage": null,
-            "time_init": "2023-04-04T16:26:17.675023+00:00",
-            "user_handle": "Koncopd",
-            "user_id": "qTQ5q0ar",
-            "user_name": "Sergei Rybakov",
+            "time_init": "2023-01-23T08:28:32.097943+00:00",
+            "user_handle": "testuser1",
+            "user_id": "DzTjkKse",
+            "user_name": "Test User1",
             "version": "0"
+        },
+        "vscode": {
+            "interpreter": {
+                "hash": "ae1fefc8646a06dd2e75004cd934adda7c5727b046986a772e3b44b0ffba9754"
+            }
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 5
+    "nbformat_minor": 4
 }
```

### Comparing `lndb_storage-0.2rc5/docs/guide/iris.csv` & `lndb_storage-0.2rc6/docs/guide/iris.csv`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc5/docs/guide/iris.data` & `lndb_storage-0.2rc6/docs/guide/iris.data`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc5/docs/guide/serialize-cache.ipynb` & `lndb_storage-0.2rc6/docs/guide/serialize-cache.ipynb`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc5/docs/guide/stream.ipynb` & `lndb_storage-0.2rc6/docs/guide/upload.ipynb`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7862165178571429%*

 * *Differences: {"'cells'": "{0: {'source': ['# Upload files'], 'id': 'dd6bf8d1-ba40-4054-9f62-a402588f7a95'}, 1: "*

 * *            "{'source': ['!lamin login testuser1\\n', '!lamin load testuser1/lndb-storage\\n', "*

 * *            "'!lamin delete lndb-storage\\n', '!lamin init --storage s3://lamindb-ci --name "*

 * *            "lndb-storage'], 'id': '8c21d20e-0f4e-4097-a37a-ba784addc412'}, 2: {'source': {insert: "*

 * *            "[(0, 'import lamindb as ln\\n'), (1, 'import pytest\\n'), (2, '\\n')]}, 'id': "*

 * *            "'8eb097f4-4114 […]*

```diff
@@ -1,303 +1,322 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
+            "id": "dd6bf8d1-ba40-4054-9f62-a402588f7a95",
             "metadata": {},
             "source": [
-                "# Streaming of annotated data matrices from the cloud"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "When working with large datasets, it is often inefficient to load entire datasets into memory.\n",
-                "\n",
-                "Here, we walk through partial streaming."
+                "# Upload files"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "8c21d20e-0f4e-4097-a37a-ba784addc412",
             "metadata": {},
             "outputs": [],
             "source": [
-                "import lamindb as ln"
+                "!lamin login testuser1\n",
+                "!lamin load testuser1/lndb-storage\n",
+                "!lamin delete lndb-storage\n",
+                "!lamin init --storage s3://lamindb-ci --name lndb-storage"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "8eb097f4-4114-4a35-8764-ebcfe1e85bdc",
             "metadata": {},
             "outputs": [],
             "source": [
+                "import lamindb as ln\n",
+                "import pytest\n",
+                "\n",
                 "ln.track()"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "b11215af-bb7f-4932-83ee-8f46f5583ed8",
             "metadata": {},
             "source": [
-                "## Prepare files"
+                "Some test data."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "077344a2-4f18-47c9-b8a5-c3c6411511db",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "pbmc68k = ln.dev.datasets.anndata_pbmc68k_reduced()"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "tags": []
-            },
+            "id": "7af3d05d-8dc3-455d-be1b-83e798621051",
+            "metadata": {},
             "source": [
-                "We already have data in the cloud:"
+                "Subset to a mini file to speed up the run time of this notebook:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "614a8766-b594-4578-a163-2497835cc9b4",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pbmc68k_h5ad = ln.File(\"s3://lamindb-ci/lndb-storage/pbmc68k.h5ad\")"
+                "pbmc68k = pbmc68k[:5, :5].copy()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "4234bb42-03e2-4676-a674-9281eb295df7",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pbmc68k_h5ad = ln.add(pbmc68k_h5ad)"
+                "pbmc68k"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "622b8012-6a94-4a41-8a6b-4c178ed4cfa6",
+            "metadata": {},
+            "source": [
+                "## Upload from memory using explicit semantic `key`"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "8138a887-2de8-4ad9-ad8b-63324263fb7d",
             "metadata": {},
             "source": [
-                "Alternatively, you can save as zarr:"
+                "### Upload h5ad"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "fcff7272-13df-46f9-ab63-25921a507f98",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pbmc68k_zarr = ln.File(\"s3://lamindb-ci/lndb-storage/pbmc68k.zarr\")"
+                "pbmc68k_h5ad = ln.File(pbmc68k, key=\"test-upload/pbmc68k.h5ad\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "a97617fd-0f41-43f1-9919-25acab3df0c5",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pbmc68k_zarr = ln.add(pbmc68k_zarr)"
+                "pbmc68k_h5ad = ln.add(pbmc68k_h5ad)"
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "14b139c3-fb1e-4cca-a75a-8ed798c189a8",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "## Caching vs streaming entire files"
+                "ln.delete(pbmc68k_h5ad, delete_data_from_storage=True)"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "ff0e34cd-8ebd-4196-a7bd-a667b2a360a1",
             "metadata": {},
             "source": [
-                "Load h5ad (a local file is cached):"
+                "### Upload zarr"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "b66ec0af-9c93-438a-8280-d93fe657bbfb",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pbmc68k_h5ad.load()"
+                "# pbmc68k_zarr = ln.File(pbmc68k, key=\"test-upload/pbmc68k.zarr\", format=\"zarr\")"
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "7da05e34-ee3c-420e-abd3-96adfae8d3d0",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "Load zarr (no caching happens here, data is streamed):"
+                "# pbmc68k_zarr = ln.add(pbmc68k_zarr)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "0e293606-f47f-4da6-9beb-433eea607309",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pbmc68k_zarr.load()"
+                "# ln.delete(pbmc68k_zarr, delete_data_from_storage=True)"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "c552af90-b4b3-4465-aaec-662949d480b3",
             "metadata": {},
             "source": [
-                "## Stream files partially"
+                "## Upload using `id` with implicit `key`"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "6ac16f8b-3952-469b-9b6c-3a78c096467c",
             "metadata": {},
             "source": [
-                "We saw that both datasets have `cell_type`: Dendritic cells, CD14+ Monocytes.\n",
-                "\n",
-                "Now let's only fetch data that are labeled as these two cell types."
+                "### Upload h5ad"
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "25675eeb-b339-44c7-9118-6178b3351100",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "First we obtain the ingested AnnData Files by querying the LaminDB instance.\n",
-                "\n",
-                "```{note}\n",
-                "\n",
-                "This is merely a database query, it does **not** download the data.\n",
-                "\n",
-                "```"
+                "pbmc68k_h5ad = ln.File(pbmc68k, name=\"pbmc68k.h5ad\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "6314e8b1-ccf3-467f-a6e0-4687f52d1033",
             "metadata": {},
             "outputs": [],
             "source": [
-                "file = ln.select(ln.File, run_id=ln.context.run.id, suffix=\".h5ad\").one()"
+                "pbmc68k_h5ad = ln.add(pbmc68k_h5ad)"
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "07e8e616-89df-433d-89a7-a9c8aed890ce",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "Next, we prepare the query strings to query the columns of `.obs` for each `AnnData` object. For details see the [pandas docs](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.query.html).\n",
-                "\n",
-                "```{note}\n",
-                "\n",
-                "Soon, we'll integrate the within-object queries with the SQL queries.\n",
-                "\n",
-                "```"
+                "ln.delete(pbmc68k_h5ad, delete_data_from_storage=True)"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "8bd5da59-c616-4e49-9f02-f4814c19032f",
             "metadata": {},
             "source": [
-                "### (A) Pandas-style query strings"
+                "### Upload zarr"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "2e6e3ae0-5ba9-4312-a902-f0278d1efdfc",
             "metadata": {},
             "outputs": [],
             "source": [
-                "query_string = \"cell_type == 'Dendritic cells' | cell_type == 'CD14+ Monocytes'\""
+                "# pbmc68k_zarr = ln.File(pbmc68k, name=\"pbmc68k.zarr\", format=\"zarr\")"
             ]
         },
         {
-            "cell_type": "markdown",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "e6f94b58-c301-4663-ac83-f60cdc9d3fed",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "Subset the `AnnData` objects based on the query strings above and load them directly into memory.\n",
-                "\n",
-                "```{note}\n",
-                "\n",
-                "No caching happens here!\n",
-                "\n",
-                "When `ln.subset` is executed, only the `.obs` columns are loaded to perform the subset. For all remaining, **only the subsets** data are loaded into memory.\n",
-                "\n",
-                "```"
+                "# pbmc68k_zarr = ln.add(pbmc68k_zarr)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "52d1336f-1e76-4eb9-93e6-1eab5333f7f4",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.subset(file, query_obs=query_string)"
+                "# ln.delete(pbmc68k_zarr, delete_data_from_storage=True)"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {},
+            "id": "06a91d99-d204-4ec2-b567-960a2aaad38d",
+            "metadata": {
+                "tags": []
+            },
             "source": [
-                "```{tip}\n",
-                "\n",
-                "Set `use_concat=True` to return a single concatenated AnnData object (runs [`anndata.concat`](https://anndata.readthedocs.io/en/latest/generated/anndata.concat.html) under the hood).\n",
-                "\n",
-                "See an example in (B) Lazy query expressions\n",
-                "```"
+                "## Error behavior"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "e5aa762a-491e-49c8-a372-8c80f019ea73",
             "metadata": {},
             "source": [
-                "### (B) Lazy query expressions"
+                "### Inexistent path"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "f760cba0-38a0-4be2-8854-d1f17689de05",
             "metadata": {},
             "source": [
-                "Lazy selectors for convenient subsetting with complicated conditions.\n",
-                "\n",
-                "Operators, methods and numpy functions are supported."
+                "Specified bucket does not exist."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "de2f9c7b-994c-417a-a700-f517a29df78e",
             "metadata": {},
             "outputs": [],
             "source": [
-                "query_string = ln.lazy.cell_type.isin((\"Dendritic cells\", \"CD14+ Monocytes\")) & (\n",
-                "    ln.lazy.percent_mito <= 0.05\n",
-                ")"
+                "with pytest.raises(FileNotFoundError):\n",
+                "    pbmc68k_h5ad = ln.File(\"s3://inexistent-bucket-239809834/pbmc68k.h5ad\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "13850c8c-6543-4cf4-b8ae-dc0a00300e2f",
             "metadata": {},
             "outputs": [],
             "source": [
-                "adata = ln.subset(file, query_obs=query_string, use_concat=True)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "adata"
+                "with pytest.raises(FileNotFoundError):\n",
+                "    pbmc68k_h5ad = ln.File(\"s3://lndb-setup-ci/pbmc68k.h5ad\")"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "bcb399bd-8c13-424a-bbb7-d6bb7cb1f5e7",
             "metadata": {},
             "source": [
-                "Let's now check whether the returned AnnData only contains queried categories:"
+                "Cross bucket moving of files."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "af74523c-553b-4a25-90db-9d820006dfc1",
             "metadata": {},
             "outputs": [],
             "source": [
-                "adata.obs[\"cell_type\"].value_counts()"
+                "with pytest.raises(ValueError):\n",
+                "    pbmc68k_h5ad = ln.File(\"s3://bionty-assets/Species.csv\")"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -312,25 +331,20 @@
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
             "version": "3.9.15"
         },
         "nbproject": {
-            "id": "YVUCtH4GfQOy",
+            "id": "psZgub4FOmzS",
             "parent": null,
             "pypackage": null,
-            "time_init": "2023-01-23T08:28:32.097943+00:00",
+            "time_init": "2023-04-09T20:01:57.780053+00:00",
             "user_handle": "testuser1",
             "user_id": "DzTjkKse",
             "user_name": "Test User1",
             "version": "0"
-        },
-        "vscode": {
-            "interpreter": {
-                "hash": "ae1fefc8646a06dd2e75004cd934adda7c5727b046986a772e3b44b0ffba9754"
-            }
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 4
+    "nbformat_minor": 5
 }
```

### Comparing `lndb_storage-0.2rc5/lndb_storage/__init__.py` & `lndb_storage-0.2rc6/lndb_storage/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
    :toctree: .
 
    store_object
    store_png
    delete_storage
 """
 
-__version__ = "0.2rc5"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.2rc6"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 from lndb.dev.upath import UPath
 from lndb.dev.upath import infer_filesystem as _infer_filesystem
 
 from ._file import delete_storage, load_to_memory, store_object
 from ._h5ad import h5ad_to_anndata
 from ._images import store_png
```

### Comparing `lndb_storage-0.2rc5/lndb_storage/_file.py` & `lndb_storage-0.2rc6/lndb_storage/_file.py`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc5/lndb_storage/_subset.py` & `lndb_storage-0.2rc6/lndb_storage/_subset.py`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc5/lndb_storage/_zarr.py` & `lndb_storage-0.2rc6/lndb_storage/_zarr.py`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc5/lndb_storage/object/_anndata.py` & `lndb_storage-0.2rc6/lndb_storage/object/_anndata.py`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc5/lndb_storage/object/_anndata_sizes.py` & `lndb_storage-0.2rc6/lndb_storage/object/_anndata_sizes.py`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc5/lndb_storage/object/_core.py` & `lndb_storage-0.2rc6/lndb_storage/object/_core.py`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc5/lndb_storage/object/_lazy_field.py` & `lndb_storage-0.2rc6/lndb_storage/object/_lazy_field.py`

 * *Files identical despite different names*

### Comparing `lndb_storage-0.2rc5/lndb_storage/object/_subset_anndata.py` & `lndb_storage-0.2rc6/lndb_storage/object/_subset_anndata.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-from typing import Optional, Union
+from functools import cached_property
+from typing import Literal, Optional, Union
 
 import h5py
+import pandas as pd
 import zarr
 from anndata import AnnData
 from anndata._io.specs.methods import _read_partial
 from anndata._io.specs.registry import read_elem, read_elem_partial
 from lndb.dev.upath import infer_filesystem as _infer_filesystem
 from lnschema_core import File
 from lnschema_core.dev._storage import filepath_from_file
@@ -92,7 +94,47 @@
             adata = _subset_adata_storage(storage, query_obs, query_var)
     elif file.suffix == ".zarr":
         mapper = fs.get_mapper(file_path_str, check=True)
         storage = zarr.open(mapper, mode="r")
         adata = _subset_adata_storage(storage, query_obs, query_var)
 
     return adata
+
+
+def get_obs_var_storage(
+    storage: Union[zarr.Group, h5py.File], which=Literal["obs", "var"]
+) -> pd.DataFrame:
+    with storage as access:
+        result = read_elem(access[which])
+    if isinstance(result, pd.DataFrame):
+        return result
+    # is array
+    elif "index" in result.dtype.fields:
+        return pd.DataFrame.from_records(result, index="index")
+    else:
+        return pd.DataFrame.from_records(result)
+
+
+class CloudAnnData:
+    def __init__(self, file: File):
+        self._file = file
+
+    def _get_obs_var(self, which=Literal["obs", "var"]) -> pd.DataFrame:
+        file_path = filepath_from_file(self._file)
+        fs, file_path_str = _infer_filesystem(file_path)
+        if self._file.suffix == ".h5ad":
+            with fs.open(file_path_str, mode="rb") as f:
+                storage = h5py.File(f, mode="r")
+                df = get_obs_var_storage(storage, which)
+        elif self._file.suffix == ".zarr" or self._file.suffix == ".zrad":
+            mapper = fs.get_mapper(file_path_str, check=True)
+            storage = zarr.open(mapper, mode="r")
+            df = get_obs_var_storage(storage, which)
+        return df
+
+    @cached_property
+    def obs(self) -> pd.DataFrame:
+        return self._get_obs_var(which="obs")
+
+    @cached_property
+    def var(self) -> pd.DataFrame:
+        return self._get_obs_var(which="var")
```

### Comparing `lndb_storage-0.2rc5/noxfile.py` & `lndb_storage-0.2rc6/noxfile.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import nox
 import requests  # type: ignore
-from laminci import move_built_docs_to_docs_slash_project_slug, upload_docs_dir
+from laminci import move_built_docs_to_docs_slash_project_slug, upload_docs_artifact
 from laminci.nox import build_docs, login_testuser1, run_pre_commit, run_pytest
 
 nox.options.reuse_existing_virtualenvs = True
 
 
 @nox.session(python=["3.7", "3.8", "3.9", "3.10", "3.11"])
 def lint(session: nox.Session) -> None:
     run_pre_commit(session)
 
 
 @nox.session(python=["3.7", "3.8", "3.9", "3.10", "3.11"])
 def build(session):
     login_testuser1(session)
     session.install(".[dev,test]")
-    response = requests.get("https://github.com/laminlabs/lamindb/tree/staging")
+    response = requests.get("https://github.com/laminlabs/lamindb/tree/cloud")
     if response.status_code < 400:
-        session.install("git+https://github.com/laminlabs/lamindb@staging")
+        session.install("git+https://github.com/laminlabs/lamindb@cloud")
     else:
         session.install("git+https://github.com/laminlabs/lamindb")
     run_pytest(session)
     build_docs(session)
-    upload_docs_dir()
+    upload_docs_artifact()
     move_built_docs_to_docs_slash_project_slug()
```

### Comparing `lndb_storage-0.2rc5/pyproject.toml` & `lndb_storage-0.2rc6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 dependencies = [
     "lnschema_core",
     "lndb>=0.41.0",
     "lamin_logger>=0.3.0",
     "nbproject",
     "readfcs",
     "python-dateutil",
-    "anndata",
     "zarr",
+    "anndata>=0.9.1",
     "boto3==1.24.59", # for aiobotocore inside s3fs, to fix deps resolution
     "botocore==1.27.59", # for aiobotocore inside s3fs, to fix deps resolution
     "fsspec==2023.1.0",
     "s3fs==2023.1.0",
     "gcsfs==2023.1.0",
     "universal_pathlib",
     "scipy",
@@ -35,14 +35,15 @@
     "pre-commit",
     "nox",
 ]
 test = [
     "pytest>=6.0",
     "pytest-cov",
     "scanpy",
+    "pyarrow",
     "lndb>=0.41rc1",
 ]
 
 [tool.black]
 preview = true
 
 [tool.pytest.ini_options]
```

### Comparing `lndb_storage-0.2rc5/PKG-INFO` & `lndb_storage-0.2rc6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: lndb_storage
-Version: 0.2rc5
+Version: 0.2rc6
 Summary: Storage → object.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnschema_core
 Requires-Dist: lndb>=0.41.0
 Requires-Dist: lamin_logger>=0.3.0
 Requires-Dist: nbproject
 Requires-Dist: readfcs
 Requires-Dist: python-dateutil
-Requires-Dist: anndata
 Requires-Dist: zarr
+Requires-Dist: anndata>=0.9.1
 Requires-Dist: boto3==1.24.59
 Requires-Dist: botocore==1.27.59
 Requires-Dist: fsspec==2023.1.0
 Requires-Dist: s3fs==2023.1.0
 Requires-Dist: gcsfs==2023.1.0
 Requires-Dist: universal_pathlib
 Requires-Dist: scipy
 Requires-Dist: pandas
 Requires-Dist: typeguard
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: nox ; extra == "dev"
 Requires-Dist: pytest>=6.0 ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: scanpy ; extra == "test"
+Requires-Dist: pyarrow ; extra == "test"
 Requires-Dist: lndb>=0.41rc1 ; extra == "test"
 Project-URL: Home, https://github.com/laminlabs/lndb-storage
 Provides-Extra: dev
 Provides-Extra: test
 
 # lndb-storage: LaminDB storage
```


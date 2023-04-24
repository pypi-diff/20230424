# Comparing `tmp/types-dj-database-url-1.3.0.0.tar.gz` & `tmp/types-dj-database-url-1.3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-dj-database-url-1.3.0.0.tar", last modified: Thu Mar 30 21:12:53 2023, max compression
+gzip compressed data, was "types-dj-database-url-1.3.0.1.tar", last modified: Mon Apr 24 12:30:06 2023, max compression
```

## Comparing `types-dj-database-url-1.3.0.0.tar` & `types-dj-database-url-1.3.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:12:53.165380 types-dj-database-url-1.3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-03-30 21:12:52.000000 types-dj-database-url-1.3.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-30 21:12:52.000000 types-dj-database-url-1.3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-03-30 21:12:53.165380 types-dj-database-url-1.3.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:12:53.165380 types-dj-database-url-1.3.0.0/dj_database_url-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-30 21:12:52.000000 types-dj-database-url-1.3.0.0/dj_database_url-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-03-30 21:12:52.000000 types-dj-database-url-1.3.0.0/dj_database_url-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 21:12:53.165380 types-dj-database-url-1.3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-03-30 21:12:52.000000 types-dj-database-url-1.3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 21:12:53.165380 types-dj-database-url-1.3.0.0/types_dj_database_url.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-03-30 21:12:53.000000 types-dj-database-url-1.3.0.0/types_dj_database_url.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-30 21:12:53.000000 types-dj-database-url-1.3.0.0/types_dj_database_url.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 21:12:53.000000 types-dj-database-url-1.3.0.0/types_dj_database_url.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-30 21:12:53.000000 types-dj-database-url-1.3.0.0/types_dj_database_url.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:30:06.109406 types-dj-database-url-1.3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-24 12:30:05.000000 types-dj-database-url-1.3.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-24 12:30:05.000000 types-dj-database-url-1.3.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-24 12:30:06.109406 types-dj-database-url-1.3.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:30:06.109406 types-dj-database-url-1.3.0.1/dj_database_url-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-24 12:30:05.000000 types-dj-database-url-1.3.0.1/dj_database_url-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-24 12:30:05.000000 types-dj-database-url-1.3.0.1/dj_database_url-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 12:30:06.109406 types-dj-database-url-1.3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-24 12:30:05.000000 types-dj-database-url-1.3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 12:30:06.109406 types-dj-database-url-1.3.0.1/types_dj_database_url.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-24 12:30:06.000000 types-dj-database-url-1.3.0.1/types_dj_database_url.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-24 12:30:06.000000 types-dj-database-url-1.3.0.1/types_dj_database_url.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 12:30:06.000000 types-dj-database-url-1.3.0.1/types_dj_database_url.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-24 12:30:06.000000 types-dj-database-url-1.3.0.1/types_dj_database_url.egg-info/top_level.txt
```

### Comparing `types-dj-database-url-1.3.0.0/CHANGELOG.md` & `types-dj-database-url-1.3.0.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 1.3.0.1 (2023-04-24)
+
+[dj-database-url] Fix CONN_MAX_AGE and conn_max_age types (#10075)
+
 ## 1.3.0.0 (2023-03-30)
 
 Bump dj-database-url to 1.3.* (#9975)
 
 Release: https://pypi.org/pypi/dj-database-url/1.3.0
 Homepage: https://github.com/jazzband/dj-database-url
 Diff: https://github.com/jazzband/dj-database-url/compare/v1.2.0...v1.3.0
```

### Comparing `types-dj-database-url-1.3.0.0/PKG-INFO` & `types-dj-database-url-1.3.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-dj-database-url
-Version: 1.3.0.0
+Version: 1.3.0.1
 Summary: Typing stubs for dj-database-url
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/dj-database-url.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `dj-database-url`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/dj-database-url. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `a06bf1fe1d0c95d431913c0276bf3615cb5b2561`.
+This package was generated from typeshed commit `22ced496450a29ecae2cc4f7d5d163185ca6a75f`.
```

### Comparing `types-dj-database-url-1.3.0.0/dj_database_url-stubs/__init__.pyi` & `types-dj-database-url-1.3.0.1/dj_database_url-stubs/__init__.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 DEFAULT_ENV: str
 SCHEMES: dict[str, str]
 
 # From https://docs.djangoproject.com/en/4.0/ref/settings/#databases
 class DBConfig(TypedDict, total=False):
     ATOMIC_REQUESTS: bool
     AUTOCOMMIT: bool
-    CONN_MAX_AGE: int
+    CONN_MAX_AGE: int | None
     DISABLE_SERVER_SIDE_CURSORS: bool
     ENGINE: str
     HOST: str
     NAME: str
     OPTIONS: dict[str, Any] | None
     PASSWORD: str
     PORT: str
@@ -29,12 +29,12 @@
     ssl_require: bool = ...,
     test_options: dict[Incomplete, Incomplete] | None = ...,
 ) -> DBConfig: ...
 def config(
     env: str = ...,
     default: str | None = ...,
     engine: str | None = ...,
-    conn_max_age: int = ...,
+    conn_max_age: int | None = ...,
     conn_health_checks: bool = ...,
     ssl_require: bool = ...,
     test_options: dict[Incomplete, Incomplete] | None = ...,
 ) -> DBConfig: ...
```

### Comparing `types-dj-database-url-1.3.0.0/setup.py` & `types-dj-database-url-1.3.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `dj-database-url`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/dj-database-url. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `a06bf1fe1d0c95d431913c0276bf3615cb5b2561`.
+This package was generated from typeshed commit `22ced496450a29ecae2cc4f7d5d163185ca6a75f`.
 '''.lstrip()
 
 setup(name=name,
-      version="1.3.0.0",
+      version="1.3.0.1",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/dj-database-url.md",
```

### Comparing `types-dj-database-url-1.3.0.0/types_dj_database_url.egg-info/PKG-INFO` & `types-dj-database-url-1.3.0.1/types_dj_database_url.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-dj-database-url
-Version: 1.3.0.0
+Version: 1.3.0.1
 Summary: Typing stubs for dj-database-url
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/dj-database-url.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `dj-database-url`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/dj-database-url. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `a06bf1fe1d0c95d431913c0276bf3615cb5b2561`.
+This package was generated from typeshed commit `22ced496450a29ecae2cc4f7d5d163185ca6a75f`.
```


# Comparing `tmp/dbt_firebolt-1.4.1.tar.gz` & `tmp/dbt_firebolt-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/dbt-firebolt/dbt-firebolt/dist/.tmp-8orlw96t/dbt_firebolt-1.4.1.tar", last modified: Thu Apr  6 12:58:32 2023, max compression
+gzip compressed data, was "/home/runner/work/dbt-firebolt/dbt-firebolt/dist/.tmp-xcyajm_u/dbt_firebolt-1.4.2.tar", last modified: Mon Apr 24 10:28:09 2023, max compression
```

## Comparing `dbt_firebolt-1.4.1.tar` & `dbt_firebolt-1.4.2.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 12:58:32.000000 dbt_firebolt-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-04-06 12:58:32.000000 dbt_firebolt-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 12:58:32.000000 dbt_firebolt-1.4.1/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 12:58:32.000000 dbt_firebolt-1.4.1/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 12:58:32.000000 dbt_firebolt-1.4.1/dbt/adapters/firebolt/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-06 12:58:22.000000 dbt_firebolt-1.4.1/dbt/adapters/firebolt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/dbt/adapters/firebolt/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/dbt/adapters/firebolt/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/dbt/adapters/firebolt/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    13013 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/dbt/adapters/firebolt/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/dbt/adapters/firebolt/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 12:58:32.000000 dbt_firebolt-1.4.1/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 12:58:32.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 12:58:32.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 12:58:32.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 12:58:32.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/macros/dbt_external_tables/
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/macros/dbt_external_tables/create_external_table.sql
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/macros/dbt_external_tables/dropif.sql
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/macros/dbt_external_tables/get_external_build_plan.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 12:58:32.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 12:58:32.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/macros/materializations/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 12:58:32.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/macros/materializations/models/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/macros/materializations/models/incremental/column_helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/macros/materializations/models/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/macros/materializations/models/incremental/is_incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/macros/materializations/models/incremental/on_schema_change.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/macros/materializations/models/incremental/strategies.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/macros/materializations/test.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/macros/materializations/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 12:58:32.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/macros/utils/except.sql
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/macros/utils/intersect.sql
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/macros/utils/position.sql
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/dbt/include/firebolt/macros/utils/timestamps.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 12:58:32.000000 dbt_firebolt-1.4.1/dbt_firebolt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-04-06 12:58:32.000000 dbt_firebolt-1.4.1/dbt_firebolt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-06 12:58:32.000000 dbt_firebolt-1.4.1/dbt_firebolt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 12:58:32.000000 dbt_firebolt-1.4.1/dbt_firebolt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-06 12:58:32.000000 dbt_firebolt-1.4.1/dbt_firebolt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-06 12:58:32.000000 dbt_firebolt-1.4.1/dbt_firebolt.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      472 2023-04-06 12:58:08.000000 dbt_firebolt-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-06 12:58:32.000000 dbt_firebolt-1.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/dbt/adapters/firebolt/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-24 10:27:59.000000 dbt_firebolt-1.4.2/dbt/adapters/firebolt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/adapters/firebolt/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/adapters/firebolt/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/adapters/firebolt/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13013 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/adapters/firebolt/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/adapters/firebolt/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/dbt_external_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/dbt_external_tables/create_external_table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/dbt_external_tables/dropif.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/dbt_external_tables/get_external_build_plan.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/models/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/models/incremental/column_helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/models/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/models/incremental/is_incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/models/incremental/merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/models/incremental/on_schema_change.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/models/incremental/strategies.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/test.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/utils/except.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/utils/intersect.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/utils/position.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/dbt/include/firebolt/macros/utils/timestamps.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/dbt_firebolt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/dbt_firebolt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/dbt_firebolt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/dbt_firebolt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/dbt_firebolt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/dbt_firebolt.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      472 2023-04-24 10:27:45.000000 dbt_firebolt-1.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-24 10:28:09.000000 dbt_firebolt-1.4.2/setup.cfg
```

### Comparing `dbt_firebolt-1.4.1/LICENSE` & `dbt_firebolt-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.1/PKG-INFO` & `dbt_firebolt-1.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt_firebolt
-Version: 1.4.1
+Version: 1.4.2
 Summary: The Firebolt adapter plugin for dbt (data build tool)
 Home-page: https://github.com/firebolt-db/dbt-firebolt
 Author: Firebolt
 Author-email: support@firebolt.io
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/firebolt-db/dbt-firebolt/issues
 Classifier: License :: OSI Approved :: Apache Software License
@@ -61,14 +61,15 @@
 | Feature                      | Supported          |
 |------------------------------|--------------------|
 | Table materializations       | :white_check_mark: |
 | Ephemeral materializations   | :white_check_mark: |
 | View materializations        | :white_check_mark: |
 | Incremental materializations - append | :white_check_mark: |
 | Incremental materializations - insert_overwrite | :white_check_mark: |
+| Incremental materializations - delete+insert | :white_check_mark: |
 | Incremental materializations - merge | :x: |
 | Snapshots                    | :x: |
 | Seeds                        | :white_check_mark: |
 | Tests                        | :white_check_mark: |
 | Documentation                | :white_check_mark: |
 | Custom schemas               | :x: (see [workaround](https://docs.getdbt.com/reference/warehouse-profiles/firebolt-profile#supporting-concurrent-development)) |
 | Custom databases             | :x: |
```

### Comparing `dbt_firebolt-1.4.1/README.md` & `dbt_firebolt-1.4.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 | Feature                      | Supported          |
 |------------------------------|--------------------|
 | Table materializations       | :white_check_mark: |
 | Ephemeral materializations   | :white_check_mark: |
 | View materializations        | :white_check_mark: |
 | Incremental materializations - append | :white_check_mark: |
 | Incremental materializations - insert_overwrite | :white_check_mark: |
+| Incremental materializations - delete+insert | :white_check_mark: |
 | Incremental materializations - merge | :x: |
 | Snapshots                    | :x: |
 | Seeds                        | :white_check_mark: |
 | Tests                        | :white_check_mark: |
 | Documentation                | :white_check_mark: |
 | Custom schemas               | :x: (see [workaround](https://docs.getdbt.com/reference/warehouse-profiles/firebolt-profile#supporting-concurrent-development)) |
 | Custom databases             | :x: |
```

### Comparing `dbt_firebolt-1.4.1/dbt/adapters/firebolt/column.py` & `dbt_firebolt-1.4.2/dbt/adapters/firebolt/column.py`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.1/dbt/adapters/firebolt/connections.py` & `dbt_firebolt-1.4.2/dbt/adapters/firebolt/connections.py`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.1/dbt/adapters/firebolt/impl.py` & `dbt_firebolt-1.4.2/dbt/adapters/firebolt/impl.py`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.1/dbt/adapters/firebolt/relation.py` & `dbt_firebolt-1.4.2/dbt/adapters/firebolt/relation.py`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.1/dbt/include/firebolt/macros/adapters/apply_grants.sql` & `dbt_firebolt-1.4.2/dbt/include/firebolt/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.1/dbt/include/firebolt/macros/adapters/relation.sql` & `dbt_firebolt-1.4.2/dbt/include/firebolt/macros/adapters/relation.sql`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.1/dbt/include/firebolt/macros/adapters.sql` & `dbt_firebolt-1.4.2/dbt/include/firebolt/macros/adapters.sql`

 * *Files 1% similar despite different names*

```diff
@@ -23,18 +23,14 @@
   {%- endfor %}
 {% endmacro %}
 
 
 {% macro firebolt__list_schemas(database) %}
   {# Return current schema. Name is a misnomer.
      TODO: Should this actually return all schemas? #}
-  {% if target.threads > 1 %}
-    {{ exceptions.raise_compiler_error("Firebolt does not currently support "
-                                       "more than one thread.") }}
-  {% endif %}
   {% call statement('list_schemas', fetch_result=True, auto_begin=False) %}
 
       SELECT 'public' AS schema
   {% endcall %}
   {{ return(load_result('list_schemas').table) }}
 {% endmacro %}
 
@@ -144,15 +140,15 @@
   {#-
   Return column information for table identified by relation as
   List[FireboltColumn].
     Args: relation: dbt Relation
   -#}
   {% set sql %}
     SELECT column_name, data_type from information_schema.columns
-    WHERE table_name = '{{ relation }}'
+    WHERE table_name = '{{ relation.identifier }}'
   {% endset %}
   {%- set result = run_query(sql) -%}
   {% set columns = [] %}
   {% for row in result %}
     {% do columns.append(adapter.get_column_class().from_description(row['column_name'],
                          adapter.resolve_special_columns(row['data_type']))) %}
   {% endfor %}
```

### Comparing `dbt_firebolt-1.4.1/dbt/include/firebolt/macros/catalog.sql` & `dbt_firebolt-1.4.2/dbt/include/firebolt/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.1/dbt/include/firebolt/macros/dbt_external_tables/create_external_table.sql` & `dbt_firebolt-1.4.2/dbt/include/firebolt/macros/dbt_external_tables/create_external_table.sql`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.1/dbt/include/firebolt/macros/dbt_external_tables/get_external_build_plan.sql` & `dbt_firebolt-1.4.2/dbt/include/firebolt/macros/dbt_external_tables/get_external_build_plan.sql`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.1/dbt/include/firebolt/macros/materializations/models/incremental/column_helpers.sql` & `dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/models/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.1/dbt/include/firebolt/macros/materializations/models/incremental/incremental.sql` & `dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/models/incremental/incremental.sql`

 * *Files 4% similar despite different names*

```diff
@@ -34,17 +34,15 @@
   Note that all new relations must first be instantiated as BaseRelation objects,
   and that those objects are used to create and query actual relations in the DB.
   Care must be taken to correctly define each BaseRelation as either a view or
   a table, lest subsequent operations on the relations (be the they objects or
   the DB tables the objects abstract) fail.
   #}
 
-  {# Not yet used
-    {% set unique_key = config.get('unique_key') %}
-  #}
+  {% set unique_key = config.get('unique_key') %}
 
   {% set grant_config = config.get('grants') %}
 
   {%- set strategy = config.get('incremental_strategy') -%}
   {%- if is_incremental() and strategy is none -%}
     {{ log('Model %s is set to incremental, but no incremental strategy is set. '
            'Defaulting to append' % this, True) }}
@@ -97,19 +95,21 @@
     {%- else -%}
       {%- do run_query(create_table_as(True, new_records, sql)) -%}
     {%- endif -%}
     {# All errors involving schema changes are dealt with in `process_schema_changes`. #}
     {%- set dest_columns = process_schema_changes(on_schema_change,
                                                   new_records,
                                                   existing) -%}
+    {%- set incremental_predicates = config.get('predicates', none) or config.get('incremental_predicates', none) -%}
     {%- set build_sql = get_incremental_sql(strategy,
                                             new_records,
                                             target,
                                             unique_key,
-                                            dest_columns) -%}
+                                            dest_columns,
+                                            incremental_predicates) -%}
   {%- endif -%}
   {%- call statement("main") -%}
     {{ build_sql }}
   {%- endcall -%}
 
   {% set should_revoke = should_revoke(existing_relation, full_refresh_mode) %}
   {% do apply_grants(target_relation, grant_config, should_revoke) %}
```

### Comparing `dbt_firebolt-1.4.1/dbt/include/firebolt/macros/materializations/models/incremental/is_incremental.sql` & `dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/models/incremental/is_incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.1/dbt/include/firebolt/macros/materializations/models/incremental/on_schema_change.sql` & `dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/models/incremental/on_schema_change.sql`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.1/dbt/include/firebolt/macros/materializations/models/incremental/strategies.sql` & `dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/models/incremental/strategies.sql`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% macro get_incremental_sql(strategy, source, target, unique_key, dest_columns) %}
+{% macro get_incremental_sql(strategy, source, target, unique_key, dest_columns, incremental_predicates) %}
   {#
   Retrieve appropriate SQL for whichever incremental strategy is given.
   Args:
     strategy: string, which incremental strategy is in to be used.
     source: string, table from which queried results will be taken.
     target: string, table into which results will be inserted.
     unique_key: string, only as a placeholder for future use
@@ -13,14 +13,16 @@
     {#- Only insert new records into existing table, relying on user to manage
        merges. -#}
     {{ get_insert_only_sql(source, target, dest_columns) }}
   {%- elif strategy == 'insert_overwrite' -%}
     {#- Insert new data. If any data is duplicate, drop partition containing
        previous data and insert new. -#}
     {{ get_insert_overwrite_sql(source, target, dest_columns) }}
+  {%- elif strategy == 'delete+insert' -%}
+    {% do return(get_delete_insert_merge_sql(target, source, unique_key, dest_columns, incremental_predicates)) %}
   {%- elif strategy is not none -%}
     {% do exceptions.raise_compiler_error('Model %s has incremental strategy %s '
                                           'specified, but that strategy is not '
                                           'supported.' % (target, strategy)) %}
   {% else %}
     {{ exceptions.raise_compiler_error('No incremental strategy was specified '
                                        'for model %s.' % (target)) }}
```

### Comparing `dbt_firebolt-1.4.1/dbt/include/firebolt/macros/materializations/seed.sql` & `dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.1/dbt/include/firebolt/macros/materializations/table.sql` & `dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.1/dbt/include/firebolt/macros/materializations/view.sql` & `dbt_firebolt-1.4.2/dbt/include/firebolt/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.1/dbt/include/firebolt/macros/utils/listagg.sql` & `dbt_firebolt-1.4.2/dbt/include/firebolt/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt_firebolt-1.4.1/dbt_firebolt.egg-info/PKG-INFO` & `dbt_firebolt-1.4.2/dbt_firebolt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-firebolt
-Version: 1.4.1
+Version: 1.4.2
 Summary: The Firebolt adapter plugin for dbt (data build tool)
 Home-page: https://github.com/firebolt-db/dbt-firebolt
 Author: Firebolt
 Author-email: support@firebolt.io
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/firebolt-db/dbt-firebolt/issues
 Classifier: License :: OSI Approved :: Apache Software License
@@ -61,14 +61,15 @@
 | Feature                      | Supported          |
 |------------------------------|--------------------|
 | Table materializations       | :white_check_mark: |
 | Ephemeral materializations   | :white_check_mark: |
 | View materializations        | :white_check_mark: |
 | Incremental materializations - append | :white_check_mark: |
 | Incremental materializations - insert_overwrite | :white_check_mark: |
+| Incremental materializations - delete+insert | :white_check_mark: |
 | Incremental materializations - merge | :x: |
 | Snapshots                    | :x: |
 | Seeds                        | :white_check_mark: |
 | Tests                        | :white_check_mark: |
 | Documentation                | :white_check_mark: |
 | Custom schemas               | :x: (see [workaround](https://docs.getdbt.com/reference/warehouse-profiles/firebolt-profile#supporting-concurrent-development)) |
 | Custom databases             | :x: |
```

### Comparing `dbt_firebolt-1.4.1/dbt_firebolt.egg-info/SOURCES.txt` & `dbt_firebolt-1.4.2/dbt_firebolt.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 ./dbt/include/firebolt/macros/materializations/seed.sql
 ./dbt/include/firebolt/macros/materializations/table.sql
 ./dbt/include/firebolt/macros/materializations/test.sql
 ./dbt/include/firebolt/macros/materializations/view.sql
 ./dbt/include/firebolt/macros/materializations/models/incremental/column_helpers.sql
 ./dbt/include/firebolt/macros/materializations/models/incremental/incremental.sql
 ./dbt/include/firebolt/macros/materializations/models/incremental/is_incremental.sql
+./dbt/include/firebolt/macros/materializations/models/incremental/merge.sql
 ./dbt/include/firebolt/macros/materializations/models/incremental/on_schema_change.sql
 ./dbt/include/firebolt/macros/materializations/models/incremental/strategies.sql
 ./dbt/include/firebolt/macros/utils/array_append.sql
 ./dbt/include/firebolt/macros/utils/array_concat.sql
 ./dbt/include/firebolt/macros/utils/array_construct.sql
 ./dbt/include/firebolt/macros/utils/bool_or.sql
 ./dbt/include/firebolt/macros/utils/cast_bool_to_text.sql
```

### Comparing `dbt_firebolt-1.4.1/setup.cfg` & `dbt_firebolt-1.4.2/setup.cfg`

 * *Files identical despite different names*


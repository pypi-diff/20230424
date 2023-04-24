# Comparing `tmp/th2_data_services-2.0.0.dev4763134463.tar.gz` & `tmp/th2_data_services-2.0.0.dev4783695011.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_data_services-2.0.0.dev4763134463.tar", last modified: Fri Apr 21 08:49:48 2023, max compression
+gzip compressed data, was "dist/th2_data_services-2.0.0.dev4783695011.tar", last modified: Mon Apr 24 07:37:07 2023, max compression
```

## Comparing `th2_data_services-2.0.0.dev4763134463.tar` & `th2_data_services-2.0.0.dev4783695011.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 08:49:48.000000 th2_data_services-2.0.0.dev4763134463/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)   614698 2023-04-21 08:49:48.000000 th2_data_services-2.0.0.dev4763134463/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)   510907 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-04-21 08:49:37.000000 th2_data_services-2.0.0.dev4763134463/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)      262 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-21 08:49:48.000000 th2_data_services-2.0.0.dev4763134463/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 08:49:48.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 08:49:48.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/config/
--rw-r--r--   0 runner    (1001) docker     (122)      660 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/config/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    28646 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 08:49:48.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/event_tree/
--rw-r--r--   0 runner    (1001) docker     (122)      806 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/event_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/event_tree/etc_driver.py
--rw-r--r--   0 runner    (1001) docker     (122)    16045 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/event_tree/event_tree.py
--rw-r--r--   0 runner    (1001) docker     (122)    25893 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/event_tree/event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2497 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/event_tree/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2501 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/event_tree/parent_event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     1680 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 08:49:48.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/interfaces/adapter.py
--rw-r--r--   0 runner    (1001) docker     (122)      956 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/interfaces/command.py
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/interfaces/data_source.py
--rw-r--r--   0 runner    (1001) docker     (122)      706 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/interfaces/source_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      886 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/interfaces/struct.py
--rw-r--r--   0 runner    (1001) docker     (122)     2255 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/interfaces/stub_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 08:49:48.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/interfaces/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/interfaces/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3023 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/interfaces/utils/converter.py
--rw-r--r--   0 runner    (1001) docker     (122)     2705 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/interfaces/utils/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 08:49:48.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      643 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/_types.py
--rw-r--r--   0 runner    (1001) docker     (122)     8635 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/aggregation_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)    15216 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/az_tree.py
--rw-r--r--   0 runner    (1001) docker     (122)      742 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/categorizers.py
--rw-r--r--   0 runner    (1001) docker     (122)      935 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/category.py
--rw-r--r--   0 runner    (1001) docker     (122)     3296 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/converters.py
--rw-r--r--   0 runner    (1001) docker     (122)      908 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/decode_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2604 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/display.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 08:49:48.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/event_utils/
--rw-r--r--   0 runner    (1001) docker     (122)      725 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/event_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11551 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/event_utils/display.py
--rw-r--r--   0 runner    (1001) docker     (122)     7107 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/event_utils/event_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5291 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/event_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (122)    12089 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/event_utils/select.py
--rw-r--r--   0 runner    (1001) docker     (122)     6805 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/event_utils/totals.py
--rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/experimental.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 08:49:48.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/message_utils/
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/message_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1014 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/message_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (122)    14456 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/message_utils/message_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    15739 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     8330 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/perfect_table.py
--rw-r--r--   0 runner    (1001) docker     (122)    33801 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/script_report_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3531 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/sse_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     5285 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (122)     6717 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/total_category_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 08:49:48.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/viewer_structs/
--rw-r--r--   0 runner    (1001) docker     (122)      609 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/viewer_structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6185 2023-04-21 08:48:37.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/viewer_structs/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 08:49:48.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)   614698 2023-04-21 08:49:48.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2273 2023-04-21 08:49:48.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-21 08:49:48.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      568 2023-04-21 08:49:48.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-21 08:49:48.000000 th2_data_services-2.0.0.dev4763134463/th2_data_services.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:37:07.000000 th2_data_services-2.0.0.dev4783695011/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)   614698 2023-04-24 07:37:07.000000 th2_data_services-2.0.0.dev4783695011/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)   510907 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-04-24 07:36:54.000000 th2_data_services-2.0.0.dev4783695011/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)      269 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-24 07:37:07.000000 th2_data_services-2.0.0.dev4783695011/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:37:07.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:37:07.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      660 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29341 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:37:07.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/event_tree/
+-rw-r--r--   0 runner    (1001) docker     (122)      806 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/event_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/event_tree/etc_driver.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16045 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/event_tree/event_tree.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25893 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/event_tree/event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2497 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/event_tree/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2501 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/event_tree/parent_event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1680 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:37:07.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/interfaces/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      956 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/interfaces/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/interfaces/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (122)      706 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/interfaces/source_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      886 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/interfaces/struct.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2255 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/interfaces/stub_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:37:07.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/interfaces/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/interfaces/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3023 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/interfaces/utils/converter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2705 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/interfaces/utils/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:37:07.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     3360 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/_json.py
+-rw-r--r--   0 runner    (1001) docker     (122)      643 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8635 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/aggregation_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15216 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/az_tree.py
+-rw-r--r--   0 runner    (1001) docker     (122)      742 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/categorizers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      935 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/category.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3296 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/converters.py
+-rw-r--r--   0 runner    (1001) docker     (122)      908 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/decode_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2604 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/display.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:37:07.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/event_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      725 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/event_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11551 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/event_utils/display.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7107 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/event_utils/event_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5291 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/event_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12089 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/event_utils/select.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6805 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/event_utils/totals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/experimental.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:37:07.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/message_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/message_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1014 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/message_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14456 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/message_utils/message_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15739 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8330 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/perfect_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33801 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/script_report_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3531 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/sse_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5285 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6717 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/total_category_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:37:07.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/viewer_structs/
+-rw-r--r--   0 runner    (1001) docker     (122)      609 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/viewer_structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6185 2023-04-24 07:36:01.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/viewer_structs/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 07:37:07.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)   614698 2023-04-24 07:37:07.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2306 2023-04-24 07:37:07.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-24 07:37:07.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2023-04-24 07:37:07.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-24 07:37:07.000000 th2_data_services-2.0.0.dev4783695011/th2_data_services.egg-info/top_level.txt
```

### Comparing `th2_data_services-2.0.0.dev4763134463/PKG-INFO` & `th2_data_services-2.0.0.dev4783695011/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 325f  : 2.1.Name: th2_
 00000020: 6461 7461 5f73 6572 7669 6365 730a 5665  data_services.Ve
 00000030: 7273 696f 6e3a 2032 2e30 2e30 2e64 6576  rsion: 2.0.0.dev
-00000040: 3437 3633 3133 3434 3633 0a53 756d 6d61  4763134463.Summa
+00000040: 3437 3833 3639 3530 3131 0a53 756d 6d61  4783695011.Summa
 00000050: 7279 3a20 7468 325f 6461 7461 5f73 6572  ry: th2_data_ser
 00000060: 7669 6365 730a 486f 6d65 2d70 6167 653a  vices.Home-page:
 00000070: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000080: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
 00000090: 6461 7461 2d73 6572 7669 6365 730a 4175  data-services.Au
 000000a0: 7468 6f72 3a20 5448 322d 6465 7673 0a41  thor: TH2-devs.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2074 6832  uthor-email: th2
```

### Comparing `th2_data_services-2.0.0.dev4763134463/README.md` & `th2_data_services-2.0.0.dev4783695011/README.md`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/setup.py` & `th2_data_services-2.0.0.dev4783695011/setup.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/config/__init__.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/config/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/config/config.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/config/config.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/data.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from typing import Callable, Dict, Generator, List, Optional, Union, Iterable, Iterator, Any, Generic
 from weakref import finalize
 import types
 from inspect import isgeneratorfunction
 from typing import TypeVar
 from th2_data_services.interfaces.adapter import IStreamAdapter, IRecordAdapter
 from th2_data_services.config import options
+from th2_data_services.utils._json import iter_json_file
 
 # LOG import logging
 
 # LOG logger = logging.getLogger(__name__)
 
 
 # LOG class _DataLogger(logging.LoggerAdapter):
@@ -676,14 +677,25 @@
 
                 for record in self:
                     pickle.dump(record, file)
 
                 file.close()
             gc.enable()
 
+    def clear_cache(self):
+        """Clears related to data object cache file.
+
+        This function won't remove external cache file.
+        """
+        if self._read_from_external_cache_file:
+            raise Exception("It's not possible to remove external cache file via this method")
+        else:
+            if self.__is_cache_file_exists():
+                self.__delete_cache()
+
     @classmethod
     def from_cache_file(cls, filename) -> "Data":
         """Creates Data object from cache file with provided name.
 
         Args:
             filename: Name or path to cache file.
 
@@ -697,24 +709,33 @@
         if not Path(filename).resolve().exists():
             raise FileNotFoundError(f"{filename} doesn't exist")
 
         data_obj = cls([], cache=True)
         data_obj._set_custom_cache_destination(filename=filename)
         return data_obj
 
-    def clear_cache(self):
-        """Clears related to data object cache file.
+    @classmethod
+    def from_json(cls, filename, buffer_limit=250) -> "Data":
+        """Creates Data object from json file with provided name.
+
+        Args:
+            filename: Name or path to cache file.
+            buffer_limit: If limit is 0 buffer will not be used. Number of messages in buffer before parsing.
+
+        Returns:
+            Data: Data object.
+
+        Raises:
+            FileNotFoundError if provided file does not exist.
 
-        This function won't remove external cache file.
         """
-        if self._read_from_external_cache_file:
-            raise Exception("It's not possible to remove external cache file via this method")
-        else:
-            if self.__is_cache_file_exists():
-                self.__delete_cache()
+        if not Path(filename).resolve().exists():
+            raise FileNotFoundError(f"{filename} doesn't exist")
+
+        return cls(iter_json_file(filename, buffer_limit))
 
     def _set_metadata(self, metadata: Dict) -> None:
         """Set metadata of object to metadata argument.
 
         Args:
             metadata (dict): New Metadata
```

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/event_tree/__init__.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/event_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/event_tree/etc_driver.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/event_tree/etc_driver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/event_tree/event_tree.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/event_tree/event_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/event_tree/event_tree_collection.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/event_tree/event_tree_collection.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/event_tree/exceptions.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/event_tree/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/event_tree/parent_event_tree_collection.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/event_tree/parent_event_tree_collection.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/exceptions.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/interfaces/__init__.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/interfaces/adapter.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/interfaces/adapter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/interfaces/command.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/interfaces/command.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/interfaces/data_source.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/interfaces/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/interfaces/source_api.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/interfaces/source_api.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/interfaces/struct.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/interfaces/struct.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/interfaces/stub_builder.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/interfaces/stub_builder.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/interfaces/utils/__init__.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/interfaces/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/interfaces/utils/converter.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/interfaces/utils/converter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/interfaces/utils/resolver.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/interfaces/utils/resolver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/_types.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/_types.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/aggregation_classes.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/aggregation_classes.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/az_tree.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/az_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/categorizers.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/categorizers.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/category.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/category.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/converters.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/converters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/decode_error_handler.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/decode_error_handler.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/display.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/event_utils/__init__.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/event_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/event_utils/display.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/event_utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/event_utils/event_utils.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/event_utils/event_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/event_utils/frequencies.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/event_utils/frequencies.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/event_utils/select.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/event_utils/select.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/event_utils/totals.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/event_utils/totals.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/experimental.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/experimental.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/message_utils/__init__.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/message_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/message_utils/frequencies.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/message_utils/frequencies.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/message_utils/message_utils.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/message_utils/message_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/misc_utils.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/perfect_table.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/perfect_table.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/script_report_utils.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/script_report_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/sse_client.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/sse_client.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/time.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/time.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/total_category_calculator.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/total_category_calculator.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/viewer_structs/__init__.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/viewer_structs/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services/utils/viewer_structs/verification.py` & `th2_data_services-2.0.0.dev4783695011/th2_data_services/utils/viewer_structs/verification.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services.egg-info/PKG-INFO` & `th2_data_services-2.0.0.dev4783695011/th2_data_services.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 322d  : 2.1.Name: th2-
 00000020: 6461 7461 2d73 6572 7669 6365 730a 5665  data-services.Ve
 00000030: 7273 696f 6e3a 2032 2e30 2e30 2e64 6576  rsion: 2.0.0.dev
-00000040: 3437 3633 3133 3434 3633 0a53 756d 6d61  4763134463.Summa
+00000040: 3437 3833 3639 3530 3131 0a53 756d 6d61  4783695011.Summa
 00000050: 7279 3a20 7468 325f 6461 7461 5f73 6572  ry: th2_data_ser
 00000060: 7669 6365 730a 486f 6d65 2d70 6167 653a  vices.Home-page:
 00000070: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000080: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
 00000090: 6461 7461 2d73 6572 7669 6365 730a 4175  data-services.Au
 000000a0: 7468 6f72 3a20 5448 322d 6465 7673 0a41  thor: TH2-devs.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2074 6832  uthor-email: th2
```

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services.egg-info/SOURCES.txt` & `th2_data_services-2.0.0.dev4783695011/th2_data_services.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 th2_data_services/interfaces/data_source.py
 th2_data_services/interfaces/source_api.py
 th2_data_services/interfaces/struct.py
 th2_data_services/interfaces/stub_builder.py
 th2_data_services/interfaces/utils/__init__.py
 th2_data_services/interfaces/utils/converter.py
 th2_data_services/interfaces/utils/resolver.py
+th2_data_services/utils/_json.py
 th2_data_services/utils/_types.py
 th2_data_services/utils/aggregation_classes.py
 th2_data_services/utils/az_tree.py
 th2_data_services/utils/categorizers.py
 th2_data_services/utils/category.py
 th2_data_services/utils/converters.py
 th2_data_services/utils/decode_error_handler.py
```

### Comparing `th2_data_services-2.0.0.dev4763134463/th2_data_services.egg-info/requires.txt` & `th2_data_services-2.0.0.dev4783695011/th2_data_services.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 requests~=2.28
 urllib3~=1.26
 treelib==1.6.1
 types-protobuf==3.19.22
 tabulate
 prettytable
 deprecated
+orjson
 
 [lwdp]
 th2-data-services-lwdp
 
 [lwdp-dev]
 th2-data-services-lwdp~=2.0.2.0.dev
```


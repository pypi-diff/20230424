# Comparing `tmp/pythonsdk-0.3.0.tar.gz` & `tmp/pythonsdk-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonsdk-0.3.0.tar", last modified: Sun Apr 23 15:32:41 2023, max compression
+gzip compressed data, was "pythonsdk-0.4.0.tar", last modified: Mon Apr 24 08:36:06 2023, max compression
```

## Comparing `pythonsdk-0.3.0.tar` & `pythonsdk-0.4.0.tar`

### file list

```diff
@@ -1,80 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:32:41.027276 pythonsdk-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-04-23 15:32:41.027276 pythonsdk-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 15:32:41.027276 pythonsdk-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:32:41.019276 pythonsdk-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:32:41.019276 pythonsdk-0.3.0/src/python_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:32:41.019276 pythonsdk-0.3.0/src/python_sdk/_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/_cli/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/_cli/_fmt.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/_cli/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:32:41.019276 pythonsdk-0.3.0/src/python_sdk/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/bin/_call.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:32:41.023276 pythonsdk-0.3.0/src/python_sdk/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11782 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/config/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/config/_config_documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/config/_config_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/config/_config_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/config/_config_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/config/_config_value_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/config/_config_value_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/config/_optional_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/config/_string_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:32:41.023276 pythonsdk-0.3.0/src/python_sdk/encoding/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/encoding/_base64url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:32:41.023276 pythonsdk-0.3.0/src/python_sdk/log/
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/log/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/log/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/log/_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/log/_formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/log/_log.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/log/_log_levels.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:32:41.023276 pythonsdk-0.3.0/src/python_sdk/secrets/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/secrets/_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:32:41.023276 pythonsdk-0.3.0/src/python_sdk/secrets/_secrets_engine/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/secrets/_secrets_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/secrets/_secrets_engine/_aws_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/secrets/_secrets_engine/_aws_secrets_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/secrets/_secrets_engine/_aws_systems_manager_parameter_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/secrets/_secrets_engine/_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/secrets/_secrets_engine/_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:32:41.023276 pythonsdk-0.3.0/src/python_sdk/sentinel/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/sentinel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/sentinel/_sentinel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:32:41.023276 pythonsdk-0.3.0/src/python_sdk/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/testing/_prepackaged_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:32:41.027276 pythonsdk-0.3.0/src/python_sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/utils/_ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/utils/_checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/utils/_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/utils/_file_watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/utils/_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/utils/_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/utils/_which.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/utils/_zipfile.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 15:32:35.000000 pythonsdk-0.3.0/src/python_sdk/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:32:41.027276 pythonsdk-0.3.0/src/python_sdk/versioning/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/versioning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/src/python_sdk/versioning/_version_file_based.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:32:41.027276 pythonsdk-0.3.0/src/pythonsdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-04-23 15:32:41.000000 pythonsdk-0.3.0/src/pythonsdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-04-23 15:32:41.000000 pythonsdk-0.3.0/src/pythonsdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 15:32:41.000000 pythonsdk-0.3.0/src/pythonsdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-23 15:32:41.000000 pythonsdk-0.3.0/src/pythonsdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-23 15:32:41.000000 pythonsdk-0.3.0/src/pythonsdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-23 15:32:41.000000 pythonsdk-0.3.0/src/pythonsdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 15:32:09.000000 pythonsdk-0.3.0/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:36:06.693134 pythonsdk-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-04-24 08:36:06.693134 pythonsdk-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 08:36:06.697134 pythonsdk-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:36:06.685134 pythonsdk-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:36:06.685134 pythonsdk-0.4.0/src/python_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:36:06.689134 pythonsdk-0.4.0/src/python_sdk/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/_cli/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/_cli/_fmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/_cli/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:36:06.689134 pythonsdk-0.4.0/src/python_sdk/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/bin/_call.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:36:06.689134 pythonsdk-0.4.0/src/python_sdk/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/config/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/config/_config_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/config/_config_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/config/_config_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/config/_config_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/config/_config_value_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/config/_config_value_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/config/_optional_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/config/_string_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:36:06.689134 pythonsdk-0.4.0/src/python_sdk/encoding/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/encoding/_base64url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:36:06.689134 pythonsdk-0.4.0/src/python_sdk/log/
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/log/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/log/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/log/_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/log/_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/log/_log_levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/log/_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:36:06.689134 pythonsdk-0.4.0/src/python_sdk/log/_logging_formatter/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/log/_logging_formatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/log/_logging_formatter/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/log/_logging_formatter/_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/log/_logging_formatter/_structured_human_readable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/log/_logging_formatter/_structured_machine_readable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:36:06.693134 pythonsdk-0.4.0/src/python_sdk/log/_logging_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/log/_logging_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/log/_logging_handler/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/log/_logging_handler/_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/log/_logging_handler/_rotating_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/log/_logging_handler/_stderr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/log/_logging_handler/_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:36:06.693134 pythonsdk-0.4.0/src/python_sdk/secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/secrets/_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:36:06.693134 pythonsdk-0.4.0/src/python_sdk/secrets/_secrets_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/secrets/_secrets_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/secrets/_secrets_engine/_aws_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/secrets/_secrets_engine/_aws_secrets_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/secrets/_secrets_engine/_aws_systems_manager_parameter_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/secrets/_secrets_engine/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/secrets/_secrets_engine/_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:36:06.693134 pythonsdk-0.4.0/src/python_sdk/sentinel/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/sentinel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/sentinel/_sentinel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:36:06.693134 pythonsdk-0.4.0/src/python_sdk/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/testing/_prepackaged_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:36:06.693134 pythonsdk-0.4.0/src/python_sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/utils/_ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/utils/_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/utils/_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/utils/_file_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/utils/_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/utils/_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/utils/_which.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/utils/_zipfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-24 08:36:01.000000 pythonsdk-0.4.0/src/python_sdk/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:36:06.693134 pythonsdk-0.4.0/src/python_sdk/versioning/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/versioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/src/python_sdk/versioning/_version_file_based.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:36:06.693134 pythonsdk-0.4.0/src/pythonsdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-04-24 08:36:06.000000 pythonsdk-0.4.0/src/pythonsdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-24 08:36:06.000000 pythonsdk-0.4.0/src/pythonsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 08:36:06.000000 pythonsdk-0.4.0/src/pythonsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-24 08:36:06.000000 pythonsdk-0.4.0/src/pythonsdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-24 08:36:06.000000 pythonsdk-0.4.0/src/pythonsdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-24 08:36:06.000000 pythonsdk-0.4.0/src/pythonsdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-24 08:35:39.000000 pythonsdk-0.4.0/version
```

### Comparing `pythonsdk-0.3.0/LICENSE` & `pythonsdk-0.4.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Lijok
+Copyright (c) 2023 Lijok
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pythonsdk-0.3.0/PKG-INFO` & `pythonsdk-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pythonsdk
-Version: 0.3.0
+Version: 0.4.0
 Summary: Python Software Dev Kit
 Author-email: lijok <lijok@pm.me>
 License: MIT License
         
-        Copyright (c) 2022 Lijok
+        Copyright (c) 2023 Lijok
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
```

### Comparing `pythonsdk-0.3.0/pyproject.toml` & `pythonsdk-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.3.0/src/python_sdk/_cli/_cli.py` & `pythonsdk-0.4.0/src/python_sdk/_cli/_cli.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.3.0/src/python_sdk/_cli/_fmt.py` & `pythonsdk-0.4.0/src/python_sdk/_cli/_fmt.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.3.0/src/python_sdk/bin/_call.py` & `pythonsdk-0.4.0/src/python_sdk/bin/_call.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.3.0/src/python_sdk/config/__init__.py` & `pythonsdk-0.4.0/src/python_sdk/config/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 from python_sdk.config._config_sources import RemoteHTTPFile as RemoteHTTPFile
 from python_sdk.config._config_sources import S3File as S3File
 from python_sdk.config._config_sources import StaticDictionary as StaticDictionary
 from python_sdk.config._config_validators import ConfigValidationError as ConfigValidationError
 from python_sdk.config._config_validators import ConfigValidator as ConfigValidator
 from python_sdk.config._config_value_types import Base64EncodedString as Base64EncodedString
 from python_sdk.config._config_value_types import ConfigValueType as ConfigValueType
-from python_sdk.config._config_value_types import UnvalidatedDict as UnvalidatedDict
 from python_sdk.config._config_value_validators import ConfigValueValidationError as ConfigValueValidationError
 from python_sdk.config._config_value_validators import ConfigValueValidator as ConfigValueValidator
-from python_sdk.config._config_value_validators import EnsureDirectoryExists as EnsureDirectoryExists
-from python_sdk.config._config_value_validators import EnsureFileExists as EnsureFileExists
-from python_sdk.config._config_value_validators import EnsureFileType as EnsureFileType
-from python_sdk.config._config_value_validators import EnsurePathIsExecutable as EnsurePathIsExecutable
-from python_sdk.config._config_value_validators import EnsurePathIsReadable as EnsurePathIsReadable
-from python_sdk.config._config_value_validators import EnsurePathIsWritable as EnsurePathIsWritable
+from python_sdk.config._config_value_validators import ValidateDirectoryExists as ValidateDirectoryExists
+from python_sdk.config._config_value_validators import ValidateFileExists as ValidateFileExists
+from python_sdk.config._config_value_validators import ValidateFileType as ValidateFileType
+from python_sdk.config._config_value_validators import ValidatePathIsExecutable as ValidatePathIsExecutable
+from python_sdk.config._config_value_validators import ValidatePathIsReadable as ValidatePathIsReadable
+from python_sdk.config._config_value_validators import ValidatePathIsWritable as ValidatePathIsWritable
```

### Comparing `pythonsdk-0.3.0/src/python_sdk/config/_config.py` & `pythonsdk-0.4.0/src/python_sdk/config/_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -214,14 +214,23 @@
     @classmethod
     def hardcode_config_value(cls, option: str, value: _config_value_types.ConfigValueType) -> None:
         config_option = cls.get_config_option(option=option)
         config_option.hardcode_value(value=value)
         cls.validate()
         cls.post_load_hook()
 
+    @classmethod
+    def last_loaded_at(cls) -> datetime.datetime | None:
+        return cls.meta.last_loaded_at
+
+    @classmethod
+    def last_load_contained_changes(cls) -> bool:
+        # TODO: Implement this
+        return False
+
 
 # TODO: How do we allow custom config sources if SOURCE is a literal?
 class ConfigSourcesConfig(
     Config,
     name="Config Sources Config",
     description="""
     Configuration used by config sources to configure their behaviour, particularly around document sourcing.
@@ -241,15 +250,15 @@
         description="Where configurations will be sourced from.",
     )
     SOURCE_LOCAL_FILE_FILEPATH: pathlib.Path | None = _config_option.Option(
         description="""
         Filepath for the LOCAL_FILE config source. Required when PYTHON_SDK_CONFIG_SOURCE is set to LOCAL_FILE.
         The file must exist and be readable by the running process.
         """,
-        validators=[_config_value_validators.EnsureFileExists(), _config_value_validators.EnsurePathIsReadable()],
+        validators=[_config_value_validators.ValidateFileExists(), _config_value_validators.ValidatePathIsReadable()],
     )
     SOURCE_REMOTE_HTTP_FILE_URL: str | None = _config_option.Option(
         description="""
         URL for the REMOTE_HTTP_FILE config source. Required when PYTHON_SDK_CONFIG_SOURCE is set to REMOTE_HTTP_FILE.
         """
     )
     SOURCE_REMOTE_HTTP_FILE_TIMEOUT: int = _config_option.Option(
```

### Comparing `pythonsdk-0.3.0/src/python_sdk/config/_config_option.py` & `pythonsdk-0.4.0/src/python_sdk/config/_config_option.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import copy
 import functools
-import types
 import typing
 
 from python_sdk import sentinel
 from python_sdk.config import _optional_type
 from python_sdk.config import _string_decoder
 
 if typing.TYPE_CHECKING:
```

### Comparing `pythonsdk-0.3.0/src/python_sdk/config/_config_sources.py` & `pythonsdk-0.4.0/src/python_sdk/config/_config_sources.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.3.0/src/python_sdk/config/_config_value_validators.py` & `pythonsdk-0.4.0/src/python_sdk/config/_config_value_validators.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 import pathlib
 import typing
 
 if typing.TYPE_CHECKING:
     from python_sdk.config import _config_option
-    from python_sdk.config import _config_value_types
 
 
 class ConfigValueValidationError(Exception):
     """Config Value does not pass validation."""
 
     ...
 
@@ -26,16 +25,16 @@
         """
         Raises:
             ConfigValueValidationError: Config value does not pass validation.
         """
         ...
 
 
-class EnsureFileExists:
-    name: str = "Ensure File Exists"
+class ValidateFileExists:
+    name: str = "Validate File Exists"
     description: str = "Validates that the file at a given path exists."
 
     def __call__(
         self,
         config_option_name: str,
         config_option: "_config_option.ConfigOption",
         config_value: pathlib.Path,
@@ -46,16 +45,16 @@
         """
         if not config_value.exists():
             raise ConfigValueValidationError(f"File at {config_value} does not exist.")
         if not config_value.is_file():
             raise ConfigValueValidationError(f"{config_value} not a file.")
 
 
-class EnsureDirectoryExists:
-    name: str = "Ensure Directory Exists"
+class ValidateDirectoryExists:
+    name: str = "Validate Directory Exists"
     description: str = "Validates that the directory at a given path exists."
 
     def __call__(
         self,
         config_option_name: str,
         config_option: "_config_option.ConfigOption",
         config_value: pathlib.Path,
@@ -66,72 +65,73 @@
         """
         if not config_value.exists():
             raise ConfigValueValidationError(f"Directory at {config_value} does not exist.")
         if not config_value.is_dir():
             raise ConfigValueValidationError(f"{config_value} not a directory.")
 
 
-class EnsurePathIsReadable:
-    name: str = "Ensure Path is Readable"
+class ValidatePathIsReadable:
+    name: str = "Validate Path is Readable"
     description: str = "Validates that a given path is readable."
 
     def __call__(
         self,
         config_option_name: str,
         config_option: "_config_option.ConfigOption",
         config_value: pathlib.Path,
     ) -> None:
         """
         Raises:
             ConfigValueValidationError: Path is not readable.
         """
-        if not os.access(config_value, os.R_OK):
+        path_to_evaluate = config_value if config_value.exists() else config_value.parent
+        if not os.access(path_to_evaluate, os.R_OK):
             raise ConfigValueValidationError(f"{config_value} is not readable.")
 
 
-class EnsurePathIsWritable:
-    name: str = "Ensure Path is Writable"
+class ValidatePathIsWritable:
+    name: str = "Validate Path is Writable"
     description: str = "Validates that a given path is writeable."
 
     def __call__(
         self,
         config_option_name: str,
         config_option: "_config_option.ConfigOption",
         config_value: pathlib.Path,
     ) -> None:
         """
         Raises:
             ConfigValueValidationError: Path is not writeable.
         """
-        if not os.access(config_value, os.W_OK):
+        path_to_evaluate = config_value if config_value.exists() else config_value.parent
+        if not os.access(path_to_evaluate, os.W_OK):
             raise ConfigValueValidationError(f"{config_value} is not writeable")
 
 
-class EnsurePathIsExecutable:
-    name: str = "Ensure Path is Executable"
+class ValidatePathIsExecutable:
+    name: str = "Validate Path is Executable"
     description: str = "Validates that a given path is executable."
 
     def __call__(
         self,
         config_option_name: str,
         config_option: "_config_option.ConfigOption",
         config_value: pathlib.Path,
     ) -> None:
         """
         Raises:
             ConfigValueValidationError: Path is not executable.
         """
-        if not os.access(config_value, os.EX_OK):
-            # with contextlib.suppress(FileNotFoundError, PermissionError):
-            #     os.chmod(config_value, os.stat(config_value).st_mode | stat.S_IEXEC)
+        path_to_evaluate = config_value if config_value.exists() else config_value.parent
+        if not os.access(path_to_evaluate, os.EX_OK):
             raise ConfigValueValidationError(f"{config_value} is not executable")
 
 
-class EnsureFileType:
-    name: str = "Ensure File Type"
+class ValidateFileType:
+    name: str = "Validate File Type"
     description: str = "Validates that the file at a given path is of set file type."
 
     def __init__(self, file_type: str) -> None:
         self.file_type = file_type if file_type[0] == "." else f".{file_type}"
 
     def __call__(
         self,
```

### Comparing `pythonsdk-0.3.0/src/python_sdk/config/_string_decoder.py` & `pythonsdk-0.4.0/src/python_sdk/config/_string_decoder.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import base64
 import functools
+import json
 import pathlib
 import typing
 
 from python_sdk.config import _config_value_types
 
 ENCODED_STRING_LIST_SEPARATOR = ","
 
@@ -15,19 +16,34 @@
     if normalized_string in {"true", "yes", "y", "1", "on"}:
         return True
     elif normalized_string in {"false", "no", "n", "0", "off"}:
         return False
     raise ValueError()
 
 
+def _str_to_dict(string: str) -> dict[str, typing.Any]:
+    try:
+        data = json.loads(string)
+    except json.JSONDecodeError:
+        raise ValueError()
+
+    if not isinstance(data, dict):
+        raise ValueError()
+
+    return data
+
+
 def _str_to_base64_encoded_string(string: str) -> str:
     string = string.strip()
     if not string:
         raise ValueError()
-    base64.b64decode(string, validate=True).decode("utf-8")  # check it can be decoded
+    try:
+        base64.b64decode(string, validate=True).decode("utf-8")  # check it can be decoded
+    except Exception as e:
+        raise ValueError() from e
     return string
 
 
 def _str_to_literal(string: str, literal: type) -> str:
     string = string.strip()
     if string not in typing.get_args(literal):
         raise ValueError()
@@ -58,15 +74,15 @@
 def _str_to_list_of_base64_encoded_strings(string: str) -> list[str]:
     string = string.strip().strip(ENCODED_STRING_LIST_SEPARATOR)
     if not string:
         raise ValueError()
     maybe_base64_encoded_strings = string.split(ENCODED_STRING_LIST_SEPARATOR)
     for i in maybe_base64_encoded_strings:
         # check they can be decoded
-        base64.b64decode(i, validate=True).decode("utf-8")
+        _str_to_base64_encoded_string(string=i)
     return maybe_base64_encoded_strings
 
 
 def _str_to_list_of_paths(string: str) -> list[pathlib.Path]:
     if not string:
         raise ValueError()
     return [pathlib.Path(path) for path in string.split(ENCODED_STRING_LIST_SEPARATOR)]
@@ -90,16 +106,16 @@
         return str
     elif data_type == int:
         return int
     elif data_type == float:
         return float
     elif data_type == bool:
         return _str_to_bool
-    elif data_type == _config_value_types.UnvalidatedDict:
-        return _config_value_types.UnvalidatedDict
+    elif getattr(data_type, "__origin__", None) == dict:
+        return _str_to_dict
     elif data_type == _config_value_types.Base64EncodedString:
         return _str_to_base64_encoded_string
     elif data_type == pathlib.Path:
         return pathlib.Path
     elif _is_literal(data_type=data_type):
         return functools.partial(_str_to_literal, literal=data_type)
```

### Comparing `pythonsdk-0.3.0/src/python_sdk/encoding/_base64url.py` & `pythonsdk-0.4.0/src/python_sdk/encoding/_base64url.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.3.0/src/python_sdk/log/__init__.py` & `pythonsdk-0.4.0/src/python_sdk/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.3.0/src/python_sdk/log/_context.py` & `pythonsdk-0.4.0/src/python_sdk/log/_context.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.3.0/src/python_sdk/log/_formatters.py` & `pythonsdk-0.4.0/src/python_sdk/log/_logging_formatter/_structured_human_readable.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 import copy
 import datetime
 import io
-import json
 import logging
 import traceback
 import types
 import typing
 
 import python_sdk
 
 
-class StructuredLogFormatter(logging.Formatter):
+class StructuredHumanReadable:
+    TYPE: str = "STRUCTURED_HUMAN_READABLE"
+
     include_current_log_filename: bool
     include_function_name: bool
     include_line_number: bool
     include_module_name: bool
     include_module_path: bool
     include_process_id: bool
     include_process_name: bool
     include_thread_id: bool
     include_thread_name: bool
     include_python_sdk_version: bool
 
     def __init__(
         self,
-        include_current_log_filename: bool = True,
-        include_function_name: bool = True,
-        include_line_number: bool = True,
-        include_module_name: bool = True,
-        include_module_path: bool = True,
-        include_process_id: bool = True,
-        include_process_name: bool = True,
-        include_thread_id: bool = True,
-        include_thread_name: bool = True,
-        include_python_sdk_version: bool = True,
+        include_current_log_filename: bool,
+        include_function_name: bool,
+        include_line_number: bool,
+        include_module_name: bool,
+        include_module_path: bool,
+        include_process_id: bool,
+        include_process_name: bool,
+        include_thread_id: bool,
+        include_thread_name: bool,
+        include_python_sdk_version: bool,
     ) -> None:
         super().__init__()
 
         self.include_current_log_filename = include_current_log_filename
         self.include_function_name = include_function_name
         self.include_line_number = include_line_number
         self.include_module_name = include_module_name
@@ -95,15 +96,21 @@
                 logging.warning(f"Attempted to overwrite log attribute: {key}. Log attributes cannot be overwritten.")
             else:
                 data[key] = context[key]
 
         return data
 
     def format(self, record: logging.LogRecord) -> str:
-        return json.dumps(self.pre_format(record=record), default=str)
+        data = self.pre_format(record=record)
+        padding = max(60 - len(data["message"]), 0)
+        text = f"{data['timestamp']} [{data['log_level']}\t] {data['message']} {' ' * padding}"
+        for key, val in data.items():
+            if key not in ["timestamp", "log_level", "message"]:
+                text += f" {key}={val}"
+        return text
 
     # taken from logging.Formatter.formatException
     def format_exception(
         self, ei: tuple[type[BaseException], BaseException, types.TracebackType | None] | tuple[None, None, None]
     ) -> str:
         """
         Format and return the specified exception information as a string.
@@ -151,24 +158,7 @@
 
             context_key, context_value = word.split("=")
             embedded_context[context_key] = context_value.strip("'")
             tokenized_message.pop(-1)
 
         new_message = " ".join(tokenized_message)
         return new_message, embedded_context
-
-
-class StructuredLogMachineReadableFormatter(StructuredLogFormatter):
-    def format(self, record: logging.LogRecord) -> str:
-        data = super().pre_format(record=record)
-        return json.dumps(data, default=str)
-
-
-class StructuredLogHumanReadableFormatter(StructuredLogFormatter):
-    def format(self, record: logging.LogRecord) -> str:
-        data = super().pre_format(record=record)
-        padding = max(60 - len(data["message"]), 0)
-        text = f"{data['timestamp']} [{data['log_level']}\t] {data['message']} {' ' * padding}"
-        for key, val in data.items():
-            if key not in ["timestamp", "log_level", "message"]:
-                text += f" {key}={val}"
-        return text
```

### Comparing `pythonsdk-0.3.0/src/python_sdk/log/_log.py` & `pythonsdk-0.4.0/src/python_sdk/log/_log.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 import logging
 import sys
 import types
 import typing
 
 from python_sdk.log import _context
 from python_sdk.log import _log_levels
+from python_sdk.log import _logger
 
 
 def _log(
     level: int,
     message: typing.Any,
     exception: BaseException
     | tuple[type[BaseException], BaseException, types.TracebackType]
     | tuple[None, None, None]
     | None = None,
     _stack_level: int = 2,
     **kwargs: typing.Any,
 ) -> None:
-    root_logger = logging.getLogger()
+    logger = _logger.logger()
 
     # root_logger.log does this check itself.
     # However, just below this, we're doing a potentially expensive dictionary merge.
     # So, as a simple performance optimization, we run this check before we do the dictionary merge.
-    if not root_logger.isEnabledFor(level=level):
+    if not logger.isEnabledFor(level=level):
         return
 
     data = _context.get_context() | kwargs
-    root_logger.log(level=level, msg=message, exc_info=exception, stacklevel=_stack_level, extra={"context": data})
+    logger.log(level=level, msg=message, exc_info=exception, stacklevel=_stack_level, extra={"context": data})
 
 
 def critical(message: typing.Any, **kwargs: typing.Any) -> None:
     _log(level=logging.CRITICAL, message=message, _stack_level=3, **kwargs)
 
 
 def error(message: typing.Any, **kwargs: typing.Any) -> None:
```

### Comparing `pythonsdk-0.3.0/src/python_sdk/secrets/__init__.py` & `pythonsdk-0.4.0/src/python_sdk/secrets/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import typing
 
+from python_sdk.secrets._config import AWSSecretsEngineConfig as AWSSecretsEngineConfig
 from python_sdk.secrets._config import SecretsConfig as SecretsConfig
 from python_sdk.secrets._secrets_engine import DoesNotExist as DoesNotExist
 from python_sdk.secrets._secrets_engine import Unauthorized as Unauthorized
 from python_sdk.secrets._secrets_engine import register_implementation as register_implementation
 from python_sdk.secrets._secrets_engine import secrets_engine as secrets_engine
```

### Comparing `pythonsdk-0.3.0/src/python_sdk/secrets/_config.py` & `pythonsdk-0.4.0/src/python_sdk/secrets/_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import typing
+
 from python_sdk import config
 
 
 # TODO(lijok): something to prevent this from being configured using secrets
 class SecretsConfig(config.Config, option_prefix="PYTHON_SDK_SECRETS_"):
     ENGINE: str = config.Option(default="AWS_SECRETS_MANAGER")
 
@@ -19,10 +21,10 @@
     SECRET_ACCESS_KEY: str | None = config.Option()
     SESSION_TOKEN: str | None = config.Option()
     REGION_NAME: str | None = config.Option()
     API_VERSION: str | None = config.Option()
     USE_SSL: bool = config.Option(default=True)
     VERIFY: bool = config.Option(default=True)
     ENDPOINT_URL: str | None = config.Option()
-    BOTOCORE_CONFIG: config.UnvalidatedDict | None = config.Option(
+    BOTOCORE_CONFIG: dict[str, typing.Any] | None = config.Option(
         description="See https://botocore.amazonaws.com/v1/documentation/api/latest/reference/config.html"
     )
```

### Comparing `pythonsdk-0.3.0/src/python_sdk/secrets/_secrets_engine/_aws_s3.py` & `pythonsdk-0.4.0/src/python_sdk/secrets/_secrets_engine/_aws_s3.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.3.0/src/python_sdk/secrets/_secrets_engine/_aws_secrets_manager.py` & `pythonsdk-0.4.0/src/python_sdk/secrets/_secrets_engine/_aws_secrets_manager.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.3.0/src/python_sdk/secrets/_secrets_engine/_aws_systems_manager_parameter_store.py` & `pythonsdk-0.4.0/src/python_sdk/secrets/_secrets_engine/_aws_systems_manager_parameter_store.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.3.0/src/python_sdk/secrets/_secrets_engine/_factory.py` & `pythonsdk-0.4.0/src/python_sdk/secrets/_secrets_engine/_factory.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.3.0/src/python_sdk/secrets/_secrets_engine/_protocol.py` & `pythonsdk-0.4.0/src/python_sdk/secrets/_secrets_engine/_protocol.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.3.0/src/python_sdk/sentinel/_sentinel.py` & `pythonsdk-0.4.0/src/python_sdk/sentinel/_sentinel.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.3.0/src/python_sdk/testing/_prepackaged_tests.py` & `pythonsdk-0.4.0/src/python_sdk/testing/_prepackaged_tests.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.3.0/src/python_sdk/utils/__init__.py` & `pythonsdk-0.4.0/src/python_sdk/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.3.0/src/python_sdk/utils/_file_watcher.py` & `pythonsdk-0.4.0/src/python_sdk/utils/_file_watcher.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.3.0/src/python_sdk/utils/_zipfile.py` & `pythonsdk-0.4.0/src/python_sdk/utils/_zipfile.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.3.0/src/python_sdk/versioning/_version_file_based.py` & `pythonsdk-0.4.0/src/python_sdk/versioning/_version_file_based.py`

 * *Files identical despite different names*

### Comparing `pythonsdk-0.3.0/src/pythonsdk.egg-info/PKG-INFO` & `pythonsdk-0.4.0/src/pythonsdk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: pythonsdk
-Version: 0.3.0
+Version: 0.4.0
 Summary: Python Software Dev Kit
 Author-email: lijok <lijok@pm.me>
 License: MIT License
         
-        Copyright (c) 2022 Lijok
+        Copyright (c) 2023 Lijok
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
```

### Comparing `pythonsdk-0.3.0/src/pythonsdk.egg-info/SOURCES.txt` & `pythonsdk-0.4.0/src/pythonsdk.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -25,17 +25,28 @@
 src/python_sdk/config/_string_decoder.py
 src/python_sdk/encoding/__init__.py
 src/python_sdk/encoding/_base64url.py
 src/python_sdk/log/__init__.py
 src/python_sdk/log/_base.py
 src/python_sdk/log/_config.py
 src/python_sdk/log/_context.py
-src/python_sdk/log/_formatters.py
 src/python_sdk/log/_log.py
 src/python_sdk/log/_log_levels.py
+src/python_sdk/log/_logger.py
+src/python_sdk/log/_logging_formatter/__init__.py
+src/python_sdk/log/_logging_formatter/_factory.py
+src/python_sdk/log/_logging_formatter/_protocol.py
+src/python_sdk/log/_logging_formatter/_structured_human_readable.py
+src/python_sdk/log/_logging_formatter/_structured_machine_readable.py
+src/python_sdk/log/_logging_handler/__init__.py
+src/python_sdk/log/_logging_handler/_factory.py
+src/python_sdk/log/_logging_handler/_protocol.py
+src/python_sdk/log/_logging_handler/_rotating_file.py
+src/python_sdk/log/_logging_handler/_stderr.py
+src/python_sdk/log/_logging_handler/_stdout.py
 src/python_sdk/secrets/__init__.py
 src/python_sdk/secrets/_config.py
 src/python_sdk/secrets/_secrets_engine/__init__.py
 src/python_sdk/secrets/_secrets_engine/_aws_s3.py
 src/python_sdk/secrets/_secrets_engine/_aws_secrets_manager.py
 src/python_sdk/secrets/_secrets_engine/_aws_systems_manager_parameter_store.py
 src/python_sdk/secrets/_secrets_engine/_factory.py
```


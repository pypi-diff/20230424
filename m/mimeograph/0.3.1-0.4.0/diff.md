# Comparing `tmp/mimeograph-0.3.1.tar.gz` & `tmp/mimeograph-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mimeograph-0.3.1.tar", last modified: Tue Apr 18 09:44:20 2023, max compression
+gzip compressed data, was "mimeograph-0.4.0.tar", last modified: Mon Apr 24 16:21:39 2023, max compression
```

## Comparing `mimeograph-0.3.1.tar` & `mimeograph-0.4.0.tar`

### file list

```diff
@@ -1,70 +1,76 @@
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-18 09:44:20.700028 mimeograph-0.3.1/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1075 2023-03-13 05:35:12.000000 mimeograph-0.3.1/LICENSE
--rw-rw-r--   0 tom       (1000) tom       (1000)       69 2023-03-31 04:40:40.000000 mimeograph-0.3.1/MANIFEST.in
--rw-rw-r--   0 tom       (1000) tom       (1000)    21308 2023-04-18 09:44:20.700028 mimeograph-0.3.1/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)    19351 2023-04-18 09:43:35.000000 mimeograph-0.3.1/README.md
--rw-rw-r--   0 tom       (1000) tom       (1000)     1422 2023-04-18 09:43:59.000000 mimeograph-0.3.1/pyproject.toml
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-04-18 09:44:20.700028 mimeograph-0.3.1/setup.cfg
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-18 09:44:20.692028 mimeograph-0.3.1/src/
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-18 09:44:20.692028 mimeograph-0.3.1/src/mimeo/
--rw-rw-r--   0 tom       (1000) tom       (1000)       53 2023-04-18 09:43:59.000000 mimeograph-0.3.1/src/mimeo/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     9525 2023-04-18 09:43:59.000000 mimeograph-0.3.1/src/mimeo/__main__.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-18 09:44:20.692028 mimeograph-0.3.1/src/mimeo/config/
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-03-13 09:26:49.000000 mimeograph-0.3.1/src/mimeo/config/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    11602 2023-04-18 09:21:02.000000 mimeograph-0.3.1/src/mimeo/config/mimeo_config.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-18 09:44:20.692028 mimeograph-0.3.1/src/mimeo/consumers/
--rw-rw-r--   0 tom       (1000) tom       (1000)      195 2023-03-27 15:10:13.000000 mimeograph-0.3.1/src/mimeo/consumers/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      353 2023-04-18 09:21:02.000000 mimeograph-0.3.1/src/mimeo/consumers/consumer.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      881 2023-04-18 09:21:02.000000 mimeograph-0.3.1/src/mimeo/consumers/consumer_factory.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      949 2023-03-31 04:40:40.000000 mimeograph-0.3.1/src/mimeo/consumers/file_consumer.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1478 2023-03-31 04:40:40.000000 mimeograph-0.3.1/src/mimeo/consumers/http_consumer.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      131 2023-03-11 12:33:58.000000 mimeograph-0.3.1/src/mimeo/consumers/raw_consumer.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-18 09:44:20.696028 mimeograph-0.3.1/src/mimeo/context/
--rw-rw-r--   0 tom       (1000) tom       (1000)      139 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/context/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1724 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/context/annotations.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      363 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/context/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4098 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/context/mimeo_context.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1506 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/context/mimeo_context_manager.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1025 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/context/mimeo_iteration.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-18 09:44:20.696028 mimeograph-0.3.1/src/mimeo/database/
--rw-rw-r--   0 tom       (1000) tom       (1000)      109 2023-03-31 04:40:40.000000 mimeograph-0.3.1/src/mimeo/database/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2085 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/database/cities.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2086 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/database/countries.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      125 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/database/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1316 2023-03-31 04:40:40.000000 mimeograph-0.3.1/src/mimeo/database/mimeo_db.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      649 2023-04-03 07:14:05.000000 mimeograph-0.3.1/src/mimeo/exceptions.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-18 09:44:20.696028 mimeograph-0.3.1/src/mimeo/generators/
--rw-rw-r--   0 tom       (1000) tom       (1000)      121 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/generators/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      891 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/generators/generator.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      512 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/generators/generator_factory.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5745 2023-04-14 15:51:40.000000 mimeograph-0.3.1/src/mimeo/generators/xml_generator.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-18 09:44:20.696028 mimeograph-0.3.1/src/mimeo/logging/
--rw-rw-r--   0 tom       (1000) tom       (1000)      380 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/logging/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      275 2023-03-31 04:40:40.000000 mimeograph-0.3.1/src/mimeo/logging/filters.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-18 09:44:20.696028 mimeograph-0.3.1/src/mimeo/meta/
--rw-rw-r--   0 tom       (1000) tom       (1000)       39 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/meta/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      993 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/meta/alive.py
--rw-rw-r--   0 tom       (1000) tom       (1000)       44 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/meta/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      625 2023-03-31 04:40:40.000000 mimeograph-0.3.1/src/mimeo/mimeo.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-18 09:44:20.696028 mimeograph-0.3.1/src/mimeo/resources/
--rw-rw-r--   0 tom       (1000) tom       (1000)        0 2023-03-31 04:40:40.000000 mimeograph-0.3.1/src/mimeo/resources/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)  1541655 2023-03-31 04:40:40.000000 mimeograph-0.3.1/src/mimeo/resources/cities.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)     4205 2023-03-31 04:40:40.000000 mimeograph-0.3.1/src/mimeo/resources/countries.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)      719 2023-03-31 04:40:40.000000 mimeograph-0.3.1/src/mimeo/resources/logging.yaml
--rw-rw-r--   0 tom       (1000) tom       (1000)      455 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/tools.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-18 09:44:20.696028 mimeograph-0.3.1/src/mimeo/utils/
--rw-rw-r--   0 tom       (1000) tom       (1000)      301 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/utils/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      132 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/utils/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6963 2023-04-18 09:43:35.000000 mimeograph-0.3.1/src/mimeo/utils/mimeo_utils.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     6555 2023-04-14 09:39:06.000000 mimeograph-0.3.1/src/mimeo/utils/renderer.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-18 09:44:20.696028 mimeograph-0.3.1/src/mimeograph.egg-info/
--rw-rw-r--   0 tom       (1000) tom       (1000)    21308 2023-04-18 09:44:20.000000 mimeograph-0.3.1/src/mimeograph.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)     1596 2023-04-18 09:44:20.000000 mimeograph-0.3.1/src/mimeograph.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-04-18 09:44:20.000000 mimeograph-0.3.1/src/mimeograph.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       46 2023-04-18 09:44:20.000000 mimeograph-0.3.1/src/mimeograph.egg-info/entry_points.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       91 2023-04-18 09:44:20.000000 mimeograph-0.3.1/src/mimeograph.egg-info/requires.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        6 2023-04-18 09:44:20.000000 mimeograph-0.3.1/src/mimeograph.egg-info/top_level.txt
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-18 09:44:20.696028 mimeograph-0.3.1/tests/
--rw-rw-r--   0 tom       (1000) tom       (1000)    31428 2023-04-14 15:51:40.000000 mimeograph-0.3.1/tests/test_mimeo_cli.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1833 2023-04-14 09:39:06.000000 mimeograph-0.3.1/tests/test_mimeograph.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      462 2023-04-14 09:39:06.000000 mimeograph-0.3.1/tests/test_utils.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 16:21:39.763099 mimeograph-0.4.0/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1075 2023-03-13 05:35:12.000000 mimeograph-0.4.0/LICENSE
+-rw-rw-r--   0 tom       (1000) tom       (1000)       30 2023-04-24 13:03:27.000000 mimeograph-0.4.0/MANIFEST.in
+-rw-rw-r--   0 tom       (1000) tom       (1000)    22572 2023-04-24 16:21:39.763099 mimeograph-0.4.0/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)    20615 2023-04-24 13:03:27.000000 mimeograph-0.4.0/README.md
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1709 2023-04-24 16:21:01.000000 mimeograph-0.4.0/pyproject.toml
+-rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-04-24 16:21:39.763099 mimeograph-0.4.0/setup.cfg
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 16:21:39.751099 mimeograph-0.4.0/src/
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 16:21:39.755099 mimeograph-0.4.0/src/mimeo/
+-rw-rw-r--   0 tom       (1000) tom       (1000)       53 2023-04-24 16:21:01.000000 mimeograph-0.4.0/src/mimeo/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     9574 2023-04-24 16:21:01.000000 mimeograph-0.4.0/src/mimeo/__main__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 16:21:39.755099 mimeograph-0.4.0/src/mimeo/config/
+-rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-04-24 16:19:51.000000 mimeograph-0.4.0/src/mimeo/config/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      553 2023-04-24 16:19:51.000000 mimeograph-0.4.0/src/mimeo/config/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    12842 2023-04-24 16:19:51.000000 mimeograph-0.4.0/src/mimeo/config/mimeo_config.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 16:21:39.755099 mimeograph-0.4.0/src/mimeo/consumers/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      195 2023-04-24 16:19:51.000000 mimeograph-0.4.0/src/mimeo/consumers/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      353 2023-04-24 16:19:51.000000 mimeograph-0.4.0/src/mimeo/consumers/consumer.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1108 2023-04-24 16:19:51.000000 mimeograph-0.4.0/src/mimeo/consumers/consumer_factory.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      949 2023-04-24 16:19:51.000000 mimeograph-0.4.0/src/mimeo/consumers/file_consumer.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1478 2023-04-24 16:19:51.000000 mimeograph-0.4.0/src/mimeo/consumers/http_consumer.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      131 2023-04-24 16:19:51.000000 mimeograph-0.4.0/src/mimeo/consumers/raw_consumer.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 16:21:39.755099 mimeograph-0.4.0/src/mimeo/context/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      139 2023-04-20 08:22:52.000000 mimeograph-0.4.0/src/mimeo/context/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1724 2023-04-24 16:19:51.000000 mimeograph-0.4.0/src/mimeo/context/annotations.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      363 2023-04-24 16:19:51.000000 mimeograph-0.4.0/src/mimeo/context/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     6402 2023-04-24 16:19:51.000000 mimeograph-0.4.0/src/mimeo/context/mimeo_context.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1506 2023-04-24 16:19:51.000000 mimeograph-0.4.0/src/mimeo/context/mimeo_context_manager.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1025 2023-04-24 16:19:51.000000 mimeograph-0.4.0/src/mimeo/context/mimeo_iteration.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 16:21:39.755099 mimeograph-0.4.0/src/mimeo/database/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      194 2023-04-24 13:03:27.000000 mimeograph-0.4.0/src/mimeo/database/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2085 2023-04-14 09:39:06.000000 mimeograph-0.4.0/src/mimeo/database/cities.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2086 2023-04-14 09:39:06.000000 mimeograph-0.4.0/src/mimeo/database/countries.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      165 2023-04-24 13:03:27.000000 mimeograph-0.4.0/src/mimeo/database/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2101 2023-04-24 13:03:27.000000 mimeograph-0.4.0/src/mimeo/database/first_names.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      860 2023-04-24 13:03:27.000000 mimeograph-0.4.0/src/mimeo/database/last_names.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2128 2023-04-24 13:03:27.000000 mimeograph-0.4.0/src/mimeo/database/mimeo_db.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      101 2023-04-24 13:03:27.000000 mimeograph-0.4.0/src/mimeo/exc.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 16:21:39.755099 mimeograph-0.4.0/src/mimeo/generators/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      121 2023-04-20 08:22:48.000000 mimeograph-0.4.0/src/mimeo/generators/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      891 2023-04-14 09:39:06.000000 mimeograph-0.4.0/src/mimeo/generators/generator.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      680 2023-04-24 13:03:27.000000 mimeograph-0.4.0/src/mimeo/generators/generator_factory.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5677 2023-04-24 16:19:51.000000 mimeograph-0.4.0/src/mimeo/generators/xml_generator.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 16:21:39.759099 mimeograph-0.4.0/src/mimeo/logging/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      380 2023-04-20 08:22:47.000000 mimeograph-0.4.0/src/mimeo/logging/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      275 2023-03-31 04:40:40.000000 mimeograph-0.4.0/src/mimeo/logging/filters.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 16:21:39.759099 mimeograph-0.4.0/src/mimeo/meta/
+-rw-rw-r--   0 tom       (1000) tom       (1000)       39 2023-04-20 08:22:45.000000 mimeograph-0.4.0/src/mimeo/meta/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      993 2023-04-14 09:39:06.000000 mimeograph-0.4.0/src/mimeo/meta/alive.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)       44 2023-04-14 09:39:06.000000 mimeograph-0.4.0/src/mimeo/meta/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      625 2023-03-31 04:40:40.000000 mimeograph-0.4.0/src/mimeo/mimeo.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 16:21:39.759099 mimeograph-0.4.0/src/mimeo/resources/
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2023-03-31 04:40:40.000000 mimeograph-0.4.0/src/mimeo/resources/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)  1541655 2023-03-31 04:40:40.000000 mimeograph-0.4.0/src/mimeo/resources/cities.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4205 2023-03-31 04:40:40.000000 mimeograph-0.4.0/src/mimeo/resources/countries.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)       44 2023-04-24 13:03:27.000000 mimeograph-0.4.0/src/mimeo/resources/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    66313 2023-04-24 13:03:27.000000 mimeograph-0.4.0/src/mimeo/resources/forenames.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)      719 2023-03-31 04:40:40.000000 mimeograph-0.4.0/src/mimeo/resources/logging.yaml
+-rw-rw-r--   0 tom       (1000) tom       (1000)  1197769 2023-04-24 13:03:27.000000 mimeograph-0.4.0/src/mimeo/resources/surnames.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)      458 2023-04-24 13:03:27.000000 mimeograph-0.4.0/src/mimeo/tools.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 16:21:39.759099 mimeograph-0.4.0/src/mimeo/utils/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      330 2023-04-24 13:03:27.000000 mimeograph-0.4.0/src/mimeo/utils/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      132 2023-04-14 09:39:06.000000 mimeograph-0.4.0/src/mimeo/utils/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     8714 2023-04-24 16:19:51.000000 mimeograph-0.4.0/src/mimeo/utils/mimeo_utils.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     7286 2023-04-24 16:19:51.000000 mimeograph-0.4.0/src/mimeo/utils/renderer.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 16:21:39.763099 mimeograph-0.4.0/src/mimeograph.egg-info/
+-rw-rw-r--   0 tom       (1000) tom       (1000)    22572 2023-04-24 16:21:39.000000 mimeograph-0.4.0/src/mimeograph.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1774 2023-04-24 16:21:39.000000 mimeograph-0.4.0/src/mimeograph.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-04-24 16:21:39.000000 mimeograph-0.4.0/src/mimeograph.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       46 2023-04-24 16:21:39.000000 mimeograph-0.4.0/src/mimeograph.egg-info/entry_points.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       98 2023-04-24 16:21:39.000000 mimeograph-0.4.0/src/mimeograph.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        6 2023-04-24 16:21:39.000000 mimeograph-0.4.0/src/mimeograph.egg-info/top_level.txt
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 16:21:39.763099 mimeograph-0.4.0/tests/
+-rw-rw-r--   0 tom       (1000) tom       (1000)    31417 2023-04-24 13:03:27.000000 mimeograph-0.4.0/tests/test_mimeo_cli.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1833 2023-04-14 09:39:06.000000 mimeograph-0.4.0/tests/test_mimeograph.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      465 2023-04-24 13:03:27.000000 mimeograph-0.4.0/tests/test_tools.py
```

### Comparing `mimeograph-0.3.1/LICENSE` & `mimeograph-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mimeograph-0.3.1/PKG-INFO` & `mimeograph-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mimeograph
-Version: 0.3.1
+Version: 0.4.0
 Summary: Generate data based on a simple template
 Author-email: "T.A. Programming Svcs." <tomasz.maciej.aniolowski@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tomasz Aniołowski
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -585,22 +585,22 @@
 {
   "City": "{city}"
 }
 ```
 
 ###### Parametrized
 
-Uses country (name, iso2, iso3) and `allow_duplicates` flag to generate a city name.
+Uses country (name, iso2, iso3) and `unique` flag to generate a city name.
 
 ```json
 {
   "CityWithDuplicates": {
     "_mimeo_util": {
       "_name": "city",
-      "allow_duplicates": true
+      "unique": false
     }
   },
   "CityOfCountryName": {
     "_mimeo_util": {
       "_name": "city",
       "country": "United Kingdom"
     }
@@ -617,15 +617,15 @@
       "country": "GBR"
     }
   },
   "CityOfCountryWithDuplicates": {
     "_mimeo_util": {
       "_name": "city",
       "country": "United Kingdom",
-      "allow_duplicates": true
+      "unique": false
     }
   }
 }
 ```
 
 ##### Country
 
@@ -646,22 +646,22 @@
 It can generate:
 - country iso3 or iso 2 instead of name
 - country with duplicates
 - country name for a provided iso3 or iso2
 - country iso2 for a provided name or iso3
 - country iso3 for a provided name or iso2
 
-When the `country` param is provided then the `allow_duplicates` flag is ignored.
+When the `country` param is provided then the `unique` flag is ignored.
 
 ```json
 {
   "CountryNameWithDuplicates": {
     "_mimeo_util": {
       "_name": "country",
-      "allow_duplicates": true
+      "unique": false
     }
   },
   "CountryISO2": {
     "_mimeo_util": {
       "_name": "country",
       "value": "iso2"
     }
@@ -684,22 +684,101 @@
       "value": "iso2",
       "country": "United Kingdom"
     }
   }
 }
 ```
 
+##### First Name
+
+Generates a first name.
+
+###### Raw
+
+By default first names will be unique across a Mimeo Context.
+
+```json
+{
+  "FirstName": "{first_name}"
+}
+```
+
+###### Parametrized
+
+Uses sex (`M` / `Male` / `F` / `Female`) and `unique` flag to generate a first name.
+
+```json
+{
+  "FirstNameWithDuplicates": {
+    "_mimeo_util": {
+      "_name": "first_name",
+      "unique": false
+    }
+  },
+  "MaleFirstName": {
+    "_mimeo_util": {
+      "_name": "first_name",
+      "sex": "M"
+    }
+  },
+  "FemaleFirstName": {
+    "_mimeo_util": {
+      "_name": "first_name",
+      "sex": "F"
+    }
+  },
+  "MaleFirstNameWithDuplicates": {
+    "_mimeo_util": {
+      "_name": "first_name",
+      "sex": "M",
+      "unique": false
+    }
+  }
+}
+```
+
+##### Last Name
+
+Generates a last name.
+
+###### Raw
+
+By default last names will be unique across a Mimeo Context.
+
+```json
+{
+  "LastName": "{last_name}"
+}
+```
+
+###### Parametrized
+
+Uses `unique` flag to generate a last name.
+
+```json
+{
+  "LastNameWithDuplicates": {
+    "_mimeo_util": {
+      "_name": "last_name",
+      "unique": false
+    }
+  }
+}
+```
+
 
 ## License
 
 MIT
 
 
 ## Authors
 
 - [@TomaszAniolowski](https://www.github.com/TomaszAniolowski)
 
 
 ## Acknowledgements
 
  - [SimpleMaps.com](https://simplemaps.com/data/world-cities) (Cities & countries data)
+ - [@hadley/data-baby-names](https://github.com/hadley/data-baby-names/) (Forenames data)
+ - [@fivethirtyeigh/data/most-common-name](https://github.com/fivethirtyeight/data/tree/master/most-common-name) (Surnames data)
```

### Comparing `mimeograph-0.3.1/README.md` & `mimeograph-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -543,22 +543,22 @@
 {
   "City": "{city}"
 }
 ```
 
 ###### Parametrized
 
-Uses country (name, iso2, iso3) and `allow_duplicates` flag to generate a city name.
+Uses country (name, iso2, iso3) and `unique` flag to generate a city name.
 
 ```json
 {
   "CityWithDuplicates": {
     "_mimeo_util": {
       "_name": "city",
-      "allow_duplicates": true
+      "unique": false
     }
   },
   "CityOfCountryName": {
     "_mimeo_util": {
       "_name": "city",
       "country": "United Kingdom"
     }
@@ -575,15 +575,15 @@
       "country": "GBR"
     }
   },
   "CityOfCountryWithDuplicates": {
     "_mimeo_util": {
       "_name": "city",
       "country": "United Kingdom",
-      "allow_duplicates": true
+      "unique": false
     }
   }
 }
 ```
 
 ##### Country
 
@@ -604,22 +604,22 @@
 It can generate:
 - country iso3 or iso 2 instead of name
 - country with duplicates
 - country name for a provided iso3 or iso2
 - country iso2 for a provided name or iso3
 - country iso3 for a provided name or iso2
 
-When the `country` param is provided then the `allow_duplicates` flag is ignored.
+When the `country` param is provided then the `unique` flag is ignored.
 
 ```json
 {
   "CountryNameWithDuplicates": {
     "_mimeo_util": {
       "_name": "country",
-      "allow_duplicates": true
+      "unique": false
     }
   },
   "CountryISO2": {
     "_mimeo_util": {
       "_name": "country",
       "value": "iso2"
     }
@@ -642,22 +642,101 @@
       "value": "iso2",
       "country": "United Kingdom"
     }
   }
 }
 ```
 
+##### First Name
+
+Generates a first name.
+
+###### Raw
+
+By default first names will be unique across a Mimeo Context.
+
+```json
+{
+  "FirstName": "{first_name}"
+}
+```
+
+###### Parametrized
+
+Uses sex (`M` / `Male` / `F` / `Female`) and `unique` flag to generate a first name.
+
+```json
+{
+  "FirstNameWithDuplicates": {
+    "_mimeo_util": {
+      "_name": "first_name",
+      "unique": false
+    }
+  },
+  "MaleFirstName": {
+    "_mimeo_util": {
+      "_name": "first_name",
+      "sex": "M"
+    }
+  },
+  "FemaleFirstName": {
+    "_mimeo_util": {
+      "_name": "first_name",
+      "sex": "F"
+    }
+  },
+  "MaleFirstNameWithDuplicates": {
+    "_mimeo_util": {
+      "_name": "first_name",
+      "sex": "M",
+      "unique": false
+    }
+  }
+}
+```
+
+##### Last Name
+
+Generates a last name.
+
+###### Raw
+
+By default last names will be unique across a Mimeo Context.
+
+```json
+{
+  "LastName": "{last_name}"
+}
+```
+
+###### Parametrized
+
+Uses `unique` flag to generate a last name.
+
+```json
+{
+  "LastNameWithDuplicates": {
+    "_mimeo_util": {
+      "_name": "last_name",
+      "unique": false
+    }
+  }
+}
+```
+
 
 ## License
 
 MIT
 
 
 ## Authors
 
 - [@TomaszAniolowski](https://www.github.com/TomaszAniolowski)
 
 
 ## Acknowledgements
 
  - [SimpleMaps.com](https://simplemaps.com/data/world-cities) (Cities & countries data)
+ - [@hadley/data-baby-names](https://github.com/hadley/data-baby-names/) (Forenames data)
+ - [@fivethirtyeigh/data/most-common-name](https://github.com/fivethirtyeight/data/tree/master/most-common-name) (Surnames data)
```

### Comparing `mimeograph-0.3.1/pyproject.toml` & `mimeograph-0.4.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mimeograph"
-version = "0.3.1"
+version = "0.4.0"
 description = "Generate data based on a simple template"
 readme = "README.md"
 authors = [{ name = "T.A. Programming Svcs.", email = "tomasz.maciej.aniolowski@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Development Status :: 4 - Beta",
@@ -26,24 +26,39 @@
     "pandas",
     "pyyaml",
     "haggis"
 ]
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
-dev = ["bumpver", "build", "twine", "isort", "pytest", "pytest-cov", "responses"]
+dev = ["bumpver", "build", "twine", "pylama", "isort", "pytest", "pytest-cov", "responses"]
 
 [project.scripts]
 mimeo = "mimeo.__main__:main"
 
 [tool.bumpver]
-current_version = "0.3.1"
+current_version = "0.4.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} to {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
 "src/mimeo/__init__.py" = ["{version}"]
-"src/mimeo/__main__.py" = ["{version}"]
+"src/mimeo/__main__.py" = ["{version}"]
+
+[tool.pylama]
+async = true
+linters = "mccabe,pycodestyle,pydocstyle,pyflakes"
+
+[tool.pylama.linter.pydocstyle]
+convention = "numpy"
+
+[[tool.pylama.files]]
+path = "*/__init__.py"
+ignore = "W0611"
+
+[[tool.pylama.files]]
+path = "tests/*"
+linters = "mccabe,pycodestyle,pyflakes"
```

### Comparing `mimeograph-0.3.1/src/mimeo/__main__.py` & `mimeograph-0.4.0/src/mimeo/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 from argparse import ArgumentParser
 from os import path, walk
 
 from mimeo import Mimeograph
 from mimeo.config import MimeoConfig
 from mimeo.context import MimeoContextManager
-from mimeo.exceptions import EnvironmentNotFound, EnvironmentsFileNotFound
+from mimeo.exc import EnvironmentNotFound, EnvironmentsFileNotFound
 from mimeo.logging import setup_logging
 
 setup_logging()
 logger = logging.getLogger(__name__)
 
 DEFAULT_ENVS_FILE_PATH = "mimeo.envs.json"
 
@@ -21,15 +21,15 @@
         super().__init__(
             prog="mimeo",
             description="Generate data based on a template")
         self.add_argument(
             "-v",
             "--version",
             action="version",
-            version="%(prog)s v0.3.1")
+            version="%(prog)s v0.4.0")
         self.add_argument(
             "paths",
             nargs="+",
             type=str,
             help="take paths to Mimeo Configurations")
 
         mimeo_config_args = self.add_argument_group("Mimeo Configuration arguments")
@@ -186,47 +186,47 @@
         if args.output is not None:
             customize_output_details(config, MimeoConfig.OUTPUT_DETAILS_DIRECTION_KEY, args.output)
         if args.directory is not None:
             customize_output_details(config, MimeoConfig.OUTPUT_DETAILS_DIRECTORY_PATH_KEY, args.directory)
         if args.file is not None:
             customize_output_details(config, MimeoConfig.OUTPUT_DETAILS_FILE_NAME_KEY, args.file)
         if args.http_method is not None:
-            customize_output_details(config, MimeoConfig.OUTPUT_DETAILS_METHOD, args.http_method)
+            customize_output_details(config, MimeoConfig.OUTPUT_DETAILS_METHOD_KEY, args.http_method)
         if args.http_protocol is not None:
-            customize_output_details(config, MimeoConfig.OUTPUT_DETAILS_PROTOCOL, args.http_protocol)
+            customize_output_details(config, MimeoConfig.OUTPUT_DETAILS_PROTOCOL_KEY, args.http_protocol)
         if args.http_auth is not None:
-            customize_output_details(config, MimeoConfig.OUTPUT_DETAILS_AUTH, args.http_auth)
+            customize_output_details(config, MimeoConfig.OUTPUT_DETAILS_AUTH_KEY, args.http_auth)
         if args.http_host is not None:
-            customize_output_details(config, MimeoConfig.OUTPUT_DETAILS_HOST, args.http_host)
+            customize_output_details(config, MimeoConfig.OUTPUT_DETAILS_HOST_KEY, args.http_host)
         if args.http_port is not None:
-            customize_output_details(config, MimeoConfig.OUTPUT_DETAILS_PORT, args.http_port)
+            customize_output_details(config, MimeoConfig.OUTPUT_DETAILS_PORT_KEY, args.http_port)
         if args.http_endpoint is not None:
-            customize_output_details(config, MimeoConfig.OUTPUT_DETAILS_ENDPOINT, args.http_endpoint)
+            customize_output_details(config, MimeoConfig.OUTPUT_DETAILS_ENDPOINT_KEY, args.http_endpoint)
         if args.http_user is not None:
-            customize_output_details(config, MimeoConfig.OUTPUT_DETAILS_USERNAME, args.http_user)
+            customize_output_details(config, MimeoConfig.OUTPUT_DETAILS_USERNAME_KEY, args.http_user)
         if args.http_password is not None:
-            customize_output_details(config, MimeoConfig.OUTPUT_DETAILS_PASSWORD, args.http_password)
+            customize_output_details(config, MimeoConfig.OUTPUT_DETAILS_PASSWORD_KEY, args.http_password)
     mimeo_config = MimeoConfig(config)
     logger.debug(f"Mimeo Config: {mimeo_config}")
     return mimeo_config
 
 
 def customize_output_details_with_env(config, envs_path, env_name):
     if path.exists(envs_path):
         with open(envs_path) as envs_file:
             envs = json.load(envs_file)
             if env_name in envs:
                 env = envs[env_name]
                 logger.debug(f"Using environment [{env_name}] from file [{envs_path}]: [{env}]")
-                for prop in [MimeoConfig.OUTPUT_DETAILS_PROTOCOL,
-                             MimeoConfig.OUTPUT_DETAILS_HOST,
-                             MimeoConfig.OUTPUT_DETAILS_PORT,
-                             MimeoConfig.OUTPUT_DETAILS_AUTH,
-                             MimeoConfig.OUTPUT_DETAILS_USERNAME,
-                             MimeoConfig.OUTPUT_DETAILS_PASSWORD]:
+                for prop in [MimeoConfig.OUTPUT_DETAILS_PROTOCOL_KEY,
+                             MimeoConfig.OUTPUT_DETAILS_HOST_KEY,
+                             MimeoConfig.OUTPUT_DETAILS_PORT_KEY,
+                             MimeoConfig.OUTPUT_DETAILS_AUTH_KEY,
+                             MimeoConfig.OUTPUT_DETAILS_USERNAME_KEY,
+                             MimeoConfig.OUTPUT_DETAILS_PASSWORD_KEY]:
                     prop_value = env.get(prop)
                     if prop_value is not None:
                         customize_output_details(config, prop, prop_value)
             else:
                 raise EnvironmentNotFound(f"No such env [{env_name}] in environments file [{envs_path}]")
     else:
         raise EnvironmentsFileNotFound(f"Environments file not found [{envs_path}]")
```

### Comparing `mimeograph-0.3.1/src/mimeo/config/mimeo_config.py` & `mimeograph-0.4.0/src/mimeo/config/mimeo_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import re
 
-from mimeo.exceptions import (IncorrectMimeoConfig, IncorrectMimeoModel,
+from mimeo.config.exc import (IncorrectMimeoConfig, IncorrectMimeoModel,
                               IncorrectMimeoTemplate, InvalidIndent,
                               InvalidVars, MissingRequiredProperty,
-                              UnsupportedAuthMethod,
-                              UnsupportedOutputDirection,
-                              UnsupportedOutputFormat,
-                              UnsupportedRequestMethod)
+                              UnsupportedPropertyValue)
 from mimeo.logging import setup_logging
 
 setup_logging()
 
 
 class MimeoDTO:
 
@@ -24,52 +21,78 @@
 class MimeoConfig(MimeoDTO):
 
     OUTPUT_FORMAT_KEY = "output_format"
     OUTPUT_DETAILS_KEY = "output_details"
     OUTPUT_DETAILS_DIRECTION_KEY = "direction"
     OUTPUT_DETAILS_DIRECTORY_PATH_KEY = "directory_path"
     OUTPUT_DETAILS_FILE_NAME_KEY = "file_name"
-    OUTPUT_DETAILS_METHOD = "method"
-    OUTPUT_DETAILS_PROTOCOL = "protocol"
-    OUTPUT_DETAILS_HOST = "host"
-    OUTPUT_DETAILS_PORT = "port"
-    OUTPUT_DETAILS_ENDPOINT = "endpoint"
-    OUTPUT_DETAILS_AUTH = "auth"
-    OUTPUT_DETAILS_USERNAME = "username"
-    OUTPUT_DETAILS_PASSWORD = "password"
+    OUTPUT_DETAILS_METHOD_KEY = "method"
+    OUTPUT_DETAILS_PROTOCOL_KEY = "protocol"
+    OUTPUT_DETAILS_HOST_KEY = "host"
+    OUTPUT_DETAILS_PORT_KEY = "port"
+    OUTPUT_DETAILS_ENDPOINT_KEY = "endpoint"
+    OUTPUT_DETAILS_AUTH_KEY = "auth"
+    OUTPUT_DETAILS_USERNAME_KEY = "username"
+    OUTPUT_DETAILS_PASSWORD_KEY = "password"
     XML_DECLARATION_KEY = "xml_declaration"
     INDENT_KEY = "indent"
     VARS_KEY = "vars"
     TEMPLATES_KEY = "_templates_"
     TEMPLATES_COUNT_KEY = "count"
     TEMPLATES_MODEL_KEY = "model"
     MODEL_CONTEXT_KEY = "context"
     MODEL_ATTRIBUTES_KEY = "_attrs"
     MODEL_VALUE_KEY = "_value"
     MODEL_MIMEO_UTIL_KEY = "_mimeo_util"
     MODEL_MIMEO_UTIL_NAME_KEY = "_name"
 
-    SUPPORTED_OUTPUT_FORMATS = ("xml",)
+    OUTPUT_FORMAT_XML = "xml"
+
+    OUTPUT_DETAILS_DIRECTION_FILE = "file"
+    OUTPUT_DETAILS_DIRECTION_STD_OUT = "stdout"
+    OUTPUT_DETAILS_DIRECTION_HTTP = "http"
+
+    OUTPUT_DETAILS_DIRECTION_HTTP_REQUEST_POST = "POST"
+    OUTPUT_DETAILS_DIRECTION_HTTP_REQUEST_PUT = "PUT"
+
+    OUTPUT_DETAILS_DIRECTION_HTTP_AUTH_BASIC = "basic"
+    OUTPUT_DETAILS_DIRECTION_HTTP_AUTH_DIGEST = "digest"
+
+    SUPPORTED_OUTPUT_FORMATS = (OUTPUT_FORMAT_XML,)
+
+    SUPPORTED_OUTPUT_DIRECTIONS = (OUTPUT_DETAILS_DIRECTION_STD_OUT,
+                                   OUTPUT_DETAILS_DIRECTION_FILE,
+                                   OUTPUT_DETAILS_DIRECTION_HTTP)
+    SUPPORTED_REQUEST_METHODS = (OUTPUT_DETAILS_DIRECTION_HTTP_REQUEST_POST,
+                                 OUTPUT_DETAILS_DIRECTION_HTTP_REQUEST_PUT)
+    SUPPORTED_AUTH_METHODS = (OUTPUT_DETAILS_DIRECTION_HTTP_AUTH_BASIC,
+                              OUTPUT_DETAILS_DIRECTION_HTTP_AUTH_DIGEST)
+    REQUIRED_HTTP_DETAILS = (OUTPUT_DETAILS_HOST_KEY,
+                             OUTPUT_DETAILS_ENDPOINT_KEY,
+                             OUTPUT_DETAILS_USERNAME_KEY,
+                             OUTPUT_DETAILS_PASSWORD_KEY)
 
     def __init__(self, config: dict):
         super().__init__(config)
         self.output_format = MimeoConfig.__get_output_format(config)
         self.output_details = MimeoOutputDetails(self.output_format, config.get(self.OUTPUT_DETAILS_KEY, {}))
         self.xml_declaration = config.get(self.XML_DECLARATION_KEY, False)
         self.indent = MimeoConfig.__get_indent(config)
         self.vars = MimeoConfig.__get_vars(config)
         self.templates = MimeoConfig.__get_templates(config)
 
     @staticmethod
     def __get_output_format(config):
-        output_format = config.get(MimeoConfig.OUTPUT_FORMAT_KEY, "xml")
+        output_format = config.get(MimeoConfig.OUTPUT_FORMAT_KEY, MimeoConfig.OUTPUT_FORMAT_XML)
         if output_format in MimeoConfig.SUPPORTED_OUTPUT_FORMATS:
             return output_format
         else:
-            raise UnsupportedOutputFormat(f"Provided format [{output_format}] is not supported!")
+            raise UnsupportedPropertyValue(MimeoConfig.OUTPUT_FORMAT_KEY,
+                                           output_format,
+                                           MimeoConfig.SUPPORTED_OUTPUT_FORMATS)
 
     @staticmethod
     def __get_indent(config):
         indent = config.get(MimeoConfig.INDENT_KEY, 0)
         if indent >= 0:
             return indent
         else:
@@ -101,32 +124,14 @@
     @staticmethod
     def __is_mimeo_util_object(obj: dict):
         return isinstance(obj, dict) and len(obj) == 1 and MimeoConfig.MODEL_MIMEO_UTIL_KEY in obj
 
 
 class MimeoOutputDetails(MimeoDTO):
 
-    FILE_DIRECTION = "file"
-    STD_OUT_DIRECTION = "stdout"
-    HTTP_DIRECTION = "http"
-
-    REQUEST_POST = "POST"
-    REQUEST_PUT = "PUT"
-
-    AUTH_BASIC = "basic"
-    AUTH_DIGEST = "digest"
-
-    SUPPORTED_OUTPUT_DIRECTIONS = (STD_OUT_DIRECTION, FILE_DIRECTION, HTTP_DIRECTION)
-    SUPPORTED_REQUEST_METHODS = (REQUEST_POST, REQUEST_PUT)
-    SUPPORTED_AUTH_METHODS = (AUTH_BASIC, AUTH_DIGEST)
-    REQUIRED_HTTP_DETAILS = (MimeoConfig.OUTPUT_DETAILS_HOST,
-                             MimeoConfig.OUTPUT_DETAILS_ENDPOINT,
-                             MimeoConfig.OUTPUT_DETAILS_USERNAME,
-                             MimeoConfig.OUTPUT_DETAILS_PASSWORD)
-
     def __init__(self, output_format: str, output_details: dict):
         super().__init__(output_details)
         self.direction = MimeoOutputDetails.__get_direction(output_details)
         MimeoOutputDetails.__validate_output_details(self.direction, output_details)
         self.directory_path = MimeoOutputDetails.__get_directory_path(self.direction, output_details)
         self.file_name_tmplt = MimeoOutputDetails.__get_file_name_tmplt(self.direction, output_details, output_format)
         self.method = MimeoOutputDetails.__get_method(self.direction, output_details)
@@ -136,89 +141,99 @@
         self.endpoint = MimeoOutputDetails.__get_endpoint(self.direction, output_details)
         self.auth = MimeoOutputDetails.__get_auth(self.direction, output_details)
         self.username = MimeoOutputDetails.__get_username(self.direction, output_details)
         self.password = MimeoOutputDetails.__get_password(self.direction, output_details)
 
     @staticmethod
     def __get_direction(output_details):
-        direction = output_details.get(MimeoConfig.OUTPUT_DETAILS_DIRECTION_KEY, MimeoOutputDetails.FILE_DIRECTION)
-        if direction in MimeoOutputDetails.SUPPORTED_OUTPUT_DIRECTIONS:
+        direction = output_details.get(MimeoConfig.OUTPUT_DETAILS_DIRECTION_KEY,
+                                       MimeoConfig.OUTPUT_DETAILS_DIRECTION_FILE)
+        if direction in MimeoConfig.SUPPORTED_OUTPUT_DIRECTIONS:
             return direction
         else:
-            raise UnsupportedOutputDirection(f"Provided direction [{direction}] is not supported!")
+            raise UnsupportedPropertyValue(MimeoConfig.OUTPUT_DETAILS_DIRECTION_KEY,
+                                           direction,
+                                           MimeoConfig.SUPPORTED_OUTPUT_DIRECTIONS)
 
     @staticmethod
     def __validate_output_details(direction: str, output_details: dict):
-        if direction == MimeoOutputDetails.HTTP_DIRECTION:
+        if direction == MimeoConfig.OUTPUT_DETAILS_DIRECTION_HTTP:
             missing_details = []
-            for detail in MimeoOutputDetails.REQUIRED_HTTP_DETAILS:
+            for detail in MimeoConfig.REQUIRED_HTTP_DETAILS:
                 if detail not in output_details:
                     missing_details.append(detail)
             if len(missing_details) > 0:
                 missing_details_str = ', '.join(missing_details)
                 raise MissingRequiredProperty(f"Missing required fields is HTTP output details: {missing_details_str}")
 
     @staticmethod
     def __get_directory_path(direction: str, output_details: dict):
-        if direction == MimeoOutputDetails.FILE_DIRECTION:
+        if direction == MimeoConfig.OUTPUT_DETAILS_DIRECTION_FILE:
             return output_details.get(MimeoConfig.OUTPUT_DETAILS_DIRECTORY_PATH_KEY, "mimeo-output")
 
     @staticmethod
     def __get_file_name_tmplt(direction: str, output_details: dict, output_format: str):
-        if direction == MimeoOutputDetails.FILE_DIRECTION:
+        if direction == MimeoConfig.OUTPUT_DETAILS_DIRECTION_FILE:
             file_name = output_details.get(MimeoConfig.OUTPUT_DETAILS_FILE_NAME_KEY, "mimeo-output")
             return f"{file_name}-{'{}'}.{output_format}"
 
     @staticmethod
     def __get_method(direction: str, output_details: dict):
-        if direction == MimeoOutputDetails.HTTP_DIRECTION:
-            method = output_details.get(MimeoConfig.OUTPUT_DETAILS_METHOD, "POST")
-            if method in MimeoOutputDetails.SUPPORTED_REQUEST_METHODS:
+        if direction == MimeoConfig.OUTPUT_DETAILS_DIRECTION_HTTP:
+            method = output_details.get(MimeoConfig.OUTPUT_DETAILS_METHOD_KEY,
+                                        MimeoConfig.OUTPUT_DETAILS_DIRECTION_HTTP_REQUEST_POST)
+            if method in MimeoConfig.SUPPORTED_REQUEST_METHODS:
                 return method
             else:
-                raise UnsupportedRequestMethod(f"Provided request method [{method}] is not supported!")
+                raise UnsupportedPropertyValue(MimeoConfig.OUTPUT_DETAILS_METHOD_KEY,
+                                               method,
+                                               MimeoConfig.SUPPORTED_REQUEST_METHODS)
 
     @staticmethod
     def __get_protocol(direction: str, output_details: dict):
-        if direction == MimeoOutputDetails.HTTP_DIRECTION:
-            return output_details.get(MimeoConfig.OUTPUT_DETAILS_PROTOCOL, "http")
+        if direction == MimeoConfig.OUTPUT_DETAILS_DIRECTION_HTTP:
+            return output_details.get(MimeoConfig.OUTPUT_DETAILS_PROTOCOL_KEY,
+                                      MimeoConfig.OUTPUT_DETAILS_DIRECTION_HTTP)
 
     @staticmethod
     def __get_host(direction: str, output_details: dict):
-        if direction == MimeoOutputDetails.HTTP_DIRECTION:
-            return output_details.get(MimeoConfig.OUTPUT_DETAILS_HOST)
+        if direction == MimeoConfig.OUTPUT_DETAILS_DIRECTION_HTTP:
+            return output_details.get(MimeoConfig.OUTPUT_DETAILS_HOST_KEY)
 
     @staticmethod
     def __get_port(direction: str, output_details: dict):
-        if direction == MimeoOutputDetails.HTTP_DIRECTION:
-            return output_details.get(MimeoConfig.OUTPUT_DETAILS_PORT)
+        if direction == MimeoConfig.OUTPUT_DETAILS_DIRECTION_HTTP:
+            return output_details.get(MimeoConfig.OUTPUT_DETAILS_PORT_KEY)
 
     @staticmethod
     def __get_endpoint(direction: str, output_details: dict):
-        if direction == MimeoOutputDetails.HTTP_DIRECTION:
-            return output_details.get(MimeoConfig.OUTPUT_DETAILS_ENDPOINT)
+        if direction == MimeoConfig.OUTPUT_DETAILS_DIRECTION_HTTP:
+            return output_details.get(MimeoConfig.OUTPUT_DETAILS_ENDPOINT_KEY)
 
     @staticmethod
     def __get_auth(direction: str, output_details: dict):
-        if direction == MimeoOutputDetails.HTTP_DIRECTION:
-            auth =  output_details.get(MimeoConfig.OUTPUT_DETAILS_AUTH, "basic")
-            if auth in MimeoOutputDetails.SUPPORTED_AUTH_METHODS:
+        if direction == MimeoConfig.OUTPUT_DETAILS_DIRECTION_HTTP:
+            auth =  output_details.get(MimeoConfig.OUTPUT_DETAILS_AUTH_KEY,
+                                       MimeoConfig.OUTPUT_DETAILS_DIRECTION_HTTP_AUTH_BASIC)
+            if auth in MimeoConfig.SUPPORTED_AUTH_METHODS:
                 return auth
             else:
-                raise UnsupportedAuthMethod(f"Provided auth [{auth}] is not supported!")
+                raise UnsupportedPropertyValue(MimeoConfig.OUTPUT_DETAILS_AUTH_KEY,
+                                               auth,
+                                               MimeoConfig.SUPPORTED_AUTH_METHODS)
 
     @staticmethod
     def __get_username(direction: str, output_details: dict):
-        if direction == MimeoOutputDetails.HTTP_DIRECTION:
-            return output_details.get(MimeoConfig.OUTPUT_DETAILS_USERNAME)
+        if direction == MimeoConfig.OUTPUT_DETAILS_DIRECTION_HTTP:
+            return output_details.get(MimeoConfig.OUTPUT_DETAILS_USERNAME_KEY)
 
     @staticmethod
     def __get_password(direction: str, output_details: dict):
-        if direction == MimeoOutputDetails.HTTP_DIRECTION:
-            return output_details.get(MimeoConfig.OUTPUT_DETAILS_PASSWORD)
+        if direction == MimeoConfig.OUTPUT_DETAILS_DIRECTION_HTTP:
+            return output_details.get(MimeoConfig.OUTPUT_DETAILS_PASSWORD_KEY)
 
 
 class MimeoTemplate(MimeoDTO):
 
     def __init__(self, template: dict):
         super().__init__(template)
         MimeoTemplate.__validate_template(template)
```

### Comparing `mimeograph-0.3.1/src/mimeo/consumers/file_consumer.py` & `mimeograph-0.4.0/src/mimeo/consumers/file_consumer.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.3.1/src/mimeo/consumers/http_consumer.py` & `mimeograph-0.4.0/src/mimeo/consumers/http_consumer.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.3.1/src/mimeo/context/annotations.py` & `mimeograph-0.4.0/src/mimeo/context/annotations.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.3.1/src/mimeo/context/mimeo_context_manager.py` & `mimeograph-0.4.0/src/mimeo/context/mimeo_context_manager.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.3.1/src/mimeo/context/mimeo_iteration.py` & `mimeograph-0.4.0/src/mimeo/context/mimeo_iteration.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.3.1/src/mimeo/database/cities.py` & `mimeograph-0.4.0/src/mimeo/database/cities.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.3.1/src/mimeo/database/countries.py` & `mimeograph-0.4.0/src/mimeo/database/countries.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.3.1/src/mimeo/database/mimeo_db.py` & `mimeograph-0.4.0/src/mimeo/database/mimeo_db.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,23 @@
-from mimeo.database import CitiesDB, City, CountriesDB, Country
+from mimeo.database import (CitiesDB, City, CountriesDB, Country, FirstName,
+                            FirstNamesDB, LastNamesDB)
 
 
 class MimeoDB:
 
     NUM_OF_CITIES = CitiesDB.NUM_OF_RECORDS
     NUM_OF_COUNTRIES = CountriesDB.NUM_OF_RECORDS
+    NUM_OF_FIRST_NAMES = FirstNamesDB.NUM_OF_RECORDS
+    NUM_OF_LAST_NAMES = LastNamesDB.NUM_OF_RECORDS
 
     def __init__(self):
         self.__cities_db = CitiesDB()
         self.__countries_db = CountriesDB()
+        self.__first_names_db = FirstNamesDB()
+        self.__last_names_db = LastNamesDB()
 
     def get_cities(self) -> list:
         return self.__cities_db.get_cities()
 
     def get_city_at(self, index: int) -> City:
         return self.__cities_db.get_city_at(index)
 
@@ -33,7 +38,22 @@
         return self.__countries_db.get_country_by_iso_3(iso_3)
 
     def get_country_by_iso_2(self, iso_2: str) -> Country:
         return self.__countries_db.get_country_by_iso_2(iso_2)
 
     def get_country_by_name(self, name: str) -> Country:
         return self.__countries_db.get_country_by_name(name)
+
+    def get_first_names(self) -> list:
+        return self.__first_names_db.get_first_names()
+
+    def get_first_name_at(self, index: int) -> FirstName:
+        return self.__first_names_db.get_first_name_at(index)
+
+    def get_first_names_by_sex(self, sex: str) -> list:
+        return self.__first_names_db.get_first_names_by_sex(sex)
+
+    def get_last_names(self) -> list:
+        return self.__last_names_db.get_last_names()
+
+    def get_last_name_at(self, index: int) -> FirstName:
+        return self.__last_names_db.get_last_name_at(index)
```

### Comparing `mimeograph-0.3.1/src/mimeo/generators/generator.py` & `mimeograph-0.4.0/src/mimeo/generators/generator.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.3.1/src/mimeo/generators/xml_generator.py` & `mimeograph-0.4.0/src/mimeo/generators/xml_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,18 +97,17 @@
                     for child in element_value:
                         grand_child_tag = next(iter(child))
                         grand_child_data = child[grand_child_tag]
                         cls._process_node(element, grand_child_tag, grand_child_data)
             else:
                 value = MimeoRenderer.render(element_value)
                 if is_special_field:
-                    context.curr_iteration().add_special_field(element_tag,
-                                                                                                 value)
+                    context.curr_iteration().add_special_field(element_tag, value)
 
-                value_str = str(value)
+                value_str = str(value) if value is not None else ""
                 element.text = value_str.lower() if isinstance(value, bool) else value_str
                 logger.fine(f"Rendered value [{element.text}]")
 
             if parent is None:
                 return element
 
     @classmethod
```

### Comparing `mimeograph-0.3.1/src/mimeo/meta/alive.py` & `mimeograph-0.4.0/src/mimeo/meta/alive.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.3.1/src/mimeo/mimeo.py` & `mimeograph-0.4.0/src/mimeo/mimeo.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.3.1/src/mimeo/resources/cities.csv` & `mimeograph-0.4.0/src/mimeo/resources/cities.csv`

 * *Files identical despite different names*

### Comparing `mimeograph-0.3.1/src/mimeo/resources/countries.csv` & `mimeograph-0.4.0/src/mimeo/resources/countries.csv`

 * *Files identical despite different names*

### Comparing `mimeograph-0.3.1/src/mimeo/resources/logging.yaml` & `mimeograph-0.4.0/src/mimeo/resources/logging.yaml`

 * *Files identical despite different names*

### Comparing `mimeograph-0.3.1/src/mimeo/utils/mimeo_utils.py` & `mimeograph-0.4.0/src/mimeo/utils/mimeo_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import string
 from abc import ABCMeta, abstractmethod
 from datetime import date, datetime, timedelta
 
 from mimeo.context import MimeoContext, MimeoContextManager
 from mimeo.context.annotations import mimeo_context
 from mimeo.database import Country, MimeoDB
-from mimeo.database.exc import CountryNotFound
+from mimeo.database.exc import CountryNotFound, InvalidSex
 from mimeo.utils.exc import InvalidValue
 
 
 class MimeoUtil(metaclass=ABCMeta):
 
     @classmethod
     def __subclasshook__(cls, subclass):
@@ -137,35 +137,35 @@
 
 class CityUtil(MimeoUtil):
 
     KEY = "city"
     __MIMEO_DB = MimeoDB()
 
     def __init__(self, **kwargs):
-        self.__allow_duplicates = kwargs.get("allow_duplicates", False)
+        self.__unique = kwargs.get("unique", True)
         self.__country = kwargs.get("country", None)
 
     @mimeo_context
     def render(self, context: MimeoContext = None):
         if self.__country is None:
-            if self.__allow_duplicates:
-                index = random.randrange(MimeoDB.NUM_OF_CITIES)
-            else:
+            if self.__unique:
                 index = context.next_city_index()
+            else:
+                index = random.randrange(MimeoDB.NUM_OF_CITIES)
             city = self.__MIMEO_DB.get_city_at(index)
         else:
             country_cities = self.__MIMEO_DB.get_cities_of(self.__country)
             country_cities_count = len(country_cities)
             if country_cities_count == 0:
                 raise CountryNotFound(f"Mimeo database does not contain any cities of provided country [{self.__country}].")
 
-            if self.__allow_duplicates:
-                index = random.randrange(country_cities_count)
-            else:
+            if self.__unique:
                 index = context.next_city_index(self.__country)
+            else:
+                index = random.randrange(country_cities_count)
             city = country_cities[index]
 
         return city.name_ascii
 
 
 class CountryUtil(MimeoUtil):
 
@@ -174,15 +174,15 @@
     __VALUE_NAME = "name"
     __VALUE_ISO3 = "iso3"
     __VALUE_ISO2 = "iso2"
     __MIMEO_DB = MimeoDB()
 
     def __init__(self, **kwargs):
         self.__value = kwargs.get("value", self.__VALUE_NAME)
-        self.__allow_duplicates = kwargs.get("allow_duplicates", False)
+        self.__unique = kwargs.get("unique", True)
         self.__country = kwargs.get("country", None)
 
     @mimeo_context
     def render(self, context: MimeoContext = None):
         if self.__value == self.__VALUE_NAME:
             return self.__get_country(context).name
         elif self.__value == self.__VALUE_ISO3:
@@ -199,14 +199,74 @@
             countries = self.__MIMEO_DB.get_countries()
             country_found = next(filter(lambda c: self.__country in [c.name, c.iso_3, c.iso_2], countries), None)
             if country_found is not None:
                 return country_found
             else:
                 raise CountryNotFound(f"Mimeo database does not contain such a country [{self.__country}].")
         else:
-            if self.__allow_duplicates:
-                index = random.randrange(MimeoDB.NUM_OF_COUNTRIES)
-            else:
+            if self.__unique:
                 index = context.next_country_index()
+            else:
+                index = random.randrange(MimeoDB.NUM_OF_COUNTRIES)
 
             country = self.__MIMEO_DB.get_country_at(index)
             return country
+
+
+class FirstNameUtil(MimeoUtil):
+
+    KEY = "first_name"
+    __MIMEO_DB = MimeoDB()
+
+    def __init__(self, **kwargs):
+        self.__unique = kwargs.get("unique", True)
+        self.__sex = self._standardize_sex(kwargs.get("sex"))
+
+    @mimeo_context
+    def render(self, context: MimeoContext = None):
+        if self.__sex is None:
+            if self.__unique:
+                index = context.next_first_name_index()
+            else:
+                index = random.randrange(MimeoDB.NUM_OF_FIRST_NAMES)
+            first_name = self.__MIMEO_DB.get_first_name_at(index)
+        else:
+            first_name_for_sex = self.__MIMEO_DB.get_first_names_by_sex(self.__sex)
+            first_name_for_sex_count = len(first_name_for_sex)
+
+            if self.__unique:
+                index = context.next_first_name_index(self.__sex)
+            else:
+                index = random.randrange(first_name_for_sex_count)
+            first_name = first_name_for_sex[index]
+
+        return first_name.name
+
+    @classmethod
+    def _standardize_sex(cls, sex: str):
+        if sex is None:
+            return sex
+        elif sex.upper() in ["M", "MALE"]:
+            return "M"
+        elif sex.upper() in ["F", "FEMALE"]:
+            return "F"
+        else:
+            raise InvalidSex("Invalid sex (use M, F, Male or Female)!")
+
+
+class LastNameUtil(MimeoUtil):
+
+    KEY = "last_name"
+    __MIMEO_DB = MimeoDB()
+
+    def __init__(self, **kwargs):
+        self.__unique = kwargs.get("unique", True)
+
+    @mimeo_context
+    def render(self, context: MimeoContext = None):
+        if self.__unique:
+            index = context.next_first_name_index()
+        else:
+            index = random.randrange(MimeoDB.NUM_OF_FIRST_NAMES)
+        last_name = self.__MIMEO_DB.get_last_name_at(index)
+
+        return last_name
```

### Comparing `mimeograph-0.3.1/src/mimeo/utils/renderer.py` & `mimeograph-0.4.0/src/mimeo/utils/renderer.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import re
 
 from mimeo.config import MimeoConfig
 from mimeo.context import MimeoContext, MimeoContextManager
 from mimeo.context.annotations import mimeo_context
 from mimeo.context.exc import VarNotFound
 from mimeo.utils import (AutoIncrementUtil, CityUtil, CountryUtil,
-                         CurrentIterationUtil, DateTimeUtil, DateUtil, KeyUtil,
-                         MimeoUtil, RandomIntegerUtil, RandomItemUtil,
-                         RandomStringUtil)
+                         CurrentIterationUtil, DateTimeUtil, DateUtil,
+                         FirstNameUtil, KeyUtil, LastNameUtil, MimeoUtil,
+                         RandomIntegerUtil, RandomItemUtil, RandomStringUtil)
 from mimeo.utils.exc import InvalidMimeoUtil, InvalidValue, NotASpecialField
 
 logger = logging.getLogger(__name__)
 
 
 class UtilsRenderer:
 
@@ -24,23 +24,26 @@
         DateUtil.KEY: DateUtil,
         DateTimeUtil.KEY: DateTimeUtil,
         AutoIncrementUtil.KEY: AutoIncrementUtil,
         CurrentIterationUtil.KEY: CurrentIterationUtil,
         KeyUtil.KEY: KeyUtil,
         CityUtil.KEY: CityUtil,
         CountryUtil.KEY: CountryUtil,
+        FirstNameUtil.KEY: FirstNameUtil,
+        LastNameUtil.KEY: LastNameUtil,
     }
     _INSTANCES = {}
 
     @classmethod
     def render_raw(cls, mimeo_util_key: str):
         return cls.render_parametrized({MimeoConfig.MODEL_MIMEO_UTIL_NAME_KEY: mimeo_util_key})
 
     @classmethod
     def render_parametrized(cls, mimeo_util_config: dict):
+        logger.fine(f"Rendering a mimeo util [{mimeo_util_config}]")
         mimeo_util = cls._get_mimeo_util(mimeo_util_config)
         return mimeo_util.render()
 
     @classmethod
     def _get_mimeo_util(cls, mimeo_util_config: dict) -> MimeoUtil:
         mimeo_util_name = mimeo_util_config.get(MimeoConfig.MODEL_MIMEO_UTIL_NAME_KEY)
         if mimeo_util_name is None:
@@ -67,22 +70,24 @@
         return mimeo_util
 
 
 class VarsRenderer:
 
     @classmethod
     def render(cls, var: str):
+        logger.fine(f"Rendering a variable [{var}]")
         return MimeoContextManager().get_var(var)
 
 
 class SpecialFieldsRenderer:
 
     @classmethod
     @mimeo_context
     def render(cls, field_name: str, context: MimeoContext = None):
+        logger.fine(f"Rendering a special field [{field_name}]")
         return context.curr_iteration().get_special_field(field_name)
 
 
 class MimeoRenderer:
 
     _UTILS_PATTERN = re.compile("^{(.+)}$")
     _VARS_PATTERN = re.compile(".*({[A-Z_0-9]+})")
@@ -107,14 +112,15 @@
 
     @classmethod
     def is_parametrized_mimeo_util(cls, value: dict):
         return isinstance(value, dict) and len(value) == 1 and MimeoConfig.MODEL_MIMEO_UTIL_KEY in value
 
     @classmethod
     def render(cls, value):
+        logger.fine(f"Rendering a value [{value}]")
         try:
             if isinstance(value, str):
                 return cls._render_string_value(value)
             elif cls.is_parametrized_mimeo_util(value):
                 return cls._render_parametrized_mimeo_util(value)
             else:
                 return value
@@ -135,26 +141,30 @@
             return value
 
     @classmethod
     def _render_special_field(cls, value):
         match = next(cls._SPECIAL_FIELDS_PATTERN.finditer(value))
         wrapped_special_field = match.group(1)
         rendered_value = SpecialFieldsRenderer.render(wrapped_special_field[2:][:-2])
-        if isinstance(rendered_value, str):
+        logger.fine(f"Rendered special field value [{rendered_value}]")
+        if len(wrapped_special_field) != len(value):
+            rendered_value = str(rendered_value).lower() if isinstance(rendered_value, bool) else str(rendered_value)
             rendered_value = value.replace(wrapped_special_field, str(rendered_value))
         return cls.render(rendered_value)
 
     @classmethod
     def _render_var(cls, value):
         match = next(cls._VARS_PATTERN.finditer(value))
         wrapped_var = match.group(1)
         rendered_value = VarsRenderer.render(wrapped_var[1:][:-1])
+        logger.fine(f"Rendered variable value [{rendered_value}]")
         if cls.is_parametrized_mimeo_util(rendered_value):
             rendered_value = cls._render_parametrized_mimeo_util(rendered_value)
-        elif isinstance(rendered_value, str):
+        if len(wrapped_var) != len(value):
+            rendered_value = str(rendered_value).lower() if isinstance(rendered_value, bool) else str(rendered_value)
             rendered_value = value.replace(wrapped_var, str(rendered_value))
         return cls.render(rendered_value)
 
     @classmethod
     def _render_raw_mimeo_util(cls, value):
         rendered_value = UtilsRenderer.render_raw(value[1:][:-1])
         return cls.render(rendered_value)
```

### Comparing `mimeograph-0.3.1/src/mimeograph.egg-info/PKG-INFO` & `mimeograph-0.4.0/src/mimeograph.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mimeograph
-Version: 0.3.1
+Version: 0.4.0
 Summary: Generate data based on a simple template
 Author-email: "T.A. Programming Svcs." <tomasz.maciej.aniolowski@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tomasz Aniołowski
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -585,22 +585,22 @@
 {
   "City": "{city}"
 }
 ```
 
 ###### Parametrized
 
-Uses country (name, iso2, iso3) and `allow_duplicates` flag to generate a city name.
+Uses country (name, iso2, iso3) and `unique` flag to generate a city name.
 
 ```json
 {
   "CityWithDuplicates": {
     "_mimeo_util": {
       "_name": "city",
-      "allow_duplicates": true
+      "unique": false
     }
   },
   "CityOfCountryName": {
     "_mimeo_util": {
       "_name": "city",
       "country": "United Kingdom"
     }
@@ -617,15 +617,15 @@
       "country": "GBR"
     }
   },
   "CityOfCountryWithDuplicates": {
     "_mimeo_util": {
       "_name": "city",
       "country": "United Kingdom",
-      "allow_duplicates": true
+      "unique": false
     }
   }
 }
 ```
 
 ##### Country
 
@@ -646,22 +646,22 @@
 It can generate:
 - country iso3 or iso 2 instead of name
 - country with duplicates
 - country name for a provided iso3 or iso2
 - country iso2 for a provided name or iso3
 - country iso3 for a provided name or iso2
 
-When the `country` param is provided then the `allow_duplicates` flag is ignored.
+When the `country` param is provided then the `unique` flag is ignored.
 
 ```json
 {
   "CountryNameWithDuplicates": {
     "_mimeo_util": {
       "_name": "country",
-      "allow_duplicates": true
+      "unique": false
     }
   },
   "CountryISO2": {
     "_mimeo_util": {
       "_name": "country",
       "value": "iso2"
     }
@@ -684,22 +684,101 @@
       "value": "iso2",
       "country": "United Kingdom"
     }
   }
 }
 ```
 
+##### First Name
+
+Generates a first name.
+
+###### Raw
+
+By default first names will be unique across a Mimeo Context.
+
+```json
+{
+  "FirstName": "{first_name}"
+}
+```
+
+###### Parametrized
+
+Uses sex (`M` / `Male` / `F` / `Female`) and `unique` flag to generate a first name.
+
+```json
+{
+  "FirstNameWithDuplicates": {
+    "_mimeo_util": {
+      "_name": "first_name",
+      "unique": false
+    }
+  },
+  "MaleFirstName": {
+    "_mimeo_util": {
+      "_name": "first_name",
+      "sex": "M"
+    }
+  },
+  "FemaleFirstName": {
+    "_mimeo_util": {
+      "_name": "first_name",
+      "sex": "F"
+    }
+  },
+  "MaleFirstNameWithDuplicates": {
+    "_mimeo_util": {
+      "_name": "first_name",
+      "sex": "M",
+      "unique": false
+    }
+  }
+}
+```
+
+##### Last Name
+
+Generates a last name.
+
+###### Raw
+
+By default last names will be unique across a Mimeo Context.
+
+```json
+{
+  "LastName": "{last_name}"
+}
+```
+
+###### Parametrized
+
+Uses `unique` flag to generate a last name.
+
+```json
+{
+  "LastNameWithDuplicates": {
+    "_mimeo_util": {
+      "_name": "last_name",
+      "unique": false
+    }
+  }
+}
+```
+
 
 ## License
 
 MIT
 
 
 ## Authors
 
 - [@TomaszAniolowski](https://www.github.com/TomaszAniolowski)
 
 
 ## Acknowledgements
 
  - [SimpleMaps.com](https://simplemaps.com/data/world-cities) (Cities & countries data)
+ - [@hadley/data-baby-names](https://github.com/hadley/data-baby-names/) (Forenames data)
+ - [@fivethirtyeigh/data/most-common-name](https://github.com/fivethirtyeight/data/tree/master/most-common-name) (Surnames data)
```

### Comparing `mimeograph-0.3.1/src/mimeograph.egg-info/SOURCES.txt` & `mimeograph-0.4.0/src/mimeograph.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 src/mimeo/__init__.py
 src/mimeo/__main__.py
-src/mimeo/exceptions.py
+src/mimeo/exc.py
 src/mimeo/mimeo.py
 src/mimeo/tools.py
 src/mimeo/config/__init__.py
+src/mimeo/config/exc.py
 src/mimeo/config/mimeo_config.py
 src/mimeo/consumers/__init__.py
 src/mimeo/consumers/consumer.py
 src/mimeo/consumers/consumer_factory.py
 src/mimeo/consumers/file_consumer.py
 src/mimeo/consumers/http_consumer.py
 src/mimeo/consumers/raw_consumer.py
@@ -21,34 +22,39 @@
 src/mimeo/context/mimeo_context.py
 src/mimeo/context/mimeo_context_manager.py
 src/mimeo/context/mimeo_iteration.py
 src/mimeo/database/__init__.py
 src/mimeo/database/cities.py
 src/mimeo/database/countries.py
 src/mimeo/database/exc.py
+src/mimeo/database/first_names.py
+src/mimeo/database/last_names.py
 src/mimeo/database/mimeo_db.py
 src/mimeo/generators/__init__.py
 src/mimeo/generators/generator.py
 src/mimeo/generators/generator_factory.py
 src/mimeo/generators/xml_generator.py
 src/mimeo/logging/__init__.py
 src/mimeo/logging/filters.py
 src/mimeo/meta/__init__.py
 src/mimeo/meta/alive.py
 src/mimeo/meta/exc.py
 src/mimeo/resources/__init__.py
 src/mimeo/resources/cities.csv
 src/mimeo/resources/countries.csv
+src/mimeo/resources/exc.py
+src/mimeo/resources/forenames.csv
 src/mimeo/resources/logging.yaml
+src/mimeo/resources/surnames.txt
 src/mimeo/utils/__init__.py
 src/mimeo/utils/exc.py
 src/mimeo/utils/mimeo_utils.py
 src/mimeo/utils/renderer.py
 src/mimeograph.egg-info/PKG-INFO
 src/mimeograph.egg-info/SOURCES.txt
 src/mimeograph.egg-info/dependency_links.txt
 src/mimeograph.egg-info/entry_points.txt
 src/mimeograph.egg-info/requires.txt
 src/mimeograph.egg-info/top_level.txt
 tests/test_mimeo_cli.py
 tests/test_mimeograph.py
-tests/test_utils.py
+tests/test_tools.py
```

### Comparing `mimeograph-0.3.1/tests/test_mimeo_cli.py` & `mimeograph-0.4.0/tests/test_mimeo_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from pathlib import Path
 
 import pytest
 import responses
 from responses import matchers
 
 import mimeo.__main__ as MimeoCLI
-from mimeo.exceptions import (EnvironmentNotFound, EnvironmentsFileNotFound,
-                              MissingRequiredProperty)
+from mimeo.config.exc import MissingRequiredProperty
+from mimeo.exc import EnvironmentNotFound, EnvironmentsFileNotFound
 
 
 @pytest.fixture(autouse=True)
 def minimum_config():
     return {
         "_templates_": [
             {
```

### Comparing `mimeograph-0.3.1/tests/test_mimeograph.py` & `mimeograph-0.4.0/tests/test_mimeograph.py`

 * *Files identical despite different names*


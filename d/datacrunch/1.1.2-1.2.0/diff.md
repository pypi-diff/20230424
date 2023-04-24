# Comparing `tmp/datacrunch-1.1.2.tar.gz` & `tmp/datacrunch-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datacrunch-1.1.2.tar", last modified: Thu Mar  2 15:43:50 2023, max compression
+gzip compressed data, was "datacrunch-1.2.0.tar", last modified: Mon Apr 24 15:02:00 2023, max compression
```

## Comparing `datacrunch-1.1.2.tar` & `datacrunch-1.2.0.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:50.980039 datacrunch-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-02 15:43:36.000000 datacrunch-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-03-02 15:43:50.980039 datacrunch-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-03-02 15:43:36.000000 datacrunch-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:50.972038 datacrunch-1.1.2/datacrunch/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-02 15:43:36.000000 datacrunch-1.1.2/datacrunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-02 15:43:36.000000 datacrunch-1.1.2/datacrunch/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:50.972038 datacrunch-1.1.2/datacrunch/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:36.000000 datacrunch-1.1.2/datacrunch/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-03-02 15:43:36.000000 datacrunch-1.1.2/datacrunch/authentication/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:50.972038 datacrunch-1.1.2/datacrunch/balance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:36.000000 datacrunch-1.1.2/datacrunch/balance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-03-02 15:43:36.000000 datacrunch-1.1.2/datacrunch/balance/balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-03-02 15:43:36.000000 datacrunch-1.1.2/datacrunch/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-03-02 15:43:36.000000 datacrunch-1.1.2/datacrunch/datacrunch.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-03-02 15:43:36.000000 datacrunch-1.1.2/datacrunch/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-02 15:43:36.000000 datacrunch-1.1.2/datacrunch/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:50.972038 datacrunch-1.1.2/datacrunch/http_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:36.000000 datacrunch-1.1.2/datacrunch/http_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-03-02 15:43:36.000000 datacrunch-1.1.2/datacrunch/http_client/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:50.972038 datacrunch-1.1.2/datacrunch/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:36.000000 datacrunch-1.1.2/datacrunch/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-03-02 15:43:36.000000 datacrunch-1.1.2/datacrunch/images/images.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:50.972038 datacrunch-1.1.2/datacrunch/instance_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:36.000000 datacrunch-1.1.2/datacrunch/instance_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-03-02 15:43:36.000000 datacrunch-1.1.2/datacrunch/instance_types/instance_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:50.972038 datacrunch-1.1.2/datacrunch/instances/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:36.000000 datacrunch-1.1.2/datacrunch/instances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13996 2023-03-02 15:43:36.000000 datacrunch-1.1.2/datacrunch/instances/instances.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:50.972038 datacrunch-1.1.2/datacrunch/ssh_keys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:36.000000 datacrunch-1.1.2/datacrunch/ssh_keys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-03-02 15:43:36.000000 datacrunch-1.1.2/datacrunch/ssh_keys/ssh_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:50.976038 datacrunch-1.1.2/datacrunch/startup_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:36.000000 datacrunch-1.1.2/datacrunch/startup_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-03-02 15:43:36.000000 datacrunch-1.1.2/datacrunch/startup_scripts/startup_scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:50.976038 datacrunch-1.1.2/datacrunch/volume_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:36.000000 datacrunch-1.1.2/datacrunch/volume_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-03-02 15:43:36.000000 datacrunch-1.1.2/datacrunch/volume_types/volume_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:50.976038 datacrunch-1.1.2/datacrunch/volumes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:36.000000 datacrunch-1.1.2/datacrunch/volumes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10282 2023-03-02 15:43:36.000000 datacrunch-1.1.2/datacrunch/volumes/volumes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:50.972038 datacrunch-1.1.2/datacrunch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-03-02 15:43:50.000000 datacrunch-1.1.2/datacrunch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-03-02 15:43:50.000000 datacrunch-1.1.2/datacrunch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 15:43:50.000000 datacrunch-1.1.2/datacrunch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-02 15:43:50.000000 datacrunch-1.1.2/datacrunch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-02 15:43:50.000000 datacrunch-1.1.2/datacrunch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-02 15:43:50.980039 datacrunch-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-03-02 15:43:36.000000 datacrunch-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:50.976038 datacrunch-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:36.000000 datacrunch-1.1.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:50.976038 datacrunch-1.1.2/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:36.000000 datacrunch-1.1.2/tests/unit_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:50.976038 datacrunch-1.1.2/tests/unit_tests/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:36.000000 datacrunch-1.1.2/tests/unit_tests/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-03-02 15:43:36.000000 datacrunch-1.1.2/tests/unit_tests/authentication/test_authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:50.976038 datacrunch-1.1.2/tests/unit_tests/balance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:36.000000 datacrunch-1.1.2/tests/unit_tests/balance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-03-02 15:43:36.000000 datacrunch-1.1.2/tests/unit_tests/balance/test_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-03-02 15:43:36.000000 datacrunch-1.1.2/tests/unit_tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:50.976038 datacrunch-1.1.2/tests/unit_tests/http_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:36.000000 datacrunch-1.1.2/tests/unit_tests/http_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-03-02 15:43:36.000000 datacrunch-1.1.2/tests/unit_tests/http_client/test_http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:50.976038 datacrunch-1.1.2/tests/unit_tests/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:36.000000 datacrunch-1.1.2/tests/unit_tests/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-03-02 15:43:36.000000 datacrunch-1.1.2/tests/unit_tests/images/test_images.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:50.976038 datacrunch-1.1.2/tests/unit_tests/instance_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:36.000000 datacrunch-1.1.2/tests/unit_tests/instance_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-03-02 15:43:36.000000 datacrunch-1.1.2/tests/unit_tests/instance_types/test_instance_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:50.976038 datacrunch-1.1.2/tests/unit_tests/instances/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:36.000000 datacrunch-1.1.2/tests/unit_tests/instances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16748 2023-03-02 15:43:36.000000 datacrunch-1.1.2/tests/unit_tests/instances/test_instances.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:50.976038 datacrunch-1.1.2/tests/unit_tests/ssh_keys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:36.000000 datacrunch-1.1.2/tests/unit_tests/ssh_keys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-03-02 15:43:36.000000 datacrunch-1.1.2/tests/unit_tests/ssh_keys/test_ssh_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:50.980039 datacrunch-1.1.2/tests/unit_tests/startup_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:36.000000 datacrunch-1.1.2/tests/unit_tests/startup_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-03-02 15:43:36.000000 datacrunch-1.1.2/tests/unit_tests/startup_scripts/test_startup_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-03-02 15:43:36.000000 datacrunch-1.1.2/tests/unit_tests/test_datacrunch.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-02 15:43:36.000000 datacrunch-1.1.2/tests/unit_tests/test_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:50.980039 datacrunch-1.1.2/tests/unit_tests/volume_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:36.000000 datacrunch-1.1.2/tests/unit_tests/volume_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-03-02 15:43:36.000000 datacrunch-1.1.2/tests/unit_tests/volume_types/test_volume_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:50.980039 datacrunch-1.1.2/tests/unit_tests/volumes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 15:43:36.000000 datacrunch-1.1.2/tests/unit_tests/volumes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15235 2023-03-02 15:43:36.000000 datacrunch-1.1.2/tests/unit_tests/volumes/test_volumes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.991226 datacrunch-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-24 15:01:48.000000 datacrunch-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-04-24 15:02:00.991226 datacrunch-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-04-24 15:01:48.000000 datacrunch-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.987226 datacrunch-1.2.0/datacrunch/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.987226 datacrunch-1.2.0/datacrunch/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/authentication/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.987226 datacrunch-1.2.0/datacrunch/balance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/balance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/balance/balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/datacrunch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.987226 datacrunch-1.2.0/datacrunch/http_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/http_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/http_client/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.987226 datacrunch-1.2.0/datacrunch/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/images/images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.987226 datacrunch-1.2.0/datacrunch/instance_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/instance_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/instance_types/instance_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.987226 datacrunch-1.2.0/datacrunch/instances/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/instances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14236 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/instances/instances.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.987226 datacrunch-1.2.0/datacrunch/ssh_keys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/ssh_keys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/ssh_keys/ssh_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.991226 datacrunch-1.2.0/datacrunch/startup_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/startup_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/startup_scripts/startup_scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.991226 datacrunch-1.2.0/datacrunch/volume_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/volume_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/volume_types/volume_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.991226 datacrunch-1.2.0/datacrunch/volumes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/volumes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10282 2023-04-24 15:01:48.000000 datacrunch-1.2.0/datacrunch/volumes/volumes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.987226 datacrunch-1.2.0/datacrunch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-04-24 15:02:00.000000 datacrunch-1.2.0/datacrunch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-24 15:02:00.000000 datacrunch-1.2.0/datacrunch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 15:02:00.000000 datacrunch-1.2.0/datacrunch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-24 15:02:00.000000 datacrunch-1.2.0/datacrunch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-24 15:02:00.000000 datacrunch-1.2.0/datacrunch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 15:02:00.991226 datacrunch-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-24 15:01:48.000000 datacrunch-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.991226 datacrunch-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.991226 datacrunch-1.2.0/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.991226 datacrunch-1.2.0/tests/unit_tests/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/authentication/test_authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.991226 datacrunch-1.2.0/tests/unit_tests/balance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/balance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/balance/test_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.991226 datacrunch-1.2.0/tests/unit_tests/http_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/http_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/http_client/test_http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.991226 datacrunch-1.2.0/tests/unit_tests/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/images/test_images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.991226 datacrunch-1.2.0/tests/unit_tests/instance_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/instance_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/instance_types/test_instance_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.991226 datacrunch-1.2.0/tests/unit_tests/instances/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/instances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16748 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/instances/test_instances.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.991226 datacrunch-1.2.0/tests/unit_tests/ssh_keys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/ssh_keys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/ssh_keys/test_ssh_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.991226 datacrunch-1.2.0/tests/unit_tests/startup_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/startup_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/startup_scripts/test_startup_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/test_datacrunch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/test_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.991226 datacrunch-1.2.0/tests/unit_tests/volume_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/volume_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/volume_types/test_volume_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:02:00.991226 datacrunch-1.2.0/tests/unit_tests/volumes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/volumes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15235 2023-04-24 15:01:48.000000 datacrunch-1.2.0/tests/unit_tests/volumes/test_volumes.py
```

### Comparing `datacrunch-1.1.2/LICENSE` & `datacrunch-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datacrunch-1.1.2/PKG-INFO` & `datacrunch-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datacrunch
-Version: 1.1.2
+Version: 1.2.0
 Summary: Official Python SDK for DataCrunch Public API
 Home-page: https://github.com/DataCrunch-io
 Author: DataCrunch Oy
 Author-email: info@datacrunch.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datacrunch Version: 1.1.2 Summary: Official Python
+Metadata-Version: 2.1 Name: datacrunch Version: 1.2.0 Summary: Official Python
 SDK for DataCrunch Public API Home-page: https://github.com/DataCrunch-io
 Author: DataCrunch Oy Author-email: info@datacrunch.io Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Development Status :: 5 - Production/
```

### Comparing `datacrunch-1.1.2/README.md` & `datacrunch-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `datacrunch-1.1.2/datacrunch/authentication/authentication.py` & `datacrunch-1.2.0/datacrunch/authentication/authentication.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.1.2/datacrunch/balance/balance.py` & `datacrunch-1.2.0/datacrunch/balance/balance.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.1.2/datacrunch/constants.py` & `datacrunch-1.2.0/datacrunch/constants.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.1.2/datacrunch/datacrunch.py` & `datacrunch-1.2.0/datacrunch/datacrunch.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.1.2/datacrunch/exceptions.py` & `datacrunch-1.2.0/datacrunch/exceptions.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.1.2/datacrunch/helpers.py` & `datacrunch-1.2.0/datacrunch/helpers.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.1.2/datacrunch/http_client/http_client.py` & `datacrunch-1.2.0/datacrunch/http_client/http_client.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.1.2/datacrunch/images/images.py` & `datacrunch-1.2.0/datacrunch/images/images.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.1.2/datacrunch/instance_types/instance_types.py` & `datacrunch-1.2.0/datacrunch/instance_types/instance_types.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.1.2/datacrunch/instances/instances.py` & `datacrunch-1.2.0/datacrunch/instances/instances.py`

 * *Files 2% similar despite different names*

```diff
@@ -345,14 +345,15 @@
                image: str,
                hostname: str,
                description: str,
                ssh_key_ids: list = [],
                location: str = "FIN1",
                startup_script_id: str = None,
                volumes: List[Dict] = None,
+               existing_volumes: List[str] = None,
                os_volume: Dict = None,
                is_spot: bool = False,
                coupon: str = None) -> Instance:
         """Creates (deploys) a new instance
 
         :param instance_type: instance type. e.g. '8V100.48M'
         :type instance_type: str
@@ -366,14 +367,16 @@
         :type description: str
         :param location: datacenter location, defaults to "FIN1"
         :type location: str, optional
         :param startup_script_id: startup script id, defaults to None
         :type startup_script_id: str, optional
         :param volumes: List of volume data dictionaries to create alongside the instance
         :type volumes: List[Dict], optional
+        :param existing_volumes: List of existing volume ids to attach to the instance
+        :type existing_volumes: List[str], optional
         :param os_volume: OS volume details, defaults to None
         :type os_volume: Dict, optional
         :param is_spot: Is spot instance
         :type is_spot: bool, optional
         :param coupon: coupon code
         :type coupon: str, optional
         :return: the new instance object
@@ -385,14 +388,15 @@
             "ssh_key_ids": ssh_key_ids,
             "startup_script_id": startup_script_id,
             "hostname": hostname,
             "description": description,
             "location": location,
             "os_volume": os_volume,
             "volumes": volumes,
+            "existing_volumes": existing_volumes,
             "is_spot": is_spot,
             "coupon": coupon
         }
         id = self._http_client.post(INSTANCES_ENDPOINT, json=payload).text
         instance = self.get_by_id(id)
         return instance
```

### Comparing `datacrunch-1.1.2/datacrunch/ssh_keys/ssh_keys.py` & `datacrunch-1.2.0/datacrunch/ssh_keys/ssh_keys.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.1.2/datacrunch/startup_scripts/startup_scripts.py` & `datacrunch-1.2.0/datacrunch/startup_scripts/startup_scripts.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.1.2/datacrunch/volume_types/volume_types.py` & `datacrunch-1.2.0/datacrunch/volume_types/volume_types.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.1.2/datacrunch/volumes/volumes.py` & `datacrunch-1.2.0/datacrunch/volumes/volumes.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.1.2/datacrunch.egg-info/PKG-INFO` & `datacrunch-1.2.0/datacrunch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datacrunch
-Version: 1.1.2
+Version: 1.2.0
 Summary: Official Python SDK for DataCrunch Public API
 Home-page: https://github.com/DataCrunch-io
 Author: DataCrunch Oy
 Author-email: info@datacrunch.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datacrunch Version: 1.1.2 Summary: Official Python
+Metadata-Version: 2.1 Name: datacrunch Version: 1.2.0 Summary: Official Python
 SDK for DataCrunch Public API Home-page: https://github.com/DataCrunch-io
 Author: DataCrunch Oy Author-email: info@datacrunch.io Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Development Status :: 5 - Production/
```

### Comparing `datacrunch-1.1.2/datacrunch.egg-info/SOURCES.txt` & `datacrunch-1.2.0/datacrunch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datacrunch-1.1.2/setup.py` & `datacrunch-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.1.2/tests/unit_tests/authentication/test_authentication.py` & `datacrunch-1.2.0/tests/unit_tests/authentication/test_authentication.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.1.2/tests/unit_tests/balance/test_balance.py` & `datacrunch-1.2.0/tests/unit_tests/balance/test_balance.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.1.2/tests/unit_tests/conftest.py` & `datacrunch-1.2.0/tests/unit_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.1.2/tests/unit_tests/http_client/test_http_client.py` & `datacrunch-1.2.0/tests/unit_tests/http_client/test_http_client.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.1.2/tests/unit_tests/images/test_images.py` & `datacrunch-1.2.0/tests/unit_tests/images/test_images.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.1.2/tests/unit_tests/instance_types/test_instance_types.py` & `datacrunch-1.2.0/tests/unit_tests/instance_types/test_instance_types.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.1.2/tests/unit_tests/instances/test_instances.py` & `datacrunch-1.2.0/tests/unit_tests/instances/test_instances.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.1.2/tests/unit_tests/ssh_keys/test_ssh_keys.py` & `datacrunch-1.2.0/tests/unit_tests/ssh_keys/test_ssh_keys.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.1.2/tests/unit_tests/startup_scripts/test_startup_scripts.py` & `datacrunch-1.2.0/tests/unit_tests/startup_scripts/test_startup_scripts.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.1.2/tests/unit_tests/test_datacrunch.py` & `datacrunch-1.2.0/tests/unit_tests/test_datacrunch.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.1.2/tests/unit_tests/test_exceptions.py` & `datacrunch-1.2.0/tests/unit_tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.1.2/tests/unit_tests/volume_types/test_volume_types.py` & `datacrunch-1.2.0/tests/unit_tests/volume_types/test_volume_types.py`

 * *Files identical despite different names*

### Comparing `datacrunch-1.1.2/tests/unit_tests/volumes/test_volumes.py` & `datacrunch-1.2.0/tests/unit_tests/volumes/test_volumes.py`

 * *Files identical despite different names*


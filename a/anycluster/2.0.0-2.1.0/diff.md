# Comparing `tmp/anycluster-2.0.0.tar.gz` & `tmp/anycluster-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anycluster-2.0.0.tar", last modified: Fri Apr 21 13:23:56 2023, max compression
+gzip compressed data, was "anycluster-2.1.0.tar", last modified: Mon Apr 24 13:43:29 2023, max compression
```

## Comparing `anycluster-2.0.0.tar` & `anycluster-2.1.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-21 13:23:56.135873 anycluster-2.0.0/
--rw-r--r--   0 tom       (1000) tom       (1000)     1078 2023-01-20 06:49:37.000000 anycluster-2.0.0/LICENSE
--rw-r--r--   0 tom       (1000) tom       (1000)      219 2023-04-21 13:23:32.000000 anycluster-2.0.0/MANIFEST.in
--rw-r--r--   0 tom       (1000) tom       (1000)     2915 2023-04-21 13:23:56.135873 anycluster-2.0.0/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     2326 2023-01-20 06:49:37.000000 anycluster-2.0.0/README.md
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-21 13:23:56.131873 anycluster-2.0.0/anycluster/
--rw-r--r--   0 tom       (1000) tom       (1000)     1594 2023-04-19 10:28:26.000000 anycluster-2.0.0/anycluster/ClusterCache.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2680 2023-04-20 07:53:43.000000 anycluster-2.0.0/anycluster/FilterComposer.py
--rw-r--r--   0 tom       (1000) tom       (1000)    31624 2023-04-19 10:53:31.000000 anycluster-2.0.0/anycluster/MapClusterer.py
--rw-r--r--   0 tom       (1000) tom       (1000)    10605 2023-03-06 13:41:59.000000 anycluster-2.0.0/anycluster/MapTools.py
--rw-r--r--   0 tom       (1000) tom       (1000)      112 2023-04-19 10:38:36.000000 anycluster-2.0.0/anycluster/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-21 13:23:56.131873 anycluster-2.0.0/anycluster/api/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-21 13:23:56.131873 anycluster-2.0.0/anycluster/api/__pycache__/
--rw-r--r--   0 tom       (1000) tom       (1000)     1584 2023-03-21 14:03:34.000000 anycluster-2.0.0/anycluster/api/__pycache__/json_schemas.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     1214 2023-03-02 08:31:15.000000 anycluster-2.0.0/anycluster/api/__pycache__/serializer_fields.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     2592 2023-04-21 13:09:53.000000 anycluster-2.0.0/anycluster/api/__pycache__/serializers.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)      940 2023-03-17 13:31:29.000000 anycluster-2.0.0/anycluster/api/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     5797 2023-04-19 10:41:51.000000 anycluster-2.0.0/anycluster/api/__pycache__/views.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     3180 2023-03-21 14:03:34.000000 anycluster-2.0.0/anycluster/api/json_schemas.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2572 2023-04-21 13:09:52.000000 anycluster-2.0.0/anycluster/api/serializers.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-21 13:23:56.131873 anycluster-2.0.0/anycluster/api/tests/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-21 13:23:56.135873 anycluster-2.0.0/anycluster/api/tests/__pycache__/
--rw-r--r--   0 tom       (1000) tom       (1000)     1066 2023-03-02 09:10:26.000000 anycluster-2.0.0/anycluster/api/tests/__pycache__/common.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     1120 2023-03-17 13:45:55.000000 anycluster-2.0.0/anycluster/api/tests/__pycache__/test_serializers.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     6965 2023-04-19 19:03:37.000000 anycluster-2.0.0/anycluster/api/tests/__pycache__/test_views.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)      826 2023-03-02 13:13:55.000000 anycluster-2.0.0/anycluster/api/tests/test_serializers.py
--rw-r--r--   0 tom       (1000) tom       (1000)     9420 2023-04-19 19:03:34.000000 anycluster-2.0.0/anycluster/api/tests/test_views.py
--rw-r--r--   0 tom       (1000) tom       (1000)      882 2023-03-17 13:31:28.000000 anycluster-2.0.0/anycluster/api/urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)     7179 2023-04-19 10:29:29.000000 anycluster-2.0.0/anycluster/api/views.py
--rw-r--r--   0 tom       (1000) tom       (1000)       95 2023-03-02 07:01:38.000000 anycluster-2.0.0/anycluster/apps.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1142 2023-01-20 06:49:37.000000 anycluster-2.0.0/anycluster/clusters.py
--rw-r--r--   0 tom       (1000) tom       (1000)      602 2023-03-21 14:48:59.000000 anycluster-2.0.0/anycluster/definitions.py
--rw-r--r--   0 tom       (1000) tom       (1000)    16529 2023-01-20 06:49:37.000000 anycluster-2.0.0/anycluster/globalmaptiles.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-21 13:23:56.131873 anycluster-2.0.0/anycluster/static/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-21 13:23:56.131873 anycluster-2.0.0/anycluster/static/anycluster/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-21 13:23:56.135873 anycluster-2.0.0/anycluster/static/anycluster/images/
--rw-r--r--   0 tom       (1000) tom       (1000)     1445 2023-01-20 06:49:37.000000 anycluster-2.0.0/anycluster/static/anycluster/images/10.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1912 2023-01-20 06:49:37.000000 anycluster-2.0.0/anycluster/static/anycluster/images/100.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2093 2023-01-20 06:49:37.000000 anycluster-2.0.0/anycluster/static/anycluster/images/1000.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2811 2023-01-20 06:49:37.000000 anycluster-2.0.0/anycluster/static/anycluster/images/10000.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1409 2023-01-20 06:49:37.000000 anycluster-2.0.0/anycluster/static/anycluster/images/10000_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1262 2023-01-20 06:49:37.000000 anycluster-2.0.0/anycluster/static/anycluster/images/1000_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1034 2023-01-20 06:49:37.000000 anycluster-2.0.0/anycluster/static/anycluster/images/100_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)      784 2023-01-20 06:49:37.000000 anycluster-2.0.0/anycluster/static/anycluster/images/10_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1253 2023-01-20 06:49:37.000000 anycluster-2.0.0/anycluster/static/anycluster/images/5.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1974 2023-01-20 06:49:37.000000 anycluster-2.0.0/anycluster/static/anycluster/images/50.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1023 2023-01-20 06:49:37.000000 anycluster-2.0.0/anycluster/static/anycluster/images/50_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)      749 2023-01-20 06:49:37.000000 anycluster-2.0.0/anycluster/static/anycluster/images/5_empty.png
--rwxr-xr-x   0 tom       (1000) tom       (1000)     1158 2023-01-20 06:49:37.000000 anycluster-2.0.0/anycluster/static/anycluster/images/pin_unknown.png
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-21 13:23:56.135873 anycluster-2.0.0/anycluster/tests/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-21 13:23:56.135873 anycluster-2.0.0/anycluster/tests/__pycache__/
--rw-r--r--   0 tom       (1000) tom       (1000)     1432 2023-04-19 10:14:42.000000 anycluster-2.0.0/anycluster/tests/__pycache__/common.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     2533 2023-04-19 10:53:00.000000 anycluster-2.0.0/anycluster/tests/__pycache__/mixins.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     3837 2023-04-21 13:16:50.000000 anycluster-2.0.0/anycluster/tests/__pycache__/test_ClusterCache.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     2790 2023-04-21 13:19:15.000000 anycluster-2.0.0/anycluster/tests/__pycache__/test_FilterComposer.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     2882 2023-04-19 08:43:21.000000 anycluster-2.0.0/anycluster/tests/__pycache__/test_Filters.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)    10728 2023-04-19 10:54:13.000000 anycluster-2.0.0/anycluster/tests/__pycache__/test_MapClusterer.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     2547 2023-04-19 10:13:34.000000 anycluster-2.0.0/anycluster/tests/common.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2096 2023-04-19 10:47:07.000000 anycluster-2.0.0/anycluster/tests/mixins.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6963 2023-04-19 10:47:33.000000 anycluster-2.0.0/anycluster/tests/test_ClusterCache.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3995 2023-04-21 13:19:10.000000 anycluster-2.0.0/anycluster/tests/test_FilterComposer.py
--rw-r--r--   0 tom       (1000) tom       (1000)    16495 2023-04-19 10:54:09.000000 anycluster-2.0.0/anycluster/tests/test_MapClusterer.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-21 13:23:56.131873 anycluster-2.0.0/anycluster.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)     2915 2023-04-21 13:23:56.000000 anycluster-2.0.0/anycluster.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     2191 2023-04-21 13:23:56.000000 anycluster-2.0.0/anycluster.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-04-21 13:23:56.000000 anycluster-2.0.0/anycluster.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       40 2023-04-21 13:23:56.000000 anycluster-2.0.0/anycluster.egg-info/requires.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       11 2023-04-21 13:23:56.000000 anycluster-2.0.0/anycluster.egg-info/top_level.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       38 2023-04-21 13:23:56.135873 anycluster-2.0.0/setup.cfg
--rw-r--r--   0 tom       (1000) tom       (1000)      989 2023-04-21 13:20:38.000000 anycluster-2.0.0/setup.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 13:43:29.679516 anycluster-2.1.0/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1078 2023-01-20 06:49:37.000000 anycluster-2.1.0/LICENSE
+-rw-r--r--   0 tom       (1000) tom       (1000)      219 2023-04-22 19:21:48.000000 anycluster-2.1.0/MANIFEST.in
+-rw-r--r--   0 tom       (1000) tom       (1000)     2257 2023-04-24 13:43:29.679516 anycluster-2.1.0/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)     1668 2023-04-22 19:37:42.000000 anycluster-2.1.0/README.md
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 13:43:29.671516 anycluster-2.1.0/anycluster/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1594 2023-04-19 10:28:26.000000 anycluster-2.1.0/anycluster/ClusterCache.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2680 2023-04-20 07:53:43.000000 anycluster-2.1.0/anycluster/FilterComposer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    31624 2023-04-19 10:53:31.000000 anycluster-2.1.0/anycluster/MapClusterer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    10605 2023-03-06 13:41:59.000000 anycluster-2.1.0/anycluster/MapTools.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      112 2023-04-19 10:38:36.000000 anycluster-2.1.0/anycluster/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 13:43:29.675516 anycluster-2.1.0/anycluster/api/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 13:43:29.675516 anycluster-2.1.0/anycluster/api/__pycache__/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1584 2023-03-21 14:03:34.000000 anycluster-2.1.0/anycluster/api/__pycache__/json_schemas.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     1214 2023-03-02 08:31:15.000000 anycluster-2.1.0/anycluster/api/__pycache__/serializer_fields.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     2618 2023-04-24 13:23:49.000000 anycluster-2.1.0/anycluster/api/__pycache__/serializers.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)      947 2023-04-24 13:16:49.000000 anycluster-2.1.0/anycluster/api/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     6016 2023-04-24 12:45:45.000000 anycluster-2.1.0/anycluster/api/__pycache__/views.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     3180 2023-03-21 14:03:34.000000 anycluster-2.1.0/anycluster/api/json_schemas.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2572 2023-04-24 13:22:43.000000 anycluster-2.1.0/anycluster/api/serializers.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 13:43:29.675516 anycluster-2.1.0/anycluster/api/tests/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 13:43:29.675516 anycluster-2.1.0/anycluster/api/tests/__pycache__/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1066 2023-03-02 09:10:26.000000 anycluster-2.1.0/anycluster/api/tests/__pycache__/common.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     1120 2023-03-17 13:45:55.000000 anycluster-2.1.0/anycluster/api/tests/__pycache__/test_serializers.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     6965 2023-04-19 19:03:37.000000 anycluster-2.1.0/anycluster/api/tests/__pycache__/test_views.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)      826 2023-03-02 13:13:55.000000 anycluster-2.1.0/anycluster/api/tests/test_serializers.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     9420 2023-04-19 19:03:34.000000 anycluster-2.1.0/anycluster/api/tests/test_views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      882 2023-04-24 12:47:36.000000 anycluster-2.1.0/anycluster/api/urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     7323 2023-04-24 12:21:50.000000 anycluster-2.1.0/anycluster/api/views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       95 2023-03-02 07:01:38.000000 anycluster-2.1.0/anycluster/apps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1142 2023-01-20 06:49:37.000000 anycluster-2.1.0/anycluster/clusters.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      602 2023-03-21 14:48:59.000000 anycluster-2.1.0/anycluster/definitions.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    16529 2023-01-20 06:49:37.000000 anycluster-2.1.0/anycluster/globalmaptiles.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 13:43:29.671516 anycluster-2.1.0/anycluster/static/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 13:43:29.671516 anycluster-2.1.0/anycluster/static/anycluster/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 13:43:29.675516 anycluster-2.1.0/anycluster/static/anycluster/images/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1445 2023-01-20 06:49:37.000000 anycluster-2.1.0/anycluster/static/anycluster/images/10.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1912 2023-01-20 06:49:37.000000 anycluster-2.1.0/anycluster/static/anycluster/images/100.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2093 2023-01-20 06:49:37.000000 anycluster-2.1.0/anycluster/static/anycluster/images/1000.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2811 2023-01-20 06:49:37.000000 anycluster-2.1.0/anycluster/static/anycluster/images/10000.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1409 2023-01-20 06:49:37.000000 anycluster-2.1.0/anycluster/static/anycluster/images/10000_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1262 2023-01-20 06:49:37.000000 anycluster-2.1.0/anycluster/static/anycluster/images/1000_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1034 2023-01-20 06:49:37.000000 anycluster-2.1.0/anycluster/static/anycluster/images/100_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      784 2023-01-20 06:49:37.000000 anycluster-2.1.0/anycluster/static/anycluster/images/10_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1253 2023-01-20 06:49:37.000000 anycluster-2.1.0/anycluster/static/anycluster/images/5.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1974 2023-01-20 06:49:37.000000 anycluster-2.1.0/anycluster/static/anycluster/images/50.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1023 2023-01-20 06:49:37.000000 anycluster-2.1.0/anycluster/static/anycluster/images/50_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      749 2023-01-20 06:49:37.000000 anycluster-2.1.0/anycluster/static/anycluster/images/5_empty.png
+-rwxr-xr-x   0 tom       (1000) tom       (1000)     1158 2023-01-20 06:49:37.000000 anycluster-2.1.0/anycluster/static/anycluster/images/pin_unknown.png
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 13:43:29.675516 anycluster-2.1.0/anycluster/tests/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 13:43:29.679516 anycluster-2.1.0/anycluster/tests/__pycache__/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1432 2023-04-19 10:14:42.000000 anycluster-2.1.0/anycluster/tests/__pycache__/common.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     2533 2023-04-19 10:53:00.000000 anycluster-2.1.0/anycluster/tests/__pycache__/mixins.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     3837 2023-04-21 13:16:50.000000 anycluster-2.1.0/anycluster/tests/__pycache__/test_ClusterCache.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     2790 2023-04-21 13:19:15.000000 anycluster-2.1.0/anycluster/tests/__pycache__/test_FilterComposer.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     2882 2023-04-19 08:43:21.000000 anycluster-2.1.0/anycluster/tests/__pycache__/test_Filters.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)    10728 2023-04-19 10:54:13.000000 anycluster-2.1.0/anycluster/tests/__pycache__/test_MapClusterer.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     2547 2023-04-19 10:13:34.000000 anycluster-2.1.0/anycluster/tests/common.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2096 2023-04-19 10:47:07.000000 anycluster-2.1.0/anycluster/tests/mixins.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6963 2023-04-19 10:47:33.000000 anycluster-2.1.0/anycluster/tests/test_ClusterCache.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3995 2023-04-21 13:19:10.000000 anycluster-2.1.0/anycluster/tests/test_FilterComposer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    16495 2023-04-19 10:54:09.000000 anycluster-2.1.0/anycluster/tests/test_MapClusterer.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 13:43:29.671516 anycluster-2.1.0/anycluster.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)     2257 2023-04-24 13:43:29.000000 anycluster-2.1.0/anycluster.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)     2191 2023-04-24 13:43:29.000000 anycluster-2.1.0/anycluster.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-04-24 13:43:29.000000 anycluster-2.1.0/anycluster.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       40 2023-04-24 13:43:29.000000 anycluster-2.1.0/anycluster.egg-info/requires.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       11 2023-04-24 13:43:29.000000 anycluster-2.1.0/anycluster.egg-info/top_level.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       38 2023-04-24 13:43:29.679516 anycluster-2.1.0/setup.cfg
+-rw-r--r--   0 tom       (1000) tom       (1000)      989 2023-04-24 13:43:01.000000 anycluster-2.1.0/setup.py
```

### Comparing `anycluster-2.0.0/LICENSE` & `anycluster-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/PKG-INFO` & `anycluster-2.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anycluster
-Version: 2.0.0
+Version: 2.1.0
 Summary: anycluster provides Server-Side clustering of map markers for Geodjango
 Home-page: https://github.com/biodiv/anycluster
 Author: Thomas Uher
 Author-email: thomas.uher@sisol-systems.com
 License: The MIT License
 Keywords: django,cluster,kmeans,grid,server-side clustering
 Platform: OS Independent
@@ -14,22 +14,31 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 anycluster (POSTGIS version)
 ============================
 
+[https://anycluster.org](https://anycluster.org)
+
 anycluster provides Server-Side clustering of map markers for Geodjango. It is suitable for large amounts of markers. 
 Depending on your server and personal feeling, it works very well with 200.000 to 500.000 markers.
 
 The postgis version is recommended. There is a mysql version with limited functionality: https://github.com/biodiv/anycluster-mysql
 
 
+Documentation
+-------------
+
+http://anycluster.readthedocs.org/en/latest/
+
+
 ChangeLog
 ---------
+- [22.04.2023] anycluster 2.0 (breaking changes, see docs), npm, Django 4.x, updated docs
 - [09.09.2019] support for Django 2.x and above (python 3), added leaflet support
 - [08.10.2015] major code improvements
 - you now need to add {% csrf_token % } somewhere in your template
 
 
 Features
 --------
@@ -39,44 +48,20 @@
 - clustering based on geometric density of the points (needs PSQL extension)
 - cluster contents of any geographic area defined as Polygon/Multipolygon
 - get all elements contained in a cluster
 
 ... and has a builtin caching mechanism: if the user pans a map, only the new areas are processed.
 
 And lots of optional customization possibilities:
-- works with google maps and Leaflet
+- works with OpenLayers, google maps and Leaflet
 - define what happens if you click on a cluster
 - use your own cluster graphics
 - define gridsize and other cluster parameters
 - apply filters to your clusters
 - use specialized markers/pins if count is 1
 
 
-Documentation
--------------
-
-http://anycluster.readthedocs.org/en/latest/
-
-
-Using the Demo
---------------
-
-To use the demo, follow these steps: 
-
-- install ``Django 2.x`` correctly
-- install ``psycopg2``
-- copy the demo folder to your system and include the anycluster folder as a django app.
-- modify the database connection in ``settings.py`` according to your setup
-- if you want to use google maps: add your google api key to ``anymap/templates/base.html``
-- remember to create the kmeans function as described in the documentation
-- from within the demo folder, run ``python manage.py migrate``
-- from within the demo folder, run ``python manage.py filldemodb 50000`` to fill the database with 50000 points
-- be patient, as this process is not very effective
-- from within the demo folder, run ``python manage.py runserver 8080``
-- open your browser and enter ``localhost:8080``
-
-
 Performance Tips
 ----------------
 
 - index your GIS database columns correctly
 - usage of a SSD can be 10-20 times faster compared to HDD
```

### Comparing `anycluster-2.0.0/README.md` & `anycluster-2.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 anycluster (POSTGIS version)
 ============================
 
+[https://anycluster.org](https://anycluster.org)
+
 anycluster provides Server-Side clustering of map markers for Geodjango. It is suitable for large amounts of markers. 
 Depending on your server and personal feeling, it works very well with 200.000 to 500.000 markers.
 
 The postgis version is recommended. There is a mysql version with limited functionality: https://github.com/biodiv/anycluster-mysql
 
 
+Documentation
+-------------
+
+http://anycluster.readthedocs.org/en/latest/
+
+
 ChangeLog
 ---------
+- [22.04.2023] anycluster 2.0 (breaking changes, see docs), npm, Django 4.x, updated docs
 - [09.09.2019] support for Django 2.x and above (python 3), added leaflet support
 - [08.10.2015] major code improvements
 - you now need to add {% csrf_token % } somewhere in your template
 
 
 Features
 --------
@@ -22,44 +31,20 @@
 - clustering based on geometric density of the points (needs PSQL extension)
 - cluster contents of any geographic area defined as Polygon/Multipolygon
 - get all elements contained in a cluster
 
 ... and has a builtin caching mechanism: if the user pans a map, only the new areas are processed.
 
 And lots of optional customization possibilities:
-- works with google maps and Leaflet
+- works with OpenLayers, google maps and Leaflet
 - define what happens if you click on a cluster
 - use your own cluster graphics
 - define gridsize and other cluster parameters
 - apply filters to your clusters
 - use specialized markers/pins if count is 1
 
 
-Documentation
--------------
-
-http://anycluster.readthedocs.org/en/latest/
-
-
-Using the Demo
---------------
-
-To use the demo, follow these steps: 
-
-- install ``Django 2.x`` correctly
-- install ``psycopg2``
-- copy the demo folder to your system and include the anycluster folder as a django app.
-- modify the database connection in ``settings.py`` according to your setup
-- if you want to use google maps: add your google api key to ``anymap/templates/base.html``
-- remember to create the kmeans function as described in the documentation
-- from within the demo folder, run ``python manage.py migrate``
-- from within the demo folder, run ``python manage.py filldemodb 50000`` to fill the database with 50000 points
-- be patient, as this process is not very effective
-- from within the demo folder, run ``python manage.py runserver 8080``
-- open your browser and enter ``localhost:8080``
-
-
 Performance Tips
 ----------------
 
 - index your GIS database columns correctly
 - usage of a SSD can be 10-20 times faster compared to HDD
```

### Comparing `anycluster-2.0.0/anycluster/ClusterCache.py` & `anycluster-2.1.0/anycluster/ClusterCache.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/FilterComposer.py` & `anycluster-2.1.0/anycluster/FilterComposer.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/MapClusterer.py` & `anycluster-2.1.0/anycluster/MapClusterer.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/MapTools.py` & `anycluster-2.1.0/anycluster/MapTools.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/api/__pycache__/json_schemas.cpython-38.pyc` & `anycluster-2.1.0/anycluster/api/__pycache__/json_schemas.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/api/__pycache__/serializer_fields.cpython-38.pyc` & `anycluster-2.1.0/anycluster/api/__pycache__/serializer_fields.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/api/__pycache__/serializers.cpython-38.pyc` & `anycluster-2.1.0/anycluster/api/__pycache__/serializers.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 21 13:09:52 2023 UTC, .py size: 2572 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 208b 4264 0c0a 0000  U....... .Bd....
+00000000: 550d 0d0a 0000 0000 a382 4664 0c0a 0000  U.........Fd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6c00 0000 6400  .....@...sl...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 5a04 6404  m.Z...d.d.l.Z.d.
 00000050: 6405 6c05 6d06 5a06 0100 6400 6406 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 0100 6407 6408 8400  m.Z.m.Z...d.d...
 00000070: 5a0a 4700 6409 640a 8400 640a 6503 6a0b  Z.G.d.d...d.e.j.
@@ -24,139 +24,141 @@
 00000170: 0053 0029 044e da06 636f 6c75 6d6e 7a17  .S.).N..columnz.
 00000180: 4669 6c74 6572 2072 6571 7569 7265 2061  Filter require a
 00000190: 2063 6f6c 756d 6e7a 2649 7420 6973 206e   columnz&It is n
 000001a0: 6f74 2061 6c6c 6f77 6564 2074 6f20 6669  ot allowed to fi
 000001b0: 6c74 6572 2043 6f6c 756d 6e20 7b30 7d29  lter Column {0})
 000001c0: 06da 0367 6574 7203 0000 00da 0f56 616c  ...getr......Val
 000001d0: 6964 6174 696f 6e45 7272 6f72 7202 0000  idationErrorr...
-000001e0: 00da 1241 4e59 434c 5553 5445 525f 4649  ...ANYCLUSTER_FI
+000001e0: 005a 1241 4e59 434c 5553 5445 525f 4649  .Z.ANYCLUSTER_FI
 000001f0: 4c54 4552 53da 0666 6f72 6d61 7429 03da  LTERS..format)..
 00000200: 0766 696c 7465 7273 da06 6669 6c74 6572  .filters..filter
-00000210: 7208 0000 00a9 0072 0f00 0000 fa3e 2f68  r......r.....>/h
-00000220: 6f6d 652f 746f 6d2f 616e 7963 6c75 7374  ome/tom/anyclust
-00000230: 6572 2f64 656d 6f2f 646a 616e 676f 2f61  er/demo/django/a
-00000240: 6e79 636c 7573 7465 722f 6170 692f 7365  nycluster/api/se
-00000250: 7269 616c 697a 6572 732e 7079 da13 6669  rializers.py..fi
-00000260: 6c74 6572 735f 6172 655f 616c 6c6f 7765  lters_are_allowe
-00000270: 640b 0000 0073 0c00 0000 0002 0801 0c01  d....s..........
-00000280: 0401 0a02 0a01 7211 0000 0063 0000 0000  ......r....c....
-00000290: 0000 0000 0000 0000 0000 0000 0500 0000  ................
-000002a0: 4000 0000 736e 0000 0065 005a 0164 005a  @...sn...e.Z.d.Z
-000002b0: 0265 036a 0464 0164 0264 0364 048d 035a  .e.j.d.d.d.d...Z
-000002c0: 0565 036a 0665 0764 0364 058d 025a 0865  .e.j.e.d.d...Z.e
-000002d0: 036a 0964 0364 068d 015a 0a65 036a 0b64  .j.d.d...Z.e.j.d
-000002e0: 0267 0064 0364 078d 035a 0c65 036a 0d64  .g.d.d...Z.e.j.d
-000002f0: 0264 0264 0364 048d 035a 0e64 0864 0984  .d.d.d...Z.d.d..
-00000300: 005a 0f64 0a64 0b84 005a 1064 0c64 0d84  .Z.d.d...Z.d.d..
-00000310: 005a 1164 0e53 0029 0fda 1843 6c75 7374  .Z.d.S.)...Clust
-00000320: 6572 5265 7175 6573 7453 6572 6961 6c69  erRequestSeriali
-00000330: 7a65 72fa 0945 5053 473a 3433 3236 4654  zer..EPSG:4326FT
-00000340: a903 da07 6465 6661 756c 74da 0872 6571  ....default..req
-00000350: 7569 7265 64da 0a77 7269 7465 5f6f 6e6c  uired..write_onl
-00000360: 79a9 02da 0763 686f 6963 6573 7217 0000  y....choicesr...
-00000370: 00a9 0172 1700 0000 a903 7216 0000 0072  ...r......r....r
-00000380: 1500 0000 7217 0000 0063 0200 0000 0000  ....r....c......
-00000390: 0000 0000 0000 0400 0000 0300 0000 4300  ..............C.
-000003a0: 0000 733e 0000 007c 0164 0119 0074 006b  ..s>...|.d...t.k
-000003b0: 0272 3a7c 0164 0219 007d 027c 0264 0319  .r:|.d...}.|.d..
-000003c0: 0064 0419 0064 0519 007d 0374 017c 0383  .d...d...}.t.|..
-000003d0: 0164 066b 0273 3a74 02a0 0364 07a1 0182  .d.k.s:t...d....
-000003e0: 017c 0153 0029 084e da0d 6765 6f6d 6574  .|.S.).N..geomet
-000003f0: 7279 5f74 7970 65da 0767 656f 6a73 6f6e  ry_type..geojson
-00000400: da08 6765 6f6d 6574 7279 da0b 636f 6f72  ..geometry..coor
-00000410: 6469 6e61 7465 7372 0100 0000 e905 0000  dinatesr........
-00000420: 007a 2156 6965 7770 6f72 7420 6d75 7374  .z!Viewport must
-00000430: 2063 6f6e 7369 7374 206f 6620 3520 706f   consist of 5 po
-00000440: 696e 7473 2904 7207 0000 00da 036c 656e  ints).r......len
-00000450: 7203 0000 0072 0a00 0000 2904 da04 7365  r....r....)...se
-00000460: 6c66 da04 6461 7461 721d 0000 0072 1f00  lf..datar....r..
-00000470: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
-00000480: 00da 0876 616c 6964 6174 6522 0000 0073  ...validate"...s
-00000490: 0c00 0000 0001 0c02 0801 1001 0c01 0a02  ................
-000004a0: 7a21 436c 7573 7465 7252 6571 7565 7374  z!ClusterRequest
-000004b0: 5365 7269 616c 697a 6572 2e76 616c 6964  Serializer.valid
-000004c0: 6174 6563 0200 0000 0000 0000 0000 0000  atec............
-000004d0: 0400 0000 0a00 0000 4300 0000 7348 0000  ........C...sH..
-000004e0: 007a 1074 00a0 017c 0174 02a1 027d 0257  .z.t...|.t...}.W
-000004f0: 006e 3204 0074 006a 036a 046b 0a72 4201  .n2..t.j.j.k.rB.
-00000500: 007d 0301 007a 1074 05a0 047c 036a 06a1  .}...z.t...|.j..
-00000510: 0182 0157 0035 0064 007d 037e 0358 0059  ...W.5.d.}.~.X.Y
-00000520: 006e 0258 007c 0153 00a9 014e 2907 da0a  .n.X.|.S...N)...
-00000530: 6a73 6f6e 7363 6865 6d61 7224 0000 0072  jsonschemar$...r
-00000540: 0500 0000 da0a 6578 6365 7074 696f 6e73  ......exceptions
-00000550: 720a 0000 0072 0300 0000 da07 6d65 7373  r....r......mess
-00000560: 6167 6529 0472 2200 0000 da05 7661 6c75  age).r".....valu
-00000570: 65da 0869 735f 7661 6c69 64da 0165 720f  e..is_valid..er.
-00000580: 0000 0072 0f00 0000 7210 0000 00da 1076  ...r....r......v
-00000590: 616c 6964 6174 655f 6765 6f6a 736f 6e2d  alidate_geojson-
-000005a0: 0000 0073 0a00 0000 0001 0201 1001 1401  ...s............
-000005b0: 1e01 7a29 436c 7573 7465 7252 6571 7565  ..z)ClusterReque
-000005c0: 7374 5365 7269 616c 697a 6572 2e76 616c  stSerializer.val
-000005d0: 6964 6174 655f 6765 6f6a 736f 6e63 0200  idate_geojsonc..
-000005e0: 0000 0000 0000 0000 0000 0200 0000 0200  ................
-000005f0: 0000 4300 0000 730c 0000 0074 007c 0183  ..C...s....t.|..
-00000600: 0101 007c 0153 0072 2500 0000 a901 7211  ...|.S.r%.....r.
-00000610: 0000 00a9 0272 2200 0000 7229 0000 0072  .....r"...r)...r
-00000620: 0f00 0000 720f 0000 0072 1000 0000 da10  ....r....r......
-00000630: 7661 6c69 6461 7465 5f66 696c 7465 7273  validate_filters
-00000640: 3400 0000 7304 0000 0000 0108 017a 2943  4...s........z)C
-00000650: 6c75 7374 6572 5265 7175 6573 7453 6572  lusterRequestSer
-00000660: 6961 6c69 7a65 722e 7661 6c69 6461 7465  ializer.validate
-00000670: 5f66 696c 7465 7273 4e29 12da 085f 5f6e  _filtersN)...__n
-00000680: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00000690: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
-000006a0: 0300 0000 da09 4368 6172 4669 656c 64da  ......CharField.
-000006b0: 0b6f 7574 7075 745f 7372 6964 da0b 4368  .output_srid..Ch
-000006c0: 6f69 6365 4669 656c 6472 0600 0000 721c  oiceFieldr....r.
-000006d0: 0000 00da 094a 534f 4e46 6965 6c64 721d  .....JSONFieldr.
-000006e0: 0000 00da 094c 6973 7446 6965 6c64 720d  .....ListFieldr.
-000006f0: 0000 00da 0c42 6f6f 6c65 616e 4669 656c  .....BooleanFiel
-00000700: 64da 0b63 6c65 6172 5f63 6163 6865 7224  d..clear_cacher$
-00000710: 0000 0072 2c00 0000 722f 0000 0072 0f00  ...r,...r/...r..
-00000720: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
-00000730: 0072 1200 0000 1600 0000 7310 0000 0008  .r........s.....
-00000740: 0210 020e 020c 0110 0210 0308 0b08 0772  ...............r
-00000750: 1200 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00000760: 0000 0000 0005 0000 0040 0000 0073 7c00  .........@...s|.
-00000770: 0000 6500 5a01 6400 5a02 6503 6a04 6401  ..e.Z.d.Z.e.j.d.
-00000780: 6402 6403 6404 8d03 5a05 6503 6a04 6401  d.d.d...Z.e.j.d.
-00000790: 6402 6403 6404 8d03 5a06 6503 6a07 6508  d.d.d...Z.e.j.e.
-000007a0: 6403 6405 8d02 5a09 6503 6a0a 6503 a00b  d.d...Z.e.j.e...
-000007b0: a100 6403 6406 8d02 5a0c 6503 6a0d 6403  ..d.d...Z.e.j.d.
-000007c0: 6407 8d01 5a0e 6503 6a0d 6403 6407 8d01  d...Z.e.j.d.d...
-000007d0: 5a0f 6503 6a0a 6402 6700 6403 6408 8d03  Z.e.j.d.g.d.d...
-000007e0: 5a10 6409 640a 8400 5a11 640b 5300 290c  Z.d.d...Z.d.S.).
-000007f0: da1f 436c 7573 7465 7243 6f6e 7465 6e74  ..ClusterContent
-00000800: 5265 7175 6573 7453 6572 6961 6c69 7a65  RequestSerialize
-00000810: 7272 1300 0000 4654 7214 0000 0072 1800  rr....FTr....r..
-00000820: 0000 2902 da05 6368 696c 6472 1700 0000  ..)...childr....
-00000830: 721a 0000 0072 1b00 0000 6302 0000 0000  r....r....c.....
-00000840: 0000 0000 0000 0002 0000 0002 0000 0043  ...............C
-00000850: 0000 0073 0c00 0000 7400 7c01 8301 0100  ...s....t.|.....
-00000860: 7c01 5300 7225 0000 0072 2d00 0000 722e  |.S.r%...r-...r.
-00000870: 0000 0072 0f00 0000 720f 0000 0072 1000  ...r....r....r..
-00000880: 0000 722f 0000 0045 0000 0073 0400 0000  ..r/...E...s....
-00000890: 0001 0801 7a30 436c 7573 7465 7243 6f6e  ....z0ClusterCon
-000008a0: 7465 6e74 5265 7175 6573 7453 6572 6961  tentRequestSeria
-000008b0: 6c69 7a65 722e 7661 6c69 6461 7465 5f66  lizer.validate_f
-000008c0: 696c 7465 7273 4e29 1272 3000 0000 7231  iltersN).r0...r1
-000008d0: 0000 0072 3200 0000 7203 0000 0072 3300  ...r2...r....r3.
-000008e0: 0000 7234 0000 00da 0a69 6e70 7574 5f73  ..r4.....input_s
-000008f0: 7269 6472 3500 0000 7206 0000 0072 1c00  ridr5...r....r..
-00000900: 0000 7237 0000 00da 0c49 6e74 6567 6572  ..r7.....Integer
-00000910: 4669 656c 64da 0369 6473 da0a 466c 6f61  Field..ids..Floa
-00000920: 7446 6965 6c64 da01 78da 0179 720d 0000  tField..x..yr...
-00000930: 0072 2f00 0000 720f 0000 0072 0f00 0000  .r/...r....r....
-00000940: 720f 0000 0072 1000 0000 723a 0000 0039  r....r....r:...9
-00000950: 0000 0073 1000 0000 0802 1001 1002 0e02  ...s............
-00000960: 1201 0c01 0c01 1002 723a 0000 0029 0eda  ........r:...)..
-00000970: 0b64 6a61 6e67 6f2e 636f 6e66 7202 0000  .django.confr...
-00000980: 00da 0e72 6573 745f 6672 616d 6577 6f72  ...rest_framewor
-00000990: 6b72 0300 0000 7226 0000 005a 0c6a 736f  kr....r&...Z.jso
-000009a0: 6e5f 7363 6865 6d61 7372 0500 0000 da16  n_schemasr......
-000009b0: 616e 7963 6c75 7374 6572 2e64 6566 696e  anycluster.defin
-000009c0: 6974 696f 6e73 7206 0000 0072 0700 0000  itionsr....r....
-000009d0: 7211 0000 00da 0a53 6572 6961 6c69 7a65  r......Serialize
-000009e0: 7272 1200 0000 723a 0000 0072 0f00 0000  rr....r:...r....
-000009f0: 720f 0000 0072 0f00 0000 7210 0000 00da  r....r....r.....
-00000a00: 083c 6d6f 6475 6c65 3e01 0000 0073 0e00  .<module>....s..
-00000a10: 0000 0c01 0c02 0802 0c02 1003 080b 1223  ...............#
+00000210: 7208 0000 00a9 0072 0e00 0000 fa58 2f68  r......r.....X/h
+00000220: 6f6d 652f 746f 6d2f 6c6f 6361 6c63 6f73  ome/tom/localcos
+00000230: 6d6f 732d 776f 726b 7370 6163 652f 636f  mos-workspace/co
+00000240: 6465 2f6c 6f63 616c 636f 736d 6f73 2d69  de/localcosmos-i
+00000250: 6e73 7469 7475 7465 2f61 6e79 636c 7573  nstitute/anyclus
+00000260: 7465 722f 6170 692f 7365 7269 616c 697a  ter/api/serializ
+00000270: 6572 732e 7079 da13 6669 6c74 6572 735f  ers.py..filters_
+00000280: 6172 655f 616c 6c6f 7765 640b 0000 0073  are_allowed....s
+00000290: 0c00 0000 0002 0801 0c01 0401 0a02 0a01  ................
+000002a0: 7210 0000 0063 0000 0000 0000 0000 0000  r....c..........
+000002b0: 0000 0000 0000 0500 0000 4000 0000 736e  ..........@...sn
+000002c0: 0000 0065 005a 0164 005a 0265 036a 0464  ...e.Z.d.Z.e.j.d
+000002d0: 0164 0264 0364 048d 035a 0565 036a 0665  .d.d.d...Z.e.j.e
+000002e0: 0764 0364 058d 025a 0865 036a 0964 0364  .d.d...Z.e.j.d.d
+000002f0: 068d 015a 0a65 036a 0b64 0267 0064 0364  ...Z.e.j.d.g.d.d
+00000300: 078d 035a 0c65 036a 0d64 0264 0264 0364  ...Z.e.j.d.d.d.d
+00000310: 048d 035a 0e64 0864 0984 005a 0f64 0a64  ...Z.d.d...Z.d.d
+00000320: 0b84 005a 1064 0c64 0d84 005a 1164 0e53  ...Z.d.d...Z.d.S
+00000330: 0029 0fda 1843 6c75 7374 6572 5265 7175  .)...ClusterRequ
+00000340: 6573 7453 6572 6961 6c69 7a65 72fa 0945  estSerializer..E
+00000350: 5053 473a 3433 3236 4654 a903 da07 6465  PSG:4326FT....de
+00000360: 6661 756c 74da 0872 6571 7569 7265 64da  fault..required.
+00000370: 0a77 7269 7465 5f6f 6e6c 79a9 02da 0763  .write_only....c
+00000380: 686f 6963 6573 7216 0000 00a9 0172 1600  hoicesr......r..
+00000390: 0000 a903 7215 0000 0072 1400 0000 7216  ....r....r....r.
+000003a0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+000003b0: 0400 0000 0300 0000 4300 0000 733e 0000  ........C...s>..
+000003c0: 007c 0164 0119 0074 006b 0272 3a7c 0164  .|.d...t.k.r:|.d
+000003d0: 0219 007d 027c 0264 0319 0064 0419 0064  ...}.|.d...d...d
+000003e0: 0519 007d 0374 017c 0383 0164 066b 0273  ...}.t.|...d.k.s
+000003f0: 3a74 02a0 0364 07a1 0182 017c 0153 0029  :t...d.....|.S.)
+00000400: 084e da0d 6765 6f6d 6574 7279 5f74 7970  .N..geometry_typ
+00000410: 65da 0767 656f 6a73 6f6e da08 6765 6f6d  e..geojson..geom
+00000420: 6574 7279 da0b 636f 6f72 6469 6e61 7465  etry..coordinate
+00000430: 7372 0100 0000 e905 0000 007a 2156 6965  sr.........z!Vie
+00000440: 7770 6f72 7420 6d75 7374 2063 6f6e 7369  wport must consi
+00000450: 7374 206f 6620 3520 706f 696e 7473 2904  st of 5 points).
+00000460: 7207 0000 00da 036c 656e 7203 0000 0072  r......lenr....r
+00000470: 0a00 0000 2904 da04 7365 6c66 da04 6461  ....)...self..da
+00000480: 7461 721c 0000 0072 1e00 0000 720e 0000  tar....r....r...
+00000490: 0072 0e00 0000 720f 0000 00da 0876 616c  .r....r......val
+000004a0: 6964 6174 6522 0000 0073 0c00 0000 0001  idate"...s......
+000004b0: 0c02 0801 1001 0c01 0a02 7a21 436c 7573  ..........z!Clus
+000004c0: 7465 7252 6571 7565 7374 5365 7269 616c  terRequestSerial
+000004d0: 697a 6572 2e76 616c 6964 6174 6563 0200  izer.validatec..
+000004e0: 0000 0000 0000 0000 0000 0400 0000 0a00  ................
+000004f0: 0000 4300 0000 7348 0000 007a 1074 00a0  ..C...sH...z.t..
+00000500: 017c 0174 02a1 027d 0257 006e 3204 0074  .|.t...}.W.n2..t
+00000510: 006a 036a 046b 0a72 4201 007d 0301 007a  .j.j.k.rB..}...z
+00000520: 1074 05a0 047c 036a 06a1 0182 0157 0035  .t...|.j.....W.5
+00000530: 0064 007d 037e 0358 0059 006e 0258 007c  .d.}.~.X.Y.n.X.|
+00000540: 0153 00a9 014e 2907 da0a 6a73 6f6e 7363  .S...N)...jsonsc
+00000550: 6865 6d61 7223 0000 0072 0500 0000 da0a  hemar#...r......
+00000560: 6578 6365 7074 696f 6e73 720a 0000 0072  exceptionsr....r
+00000570: 0300 0000 da07 6d65 7373 6167 6529 0472  ......message).r
+00000580: 2100 0000 da05 7661 6c75 65da 0869 735f  !.....value..is_
+00000590: 7661 6c69 64da 0165 720e 0000 0072 0e00  valid..er....r..
+000005a0: 0000 720f 0000 00da 1076 616c 6964 6174  ..r......validat
+000005b0: 655f 6765 6f6a 736f 6e2d 0000 0073 0a00  e_geojson-...s..
+000005c0: 0000 0001 0201 1001 1401 1e01 7a29 436c  ............z)Cl
+000005d0: 7573 7465 7252 6571 7565 7374 5365 7269  usterRequestSeri
+000005e0: 616c 697a 6572 2e76 616c 6964 6174 655f  alizer.validate_
+000005f0: 6765 6f6a 736f 6e63 0200 0000 0000 0000  geojsonc........
+00000600: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
+00000610: 730c 0000 0074 007c 0183 0101 007c 0153  s....t.|.....|.S
+00000620: 0072 2400 0000 a901 7210 0000 00a9 0272  .r$.....r......r
+00000630: 2100 0000 7228 0000 0072 0e00 0000 720e  !...r(...r....r.
+00000640: 0000 0072 0f00 0000 da10 7661 6c69 6461  ...r......valida
+00000650: 7465 5f66 696c 7465 7273 3400 0000 7304  te_filters4...s.
+00000660: 0000 0000 0108 017a 2943 6c75 7374 6572  .......z)Cluster
+00000670: 5265 7175 6573 7453 6572 6961 6c69 7a65  RequestSerialize
+00000680: 722e 7661 6c69 6461 7465 5f66 696c 7465  r.validate_filte
+00000690: 7273 4e29 12da 085f 5f6e 616d 655f 5fda  rsN)...__name__.
+000006a0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+000006b0: 7561 6c6e 616d 655f 5f72 0300 0000 da09  ualname__r......
+000006c0: 4368 6172 4669 656c 64da 0b6f 7574 7075  CharField..outpu
+000006d0: 745f 7372 6964 da0b 4368 6f69 6365 4669  t_srid..ChoiceFi
+000006e0: 656c 6472 0600 0000 721b 0000 00da 094a  eldr....r......J
+000006f0: 534f 4e46 6965 6c64 721c 0000 00da 094c  SONFieldr......L
+00000700: 6973 7446 6965 6c64 720c 0000 00da 0c42  istFieldr......B
+00000710: 6f6f 6c65 616e 4669 656c 64da 0b63 6c65  ooleanField..cle
+00000720: 6172 5f63 6163 6865 7223 0000 0072 2b00  ar_cacher#...r+.
+00000730: 0000 722e 0000 0072 0e00 0000 720e 0000  ..r....r....r...
+00000740: 0072 0e00 0000 720f 0000 0072 1100 0000  .r....r....r....
+00000750: 1600 0000 7310 0000 0008 0210 020e 020c  ....s...........
+00000760: 0110 0210 0308 0b08 0772 1100 0000 6300  .........r....c.
+00000770: 0000 0000 0000 0000 0000 0000 0000 0005  ................
+00000780: 0000 0040 0000 0073 7c00 0000 6500 5a01  ...@...s|...e.Z.
+00000790: 6400 5a02 6503 6a04 6401 6402 6403 6404  d.Z.e.j.d.d.d.d.
+000007a0: 8d03 5a05 6503 6a04 6401 6402 6403 6404  ..Z.e.j.d.d.d.d.
+000007b0: 8d03 5a06 6503 6a07 6508 6403 6405 8d02  ..Z.e.j.e.d.d...
+000007c0: 5a09 6503 6a0a 6503 a00b a100 6403 6406  Z.e.j.e.....d.d.
+000007d0: 8d02 5a0c 6503 6a0d 6403 6407 8d01 5a0e  ..Z.e.j.d.d...Z.
+000007e0: 6503 6a0d 6403 6407 8d01 5a0f 6503 6a0a  e.j.d.d...Z.e.j.
+000007f0: 6402 6700 6403 6408 8d03 5a10 6409 640a  d.g.d.d...Z.d.d.
+00000800: 8400 5a11 640b 5300 290c da1f 436c 7573  ..Z.d.S.)...Clus
+00000810: 7465 7243 6f6e 7465 6e74 5265 7175 6573  terContentReques
+00000820: 7453 6572 6961 6c69 7a65 7272 1200 0000  tSerializerr....
+00000830: 4654 7213 0000 0072 1700 0000 2902 da05  FTr....r....)...
+00000840: 6368 696c 6472 1600 0000 7219 0000 0072  childr....r....r
+00000850: 1a00 0000 6302 0000 0000 0000 0000 0000  ....c...........
+00000860: 0002 0000 0002 0000 0043 0000 0073 0c00  .........C...s..
+00000870: 0000 7400 7c01 8301 0100 7c01 5300 7224  ..t.|.....|.S.r$
+00000880: 0000 0072 2c00 0000 722d 0000 0072 0e00  ...r,...r-...r..
+00000890: 0000 720e 0000 0072 0f00 0000 722e 0000  ..r....r....r...
+000008a0: 0045 0000 0073 0400 0000 0001 0801 7a30  .E...s........z0
+000008b0: 436c 7573 7465 7243 6f6e 7465 6e74 5265  ClusterContentRe
+000008c0: 7175 6573 7453 6572 6961 6c69 7a65 722e  questSerializer.
+000008d0: 7661 6c69 6461 7465 5f66 696c 7465 7273  validate_filters
+000008e0: 4e29 1272 2f00 0000 7230 0000 0072 3100  N).r/...r0...r1.
+000008f0: 0000 7203 0000 0072 3200 0000 7233 0000  ..r....r2...r3..
+00000900: 00da 0a69 6e70 7574 5f73 7269 6472 3400  ...input_sridr4.
+00000910: 0000 7206 0000 0072 1b00 0000 7236 0000  ..r....r....r6..
+00000920: 00da 0c49 6e74 6567 6572 4669 656c 64da  ...IntegerField.
+00000930: 0369 6473 da0a 466c 6f61 7446 6965 6c64  .ids..FloatField
+00000940: da01 78da 0179 720c 0000 0072 2e00 0000  ..x..yr....r....
+00000950: 720e 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
+00000960: 0f00 0000 7239 0000 0039 0000 0073 1000  ....r9...9...s..
+00000970: 0000 0802 1001 1002 0e02 1201 0c01 0c01  ................
+00000980: 1002 7239 0000 0029 0eda 0b64 6a61 6e67  ..r9...)...djang
+00000990: 6f2e 636f 6e66 7202 0000 00da 0e72 6573  o.confr......res
+000009a0: 745f 6672 616d 6577 6f72 6b72 0300 0000  t_frameworkr....
+000009b0: 7225 0000 00da 0c6a 736f 6e5f 7363 6865  r%.....json_sche
+000009c0: 6d61 7372 0500 0000 da16 616e 7963 6c75  masr......anyclu
+000009d0: 7374 6572 2e64 6566 696e 6974 696f 6e73  ster.definitions
+000009e0: 7206 0000 0072 0700 0000 7210 0000 00da  r....r....r.....
+000009f0: 0a53 6572 6961 6c69 7a65 7272 1100 0000  .Serializerr....
+00000a00: 7239 0000 0072 0e00 0000 720e 0000 0072  r9...r....r....r
+00000a10: 0e00 0000 720f 0000 00da 083c 6d6f 6475  ....r......<modu
+00000a20: 6c65 3e01 0000 0073 0e00 0000 0c01 0c02  le>....s........
+00000a30: 0802 0c02 1003 080b 1223                 .........#
```

### Comparing `anycluster-2.0.0/anycluster/api/__pycache__/urls.cpython-38.pyc` & `anycluster-2.1.0/anycluster/api/__pycache__/urls.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Mar 17 13:31:28 2023 UTC, .py size: 882 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 b06b 1464 7203 0000  U........k.dr...
+00000000: 550d 0d0a 0000 0000 687a 4664 7203 0000  U.......hzFdr...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000a 0000 0040 0000 0073 a600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6403 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6501 6405 6505 6a06 a007 a100 6406  ..e.d.e.j.....d.
 00000060: 6407 8d03 6501 6408 6505 6a08 a007 a100  d...e.d.e.j.....
 00000070: 6409 6407 8d03 6501 640a 6505 6a09 a007  d.d...e.d.e.j...
@@ -14,46 +14,47 @@
 000000d0: 6414 5300 2915 e900 0000 0029 01da 0470  d.S.)......)...p
 000000e0: 6174 6829 01da 1666 6f72 6d61 745f 7375  ath)...format_su
 000000f0: 6666 6978 5f70 6174 7465 726e 73e9 0100  ffix_patterns...
 00000100: 0000 2901 da05 7669 6577 73da 005a 1361  ..)...views..Z.a
 00000110: 6e79 636c 7573 7465 725f 6170 695f 686f  nycluster_api_ho
 00000120: 6d65 2901 da04 6e61 6d65 7a20 6772 6964  me)...namez grid
 00000130: 2f3c 696e 743a 7a6f 6f6d 3e2f 3c69 6e74  /<int:zoom>/<int
-00000140: 3a67 7269 645f 7369 7a65 3e2f 5a0c 6772  :grid_size>/Z.gr
+00000140: 3a67 7269 645f 7369 7a65 3e2f da0c 6772  :grid_size>/..gr
 00000150: 6964 5f63 6c75 7374 6572 7a22 6b6d 6561  id_clusterz"kmea
 00000160: 6e73 2f3c 696e 743a 7a6f 6f6d 3e2f 3c69  ns/<int:zoom>/<i
-00000170: 6e74 3a67 7269 645f 7369 7a65 3e2f 5a0e  nt:grid_size>/Z.
+00000170: 6e74 3a67 7269 645f 7369 7a65 3e2f da0e  nt:grid_size>/..
 00000180: 6b6d 6561 6e73 5f63 6c75 7374 6572 7a36  kmeans_clusterz6
 00000190: 6765 742d 6b6d 6561 6e73 2d63 6c75 7374  get-kmeans-clust
 000001a0: 6572 2d63 6f6e 7465 6e74 2f3c 696e 743a  er-content/<int:
 000001b0: 7a6f 6f6d 3e2f 3c69 6e74 3a67 7269 645f  zoom>/<int:grid_
-000001c0: 7369 7a65 3e2f 5a1a 6765 745f 6b6d 6561  size>/Z.get_kmea
+000001c0: 7369 7a65 3e2f da1a 6765 745f 6b6d 6561  size>/..get_kmea
 000001d0: 6e73 5f63 6c75 7374 6572 5f63 6f6e 7465  ns_cluster_conte
 000001e0: 6e74 7a2c 6765 742d 6172 6561 2d63 6f6e  ntz,get-area-con
 000001f0: 7465 6e74 2f3c 696e 743a 7a6f 6f6d 3e2f  tent/<int:zoom>/
 00000200: 3c69 6e74 3a67 7269 645f 7369 7a65 3e2f  <int:grid_size>/
-00000210: 5a10 6765 745f 6172 6561 5f63 6f6e 7465  Z.get_area_conte
+00000210: da10 6765 745f 6172 6561 5f63 6f6e 7465  ..get_area_conte
 00000220: 6e74 7a40 6765 742d 6461 7461 7365 742d  ntz@get-dataset-
 00000230: 636f 6e74 656e 742f 3c69 6e74 3a7a 6f6f  content/<int:zoo
 00000240: 6d3e 2f3c 696e 743a 6772 6964 5f73 697a  m>/<int:grid_siz
 00000250: 653e 2f3c 696e 743a 6461 7461 7365 745f  e>/<int:dataset_
-00000260: 6964 3e2f 5a13 6765 745f 6461 7461 7365  id>/Z.get_datase
+00000260: 6964 3e2f da13 6765 745f 6461 7461 7365  id>/..get_datase
 00000270: 745f 636f 6e74 656e 74da 046a 736f 6e29  t_content..json)
 00000280: 01da 0761 6c6c 6f77 6564 4e29 0eda 0b64  ...allowedN)...d
 00000290: 6a61 6e67 6f2e 7572 6c73 7202 0000 005a  jango.urlsr....Z
 000002a0: 1a72 6573 745f 6672 616d 6577 6f72 6b2e  .rest_framework.
 000002b0: 7572 6c70 6174 7465 726e 7372 0300 0000  urlpatternsr....
-000002c0: 7206 0000 0072 0500 0000 5a07 4150 4948  r....r....Z.APIH
-000002d0: 6f6d 65da 0761 735f 7669 6577 5a0b 4772  ome..as_viewZ.Gr
-000002e0: 6964 436c 7573 7465 725a 0d4b 6d65 616e  idClusterZ.Kmean
-000002f0: 7343 6c75 7374 6572 5a11 4765 7443 6c75  sClusterZ.GetClu
-00000300: 7374 6572 436f 6e74 656e 745a 0e47 6574  sterContentZ.Get
-00000310: 4172 6561 436f 6e74 656e 745a 1147 6574  AreaContentZ.Get
+000002c0: 7206 0000 0072 0500 0000 da07 4150 4948  r....r......APIH
+000002d0: 6f6d 65da 0761 735f 7669 6577 da0b 4772  ome..as_view..Gr
+000002e0: 6964 436c 7573 7465 72da 0d4b 6d65 616e  idCluster..Kmean
+000002f0: 7343 6c75 7374 6572 da11 4765 7443 6c75  sCluster..GetClu
+00000300: 7374 6572 436f 6e74 656e 74da 0e47 6574  sterContent..Get
+00000310: 4172 6561 436f 6e74 656e 74da 1147 6574  AreaContent..Get
 00000320: 4461 7461 7365 7443 6f6e 7465 6e74 da0b  DatasetContent..
-00000330: 7572 6c70 6174 7465 726e 73a9 0072 0d00  urlpatterns..r..
-00000340: 0000 720d 0000 00fa 302f 686f 6d65 2f74  ..r.....0/home/t
+00000330: 7572 6c70 6174 7465 726e 73a9 0072 1800  urlpatterns..r..
+00000340: 0000 7218 0000 00fa 372f 686f 6d65 2f74  ..r.....7/home/t
 00000350: 6f6d 2f61 6e79 636c 7573 7465 722f 6465  om/anycluster/de
-00000360: 6d6f 2f61 6e79 636c 7573 7465 722f 6170  mo/anycluster/ap
-00000370: 692f 7572 6c73 2e70 79da 083c 6d6f 6475  i/urls.py..<modu
-00000380: 6c65 3e01 0000 0073 2000 0000 0c01 0c02  le>....s .......
-00000390: 0c03 1201 1201 1201 0c01 02ff 0402 0c01  ................
-000003a0: 02ff 0402 0c01 02ff 04f8 040c            ............
+00000360: 6d6f 2f64 6a61 6e67 6f2f 616e 7963 6c75  mo/django/anyclu
+00000370: 7374 6572 2f61 7069 2f75 726c 732e 7079  ster/api/urls.py
+00000380: da08 3c6d 6f64 756c 653e 0100 0000 7320  ..<module>....s 
+00000390: 0000 000c 010c 020c 0312 0112 0112 010c  ................
+000003a0: 0102 ff04 020c 0102 ff04 020c 0102 ff04  ................
+000003b0: f804 0c                                  ...
```

### Comparing `anycluster-2.0.0/anycluster/api/__pycache__/views.cpython-38.pyc` & `anycluster-2.1.0/anycluster/api/__pycache__/views.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Apr 19 10:29:29 2023 UTC, .py size: 7179 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 89c2 3f64 0b1c 0000  U.........?d....
+00000000: 550d 0d0a 0000 0000 5e74 4664 9b1c 0000  U.......^tFd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 0001 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 0100 6400 6406 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6400 6407 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
@@ -38,326 +38,339 @@
 00000250: 6400 5a02 6401 6402 8400 5a03 6403 5300  d.Z.d.d...Z.d.S.
 00000260: 2904 da07 4150 4948 6f6d 6563 0200 0000  )...APIHomec....
 00000270: 0000 0000 0000 0000 0400 0000 0300 0000  ................
 00000280: 4f00 0000 730c 0000 0074 0064 0164 0269  O...s....t.d.d.i
 00000290: 0183 0153 0029 034e da07 7375 6363 6573  ...S.).N..succes
 000002a0: 7354 7204 0000 0029 04da 0473 656c 66da  sTr....)...self.
 000002b0: 0772 6571 7565 7374 da04 6172 6773 da06  .request..args..
-000002c0: 6b77 6172 6773 a900 7218 0000 00fa 382f  kwargs..r.....8/
-000002d0: 686f 6d65 2f74 6f6d 2f61 6e79 636c 7573  home/tom/anyclus
-000002e0: 7465 722f 6465 6d6f 2f64 6a61 6e67 6f2f  ter/demo/django/
-000002f0: 616e 7963 6c75 7374 6572 2f61 7069 2f76  anycluster/api/v
-00000300: 6965 7773 2e70 79da 0367 6574 1300 0000  iews.py..get....
-00000310: 7302 0000 0000 017a 0b41 5049 486f 6d65  s......z.APIHome
-00000320: 2e67 6574 4ea9 04da 085f 5f6e 616d 655f  .getN....__name_
-00000330: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00000340: 5f71 7561 6c6e 616d 655f 5f72 1a00 0000  _qualname__r....
-00000350: 7218 0000 0072 1800 0000 7218 0000 0072  r....r....r....r
-00000360: 1900 0000 7212 0000 0011 0000 0073 0200  ....r........s..
-00000370: 0000 0802 7212 0000 0063 0000 0000 0000  ....r....c......
-00000380: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
-00000390: 0000 7338 0000 0065 005a 0164 005a 0264  ..s8...e.Z.d.Z.d
-000003a0: 015a 0364 0264 0384 005a 0464 0464 0584  .Z.d.d...Z.d.d..
-000003b0: 005a 0564 0664 0784 005a 0664 0864 0984  .Z.d.d...Z.d.d..
-000003c0: 005a 0764 0a64 0b84 005a 0864 0c53 0029  .Z.d.d...Z.d.S.)
-000003d0: 0dda 124d 6170 436c 7573 7465 7256 6965  ...MapClusterVie
-000003e0: 7742 6173 655a 1061 6e79 636c 7573 7465  wBaseZ.anycluste
-000003f0: 725f 6361 6368 6563 0200 0000 0000 0000  r_cachec........
-00000400: 0000 0000 0300 0000 0400 0000 4300 0000  ............C...
-00000410: 7316 0000 0074 007c 01a0 0164 01a1 0164  s....t.|...d...d
-00000420: 0219 0083 017d 027c 0253 0029 034e fa01  .....}.|.S.).N..
-00000430: 3ae9 ffff ffff 2902 da03 696e 74da 0573  :.....)...int..s
-00000440: 706c 6974 2903 7214 0000 005a 0873 7269  plit).r....Z.sri
-00000450: 645f 7374 72da 0b6f 7574 7075 745f 7372  d_str..output_sr
-00000460: 6964 7218 0000 0072 1800 0000 7219 0000  idr....r....r...
-00000470: 00da 0a70 6172 7365 5f73 7269 641b 0000  ...parse_srid...
-00000480: 0073 0400 0000 0001 1201 7a1d 4d61 7043  .s........z.MapC
-00000490: 6c75 7374 6572 5669 6577 4261 7365 2e70  lusterViewBase.p
-000004a0: 6172 7365 5f73 7269 6463 0700 0000 0000  arse_sridc......
-000004b0: 0000 0000 0000 0c00 0000 0700 0000 4b00  ..............K.
-000004c0: 0000 734e 0000 007c 0764 0119 007d 087c  ..sN...|.d...}.|
-000004d0: 0764 0219 007d 097c 0464 036b 0272 2a74  .d...}.|.d.k.r*t
-000004e0: 007c 017c 097c 027c 0364 048d 047d 0a6e  .|.|.|.|.d...}.n
-000004f0: 127c 00a0 017c 017c 097c 027c 067c 03a1  .|...|.|.|.|.|..
-00000500: 057d 0a74 027c 0a7c 087c 0564 058d 037d  .}.t.|.|.|.d...}
-00000510: 0b7c 0b53 0029 064e da09 6772 6964 5f73  .|.S.).N..grid_s
-00000520: 697a 65da 047a 6f6f 6d54 a901 da07 6669  ize..zoomT....fi
-00000530: 6c74 6572 7329 0272 2600 0000 7224 0000  lters).r&...r$..
-00000540: 0029 0372 1100 0000 da09 6765 745f 6361  .).r......get_ca
-00000550: 6368 6572 0900 0000 290c 7214 0000 00da  cher....).r.....
-00000560: 0d67 656f 6d65 7472 795f 7479 7065 da0b  .geometry_type..
-00000570: 636c 7573 7465 7274 7970 6572 2900 0000  clustertyper)...
-00000580: da0b 636c 6561 725f 6361 6368 6572 2400  ..clear_cacher$.
-00000590: 0000 7215 0000 0072 1700 0000 7226 0000  ..r....r....r&..
-000005a0: 0072 2700 0000 da0d 636c 7573 7465 725f  .r'.....cluster_
-000005b0: 6361 6368 655a 0963 6c75 7374 6572 6572  cacheZ.clusterer
-000005c0: 7218 0000 0072 1800 0000 7219 0000 00da  r....r....r.....
-000005d0: 1167 6574 5f6d 6170 5f63 6c75 7374 6572  .get_map_cluster
-000005e0: 6572 2000 0000 730e 0000 0000 0208 0108  er ...s.........
-000005f0: 0208 0112 0212 010e 017a 244d 6170 436c  .........z$MapCl
-00000600: 7573 7465 7256 6965 7742 6173 652e 6765  usterViewBase.ge
-00000610: 745f 6d61 705f 636c 7573 7465 7265 7263  t_map_clustererc
-00000620: 0600 0000 0000 0000 0000 0000 0800 0000  ................
-00000630: 0600 0000 4300 0000 732e 0000 007c 046a  ....C...s....|.j
-00000640: 00a0 017c 006a 0269 00a1 027d 0674 037c  ...|.j.i...}.t.|
-00000650: 017c 027c 037c 0564 018d 047d 077c 07a0  .|.|.|.d...}.|..
-00000660: 047c 06a1 0101 007c 0753 0029 024e 7228  .|.....|.S.).Nr(
-00000670: 0000 0029 05da 0773 6573 7369 6f6e 721a  ...)...sessionr.
-00000680: 0000 00da 0a63 6163 6865 5f6e 616d 6572  .....cache_namer
-00000690: 1100 0000 da0f 6c6f 6164 5f67 656f 6d65  ......load_geome
-000006a0: 7472 6965 7329 0872 1400 0000 722b 0000  tries).r....r+..
-000006b0: 0072 2700 0000 722c 0000 0072 1500 0000  .r'...r,...r....
-000006c0: 7229 0000 00da 0663 6163 6865 6472 2e00  r).....cachedr..
-000006d0: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
-000006e0: 0072 2a00 0000 2d00 0000 7308 0000 0000  .r*...-...s.....
-000006f0: 0110 0110 020a 017a 1c4d 6170 436c 7573  .......z.MapClus
-00000700: 7465 7256 6965 7742 6173 652e 6765 745f  terViewBase.get_
-00000710: 6361 6368 6563 0300 0000 0000 0000 0000  cachec..........
-00000720: 0000 0400 0000 0300 0000 4300 0000 7318  ..........C...s.
-00000730: 0000 007c 02a0 00a1 007d 037c 037c 016a  ...|.....}.|.|.j
-00000740: 017c 006a 023c 0064 0053 0029 014e 2903  .|.j.<.d.S.).N).
-00000750: da09 7365 7269 616c 697a 6572 3000 0000  ..serializer0...
-00000760: 7231 0000 0029 0472 1400 0000 7215 0000  r1...).r....r...
-00000770: 0072 2e00 0000 5a12 636c 7573 7465 725f  .r....Z.cluster_
-00000780: 6361 6368 655f 6a73 6f6e 7218 0000 0072  cache_jsonr....r
-00000790: 1800 0000 7219 0000 00da 0973 6574 5f63  ....r......set_c
-000007a0: 6163 6865 3500 0000 7304 0000 0000 0108  ache5...s.......
-000007b0: 017a 1c4d 6170 436c 7573 7465 7256 6965  .z.MapClusterVie
-000007c0: 7742 6173 652e 7365 745f 6361 6368 6563  wBase.set_cachec
-000007d0: 0300 0000 0000 0000 0000 0000 0500 0000  ................
-000007e0: 0500 0000 4300 0000 7322 0000 007c 01a0  ....C...s"...|..
-000007f0: 00a1 007d 0374 016a 0264 017c 027c 0364  ...}.t.j.d.|.|.d
-00000800: 028d 037d 0474 03a0 047c 04a1 0153 0029  ...}.t...|...S.)
-00000810: 034e da04 6a73 6f6e a901 da06 6669 656c  .N..json....fiel
-00000820: 6473 2905 da13 6765 745f 6769 735f 6669  ds)...get_gis_fi
-00000830: 656c 645f 6e61 6d65 7372 0200 0000 7234  eld_namesr....r4
-00000840: 0000 0072 3600 0000 da05 6c6f 6164 7329  ...r6.....loads)
-00000850: 0572 1400 0000 da0d 6d61 705f 636c 7573  .r......map_clus
-00000860: 7465 7265 725a 0e69 6e73 7461 6e63 6573  tererZ.instances
-00000870: 5f6c 6973 74da 1173 6572 6961 6c69 7a65  _list..serialize
-00000880: 725f 6669 656c 6473 da04 6461 7461 7218  r_fields..datar.
-00000890: 0000 0072 1800 0000 7219 0000 00da 1873  ...r....r......s
-000008a0: 6572 6961 6c69 7a65 5f67 6973 5f6d 6f64  erialize_gis_mod
-000008b0: 656c 5f6c 6973 743a 0000 0073 0600 0000  el_list:...s....
-000008c0: 0002 0801 1002 7a2b 4d61 7043 6c75 7374  ......z+MapClust
-000008d0: 6572 5669 6577 4261 7365 2e73 6572 6961  erViewBase.seria
-000008e0: 6c69 7a65 5f67 6973 5f6d 6f64 656c 5f6c  lize_gis_model_l
-000008f0: 6973 744e 2909 721c 0000 0072 1d00 0000  istN).r....r....
-00000900: 721e 0000 0072 3100 0000 7225 0000 0072  r....r1...r%...r
-00000910: 2f00 0000 722a 0000 0072 3500 0000 723e  /...r*...r5...r>
-00000920: 0000 0072 1800 0000 7218 0000 0072 1800  ...r....r....r..
-00000930: 0000 7219 0000 0072 1f00 0000 1700 0000  ..r....r........
-00000940: 730c 0000 0008 0204 0208 0508 0d08 0808  s...............
-00000950: 0572 1f00 0000 6300 0000 0000 0000 0000  .r....c.........
-00000960: 0000 0000 0000 0002 0000 0040 0000 0073  ...........@...s
-00000970: 2200 0000 6500 5a01 6400 5a02 6700 5a03  "...e.Z.d.Z.g.Z.
-00000980: 6700 5a04 6505 6701 5a06 6401 6402 8400  g.Z.e.g.Z.d.d...
-00000990: 5a07 6403 5300 2904 da0b 4772 6964 436c  Z.d.S.)...GridCl
-000009a0: 7573 7465 7263 0200 0000 0000 0000 0000  usterc..........
-000009b0: 0000 0c00 0000 0700 0000 4f00 0000 739c  ..........O...s.
-000009c0: 0000 0074 007c 016a 0164 018d 017d 047c  ...t.|.j.d...}.|
-000009d0: 04a0 02a1 0072 8c7c 046a 0364 0219 007d  .....r.|.j.d...}
-000009e0: 057c 00a0 047c 046a 0364 0319 00a1 017d  .|...|.j.d.....}
-000009f0: 067c 046a 0364 0419 007d 077c 006a 0574  .|.j.d...}.|.j.t
-00000a00: 0674 077c 077c 057c 067c 0166 067c 038e  .t.|.|.|.|.f.|..
-00000a10: 017d 087c 046a 0364 0519 007d 097c 0364  .}.|.j.d...}.|.d
-00000a20: 0619 007d 0a7c 08a0 087c 097c 0a7c 07a1  ...}.|...|.|.|..
-00000a30: 037d 0b7c 00a0 097c 017c 086a 0aa1 0201  .}.|...|.|.j....
-00000a40: 0074 0b7c 0b74 0c6a 0d64 078d 0253 0074  .t.|.t.j.d...S.t
-00000a50: 0b7c 046a 0e74 0c6a 0f64 078d 0253 0029  .|.j.t.j.d...S.)
-00000a60: 084e a901 723d 0000 0072 2d00 0000 7224  .N..r=...r-...r$
-00000a70: 0000 0072 2900 0000 da07 6765 6f6a 736f  ...r).....geojso
-00000a80: 6e72 2700 0000 7207 0000 0029 1072 0f00  nr'...r....).r..
-00000a90: 0000 723d 0000 00da 0869 735f 7661 6c69  ..r=.....is_vali
-00000aa0: 64da 0e76 616c 6964 6174 6564 5f64 6174  d..validated_dat
-00000ab0: 6172 2500 0000 722f 0000 0072 0a00 0000  ar%...r/...r....
-00000ac0: 720c 0000 00da 0c67 7269 645f 636c 7573  r......grid_clus
-00000ad0: 7465 7272 3500 0000 722e 0000 0072 0500  terr5...r....r..
-00000ae0: 0000 7208 0000 00da 0b48 5454 505f 3230  ..r......HTTP_20
-00000af0: 305f 4f4b da06 6572 726f 7273 da14 4854  0_OK..errors..HT
-00000b00: 5450 5f34 3030 5f42 4144 5f52 4551 5545  TP_400_BAD_REQUE
-00000b10: 5354 290c 7214 0000 0072 1500 0000 7216  ST).r....r....r.
-00000b20: 0000 0072 1700 0000 da0a 7365 7269 616c  ...r......serial
-00000b30: 697a 6572 722d 0000 0072 2400 0000 7229  izerr-...r$...r)
-00000b40: 0000 0072 3b00 0000 7241 0000 0072 2700  ...r;...rA...r'.
-00000b50: 0000 da04 6772 6964 7218 0000 0072 1800  ....gridr....r..
-00000b60: 0000 7219 0000 00da 0470 6f73 744b 0000  ..r......postK..
-00000b70: 0073 2200 0000 0002 0c02 0802 0a01 1002  .s".............
-00000b80: 0a02 0c01 0200 02ff 0201 02ff 0403 0a01  ................
-00000b90: 0802 0e02 0e01 0e02 7a10 4772 6964 436c  ........z.GridCl
-00000ba0: 7573 7465 722e 706f 7374 4e29 0872 1c00  uster.postN).r..
-00000bb0: 0000 721d 0000 0072 1e00 0000 5a16 6175  ..r....r....Z.au
-00000bc0: 7468 656e 7469 6361 7469 6f6e 5f63 6c61  thentication_cla
-00000bd0: 7373 6573 5a12 7065 726d 6973 7369 6f6e  ssesZ.permission
-00000be0: 5f63 6c61 7373 6573 7206 0000 00da 1072  _classesr......r
-00000bf0: 656e 6465 7265 725f 636c 6173 7365 7372  enderer_classesr
-00000c00: 4a00 0000 7218 0000 0072 1800 0000 7218  J...r....r....r.
-00000c10: 0000 0072 1900 0000 723f 0000 0045 0000  ...r....r?...E..
-00000c20: 0073 0800 0000 0802 0401 0401 0602 723f  .s............r?
-00000c30: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000c40: 0000 0000 0200 0000 4000 0000 7314 0000  ........@...s...
-00000c50: 0065 005a 0164 005a 0264 0164 0284 005a  .e.Z.d.Z.d.d...Z
-00000c60: 0364 0353 0029 04da 0d4b 6d65 616e 7343  .d.S.)...KmeansC
-00000c70: 6c75 7374 6572 6302 0000 0000 0000 0000  lusterc.........
-00000c80: 0000 000d 0000 0007 0000 004f 0000 0073  ...........O...s
-00000c90: a200 0000 7400 7c01 6a01 6401 8d01 7d04  ....t.|.j.d...}.
-00000ca0: 7c04 a002 a100 7292 7c04 6a03 6402 1900  |.....r.|.j.d...
-00000cb0: 7d05 7c04 6a03 6403 1900 7d06 7c00 a004  }.|.j.d...}.|...
-00000cc0: 7c04 6a03 6404 1900 a101 7d07 7c04 6a03  |.j.d.....}.|.j.
-00000cd0: 6405 1900 7d08 7c00 6a05 7c05 7406 7c08  d...}.|.j.|.t.|.
-00000ce0: 7c06 7c07 7c01 6606 7c03 8e01 7d09 7c04  |.|.|.f.|...}.|.
-00000cf0: 6a03 6406 1900 7d0a 7c03 6407 1900 7d0b  j.d...}.|.d...}.
-00000d00: 7c09 a007 7c0a 7c05 7c0b 7c08 a104 7d0c  |...|.|.|.|...}.
-00000d10: 7c00 a008 7c01 7c09 6a09 a102 0100 740a  |...|.|.j.....t.
-00000d20: 7c0c 8301 5300 740a 7c04 6a0b 740c 6a0d  |...S.t.|.j.t.j.
-00000d30: 6408 8d02 5300 2909 4e72 4000 0000 722b  d...S.).Nr@...r+
-00000d40: 0000 0072 2d00 0000 7224 0000 0072 2900  ...r-...r$...r).
-00000d50: 0000 7241 0000 0072 2700 0000 7207 0000  ..rA...r'...r...
-00000d60: 0029 0e72 0f00 0000 723d 0000 0072 4200  .).r....r=...rB.
-00000d70: 0000 7243 0000 0072 2500 0000 722f 0000  ..rC...r%...r/..
-00000d80: 0072 0d00 0000 da0e 6b6d 6561 6e73 5f63  .r......kmeans_c
-00000d90: 6c75 7374 6572 7235 0000 0072 2e00 0000  lusterr5...r....
-00000da0: 7205 0000 0072 4600 0000 7208 0000 0072  r....rF...r....r
-00000db0: 4700 0000 290d 7214 0000 0072 1500 0000  G...).r....r....
-00000dc0: 7216 0000 0072 1700 0000 7248 0000 0072  r....r....rH...r
-00000dd0: 2b00 0000 722d 0000 0072 2400 0000 7229  +...r-...r$...r)
-00000de0: 0000 0072 3b00 0000 7241 0000 0072 2700  ...r;...rA...r'.
-00000df0: 0000 da07 6d61 726b 6572 7372 1800 0000  ....markersr....
-00000e00: 7218 0000 0072 1900 0000 724a 0000 0067  r....r....rJ...g
-00000e10: 0000 0073 2200 0000 0002 0c02 0802 0a01  ...s"...........
-00000e20: 0a01 1002 0a02 0e01 02ff 0201 02ff 0403  ................
-00000e30: 0a01 0802 1001 0e01 0802 7a12 4b6d 6561  ..........z.Kmea
-00000e40: 6e73 436c 7573 7465 722e 706f 7374 4ea9  nsCluster.postN.
-00000e50: 0472 1c00 0000 721d 0000 0072 1e00 0000  .r....r....r....
-00000e60: 724a 0000 0072 1800 0000 7218 0000 0072  rJ...r....r....r
-00000e70: 1800 0000 7219 0000 0072 4c00 0000 6500  ....r....rL...e.
-00000e80: 0000 7302 0000 0008 0272 4c00 0000 6300  ..s......rL...c.
-00000e90: 0000 0000 0000 0000 0000 0000 0000 0002  ................
-00000ea0: 0000 0040 0000 0073 1400 0000 6500 5a01  ...@...s....e.Z.
-00000eb0: 6400 5a02 6401 6402 8400 5a03 6403 5300  d.Z.d.d...Z.d.S.
-00000ec0: 2904 da11 4765 7443 6c75 7374 6572 436f  )...GetClusterCo
-00000ed0: 6e74 656e 7463 0200 0000 0000 0000 0000  ntentc..........
-00000ee0: 0000 1000 0000 0900 0000 4f00 0000 73c2  ..........O...s.
-00000ef0: 0000 0074 007c 016a 0164 018d 017d 047c  ...t.|.j.d...}.|
-00000f00: 04a0 02a1 0072 b27c 046a 0364 0219 007d  .....r.|.j.d...}
-00000f10: 057c 00a0 047c 046a 0364 0319 00a1 017d  .|...|.j.d.....}
-00000f20: 067c 00a0 047c 046a 0364 0419 00a1 017d  .|...|.j.d.....}
-00000f30: 077c 046a 0364 0519 007d 087c 006a 057c  .|.j.d...}.|.j.|
-00000f40: 0574 067c 0864 067c 067c 0166 067c 038e  .t.|.d.|.|.f.|..
-00000f50: 017d 097c 046a 0364 0719 007d 0a7c 046a  .}.|.j.d...}.|.j
-00000f60: 0364 0819 007d 0b7c 046a 0364 0919 007d  .d...}.|.j.d...}
-00000f70: 0c7c 0364 0a19 007d 0d7c 096a 077c 057c  .|.d...}.|.j.|.|
-00000f80: 0a7c 0b7c 0c7c 087c 0d7c 0764 0b8d 077d  .|.|.|.|.|.d...}
-00000f90: 0e7c 00a0 087c 097c 0ea1 027d 0f74 097c  .|...|.|...}.t.|
-00000fa0: 0f83 0153 0074 097c 046a 0a74 0b6a 0c64  ...S.t.|.j.t.j.d
-00000fb0: 0c8d 0253 0029 0d4e 7240 0000 0072 2b00  ...S.).Nr@...r+.
-00000fc0: 0000 7224 0000 00da 0a69 6e70 7574 5f73  ..r$.....input_s
-00000fd0: 7269 6472 2900 0000 46da 0369 6473 da01  ridr)...F..ids..
-00000fe0: 78da 0179 7227 0000 0029 0172 5100 0000  x..yr'...).rQ...
-00000ff0: 7207 0000 0029 0d72 1000 0000 723d 0000  r....).r....r=..
-00001000: 0072 4200 0000 7243 0000 0072 2500 0000  .rB...rC...r%...
-00001010: 722f 0000 0072 0d00 0000 da1a 6765 745f  r/...r......get_
-00001020: 6b6d 6561 6e73 5f63 6c75 7374 6572 5f63  kmeans_cluster_c
-00001030: 6f6e 7465 6e74 723e 0000 0072 0500 0000  ontentr>...r....
-00001040: 7246 0000 0072 0800 0000 7247 0000 0029  rF...r....rG...)
-00001050: 1072 1400 0000 7215 0000 0072 1600 0000  .r....r....r....
-00001060: 7217 0000 0072 4800 0000 722b 0000 0072  r....rH...r+...r
-00001070: 2400 0000 7251 0000 0072 2900 0000 723b  $...rQ...r)...r;
-00001080: 0000 0072 5200 0000 7253 0000 0072 5400  ...rR...rS...rT.
-00001090: 0000 7227 0000 005a 0f63 6c75 7374 6572  ..r'...Z.cluster
-000010a0: 5f63 6f6e 7465 6e74 723d 0000 0072 1800  _contentr=...r..
-000010b0: 0000 7218 0000 0072 1900 0000 724a 0000  ..r....r....rJ..
-000010c0: 0085 0000 0073 2a00 0000 0002 0c02 0802  .....s*.........
-000010d0: 0a01 1001 1002 0a02 0e01 02ff 0201 02ff  ................
-000010e0: 0403 0a01 0a01 0a02 0802 1001 02ff 0603  ................
-000010f0: 0c02 0802 7a16 4765 7443 6c75 7374 6572  ....z.GetCluster
-00001100: 436f 6e74 656e 742e 706f 7374 4e72 4f00  Content.postNrO.
-00001110: 0000 7218 0000 0072 1800 0000 7218 0000  ..r....r....r...
-00001120: 0072 1900 0000 7250 0000 0083 0000 0073  .r....rP.......s
-00001130: 0200 0000 0802 7250 0000 0063 0000 0000  ......rP...c....
-00001140: 0000 0000 0000 0000 0000 0000 0200 0000  ................
-00001150: 4000 0000 7314 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
-00001160: 0264 0164 0284 005a 0364 0353 0029 04da  .d.d...Z.d.S.)..
-00001170: 0e47 6574 4172 6561 436f 6e74 656e 7463  .GetAreaContentc
-00001180: 0200 0000 0000 0000 0000 0000 0c00 0000  ................
-00001190: 0700 0000 4f00 0000 738a 0000 0074 007c  ....O...s....t.|
-000011a0: 016a 0164 018d 017d 047c 04a0 02a1 0072  .j.d...}.|.....r
-000011b0: 7a7c 046a 0364 0219 007d 057c 00a0 047c  z|.j.d...}.|...|
-000011c0: 046a 0364 0319 00a1 017d 067c 046a 0364  .j.d.....}.|.j.d
-000011d0: 0419 007d 077c 006a 057c 0574 067c 0764  ...}.|.j.|.t.|.d
-000011e0: 057c 067c 0166 067c 038e 017d 087c 046a  .|.|.f.|...}.|.j
-000011f0: 0364 0619 007d 097c 08a0 077c 097c 07a1  .d...}.|...|.|..
-00001200: 027d 0a7c 00a0 087c 087c 0aa1 027d 0b74  .}.|...|.|...}.t
-00001210: 097c 0b83 0153 0074 097c 046a 0a74 0b6a  .|...S.t.|.j.t.j
-00001220: 0c64 078d 0253 0029 084e 7240 0000 0072  .d...S.).Nr@...r
-00001230: 2b00 0000 7224 0000 0072 2900 0000 4672  +...r$...r)...Fr
-00001240: 4100 0000 7207 0000 0029 0d72 0f00 0000  A...r....).r....
-00001250: 723d 0000 0072 4200 0000 7243 0000 0072  r=...rB...rC...r
-00001260: 2500 0000 722f 0000 0072 0d00 0000 da10  %...r/...r......
-00001270: 6765 745f 6172 6561 5f63 6f6e 7465 6e74  get_area_content
-00001280: 723e 0000 0072 0500 0000 7246 0000 0072  r>...r....rF...r
-00001290: 0800 0000 7247 0000 0029 0c72 1400 0000  ....rG...).r....
-000012a0: 7215 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
-000012b0: 4800 0000 722b 0000 0072 2400 0000 7229  H...r+...r$...r)
-000012c0: 0000 0072 3b00 0000 7241 0000 005a 0c61  ...r;...rA...Z.a
-000012d0: 7265 615f 636f 6e74 656e 7472 3d00 0000  rea_contentr=...
-000012e0: 7218 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
-000012f0: 4a00 0000 aa00 0000 731e 0000 0000 020c  J.......s.......
-00001300: 0208 020a 0110 020a 020e 0102 ff02 0102  ................
-00001310: ff04 030a 020c 020c 0208 027a 1347 6574  ...........z.Get
-00001320: 4172 6561 436f 6e74 656e 742e 706f 7374  AreaContent.post
-00001330: 4e72 4f00 0000 7218 0000 0072 1800 0000  NrO...r....r....
-00001340: 7218 0000 0072 1900 0000 7256 0000 00a8  r....r....rV....
-00001350: 0000 0073 0200 0000 0802 7256 0000 0063  ...s......rV...c
-00001360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001370: 0200 0000 4000 0000 7314 0000 0065 005a  ....@...s....e.Z
-00001380: 0164 005a 0264 0164 0284 005a 0364 0353  .d.Z.d.d...Z.d.S
-00001390: 0029 04da 1147 6574 4461 7461 7365 7443  .)...GetDatasetC
-000013a0: 6f6e 7465 6e74 6302 0000 0000 0000 0000  ontentc.........
-000013b0: 0000 000b 0000 0007 0000 004f 0000 0073  ...........O...s
-000013c0: 6200 0000 7c01 6a00 a001 6401 6402 a102  b...|.j...d.d...
-000013d0: 7d04 6700 7d05 7c00 6a02 7403 7404 7c05  }.g.}.|.j.t.t.|.
-000013e0: 6403 7c04 7c01 6606 7c03 8e01 7d06 7c03  d.|.|.f.|...}.|.
-000013f0: 6404 1900 7d07 7c06 a005 7c07 a101 7d08  d...}.|...|...}.
-00001400: 7c06 a006 a100 7d09 7407 6a08 6405 7c08  |.....}.t.j.d.|.
-00001410: 7c09 6406 8d03 7d0a 7409 740a a00b 7c0a  |.d...}.t.t...|.
-00001420: a101 8301 5300 2907 4e72 2400 0000 69e6  ....S.).Nr$...i.
-00001430: 1000 0046 da0a 6461 7461 7365 745f 6964  ...F..dataset_id
-00001440: 7236 0000 0072 3700 0000 290c da03 4745  r6...r7...)...GE
-00001450: 5472 1a00 0000 722f 0000 0072 0a00 0000  Tr....r/...r....
-00001460: 720c 0000 00da 1367 6574 5f64 6174 6173  r......get_datas
-00001470: 6574 5f63 6f6e 7465 6e74 7239 0000 0072  et_contentr9...r
-00001480: 0200 0000 7234 0000 0072 0500 0000 7236  ....r4...r....r6
-00001490: 0000 0072 3a00 0000 290b 7214 0000 0072  ...r:...).r....r
-000014a0: 1500 0000 7216 0000 0072 1700 0000 7224  ....r....r....r$
-000014b0: 0000 0072 2900 0000 723b 0000 0072 5900  ...r)...r;...rY.
-000014c0: 0000 5a07 6461 7461 7365 7472 3c00 0000  ..Z.datasetr<...
-000014d0: 723d 0000 0072 1800 0000 7218 0000 0072  r=...r....r....r
-000014e0: 1900 0000 721a 0000 00c6 0000 0073 1800  ....r........s..
-000014f0: 0000 0002 0e02 0402 0e01 02ff 0201 02ff  ................
-00001500: 0403 0802 0a02 0801 1002 7a15 4765 7444  ..........z.GetD
-00001510: 6174 6173 6574 436f 6e74 656e 742e 6765  atasetContent.ge
-00001520: 744e 721b 0000 0072 1800 0000 7218 0000  tNr....r....r...
-00001530: 0072 1800 0000 7219 0000 0072 5800 0000  .r....r....rX...
-00001540: c400 0000 7302 0000 0008 0272 5800 0000  ....s......rX...
-00001550: 291d da0b 646a 616e 676f 2e63 6f72 6572  )...django.corer
-00001560: 0200 0000 da14 7265 7374 5f66 7261 6d65  ......rest_frame
-00001570: 776f 726b 2e76 6965 7773 7203 0000 005a  work.viewsr....Z
-00001580: 1772 6573 745f 6672 616d 6577 6f72 6b2e  .rest_framework.
-00001590: 7265 7370 6f6e 7365 7205 0000 00da 1872  responser......r
-000015a0: 6573 745f 6672 616d 6577 6f72 6b2e 7265  est_framework.re
-000015b0: 6e64 6572 6572 7372 0600 0000 da0e 7265  nderersr......re
-000015c0: 7374 5f66 7261 6d65 776f 726b 7208 0000  st_frameworkr...
-000015d0: 005a 1761 6e79 636c 7573 7465 722e 4d61  .Z.anycluster.Ma
-000015e0: 7043 6c75 7374 6572 6572 7209 0000 00da  pClustererr.....
-000015f0: 1661 6e79 636c 7573 7465 722e 6465 6669  .anycluster.defi
-00001600: 6e69 7469 6f6e 7372 0a00 0000 720b 0000  nitionsr....r...
-00001610: 0072 0c00 0000 720d 0000 0072 0f00 0000  .r....r....r....
-00001620: 7210 0000 00da 0a61 6e79 636c 7573 7465  r......anycluste
-00001630: 7272 1100 0000 7236 0000 0072 1200 0000  rr....r6...r....
-00001640: 721f 0000 0072 3f00 0000 724c 0000 0072  r....r?...rL...r
-00001650: 5000 0000 7256 0000 0072 5800 0000 7218  P...rV...rX...r.
-00001660: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
-00001670: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00001680: 7320 0000 000c 020c 010c 010c 010c 020c  s ..............
-00001690: 0118 0210 020c 0208 0210 060e 2e12 2012  .............. .
-000016a0: 1e12 2512 1c                             ..%..
+000002c0: 6b77 6172 6773 a900 7218 0000 00fa 522f  kwargs..r.....R/
+000002d0: 686f 6d65 2f74 6f6d 2f6c 6f63 616c 636f  home/tom/localco
+000002e0: 736d 6f73 2d77 6f72 6b73 7061 6365 2f63  smos-workspace/c
+000002f0: 6f64 652f 6c6f 6361 6c63 6f73 6d6f 732d  ode/localcosmos-
+00000300: 696e 7374 6974 7574 652f 616e 7963 6c75  institute/anyclu
+00000310: 7374 6572 2f61 7069 2f76 6965 7773 2e70  ster/api/views.p
+00000320: 79da 0367 6574 1300 0000 7302 0000 0000  y..get....s.....
+00000330: 017a 0b41 5049 486f 6d65 2e67 6574 4ea9  .z.APIHome.getN.
+00000340: 04da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+00000350: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+00000360: 616d 655f 5f72 1a00 0000 7218 0000 0072  ame__r....r....r
+00000370: 1800 0000 7218 0000 0072 1900 0000 7212  ....r....r....r.
+00000380: 0000 0011 0000 0073 0200 0000 0802 7212  .......s......r.
+00000390: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+000003a0: 0000 0000 0200 0000 4000 0000 7340 0000  ........@...s@..
+000003b0: 0065 005a 0164 005a 0264 015a 0364 0264  .e.Z.d.Z.d.Z.d.d
+000003c0: 0384 005a 0464 0464 0584 005a 0564 0664  ...Z.d.d...Z.d.d
+000003d0: 0784 005a 0664 0864 0984 005a 0764 0a64  ...Z.d.d...Z.d.d
+000003e0: 0b84 005a 0864 0c64 0d84 005a 0964 0e53  ...Z.d.d...Z.d.S
+000003f0: 0029 0fda 124d 6170 436c 7573 7465 7256  .)...MapClusterV
+00000400: 6965 7742 6173 655a 1061 6e79 636c 7573  iewBaseZ.anyclus
+00000410: 7465 725f 6361 6368 6563 0200 0000 0000  ter_cachec......
+00000420: 0000 0000 0000 0300 0000 0400 0000 4300  ..............C.
+00000430: 0000 7316 0000 0074 007c 01a0 0164 01a1  ..s....t.|...d..
+00000440: 0164 0219 0083 017d 027c 0253 0029 034e  .d.....}.|.S.).N
+00000450: fa01 3ae9 ffff ffff 2902 da03 696e 74da  ..:.....)...int.
+00000460: 0573 706c 6974 2903 7214 0000 00da 0873  .split).r......s
+00000470: 7269 645f 7374 72da 0b6f 7574 7075 745f  rid_str..output_
+00000480: 7372 6964 7218 0000 0072 1800 0000 7219  sridr....r....r.
+00000490: 0000 00da 0a70 6172 7365 5f73 7269 641b  .....parse_srid.
+000004a0: 0000 0073 0400 0000 0001 1201 7a1d 4d61  ...s........z.Ma
+000004b0: 7043 6c75 7374 6572 5669 6577 4261 7365  pClusterViewBase
+000004c0: 2e70 6172 7365 5f73 7269 6463 0200 0000  .parse_sridc....
+000004d0: 0000 0000 0000 0000 0200 0000 0100 0000  ................
+000004e0: 4300 0000 7304 0000 0064 0153 0029 024e  C...s....d.S.).N
+000004f0: da06 7075 626c 6963 7218 0000 0029 0272  ..publicr....).r
+00000500: 1400 0000 7215 0000 0072 1800 0000 7218  ....r....r....r.
+00000510: 0000 0072 1900 0000 da0f 6765 745f 7363  ...r......get_sc
+00000520: 6865 6d61 5f6e 616d 6520 0000 0073 0200  hema_name ...s..
+00000530: 0000 0001 7a22 4d61 7043 6c75 7374 6572  ....z"MapCluster
+00000540: 5669 6577 4261 7365 2e67 6574 5f73 6368  ViewBase.get_sch
+00000550: 656d 615f 6e61 6d65 6307 0000 0000 0000  ema_namec.......
+00000560: 0000 0000 000d 0000 0007 0000 004b 0000  .............K..
+00000570: 0073 5a00 0000 7c07 6401 1900 7d08 7c07  .sZ...|.d...}.|.
+00000580: 6402 1900 7d09 7c04 6403 6b02 722a 7400  d...}.|.d.k.r*t.
+00000590: 7c01 7c09 7c02 7c03 6404 8d04 7d0a 6e12  |.|.|.|.d...}.n.
+000005a0: 7c00 a001 7c01 7c09 7c02 7c06 7c03 a105  |...|.|.|.|.|...
+000005b0: 7d0a 7c00 a002 7c06 a101 7d0b 7403 7c0a  }.|...|...}.t.|.
+000005c0: 7c08 7c05 7c0b 6405 8d04 7d0c 7c0c 5300  |.|.|.d...}.|.S.
+000005d0: 2906 4eda 0967 7269 645f 7369 7a65 da04  ).N..grid_size..
+000005e0: 7a6f 6f6d 54a9 01da 0766 696c 7465 7273  zoomT....filters
+000005f0: 2903 7229 0000 0072 2500 0000 da0b 7363  ).r)...r%.....sc
+00000600: 6865 6d61 5f6e 616d 6529 0472 1100 0000  hema_name).r....
+00000610: da09 6765 745f 6361 6368 6572 2800 0000  ..get_cacher(...
+00000620: 7209 0000 0029 0d72 1400 0000 da0d 6765  r....).r......ge
+00000630: 6f6d 6574 7279 5f74 7970 65da 0b63 6c75  ometry_type..clu
+00000640: 7374 6572 7479 7065 722c 0000 00da 0b63  stertyper,.....c
+00000650: 6c65 6172 5f63 6163 6865 7225 0000 0072  lear_cacher%...r
+00000660: 1500 0000 7217 0000 0072 2900 0000 722a  ....r....r)...r*
+00000670: 0000 00da 0d63 6c75 7374 6572 5f63 6163  .....cluster_cac
+00000680: 6865 722d 0000 005a 0963 6c75 7374 6572  her-...Z.cluster
+00000690: 6572 7218 0000 0072 1800 0000 7219 0000  err....r....r...
+000006a0: 00da 1167 6574 5f6d 6170 5f63 6c75 7374  ...get_map_clust
+000006b0: 6572 6572 2400 0000 7310 0000 0000 0208  erer$...s.......
+000006c0: 0108 0208 0112 0212 020a 0110 017a 244d  .............z$M
+000006d0: 6170 436c 7573 7465 7256 6965 7742 6173  apClusterViewBas
+000006e0: 652e 6765 745f 6d61 705f 636c 7573 7465  e.get_map_cluste
+000006f0: 7265 7263 0600 0000 0000 0000 0000 0000  rerc............
+00000700: 0800 0000 0600 0000 4300 0000 732e 0000  ........C...s...
+00000710: 007c 046a 00a0 017c 006a 0269 00a1 027d  .|.j...|.j.i...}
+00000720: 0674 037c 017c 027c 037c 0564 018d 047d  .t.|.|.|.|.d...}
+00000730: 077c 07a0 047c 06a1 0101 007c 0753 0029  .|...|.....|.S.)
+00000740: 024e 722b 0000 0029 05da 0773 6573 7369  .Nr+...)...sessi
+00000750: 6f6e 721a 0000 00da 0a63 6163 6865 5f6e  onr......cache_n
+00000760: 616d 6572 1100 0000 da0f 6c6f 6164 5f67  amer......load_g
+00000770: 656f 6d65 7472 6965 7329 0872 1400 0000  eometries).r....
+00000780: 722f 0000 0072 2a00 0000 7230 0000 0072  r/...r*...r0...r
+00000790: 1500 0000 722c 0000 00da 0663 6163 6865  ....r,.....cache
+000007a0: 6472 3200 0000 7218 0000 0072 1800 0000  dr2...r....r....
+000007b0: 7219 0000 0072 2e00 0000 3300 0000 7308  r....r....3...s.
+000007c0: 0000 0000 0110 0110 020a 017a 1c4d 6170  ...........z.Map
+000007d0: 436c 7573 7465 7256 6965 7742 6173 652e  ClusterViewBase.
+000007e0: 6765 745f 6361 6368 6563 0300 0000 0000  get_cachec......
+000007f0: 0000 0000 0000 0400 0000 0300 0000 4300  ..............C.
+00000800: 0000 7318 0000 007c 02a0 00a1 007d 037c  ..s....|.....}.|
+00000810: 037c 016a 017c 006a 023c 0064 0053 0029  .|.j.|.j.<.d.S.)
+00000820: 014e 2903 da09 7365 7269 616c 697a 6572  .N)...serializer
+00000830: 3400 0000 7235 0000 0029 0472 1400 0000  4...r5...).r....
+00000840: 7215 0000 0072 3200 0000 5a12 636c 7573  r....r2...Z.clus
+00000850: 7465 725f 6361 6368 655f 6a73 6f6e 7218  ter_cache_jsonr.
+00000860: 0000 0072 1800 0000 7219 0000 00da 0973  ...r....r......s
+00000870: 6574 5f63 6163 6865 3b00 0000 7304 0000  et_cache;...s...
+00000880: 0000 0108 017a 1c4d 6170 436c 7573 7465  .....z.MapCluste
+00000890: 7256 6965 7742 6173 652e 7365 745f 6361  rViewBase.set_ca
+000008a0: 6368 6563 0300 0000 0000 0000 0000 0000  chec............
+000008b0: 0500 0000 0500 0000 4300 0000 7322 0000  ........C...s"..
+000008c0: 007c 01a0 00a1 007d 0374 016a 0264 017c  .|.....}.t.j.d.|
+000008d0: 027c 0364 028d 037d 0474 03a0 047c 04a1  .|.d...}.t...|..
+000008e0: 0153 0029 034e da04 6a73 6f6e a901 da06  .S.).N..json....
+000008f0: 6669 656c 6473 2905 da13 6765 745f 6769  fields)...get_gi
+00000900: 735f 6669 656c 645f 6e61 6d65 7372 0200  s_field_namesr..
+00000910: 0000 7238 0000 0072 3a00 0000 da05 6c6f  ..r8...r:.....lo
+00000920: 6164 7329 0572 1400 0000 da0d 6d61 705f  ads).r......map_
+00000930: 636c 7573 7465 7265 725a 0e69 6e73 7461  clustererZ.insta
+00000940: 6e63 6573 5f6c 6973 74da 1173 6572 6961  nces_list..seria
+00000950: 6c69 7a65 725f 6669 656c 6473 da04 6461  lizer_fields..da
+00000960: 7461 7218 0000 0072 1800 0000 7219 0000  tar....r....r...
+00000970: 00da 1873 6572 6961 6c69 7a65 5f67 6973  ...serialize_gis
+00000980: 5f6d 6f64 656c 5f6c 6973 7440 0000 0073  _model_list@...s
+00000990: 0600 0000 0002 0801 1002 7a2b 4d61 7043  ..........z+MapC
+000009a0: 6c75 7374 6572 5669 6577 4261 7365 2e73  lusterViewBase.s
+000009b0: 6572 6961 6c69 7a65 5f67 6973 5f6d 6f64  erialize_gis_mod
+000009c0: 656c 5f6c 6973 744e 290a 721c 0000 0072  el_listN).r....r
+000009d0: 1d00 0000 721e 0000 0072 3500 0000 7226  ....r....r5...r&
+000009e0: 0000 0072 2800 0000 7233 0000 0072 2e00  ...r(...r3...r..
+000009f0: 0000 7239 0000 0072 4200 0000 7218 0000  ..r9...rB...r...
+00000a00: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
+00000a10: 721f 0000 0017 0000 0073 0e00 0000 0802  r........s......
+00000a20: 0402 0805 0804 080f 0808 0805 721f 0000  ............r...
+00000a30: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00000a40: 0000 0200 0000 4000 0000 7322 0000 0065  ......@...s"...e
+00000a50: 005a 0164 005a 0267 005a 0367 005a 0465  .Z.d.Z.g.Z.g.Z.e
+00000a60: 0567 015a 0664 0164 0284 005a 0764 0353  .g.Z.d.d...Z.d.S
+00000a70: 0029 04da 0b47 7269 6443 6c75 7374 6572  .)...GridCluster
+00000a80: 6302 0000 0000 0000 0000 0000 000c 0000  c...............
+00000a90: 0007 0000 004f 0000 0073 9c00 0000 7400  .....O...s....t.
+00000aa0: 7c01 6a01 6401 8d01 7d04 7c04 a002 a100  |.j.d...}.|.....
+00000ab0: 728c 7c04 6a03 6402 1900 7d05 7c00 a004  r.|.j.d...}.|...
+00000ac0: 7c04 6a03 6403 1900 a101 7d06 7c04 6a03  |.j.d.....}.|.j.
+00000ad0: 6404 1900 7d07 7c00 6a05 7406 7407 7c07  d...}.|.j.t.t.|.
+00000ae0: 7c05 7c06 7c01 6606 7c03 8e01 7d08 7c04  |.|.|.f.|...}.|.
+00000af0: 6a03 6405 1900 7d09 7c03 6406 1900 7d0a  j.d...}.|.d...}.
+00000b00: 7c08 a008 7c09 7c0a 7c07 a103 7d0b 7c00  |...|.|.|...}.|.
+00000b10: a009 7c01 7c08 6a0a a102 0100 740b 7c0b  ..|.|.j.....t.|.
+00000b20: 740c 6a0d 6407 8d02 5300 740b 7c04 6a0e  t.j.d...S.t.|.j.
+00000b30: 740c 6a0f 6407 8d02 5300 2908 4ea9 0172  t.j.d...S.).N..r
+00000b40: 4100 0000 7231 0000 0072 2500 0000 722c  A...r1...r%...r,
+00000b50: 0000 00da 0767 656f 6a73 6f6e 722a 0000  .....geojsonr*..
+00000b60: 0072 0700 0000 2910 720f 0000 0072 4100  .r....).r....rA.
+00000b70: 0000 da08 6973 5f76 616c 6964 da0e 7661  ....is_valid..va
+00000b80: 6c69 6461 7465 645f 6461 7461 7226 0000  lidated_datar&..
+00000b90: 0072 3300 0000 720a 0000 0072 0c00 0000  .r3...r....r....
+00000ba0: 5a0c 6772 6964 5f63 6c75 7374 6572 7239  Z.grid_clusterr9
+00000bb0: 0000 0072 3200 0000 7205 0000 0072 0800  ...r2...r....r..
+00000bc0: 0000 da0b 4854 5450 5f32 3030 5f4f 4bda  ....HTTP_200_OK.
+00000bd0: 0665 7272 6f72 73da 1448 5454 505f 3430  .errors..HTTP_40
+00000be0: 305f 4241 445f 5245 5155 4553 5429 0c72  0_BAD_REQUEST).r
+00000bf0: 1400 0000 7215 0000 0072 1600 0000 7217  ....r....r....r.
+00000c00: 0000 00da 0a73 6572 6961 6c69 7a65 7272  .....serializerr
+00000c10: 3100 0000 7225 0000 0072 2c00 0000 723f  1...r%...r,...r?
+00000c20: 0000 0072 4500 0000 722a 0000 00da 0467  ...rE...r*.....g
+00000c30: 7269 6472 1800 0000 7218 0000 0072 1900  ridr....r....r..
+00000c40: 0000 da04 706f 7374 5100 0000 7322 0000  ....postQ...s"..
+00000c50: 0000 020c 0208 020a 0110 020a 020c 0102  ................
+00000c60: 0002 ff02 0102 ff04 030a 0108 020e 020e  ................
+00000c70: 010e 027a 1047 7269 6443 6c75 7374 6572  ...z.GridCluster
+00000c80: 2e70 6f73 744e 2908 721c 0000 0072 1d00  .postN).r....r..
+00000c90: 0000 721e 0000 00da 1661 7574 6865 6e74  ..r......authent
+00000ca0: 6963 6174 696f 6e5f 636c 6173 7365 73da  ication_classes.
+00000cb0: 1270 6572 6d69 7373 696f 6e5f 636c 6173  .permission_clas
+00000cc0: 7365 7372 0600 0000 da10 7265 6e64 6572  sesr......render
+00000cd0: 6572 5f63 6c61 7373 6573 724d 0000 0072  er_classesrM...r
+00000ce0: 1800 0000 7218 0000 0072 1800 0000 7219  ....r....r....r.
+00000cf0: 0000 0072 4300 0000 4b00 0000 7308 0000  ...rC...K...s...
+00000d00: 0008 0204 0104 0106 0272 4300 0000 6300  .........rC...c.
+00000d10: 0000 0000 0000 0000 0000 0000 0000 0002  ................
+00000d20: 0000 0040 0000 0073 1400 0000 6500 5a01  ...@...s....e.Z.
+00000d30: 6400 5a02 6401 6402 8400 5a03 6403 5300  d.Z.d.d...Z.d.S.
+00000d40: 2904 da0d 4b6d 6561 6e73 436c 7573 7465  )...KmeansCluste
+00000d50: 7263 0200 0000 0000 0000 0000 0000 0d00  rc..............
+00000d60: 0000 0700 0000 4f00 0000 73a2 0000 0074  ......O...s....t
+00000d70: 007c 016a 0164 018d 017d 047c 04a0 02a1  .|.j.d...}.|....
+00000d80: 0072 927c 046a 0364 0219 007d 057c 046a  .r.|.j.d...}.|.j
+00000d90: 0364 0319 007d 067c 00a0 047c 046a 0364  .d...}.|...|.j.d
+00000da0: 0419 00a1 017d 077c 046a 0364 0519 007d  .....}.|.j.d...}
+00000db0: 087c 006a 057c 0574 067c 087c 067c 077c  .|.j.|.t.|.|.|.|
+00000dc0: 0166 067c 038e 017d 097c 046a 0364 0619  .f.|...}.|.j.d..
+00000dd0: 007d 0a7c 0364 0719 007d 0b7c 09a0 077c  .}.|.d...}.|...|
+00000de0: 0a7c 057c 0b7c 08a1 047d 0c7c 00a0 087c  .|.|.|...}.|...|
+00000df0: 017c 096a 09a1 0201 0074 0a7c 0c83 0153  .|.j.....t.|...S
+00000e00: 0074 0a7c 046a 0b74 0c6a 0d64 088d 0253  .t.|.j.t.j.d...S
+00000e10: 0029 094e 7244 0000 0072 2f00 0000 7231  .).NrD...r/...r1
+00000e20: 0000 0072 2500 0000 722c 0000 0072 4500  ...r%...r,...rE.
+00000e30: 0000 722a 0000 0072 0700 0000 290e 720f  ..r*...r....).r.
+00000e40: 0000 0072 4100 0000 7246 0000 0072 4700  ...rA...rF...rG.
+00000e50: 0000 7226 0000 0072 3300 0000 720d 0000  ..r&...r3...r...
+00000e60: 005a 0e6b 6d65 616e 735f 636c 7573 7465  .Z.kmeans_cluste
+00000e70: 7272 3900 0000 7232 0000 0072 0500 0000  rr9...r2...r....
+00000e80: 7249 0000 0072 0800 0000 724a 0000 0029  rI...r....rJ...)
+00000e90: 0d72 1400 0000 7215 0000 0072 1600 0000  .r....r....r....
+00000ea0: 7217 0000 0072 4b00 0000 722f 0000 0072  r....rK...r/...r
+00000eb0: 3100 0000 7225 0000 0072 2c00 0000 723f  1...r%...r,...r?
+00000ec0: 0000 0072 4500 0000 722a 0000 00da 076d  ...rE...r*.....m
+00000ed0: 6172 6b65 7273 7218 0000 0072 1800 0000  arkersr....r....
+00000ee0: 7219 0000 0072 4d00 0000 6d00 0000 7322  r....rM...m...s"
+00000ef0: 0000 0000 020c 0208 020a 010a 0110 020a  ................
+00000f00: 020e 0102 ff02 0102 ff04 030a 0108 0210  ................
+00000f10: 010e 0108 027a 124b 6d65 616e 7343 6c75  .....z.KmeansClu
+00000f20: 7374 6572 2e70 6f73 744e a904 721c 0000  ster.postN..r...
+00000f30: 0072 1d00 0000 721e 0000 0072 4d00 0000  .r....r....rM...
+00000f40: 7218 0000 0072 1800 0000 7218 0000 0072  r....r....r....r
+00000f50: 1900 0000 7251 0000 006b 0000 0073 0200  ....rQ...k...s..
+00000f60: 0000 0802 7251 0000 0063 0000 0000 0000  ....rQ...c......
+00000f70: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
+00000f80: 0000 7314 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
+00000f90: 0164 0284 005a 0364 0353 0029 04da 1147  .d...Z.d.S.)...G
+00000fa0: 6574 436c 7573 7465 7243 6f6e 7465 6e74  etClusterContent
+00000fb0: 6302 0000 0000 0000 0000 0000 0010 0000  c...............
+00000fc0: 0009 0000 004f 0000 0073 c200 0000 7400  .....O...s....t.
+00000fd0: 7c01 6a01 6401 8d01 7d04 7c04 a002 a100  |.j.d...}.|.....
+00000fe0: 72b2 7c04 6a03 6402 1900 7d05 7c00 a004  r.|.j.d...}.|...
+00000ff0: 7c04 6a03 6403 1900 a101 7d06 7c00 a004  |.j.d.....}.|...
+00001000: 7c04 6a03 6404 1900 a101 7d07 7c04 6a03  |.j.d.....}.|.j.
+00001010: 6405 1900 7d08 7c00 6a05 7c05 7406 7c08  d...}.|.j.|.t.|.
+00001020: 6406 7c06 7c01 6606 7c03 8e01 7d09 7c04  d.|.|.f.|...}.|.
+00001030: 6a03 6407 1900 7d0a 7c04 6a03 6408 1900  j.d...}.|.j.d...
+00001040: 7d0b 7c04 6a03 6409 1900 7d0c 7c03 640a  }.|.j.d...}.|.d.
+00001050: 1900 7d0d 7c09 6a07 7c05 7c0a 7c0b 7c0c  ..}.|.j.|.|.|.|.
+00001060: 7c08 7c0d 7c07 640b 8d07 7d0e 7c00 a008  |.|.|.d...}.|...
+00001070: 7c09 7c0e a102 7d0f 7409 7c0f 8301 5300  |.|...}.t.|...S.
+00001080: 7409 7c04 6a0a 740b 6a0c 640c 8d02 5300  t.|.j.t.j.d...S.
+00001090: 290d 4e72 4400 0000 722f 0000 0072 2500  ).NrD...r/...r%.
+000010a0: 0000 da0a 696e 7075 745f 7372 6964 722c  ....input_sridr,
+000010b0: 0000 0046 da03 6964 73da 0178 da01 7972  ...F..ids..x..yr
+000010c0: 2a00 0000 2901 7255 0000 0072 0700 0000  *...).rU...r....
+000010d0: 290d 7210 0000 0072 4100 0000 7246 0000  ).r....rA...rF..
+000010e0: 0072 4700 0000 7226 0000 0072 3300 0000  .rG...r&...r3...
+000010f0: 720d 0000 005a 1a67 6574 5f6b 6d65 616e  r....Z.get_kmean
+00001100: 735f 636c 7573 7465 725f 636f 6e74 656e  s_cluster_conten
+00001110: 7472 4200 0000 7205 0000 0072 4900 0000  trB...r....rI...
+00001120: 7208 0000 0072 4a00 0000 2910 7214 0000  r....rJ...).r...
+00001130: 0072 1500 0000 7216 0000 0072 1700 0000  .r....r....r....
+00001140: 724b 0000 0072 2f00 0000 7225 0000 0072  rK...r/...r%...r
+00001150: 5500 0000 722c 0000 0072 3f00 0000 7256  U...r,...r?...rV
+00001160: 0000 0072 5700 0000 7258 0000 0072 2a00  ...rW...rX...r*.
+00001170: 0000 5a0f 636c 7573 7465 725f 636f 6e74  ..Z.cluster_cont
+00001180: 656e 7472 4100 0000 7218 0000 0072 1800  entrA...r....r..
+00001190: 0000 7219 0000 0072 4d00 0000 8b00 0000  ..r....rM.......
+000011a0: 732a 0000 0000 020c 0208 020a 0110 0110  s*..............
+000011b0: 020a 020e 0102 ff02 0102 ff04 030a 010a  ................
+000011c0: 010a 0208 0210 0102 ff06 030c 0208 027a  ...............z
+000011d0: 1647 6574 436c 7573 7465 7243 6f6e 7465  .GetClusterConte
+000011e0: 6e74 2e70 6f73 744e 7253 0000 0072 1800  nt.postNrS...r..
+000011f0: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
+00001200: 0072 5400 0000 8900 0000 7302 0000 0008  .rT.......s.....
+00001210: 0272 5400 0000 6300 0000 0000 0000 0000  .rT...c.........
+00001220: 0000 0000 0000 0002 0000 0040 0000 0073  ...........@...s
+00001230: 1400 0000 6500 5a01 6400 5a02 6401 6402  ....e.Z.d.Z.d.d.
+00001240: 8400 5a03 6403 5300 2904 da0e 4765 7441  ..Z.d.S.)...GetA
+00001250: 7265 6143 6f6e 7465 6e74 6302 0000 0000  reaContentc.....
+00001260: 0000 0000 0000 000c 0000 0007 0000 004f  ...............O
+00001270: 0000 0073 8a00 0000 7400 7c01 6a01 6401  ...s....t.|.j.d.
+00001280: 8d01 7d04 7c04 a002 a100 727a 7c04 6a03  ..}.|.....rz|.j.
+00001290: 6402 1900 7d05 7c00 a004 7c04 6a03 6403  d...}.|...|.j.d.
+000012a0: 1900 a101 7d06 7c04 6a03 6404 1900 7d07  ....}.|.j.d...}.
+000012b0: 7c00 6a05 7c05 7406 7c07 6405 7c06 7c01  |.j.|.t.|.d.|.|.
+000012c0: 6606 7c03 8e01 7d08 7c04 6a03 6406 1900  f.|...}.|.j.d...
+000012d0: 7d09 7c08 a007 7c09 7c07 a102 7d0a 7c00  }.|...|.|...}.|.
+000012e0: a008 7c08 7c0a a102 7d0b 7409 7c0b 8301  ..|.|...}.t.|...
+000012f0: 5300 7409 7c04 6a0a 740b 6a0c 6407 8d02  S.t.|.j.t.j.d...
+00001300: 5300 2908 4e72 4400 0000 722f 0000 0072  S.).NrD...r/...r
+00001310: 2500 0000 722c 0000 0046 7245 0000 0072  %...r,...FrE...r
+00001320: 0700 0000 290d 720f 0000 0072 4100 0000  ....).r....rA...
+00001330: 7246 0000 0072 4700 0000 7226 0000 0072  rF...rG...r&...r
+00001340: 3300 0000 720d 0000 005a 1067 6574 5f61  3...r....Z.get_a
+00001350: 7265 615f 636f 6e74 656e 7472 4200 0000  rea_contentrB...
+00001360: 7205 0000 0072 4900 0000 7208 0000 0072  r....rI...r....r
+00001370: 4a00 0000 290c 7214 0000 0072 1500 0000  J...).r....r....
+00001380: 7216 0000 0072 1700 0000 724b 0000 0072  r....r....rK...r
+00001390: 2f00 0000 7225 0000 0072 2c00 0000 723f  /...r%...r,...r?
+000013a0: 0000 0072 4500 0000 5a0c 6172 6561 5f63  ...rE...Z.area_c
+000013b0: 6f6e 7465 6e74 7241 0000 0072 1800 0000  ontentrA...r....
+000013c0: 7218 0000 0072 1900 0000 724d 0000 00b0  r....r....rM....
+000013d0: 0000 0073 1e00 0000 0002 0c02 0802 0a01  ...s............
+000013e0: 1002 0a02 0e01 02ff 0201 02ff 0403 0a02  ................
+000013f0: 0c02 0c02 0802 7a13 4765 7441 7265 6143  ......z.GetAreaC
+00001400: 6f6e 7465 6e74 2e70 6f73 744e 7253 0000  ontent.postNrS..
+00001410: 0072 1800 0000 7218 0000 0072 1800 0000  .r....r....r....
+00001420: 7219 0000 0072 5900 0000 ae00 0000 7302  r....rY.......s.
+00001430: 0000 0008 0272 5900 0000 6300 0000 0000  .....rY...c.....
+00001440: 0000 0000 0000 0000 0000 0002 0000 0040  ...............@
+00001450: 0000 0073 1400 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+00001460: 6401 6402 8400 5a03 6403 5300 2904 da11  d.d...Z.d.S.)...
+00001470: 4765 7444 6174 6173 6574 436f 6e74 656e  GetDatasetConten
+00001480: 7463 0200 0000 0000 0000 0000 0000 0b00  tc..............
+00001490: 0000 0700 0000 4f00 0000 7362 0000 007c  ......O...sb...|
+000014a0: 016a 00a0 0164 0164 02a1 027d 0467 007d  .j...d.d...}.g.}
+000014b0: 057c 006a 0274 0374 047c 0564 037c 047c  .|.j.t.t.|.d.|.|
+000014c0: 0166 067c 038e 017d 067c 0364 0419 007d  .f.|...}.|.d...}
+000014d0: 077c 06a0 057c 07a1 017d 087c 06a0 06a1  .|...|...}.|....
+000014e0: 007d 0974 076a 0864 057c 087c 0964 068d  .}.t.j.d.|.|.d..
+000014f0: 037d 0a74 0974 0aa0 0b7c 0aa1 0183 0153  .}.t.t...|.....S
+00001500: 0029 074e 7225 0000 0069 e610 0000 46da  .).Nr%...i....F.
+00001510: 0a64 6174 6173 6574 5f69 6472 3a00 0000  .dataset_idr:...
+00001520: 723b 0000 0029 0cda 0347 4554 721a 0000  r;...)...GETr...
+00001530: 0072 3300 0000 720a 0000 0072 0c00 0000  .r3...r....r....
+00001540: 5a13 6765 745f 6461 7461 7365 745f 636f  Z.get_dataset_co
+00001550: 6e74 656e 7472 3d00 0000 7202 0000 0072  ntentr=...r....r
+00001560: 3800 0000 7205 0000 0072 3a00 0000 723e  8...r....r:...r>
+00001570: 0000 0029 0b72 1400 0000 7215 0000 0072  ...).r....r....r
+00001580: 1600 0000 7217 0000 0072 2500 0000 722c  ....r....r%...r,
+00001590: 0000 0072 3f00 0000 725b 0000 00da 0764  ...r?...r[.....d
+000015a0: 6174 6173 6574 7240 0000 0072 4100 0000  atasetr@...rA...
+000015b0: 7218 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
+000015c0: 1a00 0000 cc00 0000 7318 0000 0000 020e  ........s.......
+000015d0: 0204 020e 0102 ff02 0102 ff04 0308 020a  ................
+000015e0: 0208 0110 027a 1547 6574 4461 7461 7365  .....z.GetDatase
+000015f0: 7443 6f6e 7465 6e74 2e67 6574 4e72 1b00  tContent.getNr..
+00001600: 0000 7218 0000 0072 1800 0000 7218 0000  ..r....r....r...
+00001610: 0072 1900 0000 725a 0000 00ca 0000 0073  .r....rZ.......s
+00001620: 0200 0000 0802 725a 0000 0029 1dda 0b64  ......rZ...)...d
+00001630: 6a61 6e67 6f2e 636f 7265 7202 0000 00da  jango.corer.....
+00001640: 1472 6573 745f 6672 616d 6577 6f72 6b2e  .rest_framework.
+00001650: 7669 6577 7372 0300 0000 da17 7265 7374  viewsr......rest
+00001660: 5f66 7261 6d65 776f 726b 2e72 6573 706f  _framework.respo
+00001670: 6e73 6572 0500 0000 da18 7265 7374 5f66  nser......rest_f
+00001680: 7261 6d65 776f 726b 2e72 656e 6465 7265  ramework.rendere
+00001690: 7273 7206 0000 00da 0e72 6573 745f 6672  rsr......rest_fr
+000016a0: 616d 6577 6f72 6b72 0800 0000 5a17 616e  ameworkr....Z.an
+000016b0: 7963 6c75 7374 6572 2e4d 6170 436c 7573  ycluster.MapClus
+000016c0: 7465 7265 7272 0900 0000 da16 616e 7963  tererr......anyc
+000016d0: 6c75 7374 6572 2e64 6566 696e 6974 696f  luster.definitio
+000016e0: 6e73 720a 0000 0072 0b00 0000 720c 0000  nsr....r....r...
+000016f0: 0072 0d00 0000 720f 0000 0072 1000 0000  .r....r....r....
+00001700: da0a 616e 7963 6c75 7374 6572 7211 0000  ..anyclusterr...
+00001710: 0072 3a00 0000 7212 0000 0072 1f00 0000  .r:...r....r....
+00001720: 7243 0000 0072 5100 0000 7254 0000 0072  rC...rQ...rT...r
+00001730: 5900 0000 725a 0000 0072 1800 0000 7218  Y...rZ...r....r.
+00001740: 0000 0072 1800 0000 7219 0000 00da 083c  ...r....r......<
+00001750: 6d6f 6475 6c65 3e01 0000 0073 2000 0000  module>....s ...
+00001760: 0c02 0c01 0c01 0c01 0c02 0c01 1802 1002  ................
+00001770: 0c02 0802 1006 0e34 1220 121e 1225 121c  .......4. ...%..
```

### Comparing `anycluster-2.0.0/anycluster/api/json_schemas.py` & `anycluster-2.1.0/anycluster/api/json_schemas.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/api/serializers.py` & `anycluster-2.1.0/anycluster/api/serializers.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/api/tests/__pycache__/common.cpython-38.pyc` & `anycluster-2.1.0/anycluster/api/tests/__pycache__/common.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/api/tests/__pycache__/test_serializers.cpython-38.pyc` & `anycluster-2.1.0/anycluster/api/tests/__pycache__/test_serializers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/api/tests/__pycache__/test_views.cpython-38.pyc` & `anycluster-2.1.0/anycluster/api/tests/__pycache__/test_views.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/api/tests/test_serializers.py` & `anycluster-2.1.0/anycluster/api/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/api/tests/test_views.py` & `anycluster-2.1.0/anycluster/api/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/api/urls.py` & `anycluster-2.1.0/anycluster/api/urls.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/api/views.py` & `anycluster-2.1.0/anycluster/api/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,24 +25,30 @@
     cache_name = 'anycluster_cache'
 
     def parse_srid(self, srid_str):
         output_srid = int(srid_str.split(':')[-1])
         return output_srid
 
 
+    def get_schema_name(self, request):
+        return 'public'
+
+
     def get_map_clusterer(self, geometry_type, clustertype, filters, clear_cache, output_srid, request, **kwargs):
 
         grid_size = kwargs['grid_size']
         zoom = kwargs['zoom']
 
         if clear_cache == True:
             cluster_cache = ClusterCache(geometry_type, zoom, clustertype, filters=filters)
         else:
             cluster_cache = self.get_cache(geometry_type, zoom, clustertype, request, filters)
-        clusterer = MapClusterer(cluster_cache, grid_size=grid_size, output_srid=output_srid)
+
+        schema_name = self.get_schema_name(request)
+        clusterer = MapClusterer(cluster_cache, grid_size=grid_size, output_srid=output_srid, schema_name=schema_name)
         return clusterer
 
 
     def get_cache(self, geometry_type, zoom, clustertype, request, filters):
         cached = request.session.get(self.cache_name, {})
         cluster_cache = ClusterCache(geometry_type, zoom, clustertype, filters=filters)
         # ClusterCache decides if the cache is still valid for the given parameters and loads the cache if so
```

### Comparing `anycluster-2.0.0/anycluster/clusters.py` & `anycluster-2.1.0/anycluster/clusters.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/definitions.py` & `anycluster-2.1.0/anycluster/definitions.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/globalmaptiles.py` & `anycluster-2.1.0/anycluster/globalmaptiles.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/static/anycluster/images/10.png` & `anycluster-2.1.0/anycluster/static/anycluster/images/10.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/static/anycluster/images/100.png` & `anycluster-2.1.0/anycluster/static/anycluster/images/100.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/static/anycluster/images/1000.png` & `anycluster-2.1.0/anycluster/static/anycluster/images/1000.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/static/anycluster/images/10000.png` & `anycluster-2.1.0/anycluster/static/anycluster/images/10000.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/static/anycluster/images/10000_empty.png` & `anycluster-2.1.0/anycluster/static/anycluster/images/10000_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/static/anycluster/images/1000_empty.png` & `anycluster-2.1.0/anycluster/static/anycluster/images/1000_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/static/anycluster/images/100_empty.png` & `anycluster-2.1.0/anycluster/static/anycluster/images/100_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/static/anycluster/images/10_empty.png` & `anycluster-2.1.0/anycluster/static/anycluster/images/10_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/static/anycluster/images/5.png` & `anycluster-2.1.0/anycluster/static/anycluster/images/5.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/static/anycluster/images/50.png` & `anycluster-2.1.0/anycluster/static/anycluster/images/50.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/static/anycluster/images/50_empty.png` & `anycluster-2.1.0/anycluster/static/anycluster/images/50_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/static/anycluster/images/5_empty.png` & `anycluster-2.1.0/anycluster/static/anycluster/images/5_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/static/anycluster/images/pin_unknown.png` & `anycluster-2.1.0/anycluster/static/anycluster/images/pin_unknown.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/tests/__pycache__/common.cpython-38.pyc` & `anycluster-2.1.0/anycluster/tests/__pycache__/common.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/tests/__pycache__/mixins.cpython-38.pyc` & `anycluster-2.1.0/anycluster/tests/__pycache__/mixins.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/tests/__pycache__/test_ClusterCache.cpython-38.pyc` & `anycluster-2.1.0/anycluster/tests/__pycache__/test_ClusterCache.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/tests/__pycache__/test_FilterComposer.cpython-38.pyc` & `anycluster-2.1.0/anycluster/tests/__pycache__/test_FilterComposer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/tests/__pycache__/test_Filters.cpython-38.pyc` & `anycluster-2.1.0/anycluster/tests/__pycache__/test_Filters.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/tests/__pycache__/test_MapClusterer.cpython-38.pyc` & `anycluster-2.1.0/anycluster/tests/__pycache__/test_MapClusterer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/tests/common.py` & `anycluster-2.1.0/anycluster/tests/common.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/tests/mixins.py` & `anycluster-2.1.0/anycluster/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/tests/test_ClusterCache.py` & `anycluster-2.1.0/anycluster/tests/test_ClusterCache.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/tests/test_FilterComposer.py` & `anycluster-2.1.0/anycluster/tests/test_FilterComposer.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster/tests/test_MapClusterer.py` & `anycluster-2.1.0/anycluster/tests/test_MapClusterer.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/anycluster.egg-info/PKG-INFO` & `anycluster-2.1.0/anycluster.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anycluster
-Version: 2.0.0
+Version: 2.1.0
 Summary: anycluster provides Server-Side clustering of map markers for Geodjango
 Home-page: https://github.com/biodiv/anycluster
 Author: Thomas Uher
 Author-email: thomas.uher@sisol-systems.com
 License: The MIT License
 Keywords: django,cluster,kmeans,grid,server-side clustering
 Platform: OS Independent
@@ -14,22 +14,31 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 anycluster (POSTGIS version)
 ============================
 
+[https://anycluster.org](https://anycluster.org)
+
 anycluster provides Server-Side clustering of map markers for Geodjango. It is suitable for large amounts of markers. 
 Depending on your server and personal feeling, it works very well with 200.000 to 500.000 markers.
 
 The postgis version is recommended. There is a mysql version with limited functionality: https://github.com/biodiv/anycluster-mysql
 
 
+Documentation
+-------------
+
+http://anycluster.readthedocs.org/en/latest/
+
+
 ChangeLog
 ---------
+- [22.04.2023] anycluster 2.0 (breaking changes, see docs), npm, Django 4.x, updated docs
 - [09.09.2019] support for Django 2.x and above (python 3), added leaflet support
 - [08.10.2015] major code improvements
 - you now need to add {% csrf_token % } somewhere in your template
 
 
 Features
 --------
@@ -39,44 +48,20 @@
 - clustering based on geometric density of the points (needs PSQL extension)
 - cluster contents of any geographic area defined as Polygon/Multipolygon
 - get all elements contained in a cluster
 
 ... and has a builtin caching mechanism: if the user pans a map, only the new areas are processed.
 
 And lots of optional customization possibilities:
-- works with google maps and Leaflet
+- works with OpenLayers, google maps and Leaflet
 - define what happens if you click on a cluster
 - use your own cluster graphics
 - define gridsize and other cluster parameters
 - apply filters to your clusters
 - use specialized markers/pins if count is 1
 
 
-Documentation
--------------
-
-http://anycluster.readthedocs.org/en/latest/
-
-
-Using the Demo
---------------
-
-To use the demo, follow these steps: 
-
-- install ``Django 2.x`` correctly
-- install ``psycopg2``
-- copy the demo folder to your system and include the anycluster folder as a django app.
-- modify the database connection in ``settings.py`` according to your setup
-- if you want to use google maps: add your google api key to ``anymap/templates/base.html``
-- remember to create the kmeans function as described in the documentation
-- from within the demo folder, run ``python manage.py migrate``
-- from within the demo folder, run ``python manage.py filldemodb 50000`` to fill the database with 50000 points
-- be patient, as this process is not very effective
-- from within the demo folder, run ``python manage.py runserver 8080``
-- open your browser and enter ``localhost:8080``
-
-
 Performance Tips
 ----------------
 
 - index your GIS database columns correctly
 - usage of a SSD can be 10-20 times faster compared to HDD
```

### Comparing `anycluster-2.0.0/anycluster.egg-info/SOURCES.txt` & `anycluster-2.1.0/anycluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anycluster-2.0.0/setup.py` & `anycluster-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     'psycopg2',
     'djangorestframework',
     'jsonschema',
 ]
 
 setup(
     name="anycluster",
-    version='2.0.0',
+    version='2.1.0',
     description='anycluster provides Server-Side clustering of map markers for Geodjango',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='The MIT License',
     platforms=['OS Independent'],
     keywords='django, cluster, kmeans, grid, server-side clustering',
     author='Thomas Uher',
```


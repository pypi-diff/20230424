# Comparing `tmp/pyaemet-1.0.2.tar.gz` & `tmp/pyaemet-1.1.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/jaimedgp/Repositories/pyAEMET/dist/tmpev79huek/pyaemet-1.0.2.tar", last modified: Fri Nov 12 12:18:22 2021, max compression
+gzip compressed data, was "pyaemet-1.1.0rc0.tar", max compression
```

## Comparing `pyaemet-1.0.2.tar` & `pyaemet-1.1.0rc0.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxrwxr-x   0 jaimedgp  (1000) jaimedgp  (1000)        0 2021-11-12 12:18:22.000000 pyaemet-1.0.2/
--rw-rw-r--   0 jaimedgp  (1000) jaimedgp  (1000)     1153 2021-11-12 12:13:58.000000 pyaemet-1.0.2/setup.py
--rw-rw-r--   0 jaimedgp  (1000) jaimedgp  (1000)      100 2021-11-08 18:14:35.000000 pyaemet-1.0.2/pyproject.toml
-drwxrwxr-x   0 jaimedgp  (1000) jaimedgp  (1000)        0 2021-11-12 12:18:22.000000 pyaemet-1.0.2/pyaemet/
--rw-rw-r--   0 jaimedgp  (1000) jaimedgp  (1000)     3251 2021-11-12 12:12:21.000000 pyaemet-1.0.2/pyaemet/utilities.py
--rw-rw-r--   0 jaimedgp  (1000) jaimedgp  (1000)    12966 2021-11-08 18:25:33.000000 pyaemet-1.0.2/pyaemet/valores_climatologicos.py
--rw-rw-r--   0 jaimedgp  (1000) jaimedgp  (1000)     2461 2021-11-08 10:24:54.000000 pyaemet-1.0.2/pyaemet/aemet_api_request.py
--rwxrwxr-x   0 jaimedgp  (1000) jaimedgp  (1000)      483 2021-07-09 15:06:05.000000 pyaemet-1.0.2/pyaemet/apikey_file.py
--rw-rw-r--   0 jaimedgp  (1000) jaimedgp  (1000)      387 2021-11-12 12:14:10.000000 pyaemet-1.0.2/pyaemet/__init__.py
--rw-rw-r--   0 jaimedgp  (1000) jaimedgp  (1000)    35149 2021-07-09 15:04:55.000000 pyaemet-1.0.2/LICENSE
--rw-rw-r--   0 jaimedgp  (1000) jaimedgp  (1000)       38 2021-11-12 12:18:22.000000 pyaemet-1.0.2/setup.cfg
--rw-rw-r--   0 jaimedgp  (1000) jaimedgp  (1000)     6127 2021-11-12 12:18:22.000000 pyaemet-1.0.2/PKG-INFO
-drwxrwxr-x   0 jaimedgp  (1000) jaimedgp  (1000)        0 2021-11-12 12:18:22.000000 pyaemet-1.0.2/pyaemet.egg-info/
--rw-rw-r--   0 jaimedgp  (1000) jaimedgp  (1000)        8 2021-11-12 12:18:22.000000 pyaemet-1.0.2/pyaemet.egg-info/top_level.txt
--rw-rw-r--   0 jaimedgp  (1000) jaimedgp  (1000)       68 2021-11-12 12:18:22.000000 pyaemet-1.0.2/pyaemet.egg-info/requires.txt
--rw-rw-r--   0 jaimedgp  (1000) jaimedgp  (1000)        1 2021-11-12 12:18:22.000000 pyaemet-1.0.2/pyaemet.egg-info/not-zip-safe
--rw-rw-r--   0 jaimedgp  (1000) jaimedgp  (1000)     6127 2021-11-12 12:18:22.000000 pyaemet-1.0.2/pyaemet.egg-info/PKG-INFO
--rw-rw-r--   0 jaimedgp  (1000) jaimedgp  (1000)      352 2021-11-12 12:18:22.000000 pyaemet-1.0.2/pyaemet.egg-info/SOURCES.txt
--rw-rw-r--   0 jaimedgp  (1000) jaimedgp  (1000)        1 2021-11-12 12:18:22.000000 pyaemet-1.0.2/pyaemet.egg-info/dependency_links.txt
--rw-rw-r--   0 jaimedgp  (1000) jaimedgp  (1000)     5530 2021-11-08 18:56:34.000000 pyaemet-1.0.2/README.md
+-rw-r--r--   0        0        0    35149 2022-08-29 18:57:39.634520 pyaemet-1.1.0rc0/LICENSE
+-rw-r--r--   0        0        0     4584 2023-04-24 20:17:14.017440 pyaemet-1.1.0rc0/README.md
+-rw-r--r--   0        0        0     1140 2023-04-24 21:11:23.196165 pyaemet-1.1.0rc0/pyproject.toml
+-rw-r--r--   0        0        0       93 2023-04-24 21:12:23.372714 pyaemet-1.1.0rc0/src/pyaemet/__init__.py
+-rw-r--r--   0        0        0     6050 2023-04-24 20:17:14.025440 pyaemet-1.1.0rc0/src/pyaemet/aemet_request.py
+-rw-r--r--   0        0        0    18982 2023-04-24 20:17:14.025440 pyaemet-1.1.0rc0/src/pyaemet/climatology.py
+-rw-r--r--   0        0        0        0 2023-04-24 20:17:14.025440 pyaemet-1.1.0rc0/src/pyaemet/static/__init__.py
+-rw-r--r--   0        0        0    33781 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc0/src/pyaemet/static/sites/data.csv
+-rw-r--r--   0        0        0     3029 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc0/src/pyaemet/static/sites/metadata.json
+-rw-r--r--   0        0        0        0 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc0/src/pyaemet/types_classes/__init__.py
+-rw-r--r--   0        0        0      866 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc0/src/pyaemet/types_classes/observations.py
+-rw-r--r--   0        0        0    10835 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc0/src/pyaemet/types_classes/sites.py
+-rw-r--r--   0        0        0        0 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc0/src/pyaemet/utilities/__init__.py
+-rw-r--r--   0        0        0     2127 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc0/src/pyaemet/utilities/coordinates.py
+-rw-r--r--   0        0        0     1865 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc0/src/pyaemet/utilities/curation.py
+-rw-r--r--   0        0        0     2511 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc0/src/pyaemet/utilities/dictionaries.py
+-rw-r--r--   0        0        0     5718 1970-01-01 00:00:00.000000 pyaemet-1.1.0rc0/setup.py
+-rw-r--r--   0        0        0     5833 1970-01-01 00:00:00.000000 pyaemet-1.1.0rc0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyaemet-1.0.2/LICENSE` & `pyaemet-1.1.0rc0/LICENSE`

 * *Files identical despite different names*


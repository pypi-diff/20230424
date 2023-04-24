# Comparing `tmp/funman-1.4.0.tar.gz` & `tmp/funman-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funman-1.4.0.tar", last modified: Fri Feb  3 17:05:44 2023, max compression
+gzip compressed data, was "funman-1.5.0.tar", last modified: Mon Apr 24 15:10:11 2023, max compression
```

## Comparing `funman-1.4.0.tar` & `funman-1.5.0.tar`

### file list

```diff
@@ -1,65 +1,68 @@
-drwxr-xr-x   0 danbryce   (501) dialout     (20)        0 2023-02-03 17:05:44.560052 funman-1.4.0/
--rw-r--r--   0 danbryce   (501) dialout     (20)     1043 2022-12-23 20:09:23.000000 funman-1.4.0/LICENSE
--rw-r--r--   0 danbryce   (501) dialout     (20)    10453 2023-02-03 17:05:44.558461 funman-1.4.0/PKG-INFO
--rw-r--r--   0 danbryce   (501) dialout     (20)    10205 2023-01-20 22:15:58.000000 funman-1.4.0/README.md
--rw-r--r--   0 danbryce   (501) dialout     (20)      912 2023-01-20 22:15:58.000000 funman-1.4.0/pyproject.toml
--rw-r--r--   0 danbryce   (501) dialout     (20)       38 2023-02-03 17:05:44.561004 funman-1.4.0/setup.cfg
--rw-r--r--   0 danbryce   (501) dialout     (20)     1141 2022-12-31 21:23:10.000000 funman-1.4.0/setup.py
-drwxr-xr-x   0 danbryce   (501) dialout     (20)        0 2023-02-03 17:05:44.292572 funman-1.4.0/src/
-drwxr-xr-x   0 danbryce   (501) dialout     (20)        0 2023-02-03 17:05:44.348259 funman-1.4.0/src/funman/
--rw-r--r--   0 danbryce   (501) dialout     (20)      375 2023-01-10 20:02:56.000000 funman-1.4.0/src/funman/__init__.py
--rw-r--r--   0 danbryce   (501) dialout     (20)      127 2023-02-03 17:05:41.000000 funman-1.4.0/src/funman/_version.py
-drwxr-xr-x   0 danbryce   (501) dialout     (20)        0 2023-02-03 17:05:44.397693 funman-1.4.0/src/funman/api/
--rw-r--r--   0 danbryce   (501) dialout     (20)       99 2023-01-20 22:15:58.000000 funman-1.4.0/src/funman/api/__init__.py
--rw-r--r--   0 danbryce   (501) dialout     (20)     4907 2023-02-02 21:28:38.000000 funman-1.4.0/src/funman/api/api.py
--rw-r--r--   0 danbryce   (501) dialout     (20)      971 2023-01-20 22:15:58.000000 funman-1.4.0/src/funman/api/client.py
--rw-r--r--   0 danbryce   (501) dialout     (20)      894 2023-02-02 21:33:05.000000 funman-1.4.0/src/funman/api/server.py
--rw-r--r--   0 danbryce   (501) dialout     (20)      205 2023-01-20 22:15:58.000000 funman-1.4.0/src/funman/constants.py
--rw-r--r--   0 danbryce   (501) dialout     (20)     3434 2023-02-02 21:25:59.000000 funman-1.4.0/src/funman/funman.py
-drwxr-xr-x   0 danbryce   (501) dialout     (20)        0 2023-02-03 17:05:44.433166 funman-1.4.0/src/funman/model/
--rw-r--r--   0 danbryce   (501) dialout     (20)      559 2023-01-04 20:33:39.000000 funman-1.4.0/src/funman/model/__init__.py
--rw-r--r--   0 danbryce   (501) dialout     (20)    12716 2023-02-02 21:35:21.000000 funman-1.4.0/src/funman/model/bilayer.py
--rw-r--r--   0 danbryce   (501) dialout     (20)      711 2023-01-30 14:42:47.000000 funman-1.4.0/src/funman/model/encoded.py
--rw-r--r--   0 danbryce   (501) dialout     (20)      667 2023-01-04 20:33:39.000000 funman-1.4.0/src/funman/model/gromet.py
--rw-r--r--   0 danbryce   (501) dialout     (20)      974 2023-01-31 20:04:40.000000 funman-1.4.0/src/funman/model/model.py
--rw-r--r--   0 danbryce   (501) dialout     (20)     1367 2023-01-30 14:42:47.000000 funman-1.4.0/src/funman/model/query.py
--rw-r--r--   0 danbryce   (501) dialout     (20)      477 2023-01-20 22:15:58.000000 funman-1.4.0/src/funman/model/simulator.py
-drwxr-xr-x   0 danbryce   (501) dialout     (20)        0 2023-02-03 17:05:44.441900 funman-1.4.0/src/funman/representation/
--rw-r--r--   0 danbryce   (501) dialout     (20)      141 2023-01-20 22:15:58.000000 funman-1.4.0/src/funman/representation/__init__.py
--rw-r--r--   0 danbryce   (501) dialout     (20)    36475 2023-02-02 21:38:31.000000 funman-1.4.0/src/funman/representation/representation.py
-drwxr-xr-x   0 danbryce   (501) dialout     (20)        0 2023-02-03 17:05:44.465772 funman-1.4.0/src/funman/scenario/
--rw-r--r--   0 danbryce   (501) dialout     (20)      180 2023-01-04 20:33:39.000000 funman-1.4.0/src/funman/scenario/__init__.py
--rw-r--r--   0 danbryce   (501) dialout     (20)     5221 2023-02-02 21:45:51.000000 funman-1.4.0/src/funman/scenario/consistency.py
--rw-r--r--   0 danbryce   (501) dialout     (20)     6258 2023-02-01 13:26:43.000000 funman-1.4.0/src/funman/scenario/parameter_synthesis.py
--rw-r--r--   0 danbryce   (501) dialout     (20)      855 2023-01-20 22:15:58.000000 funman-1.4.0/src/funman/scenario/scenario.py
--rw-r--r--   0 danbryce   (501) dialout     (20)     1591 2023-01-20 22:15:58.000000 funman-1.4.0/src/funman/scenario/simulation.py
-drwxr-xr-x   0 danbryce   (501) dialout     (20)        0 2023-02-03 17:05:44.485726 funman-1.4.0/src/funman/search/
--rw-r--r--   0 danbryce   (501) dialout     (20)      317 2023-01-20 22:15:58.000000 funman-1.4.0/src/funman/search/__init__.py
--rw-r--r--   0 danbryce   (501) dialout     (20)    31672 2023-02-02 19:46:38.000000 funman-1.4.0/src/funman/search/box_search.py
--rw-r--r--   0 danbryce   (501) dialout     (20)     2438 2023-01-20 22:15:58.000000 funman-1.4.0/src/funman/search/search.py
--rw-r--r--   0 danbryce   (501) dialout     (20)     1223 2023-02-01 13:45:54.000000 funman-1.4.0/src/funman/search/smt_check.py
-drwxr-xr-x   0 danbryce   (501) dialout     (20)        0 2023-02-03 17:05:44.508709 funman-1.4.0/src/funman/translate/
--rw-r--r--   0 danbryce   (501) dialout     (20)      228 2023-01-04 20:33:39.000000 funman-1.4.0/src/funman/translate/__init__.py
--rw-r--r--   0 danbryce   (501) dialout     (20)    17879 2023-02-02 21:34:19.000000 funman-1.4.0/src/funman/translate/bilayer.py
--rw-r--r--   0 danbryce   (501) dialout     (20)     1271 2023-01-30 14:42:47.000000 funman-1.4.0/src/funman/translate/encoded.py
--rw-r--r--   0 danbryce   (501) dialout     (20)     9018 2023-01-04 20:33:39.000000 funman-1.4.0/src/funman/translate/gromet.py
--rw-r--r--   0 danbryce   (501) dialout     (20)     6266 2023-01-30 14:42:47.000000 funman-1.4.0/src/funman/translate/translate.py
-drwxr-xr-x   0 danbryce   (501) dialout     (20)        0 2023-02-03 17:05:44.525935 funman-1.4.0/src/funman/utils/
--rw-r--r--   0 danbryce   (501) dialout     (20)       54 2023-01-04 20:33:39.000000 funman-1.4.0/src/funman/utils/__init__.py
--rw-r--r--   0 danbryce   (501) dialout     (20)     2600 2023-01-30 14:42:47.000000 funman-1.4.0/src/funman/utils/handlers.py
--rw-r--r--   0 danbryce   (501) dialout     (20)     2139 2022-12-31 21:23:10.000000 funman-1.4.0/src/funman/utils/math_utils.py
--rw-r--r--   0 danbryce   (501) dialout     (20)     6131 2023-02-01 13:16:26.000000 funman-1.4.0/src/funman/utils/smtlib_utils.py
-drwxr-xr-x   0 danbryce   (501) dialout     (20)        0 2023-02-03 17:05:44.378332 funman-1.4.0/src/funman.egg-info/
--rw-r--r--   0 danbryce   (501) dialout     (20)    10453 2023-02-03 17:05:44.000000 funman-1.4.0/src/funman.egg-info/PKG-INFO
--rw-r--r--   0 danbryce   (501) dialout     (20)     1441 2023-02-03 17:05:44.000000 funman-1.4.0/src/funman.egg-info/SOURCES.txt
--rw-r--r--   0 danbryce   (501) dialout     (20)        1 2023-02-03 17:05:44.000000 funman-1.4.0/src/funman.egg-info/dependency_links.txt
--rw-r--r--   0 danbryce   (501) dialout     (20)        1 2022-09-08 13:44:46.000000 funman-1.4.0/src/funman.egg-info/not-zip-safe
--rw-r--r--   0 danbryce   (501) dialout     (20)       87 2023-02-03 17:05:44.000000 funman-1.4.0/src/funman.egg-info/requires.txt
--rw-r--r--   0 danbryce   (501) dialout     (20)        7 2023-02-03 17:05:44.000000 funman-1.4.0/src/funman.egg-info/top_level.txt
-drwxr-xr-x   0 danbryce   (501) dialout     (20)        0 2023-02-03 17:05:44.553465 funman-1.4.0/test/
--rw-r--r--   0 danbryce   (501) dialout     (20)     8539 2023-01-26 16:27:49.000000 funman-1.4.0/test/test_api.py
--rw-r--r--   0 danbryce   (501) dialout     (20)     9065 2023-01-20 22:15:58.000000 funman-1.4.0/test/test_param_marginalize.py
--rw-r--r--   0 danbryce   (501) dialout     (20)     2061 2023-02-01 13:26:43.000000 funman-1.4.0/test/test_param_space.py
--rw-r--r--   0 danbryce   (501) dialout     (20)     1065 2023-01-30 14:42:47.000000 funman-1.4.0/test/test_read_bilayer.py
--rw-r--r--   0 danbryce   (501) dialout     (20)     1705 2023-02-01 13:26:43.000000 funman-1.4.0/test/test_toy_param_synth.py
--rw-r--r--   0 danbryce   (501) dialout     (20)     6560 2023-02-01 13:26:43.000000 funman-1.4.0/test/test_use_cases.py
+drwxr-xr-x   0 jladwig   (1000) jladwig   (1000)        0 2023-04-24 15:10:11.776294 funman-1.5.0/
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)     1043 2023-04-24 14:35:12.000000 funman-1.5.0/LICENSE
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)    10453 2023-04-24 15:10:11.776294 funman-1.5.0/PKG-INFO
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)    10205 2023-04-24 14:35:12.000000 funman-1.5.0/README.md
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)      912 2023-04-24 14:35:12.000000 funman-1.5.0/pyproject.toml
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)       38 2023-04-24 15:10:11.776294 funman-1.5.0/setup.cfg
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)     1141 2023-04-24 14:35:12.000000 funman-1.5.0/setup.py
+drwxr-xr-x   0 jladwig   (1000) jladwig   (1000)        0 2023-04-24 15:10:11.770294 funman-1.5.0/src/
+drwxr-xr-x   0 jladwig   (1000) jladwig   (1000)        0 2023-04-24 15:10:11.771294 funman-1.5.0/src/funman/
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)      375 2023-04-24 14:35:12.000000 funman-1.5.0/src/funman/__init__.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)      127 2023-04-24 15:10:08.000000 funman-1.5.0/src/funman/_version.py
+drwxr-xr-x   0 jladwig   (1000) jladwig   (1000)        0 2023-04-24 15:10:11.772294 funman-1.5.0/src/funman/api/
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)       99 2023-04-24 14:35:12.000000 funman-1.5.0/src/funman/api/__init__.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)     4907 2023-04-24 14:35:12.000000 funman-1.5.0/src/funman/api/api.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)      971 2023-04-24 14:35:12.000000 funman-1.5.0/src/funman/api/client.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)      894 2023-04-24 14:35:12.000000 funman-1.5.0/src/funman/api/server.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)      219 2023-04-24 14:35:12.000000 funman-1.5.0/src/funman/constants.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)     3679 2023-04-24 14:35:12.000000 funman-1.5.0/src/funman/funman.py
+drwxr-xr-x   0 jladwig   (1000) jladwig   (1000)        0 2023-04-24 15:10:11.773294 funman-1.5.0/src/funman/model/
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)      559 2023-04-24 14:35:12.000000 funman-1.5.0/src/funman/model/__init__.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)    13761 2023-04-24 14:35:12.000000 funman-1.5.0/src/funman/model/bilayer.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)      579 2023-04-24 14:36:33.000000 funman-1.5.0/src/funman/model/decapode.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)      722 2023-04-24 14:35:12.000000 funman-1.5.0/src/funman/model/encoded.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)      667 2023-04-24 14:35:12.000000 funman-1.5.0/src/funman/model/gromet.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)     1081 2023-04-24 14:35:12.000000 funman-1.5.0/src/funman/model/model.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)     2460 2023-04-24 14:36:33.000000 funman-1.5.0/src/funman/model/query.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)      477 2023-04-24 14:35:12.000000 funman-1.5.0/src/funman/model/simulator.py
+drwxr-xr-x   0 jladwig   (1000) jladwig   (1000)        0 2023-04-24 15:10:11.773294 funman-1.5.0/src/funman/representation/
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)      141 2023-04-24 14:35:12.000000 funman-1.5.0/src/funman/representation/__init__.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)    38194 2023-04-24 14:36:33.000000 funman-1.5.0/src/funman/representation/representation.py
+drwxr-xr-x   0 jladwig   (1000) jladwig   (1000)        0 2023-04-24 15:10:11.774294 funman-1.5.0/src/funman/scenario/
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)      180 2023-04-24 14:35:12.000000 funman-1.5.0/src/funman/scenario/__init__.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)     9058 2023-04-24 14:36:33.000000 funman-1.5.0/src/funman/scenario/consistency.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)     9175 2023-04-24 14:36:33.000000 funman-1.5.0/src/funman/scenario/parameter_synthesis.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)      855 2023-04-24 14:35:12.000000 funman-1.5.0/src/funman/scenario/scenario.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)     1591 2023-04-24 14:35:12.000000 funman-1.5.0/src/funman/scenario/simulation.py
+drwxr-xr-x   0 jladwig   (1000) jladwig   (1000)        0 2023-04-24 15:10:11.774294 funman-1.5.0/src/funman/search/
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)      317 2023-04-24 14:35:12.000000 funman-1.5.0/src/funman/search/__init__.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)    32149 2023-04-24 14:36:33.000000 funman-1.5.0/src/funman/search/box_search.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)     2437 2023-04-24 14:35:12.000000 funman-1.5.0/src/funman/search/search.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)     1600 2023-04-24 14:36:33.000000 funman-1.5.0/src/funman/search/smt_check.py
+drwxr-xr-x   0 jladwig   (1000) jladwig   (1000)        0 2023-04-24 15:10:11.775294 funman-1.5.0/src/funman/translate/
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)      228 2023-04-24 14:35:12.000000 funman-1.5.0/src/funman/translate/__init__.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)    26400 2023-04-24 14:36:33.000000 funman-1.5.0/src/funman/translate/bilayer.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)      476 2023-04-24 14:36:33.000000 funman-1.5.0/src/funman/translate/decapode.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)     1273 2023-04-24 14:36:33.000000 funman-1.5.0/src/funman/translate/encoded.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)     9018 2023-04-24 14:35:12.000000 funman-1.5.0/src/funman/translate/gromet.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)     6759 2023-04-24 14:36:33.000000 funman-1.5.0/src/funman/translate/translate.py
+drwxr-xr-x   0 jladwig   (1000) jladwig   (1000)        0 2023-04-24 15:10:11.775294 funman-1.5.0/src/funman/utils/
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)       54 2023-04-24 14:35:12.000000 funman-1.5.0/src/funman/utils/__init__.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)     2600 2023-04-24 14:35:12.000000 funman-1.5.0/src/funman/utils/handlers.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)     2139 2023-04-24 14:35:12.000000 funman-1.5.0/src/funman/utils/math_utils.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)     6131 2023-04-24 14:35:12.000000 funman-1.5.0/src/funman/utils/smtlib_utils.py
+drwxr-xr-x   0 jladwig   (1000) jladwig   (1000)        0 2023-04-24 15:10:11.772294 funman-1.5.0/src/funman.egg-info/
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)    10453 2023-04-24 15:10:11.000000 funman-1.5.0/src/funman.egg-info/PKG-INFO
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)     1525 2023-04-24 15:10:11.000000 funman-1.5.0/src/funman.egg-info/SOURCES.txt
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)        1 2023-04-24 15:10:11.000000 funman-1.5.0/src/funman.egg-info/dependency_links.txt
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)        1 2022-12-21 17:24:35.000000 funman-1.5.0/src/funman.egg-info/not-zip-safe
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)       87 2023-04-24 15:10:11.000000 funman-1.5.0/src/funman.egg-info/requires.txt
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)        7 2023-04-24 15:10:11.000000 funman-1.5.0/src/funman.egg-info/top_level.txt
+drwxr-xr-x   0 jladwig   (1000) jladwig   (1000)        0 2023-04-24 15:10:11.776294 funman-1.5.0/test/
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)     8539 2023-04-24 14:35:12.000000 funman-1.5.0/test/test_api.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)     7826 2023-04-24 14:36:33.000000 funman-1.5.0/test/test_decapode.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)     9065 2023-04-24 14:35:12.000000 funman-1.5.0/test/test_param_marginalize.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)     2061 2023-04-24 14:35:12.000000 funman-1.5.0/test/test_param_space.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)     1065 2023-04-24 14:35:12.000000 funman-1.5.0/test/test_read_bilayer.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)     1703 2023-04-24 14:35:12.000000 funman-1.5.0/test/test_toy_param_synth.py
+-rw-r--r--   0 jladwig   (1000) jladwig   (1000)     6809 2023-04-24 14:35:12.000000 funman-1.5.0/test/test_use_cases.py
```

### Comparing `funman-1.4.0/LICENSE` & `funman-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `funman-1.4.0/PKG-INFO` & `funman-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funman
-Version: 1.4.0
+Version: 1.5.0
 Summary: Functional Model Analysis Tool
 Home-page: 
 Author: Dan Bryce
 Author-email: dbryce@sift.net
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dreal
```

### Comparing `funman-1.4.0/README.md` & `funman-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `funman-1.4.0/pyproject.toml` & `funman-1.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `funman-1.4.0/setup.py` & `funman-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `funman-1.4.0/src/funman/api/api.py` & `funman-1.5.0/src/funman/api/api.py`

 * *Files identical despite different names*

### Comparing `funman-1.4.0/src/funman/api/client.py` & `funman-1.5.0/src/funman/api/client.py`

 * *Files identical despite different names*

### Comparing `funman-1.4.0/src/funman/api/server.py` & `funman-1.5.0/src/funman/api/server.py`

 * *Files identical despite different names*

### Comparing `funman-1.4.0/src/funman/funman.py` & `funman-1.5.0/src/funman/funman.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,39 +22,46 @@
         underscore_attrs_are_private = True
         arbitrary_types_allowed = True
 
     tolerance: float = 0.1
     """Algorithm-specific tolerance for approximation, used by BoxSearch"""
 
     queue_timeout: int = 1
-    """Multiprocessing queue timeout, used by BoxSearch"""    
+    """Multiprocessing queue timeout, used by BoxSearch"""
     number_of_processes: int = mp.cpu_count()
     """Number of BoxSearch processes"""
     _handler: ResultHandler = NoopResultHandler()
     wait_timeout: int = None
     """Timeout for BoxSearch procesess to wait for boxes to evaluate"""
     _wait_action: WaitAction = None
     wait_action_timeout: float = 0.05
     """Time to sleep proceses waiting for work"""
     _read_cache: ResultHandler = None
     # episode_type: =None,
     _search: str = None
     """Name of search algorithm to use"""
     solver: str = "z3"
     """Name of pysmt solver to use"""
-    max_steps: int = 2
+    num_steps: int = 2
     """Number of timesteps to encode"""
     step_size: int = 1
     """Step size for encoding"""
     num_initial_boxes: int = 1
     """Number of initial boxes for BoxSearch"""
     initial_state_tolerance = 0.0
     """Factor used to relax initial state values bounds"""
     save_smtlib: bool = False
     """Whether to save each smt invocation as an SMTLib file"""
+    dreal_precision: float = 0.001
+    """Precision delta for dreal solver"""
+    dreal_log_level: str = "off"
+    """Constraint noise term to relax constraints"""
+    constraint_noise: float = 0.0
+    """Use MCTS in dreal"""
+    dreal_mcts = False
 
     @validator("solver")
     def import_dreal(cls, v):
         if v == "dreal":
             try:
                 import funman_dreal
             except:
```

### Comparing `funman-1.4.0/src/funman/model/__init__.py` & `funman-1.5.0/src/funman/model/__init__.py`

 * *Files identical despite different names*

### Comparing `funman-1.4.0/src/funman/model/bilayer.py` & `funman-1.5.0/src/funman/model/bilayer.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     get_model,
     simplify,
     substitute,
 )
 from pysmt.typing import BOOL, INT, REAL
 
 from funman.model import Model
+from funman.representation.representation import Parameter
 
 
 class BilayerMetadata(BaseModel):
     """
     Metadata for a BilayerNode
     """
 
@@ -148,16 +149,20 @@
     Abstract representation of a Bilayer graph.
     """
 
     class Config:
         underscore_attrs_are_private = True
 
     json_graph: Dict
-    _node_incoming_edges: Dict[BilayerNode, Dict[BilayerNode, BilayerEdge]] = {}
-    _node_outgoing_edges: Dict[BilayerNode, Dict[BilayerNode, BilayerEdge]] = {}
+    _node_incoming_edges: Dict[
+        BilayerNode, Dict[BilayerNode, BilayerEdge]
+    ] = {}
+    _node_outgoing_edges: Dict[
+        BilayerNode, Dict[BilayerNode, BilayerEdge]
+    ] = {}
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.json_graph = kwargs["json_graph"]
         self._initialize_from_json()
 
     @abstractmethod
@@ -232,15 +237,14 @@
     # @staticmethod
     # def from_json(bilayer_src: Union[str, Dict]):
     #     bilayer = BilayerDynamics(json_graph=bilayer_src)
     #     bilayer.initialize_from_json()
     #     return bilayer
 
     def _initialize_from_json(self):
-
         """
         Create a BilayerDynamics object from a JSON formatted bilayer graph.
 
         Parameters
         ----------
         bilayer_src : str (filename) or dictionary
             The source bilayer representation in a file or dictionary.
@@ -476,7 +480,32 @@
         -------
         Encoder
             SMT encoder for model
         """
         from funman.translate import BilayerEncoder
 
         return BilayerEncoder(config=config)
+
+    def _parameters(self) -> List[Parameter]:
+        params = [
+            Parameter(
+                name=node.parameter,
+                lb=self.parameter_bounds[node.parameter][0],
+                ub=self.parameter_bounds[node.parameter][1],
+            )
+            for _, node in self.bilayer._flux.items()
+            if self.parameter_bounds
+            and node.parameter in self.parameter_bounds
+            and self.parameter_bounds[node.parameter]
+        ]
+        if self.measurements:
+            params += [
+                Parameter(
+                    name=node.parameter,
+                    lb=self.parameter_bounds[node.parameter][0],
+                    ub=self.parameter_bounds[node.parameter][1],
+                )
+                for _, node in self.measurements._flux.items()
+                if node.parameter in self.parameter_bounds
+                and self.parameter_bounds[node.parameter]
+            ]
+        return params
```

### Comparing `funman-1.4.0/src/funman/model/encoded.py` & `funman-1.5.0/src/funman/model/encoded.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+from pydantic import Extra
 from pysmt.formula import FNode
 from pysmt.shortcuts import TRUE
 
 from funman.model import Model
 
 
 class EncodedModel(Model):
     """
     Model that holds an SMT formula encoding a model.  This class is meant to wrap hand-coded SMT formulas.
     """
 
     class Config:
         arbitrary_types_allowed = True
-        underscore_attrs_are_private = True
+        extra = Extra.allow
 
     _formula: FNode = TRUE()
 
     def default_encoder(self, config: "FUNMANConfig") -> "Encoder":
         """
         EncodedModel uses EncodedEncoder as the default.
```

### Comparing `funman-1.4.0/src/funman/model/gromet.py` & `funman-1.5.0/src/funman/model/gromet.py`

 * *Files identical despite different names*

### Comparing `funman-1.4.0/src/funman/model/model.py` & `funman-1.5.0/src/funman/model/model.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,16 +9,20 @@
 
 
 class Model(ABC, BaseModel):
     """
     The abstract base class for Models.
     """
 
+    class Config:
+        allow_inf_nan = True
+
     init_values: Dict[str, float] = {}
     parameter_bounds: Dict[str, List[float]] = {}
+    structural_parameter_bounds: Dict[str, List[int]] = {}
 
     @abstractmethod
     def default_encoder(self, config: "FUNMANConfig") -> "Encoder":
         """
         Return the default Encoder for the model
 
         Returns
```

### Comparing `funman-1.4.0/src/funman/representation/representation.py` & `funman-1.5.0/src/funman/representation/representation.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         """
         Get a pysmt Symbol for the parameter
 
         Returns
         -------
         pysmt.fnode.FNode
             _description_
-        """        
+        """
         if not self._symbol:
             self._symbol = Symbol(self.name, REAL)
         return self._symbol
 
     def timed_copy(self, timepoint: int):
         """
         Create a time-stamped copy of a parameter.  E.g., beta becomes beta_t for a timepoint t
@@ -730,14 +730,26 @@
         """
         if self.cached_width is None or overwrite_cache:
             _, width = self._get_max_width_Parameter(normalize=normalize)
             self.cached_width = width
 
         return self.cached_width
 
+    def variance(self, overwrite_cache=False) -> float:
+        """
+        The variance of a box is the maximum variance of a parameter interval.
+        STUB for Milestone 8 sensitivity analysis
+
+        Returns
+        -------
+        float
+            Variance{p: parameter}
+        """
+        pass
+
     def split(
         self,
         points: List[List[Point]] = None,
         normalize: Dict[str, float] = {},
     ):
         """
         Split box along max width dimension. If points are provided, then pick the axis where the points are maximally distant.
@@ -759,15 +771,14 @@
                 points=[[pt.values[p] for pt in grp] for grp in points]
             )
             if mid == self.bounds[p].lb or mid == self.bounds[p].ub:
                 # Fall back to box midpoint if point-based mid is degenerate
                 p, _ = self._get_max_width_Parameter()
                 mid = self.bounds[p].midpoint()
         else:
-
             p, _ = self._get_max_width_Parameter(normalize=normalize)
             mid = self.bounds[p].midpoint()
 
         b1 = self._copy()
         b2 = self._copy()
 
         # b1 is lower half
@@ -949,14 +960,49 @@
     """
 
     true_boxes: List[Box] = []
     false_boxes: List[Box] = []
     true_points: List[Point] = []
     false_points: List[Point] = []
 
+    @staticmethod
+    def _from_configurations(
+        configurations: List[Dict[str, Union[int, "ParameterSpace"]]]
+    ) -> "ParameterSpace":
+        all_ps = ParameterSpace()
+        for result in configurations:
+            ps = result["parameter_space"]
+            num_steps = result["num_steps"]
+            step_size = result["step_size"]
+            for box in ps.true_boxes:
+                box.bounds["num_steps"] = Interval(
+                    lb=num_steps, ub=num_steps + 1
+                )
+                box.bounds["step_size"] = Interval(
+                    lb=step_size, ub=step_size + 1
+                )
+                all_ps.true_boxes.append(box)
+            for box in ps.false_boxes:
+                box.bounds["num_steps"] = Interval(
+                    lb=num_steps, ub=num_steps + 1
+                )
+                box.bounds["step_size"] = Interval(
+                    lb=step_size, ub=step_size + 1
+                )
+                all_ps.false_boxes.append(box)
+            for point in ps.true_points:
+                point.values["num_steps"] = num_steps
+                point.values["step_size"] = step_size
+                all_ps.true_points.append(point)
+            for point in ps.false_points:
+                point.values["num_steps"] = num_steps
+                point.values["step_size"] = step_size
+                all_ps.false_points.append(point)
+        return all_ps
+
     # STUB project parameter space onto a parameter
     @staticmethod
     def project() -> "ParameterSpace":
         raise NotImplementedError()
         return ParameterSpace()
 
     @staticmethod
```

### Comparing `funman-1.4.0/src/funman/scenario/parameter_synthesis.py` & `funman-1.5.0/src/funman/scenario/parameter_synthesis.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from pandas import DataFrame
 from pydantic import BaseModel
 from pysmt.formula import FNode
 from pysmt.shortcuts import BOOL, Iff, Symbol
 
 from funman.model import QueryTrue
 from funman.model.bilayer import BilayerModel
+from funman.model.decapode import DecapodeModel
 from funman.model.encoded import EncodedModel
 from funman.model.query import QueryEncoded, QueryFunction, QueryLE
 from funman.representation import Parameter
 from funman.representation.representation import ParameterSpace, Point
 from funman.scenario import (
     AnalysisScenario,
     AnalysisScenarioResult,
@@ -34,15 +35,15 @@
 
     class Config:
         underscore_attrs_are_private = True
         smart_union = True
         extra = "forbid"
 
     parameters: List[Parameter]
-    model: Union[BilayerModel, EncodedModel]
+    model: Union[DecapodeModel, BilayerModel, EncodedModel]
     query: Union[QueryLE, QueryEncoded, QueryFunction, QueryTrue] = None
     _search: str = "BoxSearch"
     _smt_encoder: Encoder = None  # TODO set to model.default_encoder()
     _model_encoding: Encoding = None
     _query_encoding: Encoding = None
     _assume_model: FNode = None
     _assume_query: FNode = None
@@ -70,23 +71,68 @@
         if config._search is None:
             from funman.search.box_search import BoxSearch
 
             search = BoxSearch()
         else:
             search = config._search()
 
-        self._encode(config)
+        if self.model.structural_parameter_bounds:
+            if self._smt_encoder is None:
+                self._smt_encoder = self.model.default_encoder(config)
+                self._smt_encoder._encode_timed_model_elements(self.model)
+
+            # FIXME these ranges are also computed in the encoder
+            num_steps_range = range(
+                self.model.structural_parameter_bounds["num_steps"][0],
+                self.model.structural_parameter_bounds["num_steps"][1] + 1,
+            )
+            step_size_range = range(
+                self.model.structural_parameter_bounds["step_size"][0],
+                self.model.structural_parameter_bounds["step_size"][1] + 1,
+            )
+            result = []
+
+            consistent = None
+            for configuration in self._smt_encoder._timed_model_elements[
+                "configurations"
+            ]:
+                num_steps = configuration["num_steps"]
+                step_size = configuration["step_size"]
+                self._encode_timed(num_steps, step_size, config)
+                r = search.search(self, config=config)
+                result.append(
+                    {
+                        "num_steps": num_steps,
+                        "step_size": step_size,
+                        "parameter_space": r,
+                    }
+                )
+                print(self._results_str(result))
+                print("-" * 80)
 
-        self._original_parameter_widths = {
-            p: minus(p.ub, p.lb) for p in self.parameters
-        }
+            parameter_space = ParameterSpace._from_configurations(result)
+        else:
+            self._encode(config)
+
+            self._original_parameter_widths = {
+                p: minus(p.ub, p.lb) for p in self.parameters
+            }
+            parameter_space: ParameterSpace = search.search(self, config)
 
-        result: ParameterSpace = search.search(self, config)
         return ParameterSynthesisScenarioResult(
-            parameter_space=result, scenario=self
+            parameter_space=parameter_space, scenario=self
+        )
+
+    def _results_str(self, result: List[Dict]):
+        return "\n".join(
+            ["num_steps\tstep_size\t|true|\t|false|"]
+            + [
+                f"{r['num_steps']}\t\t{r['step_size']}\t\t{len(r['parameter_space'].true_boxes)}\t{len(r['parameter_space'].false_boxes)}"
+                for r in result
+            ]
         )
 
     def _encode(self, config: "FUNMANConfig"):
         """
         The encoding uses assumption symbols for the model and query so that it is possible to push/pop the (possibly negated) symbols to reason about cases where the model or query must be true or false.
 
         Returns
@@ -95,22 +141,42 @@
             _description_
         """
         if self._smt_encoder is None:
             self._smt_encoder = self.model.default_encoder(config)
         self._assume_model = Symbol("assume_model")
         self._assume_query = Symbol("assume_query")
         self._model_encoding = self._smt_encoder.encode_model(self.model)
-        self._model_encoding.formula = Iff(
-            self._assume_model, self._model_encoding.formula
+        self._model_encoding._formula = Iff(
+            self._assume_model, self._model_encoding._formula
+        )
+        self._query_encoding = self._smt_encoder.encode_query(
+            self._model_encoding, self.query
+        )
+        self._query_encoding._formula = Iff(
+            self._assume_query, self._query_encoding._formula
         )
+        return self._model_encoding, self._query_encoding
+
+    def _encode_timed(self, num_steps, step_size, config: "FUNMANConfig"):
+        self._assume_model = Symbol("assume_model")
+        self._assume_query = Symbol("assume_query")
+        # This will overwrite the _model_encoding for each configuration, but the encoder will retain components of the configurations.
+        self._model_encoding = self._smt_encoder.encode_model_timed(
+            self.model, num_steps, step_size
+        )
+        self._model_encoding._formula = Iff(
+            self._assume_model, self._model_encoding._formula
+        )
+
+        # This will create a new formula for each query without caching them (its typically inexpensive)
         self._query_encoding = self._smt_encoder.encode_query(
             self._model_encoding, self.query
         )
-        self._query_encoding.formula = Iff(
-            self._assume_query, self._query_encoding.formula
+        self._query_encoding._formula = Iff(
+            self._assume_query, self._query_encoding._formula
         )
         return self._model_encoding, self._query_encoding
 
 
 class ParameterSynthesisScenarioResult(AnalysisScenarioResult, BaseModel):
     """
     ParameterSynthesisScenario result, which includes the parameter space and
```

### Comparing `funman-1.4.0/src/funman/scenario/scenario.py` & `funman-1.5.0/src/funman/scenario/scenario.py`

 * *Files identical despite different names*

### Comparing `funman-1.4.0/src/funman/scenario/simulation.py` & `funman-1.5.0/src/funman/scenario/simulation.py`

 * *Files identical despite different names*

### Comparing `funman-1.4.0/src/funman/search/box_search.py` & `funman-1.5.0/src/funman/search/box_search.py`

 * *Files 3% similar despite different names*

```diff
@@ -306,16 +306,16 @@
         solver : Solver
             pysmt solver object
         episode : episode
             data for the current search
         """
         solver.push(1)
         formula = And(
-            episode.problem._model_encoding.formula,
-            episode.problem._query_encoding.formula,
+            episode.problem._model_encoding._formula,
+            episode.problem._query_encoding._formula,
         )
         episode._formula_stack.append(formula)
         solver.add_assertion(formula)
 
     def _initialize_box(self, solver, box, episode):
         solver.push(1)
         formula = episode.problem._smt_encoder.box_to_smt(box)
@@ -339,14 +339,15 @@
             Not(episode.problem._assume_query),
         )
         episode._formula_stack.append(formula)
         solver.add_assertion(formula)
 
     def store_smtlib(self, episode, box, filename="dbg.smt2"):
         with open(filename, "w") as f:
+            print(f"Saving smtlib file: {filename}")
             smtlibscript_from_formula_list(
                 episode._formula_stack,
                 logic=QF_NRA,
             ).serialize(f, daggify=False)
 
     def _setup_true_query(self, solver, episode):
         """
@@ -375,15 +376,14 @@
             # print("Checking false query")
             self._setup_false_query(solver, episode)
             if episode.config.save_smtlib:
                 self.store_smtlib(
                     episode, box, filename=f"fp_{episode._iteration}.smt2"
                 )
             if solver.solve():
-
                 # Record the false point
                 res = solver.get_model()
                 false_points = [episode._extract_point(res)]
                 for point in false_points:
                     episode._add_false_point(point)
                     rval.put(point.dict())
             solver.pop(1)  # Remove false query
@@ -453,15 +453,27 @@
         episode : BoxSearchEpisode
             Shared search data and statistics.
         """
         process_name = f"Expander_{idx}_p{os.getpid()}"
         l = self._logger(episode.config, process_name=process_name)
 
         try:
-            with Solver(name=episode.config.solver, logic=QF_NRA) as solver:
+            if episode.config.solver == "dreal":
+                opts = {
+                    "dreal_precision": episode.config.dreal_precision,
+                    "dreal_log_level": episode.config.dreal_log_level,
+                    "dreal_mcts": episode.config.dreal_mcts,
+                }
+            else:
+                opts = {}
+            with Solver(
+                name=episode.config.solver,
+                logic=QF_NRA,
+                solver_options=opts,
+            ) as solver:
                 l.info(f"{process_name} entering process loop")
                 print("Starting initializing dynamics of model")
                 self._initialize_encoding(solver, episode)
                 print("Initialized dynamics of model")
                 while True:
                     try:
                         box: Box = episode._get_unknown()
```

### Comparing `funman-1.4.0/src/funman/search/search.py` & `funman-1.5.0/src/funman/search/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,14 @@
         super().__init__(**kw)
         self._residuals = SQueue()
         self._iteration_time = SQueue()
         self._iteration_operation = SQueue()
 
 
 class SearchStaticsMP(SearchStatistics):
-
     _multiprocessing: bool = True
     _num_true: Value = 0
     _num_false: Value = 0
     _num_unknown: Value = 0
     _residuals: Queue = None
     _current_residual: Value = 0.0
     _last_time: Array = None
```

### Comparing `funman-1.4.0/src/funman/search/smt_check.py` & `funman-1.5.0/src/funman/search/smt_check.py`

 * *Files 27% similar despite different names*

```diff
@@ -15,18 +15,30 @@
     ) -> "SearchEpisode":
         episode = SearchEpisode(config=config, problem=problem)
         result = self.expand(problem, episode)
         episode._model = result
         return result
 
     def expand(self, problem, episode):
-        with Solver(name=episode.config.solver, logic=QF_NRA) as s:
+        if episode.config.solver == "dreal":
+            opts = {
+                "dreal_precision": episode.config.dreal_precision,
+                "dreal_log_level": episode.config.dreal_log_level,
+                "dreal_mcts": episode.config.dreal_mcts,
+            }
+        else:
+            opts = {}
+        with Solver(
+            name=episode.config.solver,
+            logic=QF_NRA,
+            solver_options=opts,
+        ) as s:
             formula = And(
-                problem._model_encoding.formula,
-                problem._query_encoding.formula,
+                problem._model_encoding._formula,
+                problem._query_encoding._formula,
             )
             s.add_assertion(formula)
             self.store_smtlib(formula)
             result = s.solve()
             if result:
                 result = s.get_model()
         return result
```

### Comparing `funman-1.4.0/src/funman/translate/bilayer.py` & `funman-1.5.0/src/funman/translate/bilayer.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,16 +3,20 @@
 
 """
 import logging
 from functools import reduce
 from typing import Dict, List, Set, Union
 
 import pysmt
+from pysmt.formula import FNode
 from pysmt.shortcuts import (
+    GE,
+    GT,
     LE,
+    LT,
     TRUE,
     And,
     Equals,
     Minus,
     Plus,
     Real,
     Symbol,
@@ -61,14 +65,223 @@
     """
 
     class Config:
         underscore_attrs_are_private = True
 
     _timed_symbols: Set[str] = set([])
     _untimed_symbols: Set[str] = set([])
+    _timed_model_elements: Dict = None
+    _untimed_constraints: FNode
+    _min_time_point: int
+    _min_step_size: int
+
+    def get_structural_configurations(self, model: Model):
+        configurations: List[Dict[str, int]] = []
+        if len(model.structural_parameter_bounds) == 0:
+            self._min_time_point = 0
+            self._min_step_size = 1
+            num_steps = [1, self.config.num_steps]
+            step_size = [1, self.config.step_size]
+            max_step_size = self.config.step_size
+            max_step_index = self.config.num_steps * max_step_size
+            configurations.append(
+                {
+                    "num_steps": self.config.num_steps,
+                    "step_size": self.config.step_size,
+                }
+            )
+        else:
+            num_steps = model.structural_parameter_bounds["num_steps"]
+            step_size = model.structural_parameter_bounds["step_size"]
+            self._min_time_point = num_steps[0]
+            self._min_step_size = step_size[0]
+            max_step_size = step_size[1]
+            max_step_index = num_steps[1] * max_step_size
+            configurations += [
+                {"num_steps": ns, "step_size": ss}
+                for ns in range(num_steps[0], num_steps[1] + 1)
+                for ss in range(step_size[0], step_size[1] + 1)
+            ]
+        return configurations, max_step_index, max_step_size
+
+    def get_timepoints(self, num_steps, step_size):
+        state_timepoints = range(
+            0,
+            (step_size * num_steps) + 1,
+            step_size,
+        )
+
+        if len(list(state_timepoints)) == 0:
+            raise Exception(
+                f"Could not identify timepoints from step_size = {step_size} and num_steps = {num_steps}"
+            )
+
+        transition_timepoints = range(0, step_size * num_steps, step_size)
+        return list(state_timepoints), list(transition_timepoints)
+
+    def _encode_next_step(
+        self,
+        model: Model,
+        step: int,
+        next_step: int,
+        time_dependent_parameters=None,
+    ):
+        transition = self._encode_bilayer(
+            model.bilayer,
+            [step, next_step],
+            time_dependent_parameters=time_dependent_parameters,
+        )
+        if model.measurements:
+            measurements = self._encode_measurements(
+                model.measurements, [step + next_step]
+            )
+        else:
+            measurements = TRUE()
+
+        return And(transition, measurements).simplify()
+
+    def _encode_untimed_constraints(
+        self, model: Model, time_dependent_parameters=False
+    ):
+        untimed_constraints = []
+        parameters = model._parameters()
+        if not time_dependent_parameters:
+            untimed_constraints.append(
+                self.box_to_smt(
+                    Box(
+                        bounds={
+                            p.name: Interval(lb=p.lb, ub=p.ub)
+                            for p in parameters
+                        },
+                        closed_upper_bound=True,
+                    )
+                )
+            )
+            # Encode that all of the identical parameters are equal
+            untimed_constraints.append(
+                And(
+                    [
+                        Equals(Symbol(var1, REAL), Symbol(var2, REAL))
+                        for group in model.identical_parameters
+                        for var1 in group
+                        for var2 in group
+                        if var1 != var2
+                    ]
+                ).simplify()
+            )
+        return And(untimed_constraints).simplify()
+
+    def _encode_timed_model_elements(
+        self, model: Model, time_dependent_parameters=False
+    ):
+        # All state nodes correspond to timed symbols
+        for idx, node in model.bilayer._state.items():
+            self._timed_symbols.add(node.parameter)
+
+        # All flux nodes correspond to untimed symbols
+        for _, node in model.bilayer._flux.items():
+            self._untimed_symbols.add(node.parameter)
+
+        (
+            configurations,
+            max_step_index,
+            max_step_size,
+        ) = self.get_structural_configurations(model)
+        self._timed_model_elements = {
+            "init": self._define_init(model),
+            "time_step_constraints": [
+                [None for i in range(max_step_size)]
+                for j in range(max_step_index)
+            ],
+            "configurations": configurations,
+            "untimed_constraints": self._encode_untimed_constraints(model),
+            "timed_parameters": [
+                [None for i in range(max_step_size)]
+                for j in range(max_step_index)
+            ],
+        }
+
+    def encode_model_timed(
+        self,
+        model: Model,
+        num_steps: int,
+        step_size: int,
+        time_dependent_parameters: bool = False,
+    ):
+        if self._timed_model_elements is None:
+            self._timed_model_elements = self._encode_timed_model_elements(
+                model, time_dependent_parameters=time_dependent_parameters
+            )
+
+        state_timepoints, transition_timepoints = self.get_timepoints(
+            num_steps, step_size
+        )
+        parameters = model._parameters()
+
+        constraints = []
+
+        for i, timepoint in enumerate(transition_timepoints):
+            c = self._timed_model_elements["time_step_constraints"][timepoint][
+                step_size - self._min_step_size
+            ]
+            if c is None:
+                c = self._encode_next_step(
+                    model,
+                    state_timepoints[i],
+                    state_timepoints[i + 1],
+                    time_dependent_parameters=None,
+                )
+                self._timed_model_elements["time_step_constraints"][timepoint][
+                    step_size - self._min_step_size
+                ] = c
+            constraints.append(c)
+
+            if time_dependent_parameters:
+                params = self._timed_model_elements["timed_parameters"][
+                    timepoint
+                ][step_size - self._min_step_size]
+                if params == []:
+                    params = [p.timed_copy(timepoint) for p in parameters]
+                    self._timed_model_elements["timed_parameters"][timepoint][
+                        step_size - self._min_step_size
+                    ] = params
+                constraints.append(
+                    self.box_to_smt(
+                        Box(
+                            bounds={
+                                p.name: Interval(lb=p.lb, ub=p.ub)
+                                for p in timed_parameters
+                            }
+                        ),
+                        closed_upper_bound=True,
+                    )
+                )
+
+        if time_dependent_parameters:
+            # FIXME cache this computation
+            ## Assume that all parameters are constant
+            constraints.append(
+                self._set_parameters_constant(
+                    parameters,
+                    constraints,
+                ),
+            )
+
+        formula = And(
+            And(
+                [
+                    self._timed_model_elements["init"],
+                    self._timed_model_elements["untimed_constraints"],
+                ]
+                + constraints
+            ).simplify(),
+            (model._extra_constraints if model._extra_constraints else TRUE()),
+        ).simplify()
+        symbols = self._symbols(formula)
+        return Encoding(_formula=formula, _symbols=symbols)
 
     def encode_model(self, model: Model, time_dependent_parameters=False):
         """
         Encode the model as an SMTLib formula.
 
         Parameters
         ----------
@@ -86,25 +299,27 @@
             cannot identify encoding timepoints
         Exception
             cannot encode model type
         """
         if isinstance(model, BilayerModel):
             state_timepoints = range(
                 0,
-                self.config.max_steps + 1,
+                (self.config.num_steps * self.config.step_size) + 1,
                 self.config.step_size,
             )
 
             if len(list(state_timepoints)) == 0:
                 raise Exception(
-                    f"Could not identify timepoints from step_size = {self.config.step_size} and max_steps = {self.config.max_steps}"
+                    f"Could not identify timepoints from step_size = {self.config.step_size} and num_steps = {self.config.num_steps}"
                 )
 
             transition_timepoints = range(
-                0, self.config.max_steps, self.config.step_size
+                0,
+                self.config.num_steps * self.config.step_size,
+                self.config.step_size,
             )
 
             # All state nodes correspond to timed symbols
             for idx, node in model.bilayer._state.items():
                 self._timed_symbols.add(node.parameter)
 
             # All flux nodes correspond to untimed symbols
@@ -216,15 +431,15 @@
                 (
                     model._extra_constraints
                     if model._extra_constraints
                     else TRUE()
                 ),
             )
             symbols = self._symbols(formula)
-            return Encoding(formula=formula, symbols=symbols)
+            return Encoding(_formula=formula, _symbols=symbols)
         else:
             raise Exception(
                 f"BilayerEncoder cannot encode model of type: {type(model)}"
             )
 
     def _define_init(self, model):
         if self.config.initial_state_tolerance == 0.0:
@@ -265,15 +480,17 @@
             )
 
     def _encode_measurements(
         self, measurements: BilayerMeasurement, timepoints
     ):
         ans = And(
             [
-                self._encode_measurements_timepoint(measurements, timepoints[i])
+                self._encode_measurements_timepoint(
+                    measurements, timepoints[i]
+                )
                 for i in range(len(timepoints))
             ]
         )
         return ans
 
     def _encode_measurements_timepoint(self, measurements, t):
         observable_defs = And(
@@ -310,15 +527,17 @@
         bilayer,
         timepoint,
         next_timepoint,
         time_dependent_parameters=False,
     ):
         ## Calculate time step size
         time_step_size = next_timepoint - timepoint
-        eqns = []  ## List of SMT equations for a given timepoint. These will be
+        eqns = (
+            []
+        )  ## List of SMT equations for a given timepoint. These will be
         ## joined by an "And" command and returned
 
         for t in bilayer._tangent:  ## Loop over _tangents (derivatives)
             pos_derivative_expr_terms = []
             neg_derivative_expr_terms = []
             ## Get _tangent variable and translate it to SMT form tanvar_smt
             tanvar = bilayer._tangent[t].parameter
@@ -376,22 +595,38 @@
                 else Real(0.0)
             )
             neg_terms = (
                 reduce(lambda a, b: Plus(a, b), neg_derivative_expr_terms)
                 if len(neg_derivative_expr_terms) > 0
                 else Real(0.0)
             )
+            # noise = Symbol(f"noise_{state_var_next_step_smt}", REAL)
+            # self._timed_symbols.add(f"{noise}".rsplit("_", 1)[0])
             eqn = simplify(
-                Equals(
-                    state_var_next_step_smt,
-                    Plus(
-                        state_var_smt,
-                        Times(
-                            Real(time_step_size),
-                            Minus(pos_terms, neg_terms),
+                And(
+                    LE(
+                        state_var_next_step_smt,
+                        Plus(
+                            state_var_smt,
+                            Times(
+                                Real(time_step_size),
+                                Minus(pos_terms, neg_terms),
+                            ),
+                            Real(self.config.constraint_noise),
+                        ),
+                    ),
+                    GE(
+                        state_var_next_step_smt,
+                        Plus(
+                            state_var_smt,
+                            Times(
+                                Real(time_step_size),
+                                Minus(pos_terms, neg_terms),
+                            ),
+                            Real(-self.config.constraint_noise),
                         ),
                     ),
                 )
             )
             # print(eqn)
             eqns.append(eqn)
         return And(eqns)
@@ -476,15 +711,15 @@
 
         Returns
         -------
         Dict[str, Dict[str, float]]
             mapping from symbol and timepoint to value
         """
 
-        vars = model_encoding.symbols
+        vars = model_encoding._symbols
         vals = {}
         for var in vars:
             vals[var] = {}
             for t in vars[var]:
                 try:
                     symbol = vars[var][t]
                     vals[var][t] = float(pysmtModel.get_py_value(symbol))
```

### Comparing `funman-1.4.0/src/funman/translate/encoded.py` & `funman-1.5.0/src/funman/translate/encoded.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         Returns
         -------
         FNode
             SMTLib formula encoding the model
         """
         if isinstance(model, EncodedModel):
             encoding = Encoding(
-                formula=model._formula,
-                symbols=list(model._formula.get_free_variables()),
+                _formula=model._formula,
+                _symbols=list(model._formula.get_free_variables()),
             )
             return encoding
         else:
             raise Exception(
                 f"An EncodedEncoder cannot encode models of type: {type(model)}"
             )
```

### Comparing `funman-1.4.0/src/funman/translate/gromet.py` & `funman-1.5.0/src/funman/translate/gromet.py`

 * *Files identical despite different names*

### Comparing `funman-1.4.0/src/funman/translate/translate.py` & `funman-1.5.0/src/funman/translate/translate.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 This module defines the abstract base classes for the model encoder classes in funman.translate package.
 """
 
 from abc import ABC, abstractmethod
 from typing import Dict, List, Union
 
 import pysmt
-from pydantic import BaseModel
+from pydantic import BaseModel, Extra
 from pysmt.formula import FNode
-from pysmt.shortcuts import GE, LE, LT, REAL, TRUE, And, Real, Symbol
+from pysmt.shortcuts import GE, LE, LT, REAL, TRUE, And, Equals, Real, Symbol
 
 from funman.constants import NEG_INFINITY, POS_INFINITY
 from funman.funman import FUNMANConfig
 from funman.model.query import Query, QueryEncoded, QueryLE, QueryTrue
 from funman.representation import Parameter
 from funman.representation.representation import Box, Interval, Point
 
@@ -21,17 +21,18 @@
     """
     An encoding comprises a formula over a set of symbols.
 
     """
 
     class Config:
         arbitrary_types_allowed = True
+        extra = Extra.allow
 
-    formula: FNode = None
-    symbols: Union[List[FNode], Dict[str, Dict[str, FNode]]] = None
+    _formula: FNode = None
+    _symbols: Union[List[FNode], Dict[str, Dict[str, FNode]]] = None
 
     # @validator("formula")
     # def set_symbols(cls, v: FNode):
     #     cls.symbols = Symbol(v, REAL)
 
 
 class EncodingOptions(object):
@@ -107,24 +108,28 @@
             return query_handlers[type(query)](model_encoding, query)
         else:
             raise NotImplementedError(
                 f"Do not know how to encode query of type {type(query)}"
             )
 
     def _return_encoded_query(self, model_encoding, query):
-        return Encoding(formula=query._formula)
+        return Encoding(_formula=query._formula)
 
     def _encode_query_le(self, model_encoding, query):
-        timepoints = model_encoding.symbols[query.variable]
+        if query.variable not in model_encoding._symbols:
+            raise Exception(
+                f"Could not encode QueryLE because {query.variable} does not appear in the model_encoding symbols."
+            )
+        timepoints = model_encoding._symbols[query.variable]
         return Encoding(
-            formula=And([LE(s, Real(query.ub)) for s in timepoints.values()])
+            _formula=And([LE(s, Real(query.ub)) for s in timepoints.values()])
         )
 
     def _encode_query_true(self, model_encoding, query):
-        return Encoding(formula=TRUE())
+        return Encoding(_formula=TRUE())
 
     def symbol_timeseries(
         self, model_encoding, pysmtModel: pysmt.solvers.solver.Model
     ) -> Dict[str, List[Union[float, None]]]:
         """
         Generate a symbol (str) to timeseries (list) of values
 
@@ -139,15 +144,14 @@
             [
                 max([int(k) for k in tps.keys() if k.isdigit()] + [0])
                 for _, tps in series.items()
             ]
         )
         a_series["index"] = list(range(0, max_t + 1))
         for var, tps in series.items():
-
             vals = [None] * (int(max_t) + 1)
             for t, v in tps.items():
                 if t.isdigit():
                     vals[int(t)] = v
             a_series[var] = vals
         return a_series
 
@@ -165,27 +169,32 @@
             interpret interval as closed (i.e., p <= ub), by default False
 
         Returns
         -------
         FNode
             formula constraining p to the interval
         """
-        lower = (
-            GE(Symbol(p, REAL), Real(i.lb)) if i.lb != NEG_INFINITY else TRUE()
-        )
-        upper_ineq = LE if closed_upper_bound else LT
-        upper = (
-            upper_ineq(Symbol(p, REAL), Real(i.ub))
-            if i.ub != POS_INFINITY
-            else TRUE()
-        )
-        return And(
-            lower,
-            upper,
-        ).simplify()
+        if i.lb == i.ub and i.lb != NEG_INFINITY and i.lb != POS_INFINITY:
+            return Equals(Symbol(p, REAL), Real(i.lb))
+        else:
+            lower = (
+                GE(Symbol(p, REAL), Real(i.lb))
+                if i.lb != NEG_INFINITY
+                else TRUE()
+            )
+            upper_ineq = LE if closed_upper_bound else LT
+            upper = (
+                upper_ineq(Symbol(p, REAL), Real(i.ub))
+                if i.ub != POS_INFINITY
+                else TRUE()
+            )
+            return And(
+                lower,
+                upper,
+            ).simplify()
 
     def point_to_smt(self, pt: Point):
         return And(
             [Equals(p.symbol(), Real(value)) for p, value in pt.values.items()]
         )
 
     def box_to_smt(self, box: Box, closed_upper_bound: bool = False):
```

### Comparing `funman-1.4.0/src/funman/utils/handlers.py` & `funman-1.5.0/src/funman/utils/handlers.py`

 * *Files identical despite different names*

### Comparing `funman-1.4.0/src/funman/utils/math_utils.py` & `funman-1.5.0/src/funman/utils/math_utils.py`

 * *Files identical despite different names*

### Comparing `funman-1.4.0/src/funman/utils/smtlib_utils.py` & `funman-1.5.0/src/funman/utils/smtlib_utils.py`

 * *Files identical despite different names*

### Comparing `funman-1.4.0/src/funman.egg-info/PKG-INFO` & `funman-1.5.0/src/funman.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funman
-Version: 1.4.0
+Version: 1.5.0
 Summary: Functional Model Analysis Tool
 Home-page: 
 Author: Dan Bryce
 Author-email: dbryce@sift.net
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dreal
```

### Comparing `funman-1.4.0/src/funman.egg-info/SOURCES.txt` & `funman-1.5.0/src/funman.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 src/funman.egg-info/top_level.txt
 src/funman/api/__init__.py
 src/funman/api/api.py
 src/funman/api/client.py
 src/funman/api/server.py
 src/funman/model/__init__.py
 src/funman/model/bilayer.py
+src/funman/model/decapode.py
 src/funman/model/encoded.py
 src/funman/model/gromet.py
 src/funman/model/model.py
 src/funman/model/query.py
 src/funman/model/simulator.py
 src/funman/representation/__init__.py
 src/funman/representation/representation.py
@@ -32,20 +33,22 @@
 src/funman/scenario/simulation.py
 src/funman/search/__init__.py
 src/funman/search/box_search.py
 src/funman/search/search.py
 src/funman/search/smt_check.py
 src/funman/translate/__init__.py
 src/funman/translate/bilayer.py
+src/funman/translate/decapode.py
 src/funman/translate/encoded.py
 src/funman/translate/gromet.py
 src/funman/translate/translate.py
 src/funman/utils/__init__.py
 src/funman/utils/handlers.py
 src/funman/utils/math_utils.py
 src/funman/utils/smtlib_utils.py
 test/test_api.py
+test/test_decapode.py
 test/test_param_marginalize.py
 test/test_param_space.py
 test/test_read_bilayer.py
 test/test_toy_param_synth.py
 test/test_use_cases.py
```

### Comparing `funman-1.4.0/test/test_api.py` & `funman-1.5.0/test/test_api.py`

 * *Files identical despite different names*

### Comparing `funman-1.4.0/test/test_param_marginalize.py` & `funman-1.5.0/test/test_param_marginalize.py`

 * *Files identical despite different names*

### Comparing `funman-1.4.0/test/test_param_space.py` & `funman-1.5.0/test/test_param_space.py`

 * *Files identical despite different names*

### Comparing `funman-1.4.0/test/test_read_bilayer.py` & `funman-1.5.0/test/test_read_bilayer.py`

 * *Files identical despite different names*

### Comparing `funman-1.4.0/test/test_toy_param_synth.py` & `funman-1.5.0/test/test_toy_param_synth.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from funman.representation.representation import Parameter
 from funman.scenario.parameter_synthesis import ParameterSynthesisScenario
 from funman.translate import EncodedEncoder
 
 
 class TestCompilation(unittest.TestCase):
     def test_toy(self):
-
         parameters = [Parameter(name="x")]
         x = parameters[0].symbol()
 
         # 0.0 <= x <= 5
         model = EncodedModel(_formula=And(LE(x, Real(5.0)), GE(x, Real(0.0))))
 
         scenario = ParameterSynthesisScenario(
@@ -26,15 +25,14 @@
             query=QueryTrue(),
         )
         funman = Funman()
         config = FUNMANConfig()
         result = funman.solve(scenario, config)
 
     def test_toy_2d(self):
-
         parameters = [
             Parameter(name="x"),
             Parameter(name="y"),
         ]
         x = parameters[0].symbol()
         y = parameters[1].symbol()
```

### Comparing `funman-1.4.0/test/test_use_cases.py` & `funman-1.5.0/test/test_use_cases.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,20 +98,27 @@
             LE(x, Real(5.0)),
             GE(x, Real(0.0)),
             LE(y, Real(12.0)),
             GE(y, Real(10.0)),
         )
 
         funman = Funman()
+
         result: ParameterSynthesisScenarioResult = funman.solve(
             ParameterSynthesisScenario(
                 parameters=parameters,
                 model=EncodedModel(_formula=formula),
                 query=QueryTrue(),
-            )
+            ),
+            config=FUNMANConfig(
+                solver="dreal",
+                dreal_mcts=True,
+                tolerance=1e-8,
+                number_of_processes=1,
+            ),
         )
         assert result
 
     def setup_use_case_bilayer_common(self):
         bilayer_path = os.path.join(
             RESOURCES, "bilayer", "CHIME_SIR_dynamics_BiLayer.json"
         )
@@ -151,14 +158,16 @@
 
     def test_use_case_bilayer_parameter_synthesis(self):
         scenario = self.setup_use_case_bilayer_parameter_synthesis()
         funman = Funman()
         result: ParameterSynthesisScenarioResult = funman.solve(
             scenario,
             config=FUNMANConfig(
+                solver="dreal",
+                dreal_mcts=True,
                 tolerance=1e-8,
                 number_of_processes=1,
                 _handler=ResultCombinedHandler(
                     [
                         ResultCacheWriter(f"box_search.json"),
                         RealtimeResultPlotter(
                             scenario.parameters,
@@ -184,17 +193,17 @@
 
         funman = Funman()
 
         # Show that region in parameter space is sat (i.e., there exists a true point)
         result_sat: ConsistencyScenarioResult = funman.solve(scenario)
         df = result_sat.dataframe()
 
-        assert abs(df["I"][2] - 2.24) < 0.01
+        assert abs(df["I"][2] - 2.24) < 0.13
         beta = result_sat._parameters()["beta"]
-        assert abs(beta - 0.00005) < 0.00001
+        assert abs(beta - 0.00005) < 0.001
 
         # Show that region in parameter space is unsat/false
         scenario.model.parameter_bounds["beta"] = [
             0.000067 * 1.5,
             0.000067 * 1.75,
         ]
         result_unsat: ConsistencyScenarioResult = funman.solve(scenario)
```


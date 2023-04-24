# Comparing `tmp/ChessAnalysisPipeline-0.0.5.tar.gz` & `tmp/ChessAnalysisPipeline-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ChessAnalysisPipeline-0.0.5.tar", last modified: Wed Apr 12 18:11:58 2023, max compression
+gzip compressed data, was "ChessAnalysisPipeline-0.0.6.tar", last modified: Mon Apr 24 17:11:36 2023, max compression
```

## Comparing `ChessAnalysisPipeline-0.0.5.tar` & `ChessAnalysisPipeline-0.0.6.tar`

### file list

```diff
@@ -1,67 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:11:58.005454 ChessAnalysisPipeline-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:11:57.993453 ChessAnalysisPipeline-0.0.5/CHAP/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:11:57.997453 ChessAnalysisPipeline-0.0.5/CHAP/common/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:11:57.997453 ChessAnalysisPipeline-0.0.5/CHAP/common/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/common/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25169 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/common/models/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    25035 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/common/models/map.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24441 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/common/processor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3547 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/common/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:11:57.997453 ChessAnalysisPipeline-0.0.5/CHAP/common/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/common/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   127303 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/common/utils/fit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    48178 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/common/utils/general.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10472 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/common/utils/material.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34386 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/common/utils/scanparsers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2910 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/common/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:11:57.997453 ChessAnalysisPipeline-0.0.5/CHAP/edd/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/edd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/edd/models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13629 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/edd/processor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/edd/reader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/edd/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:11:58.001453 ChessAnalysisPipeline-0.0.5/CHAP/inference/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/inference/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2648 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/inference/processor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/inference/reader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/inference/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/pipeline.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4247 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/processor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3577 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/reader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2412 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:11:58.001453 ChessAnalysisPipeline-0.0.5/CHAP/saxswaxs/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/saxswaxs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       99 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/saxswaxs/processor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/saxswaxs/reader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/saxswaxs/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:11:58.001453 ChessAnalysisPipeline-0.0.5/CHAP/sin2psi/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/sin2psi/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       99 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/sin2psi/processor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/sin2psi/reader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/sin2psi/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:11:58.001453 ChessAnalysisPipeline-0.0.5/CHAP/tomo/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/tomo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/tomo/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    97469 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/tomo/processor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/tomo/reader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       96 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/tomo/writer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2759 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/CHAP/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:11:58.005454 ChessAnalysisPipeline-0.0.5/ChessAnalysisPipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-12 18:11:57.000000 ChessAnalysisPipeline-0.0.5/ChessAnalysisPipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-12 18:11:57.000000 ChessAnalysisPipeline-0.0.5/ChessAnalysisPipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 18:11:57.000000 ChessAnalysisPipeline-0.0.5/ChessAnalysisPipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-12 18:11:57.000000 ChessAnalysisPipeline-0.0.5/ChessAnalysisPipeline.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 18:11:57.000000 ChessAnalysisPipeline-0.0.5/ChessAnalysisPipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 18:11:57.000000 ChessAnalysisPipeline-0.0.5/ChessAnalysisPipeline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:11:58.005454 ChessAnalysisPipeline-0.0.5/MLaaS/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/MLaaS/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7467 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/MLaaS/ktrain.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2738 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/MLaaS/mnist_img.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14889 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/MLaaS/tfaas_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-12 18:11:58.005454 ChessAnalysisPipeline-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-12 18:11:44.000000 ChessAnalysisPipeline-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 18:11:58.005454 ChessAnalysisPipeline-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-12 18:11:49.000000 ChessAnalysisPipeline-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:11:36.902539 ChessAnalysisPipeline-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:11:36.890539 ChessAnalysisPipeline-0.0.6/CHAP/
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/TaskManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:11:36.894539 ChessAnalysisPipeline-0.0.6/CHAP/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:11:36.894539 ChessAnalysisPipeline-0.0.6/CHAP/common/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/common/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27105 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/common/models/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27132 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/common/models/map.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24447 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/common/processor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3941 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/common/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:11:36.894539 ChessAnalysisPipeline-0.0.6/CHAP/common/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/common/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   121894 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/common/utils/fit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    51967 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/common/utils/general.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11359 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/common/utils/material.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    44627 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/common/utils/scanparsers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3070 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/common/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:11:36.898539 ChessAnalysisPipeline-0.0.6/CHAP/edd/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/edd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/edd/models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13698 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/edd/processor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/edd/reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/edd/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:11:36.898539 ChessAnalysisPipeline-0.0.6/CHAP/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/inference/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2065 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/inference/processor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/inference/reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/inference/writer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2020 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/pipeline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3378 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/processor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3950 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3869 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:11:36.898539 ChessAnalysisPipeline-0.0.6/CHAP/saxswaxs/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/saxswaxs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       97 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/saxswaxs/processor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/saxswaxs/reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/saxswaxs/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:11:36.898539 ChessAnalysisPipeline-0.0.6/CHAP/sin2psi/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/sin2psi/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       97 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/sin2psi/processor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/sin2psi/reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/sin2psi/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:11:36.898539 ChessAnalysisPipeline-0.0.6/CHAP/tomo/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/tomo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/tomo/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104814 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/tomo/processor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      122 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/tomo/reader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      122 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/tomo/writer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3038 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/CHAP/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:11:36.902539 ChessAnalysisPipeline-0.0.6/ChessAnalysisPipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-24 17:11:36.000000 ChessAnalysisPipeline-0.0.6/ChessAnalysisPipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-24 17:11:36.000000 ChessAnalysisPipeline-0.0.6/ChessAnalysisPipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 17:11:36.000000 ChessAnalysisPipeline-0.0.6/ChessAnalysisPipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-24 17:11:36.000000 ChessAnalysisPipeline-0.0.6/ChessAnalysisPipeline.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 17:11:36.000000 ChessAnalysisPipeline-0.0.6/ChessAnalysisPipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-24 17:11:36.000000 ChessAnalysisPipeline-0.0.6/ChessAnalysisPipeline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 17:11:36.902539 ChessAnalysisPipeline-0.0.6/MLaaS/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/MLaaS/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7467 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/MLaaS/ktrain.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2738 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/MLaaS/mnist_img.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14889 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/MLaaS/tfaas_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-24 17:11:36.902539 ChessAnalysisPipeline-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-24 17:11:25.000000 ChessAnalysisPipeline-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 17:11:36.902539 ChessAnalysisPipeline-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-24 17:11:29.000000 ChessAnalysisPipeline-0.0.6/setup.py
```

### Comparing `ChessAnalysisPipeline-0.0.5/CHAP/common/__init__.py` & `ChessAnalysisPipeline-0.0.6/CHAP/common/__init__.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.5/CHAP/common/models/integration.py` & `ChessAnalysisPipeline-0.0.6/CHAP/common/models/integration.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,152 +1,176 @@
 import copy
-from functools import cache, lru_cache
-import json
-import logging
+from functools import cache
 import os
-from time import time
 from typing import Literal, Optional
 
-# from multiprocessing.pool import ThreadPool
-# from nexusformat.nexus import (NXdata,
-#                                NXdetector,
-#                                NXfield,
-#                                NXprocess,
-#                                NXroot)
 import numpy as np
 from pydantic import (BaseModel,
                       validator,
                       constr,
                       conlist,
                       conint,
                       confloat,
                       FilePath)
-#import pyFAI, pyFAI.multi_geometry, pyFAI.units
 from pyFAI import load as pyfai_load
 from pyFAI.multi_geometry import MultiGeometry
 from pyFAI.units import AZIMUTHAL_UNITS, RADIAL_UNITS
-#from pyspec.file.tiff import TiffFile
-
-#from .map import MapConfig, SpecScans
 
 
 class Detector(BaseModel):
-    """
-    Detector class to represent a single detector used in the experiment.
-    
+    """Detector class to represent a single detector used in the
+    experiment.
+
     :param prefix: Prefix of the detector in the SPEC file.
     :type prefix: str
     :param poni_file: Path to the poni file.
     :type poni_file: str
     :param mask_file: Optional path to the mask file.
     :type mask_file: str, optional
     """
     prefix: constr(strip_whitespace=True, min_length=1)
     poni_file: FilePath
     mask_file: Optional[FilePath]
+
     @validator('poni_file', allow_reuse=True)
     def validate_poni_file(cls, poni_file):
-        """
-        Validate the poni file by checking if it's a valid PONI file.
-        
+        """Validate the poni file by checking if it's a valid PONI
+        file.
+
         :param poni_file: Path to the poni file.
         :type poni_file: str
         :raises ValueError: If poni_file is not a valid PONI file.
         :returns: Absolute path to the poni file.
         :rtype: str
         """
         poni_file = os.path.abspath(poni_file)
         try:
             ai = azimuthal_integrator(poni_file)
-        except:
-            raise(ValueError(f'{poni_file} is not a valid PONI file'))
-        else:
-            return(poni_file)
+        except Exception as exc:
+            raise ValueError(f'{poni_file} is not a valid PONI file') from exc
+        return poni_file
+
     @validator('mask_file', allow_reuse=True)
     def validate_mask_file(cls, mask_file, values):
-        """
-        Validate the mask file. If a mask file is provided, it checks if it's a valid TIFF file.
-        
+        """Validate the mask file. If a mask file is provided, it
+        checks if it's a valid TIFF file.
+
         :param mask_file: Path to the mask file.
         :type mask_file: str or None
         :param values: A dictionary of the Detector fields.
         :type values: dict
-        :raises ValueError: If mask_file is provided and it's not a valid TIFF file.
+        :raises ValueError: If mask_file is provided and it's not a
+            valid TIFF file.
         :raises ValueError: If `'poni_file'` is not provided in `values`.
         :returns: Absolute path to the mask file or None.
-        :rtype: str or None        
+        :rtype: str or None
         """
         if mask_file is None:
-            return(mask_file)
-        else:
-            mask_file = os.path.abspath(mask_file)
-            poni_file = values.get('poni_file')
-            if poni_file is None:
-                raise(ValueError('Cannot validate mask file without a PONI file.'))
-            else:
-                try:
-                    mask_array = get_mask_array(mask_file, poni_file)
-                except BaseException as e:
-                    raise(ValueError(f'Unable to open {mask_file} as a TIFF file'))
-                else:
-                    return(mask_file)
+            return mask_file
+
+        mask_file = os.path.abspath(mask_file)
+        poni_file = values.get('poni_file')
+        if poni_file is None:
+            raise ValueError(
+                'Cannot validate mask file without a PONI file.')
+        try:
+            mask_array = get_mask_array(mask_file, poni_file)
+        except BaseException as exc:
+            raise ValueError(
+                f'Unable to open {mask_file} as a TIFF file') from exc
+        return mask_file
+
     @property
     def azimuthal_integrator(self):
-        return(azimuthal_integrator(self.poni_file))
+        """Return the azimuthal integrator associated with this
+        detector.
+        """
+        return azimuthal_integrator(self.poni_file)
+
     @property
     def mask_array(self):
-        return(get_mask_array(self.mask_file, self.poni_file))
+        """Return the mask array assocated with this detector."""
+        return get_mask_array(self.mask_file, self.poni_file)
+
 
 @cache
 def azimuthal_integrator(poni_file:str):
+    """Return the azimuthal integrator from a PONI file
+
+    :param poni_file: path to a PONI file
+    :type poni_file: str
+    :return: azimuthal integrator
+    :rtype: pyFAI.azimuthal_integrator.AzimuthalIntegrator
+    """
     if not isinstance(poni_file, str):
         poni_file = str(poni_file)
-    return(pyfai_load(poni_file))
+    return pyfai_load(poni_file)
+
+
 @cache
 def get_mask_array(mask_file:str, poni_file:str):
+    """Return a mask array associated with a detector loaded from a
+    tiff file.
+
+    :param mask_file: path to a .tiff file
+    :type mask_file: str
+    :param poni_file: path to a PONI file
+    :type poni_file: str
+    :return: the mask array loaded from `mask_file`
+    :rtype: numpy.ndarray
+    """
     if mask_file is not None:
         if not isinstance(mask_file, str):
             mask_file = str(mask_file)
 
         from pyspec.file.tiff import TiffFile
         with TiffFile(mask_file) as tiff:
             mask_array = tiff.asarray()
     else:
         mask_array = np.zeros(azimuthal_integrator(poni_file).detector.shape)
-    return(mask_array)
+    return mask_array
+
 
 class IntegrationConfig(BaseModel):
-    """
-    Class representing the configuration for a raw detector data integration.
+    """Class representing the configuration for a raw detector data
+    integration.
 
-    :ivar tool_type: type of integration tool; always set to "integration"
+    :ivar tool_type: type of integration tool; always set to
+        "integration"
     :type tool_type: str, optional
     :ivar title: title of the integration
     :type title: str
-    :ivar integration_type: type of integration, one of "azimuthal", "radial", or "cake"
+    :ivar integration_type: type of integration, one of "azimuthal",
+        "radial", or "cake"
     :type integration_type: str
     :ivar detectors: list of detectors used in the integration
     :type detectors: List[Detector]
-    :ivar radial_units: radial units for the integration, defaults to `'q_A^-1'`
+    :ivar radial_units: radial units for the integration, defaults to
+        `'q_A^-1'`
     :type radial_units: str, optional
     :ivar radial_min: minimum radial value for the integration range
     :type radial_min: float, optional
     :ivar radial_max: maximum radial value for the integration range
     :type radial_max: float, optional
-    :ivar radial_npt: number of points in the radial range for the integration
+    :ivar radial_npt: number of points in the radial range for the
+        integration
     :type radial_npt: int, optional
     :ivar azimuthal_units: azimuthal units for the integration
     :type azimuthal_units: str, optional
-    :ivar azimuthal_min: minimum azimuthal value for the integration range
+    :ivar azimuthal_min: minimum azimuthal value for the integration
+        range
     :type azimuthal_min: float, optional
-    :ivar azimuthal_max: maximum azimuthal value for the integration range
+    :ivar azimuthal_max: maximum azimuthal value for the integration
+        range
     :type azimuthal_max: float, optional
-    :ivar azimuthal_npt: number of points in the azimuthal range for the integration
+    :ivar azimuthal_npt: number of points in the azimuthal range for
+        the integration
     :type azimuthal_npt: int, optional
-    :ivar error_model: error model for the integration, one of "poisson" or "azimuthal"
+    :ivar error_model: error model for the integration, one of
+        "poisson" or "azimuthal"
     :type error_model: str, optional
     """
     tool_type: Literal['integration'] = 'integration'
     title: constr(strip_whitespace=True, min_length=1)
     integration_type: Literal['azimuthal', 'radial', 'cake']
     detectors: conlist(item_type=Detector, min_items=1)
     radial_units: str = 'q_A^-1'
@@ -155,361 +179,480 @@
     radial_npt: conint(gt=0) = 1800
     azimuthal_units: str = 'chi_deg'
     azimuthal_min: confloat(ge=-180) = -180
     azimuthal_max: confloat(le=360) = 180
     azimuthal_npt: conint(gt=0) = 3600
     error_model: Optional[Literal['poisson', 'azimuthal']]
     sequence_index: Optional[conint(gt=0)]
+
     @validator('radial_units', allow_reuse=True)
     def validate_radial_units(cls, radial_units):
-        """
-        Validate the radial units for the integration.
+        """Validate the radial units for the integration.
 
-        :param radial_units: unvalidated radial units for the integration
+        :param radial_units: unvalidated radial units for the
+            integration
         :type radial_units: str
-        :raises ValueError: if radial units are not one of the recognized radial units
+        :raises ValueError: if radial units are not one of the
+            recognized radial units
         :return: validated radial units
         :rtype: str
         """
         if radial_units in RADIAL_UNITS.keys():
-            return(radial_units)
-        else:
-            raise(ValueError(f'Invalid radial units: {radial_units}. Must be one of {", ".join(RADIAL_UNITS.keys())}'))
+            return radial_units
+        raise ValueError(
+            f'Invalid radial units: {radial_units}. '
+            f'Must be one of {", ".join(RADIAL_UNITS.keys())}')
+
     @validator('azimuthal_units', allow_reuse=True)
     def validate_azimuthal_units(cls, azimuthal_units):
-        """
-        Validate that `azimuthal_units` is one of the keys in the
+        """Validate that `azimuthal_units` is one of the keys in the
         `pyFAI.units.AZIMUTHAL_UNITS` dictionary.
 
-        :param azimuthal_units: The string representing the unit to be validated.
+        :param azimuthal_units: The string representing the unit to be
+            validated.
         :type azimuthal_units: str
-        :raises ValueError: If `azimuthal_units` is not one of the keys in `pyFAI.units.AZIMUTHAL_UNITS`
-        :return: The original supplied value, if is one of the keys in `pyFAI.units.AZIMUTHAL_UNITS`.
+        :raises ValueError: If `azimuthal_units` is not one of the
+            keys in `pyFAI.units.AZIMUTHAL_UNITS`
+        :return: The original supplied value, if is one of the keys in
+            `pyFAI.units.AZIMUTHAL_UNITS`.
         :rtype: str
         """
         if azimuthal_units in AZIMUTHAL_UNITS.keys():
-            return(azimuthal_units)
-        else:
-            raise(ValueError(f'Invalid azimuthal units: {azimuthal_units}. Must be one of {", ".join(AZIMUTHAL_UNITS.keys())}'))
+            return azimuthal_units
+        raise ValueError(
+            f'Invalid azimuthal units: {azimuthal_units}. '
+            f'Must be one of {", ".join(AZIMUTHAL_UNITS.keys())}')
+
     def validate_range_max(range_name:str):
         """Validate the maximum value of an integration range.
 
-        :param range_name: The name of the integration range (e.g. radial, azimuthal).
+        :param range_name: The name of the integration range
+            (e.g. radial, azimuthal).
         :type range_name: str
         :return: The callable that performs the validation.
         :rtype: callable
         """
         def _validate_range_max(cls, range_max, values):
-            """Check if the maximum value of the integration range is greater than its minimum value.
+            """Check if the maximum value of the integration range is
+            greater than its minimum value.
 
-            :param range_max: The maximum value of the integration range.
+            :param range_max: The maximum value of the integration
+                range.
             :type range_max: float
-            :param values: The values of the other fields being validated.
+            :param values: The values of the other fields being
+                validated.
             :type values: dict
-            :raises ValueError: If the maximum value of the integration range is not greater than its minimum value.
+            :raises ValueError: If the maximum value of the
+                integration range is not greater than its minimum
+                value.
             :return: The validated maximum range value
             :rtype: float
             """
             range_min = values.get(f'{range_name}_min')
             if range_min < range_max:
-                return(range_max)
-            else:
-                raise(ValueError(f'Maximum value of integration range must be greater than minimum value of integration range ({range_name}_min={range_min}).'))
-        return(_validate_range_max)
-    _validate_radial_max = validator('radial_max', allow_reuse=True)(validate_range_max('radial'))
-    _validate_azimuthal_max = validator('azimuthal_max', allow_reuse=True)(validate_range_max('azimuthal'))        
+                return range_max
+            raise ValueError(
+                'Maximum value of integration range must be '
+                'greater than minimum value of integration range '
+                f'({range_name}_min={range_min}).')
+        return _validate_range_max
+
+    _validate_radial_max = validator(
+        'radial_max',
+        allow_reuse=True)(validate_range_max('radial'))
+    _validate_azimuthal_max = validator(
+        'azimuthal_max',
+        allow_reuse=True)(validate_range_max('azimuthal'))
+
     def validate_for_map_config(self, map_config:BaseModel):
-        """
-        Validate the existence of the detector data file for all scan points in `map_config`.
-        
-        :param map_config: The `MapConfig` instance to validate against.
+        """Validate the existence of the detector data file for all
+        scan points in `map_config`.
+
+        :param map_config: The `MapConfig` instance to validate
+            against.
         :type map_config: MapConfig
-        :raises RuntimeError: If a detector data file could not be found for a scan point occurring in `map_config`.
+        :raises RuntimeError: If a detector data file could not be
+            found for a scan point occurring in `map_config`.
         :return: None
         :rtype: None
         """
         for detector in self.detectors:
             for scans in map_config.spec_scans:
                 for scan_number in scans.scan_numbers:
                     scanparser = scans.get_scanparser(scan_number)
                     for scan_step_index in range(scanparser.spec_scan_npts):
-                        # Make sure the detector data file exists for all scan points
+                        # Make sure the detector data file exists for
+                        # all scan points
                         try:
-                            detector_data_file = scanparser.get_detector_data_file(detector.prefix, scan_step_index)
-                        except:
-                            raise(RuntimeError(f'Could not find data file for detector prefix {detector.prefix} on scan number {scan_number} in spec file {scans.spec_file}'))
+                            detector_data_file = \
+                                scanparser.get_detector_data_file(
+                                    detector.prefix, scan_step_index)
+                        except Exception as exc:
+                            raise RuntimeError(
+                                'Could not find data file for detector prefix '
+                                f'{detector.prefix} '
+                                f'on scan number {scan_number} '
+                                f'in spec file {scans.spec_file}') from exc
+
     def get_azimuthal_adjustments(self):
-        """To enable a continuous range of integration in the azimuthal direction
-        for radial and cake integration, obtain adjusted values for this 
-        `IntegrationConfig`'s `azimuthal_min` and `azimuthal_max` values, the
-        angle amount by which those values were adjusted, and the proper location
-        of the discontinuity in the azimuthal direction.
+        """To enable a continuous range of integration in the
+        azimuthal direction for radial and cake integration, obtain
+        adjusted values for this `IntegrationConfig`'s `azimuthal_min`
+        and `azimuthal_max` values, the angle amount by which those
+        values were adjusted, and the proper location of the
+        discontinuity in the azimuthal direction.
 
-        :return: Adjusted chi_min, adjusted chi_max, chi_offset, chi_discontinuity
+        :return: Adjusted chi_min, adjusted chi_max, chi_offset,
+            chi_discontinuity
         :rtype: tuple[float,float,float,float]
         """
-        return(get_azimuthal_adjustments(self.azimuthal_min, self.azimuthal_max))
+        return get_azimuthal_adjustments(self.azimuthal_min,
+                                         self.azimuthal_max)
+
     def get_azimuthal_integrators(self):
-        """Get a list of `AzimuthalIntegrator`s that correspond to the detector
-        configurations in this instance of `IntegrationConfig`.
+        """Get a list of `AzimuthalIntegrator`s that correspond to the
+        detector configurations in this instance of
+        `IntegrationConfig`.
 
-        The returned `AzimuthalIntegrator`s are (if need be) artificially rotated
-        in the azimuthal direction to achieve a continuous range of integration
-        in the azimuthal direction.
+        The returned `AzimuthalIntegrator`s are (if need be)
+        artificially rotated in the azimuthal direction to achieve a
+        continuous range of integration in the azimuthal direction.
 
-        :returns: A list of `AzimuthalIntegrator`s appropriate for use by this
-            `IntegrationConfig` tool
+        :returns: A list of `AzimuthalIntegrator`s appropriate for use
+            by this `IntegrationConfig` tool
         :rtype: list[pyFAI.azimuthalIntegrator.AzimuthalIntegrator]
         """
-        chi_min, chi_max, chi_offset, chi_disc = self.get_azimuthal_adjustments()
-        return(get_azimuthal_integrators(tuple([detector.poni_file for detector in self.detectors]), chi_offset=chi_offset))        
+        chi_offset = self.get_azimuthal_adjustments()[2]
+        return get_azimuthal_integrators(
+            tuple([detector.poni_file for detector in self.detectors]),
+            chi_offset=chi_offset)
+
     def get_multi_geometry_integrator(self):
-        """Get a `MultiGeometry` integrator suitable for use by this instance of
-        `IntegrationConfig`.
+        """Get a `MultiGeometry` integrator suitable for use by this
+        instance of `IntegrationConfig`.
 
         :return: A `MultiGeometry` integrator
         :rtype: pyFAI.multi_geometry.MultiGeometry
         """
         poni_files = tuple([detector.poni_file for detector in self.detectors])
         radial_range = (self.radial_min, self.radial_max)
         azimuthal_range = (self.azimuthal_min, self.azimuthal_max)
-        return(get_multi_geometry_integrator(poni_files, self.radial_units, radial_range, azimuthal_range))
-    def get_azimuthally_integrated_data(self, spec_scans:BaseModel, scan_number:int, scan_step_index:int):
-        """Return azimuthally-integrated data for the scan step specified.
-        
-        :param spec_scans: An instance of `SpecScans` containing the scan step requested.
+        return get_multi_geometry_integrator(poni_files, self.radial_units,
+                                             radial_range, azimuthal_range)
+
+    def get_azimuthally_integrated_data(self,
+                                        spec_scans:BaseModel,
+                                        scan_number:int,
+                                        scan_step_index:int):
+        """Return azimuthally-integrated data for the scan step
+        specified.
+
+        :param spec_scans: An instance of `SpecScans` containing the
+            scan step requested.
         :type spec_scans: SpecScans
-        :param scan_number: The number of the scan containing the scan step requested.
+        :param scan_number: The number of the scan containing the scan
+            step requested.
         :type scan_number: int
         :param scan_step_index: The index of the scan step requested.
         :type scan_step_index: int
-        :return: A 1D array of azimuthally-integrated raw detector intensities.
+        :return: A 1D array of azimuthally-integrated raw detector
+            intensities.
         :rtype: np.ndarray
         """
-        detector_data = spec_scans.get_detector_data(self.detectors, scan_number, scan_step_index)
+        detector_data = spec_scans.get_detector_data(self.detectors,
+                                                     scan_number,
+                                                     scan_step_index)
         integrator = self.get_multi_geometry_integrator()
         lst_mask = [detector.mask_array for detector in self.detectors]
-        result = integrator.integrate1d(detector_data, lst_mask=lst_mask, npt=self.radial_npt, error_model=self.error_model)
+        result = integrator.integrate1d(detector_data,
+                                        lst_mask=lst_mask,
+                                        npt=self.radial_npt,
+                                        error_model=self.error_model)
         if result.sigma is None:
-            return(result.intensity)
-        else:
-            return(result.intensity, result.sigma)
-    def get_radially_integrated_data(self, spec_scans:BaseModel, scan_number:int, scan_step_index:int):
-        """Return radially-integrated data for the scan step specified.
-        
-        :param spec_scans: An instance of `SpecScans` containing the scan step requested.
+            return result.intensity
+        return result.intensity, result.sigma
+
+    def get_radially_integrated_data(self,
+                                     spec_scans:BaseModel,
+                                     scan_number:int,
+                                     scan_step_index:int):
+        """Return radially-integrated data for the scan step
+        specified.
+
+        :param spec_scans: An instance of `SpecScans` containing the
+            scan step requested.
         :type spec_scans: SpecScans
-        :param scan_number: The number of the scan containing the scan step requested.
+        :param scan_number: The number of the scan containing the scan
+            step requested.
         :type scan_number: int
         :param scan_step_index: The index of the scan step requested.
         :type scan_step_index: int
-        :return: A 1D array of radially-integrated raw detector intensities.
+        :return: A 1D array of radially-integrated raw detector
+            intensities.
         :rtype: np.ndarray
         """
-        # Handle idiosyncracies of azimuthal ranges in pyFAI
-        # Adjust chi ranges to get a continuous range of iintegrated data
-        chi_min, chi_max, chi_offset, chi_disc = self.get_azimuthal_adjustments()
+        # Handle idiosyncracies of azimuthal ranges in pyFAI Adjust
+        # chi ranges to get a continuous range of iintegrated data
+        chi_min, chi_max, *adjust = self.get_azimuthal_adjustments()
         # Perform radial integration on a detector-by-detector basis.
-        I_each_detector = []
+        intensity_each_detector = []
         variance_each_detector = []
         integrators = self.get_azimuthal_integrators()
-        for i,(integrator,detector) in enumerate(zip(integrators,self.detectors)):
-            detector_data = spec_scans.get_detector_data([detector], scan_number, scan_step_index)[0]
-            result = integrator.integrate_radial(detector_data, self.azimuthal_npt,
-                                                 unit=self.azimuthal_units, azimuth_range=(chi_min,chi_max),
-                                                 radial_unit=self.radial_units, radial_range=(self.radial_min,self.radial_max),
-                                                 mask=detector.mask_array) #, error_model=self.error_model)
-            I_each_detector.append(result.intensity)
+        for integrator, detector in zip(integrators, self.detectors):
+            detector_data = spec_scans.get_detector_data(
+                [detector], scan_number, scan_step_index)[0]
+            result = integrator.integrate_radial(
+                detector_data,
+                self.azimuthal_npt,
+                unit=self.azimuthal_units,
+                azimuth_range=(chi_min, chi_max),
+                radial_unit=self.radial_units,
+                radial_range=(self.radial_min, self.radial_max),
+                mask=detector.mask_array)  # , error_model=self.error_model)
+            intensity_each_detector.append(result.intensity)
             if result.sigma is not None:
                 variance_each_detector.append(result.sigma**2)
-        # Add the individual detectors' integrated intensities together
-        I = np.nansum(I_each_detector, axis=0)
+        # Add the individual detectors' integrated intensities
+        # together
+        intensity = np.nansum(intensity_each_detector, axis=0)
         # Ignore data at values of chi for which there was no data
-        I = np.where(I==0, np.nan, I)
-        if len(I_each_detector) != len(variance_each_detector):
-            return(I)
-        else:
-            # Get the standard deviation of the summed detectors' intensities
-            sigma = np.sqrt(np.nansum(variance_each_detector, axis=0))
-            return(I, sigma)
-    def get_cake_integrated_data(self, spec_scans:BaseModel, scan_number:int, scan_step_index:int):
+        intensity = np.where(intensity == 0, np.nan, intensity)
+        if len(intensity_each_detector) != len(variance_each_detector):
+            return intensity
+
+        # Get the standard deviation of the summed detectors'
+        # intensities
+        sigma = np.sqrt(np.nansum(variance_each_detector, axis=0))
+        return intensity, sigma
+
+    def get_cake_integrated_data(self,
+                                 spec_scans:BaseModel,
+                                 scan_number:int,
+                                 scan_step_index:int):
         """Return cake-integrated data for the scan step specified.
-        
-        :param spec_scans: An instance of `SpecScans` containing the scan step requested.
+
+        :param spec_scans: An instance of `SpecScans` containing the
+            scan step requested.
         :type spec_scans: SpecScans
-        :param scan_number: The number of the scan containing the scan step requested.
+        :param scan_number: The number of the scan containing the scan
+            step requested.
         :type scan_number: int
         :param scan_step_index: The index of the scan step requested.
         :type scan_step_index: int
-        :return: A 2D array of cake-integrated raw detector intensities.
+        :return: A 2D array of cake-integrated raw detector
+            intensities.
         :rtype: np.ndarray
         """
-        detector_data = spec_scans.get_detector_data(self.detectors, scan_number, scan_step_index)
+        detector_data = spec_scans.get_detector_data(
+            self.detectors, scan_number, scan_step_index)
         integrator = self.get_multi_geometry_integrator()
         lst_mask = [detector.mask_array for detector in self.detectors]
-        result = integrator.integrate2d(detector_data, lst_mask=lst_mask,
-                                        npt_rad=self.radial_npt, npt_azim=self.azimuthal_npt,
-                                        method='bbox',
-                                        error_model=self.error_model)
+        result = integrator.integrate2d(
+            detector_data,
+            lst_mask=lst_mask,
+            npt_rad=self.radial_npt,
+            npt_azim=self.azimuthal_npt,
+            method='bbox',
+            error_model=self.error_model)
         if result.sigma is None:
-            return(result.intensity)
-        else:
-            return(result.intensity, result.sigma)
-    def get_integrated_data(self, spec_scans:BaseModel, scan_number:int, scan_step_index:int):
+            return result.intensity
+        return result.intensity, result.sigma
+
+    def get_integrated_data(self,
+                            spec_scans:BaseModel,
+                            scan_number:int,
+                            scan_step_index:int):
         """Return integrated data for the scan step specified.
-        
-        :param spec_scans: An instance of `SpecScans` containing the scan step requested.
+
+        :param spec_scans: An instance of `SpecScans` containing the
+            scan step requested.
         :type spec_scans: SpecScans
-        :param scan_number: The number of the scan containing the scan step requested.
+        :param scan_number: The number of the scan containing the scan
+            step requested.
         :type scan_number: int
         :param scan_step_index: The index of the scan step requested.
         :type scan_step_index: int
         :return: An array of integrated raw detector intensities.
         :rtype: np.ndarray
         """
         if self.integration_type == 'azimuthal':
-            return(self.get_azimuthally_integrated_data(spec_scans, scan_number, scan_step_index))
-        elif self.integration_type == 'radial':
-            return(self.get_radially_integrated_data(spec_scans, scan_number, scan_step_index))
-        elif self.integration_type == 'cake':
-            return(self.get_cake_integrated_data(spec_scans, scan_number, scan_step_index))
+            return self.get_azimuthally_integrated_data(spec_scans,
+                                                        scan_number,
+                                                        scan_step_index)
+        if self.integration_type == 'radial':
+            return self.get_radially_integrated_data(spec_scans,
+                                                     scan_number,
+                                                     scan_step_index)
+        if self.integration_type == 'cake':
+            return self.get_cake_integrated_data(spec_scans,
+                                                 scan_number,
+                                                 scan_step_index)
+        return None
 
     @property
     def integrated_data_coordinates(self):
-        """
-        Return a dictionary of coordinate arrays for navigating the dimension(s)
-        of the integrated data produced by this instance of `IntegrationConfig`.
-        
-        :return: A dictionary with either one or two keys: 'azimuthal' and/or
-            'radial', each of which points to a 1-D `numpy` array of coordinate
-            values.
+        """Return a dictionary of coordinate arrays for navigating the
+        dimension(s) of the integrated data produced by this instance
+        of `IntegrationConfig`.
+
+        :return: A dictionary with either one or two keys: 'azimuthal'
+            and/or 'radial', each of which points to a 1-D `numpy`
+            array of coordinate values.
         :rtype: dict[str,np.ndarray]
         """
         if self.integration_type == 'azimuthal':
-            return(get_integrated_data_coordinates(radial_range=(self.radial_min,self.radial_max),
-                                                   radial_npt=self.radial_npt))
-        elif self.integration_type == 'radial':
-            return(get_integrated_data_coordinates(azimuthal_range=(self.azimuthal_min,self.azimuthal_max),
-                                                   azimuthal_npt=self.azimuthal_npt))
-        elif self.integration_type == 'cake':
-            return(get_integrated_data_coordinates(radial_range=(self.radial_min,self.radial_max),
-                                                   radial_npt=self.radial_npt,
-                                                   azimuthal_range=(self.azimuthal_min,self.azimuthal_max),
-                                                   azimuthal_npt=self.azimuthal_npt))
+            return get_integrated_data_coordinates(
+                radial_range=(self.radial_min, self.radial_max),
+                radial_npt=self.radial_npt)
+        if self.integration_type == 'radial':
+            return get_integrated_data_coordinates(
+                azimuthal_range=(self.azimuthal_min, self.azimuthal_max),
+                azimuthal_npt=self.azimuthal_npt)
+        if self.integration_type == 'cake':
+            return get_integrated_data_coordinates(
+                radial_range=(self.radial_min, self.radial_max),
+                radial_npt=self.radial_npt,
+                azimuthal_range=(self.azimuthal_min, self.azimuthal_max),
+                azimuthal_npt=self.azimuthal_npt)
+        return None
+
     @property
     def integrated_data_dims(self):
-        """Return a tuple of the coordinate labels for the integrated data
-        produced by this instance of `IntegrationConfig`.
+        """Return a tuple of the coordinate labels for the integrated
+        data produced by this instance of `IntegrationConfig`.
         """
         directions = list(self.integrated_data_coordinates.keys())
-        dim_names = [getattr(self, f'{direction}_units') for direction in directions]
-        return(dim_names)
+        dim_names = [getattr(self, f'{direction}_units')
+                     for direction in directions]
+        return dim_names
+
     @property
     def integrated_data_shape(self):
-        """Return a tuple representing the shape of the integrated data
-        produced by this instance of `IntegrationConfig` for a single scan step.
-        """
-        return(tuple([len(coordinate_values) for coordinate_name,coordinate_values in self.integrated_data_coordinates.items()]))
+        """Return a tuple representing the shape of the integrated
+        data produced by this instance of `IntegrationConfig` for a
+        single scan step.
+        """
+        return tuple([len(coordinate_values)
+                      for coordinate_name, coordinate_values
+                      in self.integrated_data_coordinates.items()])
+
 
 @cache
 def get_azimuthal_adjustments(chi_min:float, chi_max:float):
-    """
-    Fix chi discontinuity at 180 degrees and return the adjusted chi range,
-    offset, and discontinuty.
+    """Fix chi discontinuity at 180 degrees and return the adjusted
+    chi range, offset, and discontinuty.
 
-    If the discontinuity is crossed, obtain the offset to artificially rotate
-    detectors to achieve a continuous azimuthal integration range.
+    If the discontinuity is crossed, obtain the offset to artificially
+    rotate detectors to achieve a continuous azimuthal integration
+    range.
 
     :param chi_min: The minimum value of the azimuthal range.
     :type chi_min: float
     :param chi_max: The maximum value of the azimuthal range.
     :type chi_max: float
-    :return: The following four values: the adjusted minimum value of the
-        azimuthal range, the adjusted maximum value of the azimuthal range, the
-        value by which the chi angle was adjusted, the position of the chi
-        discontinuity.
+    :return: The following four values: the adjusted minimum value of
+        the azimuthal range, the adjusted maximum value of the
+        azimuthal range, the value by which the chi angle was
+        adjusted, the position of the chi discontinuity.
     """
     # Fix chi discontinuity at 180 degrees for now.
     chi_disc = 180
-    # If the discontinuity is crossed, artificially rotate the detectors to
-    # achieve a continuous azimuthal integration range
+    # If the discontinuity is crossed, artificially rotate the
+    # detectors to achieve a continuous azimuthal integration range
     if chi_min < chi_disc and chi_max > chi_disc:
         chi_offset = chi_max - chi_disc
     else:
         chi_offset = 0
-    return(chi_min-chi_offset, chi_max-chi_offset, chi_offset, chi_disc)
+    return chi_min-chi_offset, chi_max-chi_offset, chi_offset, chi_disc
+
+
 @cache
 def get_azimuthal_integrators(poni_files:tuple, chi_offset=0):
-    """
-    Return a list of `AzimuthalIntegrator` objects generated from PONI files.
-    
-    :param poni_files: Tuple of strings, each string being a path to a PONI file. : tuple
+    """Return a list of `AzimuthalIntegrator` objects generated from
+    PONI files.
+
+    :param poni_files: Tuple of strings, each string being a path to a
+        PONI file.
     :type poni_files: tuple
-    :param chi_offset: The angle in degrees by which the `AzimuthalIntegrator` objects will be rotated, defaults to 0.
+    :param chi_offset: The angle in degrees by which the
+        `AzimuthalIntegrator` objects will be rotated, defaults to 0.
     :type chi_offset: float, optional
     :return: List of `AzimuthalIntegrator` objects
     :rtype: list[pyFAI.azimuthalIntegrator.AzimuthalIntegrator]
     """
     ais = []
     for poni_file in poni_files:
         ai = copy.deepcopy(azimuthal_integrator(poni_file))
         ai.rot3 += chi_offset * np.pi/180
         ais.append(ai)
-    return(ais)
+    return ais
+
+
 @cache
-def get_multi_geometry_integrator(poni_files:tuple, radial_unit:str, radial_range:tuple, azimuthal_range:tuple):
-    """Return a `MultiGeometry` instance that can be used for azimuthal or cake
-    integration.
+def get_multi_geometry_integrator(poni_files:tuple, radial_unit:str,
+                                  radial_range:tuple, azimuthal_range:tuple):
+    """Return a `MultiGeometry` instance that can be used for
+    azimuthal or cake integration.
 
-    :param poni_files: Tuple of PONI files that describe the detectors to be
-        integrated.
+    :param poni_files: Tuple of PONI files that describe the detectors
+        to be integrated.
     :type poni_files: tuple
     :param radial_unit: Unit to use for radial integration range.
     :type radial_unit: str
     :param radial_range: Tuple describing the range for radial integration.
     :type radial_range: tuple[float,float]
-    :param azimuthal_range:Tuple describing the range for azimuthal integration.
-    :type azimuthal_range: tuple[float,float]
-    :return: `MultiGeometry` instance that can be used for azimuthal or cake
+    :param azimuthal_range:Tuple describing the range for azimuthal
         integration.
+    :type azimuthal_range: tuple[float,float]
+    :return: `MultiGeometry` instance that can be used for azimuthal
+        or cake integration.
     :rtype: pyFAI.multi_geometry.MultiGeometry
     """
-    chi_min, chi_max, chi_offset, chi_disc = get_azimuthal_adjustments(*azimuthal_range)
-    ais = copy.deepcopy(get_azimuthal_integrators(poni_files, chi_offset=chi_offset))
-    multi_geometry = MultiGeometry(ais,
-                                   unit=radial_unit,
-                                   radial_range=radial_range,
-                                   azimuth_range=(chi_min,chi_max),
-                                   wavelength=sum([ai.wavelength for ai in ais])/len(ais),
-                                   chi_disc=chi_disc)
-    return(multi_geometry)
+    chi_min, chi_max, chi_offset, chi_disc = \
+        get_azimuthal_adjustments(*azimuthal_range)
+    ais = copy.deepcopy(get_azimuthal_integrators(poni_files,
+                                                  chi_offset=chi_offset))
+    multi_geometry = MultiGeometry(
+        ais,
+        unit=radial_unit,
+        radial_range=radial_range,
+        azimuth_range=(chi_min, chi_max),
+        wavelength=sum([ai.wavelength for ai in ais])/len(ais),
+        chi_disc=chi_disc)
+    return multi_geometry
+
+
 @cache
-def get_integrated_data_coordinates(azimuthal_range:tuple=None, azimuthal_npt:int=None, radial_range:tuple=None, radial_npt:int=None):
-    """
-    Return a dictionary of coordinate arrays for the specified radial and/or
-    azimuthal integration ranges.
-        
-    :param azimuthal_range: Tuple specifying the range of azimuthal angles over
-        which to generate coordinates, in the format (min, max), defaults to
-        None.
+def get_integrated_data_coordinates(azimuthal_range:tuple = None,
+                                    azimuthal_npt:int = None,
+                                    radial_range:tuple = None,
+                                    radial_npt:int = None):
+    """Return a dictionary of coordinate arrays for the specified
+    radial and/or azimuthal integration ranges.
+
+    :param azimuthal_range: Tuple specifying the range of azimuthal
+        angles over which to generate coordinates, in the format (min,
+        max), defaults to None.
     :type azimuthal_range: tuple[float,float], optional
-    :param azimuthal_npt: Number of azimuthal coordinate points to generate,
-        defaults to None.
+    :param azimuthal_npt: Number of azimuthal coordinate points to
+        generate, defaults to None.
     :type azimuthal_npt: int, optional
-    :param radial_range: Tuple specifying the range of radial distances over
-        which to generate coordinates, in the format (min, max), defaults to
-        None.
+    :param radial_range: Tuple specifying the range of radial
+        distances over which to generate coordinates, in the format
+        (min, max), defaults to None.
     :type radial_range: tuple[float,float], optional
-    :param radial_npt: Number of radial coordinate points to generate, defaults
-        to None.
+    :param radial_npt: Number of radial coordinate points to generate,
+        defaults to None.
     :type radial_npt: int, optional
-    :return: A dictionary with either one or two keys: 'azimuthal' and/or
-        'radial', each of which points to a 1-D `numpy` array of coordinate
-        values.
+    :return: A dictionary with either one or two keys: 'azimuthal'
+        and/or 'radial', each of which points to a 1-D `numpy` array
+        of coordinate values.
     :rtype: dict[str,np.ndarray]
     """
     integrated_data_coordinates = {}
     if azimuthal_range is not None and azimuthal_npt is not None:
-        integrated_data_coordinates['azimuthal'] = np.linspace(*azimuthal_range, azimuthal_npt)
+        integrated_data_coordinates['azimuthal'] = np.linspace(
+            *azimuthal_range, azimuthal_npt)
     if radial_range is not None and radial_npt is not None:
-        integrated_data_coordinates['radial'] = np.linspace(*radial_range, radial_npt)
-    return(integrated_data_coordinates)
+        integrated_data_coordinates['radial'] = np.linspace(
+            *radial_range, radial_npt)
+    return integrated_data_coordinates
```

### Comparing `ChessAnalysisPipeline-0.0.5/CHAP/common/models/map.py` & `ChessAnalysisPipeline-0.0.6/CHAP/common/models/map.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,534 +2,686 @@
 import os
 from typing import Literal, Optional, Union
 
 import numpy as np
 from pydantic import (BaseModel,
                       conint,
                       conlist,
-                      confloat,
                       constr,
                       FilePath,
                       PrivateAttr,
-                      ValidationError,
                       validator)
 from pyspec.file.spec import FileSpec
 
+
 class Sample(BaseModel):
-    """
-    Class representing a sample metadata configuration.
+    """Class representing a sample metadata configuration.
 
     :ivar name: The name of the sample.
     :type name: str
     :ivar description: A description of the sample.
     :type description: Optional[str]
     """
     name: constr(min_length=1)
     description: Optional[str]
 
+
 class SpecScans(BaseModel):
-    """
-    Class representing a set of scans from a single SPEC file.
+    """Class representing a set of scans from a single SPEC file.
 
     :ivar spec_file: Path to the SPEC file.
     :type spec_file: str
     :ivar scan_numbers: List of scan numbers to use.
     :type scan_numbers: list[int]
     """
     spec_file: FilePath
     scan_numbers: conlist(item_type=conint(gt=0), min_items=1)
+
     @validator('spec_file', allow_reuse=True)
     def validate_spec_file(cls, spec_file):
-        """
-        Validate the specified SPEC file.
+        """Validate the specified SPEC file.
 
         :param spec_file: Path to the SPEC file.
         :type spec_file: str
         :raises ValueError: If the SPEC file is invalid.
         :return: Absolute path to the SPEC file, if it is valid.
         :rtype: str
         """
         try:
             spec_file = os.path.abspath(spec_file)
             sspec_file = FileSpec(spec_file)
         except:
-            raise(ValueError(f'Invalid SPEC file {spec_file}'))
-        else:
-            return(spec_file)
+            raise ValueError(f'Invalid SPEC file {spec_file}')
+        return spec_file
+
     @validator('scan_numbers', allow_reuse=True)
     def validate_scan_numbers(cls, scan_numbers, values):
-        """
-        Validate the specified list of scan numbers.
+        """Validate the specified list of scan numbers.
 
         :param scan_numbers: List of scan numbers.
         :type scan_numbers: list of int
         :param values: Dictionary of values for all fields of the model.
         :type values: dict
-        :raises ValueError: If a specified scan number is not found in the SPEC file.
+        :raises ValueError: If a specified scan number is not found in
+            the SPEC file.
         :return: List of scan numbers.
         :rtype: list of int
         """
         spec_file = values.get('spec_file')
         if spec_file is not None:
             spec_scans = FileSpec(spec_file)
             for scan_number in scan_numbers:
                 scan = spec_scans.get_scan_by_number(scan_number)
                 if scan is None:
-                    raise(ValueError(f'There is no scan number {scan_number} in {spec_file}'))
-        return(scan_numbers)
+                    raise ValueError(
+                        f'No scan number {scan_number} in {spec_file}')
+        return scan_numbers
 
     @property
     def scanparsers(self):
-        '''A list of `ScanParser`s for each of the scans specified by the SPEC
-        file and scan numbers belonging to this instance of `SpecScans`
-        '''
-        return([self.get_scanparser(scan_no) for scan_no in self.scan_numbers])
+        """A list of `ScanParser`s for each of the scans specified by
+        the SPEC file and scan numbers belonging to this instance of
+        `SpecScans`
+        """
+        return [self.get_scanparser(scan_no) for scan_no in self.scan_numbers]
 
     def get_scanparser(self, scan_number):
-        """This method returns a `ScanParser` for the specified scan number in
-        the specified SPEC file.
+        """This method returns a `ScanParser` for the specified scan
+        number in the specified SPEC file.
 
         :param scan_number: Scan number to get a `ScanParser` for
         :type scan_number: int
         :return: `ScanParser` for the specified scan number
         :rtype: ScanParser
         """
-        return(get_scanparser(self.spec_file, scan_number))
+        return get_scanparser(self.spec_file, scan_number)
+
     def get_index(self, scan_number:int, scan_step_index:int, map_config):
-        """This method returns a tuple representing the index of a specific step
-        in a specific spec scan within a map.
+        """This method returns a tuple representing the index of a
+        specific step in a specific spec scan within a map.
 
         :param scan_number: Scan number to get index for
         :type scan_number: int
         :param scan_step_index: Scan step index to get index for
         :type scan_step_index: int
         :param map_config: Map configuration to get index for
         :type map_config: MapConfig
-        :return: Index for the specified scan number and scan step index within
-            the specified map configuration
+        :return: Index for the specified scan number and scan step
+            index within the specified map configuration
         :rtype: tuple
         """
         index = ()
         for independent_dimension in map_config.independent_dimensions:
-            coordinate_index = list(map_config.coords[independent_dimension.label]).index(independent_dimension.get_value(self, scan_number, scan_step_index))
+            coordinate_index = list(
+                map_config.coords[independent_dimension.label]).index(
+                    independent_dimension.get_value(
+                        self, scan_number, scan_step_index))
             index = (coordinate_index, *index)
-        return(index)
-    def get_detector_data(self, detectors:list, scan_number:int, scan_step_index:int):
-        """
-        Return the raw data from the specified detectors at the specified scan
-        number and scan step index.
+        return index
+
+    def get_detector_data(self,
+                          detectors:list,
+                          scan_number:int,
+                          scan_step_index:int):
+        """Return the raw data from the specified detectors at the
+        specified scan number and scan step index.
 
         :param detectors: List of detector prefixes to get raw data for
         :type detectors: list[str]
         :param scan_number: Scan number to get data for
         :type scan_number: int
         :param scan_step_index: Scan step index to get data for
         :type scan_step_index: int
-        :return: Data from the specified detectors for the specified scan number
-            and scan step index
+        :return: Data from the specified detectors for the specified
+            scan number and scan step index
         :rtype: list[np.ndarray]
         """
-        return(get_detector_data(tuple([detector.prefix for detector in detectors]), self.spec_file, scan_number, scan_step_index))
+        return get_detector_data(
+            tuple([detector.prefix for detector in detectors]),
+            self.spec_file,
+            scan_number,
+            scan_step_index)
+
+
 @cache
 def get_available_scan_numbers(spec_file:str):
     scans = FileSpec(spec_file).scans
     scan_numbers = list(scans.keys())
-    return(scan_numbers)
+    return scan_numbers
+
+
 @cache
 def get_scanparser(spec_file:str, scan_number:int):
     if scan_number not in get_available_scan_numbers(spec_file):
-        return(None)
-    else:
-        return(ScanParser(spec_file, scan_number))
+        return None
+    return ScanParser(spec_file, scan_number)
+
+
 @lru_cache(maxsize=10)
-def get_detector_data(detector_prefixes:tuple, spec_file:str, scan_number:int, scan_step_index:int):
+def get_detector_data(
+        detector_prefixes:tuple,
+        spec_file:str,
+        scan_number:int,
+        scan_step_index:int):
     detector_data = []
     scanparser = get_scanparser(spec_file, scan_number)
     for prefix in detector_prefixes:
         image_data = scanparser.get_detector_data(prefix, scan_step_index)
         detector_data.append(image_data)
-    return(detector_data)
+    return detector_data
+
 
 class PointByPointScanData(BaseModel):
-    """Class representing a source of raw scalar-valued data for which a value
-    was recorded at every point in a `MapConfig`.
+    """Class representing a source of raw scalar-valued data for which
+    a value was recorded at every point in a `MapConfig`.
 
-    :ivar label: A user-defined label for referring to this data in the NeXus
-        file and in other tools.
+    :ivar label: A user-defined label for referring to this data in
+        the NeXus file and in other tools.
     :type label: str
     :ivar units: The units in which the data were recorded.
     :type units: str
-    :ivar data_type: Represents how these data were recorded at time of data
-        collection.
+    :ivar data_type: Represents how these data were recorded at time
+        of data collection.
     :type data_type: Literal['spec_motor', 'scan_column', 'smb_par']
-    :ivar name: Represents the name with which these raw data were recorded at
-        time of data collection.
+    :ivar name: Represents the name with which these raw data were
+        recorded at time of data collection.
     :type name: str
     """
     label: constr(min_length=1)
     units: constr(strip_whitespace=True, min_length=1)
     data_type: Literal['spec_motor', 'scan_column', 'smb_par']
     name: constr(strip_whitespace=True, min_length=1)
+
     @validator('label')
     def validate_label(cls, label):
-        """Validate that the supplied `label` does not conflict with any of the
-        values for `label` reserved for certain data needed to perform
-        corrections.
-        
+        """Validate that the supplied `label` does not conflict with
+        any of the values for `label` reserved for certain data needed
+        to perform corrections.
+
         :param label: The value of `label` to validate
         :type label: str
         :raises ValueError: If `label` is one of the reserved values.
-        :return: The original supplied value `label`, if it is allowed.
+        :return: The original supplied value `label`, if it is
+            allowed.
         :rtype: str
         """
-        #if (not issubclass(cls,CorrectionsData)) and label in CorrectionsData.__fields__['label'].type_.__args__:
-        if (not issubclass(cls,CorrectionsData)) and label in CorrectionsData.reserved_labels():
-            raise(ValueError(f'{cls.__name__}.label may not be any of the following reserved values: {CorrectionsData.reserved_labels()}'))
-        return(label)
+        if ((not issubclass(cls,CorrectionsData))
+                and label in CorrectionsData.reserved_labels()):
+            raise ValueError(
+                f'{cls.__name__}.label may not be any of the following '
+                f'reserved values: {CorrectionsData.reserved_labels()}')
+        return label
+
     def validate_for_station(self, station:str):
-        """Validate this instance of `PointByPointScanData` for a certain choice
-        of station (beamline).
-        
+        """Validate this instance of `PointByPointScanData` for a
+        certain choice of station (beamline).
+
         :param station: The name of the station (in 'idxx' format).
         :type station: str
-        :raises TypeError: If the station is not compatible with the value of the
-            `data_type` attribute for this instance of PointByPointScanData.
+        :raises TypeError: If the station is not compatible with the
+            value of the `data_type` attribute for this instance of
+            PointByPointScanData.
         :return: None
         :rtype: None
         """
-        if station.lower() not in ('id1a3', 'id3a') and self.data_type == 'smb_par':
-            raise(TypeError(f'{self.__class__.__name__}.data_type may not be "smb_par" when station is "{station}"'))
-    def validate_for_spec_scans(self, spec_scans:list[SpecScans], scan_step_index:Union[Literal['all'],int]='all'):
-        """Validate this instance of `PointByPointScanData` for a list of
-        `SpecScans`.
-
-        :param spec_scans: A list of `SpecScans` whose raw data will be checked
-            for the presence of the data represented by this instance of
-            `PointByPointScanData`
+        if (station.lower() not in ('id1a3', 'id3a')
+                and self.data_type == 'smb_par'):
+            raise TypeError(
+                f'{self.__class__.__name__}.data_type may not be "smb_par" '
+                f'when station is "{station}"')
+
+    def validate_for_spec_scans(
+            self, spec_scans:list[SpecScans],
+            scan_step_index:Union[Literal['all'],int] = 'all'):
+        """Validate this instance of `PointByPointScanData` for a list
+        of `SpecScans`.
+
+        :param spec_scans: A list of `SpecScans` whose raw data will
+            be checked for the presence of the data represented by
+            this instance of `PointByPointScanData`
         :type spec_scans: list[SpecScans]
-        :param scan_step_index: A specific scan step index to validate, defaults
-            to `'all'`.
+        :param scan_step_index: A specific scan step index to validate,
+            defaults to `'all'`.
         :type scan_step_index: Union[Literal['all'],int], optional
         :raises RuntimeError: If the data represented by this instance of
             `PointByPointScanData` is missing for the specified scan steps.
         :return: None
         :rtype: None
         """
         for scans in spec_scans:
             for scan_number in scans.scan_numbers:
                 scanparser = scans.get_scanparser(scan_number)
                 if scan_step_index == 'all':
                     scan_step_index_range = range(scanparser.spec_scan_npts)
                 else:
-                    scan_step_index_range = range(scan_step_index,scan_step_index+1)
+                    scan_step_index_range = range(
+                        scan_step_index, 1+scan_step_index)
                 for index in scan_step_index_range:
                     try:
                         self.get_value(scans, scan_number, index)
                     except:
-                        raise(RuntimeError(f'Could not find data for {self.name} (data_type "{self.data_type}") on scan number {scan_number} for index {index} in spec file {scans.spec_file}'))
-    def get_value(self, spec_scans:SpecScans, scan_number:int, scan_step_index:int):
-        """Return the value recorded for this instance of `PointByPointScanData`
-        at a specific scan step.
-        
-        :param spec_scans: An instance of `SpecScans` in which the requested scan step occurs.
+                        raise RuntimeError(
+                            f'Could not find data for {self.name} '
+                            f'(data_type "{self.data_type}") '
+                            f'on scan number {scan_number} '
+                            f'for index {index} '
+                            f'in spec file {scans.spec_file}')
+
+    def get_value(self, spec_scans:SpecScans,
+                  scan_number:int, scan_step_index:int):
+        """Return the value recorded for this instance of
+        `PointByPointScanData` at a specific scan step.
+
+        :param spec_scans: An instance of `SpecScans` in which the
+            requested scan step occurs.
         :type spec_scans: SpecScans
-        :param scan_number: The number of the scan in which the requested scan step occurs.
+        :param scan_number: The number of the scan in which the
+            requested scan step occurs.
         :type scan_number: int
         :param scan_step_index: The index of the requested scan step.
         :type scan_step_index: int
-        :return: The value recorded of the data represented by this instance of
-            `PointByPointScanData` at the scan step requested
+        :return: The value recorded of the data represented by this
+            instance of `PointByPointScanData` at the scan step
+            requested
         :rtype: float
         """
         if self.data_type == 'spec_motor':
-            return(get_spec_motor_value(spec_scans.spec_file, scan_number, scan_step_index, self.name))
-        elif self.data_type == 'scan_column':
-            return(get_spec_counter_value(spec_scans.spec_file, scan_number, scan_step_index, self.name))
-        elif self.data_type == 'smb_par':
-            return(get_smb_par_value(spec_scans.spec_file, scan_number, self.name))
+            return get_spec_motor_value(spec_scans.spec_file,
+                                        scan_number,
+                                        scan_step_index,
+                                        self.name)
+        if self.data_type == 'scan_column':
+            return get_spec_counter_value(spec_scans.spec_file,
+                                          scan_number,
+                                          scan_step_index,
+                                          self.name)
+        if self.data_type == 'smb_par':
+            return get_smb_par_value(spec_scans.spec_file,
+                                     scan_number,
+                                     self.name)
+        return None
+
+
 @cache
-def get_spec_motor_value(spec_file:str, scan_number:int, scan_step_index:int, spec_mnemonic:str):
-    """Return the value recorded for a SPEC motor at a specific scan step.
+def get_spec_motor_value(spec_file:str, scan_number:int,
+                         scan_step_index:int, spec_mnemonic:str):
+    """Return the value recorded for a SPEC motor at a specific scan
+    step.
 
-    :param spec_file: Location of a SPEC file in which the requested scan step occurs.
+    :param spec_file: Location of a SPEC file in which the requested
+        scan step occurs.
     :type spec_scans: str
-    :param scan_number: The number of the scan in which the requested scan step occurs.
+    :param scan_number: The number of the scan in which the requested
+        scan step occurs.
     :type scan_number: int
     :param scan_step_index: The index of the requested scan step.
     :type scan_step_index: int
     :param spec_mnemonic: The menmonic of a SPEC motor.
     :type spec_mnemonic: str
     :return: The value of the motor at the scan step requested
     :rtype: float
     """
     scanparser = get_scanparser(spec_file, scan_number)
     if spec_mnemonic in scanparser.spec_scan_motor_mnes:
         motor_i = scanparser.spec_scan_motor_mnes.index(spec_mnemonic)
         if scan_step_index >= 0:
-            scan_step = np.unravel_index(scan_step_index, scanparser.spec_scan_shape, order='F')
-            motor_value = scanparser.spec_scan_motor_vals[motor_i][scan_step[motor_i]]
+            scan_step = np.unravel_index(
+                scan_step_index,
+                scanparser.spec_scan_shape,
+                order='F')
+            motor_value = \
+                scanparser.spec_scan_motor_vals[motor_i][scan_step[motor_i]]
         else:
             motor_value = scanparser.spec_scan_motor_vals[motor_i]
     else:
         motor_value = scanparser.get_spec_positioner_value(spec_mnemonic)
-    return(motor_value)
+    return motor_value
+
+
 @cache
-def get_spec_counter_value(spec_file:str, scan_number:int, scan_step_index:int, spec_column_label:str):
-    """Return the value recorded for a SPEC counter at a specific scan step.
+def get_spec_counter_value(spec_file:str, scan_number:int,
+                           scan_step_index:int, spec_column_label:str):
+    """Return the value recorded for a SPEC counter at a specific scan
+    step.
 
-    :param spec_file: Location of a SPEC file in which the requested scan step occurs.
+    :param spec_file: Location of a SPEC file in which the requested
+        scan step occurs.
     :type spec_scans: str
-    :param scan_number: The number of the scan in which the requested scan step occurs.
+    :param scan_number: The number of the scan in which the requested
+        scan step occurs.
     :type scan_number: int
     :param scan_step_index: The index of the requested scan step.
     :type scan_step_index: int
     :param spec_column_label: The label of a SPEC data column.
     :type spec_column_label: str
     :return: The value of the counter at the scan step requested
     :rtype: float
     """
     scanparser = get_scanparser(spec_file, scan_number)
     if scan_step_index >= 0:
-        return(scanparser.spec_scan_data[spec_column_label][scan_step_index])
-    else:
-        return(scanparser.spec_scan_data[spec_column_label])
+        return scanparser.spec_scan_data[spec_column_label][scan_step_index]
+    return scanparser.spec_scan_data[spec_column_label]
+
+
 @cache
 def get_smb_par_value(spec_file:str, scan_number:int, par_name:str):
-    """Return the value recorded for a specific scan in SMB-tyle .par file.
+    """Return the value recorded for a specific scan in SMB-tyle .par
+    file.
 
-    :param spec_file: Location of a SPEC file in which the requested scan step occurs.
+    :param spec_file: Location of a SPEC file in which the requested
+        scan step occurs.
     :type spec_scans: str
-    :param scan_number: The number of the scan in which the requested scan step occurs.
+    :param scan_number: The number of the scan in which the requested
+        scan step occurs.
     :type scan_number: int
     :param par_name: The name of the column in the .par file
     :type par_name: str
     :return: The value of the .par file value for  the scan requested.
     :rtype: float
     """
     scanparser = get_scanparser(spec_file, scan_number)
-    return(scanparser.pars[par_name])
+    return scanparser.pars[par_name]
+
+
 def validate_data_source_for_map_config(data_source, values):
+    """Confirm that an instance of PointByPointScanData is valid for
+    the station and scans provided by a map configuration dictionary.
+
+    :param data_source: the input object to validate
+    :type data_source: PintByPointScanData
+    :param values: the map configuration dictionary
+    :type values: dict
+    :raises Exception: if `data_source` cannot be validated for
+        `values`.
+    :return: `data_source`, iff it is valid.
+    :rtype: PointByPointScanData
+    """
     if data_source is not None:
         import_scanparser(values.get('station'), values.get('experiment_type'))
         data_source.validate_for_station(values.get('station'))
         data_source.validate_for_spec_scans(values.get('spec_scans'))
-    return(data_source)
+    return data_source
 
-class CorrectionsData(PointByPointScanData):
-    """Class representing the special instances of `PointByPointScanData` that
-    are used by certain kinds of `CorrectionConfig` tools.
 
-    :ivar label: One of the reserved values required by `CorrectionConfig`, 
-        `'presample_intensity'`, `'postsample_intensity'`, or
-        `'dwell_time_actual'`.
-    :type label: Literal['presample_intensity','postsample_intensity','dwell_time_actual']
+class CorrectionsData(PointByPointScanData):
+    """Class representing the special instances of
+    `PointByPointScanData` that are used by certain kinds of
+    `CorrectionConfig` tools.
+
+    :ivar label: One of the reserved values required by
+        `CorrectionConfig`, `'presample_intensity'`,
+        `'postsample_intensity'`, or `'dwell_time_actual'`.
+    :type label: Literal['presample_intensity',
+                         'postsample_intensity',
+                         'dwell_time_actual']
     :ivar units: The units in which the data were recorded.
     :type units: str
-    :ivar data_type: Represents how these data were recorded at time of data
-        collection.
+    :ivar data_type: Represents how these data were recorded at time
+        of data collection.
     :type data_type: Literal['scan_column', 'smb_par']
-    :ivar name: Represents the name with which these raw data were recorded at
-        time of data collection.
+    :ivar name: Represents the name with which these raw data were
+        recorded at time of data collection.
     :type name: str
     """
-    label: Literal['presample_intensity','postsample_intensity','dwell_time_actual']
+    label: Literal['presample_intensity',
+                   'postsample_intensity',
+                   'dwell_time_actual']
     data_type: Literal['scan_column','smb_par']
+
     @classmethod
     def reserved_labels(cls):
-        """Return a list of all the labels reserved for corrections-related
-        scalar data.
+        """Return a list of all the labels reserved for
+        corrections-related scalar data.
 
         :return: A list of reserved labels
         :rtype: list[str]
         """
-        return(list(cls.__fields__['label'].type_.__args__))
+        return list(cls.__fields__['label'].type_.__args__)
+
+
 class PresampleIntensity(CorrectionsData):
-    """Class representing a source of raw data for the intensity of the beam that
-    is incident on the sample.
+    """Class representing a source of raw data for the intensity of
+    the beam that is incident on the sample.
 
     :ivar label: Must be `"presample_intensity"`
     :type label: Literal["presample_intensity"]
     :ivar units: Must be `"counts"`
     :type units: Literal["counts"]
-    :ivar data_type: Represents how these data were recorded at time of data
-        collection.
+    :ivar data_type: Represents how these data were recorded at time
+        of data collection.
     :type data_type: Literal['scan_column', 'smb_par']
-    :ivar name: Represents the name with which these raw data were recorded at
-        time of data collection.
+    :ivar name: Represents the name with which these raw data were
+        recorded at time of data collection.
     :type name: str
     """
     label: Literal['presample_intensity'] = 'presample_intensity'
     units: Literal['counts'] = 'counts'
+
+
 class PostsampleIntensity(CorrectionsData):
-    """Class representing a source of raw data for the intensity of the beam that
-    has passed through the sample.
+    """Class representing a source of raw data for the intensity of
+    the beam that has passed through the sample.
 
     :ivar label: Must be `"postsample_intensity"`
     :type label: Literal["postsample_intensity"]
     :ivar units: Must be `"counts"`
     :type units: Literal["counts"]
-    :ivar data_type: Represents how these data were recorded at time of data
-        collection.
+    :ivar data_type: Represents how these data were recorded at time
+        of data collection.
     :type data_type: Literal['scan_column', 'smb_par']
-    :ivar name: Represents the name with which these raw data were recorded at
-        time of data collection.
+    :ivar name: Represents the name with which these raw data were
+        recorded at time of data collection.
     :type name: str
     """
     label: Literal['postsample_intensity'] = 'postsample_intensity'
     units: Literal['counts'] = 'counts'
+
+
 class DwellTimeActual(CorrectionsData):
-    """Class representing a source of raw data for the actual dwell time at each
-    scan point in SPEC (with some scan types, this value can vary slightly
-    point-to-point from the dwell time specified in the command).
+    """Class representing a source of raw data for the actual dwell
+    time at each scan point in SPEC (with some scan types, this value
+    can vary slightly point-to-point from the dwell time specified in
+    the command).
 
     :ivar label: Must be `"dwell_time_actual"`
     :type label: Literal["dwell_time_actual"]
     :ivar units: Must be `"counts"`
     :type units: Literal["counts"]
-    :ivar data_type: Represents how these data were recorded at time of data
-        collection.
+    :ivar data_type: Represents how these data were recorded at time
+        of data collection.
     :type data_type: Literal['scan_column', 'smb_par']
-    :ivar name: Represents the name with which these raw data were recorded at
-        time of data collection.
+    :ivar name: Represents the name with which these raw data were
+        recorded at time of data collection.
     :type name: str
     """
     label: Literal['dwell_time_actual'] = 'dwell_time_actual'
     units: Literal['s'] = 's'
 
+
 class MapConfig(BaseModel):
-    """Class representing an experiment consisting of one or more SPEC scans.
+    """Class representing an experiment consisting of one or more SPEC
+    scans.
 
     :ivar title: The title for the map configuration.
     :type title: str
-    :ivar station: The name of the station at which the map was collected.
+    :ivar station: The name of the station at which the map was
+        collected.
     :type station: Literal['id1a3','id3a','id3b']
     :ivar spec_scans: A list of the spec scans that compose the map.
     :type spec_scans: list[SpecScans]
-    :ivar independent_dimensions: A list of the sources of data representing the
-        raw values of each independent dimension of the map.
+    :ivar independent_dimensions: A list of the sources of data
+        representing the raw values of each independent dimension of
+        the map.
     :type independent_dimensions: list[PointByPointScanData]
-    :ivar presample_intensity: A source of point-by-point presample beam
-        intensity data. Required when applying a CorrectionConfig tool.
+    :ivar presample_intensity: A source of point-by-point presample
+        beam intensity data. Required when applying a CorrectionConfig
+        tool.
     :type presample_intensity: Optional[PresampleIntensity]
-    :ivar dwell_time_actual: A source of point-by-point actual dwell times for
-        spec scans. Required when applying a CorrectionConfig tool.
+    :ivar dwell_time_actual: A source of point-by-point actual dwell
+        times for spec scans. Required when applying a
+        CorrectionConfig tool.
     :type dwell_time_actual: Optional[DwellTimeActual]
-    :ivar presample_intensity: A source of point-by-point postsample beam
-        intensity data. Required when applying a CorrectionConfig tool with
-        `correction_type="flux_absorption"` or
+    :ivar presample_intensity: A source of point-by-point postsample
+        beam intensity data. Required when applying a CorrectionConfig
+        tool with `correction_type="flux_absorption"` or
         `correction_type="flux_absorption_background"`.
     :type presample_intensity: Optional[PresampleIntensity]
-    :ivar scalar_data: A list of the sources of data representing other scalar
-        raw data values collected at each point ion the map. In the NeXus file
-        representation of the map, datasets for these values will be included.
+    :ivar scalar_data: A list of the sources of data representing
+        other scalar raw data values collected at each point ion the
+        map. In the NeXus file representation of the map, datasets for
+        these values will be included.
     :type scalar_values: Optional[list[PointByPointScanData]]
     """
     title: constr(strip_whitespace=True, min_length=1)
     station: Literal['id1a3','id3a','id3b']
     experiment_type: Literal['SAXSWAXS', 'EDD', 'XRF', 'TOMO']
     sample: Sample
     spec_scans: conlist(item_type=SpecScans, min_items=1)
-    independent_dimensions: conlist(item_type=PointByPointScanData, min_items=1)
+    independent_dimensions: conlist(item_type=PointByPointScanData,
+                                    min_items=1)
     presample_intensity: Optional[PresampleIntensity]
     dwell_time_actual: Optional[DwellTimeActual]
     postsample_intensity: Optional[PostsampleIntensity]
     scalar_data: Optional[list[PointByPointScanData]] = []
     _coords: dict = PrivateAttr()
-    _validate_independent_dimensions = validator('independent_dimensions', each_item=True, allow_reuse=True)(validate_data_source_for_map_config)
-    _validate_presample_intensity = validator('presample_intensity', allow_reuse=True)(validate_data_source_for_map_config)
-    _validate_dwell_time_actual = validator('dwell_time_actual', allow_reuse=True)(validate_data_source_for_map_config)
-    _validate_postsample_intensity = validator('postsample_intensity', allow_reuse=True)(validate_data_source_for_map_config)
-    _validate_scalar_data = validator('scalar_data', each_item=True, allow_reuse=True)(validate_data_source_for_map_config)
+
+    _validate_independent_dimensions = validator(
+        'independent_dimensions',
+        each_item=True,
+        allow_reuse=True)(validate_data_source_for_map_config)
+    _validate_presample_intensity = validator(
+        'presample_intensity',
+        allow_reuse=True)(validate_data_source_for_map_config)
+    _validate_dwell_time_actual = validator(
+        'dwell_time_actual',
+        allow_reuse=True)(validate_data_source_for_map_config)
+    _validate_postsample_intensity = validator(
+        'postsample_intensity',
+        allow_reuse=True)(validate_data_source_for_map_config)
+    _validate_scalar_data = validator(
+        'scalar_data',
+        each_item=True,
+        allow_reuse=True)(validate_data_source_for_map_config)
+
     @validator('experiment_type')
     def validate_experiment_type(cls, value, values):
-        '''Ensure values for the station and experiment_type fields are compatible'''
+        """Ensure values for the station and experiment_type fields are
+        compatible
+        """
         station = values.get('station')
         if station == 'id1a3':
             allowed_experiment_types = ['SAXSWAXS', 'EDD', 'TOMO']
         elif station == 'id3a':
             allowed_experiment_types = ['EDD', 'TOMO']
         elif station == 'id3b':
             allowed_experiment_types = ['SAXSWAXS', 'XRF', 'TOMO']
         else:
             allowed_experiment_types = []
         if value not in allowed_experiment_types:
-            raise(ValueError(f'For station {station}, allowed experiment types are {allowed_experiment_types} (suuplied experiment type {value} is not allowed)'))
-        return(value)
+            raise ValueError(
+                f'For station {station}, allowed experiment types are '
+                f'{", ".join(allowed_experiment_types)}. '
+                f'Supplied experiment type {value} is not allowed.')
+        return value
+
     @property
     def coords(self):
-        """Return a dictionary of the values of each independent dimension across
-        the map.
+        """Return a dictionary of the values of each independent
+        dimension across the map.
 
         :returns: A dictionary ofthe map's  coordinate values.
         :rtype: dict[str,list[float]]
         """
         try:
-            return(self._coords)
+            coords = self._coords
         except:
             coords = {}
             for independent_dimension in self.independent_dimensions:
                 coords[independent_dimension.label] = []
                 for scans in self.spec_scans:
                     for scan_number in scans.scan_numbers:
                         scanparser = scans.get_scanparser(scan_number)
-                        for scan_step_index in range(scanparser.spec_scan_npts):
-                            coords[independent_dimension.label].append(independent_dimension.get_value(scans, scan_number, scan_step_index))
-                coords[independent_dimension.label] = np.unique(coords[independent_dimension.label])
-            self._coords = coords
-            return(self._coords)
+                        for scan_step_index in range(
+                                scanparser.spec_scan_npts):
+                            coords[independent_dimension.label].append(
+                                independent_dimension.get_value(
+                                    scans, scan_number, scan_step_index))
+                coords[independent_dimension.label] = np.unique(
+                    coords[independent_dimension.label])
+                self._coords = coords
+        return coords
+
     @property
     def dims(self):
-        """Return a tuple of the independent dimension labels for the map."""
-        return([point_by_point_scan_data.label for point_by_point_scan_data in self.independent_dimensions[::-1]])
+        """Return a tuple of the independent dimension labels for the
+        map.
+        """
+        return [point_by_point_scan_data.label
+                for point_by_point_scan_data
+                in self.independent_dimensions[::-1]]
+
     @property
     def shape(self):
-        """Return the shape of the map -- a tuple representing the number of
-        unique values of each dimension across the map.
+        """Return the shape of the map -- a tuple representing the
+        number of unique values of each dimension across the map.
         """
-        return(tuple([len(values) for key,values in self.coords.items()][::-1]))
+        return tuple([len(values) for key,values in self.coords.items()][::-1])
+
     @property
     def all_scalar_data(self):
-        """Return a list of all instances of `PointByPointScanData` for which
-        this map configuration will collect dataset-like data (as opposed to
-        axes-like data).
-
-        This will be any and all of the items in the corrections-data-related
-        fields, as well as any additional items in the optional `scalar_data`
-        field."""
-        return([getattr(self,l,None) for l in CorrectionsData.reserved_labels() if getattr(self,l,None) is not None] + self.scalar_data)
+        """Return a list of all instances of `PointByPointScanData`
+        for which this map configuration will collect dataset-like
+        data (as opposed to axes-like data).
+
+        This will be any and all of the items in the
+        corrections-data-related fields, as well as any additional
+        items in the optional `scalar_data` field.
+        """
+        return [getattr(self, label, None)
+                for label in CorrectionsData.reserved_labels()
+                if getattr(self, label, None) is not None] + self.scalar_data
+
 
 def import_scanparser(station, experiment):
-    '''Given the name of a CHESS station and experiment type, import the
-    corresponding subclass of `ScanParser` as `ScanParser`.
+    """Given the name of a CHESS station and experiment type, import
+    the corresponding subclass of `ScanParser` as `ScanParser`.
 
     :param station: The station name ("IDxx", not the beamline acronym)
     :type station: str
     :param experiment: The experiment type
     :type experiment: Literal["SAXSWAXS","EDD","XRF","Tomo","Powder"]
     :return: None
-    '''
+    """
 
     station = station.lower()
     experiment = experiment.lower()
 
     if station in ('id1a3', 'id3a'):
         if experiment in ('saxswaxs', 'powder'):
-            from CHAP.common.utils.scanparsers import SMBLinearScanParser as ScanParser
+            from CHAP.common.utils.scanparsers \
+                import SMBLinearScanParser as ScanParser
         elif experiment == 'edd':
-            from CHAP.common.utils.scanparsers import SMBMCAScanParser as ScanParser
+            from CHAP.common.utils.scanparsers \
+                import SMBMCAScanParser as ScanParser
         elif experiment == 'tomo':
-            from CHAP.common.utils.scanparsers import SMBRotationScanParser as ScanParser
+            from CHAP.common.utils.scanparsers \
+                import SMBRotationScanParser as ScanParser
         else:
-            raise(ValueError(f'Invalid experiment type for station {station}: {experiment}'))
+            raise ValueError(
+                f'Invalid experiment type for station {station}: {experiment}')
     elif station == 'id3b':
         if experiment == 'saxswaxs':
-            from CHAP.common.utils.scanparsers import FMBSAXSWAXSScanParser as ScanParser
+            from CHAP.common.utils.scanparsers \
+                import FMBSAXSWAXSScanParser as ScanParser
         elif experiment == 'tomo':
-            from CHAP.common.utils.scanparsers import FMBRotationScanParser as ScanParser
+            from CHAP.common.utils.scanparsers \
+                import FMBRotationScanParser as ScanParser
         elif experiment == 'xrf':
-            from CHAP.common.utils.scanparsers import FMBXRFScanParser as ScanParser
+            from CHAP.common.utils.scanparsers \
+                import FMBXRFScanParser as ScanParser
         else:
-            raise(ValueError(f'Invalid experiment type for station {station}: {experiment}'))
+            raise ValueError(
+                f'Invalid experiment type for station {station}: {experiment}')
     else:
-        raise(ValueError(f'Invalid station: {station}'))
+        raise ValueError(f'Invalid station: {station}')
 
     globals()['ScanParser'] = ScanParser
```

### Comparing `ChessAnalysisPipeline-0.0.5/CHAP/common/processor.py` & `ChessAnalysisPipeline-0.0.6/CHAP/common/processor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,132 +1,137 @@
 #!/usr/bin/env python
 #-*- coding: utf-8 -*-
 #pylint: disable=
-'''
+"""
 File       : processor.py
 Author     : Valentin Kuznetsov <vkuznet AT gmail dot com>
-Description: Module for Processors used in multiple experiment-specific workflows.
-'''
+Description: Module for Processors used in multiple experiment-specific
+             workflows.
+"""
 
 # system modules
-import argparse
-import logging
-import json
-import sys
+from json import dumps
 from time import time
 
 # local modules
 from CHAP import Processor
 
+
 class AsyncProcessor(Processor):
-    '''A Processor to process multiple sets of input data via asyncio module
+    """A Processor to process multiple sets of input data via asyncio
+    module
 
     :ivar mgr: The `Processor` used to process every set of input data
     :type mgr: Processor
-    '''
+    """
     def __init__(self, mgr):
         super().__init__()
         self.mgr = mgr
 
-    def _process(self, docs):
-        '''Asynchronously process the input documents with the `self.mgr`
-        `Processor`.
-        
-        :param docs: input documents to process
+    def _process(self, data):
+        """Asynchronously process the input documents with the
+        `self.mgr` `Processor`.
+
+        :param data: input data documents to process
         :type docs: iterable
-        '''
+        """
 
         import asyncio
 
         async def task(mgr, doc):
-            '''Process given data using provided `Processor`
-        
+            """Process given data using provided `Processor`
+
             :param mgr: the object that will process given data
             :type mgr: Processor
             :param doc: the data to process
             :type doc: object
             :return: processed data
             :rtype: object
-            '''
+            """
             return mgr.process(doc)
 
-        async def executeTasks(mgr, docs):
-            '''Process given set of documents using provided task manager
-        
+        async def execute_tasks(mgr, docs):
+            """Process given set of documents using provided task
+            manager
+
             :param mgr: the object that will process all documents
             :type mgr: Processor
             :param docs: the set of data documents to process
             :type doc: iterable
-            '''
-            coRoutines = [task(mgr, d) for d in docs]
-            await asyncio.gather(*coRoutines)
+            """
+            coroutines = [task(mgr, d) for d in docs]
+            await asyncio.gather(*coroutines)
+
+        asyncio.run(execute_tasks(self.mgr, data))
 
-        asyncio.run(executeTasks(self.mgr, docs))
 
 class IntegrationProcessor(Processor):
-    '''A processor for integrating 2D data with pyFAI
-    '''
+    """A processor for integrating 2D data with pyFAI"""
 
     def _process(self, data):
-        '''Integrate the input data with the integration method and keyword
-        arguments supplied and return the results.
-                                                                                                                         
-        :param data: input data, including raw data, integration method, and
-            keyword args for the integration method.
-        :type data: tuple[typing.Union[numpy.ndarray, list[numpy.ndarray]],
-                          callable,
-                          dict]
+        """Integrate the input data with the integration method and
+        keyword arguments supplied and return the results.
+
+        :param data: input data, including raw data, integration
+            method, and keyword args for the integration method.
+        :type data: tuple[typing.Union[numpy.ndarray,
+                          list[numpy.ndarray]], callable, dict]
         :param integration_method: the method of a
             `pyFAI.azimuthalIntegrator.AzimuthalIntegrator` or
-            `pyFAI.multi_geometry.MultiGeometry` that returns the desired
-            integration results.
+            `pyFAI.multi_geometry.MultiGeometry` that returns the
+            desired integration results.
         :return: integrated raw data
         :rtype: pyFAI.containers.IntegrateResult
-        '''
-
+        """
         detector_data, integration_method, integration_kwargs = data
 
-        return(integration_method(detector_data, **integration_kwargs))
+        return integration_method(detector_data, **integration_kwargs)
+
 
 class IntegrateMapProcessor(Processor):
-    '''Class representing a process that takes a map and integration
-    configuration and returns a `nexusformat.nexus.NXprocess` containing a map of
-    the integrated detector data requested.
-    '''
+    """Class representing a process that takes a map and integration
+    configuration and returns a `nexusformat.nexus.NXprocess`
+    containing a map of the integrated detector data requested.
+    """
 
     def _process(self, data):
-        '''Process the output of a `Reader` that contains a map and integration
-        configuration and return a `nexusformat.nexus.NXprocess` containing a map
-        of the integrated detector data requested
-
-        :param data: Result of `Reader.read` where at least one item has the
-            value `'MapConfig'` for the `'schema'` key, and at least one item has
-            the value `'IntegrationConfig'` for the `'schema'` key.
+        """Process the output of a `Reader` that contains a map and
+        integration configuration and return a
+        `nexusformat.nexus.NXprocess` containing a map of the
+        integrated detector data requested
+
+        :param data: Result of `Reader.read` where at least one item
+            has the value `'MapConfig'` for the `'schema'` key, and at
+            least one item has the value `'IntegrationConfig'` for the
+            `'schema'` key.
         :type data: list[dict[str,object]]
         :return: integrated data and process metadata
         :rtype: nexusformat.nexus.NXprocess
-        '''
+        """
 
         map_config, integration_config = self.get_configs(data)
         nxprocess = self.get_nxprocess(map_config, integration_config)
 
-        return(nxprocess)
+        return nxprocess
 
     def get_configs(self, data):
-        '''Return valid instances of `MapConfig` and `IntegrationConfig` from the
-        input supplied by `MultipleReader`.
-
-        :param data: Result of `Reader.read` where at least one item has the
-            value `'MapConfig'` for the `'schema'` key, and at least one item has
-            the value `'IntegrationConfig'` for the `'schema'` key.
+        """Return valid instances of `MapConfig` and
+        `IntegrationConfig` from the input supplied by
+        `MultipleReader`.
+
+        :param data: Result of `Reader.read` where at least one item
+            has the value `'MapConfig'` for the `'schema'` key, and at
+            least one item has the value `'IntegrationConfig'` for the
+            `'schema'` key.
         :type data: list[dict[str,object]]
-        :raises ValueError: if `data` cannot be parsed into map and integration configurations.
+        :raises ValueError: if `data` cannot be parsed into map and
+            integration configurations.
         :return: valid map and integration configuration objects.
         :rtype: tuple[MapConfig, IntegrationConfig]
-        '''
+        """
 
         self.logger.debug('Getting configuration objects')
         t0 = time()
 
         from CHAP.common.models.map import MapConfig
         from CHAP.common.models.integration import IntegrationConfig
 
@@ -138,243 +143,257 @@
                     schema = item.get('schema')
                     if schema == 'MapConfig':
                         map_config = item.get('data')
                     elif schema == 'IntegrationConfig':
                         integration_config = item.get('data')
 
         if not map_config:
-            raise(ValueError('No map configuration found'))
+            raise ValueError('No map configuration found')
         if not integration_config:
-            raise(ValueError('No integration configuration found'))
+            raise ValueError('No integration configuration found')
 
         map_config = MapConfig(**map_config)
         integration_config = IntegrationConfig(**integration_config)
 
-        self.logger.debug(f'Got configuration objects in {time()-t0:.3f} seconds')
+        self.logger.debug(
+            f'Got configuration objects in {time()-t0:.3f} seconds')
 
-        return(map_config, integration_config)
+        return map_config, integration_config
 
     def get_nxprocess(self, map_config, integration_config):
-        '''Use a `MapConfig` and `IntegrationConfig` to construct a
+        """Use a `MapConfig` and `IntegrationConfig` to construct a
         `nexusformat.nexus.NXprocess`
 
         :param map_config: a valid map configuration
         :type map_config: MapConfig
         :param integration_config: a valid integration configuration
         :type integration_config: IntegrationConfig
-        :return: the integrated detector data and metadata contained in a NeXus
-            structure
+        :return: the integrated detector data and metadata contained
+            in a NeXus structure
         :rtype: nexusformat.nexus.NXprocess
-        '''
+        """
 
         self.logger.debug('Constructing NXprocess')
         t0 = time()
 
         from nexusformat.nexus import (NXdata,
                                        NXdetector,
                                        NXfield,
                                        NXprocess)
         import numpy as np
         import pyFAI
 
         nxprocess = NXprocess(name=integration_config.title)
 
-        nxprocess.map_config = json.dumps(map_config.dict())
-        nxprocess.integration_config = json.dumps(integration_config.dict())
+        nxprocess.map_config = dumps(map_config.dict())
+        nxprocess.integration_config = dumps(integration_config.dict())
 
         nxprocess.program = 'pyFAI'
         nxprocess.version = pyFAI.version
 
-        for k,v in integration_config.dict().items():
+        for k, v in integration_config.dict().items():
             if k == 'detectors':
                 continue
             nxprocess.attrs[k] = v
 
         for detector in integration_config.detectors:
             nxprocess[detector.prefix] = NXdetector()
             nxdetector = nxprocess[detector.prefix]
             nxdetector.local_name = detector.prefix
             nxdetector.distance = detector.azimuthal_integrator.dist
             nxdetector.distance.attrs['units'] = 'm'
-            nxdetector.calibration_wavelength = detector.azimuthal_integrator.wavelength
+            nxdetector.calibration_wavelength = \
+                detector.azimuthal_integrator.wavelength
             nxdetector.calibration_wavelength.attrs['units'] = 'm'
             nxdetector.attrs['poni_file'] = str(detector.poni_file)
             nxdetector.attrs['mask_file'] = str(detector.mask_file)
-            nxdetector.raw_data_files = np.full(map_config.shape, '', dtype='|S256')
+            nxdetector.raw_data_files = np.full(map_config.shape,
+                                                '', dtype='|S256')
 
         nxprocess.data = NXdata()
 
         nxprocess.data.attrs['axes'] = (
             *map_config.dims,
             *integration_config.integrated_data_dims
         )
-        for i,dim in enumerate(map_config.independent_dimensions[::-1]):
+        for i, dim in enumerate(map_config.independent_dimensions[::-1]):
             nxprocess.data[dim.label] = NXfield(
                 value=map_config.coords[dim.label],
                 units=dim.units,
                 attrs={'long_name': f'{dim.label} ({dim.units})',
                        'data_type': dim.data_type,
                        'local_name': dim.name})
             nxprocess.data.attrs[f'{dim.label}_indices'] = i
 
-        for i,(coord_name,coord_values) in \
-            enumerate(integration_config.integrated_data_coordinates.items()):
+        for i, (coord_name, coord_values) in enumerate(
+                integration_config.integrated_data_coordinates.items()):
             if coord_name == 'radial':
                 type_ = pyFAI.units.RADIAL_UNITS
             elif coord_name == 'azimuthal':
                 type_ = pyFAI.units.AZIMUTHAL_UNITS
             coord_units = pyFAI.units.to_unit(
                 getattr(integration_config, f'{coord_name}_units'),
                 type_=type_)
             nxprocess.data[coord_units.name] = coord_values
-            nxprocess.data.attrs[f'{coord_units.name}_indices'] = i+len(map_config.coords)
+            nxprocess.data.attrs[f'{coord_units.name}_indices'] = i + len(
+                map_config.coords)
             nxprocess.data[coord_units.name].units = coord_units.unit_symbol
-            nxprocess.data[coord_units.name].attrs['long_name'] = coord_units.label
+            nxprocess.data[coord_units.name].attrs['long_name'] = \
+                coord_units.label
 
         nxprocess.data.attrs['signal'] = 'I'
         nxprocess.data.I = NXfield(
             value=np.empty(
                 (*tuple(
-                    [len(coord_values) for coord_name,coord_values in map_config.coords.items()][::-1]
-                  ),
-                 *integration_config.integrated_data_shape
-                )
-            ),
+                    [len(coord_values) for coord_name, coord_values
+                     in map_config.coords.items()][::-1]),
+                 *integration_config.integrated_data_shape)),
             units='a.u',
             attrs={'long_name':'Intensity (a.u)'})
 
         integrator = integration_config.get_multi_geometry_integrator()
         if integration_config.integration_type == 'azimuthal':
             integration_method = integrator.integrate1d
             integration_kwargs = {
-                'lst_mask': [detector.mask_array for detector in integration_config.detectors],
+                'lst_mask': [detector.mask_array
+                             for detector
+                             in integration_config.detectors],
                 'npt': integration_config.radial_npt
             }
         elif integration_config.integration_type == 'cake':
             integration_method = integrator.integrate2d
             integration_kwargs = {
-                'lst_mask': [detector.mask_array for detector in integration_config.detectors],
+                'lst_mask': [detector.mask_array
+                             for detector
+                             in integration_config.detectors],
                 'npt_rad': integration_config.radial_npt,
                 'npt_azim': integration_config.azimuthal_npt,
                 'method': 'bbox'
             }
 
         integration_processor = IntegrationProcessor()
         integration_processor.logger.setLevel(self.logger.getEffectiveLevel())
         integration_processor.logger.addHandler(self.logger.handlers[0])
-        lst_args = []
         for scans in map_config.spec_scans:
             for scan_number in scans.scan_numbers:
                 scanparser = scans.get_scanparser(scan_number)
                 for scan_step_index in range(scanparser.spec_scan_npts):
                     map_index = scans.get_index(
                         scan_number,
                         scan_step_index,
                         map_config)
                     detector_data = scans.get_detector_data(
                         integration_config.detectors,
                         scan_number,
                         scan_step_index)
                     result = integration_processor.process(
-                        (detector_data, integration_method, integration_kwargs))
+                        (detector_data,
+                         integration_method, integration_kwargs))
                     nxprocess.data.I[map_index] = result.intensity
 
                     for detector in integration_config.detectors:
-                        nxprocess[detector.prefix].raw_data_files[map_index] = \
+                        nxprocess[detector.prefix].raw_data_files[map_index] =\
                             scanparser.get_detector_data_file(
-                                detector.prefix,
-                                scan_step_index)
+                                detector.prefix, scan_step_index)
 
         self.logger.debug(f'Constructed NXprocess in {time()-t0:.3f} seconds')
 
-        return(nxprocess)
+        return nxprocess
+
 
 class MapProcessor(Processor):
-    '''A Processor to take a map configuration and return a
-    `nexusformat.nexus.NXentry` representing that map's metadata and any
-    scalar-valued raw data requseted by the supplied map configuration.
-    '''
+    """A Processor to take a map configuration and return a
+    `nexusformat.nexus.NXentry` representing that map's metadata and
+    any scalar-valued raw data requseted by the supplied map
+    configuration.
+    """
 
     def _process(self, data):
-        '''Process the output of a `Reader` that contains a map configuration and
-        return a `nexusformat.nexus.NXentry` representing the map.
+        """Process the output of a `Reader` that contains a map
+        configuration and return a `nexusformat.nexus.NXentry`
+        representing the map.
 
-        :param data: Result of `Reader.read` where at least one item has the
-            value `'MapConfig'` for the `'schema'` key.
+        :param data: Result of `Reader.read` where at least one item
+            has the value `'MapConfig'` for the `'schema'` key.
         :type data: list[dict[str,object]]
         :return: Map data & metadata
         :rtype: nexusformat.nexus.NXentry
-        '''
+        """
 
         map_config = self.get_map_config(data)
         nxentry = self.__class__.get_nxentry(map_config)
 
-        return(nxentry)
+        return nxentry
 
     def get_map_config(self, data):
-        '''Get an instance of `MapConfig` from a returned value of `Reader.read`
+        """Get an instance of `MapConfig` from a returned value of
+        `Reader.read`
 
-        :param data: Result of `Reader.read` where at least one item has the
-            value `'MapConfig'` for the `'schema'` key.
+        :param data: Result of `Reader.read` where at least one item
+            has the value `'MapConfig'` for the `'schema'` key.
         :type data: list[dict[str,object]]
-        :raises Exception: If a valid `MapConfig` cannot be constructed from `data`.
-        :return: a valid instance of `MapConfig` with field values taken from `data`.
+        :raises Exception: If a valid `MapConfig` cannot be
+            constructed from `data`.
+        :return: a valid instance of `MapConfig` with field values
+            taken from `data`.
         :rtype: MapConfig
-        '''
+        """
 
-        from .models.map import MapConfig
+        from CHAP.common.models.map import MapConfig
 
         map_config = False
         if isinstance(data, list):
             for item in data:
                 if isinstance(item, dict):
                     if item.get('schema') == 'MapConfig':
                         map_config = item.get('data')
                         break
 
         if not map_config:
-            raise(ValueError('No map configuration found'))
+            raise ValueError('No map configuration found')
 
-        return(MapConfig(**map_config))
+        return MapConfig(**map_config)
 
     @staticmethod
     def get_nxentry(map_config):
-        '''Use a `MapConfig` to construct a `nexusformat.nexus.NXentry`
+        """Use a `MapConfig` to construct a
+        `nexusformat.nexus.NXentry`
 
         :param map_config: a valid map configuration
         :type map_config: MapConfig
-        :return: the map's data and metadata contained in a NeXus structure
+        :return: the map's data and metadata contained in a NeXus
+            structure
         :rtype: nexusformat.nexus.NXentry
-        '''
+        """
 
         from nexusformat.nexus import (NXcollection,
                                        NXdata,
                                        NXentry,
                                        NXfield,
                                        NXsample)
         import numpy as np
 
         nxentry = NXentry(name=map_config.title)
 
-        nxentry.map_config = json.dumps(map_config.dict())
+        nxentry.map_config = dumps(map_config.dict())
 
         nxentry[map_config.sample.name] = NXsample(**map_config.sample.dict())
 
         nxentry.attrs['station'] = map_config.station
 
         nxentry.spec_scans = NXcollection()
         for scans in map_config.spec_scans:
             nxentry.spec_scans[scans.scanparsers[0].scan_name] = \
                 NXfield(value=scans.scan_numbers,
                         dtype='int8',
-                        attrs={'spec_file':str(scans.spec_file)})
+                        attrs={'spec_file': str(scans.spec_file)})
 
         nxentry.data = NXdata()
         nxentry.data.attrs['axes'] = map_config.dims
-        for i,dim in enumerate(map_config.independent_dimensions[::-1]):
+        for i, dim in enumerate(map_config.independent_dimensions[::-1]):
             nxentry.data[dim.label] = NXfield(
                 value=map_config.coords[dim.label],
                 units=dim.units,
                 attrs={'long_name': f'{dim.label} ({dim.units})',
                        'data_type': dim.data_type,
                        'local_name': dim.name})
             nxentry.data.attrs[f'{dim.label}_indices'] = i
@@ -407,238 +426,257 @@
                         map_config)
                     for data in map_config.all_scalar_data:
                         nxentry.data[data.label][map_index] = data.get_value(
                             scans,
                             scan_number,
                             scan_step_index)
 
-        return(nxentry)
+        return nxentry
+
 
 class NexusToNumpyProcessor(Processor):
-    '''A Processor to convert the default plottable data in an `NXobject` into
-    an `numpy.ndarray`.
-    '''
+    """A Processor to convert the default plottable data in an
+    `NXobject` into an `numpy.ndarray`.
+    """
 
     def _process(self, data):
-        '''Return the default plottable data signal in `data` as an
+        """Return the default plottable data signal in `data` as an
         `numpy.ndarray`.
-                                                                                    
+
         :param data: input NeXus structure
         :type data: nexusformat.nexus.tree.NXobject
-        :raises ValueError: if `data` has no default plottable data signal
+        :raises ValueError: if `data` has no default plottable data
+            signal
         :return: default plottable data signal in `data`
         :rtype: numpy.ndarray
-        '''
+        """
 
         default_data = data.plottable_data
 
         if default_data is None:
             default_data_path = data.attrs['default']
             default_data = data.get(default_data_path)
         if default_data is None:
-            raise(ValueError(f'The structure of {data} contains no default data'))
+            raise ValueError(
+                f'The structure of {data} contains no default data')
 
         default_signal = default_data.attrs.get('signal')
         if default_signal is None:
-            raise(ValueError(f'The signal of {default_data} is unknown'))
+            raise ValueError(f'The signal of {default_data} is unknown')
         default_signal = default_signal.nxdata
 
         np_data = default_data[default_signal].nxdata
 
-        return(np_data)
+        return np_data
+
 
 class NexusToXarrayProcessor(Processor):
-    '''A Processor to convert the default plottable data in an `NXobject` into
-    an `xarray.DataArray`.'''
+    """A Processor to convert the default plottable data in an
+    `NXobject` into an `xarray.DataArray`.
+    """
 
     def _process(self, data):
-        '''Return the default plottable data signal in `data` as an
+        """Return the default plottable data signal in `data` as an
         `xarray.DataArray`.
-                                                                                    
+
         :param data: input NeXus structure
         :type data: nexusformat.nexus.tree.NXobject
-        :raises ValueError: if metadata for `xarray` is absent from `data`
+        :raises ValueError: if metadata for `xarray` is absent from
+            `data`
         :return: default plottable data signal in `data`
         :rtype: xarray.DataArray
-        '''
+        """
 
         from xarray import DataArray
 
         default_data = data.plottable_data
 
         if default_data is None:
             default_data_path = data.attrs['default']
             default_data = data.get(default_data_path)
         if default_data is None:
-            raise(ValueError(f'The structure of {data} contains no default data'))
+            raise ValueError(
+                f'The structure of {data} contains no default data')
 
         default_signal = default_data.attrs.get('signal')
         if default_signal is None:
-            raise(ValueError(f'The signal of {default_data} is unknown'))
+            raise ValueError(f'The signal of {default_data} is unknown')
         default_signal = default_signal.nxdata
 
         signal_data = default_data[default_signal].nxdata
 
         axes = default_data.attrs['axes']
         coords = {}
         for axis_name in axes:
             axis = default_data[axis_name]
             coords[axis_name] = (axis_name,
                                  axis.nxdata,
                                  axis.attrs)
 
         dims = tuple(axes)
-
         name = default_signal
-
         attrs = default_data[default_signal].attrs
 
-        return(DataArray(data=signal_data,
+        return DataArray(data=signal_data,
                          coords=coords,
                          dims=dims,
                          name=name,
-                         attrs=attrs))
+                         attrs=attrs)
+
 
 class PrintProcessor(Processor):
-    '''A Processor to simply print the input data to stdout and return the
-    original input data, unchanged in any way.
-    '''
+    """A Processor to simply print the input data to stdout and return
+    the original input data, unchanged in any way.
+    """
 
     def _process(self, data):
-        '''Print and return the input data.
+        """Print and return the input data.
 
         :param data: Input data
         :type data: object
         :return: `data`
         :rtype: object
-        '''
+        """
 
         print(f'{self.__name__} data :')
 
         if callable(getattr(data, '_str_tree', None)):
-            # If data is likely an NXobject, print its tree representation
-            # (since NXobjects' str representations are just their nxname)
+            # If data is likely an NXobject, print its tree
+            # representation (since NXobjects' str representations are
+            # just their nxname)
             print(data._str_tree(attrs=True, recursive=True))
         else:
             print(str(data))
 
-        return(data)
+        return data
+
 
 class StrainAnalysisProcessor(Processor):
-    '''A Processor to compute a map of sample strains by fitting bragg peaks in
-    1D detector data and analyzing the difference between measured peak
-    locations and expected peak locations for the sample measured.
-    '''
+    """A Processor to compute a map of sample strains by fitting bragg
+    peaks in 1D detector data and analyzing the difference between
+    measured peak locations and expected peak locations for the sample
+    measured.
+    """
 
     def _process(self, data):
-        '''Process the input map detector data & configuration for the strain
-        analysis procedure, and return a map of sample strains.
+        """Process the input map detector data & configuration for the
+        strain analysis procedure, and return a map of sample strains.
 
-        :param data: results of `MutlipleReader.read` containing input map
-            detector data and strain analysis configuration
+        :param data: results of `MutlipleReader.read` containing input
+            map detector data and strain analysis configuration
         :type data: dict[list[str,object]]
         :return: map of sample strains
         :rtype: xarray.Dataset
-        '''
+        """
 
         strain_analysis_config = self.get_config(data)
 
-        return(data)
+        return data
 
     def get_config(self, data):
-        '''Get instances of the configuration objects needed by this
+        """Get instances of the configuration objects needed by this
         `Processor` from a returned value of `Reader.read`
 
-        :param data: Result of `Reader.read` where at least one item has the
-            value `'StrainAnalysisConfig'` for the `'schema'` key.
+        :param data: Result of `Reader.read` where at least one item
+            has the value `'StrainAnalysisConfig'` for the `'schema'`
+            key.
         :type data: list[dict[str,object]]
-        :raises Exception: If valid config objects cannot be constructed from `data`.
-        :return: valid instances of the configuration objects with field values
-            taken from `data`.
+        :raises Exception: If valid config objects cannot be
+            constructed from `data`.
+        :return: valid instances of the configuration objects with
+            field values taken from `data`.
         :rtype: StrainAnalysisConfig
-        '''
+        """
 
         strain_analysis_config = False
         if isinstance(data, list):
             for item in data:
                 if isinstance(item, dict):
-                    schema = item.get('schema')
                     if item.get('schema') == 'StrainAnalysisConfig':
                         strain_analysis_config = item.get('data')
 
         if not strain_analysis_config:
-            raise(ValueError('No strain analysis configuration found in input data'))
+            raise ValueError(
+                'No strain analysis configuration found in input data')
 
-        return(strain_analysis_config)
+        return strain_analysis_config
 
 
 class URLResponseProcessor(Processor):
-    '''A Processor to decode and return data resulting from from URLReader.read'''
+    """A Processor to decode and return data resulting from from
+    URLReader.read
+    """
+
     def _process(self, data):
-        '''Take data returned from URLReader.read and return a decoded version
-        of the content.
+        """Take data returned from URLReader.read and return a decoded
+        version of the content.
 
         :param data: input data (output of URLReader.read)
         :type data: list[dict]
         :return: decoded data contents
         :rtype: object
-        '''
+        """
 
         data = data[0]
 
         content = data['data']
         encoding = data['encoding']
 
-        self.logger.debug(f'Decoding content of type {type(content)} with {encoding}')
+        self.logger.debug(
+            f'Decoding content of type {type(content)} with {encoding}')
 
         try:
             content = content.decode(encoding)
         except:
-            self.logger.warning(f'Failed to decode content of type {type(content)} with {encoding}')
+            self.logger.warning('Failed to decode content of type '
+                                f'{type(content)} with {encoding}')
+
+        return content
 
-        return(content)
 
 class XarrayToNexusProcessor(Processor):
-    '''A Processor to convert the data in an `xarray` structure to an
+    """A Processor to convert the data in an `xarray` structure to an
     `nexusformat.nexus.NXdata`.
-    '''
+    """
 
     def _process(self, data):
-        '''Return `data` represented as an `nexusformat.nexus.NXdata`.
+        """Return `data` represented as an `nexusformat.nexus.NXdata`.
 
         :param data: The input `xarray` structure
         :type data: typing.Union[xarray.DataArray, xarray.Dataset]
         :return: The data and metadata in `data`
         :rtype: nexusformat.nexus.NXdata
-        '''
+        """
 
         from nexusformat.nexus import NXdata, NXfield
 
         signal = NXfield(value=data.data, name=data.name, attrs=data.attrs)
 
         axes = []
         for name, coord in data.coords.items():
-            axes.append(NXfield(value=coord.data, name=name, attrs=coord.attrs))
+            axes.append(
+                NXfield(value=coord.data, name=name, attrs=coord.attrs))
         axes = tuple(axes)
 
-        return(NXdata(signal=signal, axes=axes))
+        return NXdata(signal=signal, axes=axes)
+
 
 class XarrayToNumpyProcessor(Processor):
-    '''A Processor to convert the data in an `xarray.DataArray` structure to an
-    `numpy.ndarray`.
-    '''
+    """A Processor to convert the data in an `xarray.DataArray`
+    structure to an `numpy.ndarray`.
+    """
 
     def _process(self, data):
-        '''Return just the signal values contained in `data`.
-                                                                                    
+        """Return just the signal values contained in `data`.
+
         :param data: The input `xarray.DataArray`
         :type data: xarray.DataArray
         :return: The data in `data`
         :rtype: numpy.ndarray
-        '''
+        """
+
+        return data.data
 
-        return(data.data)
 
 if __name__ == '__main__':
     from CHAP.processor import main
     main()
-
```

### Comparing `ChessAnalysisPipeline-0.0.5/CHAP/common/reader.py` & `ChessAnalysisPipeline-0.0.6/CHAP/common/reader.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,119 +1,132 @@
 #!/usr/bin/env python
-'''
+"""
 File       : reader.py
 Author     : Valentin Kuznetsov <vkuznet AT gmail dot com>
-Description: Module for Writers used in multiple experiment-specific workflows.
-'''
+Description: Module for Writers used in multiple experiment-specific
+             workflows.
+"""
 
 # system modules
-import argparse
-import json
-import logging
-import sys
+from sys import modules
 from time import time
 
 # local modules
 from CHAP import Reader
 
+
 class BinaryFileReader(Reader):
+    """Reader for binary files"""
     def _read(self, filename):
-        '''Return a content of a given file name
+        """Return a content of a given file name
 
         :param filename: name of the binart file to read from
         :return: the content of `filename`
         :rtype: binary
-        '''
+        """
+
         with open(filename, 'rb') as file:
             data = file.read()
-        return(data)
+        return data
+
 
 class MultipleReader(Reader):
-    def read(self, readers):
-        '''Return resuts from multiple `Reader`s.
+    def read(self, readers, **_read_kwargs):
+        """Return resuts from multiple `Reader`s.
 
-        :param readers: a dictionary where the keys are specific names that are
-            used by the next item in the `Pipeline`, and the values are `Reader`
-            configurations.
+        :param readers: a dictionary where the keys are specific names
+            that are used by the next item in the `Pipeline`, and the
+            values are `Reader` configurations.
         :type readers: list[dict]
-        :return: The results of calling `Reader.read(**kwargs)` for each item
-            configured in `readers`.
+        :return: The results of calling `Reader.read(**kwargs)` for
+            each item configured in `readers`.
         :rtype: list[dict[str,object]]
-        '''
+        """
 
         t0 = time()
         self.logger.info(f'Executing "read" with {len(readers)} Readers')
 
         data = []
         for reader_config in readers:
             reader_name = list(reader_config.keys())[0]
-            reader_class = getattr(sys.modules[__name__], reader_name)
+            reader_class = getattr(modules[__name__], reader_name)
             reader = reader_class()
             reader_kwargs = reader_config[reader_name]
 
-            data.extend(reader.read(**reader_kwargs))
+            # Combine keyword arguments to MultipleReader.read with those to the reader
+            # giving precedence to those in the latter
+            combined_kwargs = {**_read_kwargs, **reader_kwargs}
+            data.extend(reader.read(**combined_kwargs))
 
         self.logger.info(f'Finished "read" in {time()-t0:.3f} seconds\n')
 
-        return(data)
+        return data
+
 
 class NexusReader(Reader):
+    """Reader for NeXus files"""
     def _read(self, filename, nxpath='/'):
-        '''Return the NeXus object stored at `nxpath` in the nexus file
-        `filename`.
+        """Return the NeXus object stored at `nxpath` in the nexus
+        file `filename`.
 
         :param filename: name of the NeXus file to read from
         :type filename: str
-        :param nxpath: path to a specific loaction in the NeXus file to read
-            from, defaults to `'/'`
+        :param nxpath: path to a specific loaction in the NeXus file
+            to read from, defaults to `'/'`
         :type nxpath: str, optional
-        :raises nexusformat.nexus.NeXusError: if `filename` is not a NeXus
-            file or `nxpath` is not in `filename`.
+        :raises nexusformat.nexus.NeXusError: if `filename` is not a
+            NeXus file or `nxpath` is not in `filename`.
         :return: the NeXus structure indicated by `filename` and `nxpath`.
         :rtype: nexusformat.nexus.NXobject
-        '''
+        """
 
         from nexusformat.nexus import nxload
 
         nxobject = nxload(filename)[nxpath]
-        return(nxobject)
+        return nxobject
+
 
 class URLReader(Reader):
-    def _read(self, url, headers={}):
-        '''Make an HTTPS request to the provided URL and return the results.
-        Headers for the request are optional.
+    """Reader for data available over HTTPS"""
+    def _read(self, url, headers={}, timeout=10):
+        """Make an HTTPS request to the provided URL and return the
+        results.  Headers for the request are optional.
 
         :param url: the URL to read
         :type url: str
-        :param headers: headers to attach to the request, defaults to `{}`
+        :param headers: headers to attach to the request, defaults to
+            `{}`
         :type headers: dict, optional
         :return: the content of the response
         :rtype: object
-        '''
+        """
 
         import requests
 
-        resp = requests.get(url, headers=headers)
+        resp = requests.get(url, headers=headers, timeout=timeout)
         data = resp.content
 
         self.logger.debug(f'Response content: {data}')
 
-        return(data)
+        return data
+
 
 class YAMLReader(Reader):
+    """Reader for YAML files"""
     def _read(self, filename):
-        '''Return a dictionary from the contents of a yaml file.
+        """Return a dictionary from the contents of a yaml file.
 
         :param filename: name of the YAML file to read from
         :return: the contents of `filename`
         :rtype: dict
-        '''
+        """
 
         import yaml
 
         with open(filename) as file:
             data = yaml.safe_load(file)
-        return(data)
+        return data
+
 
 if __name__ == '__main__':
     from CHAP.reader import main
     main()
```

### Comparing `ChessAnalysisPipeline-0.0.5/CHAP/common/utils/fit.py` & `ChessAnalysisPipeline-0.0.6/CHAP/common/utils/fit.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,87 +1,111 @@
-#!/usr/bin/env python3
-
-# -*- coding: utf-8 -*-
+#!/usr/bin/env python
+#-*- coding: utf-8 -*-
+#pylint: disable=
 """
-Created on Mon Dec  6 15:36:22 2021
-
-@author: rv43
+File       : fit.py
+Author     : Rolf Verberg <rolfverberg AT gmail dot com>
+Description: General curve fitting module
 """
 
-import logging
-
-try:
-    from asteval import Interpreter, get_ast_names
-except:
-    pass
+# System modules
 from copy import deepcopy
+from logging import getLogger
+from os import (
+    cpu_count,
+    mkdir,
+    path,
+)
+from re import compile as re_compile
+from re import sub
+from shutil import rmtree
+from sys import float_info
+
+# Third party modules
 try:
-    from lmfit import Model, Parameters
-    from lmfit.model import ModelResult
-    from lmfit.models import ConstantModel, LinearModel, QuadraticModel, PolynomialModel,\
-            ExponentialModel, StepModel, RectangleModel, ExpressionModel, GaussianModel,\
-            LorentzianModel
-except:
-    pass
+    from joblib import (
+        Parallel,
+        delayed,
+    )
+    HAVE_JOBLIB = True
+except ImportError:
+    HAVE_JOBLIB = False
+from lmfit import (
+    Parameters,
+    Model,
+)
+from lmfit.model import ModelResult
+from lmfit.models import (
+    ConstantModel,
+    LinearModel,
+    QuadraticModel,
+    PolynomialModel,
+    ExponentialModel,
+    StepModel,
+    RectangleModel,
+    ExpressionModel,
+    GaussianModel,
+    LorentzianModel,
+)
 import numpy as np
-from os import cpu_count, getpid, listdir, mkdir, path
-from re import compile, sub
-from shutil import rmtree
 try:
-    from sympy import diff, simplify
-except:
+    from sympy import (
+        diff,
+        simplify,
+    )
+except ImportError:
     pass
 try:
-    from joblib import Parallel, delayed
-    have_joblib = True
-except:
-    have_joblib = False
-try:
     import xarray as xr
-    have_xarray = True
-except:
-    have_xarray = False
-
-try:
-    from .general import illegal_value, is_int, is_dict_series, is_index, index_nearest, \
-            almost_equal, quick_plot #, eval_expr
-except:
-    try:
-        from sys import path as syspath
-        syspath.append(f'/nfs/chess/user/rv43/msnctools/msnctools')
-        from general import illegal_value, is_int, is_dict_series, is_index, index_nearest, \
-                almost_equal, quick_plot #, eval_expr
-    except:
-        from general import illegal_value, is_int, is_dict_series, is_index, index_nearest, \
-                almost_equal, quick_plot #, eval_expr
-
-from sys import float_info
-float_min = float_info.min
-float_max = float_info.max
+    HAVE_XARRAY = True
+except ImportError:
+    HAVE_XARRAY = False
+
+# Local modules
+from CHAP.common.utils.general import (
+    is_int,
+    is_num,
+    is_dict_series,
+    is_index,
+    index_nearest,
+    input_num,
+    quick_plot,
+)
+#    eval_expr,
+
+logger = getLogger(__name__)
+FLOAT_MIN = float_info.min
+FLOAT_MAX = float_info.max
 
 # sigma = fwhm_factor*fwhm
 fwhm_factor = {
-    'gaussian': f'fwhm/(2*sqrt(2*log(2)))',
-    'lorentzian': f'0.5*fwhm',
-    'splitlorentzian': f'0.5*fwhm', # sigma = sigma_r
-    'voight': f'0.2776*fwhm', # sigma = gamma
-    'pseudovoight': f'0.5*fwhm'} # fraction = 0.5
+    'gaussian': 'fwhm/(2*sqrt(2*log(2)))',
+    'lorentzian': '0.5*fwhm',
+    'splitlorentzian': '0.5*fwhm',  # sigma = sigma_r
+    'voight': '0.2776*fwhm',        # sigma = gamma
+    'pseudovoight': '0.5*fwhm',     # fraction = 0.5
+}
 
 # amplitude = height_factor*height*fwhm
 height_factor = {
-    'gaussian': f'height*fwhm*0.5*sqrt(pi/log(2))',
-    'lorentzian': f'height*fwhm*0.5*pi',
-    'splitlorentzian': f'height*fwhm*0.5*pi', # sigma = sigma_r
-    'voight': f'3.334*height*fwhm', # sigma = gamma
-    'pseudovoight': f'1.268*height*fwhm'} # fraction = 0.5
+    'gaussian': 'height*fwhm*0.5*sqrt(pi/log(2))',
+    'lorentzian': 'height*fwhm*0.5*pi',
+    'splitlorentzian': 'height*fwhm*0.5*pi',  # sigma = sigma_r
+    'voight': '3.334*height*fwhm',            # sigma = gamma
+    'pseudovoight': '1.268*height*fwhm',      # fraction = 0.5
+}
+
 
 class Fit:
-    """Wrapper class for lmfit
+    """
+    Wrapper class for lmfit.
     """
     def __init__(self, y, x=None, models=None, normalize=True, **kwargs):
+        """Initialize Fit."""
+        # Third party modules
         if not isinstance(normalize, bool):
             raise ValueError(f'Invalid parameter normalize ({normalize})')
         self._mask = None
         self._model = None
         self._norm = None
         self._normalized = False
         self._parameters = Parameters()
@@ -91,48 +115,54 @@
         self._nonlinear_parameters = []
         self._result = None
         self._try_linear_fit = True
         self._y = None
         self._y_norm = None
         self._y_range = None
         if 'try_linear_fit' in kwargs:
-            try_linear_fit = kwargs.pop('try_linear_fit')
-            if not isinstance(try_linear_fit, bool):
-                illegal_value(try_linear_fit, 'try_linear_fit', 'Fit.fit', raise_error=True)
-            self._try_linear_fit = try_linear_fit
+            self._try_linear_fit = kwargs.pop('try_linear_fit')
+            if not isinstance(self._try_linear_fit, bool):
+                raise ValueError(
+                    'Invalid value of keyword argument try_linear_fit '
+                    f'({self._try_linear_fit})')
         if y is not None:
             if isinstance(y, (tuple, list, np.ndarray)):
                 self._x = np.asarray(x)
                 self._y = np.asarray(y)
-            elif have_xarray and isinstance(y, xr.DataArray):
+            elif HAVE_XARRAY and isinstance(y, xr.DataArray):
                 if x is not None:
-                    logging.warning('Ignoring superfluous input x ({x}) in Fit.__init__')
+                    logger.warning('Ignoring superfluous input x ({x})')
                 if y.ndim != 1:
-                    illegal_value(y.ndim, 'DataArray dimensions', 'Fit:__init__', raise_error=True)
+                    raise ValueError(
+                        'Invalid DataArray dimensions for parameter y '
+                        f'({y.ndim})')
                 self._x = np.asarray(y[y.dims[0]])
                 self._y = y
             else:
-                illegal_value(y, 'y', 'Fit:__init__', raise_error=True)
+                raise ValueError(f'Invalid parameter y ({y})')
             if self._x.ndim != 1:
-                raise ValueError(f'Invalid dimension for input x ({self._x.ndim})')
+                raise ValueError(
+                    f'Invalid dimension for input x ({self._x.ndim})')
             if self._x.size != self._y.size:
-                raise ValueError(f'Inconsistent x and y dimensions ({self._x.size} vs '+
-                        f'{self._y.size})')
+                raise ValueError(
+                    f'Inconsistent x and y dimensions ({self._x.size} vs '
+                    f'{self._y.size})')
             if 'mask' in kwargs:
                 self._mask = kwargs.pop('mask')
             if self._mask is None:
                 y_min = float(self._y.min())
                 self._y_range = float(self._y.max())-y_min
                 if normalize and self._y_range > 0.0:
                     self._norm = (y_min, self._y_range)
             else:
                 self._mask = np.asarray(self._mask).astype(bool)
                 if self._x.size != self._mask.size:
-                    raise ValueError(f'Inconsistent x and mask dimensions ({self._x.size} vs '+
-                            f'{self._mask.size})')
+                    raise ValueError(
+                        f'Inconsistent x and mask dimensions ({self._x.size} '
+                        f'vs {self._mask.size})')
                 y_masked = np.asarray(self._y)[~self._mask]
                 y_min = float(y_masked.min())
                 self._y_range = float(y_masked.max())-y_min
                 if normalize and self._y_range > 0.0:
                     if normalize and self._y_range > 0.0:
                         self._norm = (y_min, self._y_range)
         if models is not None:
@@ -141,815 +171,899 @@
             elif isinstance(models, (tuple, list)):
                 for model in models:
                     kwargs = self.add_model(model, **kwargs)
             self.fit(**kwargs)
 
     @classmethod
     def fit_data(cls, y, models, x=None, normalize=True, **kwargs):
-        return(cls(y, x=x, models=models, normalize=normalize, **kwargs))
+        """Class method for Fit."""
+        return cls(y, x=x, models=models, normalize=normalize, **kwargs)
 
     @property
     def best_errors(self):
+        """Return errors in the best fit parameters."""
         if self._result is None:
-            return(None)
-        return({name:self._result.params[name].stderr for name in sorted(self._result.params)
-                if name != 'tmp_normalization_offset_c'})
+            return None
+        return {name:self._result.params[name].stderr
+                for name in sorted(self._result.params)
+                if name != 'tmp_normalization_offset_c'}
 
     @property
     def best_fit(self):
+        """Return the best fit."""
         if self._result is None:
-            return(None)
-        return(self._result.best_fit)
+            return None
+        return self._result.best_fit
 
-    @property
     def best_parameters(self):
+        """Return the best fit parameters."""
         if self._result is None:
-            return(None)
+            return None
         parameters = {}
         for name in sorted(self._result.params):
             if name != 'tmp_normalization_offset_c':
                 par = self._result.params[name]
-                parameters[name] = {'value': par.value, 'error': par.stderr,
-                        'init_value': par.init_value, 'min': par.min, 'max': par.max,
-                        'vary': par.vary, 'expr': par.expr}
-        return(parameters)
+                parameters[name] = {
+                    'value': par.value,
+                    'error': par.stderr,
+                    'init_value': par.init_value,
+                    'min': par.min,
+                    'max': par.max,
+                    'vary': par.vary, 'expr': par.expr
+                }
+        return parameters
 
     @property
     def best_results(self):
-        """Convert the input data array to a data set and add the fit results.
+        """
+        Convert the input DataArray to a data set and add the fit
+        results.
         """
         if self._result is None:
-            return(None)
-        if not have_xarray:
-            logging.warning('fit.best_results requires xarray in the conda environment')
-            return(None)
+            return None
+        if not HAVE_XARRAY:
+            logger.warning(
+                'fit.best_results requires xarray in the conda environment')
+            return None
         if isinstance(self._y, xr.DataArray):
             best_results = self._y.to_dataset()
             dims = self._y.dims
             fit_name = f'{self._y.name}_fit'
         else:
             coords = {'x': (['x'], self._x)}
-            dims = ('x')
+            dims = ('x',)
             best_results = xr.Dataset(coords=coords)
             best_results['y'] = (dims, self._y)
             fit_name = 'y_fit'
         best_results[fit_name] = (dims, self.best_fit)
         if self._mask is not None:
             best_results['mask'] = self._mask
-        best_results.coords['par_names'] = ('peak', [name for name in self.best_values.keys()])
-        best_results['best_values'] = (['par_names'], [v for v in self.best_values.values()])
-        best_results['best_errors'] = (['par_names'], [v for v in self.best_errors.values()])
+        best_results.coords['par_names'] = ('peak', self.best_values.keys())
+        best_results['best_values'] = \
+            (['par_names'], self.best_values.values())
+        best_results['best_errors'] = \
+            (['par_names'], self.best_errors.values())
         best_results.attrs['components'] = self.components
-        return(best_results)
+        return best_results
 
     @property
     def best_values(self):
+        """Return values of the best fit parameters."""
         if self._result is None:
-            return(None)
-        return({name:self._result.params[name].value for name in sorted(self._result.params)
-                if name != 'tmp_normalization_offset_c'})
+            return None
+        return {name:self._result.params[name].value
+                for name in sorted(self._result.params)
+                if name != 'tmp_normalization_offset_c'}
 
     @property
     def chisqr(self):
+        """Return the chisqr value of the best fit."""
         if self._result is None:
-            return(None)
-        return(self._result.chisqr)
+            return None
+        return self._result.chisqr
 
     @property
     def components(self):
+        """Return the fit model components info."""
         components = {}
         if self._result is None:
-            logging.warning('Unable to collect components in Fit.components')
-            return(components)
+            logger.warning('Unable to collect components in Fit.components')
+            return components
         for component in self._result.components:
             if 'tmp_normalization_offset_c' in component.param_names:
                 continue
             parameters = {}
             for name in component.param_names:
                 par = self._parameters[name]
-                parameters[name] = {'free': par.vary, 'value': self._result.params[name].value}
+                parameters[name] = {
+                    'free': par.vary,
+                    'value': self._result.params[name].value,
+                }
                 if par.expr is not None:
                     parameters[name]['expr'] = par.expr
             expr = None
             if isinstance(component, ExpressionModel):
                 name = component._name
                 if name[-1] == '_':
                     name = name[:-1]
                 expr = component.expr
             else:
                 prefix = component.prefix
-                if len(prefix):
+                if prefix:
                     if prefix[-1] == '_':
                         prefix = prefix[:-1]
                     name = f'{prefix} ({component._name})'
                 else:
                     name = f'{component._name}'
             if expr is None:
-                components[name] = {'parameters': parameters}
-            else:
-                components[name] = {'expr': expr, 'parameters': parameters}
-        return(components)
+                components[name] = {
+                    'parameters': parameters,
+                }
+            else:
+                components[name] = {
+                    'expr': expr,
+                    'parameters': parameters,
+                }
+        return components
 
     @property
     def covar(self):
+        """Return the covarience matrix of the best fit parameters."""
         if self._result is None:
-            return(None)
-        return(self._result.covar)
+            return None
+        return self._result.covar
 
     @property
     def init_parameters(self):
+        """Return the initial parameters for the fit model."""
         if self._result is None or self._result.init_params is None:
-            return(None)
+            return None
         parameters = {}
         for name in sorted(self._result.init_params):
             if name != 'tmp_normalization_offset_c':
                 par = self._result.init_params[name]
-                parameters[name] = {'value': par.value, 'min': par.min, 'max': par.max,
-                        'vary': par.vary, 'expr': par.expr}
-        return(parameters)
+                parameters[name] = {
+                    'value': par.value,
+                    'min': par.min,
+                    'max': par.max,
+                    'vary': par.vary,
+                    'expr': par.expr,
+                }
+        return parameters
 
     @property
     def init_values(self):
+        """Return the initial values for the fit parameters."""
         if self._result is None or self._result.init_params is None:
-            return(None)
-        return({name:self._result.init_params[name].value for name in
-                sorted(self._result.init_params) if name != 'tmp_normalization_offset_c'})
+            return None
+        return {name:self._result.init_params[name].value
+                for name in sorted(self._result.init_params)
+                if name != 'tmp_normalization_offset_c'}
 
     @property
     def normalization_offset(self):
+        """Return the normalization_offset for the fit model."""
         if self._result is None:
-            return(None)
+            return None
         if self._norm is None:
-            return(0.0)
-        else:
-            if self._result.init_params is not None:
-                normalization_offset = float(self._result.init_params['tmp_normalization_offset_c'])
-            else:
-                normalization_offset = float(self._result.params['tmp_normalization_offset_c'])
-            return(normalization_offset)
+            return 0.0
+        if self._result.init_params is not None:
+            normalization_offset = float(
+                self._result.init_params['tmp_normalization_offset_c'])
+        else:
+            normalization_offset = float(
+                self._result.params['tmp_normalization_offset_c'])
+        return normalization_offset
 
     @property
     def num_func_eval(self):
+        """
+        Return the number of function evaluations for the best fit.
+        """
         if self._result is None:
-            return(None)
-        return(self._result.nfev)
+            return None
+        return self._result.nfev
 
     @property
     def parameters(self):
-        return({name:{'min': par.min, 'max': par.max, 'vary': par.vary, 'expr': par.expr}
-                for name, par in self._parameters.items() if name != 'tmp_normalization_offset_c'})
+        """Return the fit parameter info."""
+        return {name:{'min': par.min, 'max': par.max, 'vary': par.vary,
+                'expr': par.expr} for name, par in self._parameters.items()
+                if name != 'tmp_normalization_offset_c'}
 
     @property
     def redchi(self):
+        """Return the redchi value of the best fit."""
         if self._result is None:
-            return(None)
-        return(self._result.redchi)
+            return None
+        return self._result.redchi
 
     @property
     def residual(self):
+        """Return the residual in the best fit."""
         if self._result is None:
-            return(None)
-        return(self._result.residual)
+            return None
+        return self._result.residual
 
     @property
     def success(self):
+        """Return the success value for the fit."""
         if self._result is None:
-            return(None)
+            return None
         if not self._result.success:
-#            print(f'ier = {self._result.ier}')
-#            print(f'lmdif_message = {self._result.lmdif_message}')
-#            print(f'message = {self._result.message}')
-#            print(f'nfev = {self._result.nfev}')
-#            print(f'redchi = {self._result.redchi}')
-#            print(f'success = {self._result.success}')
-            if self._result.ier == 0 or self._result.ier == 5:
-                logging.warning(f'ier = {self._result.ier}: {self._result.message}')
-            else:
-                logging.warning(f'ier = {self._result.ier}: {self._result.message}')
-                return(True)
-#            self.print_fit_report()
-#            self.plot()
-        return(self._result.success)
+            logger.warning(
+                f'ier = {self._result.ier}: {self._result.message}')
+            if self._result.ier and self._result.ier != 5:
+                return True
+        return self._result.success
 
     @property
     def var_names(self):
-        """Intended to be used with covar
+        """
+        Return the variable names for the covarience matrix property.
         """
         if self._result is None:
-            return(None)
-        return(getattr(self._result, 'var_names', None))
+            return None
+        return getattr(self._result, 'var_names', None)
 
     @property
     def x(self):
-        return(self._x)
+        """Return the input x-array."""
+        return self._x
 
     @property
     def y(self):
-        return(self._y)
+        """Return the input y-array."""
+        return self._y
 
     def print_fit_report(self, result=None, show_correl=False):
+        """Print a fit report."""
         if result is None:
             result = self._result
         if result is not None:
             print(result.fit_report(show_correl=show_correl))
 
     def add_parameter(self, **parameter):
+        """Add a fit fit parameter to the fit model."""
         if not isinstance(parameter, dict):
             raise ValueError(f'Invalid parameter ({parameter})')
         if parameter.get('expr') is not None:
             raise KeyError(f'Invalid "expr" key in parameter {parameter}')
         name = parameter['name']
         if not isinstance(name, str):
-            raise ValueError(f'Invalid "name" value ({name}) in parameter {parameter}')
+            raise ValueError(
+                f'Invalid "name" value ({name}) in parameter {parameter}')
         if parameter.get('norm') is None:
             self._parameter_norms[name] = False
         else:
             norm = parameter.pop('norm')
             if self._norm is None:
-                logging.warning(f'Ignoring norm in parameter {name} in '+
-                            f'Fit.add_parameter (normalization is turned off)')
+                logger.warning(
+                    f'Ignoring norm in parameter {name} in Fit.add_parameter '
+                    '(normalization is turned off)')
                 self._parameter_norms[name] = False
             else:
                 if not isinstance(norm, bool):
-                    raise ValueError(f'Invalid "norm" value ({norm}) in parameter {parameter}')
+                    raise ValueError(
+                        f'Invalid "norm" value ({norm}) in parameter '
+                        f'{parameter}')
                 self._parameter_norms[name] = norm
         vary = parameter.get('vary')
         if vary is not None:
             if not isinstance(vary, bool):
-                raise ValueError(f'Invalid "vary" value ({vary}) in parameter {parameter}')
+                raise ValueError(
+                    f'Invalid "vary" value ({vary}) in parameter {parameter}')
             if not vary:
                 if 'min' in parameter:
-                    logging.warning(f'Ignoring min in parameter {name} in '+
-                            f'Fit.add_parameter (vary = {vary})')
+                    logger.warning(
+                        f'Ignoring min in parameter {name} in '
+                        f'Fit.add_parameter (vary = {vary})')
                     parameter.pop('min')
                 if 'max' in parameter:
-                    logging.warning(f'Ignoring max in parameter {name} in '+
-                            f'Fit.add_parameter (vary = {vary})')
+                    logger.warning(
+                        f'Ignoring max in parameter {name} in '
+                        f'Fit.add_parameter (vary = {vary})')
                     parameter.pop('max')
         if self._norm is not None and name not in self._parameter_norms:
-            raise ValueError(f'Missing parameter normalization type for paremeter {name}')
+            raise ValueError(
+                f'Missing parameter normalization type for parameter {name}')
         self._parameters.add(**parameter)
 
-    def add_model(self, model, prefix=None, parameters=None, parameter_norms=None, **kwargs):
-        # Create the new model
-#        print(f'at start add_model:\nself._parameters:\n{self._parameters}')
-#        print(f'at start add_model: kwargs = {kwargs}')
-#        print(f'parameters = {parameters}')
-#        print(f'parameter_norms = {parameter_norms}')
-#        if len(self._parameters.keys()):
-#            print('\nAt start adding model:')
-#            self._parameters.pretty_print()
-#            print(f'parameter_norms:\n{self._parameter_norms}')
+    def add_model(
+            self, model, prefix=None, parameters=None, parameter_norms=None,
+            **kwargs):
+        """Add a model component to the fit model."""
+        # Third party modules
+        from asteval import (
+            Interpreter,
+            get_ast_names,
+        )
+
         if prefix is not None and not isinstance(prefix, str):
-            logging.warning('Ignoring illegal prefix: {model} {type(model)}')
+            logger.warning('Ignoring illegal prefix: {model} {type(model)}')
             prefix = None
         if prefix is None:
             pprefix = ''
         else:
             pprefix = prefix
         if parameters is not None:
             if isinstance(parameters, dict):
                 parameters = (parameters, )
             elif not is_dict_series(parameters):
-                illegal_value(parameters, 'parameters', 'Fit.add_model', raise_error=True)
+                raise ValueError('Invalid parameter parameters ({parameters})')
             parameters = deepcopy(parameters)
         if parameter_norms is not None:
             if isinstance(parameter_norms, dict):
                 parameter_norms = (parameter_norms, )
             if not is_dict_series(parameter_norms):
-                illegal_value(parameter_norms, 'parameter_norms', 'Fit.add_model', raise_error=True)
+                raise ValueError(
+                    'Invalid parameter parameters_norms ({parameters_norms})')
         new_parameter_norms = {}
         if callable(model):
             # Linear fit not yet implemented for callable models
             self._try_linear_fit = False
             if parameter_norms is None:
                 if parameters is None:
-                    raise ValueError('Either "parameters" or "parameter_norms" is required in '+
-                            f'{model}')
+                    raise ValueError(
+                        'Either parameters or parameter_norms is required in '
+                        f'{model}')
                 for par in parameters:
                     name = par['name']
                     if not isinstance(name, str):
-                        raise ValueError(f'Invalid "name" value ({name}) in input parameters')
+                        raise ValueError(
+                            f'Invalid "name" value ({name}) in input '
+                            'parameters')
                     if par.get('norm') is not None:
                         norm = par.pop('norm')
                         if not isinstance(norm, bool):
-                            raise ValueError(f'Invalid "norm" value ({norm}) in input parameters')
+                            raise ValueError(
+                                f'Invalid "norm" value ({norm}) in input '
+                                'parameters')
                         new_parameter_norms[f'{pprefix}{name}'] = norm
             else:
                 for par in parameter_norms:
                     name = par['name']
                     if not isinstance(name, str):
-                        raise ValueError(f'Invalid "name" value ({name}) in input parameters')
+                        raise ValueError(
+                            f'Invalid "name" value ({name}) in input '
+                            'parameters')
                     norm = par.get('norm')
                     if norm is None or not isinstance(norm, bool):
-                        raise ValueError(f'Invalid "norm" value ({norm}) in input parameters')
+                        raise ValueError(
+                            f'Invalid "norm" value ({norm}) in input '
+                            'parameters')
                     new_parameter_norms[f'{pprefix}{name}'] = norm
             if parameters is not None:
                 for par in parameters:
                     if par.get('expr') is not None:
-                        raise KeyError(f'Invalid "expr" key ({par.get("expr")}) in parameter '+
-                                f'{name} for a callable model {model}')
+                        raise KeyError(
+                            f'Invalid "expr" key ({par.get("expr")}) in '
+                            f'parameter {name} for a callable model {model}')
                     name = par['name']
                     if not isinstance(name, str):
-                        raise ValueError(f'Invalid "name" value ({name}) in input parameters')
-# RV FIX callable model will need partial deriv functions for any linear pars to get the linearized matrix, so for now skip linear solution option
+                        raise ValueError(
+                            f'Invalid "name" value ({name}) in input '
+                            'parameters')
+# RV callable model will need partial deriv functions for any linear
+#     parameter to get the linearized matrix, so for now skip linear
+#     solution option
             newmodel = Model(model, prefix=prefix)
         elif isinstance(model, str):
-            if model == 'constant':      # Par: c
+            if model == 'constant':
+                # Par: c
                 newmodel = ConstantModel(prefix=prefix)
                 new_parameter_norms[f'{pprefix}c'] = True
                 self._linear_parameters.append(f'{pprefix}c')
-            elif model == 'linear':      # Par: slope, intercept
+            elif model == 'linear':
+                # Par: slope, intercept
                 newmodel = LinearModel(prefix=prefix)
                 new_parameter_norms[f'{pprefix}slope'] = True
                 new_parameter_norms[f'{pprefix}intercept'] = True
                 self._linear_parameters.append(f'{pprefix}slope')
                 self._linear_parameters.append(f'{pprefix}intercept')
-            elif model == 'quadratic':   # Par: a, b, c
+            elif model == 'quadratic':
+                # Par: a, b, c
                 newmodel = QuadraticModel(prefix=prefix)
                 new_parameter_norms[f'{pprefix}a'] = True
                 new_parameter_norms[f'{pprefix}b'] = True
                 new_parameter_norms[f'{pprefix}c'] = True
                 self._linear_parameters.append(f'{pprefix}a')
                 self._linear_parameters.append(f'{pprefix}b')
                 self._linear_parameters.append(f'{pprefix}c')
-            elif model == 'polynomial': # Par: c0, c1,..., c7
+            elif model == 'polynomial':
+                # Par: c0, c1,..., c7
                 degree = kwargs.get('degree')
                 if degree is not None:
                     kwargs.pop('degree')
                 if degree is None or not is_int(degree, ge=0, le=7):
-                    raise ValueError(f'Invalid parameter degree for build-in step model ({degree})')
+                    raise ValueError(
+                        'Invalid parameter degree for build-in step model '
+                        f'({degree})')
                 newmodel = PolynomialModel(degree=degree, prefix=prefix)
                 for i in range(degree+1):
                     new_parameter_norms[f'{pprefix}c{i}'] = True
                     self._linear_parameters.append(f'{pprefix}c{i}')
-            elif model == 'gaussian':    # Par: amplitude, center, sigma (fwhm, height)
+            elif model == 'gaussian':
+                # Par: amplitude, center, sigma (fwhm, height)
                 newmodel = GaussianModel(prefix=prefix)
                 new_parameter_norms[f'{pprefix}amplitude'] = True
                 new_parameter_norms[f'{pprefix}center'] = False
                 new_parameter_norms[f'{pprefix}sigma'] = False
                 self._linear_parameters.append(f'{pprefix}amplitude')
                 self._nonlinear_parameters.append(f'{pprefix}center')
                 self._nonlinear_parameters.append(f'{pprefix}sigma')
-                # parameter norms for height and fwhm are needed to get correct errors
+                # parameter norms for height and fwhm are needed to
+                #   get correct errors
                 new_parameter_norms[f'{pprefix}height'] = True
                 new_parameter_norms[f'{pprefix}fwhm'] = False
-            elif model == 'lorentzian':    # Par: amplitude, center, sigma (fwhm, height)
+            elif model == 'lorentzian':
+                # Par: amplitude, center, sigma (fwhm, height)
                 newmodel = LorentzianModel(prefix=prefix)
                 new_parameter_norms[f'{pprefix}amplitude'] = True
                 new_parameter_norms[f'{pprefix}center'] = False
                 new_parameter_norms[f'{pprefix}sigma'] = False
                 self._linear_parameters.append(f'{pprefix}amplitude')
                 self._nonlinear_parameters.append(f'{pprefix}center')
                 self._nonlinear_parameters.append(f'{pprefix}sigma')
-                # parameter norms for height and fwhm are needed to get correct errors
+                # parameter norms for height and fwhm are needed to
+                #   get correct errors
                 new_parameter_norms[f'{pprefix}height'] = True
                 new_parameter_norms[f'{pprefix}fwhm'] = False
-            elif model == 'exponential': # Par: amplitude, decay
+            elif model == 'exponential':
+                # Par: amplitude, decay
                 newmodel = ExponentialModel(prefix=prefix)
                 new_parameter_norms[f'{pprefix}amplitude'] = True
                 new_parameter_norms[f'{pprefix}decay'] = False
                 self._linear_parameters.append(f'{pprefix}amplitude')
                 self._nonlinear_parameters.append(f'{pprefix}decay')
-            elif model == 'step':        # Par: amplitude, center, sigma
+            elif model == 'step':
+                # Par: amplitude, center, sigma
                 form = kwargs.get('form')
                 if form is not None:
                     kwargs.pop('form')
-                if form is None or form not in ('linear', 'atan', 'arctan', 'erf', 'logistic'):
-                    raise ValueError(f'Invalid parameter form for build-in step model ({form})')
+                if (form is None or form not in
+                        ('linear', 'atan', 'arctan', 'erf', 'logistic')):
+                    raise ValueError(
+                        'Invalid parameter form for build-in step model '
+                        f'({form})')
                 newmodel = StepModel(prefix=prefix, form=form)
                 new_parameter_norms[f'{pprefix}amplitude'] = True
                 new_parameter_norms[f'{pprefix}center'] = False
                 new_parameter_norms[f'{pprefix}sigma'] = False
                 self._linear_parameters.append(f'{pprefix}amplitude')
                 self._nonlinear_parameters.append(f'{pprefix}center')
                 self._nonlinear_parameters.append(f'{pprefix}sigma')
-            elif model == 'rectangle':   # Par: amplitude, center1, center2, sigma1, sigma2
+            elif model == 'rectangle':
+                # Par: amplitude, center1, center2, sigma1, sigma2
                 form = kwargs.get('form')
                 if form is not None:
                     kwargs.pop('form')
-                if form is None or form not in ('linear', 'atan', 'arctan', 'erf', 'logistic'):
-                    raise ValueError('Invalid parameter form for build-in rectangle model '+
-                            f'({form})')
+                if (form is None or form not in
+                        ('linear', 'atan', 'arctan', 'erf', 'logistic')):
+                    raise ValueError(
+                        'Invalid parameter form for build-in rectangle model '
+                        f'({form})')
                 newmodel = RectangleModel(prefix=prefix, form=form)
                 new_parameter_norms[f'{pprefix}amplitude'] = True
                 new_parameter_norms[f'{pprefix}center1'] = False
                 new_parameter_norms[f'{pprefix}center2'] = False
                 new_parameter_norms[f'{pprefix}sigma1'] = False
                 new_parameter_norms[f'{pprefix}sigma2'] = False
                 self._linear_parameters.append(f'{pprefix}amplitude')
                 self._nonlinear_parameters.append(f'{pprefix}center1')
                 self._nonlinear_parameters.append(f'{pprefix}center2')
                 self._nonlinear_parameters.append(f'{pprefix}sigma1')
                 self._nonlinear_parameters.append(f'{pprefix}sigma2')
-            elif model == 'expression':  # Par: by expression
+            elif model == 'expression':
+                # Par: by expression
                 expr = kwargs['expr']
                 if not isinstance(expr, str):
-                    raise ValueError(f'Invalid "expr" value ({expr}) in {model}')
+                    raise ValueError(
+                        f'Invalid "expr" value ({expr}) in {model}')
                 kwargs.pop('expr')
                 if parameter_norms is not None:
-                        logging.warning('Ignoring parameter_norms (normalization determined from '+
-                                'linearity)}')
+                    logger.warning(
+                        'Ignoring parameter_norms (normalization '
+                        'determined from linearity)}')
                 if parameters is not None:
                     for par in parameters:
                         if par.get('expr') is not None:
-                            raise KeyError(f'Invalid "expr" key ({par.get("expr")}) in parameter '+
-                                    f'({par}) for an expression model')
+                            raise KeyError(
+                                f'Invalid "expr" key ({par.get("expr")}) in '
+                                f'parameter ({par}) for an expression model')
                         if par.get('norm') is not None:
-                            logging.warning(f'Ignoring "norm" key in parameter ({par}) '+
-                                '(normalization determined from linearity)}')
+                            logger.warning(
+                                f'Ignoring "norm" key in parameter ({par}) '
+                                '(normalization determined from linearity)')
                             par.pop('norm')
                         name = par['name']
                         if not isinstance(name, str):
-                            raise ValueError(f'Invalid "name" value ({name}) in input parameters')
+                            raise ValueError(
+                                f'Invalid "name" value ({name}) in input '
+                                'parameters')
                 ast = Interpreter()
-                expr_parameters = [name for name in get_ast_names(ast.parse(expr))
-                        if name != 'x' and name not in self._parameters
-                        and name not in ast.symtable]
-#                print(f'\nexpr_parameters: {expr_parameters}')
-#                print(f'expr = {expr}')
+                expr_parameters = [
+                    name for name in get_ast_names(ast.parse(expr))
+                    if (name != 'x' and name not in self._parameters
+                        and name not in ast.symtable)]
                 if prefix is None:
                     newmodel = ExpressionModel(expr=expr)
                 else:
                     for name in expr_parameters:
                         expr = sub(rf'\b{name}\b', f'{prefix}{name}', expr)
-                    expr_parameters = [f'{prefix}{name}' for name in expr_parameters]
-#                    print(f'\nexpr_parameters: {expr_parameters}')
-#                    print(f'expr = {expr}')
+                    expr_parameters = [
+                        f'{prefix}{name}' for name in expr_parameters]
                     newmodel = ExpressionModel(expr=expr, name=name)
-#                print(f'\nnewmodel = {newmodel.__dict__}')
-#                print(f'params_names = {newmodel._param_names}')
-#                print(f'params_names = {newmodel.param_names}')
                 # Remove already existing names
                 for name in newmodel.param_names.copy():
                     if name not in expr_parameters:
                         newmodel._func_allargs.remove(name)
                         newmodel._param_names.remove(name)
-#                print(f'params_names = {newmodel._param_names}')
-#                print(f'params_names = {newmodel.param_names}')
             else:
                 raise ValueError(f'Unknown build-in fit model ({model})')
         else:
-            illegal_value(model, 'model', 'Fit.add_model', raise_error=True)
+            raise ValueError('Invalid parameter model ({model})')
 
         # Add the new model to the current one
-#        print('\nBefore adding model:')
-#        print(f'\nnewmodel = {newmodel.__dict__}')
-#        if len(self._parameters):
-#            self._parameters.pretty_print()
         if self._model is None:
             self._model = newmodel
         else:
             self._model += newmodel
         new_parameters = newmodel.make_params()
         self._parameters += new_parameters
-#        print('\nAfter adding model:')
-#        print(f'\nnewmodel = {newmodel.__dict__}')
-#        print(f'\nnew_parameters = {new_parameters}')
-#        self._parameters.pretty_print()
 
-        # Check linearity of expression model paremeters
+        # Check linearity of expression model parameters
         if isinstance(newmodel, ExpressionModel):
             for name in newmodel.param_names:
                 if not diff(newmodel.expr, name, name):
                     if name not in self._linear_parameters:
                         self._linear_parameters.append(name)
                         new_parameter_norms[name] = True
-#                        print(f'\nADDING {name} TO LINEAR')
                 else:
                     if name not in self._nonlinear_parameters:
                         self._nonlinear_parameters.append(name)
                         new_parameter_norms[name] = False
-#                        print(f'\nADDING {name} TO NONLINEAR')
-#        print(f'new_parameter_norms:\n{new_parameter_norms}')
 
         # Scale the default initial model parameters
         if self._norm is not None:
             for name, norm in new_parameter_norms.copy().items():
                 par = self._parameters.get(name)
                 if par is None:
                     new_parameter_norms.pop(name)
                     continue
                 if par.expr is None and norm:
                     value = par.value*self._norm[1]
                     _min = par.min
                     _max = par.max
-                    if not np.isinf(_min) and abs(_min) != float_min:
+                    if not np.isinf(_min) and abs(_min) != FLOAT_MIN:
                         _min *= self._norm[1]
-                    if not np.isinf(_max) and abs(_max) != float_min:
+                    if not np.isinf(_max) and abs(_max) != FLOAT_MIN:
                         _max *= self._norm[1]
                     par.set(value=value, min=_min, max=_max)
-#        print('\nAfter norm defaults:')
-#        self._parameters.pretty_print()
-#        print(f'parameters:\n{parameters}')
-#        print(f'all_parameters:\n{list(self.parameters)}')
-#        print(f'new_parameter_norms:\n{new_parameter_norms}')
-#        print(f'parameter_norms:\n{self._parameter_norms}')
 
         # Initialize the model parameters from parameters
         if prefix is None:
-            prefix = ""
+            prefix = ''
         if parameters is not None:
             for parameter in parameters:
                 name = parameter['name']
                 if not isinstance(name, str):
-                    raise ValueError(f'Invalid "name" value ({name}) in input parameters')
+                    raise ValueError(
+                        f'Invalid "name" value ({name}) in input parameters')
                 if name not in new_parameters:
                     name = prefix+name
                     parameter['name'] = name
                 if name not in new_parameters:
-                    logging.warning(f'Ignoring superfluous parameter info for {name}')
+                    logger.warning(
+                        f'Ignoring superfluous parameter info for {name}')
                     continue
                 if name in self._parameters:
                     parameter.pop('name')
                     if 'norm' in parameter:
                         if not isinstance(parameter['norm'], bool):
-                            illegal_value(parameter['norm'], 'norm', 'Fit.add_model',
-                                    raise_error=True)
+                            raise ValueError(
+                                f'Invalid "norm" value ({norm}) in the '
+                                f'input parameter {name}')
                         new_parameter_norms[name] = parameter['norm']
                         parameter.pop('norm')
                     if parameter.get('expr') is not None:
                         if 'value' in parameter:
-                            logging.warning(f'Ignoring value in parameter {name} '+
-                                    f'(set by expression: {parameter["expr"]})')
+                            logger.warning(
+                                f'Ignoring value in parameter {name} '
+                                f'(set by expression: {parameter["expr"]})')
                             parameter.pop('value')
                         if 'vary' in parameter:
-                            logging.warning(f'Ignoring vary in parameter {name} '+
-                                    f'(set by expression: {parameter["expr"]})')
+                            logger.warning(
+                                f'Ignoring vary in parameter {name} '
+                                f'(set by expression: {parameter["expr"]})')
                             parameter.pop('vary')
                         if 'min' in parameter:
-                            logging.warning(f'Ignoring min in parameter {name} '+
-                                    f'(set by expression: {parameter["expr"]})')
+                            logger.warning(
+                                f'Ignoring min in parameter {name} '
+                                f'(set by expression: {parameter["expr"]})')
                             parameter.pop('min')
                         if 'max' in parameter:
-                            logging.warning(f'Ignoring max in parameter {name} '+
-                                    f'(set by expression: {parameter["expr"]})')
+                            logger.warning(
+                                f'Ignoring max in parameter {name} '
+                                f'(set by expression: {parameter["expr"]})')
                             parameter.pop('max')
                     if 'vary' in parameter:
                         if not isinstance(parameter['vary'], bool):
-                            illegal_value(parameter['vary'], 'vary', 'Fit.add_model',
-                                    raise_error=True)
+                            raise ValueError(
+                                f'Invalid "vary" value ({parameter["vary"]}) '
+                                f'in the input parameter {name}')
                         if not parameter['vary']:
                             if 'min' in parameter:
-                                logging.warning(f'Ignoring min in parameter {name} in '+
-                                        f'Fit.add_model (vary = {parameter["vary"]})')
+                                logger.warning(
+                                    f'Ignoring min in parameter {name} '
+                                    f'(vary = {parameter["vary"]})')
                                 parameter.pop('min')
                             if 'max' in parameter:
-                                logging.warning(f'Ignoring max in parameter {name} in '+
-                                        f'Fit.add_model (vary = {parameter["vary"]})')
+                                logger.warning(
+                                    f'Ignoring max in parameter {name} '
+                                    f'(vary = {parameter["vary"]})')
                                 parameter.pop('max')
                     self._parameters[name].set(**parameter)
                     parameter['name'] = name
                 else:
-                    illegal_value(parameter, 'parameter name', 'Fit.model', raise_error=True)
-        self._parameter_norms = {**self._parameter_norms, **new_parameter_norms}
-#        print('\nAfter parameter init:')
-#        self._parameters.pretty_print()
-#        print(f'parameters:\n{parameters}')
-#        print(f'new_parameter_norms:\n{new_parameter_norms}')
-#        print(f'parameter_norms:\n{self._parameter_norms}')
-#        print(f'kwargs:\n{kwargs}')
+                    raise ValueError(
+                        'Invalid parameter name in parameters ({name})')
+        self._parameter_norms = {
+            **self._parameter_norms,
+            **new_parameter_norms,
+        }
 
         # Initialize the model parameters from kwargs
         for name, value in {**kwargs}.items():
             full_name = f'{pprefix}{name}'
-            if full_name in new_parameter_norms and isinstance(value, (int, float)):
+            if (full_name in new_parameter_norms
+                    and isinstance(value, (int, float))):
                 kwargs.pop(name)
                 if self._parameters[full_name].expr is None:
                     self._parameters[full_name].set(value=value)
                 else:
-                    logging.warning(f'Ignoring parameter {name} in Fit.fit (set by expression: '+
-                            f'{self._parameters[full_name].expr})')
-#        print('\nAfter kwargs init:')
-#        self._parameters.pretty_print()
-#        print(f'parameter_norms:\n{self._parameter_norms}')
-#        print(f'kwargs:\n{kwargs}')
-
-        # Check parameter norms (also need it for expressions to renormalize the errors)
-        if self._norm is not None and (callable(model) or model == 'expression'):
+                    logger.warning(
+                        f'Ignoring parameter {name} (set by expression: '
+                        f'{self._parameters[full_name].expr})')
+
+        # Check parameter norms
+        # (also need it for expressions to renormalize the errors)
+        if (self._norm is not None
+                and (callable(model) or model == 'expression')):
             missing_norm = False
             for name in new_parameters.valuesdict():
                 if name not in self._parameter_norms:
                     print(f'new_parameters:\n{new_parameters.valuesdict()}')
                     print(f'self._parameter_norms:\n{self._parameter_norms}')
-                    logging.error(f'Missing parameter normalization type for {name} in {model}')
+                    logger.error(
+                        f'Missing parameter normalization type for {name} in '
+                        f'{model}')
                     missing_norm = True
             if missing_norm:
                 raise ValueError
 
-#        print(f'at end add_model:\nself._parameters:\n{list(self.parameters)}')
-#        print(f'at end add_model: kwargs = {kwargs}')
-#        print(f'\nat end add_model: newmodel:\n{newmodel.__dict__}\n')
-        return(kwargs)
+        return kwargs
 
     def eval(self, x, result=None):
+        """Evaluate the best fit."""
         if result is None:
             result = self._result
         if result is None:
-            return
-        return(result.eval(x=np.asarray(x))-self.normalization_offset)
+            return None
+        return result.eval(x=np.asarray(x))-self.normalization_offset
 
-    def fit(self, interactive=False, guess=False, **kwargs):
+    def fit(self, **kwargs):
+        """Fit the model to the input data."""
         # Check inputs
         if self._model is None:
-            logging.error('Undefined fit model')
-            return
-        if not isinstance(interactive, bool):
-            illegal_value(interactive, 'interactive', 'Fit.fit', raise_error=True)
-        if not isinstance(guess, bool):
-            illegal_value(guess, 'guess', 'Fit.fit', raise_error=True)
+            logger.error('Undefined fit model')
+            return None
+        if 'interactive' in kwargs:
+            interactive = kwargs.pop('interactive')
+            if not isinstance(interactive, bool):
+                raise ValueError(
+                    'Invalid value of keyword argument interactive '
+                    f'({interactive})')
+        else:
+            interactive = False
+        if 'guess' in kwargs:
+            guess = kwargs.pop('guess')
+            if not isinstance(guess, bool):
+                raise ValueError(
+                    f'Invalid value of keyword argument guess ({guess})')
+        else:
+            guess = False
         if 'try_linear_fit' in kwargs:
             try_linear_fit = kwargs.pop('try_linear_fit')
             if not isinstance(try_linear_fit, bool):
-                illegal_value(try_linear_fit, 'try_linear_fit', 'Fit.fit', raise_error=True)
+                raise ValueError(
+                    'Invalid value of keyword argument try_linear_fit '
+                    f'({try_linear_fit})')
             if not self._try_linear_fit:
-                logging.warning('Ignore superfluous keyword argument "try_linear_fit" (not '+
-                        'yet supported for callable models)')
+                logger.warning(
+                    'Ignore superfluous keyword argument "try_linear_fit" '
+                    '(not yet supported for callable models)')
             else:
                 self._try_linear_fit = try_linear_fit
-#        if self._result is None:
-#            if 'parameters' in kwargs:
-#                raise ValueError('Invalid parameter parameters ({kwargs["parameters"]})')
-#        else:
         if self._result is not None:
             if guess:
-                logging.warning('Ignoring input parameter guess in Fit.fit during refitting')
+                logger.warning(
+                    'Ignoring input parameter guess during refitting')
                 guess = False
 
         # Check for circular expressions
-        # FIX TODO
+        # RV
 #        for name1, par1 in self._parameters.items():
 #            if par1.expr is not None:
 
         # Apply mask if supplied:
         if 'mask' in kwargs:
             self._mask = kwargs.pop('mask')
         if self._mask is not None:
             self._mask = np.asarray(self._mask).astype(bool)
             if self._x.size != self._mask.size:
-                raise ValueError(f'Inconsistent x and mask dimensions ({self._x.size} vs '+
-                        f'{self._mask.size})')
+                raise ValueError(
+                    f'Inconsistent x and mask dimensions ({self._x.size} vs '
+                    f'{self._mask.size})')
 
-        # Estimate initial parameters with build-in lmfit guess method (only for a single model)
-#        print(f'\nat start fit: kwargs = {kwargs}')
-#RV        print('\nAt start of fit:')
-#RV        self._parameters.pretty_print()
-#        print(f'parameter_norms:\n{self._parameter_norms}')
+        # Estimate initial parameters with build-in lmfit guess method
+        # (only mplemented for a single model)
         if guess:
             if self._mask is None:
                 self._parameters = self._model.guess(self._y, x=self._x)
             else:
-                self._parameters = self._model.guess(np.asarray(self._y)[~self._mask],
-                        x=self._x[~self._mask])
-#            print('\nAfter guess:')
-#            self._parameters.pretty_print()
+                self._parameters = self._model.guess(
+                    np.asarray(self._y)[~self._mask], x=self._x[~self._mask])
 
         # Add constant offset for a normalized model
         if self._result is None and self._norm is not None and self._norm[0]:
-            self.add_model('constant', prefix='tmp_normalization_offset_', parameters={'name': 'c',
-                    'value': -self._norm[0], 'vary': False, 'norm': True})
-                    #'value': -self._norm[0]/self._norm[1], 'vary': False, 'norm': False})
+            self.add_model(
+                'constant', prefix='tmp_normalization_offset_',
+                parameters={
+                    'name': 'c',
+                    'value': -self._norm[0],
+                    'vary': False,
+                    'norm': True,
+                })
+#                    'value': -self._norm[0]/self._norm[1],
+#                    'vary': False,
+#                    'norm': False,
 
         # Adjust existing parameters for refit:
         if 'parameters' in kwargs:
             parameters = kwargs.pop('parameters')
             if isinstance(parameters, dict):
                 parameters = (parameters, )
             elif not is_dict_series(parameters):
-                illegal_value(parameters, 'parameters', 'Fit.fit', raise_error=True)
+                raise ValueError(
+                    'Invalid value of keyword argument parameters '
+                    f'({parameters})')
             for par in parameters:
                 name = par['name']
                 if name not in self._parameters:
-                    raise ValueError(f'Unable to match {name} parameter {par} to an existing one')
+                    raise ValueError(
+                        f'Unable to match {name} parameter {par} to an '
+                        'existing one')
                 if self._parameters[name].expr is not None:
-                    raise ValueError(f'Unable to modify {name} parameter {par} (currently an '+
-                            'expression)')
+                    raise ValueError(
+                        f'Unable to modify {name} parameter {par} '
+                        '(currently an expression)')
                 if par.get('expr') is not None:
-                    raise KeyError(f'Invalid "expr" key in {name} parameter {par}')
+                    raise KeyError(
+                        f'Invalid "expr" key in {name} parameter {par}')
                 self._parameters[name].set(vary=par.get('vary'))
                 self._parameters[name].set(min=par.get('min'))
                 self._parameters[name].set(max=par.get('max'))
                 self._parameters[name].set(value=par.get('value'))
-#RV            print('\nAfter adjust:')
-#RV            self._parameters.pretty_print()
 
         # Apply parameter updates through keyword arguments
-#        print(f'kwargs = {kwargs}')
-#        print(f'parameter_norms = {self._parameter_norms}')
         for name in set(self._parameters) & set(kwargs):
             value = kwargs.pop(name)
             if self._parameters[name].expr is None:
                 self._parameters[name].set(value=value)
             else:
-                logging.warning(f'Ignoring parameter {name} in Fit.fit (set by expression: '+
-                        f'{self._parameters[name].expr})')
+                logger.warning(
+                    f'Ignoring parameter {name} (set by expression: '
+                    f'{self._parameters[name].expr})')
 
         # Check for uninitialized parameters
         for name, par in self._parameters.items():
             if par.expr is None:
                 value = par.value
                 if value is None or np.isinf(value) or np.isnan(value):
                     if interactive:
-                        value = input_num(f'Enter an initial value for {name}', default=1.0)
+                        value = input_num(
+                            f'Enter an initial value for {name}', default=1.0)
                     else:
                         value = 1.0
                     if self._norm is None or name not in self._parameter_norms:
                         self._parameters[name].set(value=value)
                     elif self._parameter_norms[name]:
                         self._parameters[name].set(value=value*self._norm[1])
 
         # Check if model is linear
         try:
             linear_model = self._check_linearity_model()
         except:
             linear_model = False
-#        print(f'\n\n--------> linear_model = {linear_model}\n')
         if kwargs.get('check_only_linearity') is not None:
-            return(linear_model)
+            return linear_model
 
         # Normalize the data and initial parameters
-#RV        print('\nBefore normalization:')
-#RV        self._parameters.pretty_print()
-#        print(f'parameter_norms:\n{self._parameter_norms}')
         self._normalize()
-#        print(f'norm = {self._norm}') 
-#RV        print('\nAfter normalization:')
-#RV        self._parameters.pretty_print()
-#        self.print_fit_report()
-#        print(f'parameter_norms:\n{self._parameter_norms}')
 
         if linear_model:
             # Perform a linear fit by direct matrix solution with numpy
             try:
                 if self._mask is None:
                     self._fit_linear_model(self._x, self._y_norm)
                 else:
-                    self._fit_linear_model(self._x[~self._mask],
-                            np.asarray(self._y_norm)[~self._mask])
+                    self._fit_linear_model(
+                        self._x[~self._mask],
+                        np.asarray(self._y_norm)[~self._mask])
             except:
                 linear_model = False
         if not linear_model:
             # Perform a non-linear fit with lmfit
             # Prevent initial values from sitting at boundaries
-            self._parameter_bounds = {name:{'min': par.min, 'max': par.max} for name, par in
-                    self._parameters.items() if par.vary}
+            self._parameter_bounds = {
+                name:{'min': par.min, 'max': par.max}
+                for name, par in self._parameters.items() if par.vary}
             for par in self._parameters.values():
                 if par.vary:
                     par.set(value=self._reset_par_at_boundary(par, par.value))
-#            print('\nAfter checking boundaries:')
-#            self._parameters.pretty_print()
 
             # Perform the fit
 #            fit_kws = None
 #            if 'Dfun' in kwargs:
 #                fit_kws = {'Dfun': kwargs.pop('Dfun')}
-#            self._result = self._model.fit(self._y_norm, self._parameters, x=self._x,
-#                    fit_kws=fit_kws, **kwargs)
+#            self._result = self._model.fit(
+#                self._y_norm, self._parameters, x=self._x, fit_kws=fit_kws,
+#                **kwargs)
             if self._mask is None:
-                self._result = self._model.fit(self._y_norm, self._parameters, x=self._x, **kwargs)
+                self._result = self._model.fit(
+                    self._y_norm, self._parameters, x=self._x, **kwargs)
             else:
-                self._result = self._model.fit(np.asarray(self._y_norm)[~self._mask],
-                        self._parameters, x=self._x[~self._mask], **kwargs)
-#RV        print('\nAfter fit:')
-#        print(f'\nself._result ({self._result}):\n\t{self._result.__dict__}')
-#RV        self._parameters.pretty_print()
-#        self.print_fit_report()
+                self._result = self._model.fit(
+                    np.asarray(self._y_norm)[~self._mask], self._parameters,
+                    x=self._x[~self._mask], **kwargs)
 
         # Set internal parameter values to fit results upon success
         if self.success:
             for name, par in self._parameters.items():
                 if par.expr is None and par.vary:
                     par.set(value=self._result.params[name].value)
-#            print('\nAfter update parameter values:')
-#            self._parameters.pretty_print()
 
         # Renormalize the data and results
         self._renormalize()
-#RV        print('\nAfter renormalization:')
-#RV        self._parameters.pretty_print()
-#        self.print_fit_report()
 
-    def plot(self, y=None, y_title=None, result=None, skip_init=False, plot_comp=True,
-            plot_comp_legends=False, plot_residual=False, plot_masked_data=True, **kwargs):
+        return None
+
+    def plot(
+            self, y=None, y_title=None, title=None, result=None,
+            skip_init=False, plot_comp=True, plot_comp_legends=False,
+            plot_residual=False, plot_masked_data=True, **kwargs):
+        """Plot the best fit."""
         if result is None:
             result = self._result
         if result is None:
             return
         plots = []
         legend = []
         if self._mask is None:
             mask = np.zeros(self._x.size).astype(bool)
             plot_masked_data = False
         else:
             mask = self._mask
         if y is not None:
             if not isinstance(y, (tuple, list, np.ndarray)):
-                illegal_value(y, 'y', 'Fit.plot')
+                logger.warning('Ignorint invalid parameter y ({y}')
             if len(y) != len(self._x):
-                logging.warning('Ignoring parameter y in Fit.plot (wrong dimension)')
+                logger.warning(
+                    'Ignoring parameter y in plot (wrong dimension)')
                 y = None
         if y is not None:
             if y_title is None or not isinstance(y_title, str):
                 y_title = 'data'
             plots += [(self._x, y, '.')]
             legend += [y_title]
         if self._y is not None:
@@ -969,114 +1083,106 @@
         if plot_comp:
             components = result.eval_components(x=self._x[~mask])
             num_components = len(components)
             if 'tmp_normalization_offset_' in components:
                 num_components -= 1
             if num_components > 1:
                 eval_index = 0
-                for modelname, y in components.items():
+                for modelname, y_comp in components.items():
                     if modelname == 'tmp_normalization_offset_':
                         continue
                     if modelname == '_eval':
                         modelname = f'eval{eval_index}'
                     if len(modelname) > 20:
                         modelname = f'{modelname[0:16]} ...'
-                    if isinstance(y, (int, float)):
-                        y *= np.ones(self._x[~mask].size)
-                    plots += [(self._x[~mask], y, '--')]
+                    if isinstance(y_comp, (int, float)):
+                        y_comp *= np.ones(self._x[~mask].size)
+                    plots += [(self._x[~mask], y_comp, '--')]
                     if plot_comp_legends:
                         if modelname[-1] == '_':
                             legend.append(modelname[:-1])
                         else:
                             legend.append(modelname)
-        title = kwargs.get('title')
-        if title is not None:
-            kwargs.pop('title')
-        quick_plot(tuple(plots), legend=legend, title=title, block=True, **kwargs)
+        quick_plot(
+            tuple(plots), legend=legend, title=title, block=True, **kwargs)
 
     @staticmethod
-    def guess_init_peak(x, y, *args, center_guess=None, use_max_for_center=True):
-        """ Return a guess for the initial height, center and fwhm for a peak
+    def guess_init_peak(
+            x, y, *args, center_guess=None, use_max_for_center=True):
+        """
+        Return a guess for the initial height, center and fwhm for a
+        single peak.
         """
-#        print(f'\n\nargs = {args}')
-#        print(f'center_guess = {center_guess}')
-#        quick_plot(x, y, vlines=center_guess, block=True)
         center_guesses = None
         x = np.asarray(x)
         y = np.asarray(y)
         if len(x) != len(y):
-            logging.error(f'Invalid x and y lengths ({len(x)}, {len(y)}), skip initial guess')
-            return(None, None, None)
+            logger.error(
+                f'Invalid x and y lengths ({len(x)}, {len(y)}), '
+                'skip initial guess')
+            return None, None, None
         if isinstance(center_guess, (int, float)):
-            if len(args):
-                logging.warning('Ignoring additional arguments for single center_guess value')
+            if args:
+                logger.warning(
+                    'Ignoring additional arguments for single center_guess '
+                    'value')
             center_guesses = [center_guess]
         elif isinstance(center_guess, (tuple, list, np.ndarray)):
             if len(center_guess) == 1:
-                logging.warning('Ignoring additional arguments for single center_guess value')
+                logger.warning(
+                    'Ignoring additional arguments for single center_guess '
+                    'value')
                 if not isinstance(center_guess[0], (int, float)):
-                    raise ValueError(f'Invalid parameter center_guess ({type(center_guess[0])})')
+                    raise ValueError(
+                        'Invalid parameter center_guess '
+                        f'({type(center_guess[0])})')
                 center_guess = center_guess[0]
             else:
                 if len(args) != 1:
-                    raise ValueError(f'Invalid number of arguments ({len(args)})')
+                    raise ValueError(
+                        f'Invalid number of arguments ({len(args)})')
                 n = args[0]
                 if not is_index(n, 0, len(center_guess)):
                     raise ValueError('Invalid argument')
                 center_guesses = center_guess
                 center_guess = center_guesses[n]
         elif center_guess is not None:
-            raise ValueError(f'Invalid center_guess type ({type(center_guess)})')
-#        print(f'x = {x}')
-#        print(f'y = {y}')
-#        print(f'center_guess = {center_guess}')
+            raise ValueError(
+                f'Invalid center_guess type ({type(center_guess)})')
 
         # Sort the inputs
         index = np.argsort(x)
         x = x[index]
         y = y[index]
         miny = y.min()
-#        print(f'miny = {miny}')
-#        print(f'x_range = {x[0]} {x[-1]} {len(x)}')
-#        print(f'y_range = {y[0]} {y[-1]} {len(y)}')
-#        quick_plot(x, y, vlines=center_guess, block=True)
 
-#        xx = x
-#        yy = y
         # Set range for current peak
-#        print(f'n = {n}')
-#        print(f'center_guesses = {center_guesses}')
         if center_guesses is not None:
             if len(center_guesses) > 1:
                 index = np.argsort(center_guesses)
                 n = list(index).index(n)
-#                print(f'n = {n}')
-#                print(f'index = {index}')
                 center_guesses = np.asarray(center_guesses)[index]
-#                print(f'center_guesses = {center_guesses}')
             if n == 0:
-               low = 0
-               upp = index_nearest(x, (center_guesses[0]+center_guesses[1])/2)
+                low = 0
+                upp = index_nearest(
+                    x, (center_guesses[0]+center_guesses[1]) / 2)
             elif n == len(center_guesses)-1:
-               low = index_nearest(x, (center_guesses[n-1]+center_guesses[n])/2)
-               upp = len(x)
-            else:
-               low = index_nearest(x, (center_guesses[n-1]+center_guesses[n])/2)
-               upp = index_nearest(x, (center_guesses[n]+center_guesses[n+1])/2)
-#            print(f'low = {low}')
-#            print(f'upp = {upp}')
+                low = index_nearest(
+                    x, (center_guesses[n-1]+center_guesses[n]) / 2)
+                upp = len(x)
+            else:
+                low = index_nearest(
+                    x, (center_guesses[n-1]+center_guesses[n]) / 2)
+                upp = index_nearest(
+                    x, (center_guesses[n]+center_guesses[n+1]) / 2)
             x = x[low:upp]
             y = y[low:upp]
-#            quick_plot(x, y, vlines=(x[0], center_guess, x[-1]), block=True)
 
-        # Estimate FHHM
+        # Estimate FWHM
         maxy = y.max()
-#        print(f'x_range = {x[0]} {x[-1]} {len(x)}')
-#        print(f'y_range = {y[0]} {y[-1]} {len(y)} {miny} {maxy}')
-#        print(f'center_guess = {center_guess}')
         if center_guess is None:
             center_index = np.argmax(y)
             center = x[center_index]
             height = maxy-miny
         else:
             if use_max_for_center:
                 center_index = np.argmax(y)
@@ -1084,60 +1190,51 @@
                 if center_index < 0.1*len(x) or center_index > 0.9*len(x):
                     center_index = index_nearest(x, center_guess)
                     center = center_guess
             else:
                 center_index = index_nearest(x, center_guess)
                 center = center_guess
             height = y[center_index]-miny
-#        print(f'center_index = {center_index}')
-#        print(f'center = {center}')
-#        print(f'height = {height}')
-        half_height = miny+0.5*height
-#        print(f'half_height = {half_height}')
+        half_height = miny + 0.5*height
         fwhm_index1 = 0
         for i in range(center_index, fwhm_index1, -1):
             if y[i] < half_height:
                 fwhm_index1 = i
                 break
-#        print(f'fwhm_index1 = {fwhm_index1} {x[fwhm_index1]}')
         fwhm_index2 = len(x)-1
         for i in range(center_index, fwhm_index2):
             if y[i] < half_height:
                 fwhm_index2 = i
                 break
-#        print(f'fwhm_index2 = {fwhm_index2} {x[fwhm_index2]}')
-#        quick_plot((x,y,'o'), vlines=(x[fwhm_index1], center, x[fwhm_index2]), block=True)
         if fwhm_index1 == 0 and fwhm_index2 < len(x)-1:
-            fwhm = 2*(x[fwhm_index2]-center)
+            fwhm = 2 * (x[fwhm_index2]-center)
         elif fwhm_index1 > 0 and fwhm_index2 == len(x)-1:
-            fwhm = 2*(center-x[fwhm_index1])
+            fwhm = 2 * (center-x[fwhm_index1])
         else:
             fwhm = x[fwhm_index2]-x[fwhm_index1]
-#        print(f'fwhm_index1 = {fwhm_index1} {x[fwhm_index1]}')
-#        print(f'fwhm_index2 = {fwhm_index2} {x[fwhm_index2]}')
-#        print(f'fwhm = {fwhm}')
-
-        # Return height, center and FWHM
-#        quick_plot((x,y,'o'), (xx,yy), vlines=(x[fwhm_index1], center, x[fwhm_index2]), block=True)
-        return(height, center, fwhm)
+
+        return height, center, fwhm
 
     def _check_linearity_model(self):
-        """Identify the linearity of all model parameters and check if the model is linear or not
+        """
+        Identify the linearity of all model parameters and check if
+        the model is linear or not.
         """
         if not self._try_linear_fit:
-            logging.info('Skip linearity check (not yet supported for callable models)')
-            return(False)
-        free_parameters = [name for name, par in self._parameters.items() if par.vary]
+            logger.info(
+                'Skip linearity check (not yet supported for callable models)')
+            return False
+        free_parameters = \
+            [name for name, par in self._parameters.items() if par.vary]
         for component in self._model.components:
             if 'tmp_normalization_offset_c' in component.param_names:
                 continue
             if isinstance(component, ExpressionModel):
                 for name in free_parameters:
                     if diff(component.expr, name, name):
-#                        print(f'\t\t{component.expr} is non-linear in {name}')
                         self._nonlinear_parameters.append(name)
                         if name in self._linear_parameters:
                             self._linear_parameters.remove(name)
             else:
                 model_parameters = component.param_names.copy()
                 for basename, hint in component.param_hints.items():
                     name = f'{component.prefix}{basename}'
@@ -1145,494 +1242,492 @@
                         model_parameters.remove(name)
                 for name in model_parameters:
                     expr = self._parameters[name].expr
                     if expr is not None:
                         for nname in free_parameters:
                             if name in self._nonlinear_parameters:
                                 if diff(expr, nname):
-#                                    print(f'\t\t{component} is non-linear in {nname} (through {name} = "{expr}")')
                                     self._nonlinear_parameters.append(nname)
                                     if nname in self._linear_parameters:
                                         self._linear_parameters.remove(nname)
                             else:
-                                assert(name in self._linear_parameters)
-#                                print(f'\n\nexpr ({type(expr)}) = {expr}\nnname ({type(nname)}) = {nname}\n\n')
+                                assert name in self._linear_parameters
                                 if diff(expr, nname, nname):
-#                                    print(f'\t\t{component} is non-linear in {nname} (through {name} = "{expr}")')
                                     self._nonlinear_parameters.append(nname)
                                     if nname in self._linear_parameters:
                                         self._linear_parameters.remove(nname)
-#        print(f'\nfree parameters:\n\t{free_parameters}')
-#        print(f'linear parameters:\n\t{self._linear_parameters}')
-#        print(f'nonlinear parameters:\n\t{self._nonlinear_parameters}\n')
-        if any(True for name in self._nonlinear_parameters if self._parameters[name].vary):
-            return(False)
-        return(True)
+        if any(True for name in self._nonlinear_parameters
+                if self._parameters[name].vary):
+            return False
+        return True
 
     def _fit_linear_model(self, x, y):
-        """Perform a linear fit by direct matrix solution with numpy
         """
+        Perform a linear fit by direct matrix solution with numpy.
+        """
+        # Third party modules
+        from asteval import Interpreter
+
         # Construct the matrix and the free parameter vector
-#        print(f'\nparameters:')
-#        self._parameters.pretty_print()
-#        print(f'\nparameter_norms:\n\t{self._parameter_norms}')
-#        print(f'\nlinear_parameters:\n\t{self._linear_parameters}')
-#        print(f'nonlinear_parameters:\n\t{self._nonlinear_parameters}')
-        free_parameters = [name for name, par in self._parameters.items() if par.vary]
-#        print(f'free parameters:\n\t{free_parameters}\n')
-        expr_parameters = {name:par.expr for name, par in self._parameters.items()
-                if par.expr is not None}
+        free_parameters = \
+            [name for name, par in self._parameters.items() if par.vary]
+        expr_parameters = {
+            name:par.expr for name, par in self._parameters.items()
+            if par.expr is not None}
         model_parameters = []
         for component in self._model.components:
             if 'tmp_normalization_offset_c' in component.param_names:
                 continue
             model_parameters += component.param_names
             for basename, hint in component.param_hints.items():
                 name = f'{component.prefix}{basename}'
                 if hint.get('expr') is not None:
                     expr_parameters.pop(name)
                     model_parameters.remove(name)
-#        print(f'expr parameters:\n{expr_parameters}')
-#        print(f'model parameters:\n\t{model_parameters}\n')
         norm = 1.0
         if self._normalized:
             norm = self._norm[1]
-#        print(f'\n\nself._normalized = {self._normalized}\nnorm = {norm}\nself._norm = {self._norm}\n')
         # Add expression parameters to asteval
         ast = Interpreter()
-#        print(f'Adding to asteval sym table:')
         for name, expr in expr_parameters.items():
-#            print(f'\tadding {name} {expr}')
             ast.symtable[name] = expr
         # Add constant parameters to asteval
-        # (renormalize to use correctly in evaluation of expression models)
+        # (renormalize to use correctly in evaluation of expression
+        #     models)
         for name, par in self._parameters.items():
             if par.expr is None and not par.vary:
                 if self._parameter_norms[name]:
-#                    print(f'\tadding {name} {par.value*norm}')
                     ast.symtable[name] = par.value*norm
                 else:
-#                    print(f'\tadding {name} {par.value}')
                     ast.symtable[name] = par.value
-        A = np.zeros((len(x), len(free_parameters)), dtype='float64')
+        mat_a = np.zeros((len(x), len(free_parameters)), dtype='float64')
         y_const = np.zeros(len(x), dtype='float64')
         have_expression_model = False
         for component in self._model.components:
             if isinstance(component, ConstantModel):
                 name = component.param_names[0]
-#                print(f'\nConstant model: {name} {self._parameters[name]}\n')
                 if name in free_parameters:
-#                    print(f'\t\t{name} is a free constant set matrix column {free_parameters.index(name)} to 1.0')
-                    A[:,free_parameters.index(name)] = 1.0
+                    mat_a[:,free_parameters.index(name)] = 1.0
                 else:
                     if self._parameter_norms[name]:
-                        delta_y_const = self._parameters[name]*np.ones(len(x))
+                        delta_y_const = \
+                            self._parameters[name] * np.ones(len(x))
                     else:
-                        delta_y_const = (self._parameters[name]*norm)*np.ones(len(x))
+                        delta_y_const = \
+                            (self._parameters[name]*norm) * np.ones(len(x))
                     y_const += delta_y_const
-#                    print(f'\ndelta_y_const ({type(delta_y_const)}):\n{delta_y_const}\n')
             elif isinstance(component, ExpressionModel):
                 have_expression_model = True
                 const_expr = component.expr
-#                print(f'\nExpression model:\nconst_expr: {const_expr}\n')
                 for name in free_parameters:
                     dexpr_dname = diff(component.expr, name)
                     if dexpr_dname:
-                        const_expr = f'{const_expr}-({str(dexpr_dname)})*{name}'
-#                        print(f'\tconst_expr: {const_expr}')
+                        const_expr = \
+                            f'{const_expr}-({str(dexpr_dname)})*{name}'
                         if not self._parameter_norms[name]:
                             dexpr_dname = f'({dexpr_dname})/{norm}'
-#                        print(f'\t{component.expr} is linear in {name}\n\t\tadd "{str(dexpr_dname)}" to matrix as column {free_parameters.index(name)}')
-                        fx = [(lambda _: ast.eval(str(dexpr_dname)))(ast(f'x={v}')) for v in x]
-#                        print(f'\tfx:\n{fx}')
-                        if len(ast.error):
-                            raise ValueError(f'Unable to evaluate {dexpr_dname}')
-                        A[:,free_parameters.index(name)] += fx
-#                        if self._parameter_norms[name]:
-#                            print(f'\t\t{component.expr} is linear in {name} add "{str(dexpr_dname)}" to matrix as column {free_parameters.index(name)}')
-#                            A[:,free_parameters.index(name)] += fx
-#                        else:
-#                            print(f'\t\t{component.expr} is linear in {name} add "({str(dexpr_dname)})/{norm}" to matrix as column {free_parameters.index(name)}')
-#                            A[:,free_parameters.index(name)] += np.asarray(fx)/norm
-                # FIX: find another solution if expr not supported by simplify
+                        y_expr = [(lambda _: ast.eval(str(dexpr_dname)))
+                                  (ast(f'x={v}')) for v in x]
+                        if ast.error:
+                            raise ValueError(
+                                f'Unable to evaluate {dexpr_dname}')
+                        mat_a[:,free_parameters.index(name)] += y_expr
+                # RV find another solution if expr not supported by
+                #     simplify
                 const_expr = str(simplify(f'({const_expr})/{norm}'))
-#                print(f'\nconst_expr: {const_expr}')
-                delta_y_const = [(lambda _: ast.eval(const_expr))(ast(f'x = {v}')) for v in x]
+                delta_y_const = [(lambda _: ast.eval(const_expr))
+                                 (ast(f'x = {v}')) for v in x]
                 y_const += delta_y_const
-#                print(f'\ndelta_y_const ({type(delta_y_const)}):\n{delta_y_const}\n')
-                if len(ast.error):
+                if ast.error:
                     raise ValueError(f'Unable to evaluate {const_expr}')
             else:
-                free_model_parameters = [name for name in component.param_names
-                        if name in free_parameters or name in expr_parameters]
-#                print(f'\nBuild-in model ({component}):\nfree_model_parameters: {free_model_parameters}\n')
-                if not len(free_model_parameters):
+                free_model_parameters = [
+                    name for name in component.param_names
+                    if name in free_parameters or name in expr_parameters]
+                if not free_model_parameters:
                     y_const += component.eval(params=self._parameters, x=x)
                 elif isinstance(component, LinearModel):
-                    if f'{component.prefix}slope' in free_model_parameters:
-                        A[:,free_parameters.index(f'{component.prefix}slope')] = x
+                    name = f'{component.prefix}slope'
+                    if name in free_model_parameters:
+                        mat_a[:,free_parameters.index(name)] = x
                     else:
-                        y_const += self._parameters[f'{component.prefix}slope'].value*x
-                    if f'{component.prefix}intercept' in free_model_parameters:
-                        A[:,free_parameters.index(f'{component.prefix}intercept')] = 1.0
+                        y_const += self._parameters[name].value * x
+                    name = f'{component.prefix}intercept'
+                    if name in free_model_parameters:
+                        mat_a[:,free_parameters.index(name)] = 1.0
                     else:
-                        y_const += self._parameters[f'{component.prefix}intercept'].value* \
-                                np.ones(len(x))
+                        y_const += self._parameters[name].value \
+                            * np.ones(len(x))
                 elif isinstance(component, QuadraticModel):
-                    if f'{component.prefix}a' in free_model_parameters:
-                        A[:,free_parameters.index(f'{component.prefix}a')] = x**2
+                    name = f'{component.prefix}a'
+                    if name in free_model_parameters:
+                        mat_a[:,free_parameters.index(name)] = x**2
                     else:
-                        y_const += self._parameters[f'{component.prefix}a'].value*x**2
-                    if f'{component.prefix}b' in free_model_parameters:
-                        A[:,free_parameters.index(f'{component.prefix}b')] = x
+                        y_const += self._parameters[name].value * x**2
+                    name = f'{component.prefix}b'
+                    if name in free_model_parameters:
+                        mat_a[:,free_parameters.index(name)] = x
                     else:
-                        y_const += self._parameters[f'{component.prefix}b'].value*x
-                    if f'{component.prefix}c' in free_model_parameters:
-                        A[:,free_parameters.index(f'{component.prefix}c')] = 1.0
+                        y_const += self._parameters[name].value * x
+                    name = f'{component.prefix}c'
+                    if name in free_model_parameters:
+                        mat_a[:,free_parameters.index(name)] = 1.0
                     else:
-                        y_const += self._parameters[f'{component.prefix}c'].value*np.ones(len(x))
+                        y_const += self._parameters[name].value \
+                            * np.ones(len(x))
                 else:
-                    # At this point each build-in model must be strictly proportional to each linear
-                    #   model parameter. Without this assumption, the model equation is needed
-                    #   For the current build-in lmfit models, this can only ever be the amplitude
-                    assert(len(free_model_parameters) == 1)
+                    # At this point each build-in model must be
+                    #     strictly proportional to each linear model
+                    #     parameter. Without this assumption, the model
+                    #     equation is needed
+                    # For the current build-in lmfit models, this can
+                    #     only ever be the amplitude
+                    assert len(free_model_parameters) == 1
                     name = f'{component.prefix}amplitude'
-                    assert(free_model_parameters[0] == name)
-                    assert(self._parameter_norms[name])
+                    assert free_model_parameters[0] == name
+                    assert self._parameter_norms[name]
                     expr = self._parameters[name].expr
                     if expr is None:
-#                        print(f'\t{component} is linear in {name} add to matrix as column {free_parameters.index(name)}')
                         parameters = deepcopy(self._parameters)
                         parameters[name].set(value=1.0)
-                        index = free_parameters.index(name)
-                        A[:,free_parameters.index(name)] += component.eval(params=parameters, x=x)
+                        mat_a[:,free_parameters.index(name)] += component.eval(
+                            params=parameters, x=x)
                     else:
                         const_expr = expr
-#                        print(f'\tconst_expr: {const_expr}')
                         parameters = deepcopy(self._parameters)
                         parameters[name].set(value=1.0)
                         dcomp_dname = component.eval(params=parameters, x=x)
-#                        print(f'\tdcomp_dname ({type(dcomp_dname)}):\n{dcomp_dname}')
                         for nname in free_parameters:
-                            dexpr_dnname =  diff(expr, nname)
+                            dexpr_dnname = diff(expr, nname)
                             if dexpr_dnname:
-                                assert(self._parameter_norms[name])
-#                                print(f'\t\td({expr})/d{nname} = {dexpr_dnname}')
-#                                print(f'\t\t{component} is linear in {nname} (through {name} = "{expr}", add to matrix as column {free_parameters.index(nname)})')
-                                fx = np.asarray(dexpr_dnname*dcomp_dname, dtype='float64')
-#                                print(f'\t\tfx ({type(fx)}): {fx}')
-#                                print(f'free_parameters.index({nname}): {free_parameters.index(nname)}')
+                                assert self._parameter_norms[name]
+                                y_expr = np.asarray(
+                                    dexpr_dnname*dcomp_dname, dtype='float64')
                                 if self._parameter_norms[nname]:
-                                    A[:,free_parameters.index(nname)] += fx
+                                    mat_a[:,free_parameters.index(nname)] += \
+                                        y_expr
                                 else:
-                                    A[:,free_parameters.index(nname)] += fx/norm
-                                const_expr = f'{const_expr}-({dexpr_dnname})*{nname}'
-#                                print(f'\t\tconst_expr: {const_expr}')
+                                    mat_a[:,free_parameters.index(nname)] += \
+                                        y_expr/norm
+                                const_expr = \
+                                    f'{const_expr}-({dexpr_dnname})*{nname}'
                         const_expr = str(simplify(f'({const_expr})/{norm}'))
-#                        print(f'\tconst_expr: {const_expr}')
-                        fx = [(lambda _: ast.eval(const_expr))(ast(f'x = {v}')) for v in x]
-#                        print(f'\tfx: {fx}')
-                        delta_y_const = np.multiply(fx, dcomp_dname)
+                        y_expr = [
+                            (lambda _: ast.eval(const_expr))(ast(f'x = {v}'))
+                            for v in x]
+                        delta_y_const = np.multiply(y_expr, dcomp_dname)
                         y_const += delta_y_const
-#                        print(f'\ndelta_y_const ({type(delta_y_const)}):\n{delta_y_const}\n')
-#            print(A)
-#            print(y_const)
-        solution, residual, rank, s = np.linalg.lstsq(A, y-y_const, rcond=None)
-#        print(f'\nsolution ({type(solution)} {solution.shape}):\n\t{solution}')
-#        print(f'\nresidual ({type(residual)} {residual.shape}):\n\t{residual}')
-#        print(f'\nrank ({type(rank)} {rank.shape}):\n\t{rank}')
-#        print(f'\ns ({type(s)} {s.shape}):\n\t{s}\n')
+        solution, _, _, _ = np.linalg.lstsq(
+            mat_a, y-y_const, rcond=None)
 
-        # Assemble result (compensate for normalization in expression models)
+        # Assemble result
+        # (compensate for normalization in expression models)
         for name, value in zip(free_parameters, solution):
             self._parameters[name].set(value=value)
-        if self._normalized and (have_expression_model or len(expr_parameters)):
+        if (self._normalized
+                and (have_expression_model or expr_parameters)):
             for name, norm in self._parameter_norms.items():
                 par = self._parameters[name]
                 if par.expr is None and norm:
                     self._parameters[name].set(value=par.value*self._norm[1])
-#        self._parameters.pretty_print()
-#        print(f'\nself._parameter_norms:\n\t{self._parameter_norms}')
         self._result = ModelResult(self._model, deepcopy(self._parameters))
         self._result.best_fit = self._model.eval(params=self._parameters, x=x)
-        if self._normalized and (have_expression_model or len(expr_parameters)):
+        if (self._normalized
+                and (have_expression_model or expr_parameters)):
             if 'tmp_normalization_offset_c' in self._parameters:
                 offset = self._parameters['tmp_normalization_offset_c']
             else:
                 offset = 0.0
-            self._result.best_fit = (self._result.best_fit-offset-self._norm[0])/self._norm[1]
+            self._result.best_fit = \
+                (self._result.best_fit-offset-self._norm[0]) / self._norm[1]
             if self._normalized:
                 for name, norm in self._parameter_norms.items():
                     par = self._parameters[name]
                     if par.expr is None and norm:
                         value = par.value/self._norm[1]
                         self._parameters[name].set(value=value)
                         self._result.params[name].set(value=value)
-#        self._parameters.pretty_print()
         self._result.residual = self._result.best_fit-y
         self._result.components = self._model.components
         self._result.init_params = None
-#        quick_plot((x, y, '.'), (x, y_const, 'g'), (x, self._result.best_fit, 'k'), (x, self._result.residual, 'r'), block=True)
 
     def _normalize(self):
-        """Normalize the data and initial parameters
-        """
+        """Normalize the data and initial parameters."""
         if self._normalized:
             return
         if self._norm is None:
             if self._y is not None and self._y_norm is None:
                 self._y_norm = np.asarray(self._y)
         else:
             if self._y is not None and self._y_norm is None:
-                self._y_norm = (np.asarray(self._y)-self._norm[0])/self._norm[1]
+                self._y_norm = \
+                    (np.asarray(self._y)-self._norm[0]) / self._norm[1]
             self._y_range = 1.0
             for name, norm in self._parameter_norms.items():
                 par = self._parameters[name]
                 if par.expr is None and norm:
                     value = par.value/self._norm[1]
                     _min = par.min
                     _max = par.max
-                    if not np.isinf(_min) and abs(_min) != float_min:
+                    if not np.isinf(_min) and abs(_min) != FLOAT_MIN:
                         _min /= self._norm[1]
-                    if not np.isinf(_max) and abs(_max) != float_min:
+                    if not np.isinf(_max) and abs(_max) != FLOAT_MIN:
                         _max /= self._norm[1]
                     par.set(value=value, min=_min, max=_max)
             self._normalized = True
 
     def _renormalize(self):
-        """Renormalize the data and results
-        """
+        """Renormalize the data and results."""
         if self._norm is None or not self._normalized:
             return
         self._normalized = False
         for name, norm in self._parameter_norms.items():
             par = self._parameters[name]
             if par.expr is None and norm:
                 value = par.value*self._norm[1]
                 _min = par.min
                 _max = par.max
-                if not np.isinf(_min) and abs(_min) != float_min:
+                if not np.isinf(_min) and abs(_min) != FLOAT_MIN:
                     _min *= self._norm[1]
-                if not np.isinf(_max) and abs(_max) != float_min:
+                if not np.isinf(_max) and abs(_max) != FLOAT_MIN:
                     _max *= self._norm[1]
                 par.set(value=value, min=_min, max=_max)
         if self._result is None:
             return
-        self._result.best_fit = self._result.best_fit*self._norm[1]+self._norm[0]
+        self._result.best_fit = (
+            self._result.best_fit*self._norm[1] + self._norm[0])
         for name, par in self._result.params.items():
             if self._parameter_norms.get(name, False):
                 if par.stderr is not None:
                     par.stderr *= self._norm[1]
                 if par.expr is None:
                     _min = par.min
                     _max = par.max
                     value = par.value*self._norm[1]
                     if par.init_value is not None:
                         par.init_value *= self._norm[1]
-                    if not np.isinf(_min) and abs(_min) != float_min:
+                    if not np.isinf(_min) and abs(_min) != FLOAT_MIN:
                         _min *= self._norm[1]
-                    if not np.isinf(_max) and abs(_max) != float_min:
+                    if not np.isinf(_max) and abs(_max) != FLOAT_MIN:
                         _max *= self._norm[1]
                     par.set(value=value, min=_min, max=_max)
         if hasattr(self._result, 'init_fit'):
-            self._result.init_fit = self._result.init_fit*self._norm[1]+self._norm[0]
+            self._result.init_fit = (
+                self._result.init_fit*self._norm[1] + self._norm[0])
         if hasattr(self._result, 'init_values'):
             init_values = {}
             for name, value in self._result.init_values.items():
-                if name not in self._parameter_norms or self._parameters[name].expr is not None:
+                if (name not in self._parameter_norms
+                        or self._parameters[name].expr is not None):
                     init_values[name] = value
                 elif self._parameter_norms[name]:
                     init_values[name] = value*self._norm[1]
             self._result.init_values = init_values
             for name, par in self._result.init_params.items():
                 if par.expr is None and self._parameter_norms.get(name, False):
                     value = par.value
                     _min = par.min
                     _max = par.max
                     value *= self._norm[1]
-                    if not np.isinf(_min) and abs(_min) != float_min:
+                    if not np.isinf(_min) and abs(_min) != FLOAT_MIN:
                         _min *= self._norm[1]
-                    if not np.isinf(_max) and abs(_max) != float_min:
+                    if not np.isinf(_max) and abs(_max) != FLOAT_MIN:
                         _max *= self._norm[1]
                     par.set(value=value, min=_min, max=_max)
                 par.init_value = par.value
-        # Don't renormalize chisqr, it has no useful meaning in physical units
-        #self._result.chisqr *= self._norm[1]*self._norm[1]
+        # Don't renormalize chisqr, it has no useful meaning in
+        #     physical units
+#        self._result.chisqr *= self._norm[1]*self._norm[1]
         if self._result.covar is not None:
             for i, name in enumerate(self._result.var_names):
                 if self._parameter_norms.get(name, False):
                     for j in range(len(self._result.var_names)):
                         if self._result.covar[i,j] is not None:
                             self._result.covar[i,j] *= self._norm[1]
                         if self._result.covar[j,i] is not None:
                             self._result.covar[j,i] *= self._norm[1]
-        # Don't renormalize redchi, it has no useful meaning in physical units
-        #self._result.redchi *= self._norm[1]*self._norm[1]
+        # Don't renormalize redchi, it has no useful meaning in
+        #     physical units
+#        self._result.redchi *= self._norm[1]*self._norm[1]
         if self._result.residual is not None:
             self._result.residual *= self._norm[1]
 
     def _reset_par_at_boundary(self, par, value):
-        assert(par.vary)
+        assert par.vary
         name = par.name
         _min = self._parameter_bounds[name]['min']
         _max = self._parameter_bounds[name]['max']
         if np.isinf(_min):
             if not np.isinf(_max):
                 if self._parameter_norms.get(name, False):
                     upp = _max-0.1*self._y_range
                 elif _max == 0.0:
                     upp = _max-0.1
                 else:
                     upp = _max-0.1*abs(_max)
                 if value >= upp:
-                    return(upp)
+                    return upp
         else:
             if np.isinf(_max):
                 if self._parameter_norms.get(name, False):
-                    low = _min+0.1*self._y_range
+                    low = _min + 0.1*self._y_range
                 elif _min == 0.0:
                     low = _min+0.1
                 else:
-                    low = _min+0.1*abs(_min)
+                    low = _min + 0.1*abs(_min)
                 if value <= low:
-                    return(low)
+                    return low
             else:
-                low = 0.9*_min+0.1*_max
-                upp = 0.1*_min+0.9*_max
+                low = 0.9*_min + 0.1*_max
+                upp = 0.1*_min + 0.9*_max
                 if value <= low:
-                    return(low)
-                elif value >= upp:
-                    return(upp)
-        return(value)
+                    return low
+                if value >= upp:
+                    return upp
+        return value
 
 
 class FitMultipeak(Fit):
-    """Fit data with multiple peaks
+    """
+    Wrapper to the Fit class to fit data with multiple peaks
     """
     def __init__(self, y, x=None, normalize=True):
+        """Initialize FitMultipeak."""
         super().__init__(y, x=x, normalize=normalize)
         self._fwhm_max = None
         self._sigma_max = None
 
     @classmethod
-    def fit_multipeak(cls, y, centers, x=None, normalize=True, peak_models='gaussian',
+    def fit_multipeak(
+            cls, y, centers, x=None, normalize=True, peak_models='gaussian',
             center_exprs=None, fit_type=None, background=None, fwhm_max=None,
             print_report=False, plot=False, x_eval=None):
-        """Make sure that centers and fwhm_max are in the correct units and consistent with expr
-           for a uniform fit (fit_type == 'uniform')
+        """Class method for FitMultipeak.
+
+        Make sure that centers and fwhm_max are in the correct units
+        and consistent with expr for a uniform fit (fit_type ==
+        'uniform').
         """
-        if x_eval is not None and not isinstance(x_eval, (tuple, list, np.ndarray)):
+        if (x_eval is not None
+                and not isinstance(x_eval, (tuple, list, np.ndarray))):
             raise ValueError(f'Invalid parameter x_eval ({x_eval})')
         fit = cls(y, x=x, normalize=normalize)
-        success = fit.fit(centers, fit_type=fit_type, peak_models=peak_models, fwhm_max=fwhm_max,
-                center_exprs=center_exprs, background=background, print_report=print_report,
-                plot=plot)
+        success = fit.fit(
+            centers=centers, fit_type=fit_type, peak_models=peak_models,
+            fwhm_max=fwhm_max, center_exprs=center_exprs,
+            background=background, print_report=print_report, plot=plot)
         if x_eval is None:
             best_fit = fit.best_fit
         else:
             best_fit = fit.eval(x_eval)
         if success:
-            return(best_fit, fit.residual, fit.best_values, fit.best_errors, fit.redchi, \
-                    fit.success)
-        else:
-            return(np.array([]), np.array([]), {}, {}, float_max, False)
-
-    def fit(self, centers, fit_type=None, peak_models=None, center_exprs=None, fwhm_max=None,
-                background=None, print_report=False, plot=True, param_constraint=False):
+            return (
+                best_fit, fit.residual, fit.best_values, fit.best_errors,
+                fit.redchi, fit.success)
+        return np.array([]), np.array([]), {}, {}, FLOAT_MAX, False
+
+    def fit(
+            self, centers=None, fit_type=None, peak_models=None,
+            center_exprs=None, fwhm_max=None, background=None,
+            print_report=False, plot=True, param_constraint=False, **kwargs):
+        """Fit the model to the input data."""
+        if centers is None:
+            raise ValueError('Missing required parameter centers')
+        if not isinstance(centers, (int, float, tuple, list, np.ndarray)):
+            raise ValueError(f'Invalid parameter centers ({centers})')
         self._fwhm_max = fwhm_max
-        # Create the multipeak model
-        self._create_model(centers, fit_type, peak_models, center_exprs, background,
-                param_constraint)
-
-        # RV: Obsolete Normalize the data and results
-#        print('\nBefore fit before normalization in FitMultipeak:')
-#        self._parameters.pretty_print()
-#        self._normalize()
-#        print('\nBefore fit after normalization in FitMultipeak:')
-#        self._parameters.pretty_print()
+        self._create_model(
+            centers, fit_type, peak_models, center_exprs, background,
+            param_constraint)
 
         # Perform the fit
         try:
             if param_constraint:
-                super().fit(fit_kws={'xtol': 1.e-5, 'ftol': 1.e-5, 'gtol': 1.e-5})
+                super().fit(
+                    fit_kws={'xtol': 1.e-5, 'ftol': 1.e-5, 'gtol': 1.e-5})
             else:
                 super().fit()
         except:
-            return(False)
+            return False
 
         # Check for valid fit parameter results
         fit_failure = self._check_validity()
         success = True
         if fit_failure:
             if param_constraint:
-                logging.warning('  -> Should not happen with param_constraint set, fail the fit')
+                logger.warning(
+                    '  -> Should not happen with param_constraint set, '
+                    'fail the fit')
                 success = False
             else:
-                logging.info('  -> Retry fitting with constraints')
-                self.fit(centers, fit_type, peak_models, center_exprs, fwhm_max=fwhm_max,
-                        background=background, print_report=print_report, plot=plot,
-                        param_constraint=True)
-        else:
-            # RV: Obsolete Renormalize the data and results
-#            print('\nAfter fit before renormalization in FitMultipeak:')
-#            self._parameters.pretty_print()
-#            self.print_fit_report()
-#            self._renormalize()
-#            print('\nAfter fit after renormalization in FitMultipeak:')
-#            self._parameters.pretty_print()
-#            self.print_fit_report()
-
+                logger.info('  -> Retry fitting with constraints')
+                self.fit(
+                    centers, fit_type, peak_models, center_exprs,
+                    fwhm_max=fwhm_max, background=background,
+                    print_report=print_report, plot=plot,
+                    param_constraint=True)
+        else:
             # Print report and plot components if requested
             if print_report:
                 self.print_fit_report()
             if plot:
-                self.plot(skip_init=True, plot_comp=True, plot_comp_legends=True,
-                        plot_residual=True)
-
-        return(success)
+                self.plot(
+                    skip_init=True, plot_comp=True, plot_comp_legends=True,
+                    plot_residual=True)
+
+        return success
+
+    def _create_model(
+            self, centers, fit_type=None, peak_models=None, center_exprs=None,
+            background=None, param_constraint=False):
+        """Create the multipeak model."""
+        # Third party modules
+        from asteval import Interpreter
 
-    def _create_model(self, centers, fit_type=None, peak_models=None, center_exprs=None,
-                background=None, param_constraint=False):
-        """Create the multipeak model
-        """
         if isinstance(centers, (int, float)):
             centers = [centers]
         num_peaks = len(centers)
         if peak_models is None:
             peak_models = num_peaks*['gaussian']
-        elif isinstance(peak_models, str) and peak_models in ('gaussian', 'lorentzian'):
+        elif (isinstance(peak_models, str)
+                and peak_models in ('gaussian', 'lorentzian')):
             peak_models = num_peaks*[peak_models]
         else:
-            raise ValueError(f'Invalid peak model parameter ({peak_models})')
+            raise ValueError(f'Invalid parameter peak model ({peak_models})')
         if len(peak_models) != num_peaks:
-            raise ValueError(f'Inconsistent number of peaks in peak_models ({len(peak_models)} vs '+
-                    f'{num_peaks})')
+            raise ValueError(
+                'Inconsistent number of peaks in peak_models '
+                f'({len(peak_models)} vs {num_peaks})')
         if num_peaks == 1:
             if fit_type is not None:
-                logging.debug('Ignoring fit_type input for fitting one peak')
+                logger.debug('Ignoring fit_type input for fitting one peak')
             fit_type = None
             if center_exprs is not None:
-                logging.debug('Ignoring center_exprs input for fitting one peak')
+                logger.debug(
+                    'Ignoring center_exprs input for fitting one peak')
                 center_exprs = None
         else:
             if fit_type == 'uniform':
                 if center_exprs is None:
                     center_exprs = [f'scale_factor*{cen}' for cen in centers]
                 if len(center_exprs) != num_peaks:
-                    raise ValueError(f'Inconsistent number of peaks in center_exprs '+
-                            f'({len(center_exprs)} vs {num_peaks})')
+                    raise ValueError(
+                        'Inconsistent number of peaks in center_exprs '
+                        f'({len(center_exprs)} vs {num_peaks})')
             elif fit_type == 'unconstrained' or fit_type is None:
                 if center_exprs is not None:
-                    logging.warning('Ignoring center_exprs input for unconstrained fit')
+                    logger.warning(
+                        'Ignoring center_exprs input for unconstrained fit')
                     center_exprs = None
             else:
-                raise ValueError(f'Invalid fit_type in fit_multigaussian {fit_type}')
+                raise ValueError(
+                    f'Invalid parameter fit_type ({fit_type})')
         self._sigma_max = None
         if param_constraint:
-            min_value = float_min
+            min_value = FLOAT_MIN
             if self._fwhm_max is not None:
                 self._sigma_max = np.zeros(num_peaks)
         else:
             min_value = None
 
         # Reset the fit
         self._model = None
@@ -1644,113 +1739,143 @@
             if isinstance(background, dict):
                 background = [background]
             if isinstance(background, str):
                 self.add_model(background, prefix='bkgd_')
             elif is_dict_series(background):
                 for model in deepcopy(background):
                     if 'model' not in model:
-                        raise KeyError(f'Missing keyword "model" in model in background ({model})')
+                        raise KeyError(
+                            'Missing keyword "model" in model in background '
+                            f'({model})')
                     name = model.pop('model')
-                    parameters=model.pop('parameters', None)
-                    self.add_model(name, prefix=f'bkgd_{name}_', parameters=parameters, **model)
+                    parameters = model.pop('parameters', None)
+                    self.add_model(
+                        name, prefix=f'bkgd_{name}_', parameters=parameters,
+                        **model)
             else:
-                raise ValueError(f'Invalid parameter background ({background})')
+                raise ValueError(
+                    f'Invalid parameter background ({background})')
 
         # Add peaks and guess initial fit parameters
         ast = Interpreter()
         if num_peaks == 1:
-            height_init, cen_init, fwhm_init = self.guess_init_peak(self._x, self._y)
+            height_init, cen_init, fwhm_init = self.guess_init_peak(
+                self._x, self._y)
             if self._fwhm_max is not None and fwhm_init > self._fwhm_max:
                 fwhm_init = self._fwhm_max
             ast(f'fwhm = {fwhm_init}')
             ast(f'height = {height_init}')
             sig_init = ast(fwhm_factor[peak_models[0]])
             amp_init = ast(height_factor[peak_models[0]])
             sig_max = None
             if self._sigma_max is not None:
                 ast(f'fwhm = {self._fwhm_max}')
                 sig_max = ast(fwhm_factor[peak_models[0]])
                 self._sigma_max[0] = sig_max
-            self.add_model(peak_models[0], parameters=(
+            self.add_model(
+                peak_models[0],
+                parameters=(
                     {'name': 'amplitude', 'value': amp_init, 'min': min_value},
                     {'name': 'center', 'value': cen_init, 'min': min_value},
-                    {'name': 'sigma', 'value': sig_init, 'min': min_value, 'max': sig_max}))
+                    {'name': 'sigma', 'value': sig_init, 'min': min_value,
+                     'max': sig_max},
+                ))
         else:
             if fit_type == 'uniform':
                 self.add_parameter(name='scale_factor', value=1.0)
             for i in range(num_peaks):
-                height_init, cen_init, fwhm_init = self.guess_init_peak(self._x, self._y, i,
-                        center_guess=centers)
+                height_init, cen_init, fwhm_init = self.guess_init_peak(
+                    self._x, self._y, i, center_guess=centers)
                 if self._fwhm_max is not None and fwhm_init > self._fwhm_max:
                     fwhm_init = self._fwhm_max
                 ast(f'fwhm = {fwhm_init}')
                 ast(f'height = {height_init}')
                 sig_init = ast(fwhm_factor[peak_models[i]])
                 amp_init = ast(height_factor[peak_models[i]])
                 sig_max = None
                 if self._sigma_max is not None:
                     ast(f'fwhm = {self._fwhm_max}')
                     sig_max = ast(fwhm_factor[peak_models[i]])
                     self._sigma_max[i] = sig_max
                 if fit_type == 'uniform':
-                    self.add_model(peak_models[i], prefix=f'peak{i+1}_', parameters=(
-                            {'name': 'amplitude', 'value': amp_init, 'min': min_value},
+                    self.add_model(
+                        peak_models[i], prefix=f'peak{i+1}_',
+                        parameters=(
+                            {'name': 'amplitude', 'value': amp_init,
+                             'min': min_value},
                             {'name': 'center', 'expr': center_exprs[i]},
-                            {'name': 'sigma', 'value': sig_init, 'min': min_value,
-                            'max': sig_max}))
+                            {'name': 'sigma', 'value': sig_init,
+                             'min': min_value, 'max': sig_max},
+                        ))
                 else:
-                    self.add_model('gaussian', prefix=f'peak{i+1}_', parameters=(
-                            {'name': 'amplitude', 'value': amp_init, 'min': min_value},
-                            {'name': 'center', 'value': cen_init, 'min': min_value},
-                            {'name': 'sigma', 'value': sig_init, 'min': min_value,
-                            'max': sig_max}))
+                    self.add_model(
+                        'gaussian',
+                        prefix=f'peak{i+1}_',
+                        parameters=(
+                            {'name': 'amplitude', 'value': amp_init,
+                             'min': min_value},
+                            {'name': 'center', 'value': cen_init,
+                             'min': min_value},
+                            {'name': 'sigma', 'value': sig_init,
+                             'min': min_value, 'max': sig_max},
+                        ))
 
     def _check_validity(self):
-        """Check for valid fit parameter results
-        """
+        """Check for valid fit parameter results."""
         fit_failure = False
-        index = compile(r'\d+')
-        for name, par in self.best_parameters.items():
+        index = re_compile(r'\d+')
+        for name, par in self.best_parameters().items():
             if 'bkgd' in name:
-#                if ((name == 'bkgd_c' and par['value'] <= 0.0) or
-#                        (name.endswith('amplitude') and par['value'] <= 0.0) or
-                 if ((name.endswith('amplitude') and par['value'] <= 0.0) or
-                        (name.endswith('decay') and par['value'] <= 0.0)):
-                    logging.info(f'Invalid fit result for {name} ({par["value"]})')
+                if ((name.endswith('amplitude') and par['value'] <= 0.0)
+                        or (name.endswith('decay') and par['value'] <= 0.0)):
+                    logger.info(
+                        f'Invalid fit result for {name} ({par["value"]})')
                     fit_failure = True
-            elif (((name.endswith('amplitude') or name.endswith('height')) and
-                    par['value'] <= 0.0) or
-                    ((name.endswith('sigma') or name.endswith('fwhm')) and par['value'] <= 0.0) or
-                    (name.endswith('center') and par['value'] <= 0.0) or
-                    (name == 'scale_factor' and par['value'] <= 0.0)):
-                logging.info(f'Invalid fit result for {name} ({par["value"]})')
+            elif (((name.endswith('amplitude') or name.endswith('height'))
+                    and par['value'] <= 0.0)
+                    or ((name.endswith('sigma') or name.endswith('fwhm'))
+                        and par['value'] <= 0.0)
+                    or (name.endswith('center') and par['value'] <= 0.0)
+                    or (name == 'scale_factor' and par['value'] <= 0.0)):
+                logger.info(f'Invalid fit result for {name} ({par["value"]})')
                 fit_failure = True
-            if 'bkgd' not in name and name.endswith('sigma') and self._sigma_max is not None:
+            if ('bkgd' not in name and name.endswith('sigma')
+                    and self._sigma_max is not None):
                 if name == 'sigma':
                     sigma_max = self._sigma_max[0]
                 else:
-                    sigma_max = self._sigma_max[int(index.search(name).group())-1]
+                    sigma_max = self._sigma_max[
+                        int(index.search(name).group())-1]
                 if par['value'] > sigma_max:
-                    logging.info(f'Invalid fit result for {name} ({par["value"]})')
+                    logger.info(
+                        f'Invalid fit result for {name} ({par["value"]})')
                     fit_failure = True
                 elif par['value'] == sigma_max:
-                    logging.warning(f'Edge result on for {name} ({par["value"]})')
-            if 'bkgd' not in name and name.endswith('fwhm') and self._fwhm_max is not None:
+                    logger.warning(
+                        f'Edge result on for {name} ({par["value"]})')
+            if ('bkgd' not in name and name.endswith('fwhm')
+                    and self._fwhm_max is not None):
                 if par['value'] > self._fwhm_max:
-                    logging.info(f'Invalid fit result for {name} ({par["value"]})')
+                    logger.info(
+                        f'Invalid fit result for {name} ({par["value"]})')
                     fit_failure = True
                 elif par['value'] == self._fwhm_max:
-                    logging.warning(f'Edge result on for {name} ({par["value"]})')
-        return(fit_failure)
+                    logger.warning(
+                        f'Edge result on for {name} ({par["value"]})')
+        return fit_failure
 
 
 class FitMap(Fit):
-    """Fit a map of data
     """
-    def __init__(self, ymap, x=None, models=None, normalize=True, transpose=None, **kwargs):
+    Wrapper to the Fit class to fit dat on a N-dimensional map
+    """
+    def __init__(
+            self, ymap, x=None, models=None, normalize=True, transpose=None,
+            **kwargs):
+        """Initialize FitMap."""
         super().__init__(None)
         self._best_errors = None
         self._best_fit = None
         self._best_parameters = None
         self._best_values = None
         self._inv_transpose = None
         self._max_nfev = None
@@ -1762,755 +1887,834 @@
         self._redchi = None
         self._redchi_cutoff = 0.1
         self._skip_init = True
         self._success = None
         self._transpose = None
         self._try_no_bounds = True
 
-        # At this point the fastest index should always be the signal dimension so that the slowest 
-        #    ndim-1 dimensions are the map dimensions
+        # At this point the fastest index should always be the signal
+        #     dimension so that the slowest ndim-1 dimensions are the
+        #     map dimensions
         if isinstance(ymap, (tuple, list, np.ndarray)):
             self._x = np.asarray(x)
-        elif have_xarray and isinstance(ymap, xr.DataArray):
+        elif HAVE_XARRAY and isinstance(ymap, xr.DataArray):
             if x is not None:
-                logging.warning('Ignoring superfluous input x ({x}) in Fit.__init__')
+                logger.warning('Ignoring superfluous input x ({x})')
             self._x = np.asarray(ymap[ymap.dims[-1]])
         else:
-            illegal_value(ymap, 'ymap', 'FitMap:__init__', raise_error=True)
+            raise ValueError('Invalid parameter ymap ({ymap})')
         self._ymap = ymap
 
         # Verify the input parameters
         if self._x.ndim != 1:
             raise ValueError(f'Invalid dimension for input x {self._x.ndim}')
         if self._ymap.ndim < 2:
-            raise ValueError('Invalid number of dimension of the input dataset '+
-                    f'{self._ymap.ndim}')
+            raise ValueError(
+                'Invalid number of dimension of the input dataset '
+                f'{self._ymap.ndim}')
         if self._x.size != self._ymap.shape[-1]:
-            raise ValueError(f'Inconsistent x and y dimensions ({self._x.size} vs '+
-                    f'{self._ymap.shape[-1]})')
+            raise ValueError(
+                f'Inconsistent x and y dimensions ({self._x.size} vs '
+                f'{self._ymap.shape[-1]})')
         if not isinstance(normalize, bool):
-            logging.warning(f'Invalid value for normalize ({normalize}) in Fit.__init__: '+
-                    'setting normalize to True')
+            logger.warning(
+                f'Invalid value for normalize ({normalize}) in Fit.__init__: '
+                'setting normalize to True')
             normalize = True
         if isinstance(transpose, bool) and not transpose:
             transpose = None
         if transpose is not None and self._ymap.ndim < 3:
-            logging.warning(f'Transpose meaningless for {self._ymap.ndim-1}D data maps: ignoring '+
-                    'transpose')
+            logger.warning(
+                f'Transpose meaningless for {self._ymap.ndim-1}D data maps: '
+                'ignoring transpose')
         if transpose is not None:
-            if self._ymap.ndim == 3 and isinstance(transpose, bool) and transpose:
+            if (self._ymap.ndim == 3 and isinstance(transpose, bool)
+                    and transpose):
                 self._transpose = (1, 0)
             elif not isinstance(transpose, (tuple, list)):
-                logging.warning(f'Invalid data type for transpose ({transpose}, '+
-                        f'{type(transpose)}) in Fit.__init__: setting transpose to False')
-            elif len(transpose) != self._ymap.ndim-1:
-                logging.warning(f'Invalid dimension for transpose ({transpose}, must be equal to '+
-                        f'{self._ymap.ndim-1}) in Fit.__init__: setting transpose to False')
+                logger.warning(
+                    f'Invalid data type for transpose ({transpose}, '
+                    f'{type(transpose)}): setting transpose to False')
+            elif transpose != self._ymap.ndim-1:
+                logger.warning(
+                    f'Invalid dimension for transpose ({transpose}, must be '
+                    f'equal to {self._ymap.ndim-1}): '
+                    'setting transpose to False')
             elif any(i not in transpose for i in range(len(transpose))):
-                logging.warning(f'Invalid index in transpose ({transpose}) '+
-                        f'in Fit.__init__: setting transpose to False')
-            elif not all(i==transpose[i] for i in range(self._ymap.ndim-1)):
+                logger.warning(
+                    f'Invalid index in transpose ({transpose}): '
+                    'setting transpose to False')
+            elif not all(i == transpose[i] for i in range(self._ymap.ndim-1)):
                 self._transpose = transpose
             if self._transpose is not None:
-                self._inv_transpose = tuple(self._transpose.index(i)
-                        for i in range(len(self._transpose)))
+                self._inv_transpose = tuple(
+                    self._transpose.index(i)
+                    for i in range(len(self._transpose)))
 
         # Flatten the map (transpose if requested)
-        # Store the flattened map in self._ymap_norm, whether normalized or not
+        # Store the flattened map in self._ymap_norm, whether
+        #     normalized or not
         if self._transpose is not None:
-            self._ymap_norm = np.transpose(np.asarray(self._ymap), list(self._transpose)+
-                    [len(self._transpose)])
+            self._ymap_norm = np.transpose(
+                np.asarray(self._ymap),
+                list(self._transpose) + [len(self._transpose)])
         else:
             self._ymap_norm = np.asarray(self._ymap)
         self._map_dim = int(self._ymap_norm.size/self._x.size)
         self._map_shape = self._ymap_norm.shape[:-1]
-        self._ymap_norm = np.reshape(self._ymap_norm, (self._map_dim, self._x.size))
+        self._ymap_norm = np.reshape(
+            self._ymap_norm, (self._map_dim, self._x.size))
 
         # Check if a mask is provided
         if 'mask' in kwargs:
             self._mask = kwargs.pop('mask')
         if self._mask is None:
             ymap_min = float(self._ymap_norm.min())
             ymap_max = float(self._ymap_norm.max())
         else:
             self._mask = np.asarray(self._mask).astype(bool)
             if self._x.size != self._mask.size:
-                raise ValueError(f'Inconsistent mask dimension ({self._x.size} vs '+
-                        f'{self._mask.size})')
+                raise ValueError(
+                    f'Inconsistent mask dimension ({self._x.size} vs '
+                    f'{self._mask.size})')
             ymap_masked = np.asarray(self._ymap_norm)[:,~self._mask]
             ymap_min = float(ymap_masked.min())
             ymap_max = float(ymap_masked.max())
 
         # Normalize the data
         self._y_range = ymap_max-ymap_min
         if normalize and self._y_range > 0.0:
             self._norm = (ymap_min, self._y_range)
-            self._ymap_norm = (self._ymap_norm-self._norm[0])/self._norm[1]
+            self._ymap_norm = (self._ymap_norm-self._norm[0]) / self._norm[1]
         else:
             self._redchi_cutoff *= self._y_range**2
         if models is not None:
             if callable(models) or isinstance(models, str):
                 kwargs = self.add_model(models, **kwargs)
             elif isinstance(models, (tuple, list)):
                 for model in models:
                     kwargs = self.add_model(model, **kwargs)
             self.fit(**kwargs)
 
     @classmethod
     def fit_map(cls, ymap, models, x=None, normalize=True, **kwargs):
-        return(cls(ymap, x=x, models=models, normalize=normalize, **kwargs))
+        """Class method for FitMap."""
+        return cls(ymap, x=x, models=models, normalize=normalize, **kwargs)
 
     @property
     def best_errors(self):
-        return(self._best_errors)
+        """Return errors in the best fit parameters."""
+        return self._best_errors
 
     @property
     def best_fit(self):
-        return(self._best_fit)
+        """Return the best fits."""
+        return self._best_fit
 
     @property
     def best_results(self):
-        """Convert the input data array to a data set and add the fit results.
         """
-        if self.best_values is None or self.best_errors is None or self.best_fit is None:
-            return(None)
-        if not have_xarray:
-            logging.warning('Unable to load xarray module')
-            return(None)
+        Convert the input DataArray to a data set and add the fit
+        results.
+        """
+        if (self.best_values is None or self.best_errors is None
+                or self.best_fit is None):
+            return None
+        if not HAVE_XARRAY:
+            logger.warning('Unable to load xarray module')
+            return None
         best_values = self.best_values
         best_errors = self.best_errors
         if isinstance(self._ymap, xr.DataArray):
             best_results = self._ymap.to_dataset()
             dims = self._ymap.dims
             fit_name = f'{self._ymap.name}_fit'
         else:
-            coords = {f'dim{n}_index':([f'dim{n}_index'], range(self._ymap.shape[n]))
-                    for n in range(self._ymap.ndim-1)}
+            coords = {
+                f'dim{n}_index':([f'dim{n}_index'], range(self._ymap.shape[n]))
+                for n in range(self._ymap.ndim-1)}
             coords['x'] = (['x'], self._x)
             dims = list(coords.keys())
             best_results = xr.Dataset(coords=coords)
             best_results['y'] = (dims, self._ymap)
             fit_name = 'y_fit'
         best_results[fit_name] = (dims, self.best_fit)
         if self._mask is not None:
             best_results['mask'] = self._mask
         for n in range(best_values.shape[0]):
-            best_results[f'{self._best_parameters[n]}_values'] = (dims[:-1], best_values[n])
-            best_results[f'{self._best_parameters[n]}_errors'] = (dims[:-1], best_errors[n])
+            best_results[f'{self._best_parameters[n]}_values'] = \
+                (dims[:-1], best_values[n])
+            best_results[f'{self._best_parameters[n]}_errors'] = \
+                (dims[:-1], best_errors[n])
         best_results.attrs['components'] = self.components
-        return(best_results)
+        return best_results
 
     @property
     def best_values(self):
-        return(self._best_values)
+        """Return values of the best fit parameters."""
+        return self._best_values
 
     @property
     def chisqr(self):
-        logging.warning('property chisqr not defined for fit.FitMap')
-        return(None)
+        """Return the chisqr value of each best fit."""
+        logger.warning('Undefined property chisqr')
 
     @property
     def components(self):
+        """Return the fit model components info."""
         components = {}
         if self._result is None:
-            logging.warning('Unable to collect components in FitMap.components')
-            return(components)
+            logger.warning(
+                'Unable to collect components in FitMap.components')
+            return components
         for component in self._result.components:
             if 'tmp_normalization_offset_c' in component.param_names:
                 continue
             parameters = {}
             for name in component.param_names:
                 if self._parameters[name].vary:
                     parameters[name] = {'free': True}
                 elif self._parameters[name].expr is not None:
-                    parameters[name] = {'free': False, 'expr': self._parameters[name].expr}
+                    parameters[name] = {
+                        'free': False,
+                        'expr': self._parameters[name].expr,
+                    }
                 else:
-                    parameters[name] = {'free': False, 'value': self.init_parameters[name]['value']}
+                    parameters[name] = {
+                        'free': False,
+                        'value': self.init_parameters[name]['value'],
+                    }
             expr = None
             if isinstance(component, ExpressionModel):
                 name = component._name
                 if name[-1] == '_':
                     name = name[:-1]
                 expr = component.expr
             else:
                 prefix = component.prefix
-                if len(prefix):
+                if prefix:
                     if prefix[-1] == '_':
                         prefix = prefix[:-1]
                     name = f'{prefix} ({component._name})'
                 else:
                     name = f'{component._name}'
             if expr is None:
                 components[name] = {'parameters': parameters}
             else:
                 components[name] = {'expr': expr, 'parameters': parameters}
-        return(components)
+        return components
 
     @property
     def covar(self):
-        logging.warning('property covar not defined for fit.FitMap')
-        return(None)
+        """
+        Return the covarience matrices of the best fit parameters.
+        """
+        logger.warning('Undefined property covar')
 
     @property
     def max_nfev(self):
-        return(self._max_nfev)
+        """
+        Return the maximum number of function evaluations for each fit.
+        """
+        return self._max_nfev
 
     @property
     def num_func_eval(self):
-        logging.warning('property num_func_eval not defined for fit.FitMap')
-        return(None)
+        """
+        Return the number of function evaluations for each best fit.
+        """
+        logger.warning('Undefined property num_func_eval')
 
     @property
     def out_of_bounds(self):
-        return(self._out_of_bounds)
+        """Return the out_of_bounds value of each best fit."""
+        return self._out_of_bounds
 
     @property
     def redchi(self):
-        return(self._redchi)
+        """Return the redchi value of each best fit."""
+        return self._redchi
 
     @property
     def residual(self):
+        """Return the residual in each best fit."""
         if self.best_fit is None:
-            return(None)
+            return None
         if self._mask is None:
-            return(np.asarray(self._ymap)-self.best_fit)
+            residual = np.asarray(self._ymap)-self.best_fit
         else:
-            ymap_flat = np.reshape(np.asarray(self._ymap), (self._map_dim, self._x.size))
+            ymap_flat = np.reshape(
+                np.asarray(self._ymap), (self._map_dim, self._x.size))
             ymap_flat_masked = ymap_flat[:,~self._mask]
-            ymap_masked = np.reshape(ymap_flat_masked,
-                    list(self._map_shape)+[ymap_flat_masked.shape[-1]])
-            return(ymap_masked-self.best_fit)
+            ymap_masked = np.reshape(
+                ymap_flat_masked,
+                list(self._map_shape) + [ymap_flat_masked.shape[-1]])
+            residual = ymap_masked-self.best_fit
+        return residual
 
     @property
     def success(self):
-        return(self._success)
+        """Return the success value for each fit."""
+        return self._success
 
     @property
     def var_names(self):
-        logging.warning('property var_names not defined for fit.FitMap')
-        return(None)
+        """
+        Return the variable names for the covarience matrix property.
+        """
+        logger.warning('Undefined property var_names')
 
     @property
     def y(self):
-        logging.warning('property y not defined for fit.FitMap')
-        return(None)
+        """Return the input y-array."""
+        logger.warning('Undefined property y')
 
     @property
     def ymap(self):
-        return(self._ymap)
+        """Return the input y-array map."""
+        return self._ymap
 
     def best_parameters(self, dims=None):
+        """Return the best fit parameters."""
         if dims is None:
-            return(self._best_parameters)
-        if not isinstance(dims, (list, tuple)) or len(dims) != len(self._map_shape):
-            illegal_value(dims, 'dims', 'FitMap.best_parameters', raise_error=True)
+            return self._best_parameters
+        if (not isinstance(dims, (list, tuple))
+                or len(dims) != len(self._map_shape)):
+            raise ValueError('Invalid parameter dims ({dims})')
         if self.best_values is None or self.best_errors is None:
-            logging.warning(f'Unable to obtain best parameter values for dims = {dims} in '+
-                    'FitMap.best_parameters')
-            return({})
+            logger.warning(
+                f'Unable to obtain best parameter values for dims = {dims}')
+            return {}
         # Create current parameters
         parameters = deepcopy(self._parameters)
         for n, name in enumerate(self._best_parameters):
             if self._parameters[name].vary:
                 parameters[name].set(value=self.best_values[n][dims])
             parameters[name].stderr = self.best_errors[n][dims]
         parameters_dict = {}
         for name in sorted(parameters):
             if name != 'tmp_normalization_offset_c':
                 par = parameters[name]
-                parameters_dict[name] = {'value': par.value, 'error': par.stderr,
-                        'init_value': self.init_parameters[name]['value'], 'min': par.min,
-                        'max': par.max, 'vary': par.vary, 'expr': par.expr}
-        return(parameters_dict)
+                parameters_dict[name] = {
+                    'value': par.value,
+                    'error': par.stderr,
+                    'init_value': self.init_parameters[name]['value'],
+                    'min': par.min,
+                    'max': par.max,
+                    'vary': par.vary,
+                    'expr': par.expr,
+                }
+        return parameters_dict
 
     def freemem(self):
+        """Free memory allocated for parallel processing."""
         if self._memfolder is None:
             return
         try:
             rmtree(self._memfolder)
             self._memfolder = None
         except:
-            logging.warning('Could not clean-up automatically.')
+            logger.warning('Could not clean-up automatically.')
 
-    def plot(self, dims, y_title=None, plot_residual=False, plot_comp_legends=False,
-            plot_masked_data=True):
-        if not isinstance(dims, (list, tuple)) or len(dims) != len(self._map_shape):
-            illegal_value(dims, 'dims', 'FitMap.plot', raise_error=True)
-        if self._result is None or self.best_fit is None or self.best_values is None:
-            logging.warning(f'Unable to plot fit for dims = {dims} in FitMap.plot')
+    def plot(
+            self, dims=None, y_title=None, plot_residual=False,
+            plot_comp_legends=False, plot_masked_data=True, **kwargs):
+        """Plot the best fits."""
+        if dims is None:
+            dims = [0]*len(self._map_shape)
+        if (not isinstance(dims, (list, tuple))
+                or len(dims) != len(self._map_shape)):
+            raise ValueError('Invalid parameter dims ({dims})')
+        if (self._result is None or self.best_fit is None
+                or self.best_values is None):
+            logger.warning(
+                f'Unable to plot fit for dims = {dims}')
             return
         if y_title is None or not isinstance(y_title, str):
             y_title = 'data'
         if self._mask is None:
             mask = np.zeros(self._x.size).astype(bool)
             plot_masked_data = False
         else:
             mask = self._mask
         plots = [(self._x, np.asarray(self._ymap[dims]), 'b.')]
         legend = [y_title]
         if plot_masked_data:
-            plots += [(self._x[mask], np.asarray(self._ymap)[(*dims,mask)], 'bx')]
+            plots += \
+                [(self._x[mask], np.asarray(self._ymap)[(*dims,mask)], 'bx')]
             legend += ['masked data']
         plots += [(self._x[~mask], self.best_fit[dims], 'k-')]
         legend += ['best fit']
         if plot_residual:
             plots += [(self._x[~mask], self.residual[dims], 'r--')]
             legend += ['residual']
         # Create current parameters
         parameters = deepcopy(self._parameters)
         for name in self._best_parameters:
             if self._parameters[name].vary:
-                parameters[name].set(value=
-                        self.best_values[self._best_parameters.index(name)][dims])
+                parameters[name].set(
+                    value=self.best_values[self._best_parameters.index(name)]
+                    [dims])
         for component in self._result.components:
             if 'tmp_normalization_offset_c' in component.param_names:
                 continue
             if isinstance(component, ExpressionModel):
                 prefix = component._name
                 if prefix[-1] == '_':
                     prefix = prefix[:-1]
                 modelname = f'{prefix}: {component.expr}'
             else:
                 prefix = component.prefix
-                if len(prefix):
+                if prefix:
                     if prefix[-1] == '_':
                         prefix = prefix[:-1]
                     modelname = f'{prefix} ({component._name})'
                 else:
                     modelname = f'{component._name}'
             if len(modelname) > 20:
                 modelname = f'{modelname[0:16]} ...'
             y = component.eval(params=parameters, x=self._x[~mask])
             if isinstance(y, (int, float)):
                 y *= np.ones(self._x[~mask].size)
             plots += [(self._x[~mask], y, '--')]
             if plot_comp_legends:
                 legend.append(modelname)
-        quick_plot(tuple(plots), legend=legend, title=str(dims), block=True)
+        quick_plot(
+            tuple(plots), legend=legend, title=str(dims), block=True, **kwargs)
 
     def fit(self, **kwargs):
-#        t0 = time()
+        """Fit the model to the input data."""
         # Check input parameters
         if self._model is None:
-            logging.error('Undefined fit model')
+            logger.error('Undefined fit model')
         if 'num_proc' in kwargs:
             num_proc = kwargs.pop('num_proc')
             if not is_int(num_proc, ge=1):
-                illegal_value(num_proc, 'num_proc', 'FitMap.fit', raise_error=True)
+                raise ValueError(
+                    'Invalid value for keyword argument num_proc ({num_proc})')
         else:
             num_proc = cpu_count()
-        if num_proc > 1 and not have_joblib:
-            logging.warning(f'Missing joblib in the conda environment, running FitMap serially')
+        if num_proc > 1 and not HAVE_JOBLIB:
+            logger.warning(
+                'Missing joblib in the conda environment, running serially')
             num_proc = 1
         if num_proc > cpu_count():
-            logging.warning(f'The requested number of processors ({num_proc}) exceeds the maximum '+
-                    f'number of processors, num_proc reduced to ({cpu_count()})')
+            logger.warning(
+                f'The requested number of processors ({num_proc}) exceeds the '
+                'maximum number of processors, num_proc reduced to '
+                f'({cpu_count()})')
             num_proc = cpu_count()
         if 'try_no_bounds' in kwargs:
             self._try_no_bounds = kwargs.pop('try_no_bounds')
             if not isinstance(self._try_no_bounds, bool):
-                illegal_value(self._try_no_bounds, 'try_no_bounds', 'FitMap.fit', raise_error=True)
+                raise ValueError(
+                    'Invalid value for keyword argument try_no_bounds '
+                    f'({self._try_no_bounds})')
         if 'redchi_cutoff' in kwargs:
             self._redchi_cutoff = kwargs.pop('redchi_cutoff')
             if not is_num(self._redchi_cutoff, gt=0):
-                illegal_value(self._redchi_cutoff, 'redchi_cutoff', 'FitMap.fit', raise_error=True)
+                raise ValueError(
+                    'Invalid value for keyword argument redchi_cutoff'
+                    f'({self._redchi_cutoff})')
         if 'print_report' in kwargs:
             self._print_report = kwargs.pop('print_report')
             if not isinstance(self._print_report, bool):
-                illegal_value(self._print_report, 'print_report', 'FitMap.fit', raise_error=True)
+                raise ValueError(
+                    'Invalid value for keyword argument print_report'
+                    f'({self._print_report})')
         if 'plot' in kwargs:
             self._plot = kwargs.pop('plot')
             if not isinstance(self._plot, bool):
-                illegal_value(self._plot, 'plot', 'FitMap.fit', raise_error=True)
+                raise ValueError(
+                    'Invalid value for keyword argument plot'
+                    f'({self._plot})')
         if 'skip_init' in kwargs:
             self._skip_init = kwargs.pop('skip_init')
             if not isinstance(self._skip_init, bool):
-                illegal_value(self._skip_init, 'skip_init', 'FitMap.fit', raise_error=True)
+                raise ValueError(
+                    'Invalid value for keyword argument skip_init'
+                    f'({self._skip_init})')
 
         # Apply mask if supplied:
         if 'mask' in kwargs:
             self._mask = kwargs.pop('mask')
         if self._mask is not None:
             self._mask = np.asarray(self._mask).astype(bool)
             if self._x.size != self._mask.size:
-                raise ValueError(f'Inconsistent x and mask dimensions ({self._x.size} vs '+
-                        f'{self._mask.size})')
+                raise ValueError(
+                    f'Inconsistent x and mask dimensions ({self._x.size} vs '
+                    f'{self._mask.size})')
 
         # Add constant offset for a normalized single component model
         if self._result is None and self._norm is not None and self._norm[0]:
-            self.add_model('constant', prefix='tmp_normalization_offset_', parameters={'name': 'c',
-                    'value': -self._norm[0], 'vary': False, 'norm': True})
-                    #'value': -self._norm[0]/self._norm[1], 'vary': False, 'norm': False})
+            self.add_model(
+                'constant',
+                prefix='tmp_normalization_offset_',
+                parameters={
+                    'name': 'c',
+                    'value': -self._norm[0],
+                    'vary': False,
+                    'norm': True,
+                })
+#                    'value': -self._norm[0]/self._norm[1],
+#                    'vary': False,
+#                    'norm': False,
 
         # Adjust existing parameters for refit:
         if 'parameters' in kwargs:
-#            print('\nIn FitMap before adjusting existing parameters for refit:')
-#            self._parameters.pretty_print()
-#            if self._result is None:
-#                raise ValueError('Invalid parameter parameters ({parameters})')
-#            if self._best_values is None:
-#                raise ValueError('Valid self._best_values required for refitting in FitMap.fit')
             parameters = kwargs.pop('parameters')
-#            print(f'\nparameters:\n{parameters}')
             if isinstance(parameters, dict):
                 parameters = (parameters, )
             elif not is_dict_series(parameters):
-                illegal_value(parameters, 'parameters', 'Fit.fit', raise_error=True)
+                raise ValueError(
+                    'Invalid value for keyword argument parameters'
+                    f'({parameters})')
             for par in parameters:
                 name = par['name']
                 if name not in self._parameters:
-                    raise ValueError(f'Unable to match {name} parameter {par} to an existing one')
+                    raise ValueError(
+                        f'Unable to match {name} parameter {par} to an '
+                        'existing one')
                 if self._parameters[name].expr is not None:
-                    raise ValueError(f'Unable to modify {name} parameter {par} (currently an '+
-                            'expression)')
-                value =  par.get('value')
-                vary =  par.get('vary')
+                    raise ValueError(
+                        f'Unable to modify {name} parameter {par} '
+                        '(currently an expression)')
+                value = par.get('value')
+                vary = par.get('vary')
                 if par.get('expr') is not None:
-                    raise KeyError(f'Invalid "expr" key in {name} parameter {par}')
-                self._parameters[name].set(value=value, vary=vary, min=par.get('min'),
-                        max=par.get('max'))
-                # Overwrite existing best values for fixed parameters when a value is specified
-#                print(f'best values befored resetting:\n{self._best_values}')
+                    raise KeyError(
+                        f'Invalid "expr" key in {name} parameter {par}')
+                self._parameters[name].set(
+                    value=value, vary=vary, min=par.get('min'),
+                    max=par.get('max'))
+                # Overwrite existing best values for fixed parameters
+                #     when a value is specified
                 if isinstance(value, (int, float)) and vary is False:
                     for i, nname in enumerate(self._best_parameters):
                         if nname == name:
                             self._best_values[i] = value
-#                print(f'best values after resetting (value={value}, vary={vary}):\n{self._best_values}')
-#RV            print('\nIn FitMap after adjusting existing parameters for refit:')
-#RV            self._parameters.pretty_print()
 
         # Check for uninitialized parameters
         for name, par in self._parameters.items():
             if par.expr is None:
                 value = par.value
                 if value is None or np.isinf(value) or np.isnan(value):
                     value = 1.0
                     if self._norm is None or name not in self._parameter_norms:
                         self._parameters[name].set(value=value)
                     elif self._parameter_norms[name]:
                         self._parameters[name].set(value=value*self._norm[1])
 
-        # Create the best parameter list, consisting of all varying parameters plus the expression
-        #   parameters in order to collect their errors
+        # Create the best parameter list, consisting of all varying
+        #     parameters plus the expression parameters in order to
+        #     collect their errors
         if self._result is None:
             # Initial fit
-            assert(self._best_parameters is None)
-            self._best_parameters = [name for name, par in self._parameters.items()
-                    if par.vary or par.expr is not None]
+            assert self._best_parameters is None
+            self._best_parameters = [
+                name for name, par in self._parameters.items()
+                if par.vary or par.expr is not None]
             num_new_parameters = 0
         else:
             # Refit
-            assert(len(self._best_parameters))
-            self._new_parameters = [name for name, par in self._parameters.items()
-                if name != 'tmp_normalization_offset_c' and name not in self._best_parameters and
-                    (par.vary or par.expr is not None)]
+            assert self._best_parameters
+            self._new_parameters = [
+                name for name, par in self._parameters.items()
+                if name != 'tmp_normalization_offset_c'
+                and name not in self._best_parameters
+                and (par.vary or par.expr is not None)]
             num_new_parameters = len(self._new_parameters)
         num_best_parameters = len(self._best_parameters)
 
-        # Flatten and normalize the best values of the previous fit, remove the remaining results
-        #   of the previous fit
+        # Flatten and normalize the best values of the previous fit,
+        #     remove the remaining results of the previous fit
         if self._result is not None:
-#            print('\nBefore flatten and normalize:')
-#            print(f'self._best_values:\n{self._best_values}')
             self._out_of_bounds = None
             self._max_nfev = None
             self._redchi = None
             self._success = None
             self._best_fit = None
             self._best_errors = None
-            assert(self._best_values is not None)
-            assert(self._best_values.shape[0] == num_best_parameters)
-            assert(self._best_values.shape[1:] == self._map_shape)
+            assert self._best_values is not None
+            assert self._best_values.shape[0] == num_best_parameters
+            assert self._best_values.shape[1:] == self._map_shape
             if self._transpose is not None:
-                self._best_values = np.transpose(self._best_values,
-                        [0]+[i+1 for i in self._transpose])
-            self._best_values = [np.reshape(self._best_values[i], self._map_dim)
+                self._best_values = np.transpose(
+                    self._best_values, [0]+[i+1 for i in self._transpose])
+            self._best_values = [
+                np.reshape(self._best_values[i], self._map_dim)
                 for i in range(num_best_parameters)]
             if self._norm is not None:
                 for i, name in enumerate(self._best_parameters):
                     if self._parameter_norms.get(name, False):
                         self._best_values[i] /= self._norm[1]
-#RV            print('\nAfter flatten and normalize:')
-#RV            print(f'self._best_values:\n{self._best_values}')
 
-        # Normalize the initial parameters (and best values for a refit)
-#        print('\nIn FitMap before normalize:')
-#        self._parameters.pretty_print()
-#        print(f'\nparameter_norms:\n{self._parameter_norms}\n')
+        # Normalize the initial parameters
+        #     (and best values for a refit)
         self._normalize()
-#        print('\nIn FitMap after normalize:')
-#        self._parameters.pretty_print()
-#        print(f'\nparameter_norms:\n{self._parameter_norms}\n')
 
         # Prevent initial values from sitting at boundaries
-        self._parameter_bounds = {name:{'min': par.min, 'max': par.max}
-                for name, par in self._parameters.items() if par.vary}
+        self._parameter_bounds = {
+            name:{'min': par.min, 'max': par.max}
+            for name, par in self._parameters.items() if par.vary}
         for name, par in self._parameters.items():
             if par.vary:
                 par.set(value=self._reset_par_at_boundary(par, par.value))
-#        print('\nAfter checking boundaries:')
-#        self._parameters.pretty_print()
 
-        # Set parameter bounds to unbound (only use bounds when fit fails)
+        # Set parameter bounds to unbound
+        #     (only use bounds when fit fails)
         if self._try_no_bounds:
             for name in self._parameter_bounds.keys():
                 self._parameters[name].set(min=-np.inf, max=np.inf)
 
         # Allocate memory to store fit results
         if self._mask is None:
             x_size = self._x.size
         else:
             x_size = self._x[~self._mask].size
         if num_proc == 1:
             self._out_of_bounds_flat = np.zeros(self._map_dim, dtype=bool)
             self._max_nfev_flat = np.zeros(self._map_dim, dtype=bool)
             self._redchi_flat = np.zeros(self._map_dim, dtype=np.float64)
             self._success_flat = np.zeros(self._map_dim, dtype=bool)
-            self._best_fit_flat = np.zeros((self._map_dim, x_size),
-                    dtype=self._ymap_norm.dtype)
-            self._best_errors_flat = [np.zeros(self._map_dim, dtype=np.float64)
-                    for _ in range(num_best_parameters+num_new_parameters)]
+            self._best_fit_flat = np.zeros(
+                (self._map_dim, x_size), dtype=self._ymap_norm.dtype)
+            self._best_errors_flat = [
+                np.zeros(self._map_dim, dtype=np.float64)
+                for _ in range(num_best_parameters+num_new_parameters)]
             if self._result is None:
-                self._best_values_flat = [np.zeros(self._map_dim, dtype=np.float64)
-                        for _ in range(num_best_parameters)]
+                self._best_values_flat = [
+                    np.zeros(self._map_dim, dtype=np.float64)
+                    for _ in range(num_best_parameters)]
             else:
                 self._best_values_flat = self._best_values
-                self._best_values_flat += [np.zeros(self._map_dim, dtype=np.float64)
-                        for _ in range(num_new_parameters)]
+                self._best_values_flat += [
+                    np.zeros(self._map_dim, dtype=np.float64)
+                    for _ in range(num_new_parameters)]
         else:
             self._memfolder = './joblib_memmap'
             try:
                 mkdir(self._memfolder)
             except FileExistsError:
                 pass
-            filename_memmap = path.join(self._memfolder, 'out_of_bounds_memmap')
-            self._out_of_bounds_flat = np.memmap(filename_memmap, dtype=bool,
-                    shape=(self._map_dim), mode='w+')
+            filename_memmap = path.join(
+                self._memfolder, 'out_of_bounds_memmap')
+            self._out_of_bounds_flat = np.memmap(
+                filename_memmap, dtype=bool, shape=(self._map_dim), mode='w+')
             filename_memmap = path.join(self._memfolder, 'max_nfev_memmap')
-            self._max_nfev_flat = np.memmap(filename_memmap, dtype=bool,
-                    shape=(self._map_dim), mode='w+')
+            self._max_nfev_flat = np.memmap(
+                filename_memmap, dtype=bool, shape=(self._map_dim), mode='w+')
             filename_memmap = path.join(self._memfolder, 'redchi_memmap')
-            self._redchi_flat = np.memmap(filename_memmap, dtype=np.float64,
-                    shape=(self._map_dim), mode='w+')
+            self._redchi_flat = np.memmap(
+                filename_memmap, dtype=np.float64, shape=(self._map_dim),
+                mode='w+')
             filename_memmap = path.join(self._memfolder, 'success_memmap')
-            self._success_flat = np.memmap(filename_memmap, dtype=bool,
-                    shape=(self._map_dim), mode='w+')
+            self._success_flat = np.memmap(
+                filename_memmap, dtype=bool, shape=(self._map_dim), mode='w+')
             filename_memmap = path.join(self._memfolder, 'best_fit_memmap')
-            self._best_fit_flat = np.memmap(filename_memmap, dtype=self._ymap_norm.dtype,
-                    shape=(self._map_dim, x_size), mode='w+')
+            self._best_fit_flat = np.memmap(
+                filename_memmap, dtype=self._ymap_norm.dtype,
+                shape=(self._map_dim, x_size), mode='w+')
             self._best_errors_flat = []
             for i in range(num_best_parameters+num_new_parameters):
-                filename_memmap = path.join(self._memfolder, f'best_errors_memmap_{i}')
-                self._best_errors_flat.append(np.memmap(filename_memmap, dtype=np.float64,
-                        shape=self._map_dim, mode='w+'))
+                filename_memmap = path.join(
+                    self._memfolder, f'best_errors_memmap_{i}')
+                self._best_errors_flat.append(
+                    np.memmap(filename_memmap, dtype=np.float64,
+                              shape=self._map_dim, mode='w+'))
             self._best_values_flat = []
             for i in range(num_best_parameters):
-                filename_memmap = path.join(self._memfolder, f'best_values_memmap_{i}')
-                self._best_values_flat.append(np.memmap(filename_memmap, dtype=np.float64,
-                        shape=self._map_dim, mode='w+'))
+                filename_memmap = path.join(
+                    self._memfolder, f'best_values_memmap_{i}')
+                self._best_values_flat.append(
+                    np.memmap(filename_memmap, dtype=np.float64,
+                              shape=self._map_dim, mode='w+'))
                 if self._result is not None:
                     self._best_values_flat[i][:] = self._best_values[i][:]
             for i in range(num_new_parameters):
-                filename_memmap = path.join(self._memfolder,
-                        f'best_values_memmap_{i+num_best_parameters}')
-                self._best_values_flat.append(np.memmap(filename_memmap, dtype=np.float64,
-                        shape=self._map_dim, mode='w+'))
+                filename_memmap = path.join(
+                    self._memfolder,
+                    f'best_values_memmap_{i+num_best_parameters}')
+                self._best_values_flat.append(
+                    np.memmap(filename_memmap, dtype=np.float64,
+                              shape=self._map_dim, mode='w+'))
 
         # Update the best parameter list
         if num_new_parameters:
             self._best_parameters += self._new_parameters
 
-        # Perform the first fit to get model component info and initial parameters
+        # Perform the first fit to get model component info and
+        #     initial parameters
         current_best_values = {}
-#        print(f'0 before:\n{current_best_values}')
-#        t1 = time()
-        self._result = self._fit(0, current_best_values, return_result=True, **kwargs)
-#        t2 = time()
-#        print(f'0 after:\n{current_best_values}')
-#        print('\nAfter the first fit:')
-#        self._parameters.pretty_print()
-#        print(self._result.fit_report(show_correl=False))
+        self._result = self._fit(
+            0, current_best_values, return_result=True, **kwargs)
 
         # Remove all irrelevant content from self._result
-        for attr in ('_abort', 'aborted', 'aic', 'best_fit', 'best_values', 'bic', 'calc_covar',
-                'call_kws', 'chisqr', 'ci_out', 'col_deriv', 'covar', 'data', 'errorbars',
-                'flatchain', 'ier', 'init_vals', 'init_fit', 'iter_cb', 'jacfcn', 'kws',
-                'last_internal_values', 'lmdif_message', 'message', 'method', 'nan_policy',
-                'ndata', 'nfev', 'nfree', 'params', 'redchi', 'reduce_fcn', 'residual', 'result',
-                'scale_covar', 'show_candidates', 'calc_covar', 'success', 'userargs', 'userfcn',
-                'userkws', 'values', 'var_names', 'weights', 'user_options'):
+        for attr in (
+                '_abort', 'aborted', 'aic', 'best_fit', 'best_values', 'bic',
+                'calc_covar', 'call_kws', 'chisqr', 'ci_out', 'col_deriv',
+                'covar', 'data', 'errorbars', 'flatchain', 'ier', 'init_vals',
+                'init_fit', 'iter_cb', 'jacfcn', 'kws', 'last_internal_values',
+                'lmdif_message', 'message', 'method', 'nan_policy', 'ndata',
+                'nfev', 'nfree', 'params', 'redchi', 'reduce_fcn', 'residual',
+                'result', 'scale_covar', 'show_candidates', 'calc_covar',
+                'success', 'userargs', 'userfcn', 'userkws', 'values',
+                'var_names', 'weights', 'user_options'):
             try:
                 delattr(self._result, attr)
             except AttributeError:
-#                logging.warning(f'Unknown attribute {attr} in fit.FtMap._cleanup_result')
                 pass
 
-#        t3 = time()
         if num_proc == 1:
             # Perform the remaining fits serially
             for n in range(1, self._map_dim):
-#                print(f'{n} before:\n{current_best_values}')
                 self._fit(n, current_best_values, **kwargs)
-#                print(f'{n} after:\n{current_best_values}')
         else:
             # Perform the remaining fits in parallel
             num_fit = self._map_dim-1
-#            print(f'num_fit = {num_fit}')
             if num_proc > num_fit:
-                logging.warning(f'The requested number of processors ({num_proc}) exceeds the '+
-                        f'number of fits, num_proc reduced to ({num_fit})')
+                logger.warning(
+                    f'The requested number of processors ({num_proc}) exceeds '
+                    f'the number of fits, num_proc reduced to ({num_fit})')
                 num_proc = num_fit
                 num_fit_per_proc = 1
             else:
                 num_fit_per_proc = round((num_fit)/num_proc)
                 if num_proc*num_fit_per_proc < num_fit:
-                    num_fit_per_proc +=1
-#            print(f'num_fit_per_proc = {num_fit_per_proc}')
+                    num_fit_per_proc += 1
             num_fit_batch = min(num_fit_per_proc, 40)
-#            print(f'num_fit_batch = {num_fit_batch}')
             with Parallel(n_jobs=num_proc) as parallel:
-                parallel(delayed(self._fit_parallel)(current_best_values, num_fit_batch,
-                        n_start, **kwargs) for n_start in range(1, self._map_dim, num_fit_batch))
-#        t4 = time()
+                parallel(
+                    delayed(self._fit_parallel)
+                        (current_best_values, num_fit_batch, n_start, **kwargs)
+                    for n_start in range(1, self._map_dim, num_fit_batch))
 
         # Renormalize the initial parameters for external use
         if self._norm is not None and self._normalized:
             init_values = {}
             for name, value in self._result.init_values.items():
-                if name not in self._parameter_norms or self._parameters[name].expr is not None:
+                if (name not in self._parameter_norms
+                        or self._parameters[name].expr is not None):
                     init_values[name] = value
                 elif self._parameter_norms[name]:
                     init_values[name] = value*self._norm[1]
             self._result.init_values = init_values
             for name, par in self._result.init_params.items():
                 if par.expr is None and self._parameter_norms.get(name, False):
                     _min = par.min
                     _max = par.max
                     value = par.value*self._norm[1]
-                    if not np.isinf(_min) and abs(_min) != float_min:
+                    if not np.isinf(_min) and abs(_min) != FLOAT_MIN:
                         _min *= self._norm[1]
-                    if not np.isinf(_max) and abs(_max) != float_min:
+                    if not np.isinf(_max) and abs(_max) != FLOAT_MIN:
                         _max *= self._norm[1]
                     par.set(value=value, min=_min, max=_max)
                 par.init_value = par.value
 
         # Remap the best results
-#        t5 = time()
-        self._out_of_bounds = np.copy(np.reshape(self._out_of_bounds_flat, self._map_shape))
-        self._max_nfev = np.copy(np.reshape(self._max_nfev_flat, self._map_shape))
+        self._out_of_bounds = np.copy(np.reshape(
+            self._out_of_bounds_flat, self._map_shape))
+        self._max_nfev = np.copy(np.reshape(
+            self._max_nfev_flat, self._map_shape))
         self._redchi = np.copy(np.reshape(self._redchi_flat, self._map_shape))
-        self._success = np.copy(np.reshape(self._success_flat, self._map_shape))
-        self._best_fit = np.copy(np.reshape(self._best_fit_flat,
-               list(self._map_shape)+[x_size]))
-        self._best_values = np.asarray([np.reshape(par, list(self._map_shape))
-                for par in self._best_values_flat])
-        self._best_errors = np.asarray([np.reshape(par, list(self._map_shape))
-                for par in self._best_errors_flat])
+        self._success = np.copy(np.reshape(
+            self._success_flat, self._map_shape))
+        self._best_fit = np.copy(np.reshape(
+            self._best_fit_flat, list(self._map_shape)+[x_size]))
+        self._best_values = np.asarray([np.reshape(
+            par, list(self._map_shape)) for par in self._best_values_flat])
+        self._best_errors = np.asarray([np.reshape(
+            par, list(self._map_shape)) for par in self._best_errors_flat])
         if self._inv_transpose is not None:
-            self._out_of_bounds = np.transpose(self._out_of_bounds, self._inv_transpose)
+            self._out_of_bounds = np.transpose(
+                self._out_of_bounds, self._inv_transpose)
             self._max_nfev = np.transpose(self._max_nfev, self._inv_transpose)
             self._redchi = np.transpose(self._redchi, self._inv_transpose)
             self._success = np.transpose(self._success, self._inv_transpose)
-            self._best_fit = np.transpose(self._best_fit,
-                    list(self._inv_transpose)+[len(self._inv_transpose)])
-            self._best_values = np.transpose(self._best_values,
-                    [0]+[i+1 for i in self._inv_transpose])
-            self._best_errors = np.transpose(self._best_errors,
-                    [0]+[i+1 for i in self._inv_transpose])
+            self._best_fit = np.transpose(
+                self._best_fit,
+                list(self._inv_transpose) + [len(self._inv_transpose)])
+            self._best_values = np.transpose(
+                self._best_values, [0] + [i+1 for i in self._inv_transpose])
+            self._best_errors = np.transpose(
+                self._best_errors, [0] + [i+1 for i in self._inv_transpose])
         del self._out_of_bounds_flat
         del self._max_nfev_flat
         del self._redchi_flat
         del self._success_flat
         del self._best_fit_flat
         del self._best_values_flat
         del self._best_errors_flat
-#        t6 = time()
 
         # Restore parameter bounds and renormalize the parameters
         for name, par in self._parameter_bounds.items():
             self._parameters[name].set(min=par['min'], max=par['max'])
         self._normalized = False
         if self._norm is not None:
             for name, norm in self._parameter_norms.items():
                 par = self._parameters[name]
                 if par.expr is None and norm:
                     value = par.value*self._norm[1]
                     _min = par.min
                     _max = par.max
-                    if not np.isinf(_min) and abs(_min) != float_min:
+                    if not np.isinf(_min) and abs(_min) != FLOAT_MIN:
                         _min *= self._norm[1]
-                    if not np.isinf(_max) and abs(_max) != float_min:
+                    if not np.isinf(_max) and abs(_max) != FLOAT_MIN:
                         _max *= self._norm[1]
                     par.set(value=value, min=_min, max=_max)
-#        t7 = time()
-#        print(f'total run time in fit: {t7-t0:.2f} seconds')
-#        print(f'run time first fit: {t2-t1:.2f} seconds')
-#        print(f'run time remaining fits: {t4-t3:.2f} seconds')
-#        print(f'run time remapping results: {t6-t5:.2f} seconds')
-
-#        print('\n\nAt end fit:')
-#        self._parameters.pretty_print()
-#        print(f'self._best_values:\n{self._best_values}\n\n')
 
         # Free the shared memory
         self.freemem()
 
     def _fit_parallel(self, current_best_values, num, n_start, **kwargs):
         num = min(num, self._map_dim-n_start)
         for n in range(num):
-#            print(f'{n_start+n} before:\n{current_best_values}')
             self._fit(n_start+n, current_best_values, **kwargs)
-#            print(f'{n_start+n} after:\n{current_best_values}')
 
     def _fit(self, n, current_best_values, return_result=False, **kwargs):
-#RV        print(f'\n\nstart FitMap._fit {n}\n')
-#RV        print(f'current_best_values = {current_best_values}')
-#RV        print(f'self._best_parameters = {self._best_parameters}')
-#RV        print(f'self._new_parameters = {self._new_parameters}\n\n')
-#        self._parameters.pretty_print()
-        # Set parameters to current best values, but prevent them from sitting at boundaries
+        # Set parameters to current best values, but prevent them from
+        #     sitting at boundaries
         if self._new_parameters is None:
             # Initial fit
             for name, value in current_best_values.items():
                 par = self._parameters[name]
                 par.set(value=self._reset_par_at_boundary(par, value))
         else:
             # Refit
             for i, name in enumerate(self._best_parameters):
                 par = self._parameters[name]
                 if name in self._new_parameters:
                     if name in current_best_values:
-                        par.set(value=self._reset_par_at_boundary(par, current_best_values[name]))
+                        par.set(value=self._reset_par_at_boundary(
+                            par, current_best_values[name]))
                 elif par.expr is None:
                     par.set(value=self._best_values[i][n])
-#RV        print(f'\nbefore fit {n}')
-#RV        self._parameters.pretty_print()
         if self._mask is None:
-            result = self._model.fit(self._ymap_norm[n], self._parameters, x=self._x, **kwargs)
+            result = self._model.fit(
+                self._ymap_norm[n], self._parameters, x=self._x, **kwargs)
         else:
-            result = self._model.fit(self._ymap_norm[n][~self._mask], self._parameters,
-                    x=self._x[~self._mask], **kwargs)
-#        print(f'\nafter fit {n}')
-#        self._parameters.pretty_print()
-#        print(result.fit_report(show_correl=False))
+            result = self._model.fit(
+                self._ymap_norm[n][~self._mask], self._parameters,
+                x=self._x[~self._mask], **kwargs)
         out_of_bounds = False
         for name, par in self._parameter_bounds.items():
             value = result.params[name].value
             if not np.isinf(par['min']) and value < par['min']:
                 out_of_bounds = True
                 break
             if not np.isinf(par['max']) and value > par['max']:
                 out_of_bounds = True
                 break
         self._out_of_bounds_flat[n] = out_of_bounds
         if self._try_no_bounds and out_of_bounds:
             # Rerun fit with parameter bounds in place
             for name, par in self._parameter_bounds.items():
                 self._parameters[name].set(min=par['min'], max=par['max'])
-            # Set parameters to current best values, but prevent them from sitting at boundaries
+            # Set parameters to current best values, but prevent them
+            #     from sitting at boundaries
             if self._new_parameters is None:
                 # Initial fit
                 for name, value in current_best_values.items():
                     par = self._parameters[name]
                     par.set(value=self._reset_par_at_boundary(par, value))
             else:
                 # Refit
@@ -2518,96 +2722,98 @@
                     par = self._parameters[name]
                     if name in self._new_parameters:
                         if name in current_best_values:
                             par.set(value=self._reset_par_at_boundary(par,
                                     current_best_values[name]))
                     elif par.expr is None:
                         par.set(value=self._best_values[i][n])
-#            print('\nbefore fit')
-#            self._parameters.pretty_print()
-#            print(result.fit_report(show_correl=False))
             if self._mask is None:
-                result = self._model.fit(self._ymap_norm[n], self._parameters, x=self._x, **kwargs)
+                result = self._model.fit(
+                    self._ymap_norm[n], self._parameters, x=self._x, **kwargs)
             else:
-                result = self._model.fit(self._ymap_norm[n][~self._mask], self._parameters,
+                result = self._model.fit(
+                    self._ymap_norm[n][~self._mask], self._parameters,
                     x=self._x[~self._mask], **kwargs)
-#            print(f'\nafter fit {n}')
-#            self._parameters.pretty_print()
-#            print(result.fit_report(show_correl=False))
             out_of_bounds = False
             for name, par in self._parameter_bounds.items():
                 value = result.params[name].value
                 if not np.isinf(par['min']) and value < par['min']:
                     out_of_bounds = True
                     break
                 if not np.isinf(par['max']) and value > par['max']:
                     out_of_bounds = True
                     break
-#            print(f'{n} redchi < redchi_cutoff = {result.redchi < self._redchi_cutoff} success = {result.success} out_of_bounds = {out_of_bounds}')
             # Reset parameters back to unbound
             for name in self._parameter_bounds.keys():
                 self._parameters[name].set(min=-np.inf, max=np.inf)
-        assert(not out_of_bounds)
+        assert not out_of_bounds
         if result.redchi >= self._redchi_cutoff:
             result.success = False
         if result.nfev == result.max_nfev:
-#            print(f'Maximum number of function evaluations reached for n = {n}')
-#            logging.warning(f'Maximum number of function evaluations reached for n = {n}')
             if result.redchi < self._redchi_cutoff:
                 result.success = True
             self._max_nfev_flat[n] = True
         if result.success:
-            assert(all(True for par in current_best_values if par in result.params.values()))
+            assert all(
+                True for par in current_best_values
+                if par in result.params.values())
             for par in result.params.values():
                 if par.vary:
                     current_best_values[par.name] = par.value
         else:
-            logging.warning(f'Fit for n = {n} failed: {result.lmdif_message}')
+            logger.warning(f'Fit for n = {n} failed: {result.lmdif_message}')
         # Renormalize the data and results
         self._renormalize(n, result)
         if self._print_report:
             print(result.fit_report(show_correl=False))
         if self._plot:
             dims = np.unravel_index(n, self._map_shape)
             if self._inv_transpose is not None:
-                dims= tuple(dims[self._inv_transpose[i]] for i in range(len(dims)))
-            super().plot(result=result, y=np.asarray(self._ymap[dims]), plot_comp_legends=True,
-                skip_init=self._skip_init, title=str(dims))
-#RV        print(f'\n\nend FitMap._fit {n}\n')
-#RV        print(f'current_best_values = {current_best_values}')
-#        self._parameters.pretty_print()
-#        print(result.fit_report(show_correl=False))
-#RV        print(f'\nself._best_values_flat:\n{self._best_values_flat}\n\n')
+                dims = tuple(
+                    dims[self._inv_transpose[i]] for i in range(len(dims)))
+            super().plot(
+                result=result, y=np.asarray(self._ymap[dims]),
+                plot_comp_legends=True, skip_init=self._skip_init,
+                title=str(dims))
         if return_result:
-            return(result)
+            return result
+        return None
 
     def _renormalize(self, n, result):
         self._redchi_flat[n] = np.float64(result.redchi)
         self._success_flat[n] = result.success
         if self._norm is None or not self._normalized:
             self._best_fit_flat[n] = result.best_fit
             for i, name in enumerate(self._best_parameters):
-                self._best_values_flat[i][n] = np.float64(result.params[name].value)
-                self._best_errors_flat[i][n] = np.float64(result.params[name].stderr)
+                self._best_values_flat[i][n] = np.float64(
+                    result.params[name].value)
+                self._best_errors_flat[i][n] = np.float64(
+                    result.params[name].stderr)
         else:
             pars = set(self._parameter_norms) & set(self._best_parameters)
             for name, par in result.params.items():
                 if name in pars and self._parameter_norms[name]:
                     if par.stderr is not None:
                         par.stderr *= self._norm[1]
                     if par.expr is None:
                         par.value *= self._norm[1]
                         if self._print_report:
                             if par.init_value is not None:
                                 par.init_value *= self._norm[1]
-                            if not np.isinf(par.min) and abs(par.min) != float_min:
+                            if (not np.isinf(par.min)
+                                    and abs(par.min) != FLOAT_MIN):
                                 par.min *= self._norm[1]
-                            if not np.isinf(par.max) and abs(par.max) != float_min:
+                            if (not np.isinf(par.max)
+                                    and abs(par.max) != FLOAT_MIN):
                                 par.max *= self._norm[1]
-            self._best_fit_flat[n] = result.best_fit*self._norm[1]+self._norm[0]
+            self._best_fit_flat[n] = (
+                result.best_fit*self._norm[1] + self._norm[0])
             for i, name in enumerate(self._best_parameters):
-                self._best_values_flat[i][n] = np.float64(result.params[name].value)
-                self._best_errors_flat[i][n] = np.float64(result.params[name].stderr)
+                self._best_values_flat[i][n] = np.float64(
+                    result.params[name].value)
+                self._best_errors_flat[i][n] = np.float64(
+                    result.params[name].stderr)
             if self._plot:
                 if not self._skip_init:
-                    result.init_fit = result.init_fit*self._norm[1]+self._norm[0]
+                    result.init_fit = (
+                        result.init_fit*self._norm[1] + self._norm[0])
                 result.best_fit = np.copy(self._best_fit_flat[n])
```

### Comparing `ChessAnalysisPipeline-0.0.5/CHAP/common/utils/general.py` & `ChessAnalysisPipeline-0.0.6/CHAP/common/utils/general.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,77 +1,105 @@
 #!/usr/bin/env python3
-
-#FIX write a function that returns a list of peak indices for a given plot
-#FIX use raise_error concept on more functions to optionally raise an error
-
 # -*- coding: utf-8 -*-
+#pylint: disable=
 """
-Created on Mon Dec  6 15:36:22 2021
-
-@author: rv43
+File       : general.py
+Author     : Rolf Verberg <rolfverberg AT gmail dot com>
+Description: A collection of general modules
 """
+# RV write function that returns a list of peak indices for a given plot
+# RV use raise_error concept on more functions
 
-from logging import getLogger
-logger = getLogger(__name__)
-
+# System modules
 from ast import literal_eval
+from logging import getLogger
+from os import path as os_path
+from os import (
+    access,
+    R_OK,
+)
 from re import compile as re_compile
 from re import split as re_split
 from re import sub as re_sub
 from sys import float_info
 
+# Third party modules
 import numpy as np
 try:
     import matplotlib.pyplot as plt
     from matplotlib.widgets import Button
-except:
+except ImportError:
     pass
 
-def depth_list(L): return isinstance(L, list) and max(map(depth_list, L))+1
-def depth_tuple(T): return isinstance(T, tuple) and max(map(depth_tuple, T))+1
-def unwrap_tuple(T):
-    if depth_tuple(T) > 1 and len(T) == 1:
-        T = unwrap_tuple(*T)
-    return T
+logger = getLogger(__name__)
+
+
+def depth_list(_list):
+    """Return the depth of a list."""
+    return isinstance(_list, list) and 1+max(map(depth_list, _list))
+
+
+def depth_tuple(_tuple):
+    """Return the depth of a tuple."""
+    return isinstance(_tuple, tuple) and 1+max(map(depth_tuple, _tuple))
+
+
+def unwrap_tuple(_tuple):
+    """Unwrap a tuple."""
+    if depth_tuple(_tuple) > 1 and len(_tuple) == 1:
+        _tuple = unwrap_tuple(*_tuple)
+    return _tuple
+
 
 def illegal_value(value, name, location=None, raise_error=False, log=True):
+    """Print illegal value message and/or raise error."""
     if not isinstance(location, str):
         location = ''
     else:
         location = f'in {location} '
     if isinstance(name, str):
-        error_msg = f'Illegal value for {name} {location}({value}, {type(value)})'
+        error_msg = \
+            f'Illegal value for {name} {location}({value}, {type(value)})'
     else:
         error_msg = f'Illegal value {location}({value}, {type(value)})'
     if log:
         logger.error(error_msg)
     if raise_error:
         raise ValueError(error_msg)
 
-def illegal_combination(value1, name1, value2, name2, location=None, raise_error=False,
+
+def illegal_combination(
+        value1, name1, value2, name2, location=None, raise_error=False,
         log=True):
+    """Print illegal combination message and/or raise error."""
     if not isinstance(location, str):
         location = ''
     else:
         location = f'in {location} '
     if isinstance(name1, str):
-        error_msg = f'Illegal combination for {name1} and {name2} {location}'+ \
-                f'({value1}, {type(value1)} and {value2}, {type(value2)})'
+        error_msg = f'Illegal combination for {name1} and {name2} {location}' \
+            f'({value1}, {type(value1)} and {value2}, {type(value2)})'
     else:
-        error_msg = f'Illegal combination {location}'+ \
-                f'({value1}, {type(value1)} and {value2}, {type(value2)})'
+        error_msg = f'Illegal combination {location}' \
+            f'({value1}, {type(value1)} and {value2}, {type(value2)})'
     if log:
         logger.error(error_msg)
     if raise_error:
         raise ValueError(error_msg)
 
-def test_ge_gt_le_lt(ge, gt, le, lt, func, location=None, raise_error=False, log=True):
-    """Check individual and mutual validity of ge, gt, le, lt qualifiers
-       func: is_int or is_num to test for int or numbers
-       Return: True upon success or False when mutually exlusive
+
+def test_ge_gt_le_lt(
+        ge, gt, le, lt, func, location=None, raise_error=False, log=True):
+    """
+    Check individual and mutual validity of ge, gt, le, lt qualifiers.
+
+    :param func: Test for integers or numbers
+    :type func: callable: is_int, is_num
+    :return: True upon success or False when mutually exlusive
+    :rtype: bool
     """
     if ge is None and gt is None and le is None and lt is None:
         return True
     if ge is not None:
         if not func(ge):
             illegal_value(ge, 'ge', location, raise_error, log)
             return False
@@ -91,29 +119,32 @@
     elif lt is not None and not func(lt):
         illegal_value(lt, 'lt', location, raise_error, log)
         return False
     if ge is not None:
         if le is not None and ge > le:
             illegal_combination(ge, 'ge', le, 'le', location, raise_error, log)
             return False
-        elif lt is not None and ge >= lt:
+        if lt is not None and ge >= lt:
             illegal_combination(ge, 'ge', lt, 'lt', location, raise_error, log)
             return False
     elif gt is not None:
         if le is not None and gt >= le:
             illegal_combination(gt, 'gt', le, 'le', location, raise_error, log)
             return False
-        elif lt is not None and gt >= lt:
+        if lt is not None and gt >= lt:
             illegal_combination(gt, 'gt', lt, 'lt', location, raise_error, log)
             return False
     return True
 
+
 def range_string_ge_gt_le_lt(ge=None, gt=None, le=None, lt=None):
-    """Return a range string representation matching the ge, gt, le, lt qualifiers
-       Does not validate the inputs, do that as needed before calling
+    """
+    Return a range string representation matching the ge, gt, le, lt
+    qualifiers. Does not validate the inputs, do that as needed before
+    calling.
     """
     range_string = ''
     if ge is not None:
         if le is None and lt is None:
             range_string += f'>= {ge}'
         else:
             range_string += f'[{ge}, '
@@ -130,39 +161,53 @@
     elif lt is not None:
         if ge is None and gt is None:
             range_string += f'< {lt}'
         else:
             range_string += f'{lt})'
     return range_string
 
+
 def is_int(v, ge=None, gt=None, le=None, lt=None, raise_error=False, log=True):
-    """Value is an integer in range ge <= v <= le or gt < v < lt or some combination.
-       Return: True if yes or False is no
+    """
+    Value is an integer in range ge <= v <= le or gt < v < lt or some
+    combination.
+
+    :return: True if yes or False is no
+    :rtype: bool
     """
     return _is_int_or_num(v, 'int', ge, gt, le, lt, raise_error, log)
 
+
 def is_num(v, ge=None, gt=None, le=None, lt=None, raise_error=False, log=True):
-    """Value is a number in range ge <= v <= le or gt < v < lt or some combination.
-       Return: True if yes or False is no
+    """
+    Value is a number in range ge <= v <= le or gt < v < lt or some
+    combination.
+
+    :return: True if yes or False is no
+    :rtype: bool
     """
     return _is_int_or_num(v, 'num', ge, gt, le, lt, raise_error, log)
 
-def _is_int_or_num(v, type_str, ge=None, gt=None, le=None, lt=None, raise_error=False,
+
+def _is_int_or_num(
+        v, type_str, ge=None, gt=None, le=None, lt=None, raise_error=False,
         log=True):
     if type_str == 'int':
         if not isinstance(v, int):
             illegal_value(v, 'v', '_is_int_or_num', raise_error, log)
             return False
-        if not test_ge_gt_le_lt(ge, gt, le, lt, is_int, '_is_int_or_num', raise_error, log):
+        if not test_ge_gt_le_lt(
+                ge, gt, le, lt, is_int, '_is_int_or_num', raise_error, log):
             return False
     elif type_str == 'num':
         if not isinstance(v, (int, float)):
             illegal_value(v, 'v', '_is_int_or_num', raise_error, log)
             return False
-        if not test_ge_gt_le_lt(ge, gt, le, lt, is_num, '_is_int_or_num', raise_error, log):
+        if not test_ge_gt_le_lt(
+                ge, gt, le, lt, is_num, '_is_int_or_num', raise_error, log):
             return False
     else:
         illegal_value(type_str, 'type_str', '_is_int_or_num', raise_error, log)
         return False
     if ge is None and gt is None and le is None and lt is None:
         return True
     error = False
@@ -182,396 +227,502 @@
         if log:
             logger.error(error_msg)
         if raise_error:
             raise ValueError(error_msg)
         return False
     return True
 
-def is_int_pair(v, ge=None, gt=None, le=None, lt=None, raise_error=False, log=True):
-    """Value is an integer pair, each in range ge <= v[i] <= le or gt < v[i] < lt or
-           ge[i] <= v[i] <= le[i] or gt[i] < v[i] < lt[i] or some combination.
-       Return: True if yes or False is no
+
+def is_int_pair(
+        v, ge=None, gt=None, le=None, lt=None, raise_error=False, log=True):
+    """
+    Value is an integer pair, each in range ge <= v[i] <= le or
+    gt < v[i] < lt or ge[i] <= v[i] <= le[i] or gt[i] < v[i] < lt[i]
+    or some combination.
+
+    :return: True if yes or False is no
+    :rtype: bool
     """
     return _is_int_or_num_pair(v, 'int', ge, gt, le, lt, raise_error, log)
 
-def is_num_pair(v, ge=None, gt=None, le=None, lt=None, raise_error=False, log=True):
-    """Value is a number pair, each in range ge <= v[i] <= le or gt < v[i] < lt or
-           ge[i] <= v[i] <= le[i] or gt[i] < v[i] < lt[i] or some combination.
-       Return: True if yes or False is no
+
+def is_num_pair(
+        v, ge=None, gt=None, le=None, lt=None, raise_error=False, log=True):
+    """
+    Value is a number pair, each in range ge <= v[i] <= le or
+    gt < v[i] < lt or ge[i] <= v[i] <= le[i] or gt[i] < v[i] < lt[i]
+    or some combination.
+
+    :return: True if yes or False is no
+    :rtype: bool
     """
     return _is_int_or_num_pair(v, 'num', ge, gt, le, lt, raise_error, log)
 
-def _is_int_or_num_pair(v, type_str, ge=None, gt=None, le=None, lt=None, raise_error=False,
+
+def _is_int_or_num_pair(
+        v, type_str, ge=None, gt=None, le=None, lt=None, raise_error=False,
         log=True):
     if type_str == 'int':
-        if not (isinstance(v, (tuple, list)) and len(v) == 2 and isinstance(v[0], int) and
-                isinstance(v[1], int)):
+        if not (isinstance(v, (tuple, list)) and len(v) == 2
+                and isinstance(v[0], int) and isinstance(v[1], int)):
             illegal_value(v, 'v', '_is_int_or_num_pair', raise_error, log)
             return False
         func = is_int
     elif type_str == 'num':
-        if not (isinstance(v, (tuple, list)) and len(v) == 2 and isinstance(v[0], (int, float)) and
-                isinstance(v[1], (int, float))):
+        if not (isinstance(v, (tuple, list)) and len(v) == 2
+                and isinstance(v[0], (int, float))
+                and isinstance(v[1], (int, float))):
             illegal_value(v, 'v', '_is_int_or_num_pair', raise_error, log)
             return False
         func = is_num
     else:
-        illegal_value(type_str, 'type_str', '_is_int_or_num_pair', raise_error, log)
+        illegal_value(
+            type_str, 'type_str', '_is_int_or_num_pair', raise_error, log)
         return False
     if ge is None and gt is None and le is None and lt is None:
         return True
     if ge is None or func(ge, log=True):
         ge = 2*[ge]
-    elif not _is_int_or_num_pair(ge, type_str, raise_error=raise_error, log=log):
+    elif not _is_int_or_num_pair(
+            ge, type_str, raise_error=raise_error, log=log):
         return False
     if gt is None or func(gt, log=True):
         gt = 2*[gt]
-    elif not _is_int_or_num_pair(gt, type_str, raise_error=raise_error, log=log):
+    elif not _is_int_or_num_pair(
+            gt, type_str, raise_error=raise_error, log=log):
         return False
     if le is None or func(le, log=True):
         le = 2*[le]
-    elif not _is_int_or_num_pair(le, type_str, raise_error=raise_error, log=log):
+    elif not _is_int_or_num_pair(
+            le, type_str, raise_error=raise_error, log=log):
         return False
     if lt is None or func(lt, log=True):
         lt = 2*[lt]
-    elif not _is_int_or_num_pair(lt, type_str, raise_error=raise_error, log=log):
+    elif not _is_int_or_num_pair(
+            lt, type_str, raise_error=raise_error, log=log):
         return False
-    if (not func(v[0], ge[0], gt[0], le[0], lt[0], raise_error, log) or
-            not func(v[1], ge[1], gt[1], le[1], lt[1], raise_error, log)):
+    if (not func(v[0], ge[0], gt[0], le[0], lt[0], raise_error, log)
+            or not func(v[1], ge[1], gt[1], le[1], lt[1], raise_error, log)):
         return False
     return True
 
-def is_int_series(l, ge=None, gt=None, le=None, lt=None, raise_error=False, log=True):
-    """Value is a tuple or list of integers, each in range ge <= l[i] <= le or
-       gt < l[i] < lt or some combination.
+
+def is_int_series(
+        t_or_l, ge=None, gt=None, le=None, lt=None, raise_error=False,
+        log=True):
+    """
+    Value is a tuple or list of integers, each in range
+    ge <= l[i] <= le or gt < l[i] < lt or some combination.
     """
-    if not test_ge_gt_le_lt(ge, gt, le, lt, is_int, 'is_int_series', raise_error, log):
+    if not test_ge_gt_le_lt(
+            ge, gt, le, lt, is_int, 'is_int_series', raise_error, log):
         return False
-    if not isinstance(l, (tuple, list)):
-        illegal_value(l, 'l', 'is_int_series', raise_error, log)
+    if not isinstance(t_or_l, (tuple, list)):
+        illegal_value(t_or_l, 't_or_l', 'is_int_series', raise_error, log)
         return False
-    if any(True if not is_int(v, ge, gt, le, lt, raise_error, log) else False for v in l):
+    if any(not is_int(v, ge, gt, le, lt, raise_error, log) for v in t_or_l):
         return False
     return True
 
-def is_num_series(l, ge=None, gt=None, le=None, lt=None, raise_error=False, log=True):
-    """Value is a tuple or list of numbers, each in range ge <= l[i] <= le or
-       gt < l[i] < lt or some combination.
+
+def is_num_series(
+        t_or_l, ge=None, gt=None, le=None, lt=None, raise_error=False,
+        log=True):
     """
-    if not test_ge_gt_le_lt(ge, gt, le, lt, is_int, 'is_int_series', raise_error, log):
+    Value is a tuple or list of numbers, each in range ge <= l[i] <= le
+    or gt < l[i] < lt or some combination.
+    """
+    if not test_ge_gt_le_lt(
+            ge, gt, le, lt, is_int, 'is_int_series', raise_error, log):
         return False
-    if not isinstance(l, (tuple, list)):
-        illegal_value(l, 'l', 'is_num_series', raise_error, log)
+    if not isinstance(t_or_l, (tuple, list)):
+        illegal_value(t_or_l, 't_or_l', 'is_num_series', raise_error, log)
         return False
-    if any(True if not is_num(v, ge, gt, le, lt, raise_error, log) else False for v in l):
+    if any(not is_num(v, ge, gt, le, lt, raise_error, log) for v in t_or_l):
         return False
     return True
 
-def is_str_series(l, raise_error=False, log=True):
-    """Value is a tuple or list of strings.
+
+def is_str_series(t_or_l, raise_error=False, log=True):
     """
-    if (not isinstance(l, (tuple, list)) or
-            any(True if not isinstance(s, str) else False for s in l)):
-        illegal_value(l, 'l', 'is_str_series', raise_error, log)
+    Value is a tuple or list of strings.
+    """
+    if (not isinstance(t_or_l, (tuple, list))
+            or any(not isinstance(s, str) for s in t_or_l)):
+        illegal_value(t_or_l, 't_or_l', 'is_str_series', raise_error, log)
         return False
     return True
 
-def is_dict_series(l, raise_error=False, log=True):
-    """Value is a tuple or list of dictionaries.
+
+def is_dict_series(t_or_l, raise_error=False, log=True):
     """
-    if (not isinstance(l, (tuple, list)) or
-            any(True if not isinstance(d, dict) else False for d in l)):
-        illegal_value(l, 'l', 'is_dict_series', raise_error, log)
+    Value is a tuple or list of dictionaries.
+    """
+    if (not isinstance(t_or_l, (tuple, list))
+            or any(not isinstance(d, dict) for d in t_or_l)):
+        illegal_value(t_or_l, 't_or_l', 'is_dict_series', raise_error, log)
         return False
     return True
 
-def is_dict_nums(l, raise_error=False, log=True):
-    """Value is a dictionary with single number values
+
+def is_dict_nums(d, raise_error=False, log=True):
     """
-    if (not isinstance(l, dict) or
-            any(True if not is_num(v, log=False) else False for v in l.values())):
-        illegal_value(l, 'l', 'is_dict_nums', raise_error, log)
+    Value is a dictionary with single number values
+    """
+    if (not isinstance(d, dict)
+            or any(not is_num(v, log=False) for v in d.values())):
+        illegal_value(d, 'd', 'is_dict_nums', raise_error, log)
         return False
     return True
 
-def is_dict_strings(l, raise_error=False, log=True):
-    """Value is a dictionary with single string values
+
+def is_dict_strings(d, raise_error=False, log=True):
     """
-    if (not isinstance(l, dict) or
-            any(True if not isinstance(v, str) else False for v in l.values())):
-        illegal_value(l, 'l', 'is_dict_strings', raise_error, log)
+    Value is a dictionary with single string values
+    """
+    if (not isinstance(d, dict)
+            or any(not isinstance(v, str) for v in d.values())):
+        illegal_value(d, 'd', 'is_dict_strings', raise_error, log)
         return False
     return True
 
+
 def is_index(v, ge=0, lt=None, raise_error=False, log=True):
-    """Value is an array index in range ge <= v < lt.
-       NOTE lt IS NOT included!
+    """
+    Value is an array index in range ge <= v < lt. NOTE lt IS NOT
+    included!
     """
     if isinstance(lt, int):
         if lt <= ge:
-            illegal_combination(ge, 'ge', lt, 'lt', 'is_index', raise_error, log)
+            illegal_combination(
+                ge, 'ge', lt, 'lt', 'is_index', raise_error, log)
             return False
     return is_int(v, ge=ge, lt=lt, raise_error=raise_error, log=log)
 
+
 def is_index_range(v, ge=0, le=None, lt=None, raise_error=False, log=True):
-    """Value is an array index range in range ge <= v[0] <= v[1] <= le or ge <= v[0] <= v[1] < lt.
-       NOTE le IS included!
+    """
+    Value is an array index range in range ge <= v[0] <= v[1] <= le or
+    ge <= v[0] <= v[1] < lt. NOTE le IS included!
     """
     if not is_int_pair(v, raise_error=raise_error, log=log):
         return False
-    if not test_ge_gt_le_lt(ge, None, le, lt, is_int, 'is_index_range', raise_error, log):
+    if not test_ge_gt_le_lt(
+            ge, None, le, lt, is_int, 'is_index_range', raise_error, log):
         return False
-    if not ge <= v[0] <= v[1] or (le is not None and v[1] > le) or (lt is not None and v[1] >= lt):
+    if (not ge <= v[0] <= v[1] or (le is not None and v[1] > le)
+            or (lt is not None and v[1] >= lt)):
         if le is not None:
-            error_msg = f'Value {v} out of range: !({ge} <= {v[0]} <= {v[1]} <= {le})'
+            error_msg = \
+                f'Value {v} out of range: !({ge} <= {v[0]} <= {v[1]} <= {le})'
         else:
-            error_msg = f'Value {v} out of range: !({ge} <= {v[0]} <= {v[1]} < {lt})'
+            error_msg = \
+                f'Value {v} out of range: !({ge} <= {v[0]} <= {v[1]} < {lt})'
         if log:
             logger.error(error_msg)
         if raise_error:
             raise ValueError(error_msg)
         return False
     return True
 
+
 def index_nearest(a, value):
+    """Return index of nearest array value."""
     a = np.asarray(a)
     if a.ndim > 1:
-        raise ValueError(f'Invalid array dimension for parameter a ({a.ndim}, {a})')
+        raise ValueError(
+            f'Invalid array dimension for parameter a ({a.ndim}, {a})')
     # Round up for .5
     value *= 1.0+float_info.epsilon
     return (int)(np.argmin(np.abs(a-value)))
 
+
 def index_nearest_low(a, value):
+    """Return index of nearest array value, rounded down"""
     a = np.asarray(a)
     if a.ndim > 1:
-        raise ValueError(f'Invalid array dimension for parameter a ({a.ndim}, {a})')
+        raise ValueError(
+            f'Invalid array dimension for parameter a ({a.ndim}, {a})')
     index = int(np.argmin(np.abs(a-value)))
     if value < a[index] and index > 0:
         index -= 1
     return index
 
+
 def index_nearest_upp(a, value):
+    """Return index of nearest array value, rounded upp."""
     a = np.asarray(a)
     if a.ndim > 1:
-        raise ValueError(f'Invalid array dimension for parameter a ({a.ndim}, {a})')
+        raise ValueError(
+            f'Invalid array dimension for parameter a ({a.ndim}, {a})')
     index = int(np.argmin(np.abs(a-value)))
     if value > a[index] and index < a.size-1:
         index += 1
     return index
 
+
 def round_to_n(x, n=1):
+    """Round to a specific number of decimals."""
     if x == 0.0:
         return 0
-    else:
-        return type(x)(round(x, n-1-int(np.floor(np.log10(abs(x))))))
+    return type(x)(round(x, n-1-int(np.floor(np.log10(abs(x))))))
+
 
 def round_up_to_n(x, n=1):
-    xr = round_to_n(x, n)
-    if abs(x/xr) > 1.0:
-        xr += np.sign(x)*10**(np.floor(np.log10(abs(x)))+1-n)
-    return type(x)(xr)
+    """Round up to a specific number of decimals."""
+    x_round = round_to_n(x, n)
+    if abs(x/x_round) > 1.0:
+        x_round += np.sign(x) * 10**(np.floor(np.log10(abs(x)))+1-n)
+    return type(x)(x_round)
+
 
 def trunc_to_n(x, n=1):
-    xr = round_to_n(x, n)
-    if abs(xr/x) > 1.0:
-        xr -= np.sign(x)*10**(np.floor(np.log10(abs(x)))+1-n)
-    return type(x)(xr)
+    """Truncate to a specific number of decimals."""
+    x_round = round_to_n(x, n)
+    if abs(x_round/x) > 1.0:
+        x_round -= np.sign(x) * 10**(np.floor(np.log10(abs(x)))+1-n)
+    return type(x)(x_round)
+
 
 def almost_equal(a, b, sig_figs):
+    """
+    Check if equal to within a certain number of significant digits.
+    """
     if is_num(a) and is_num(b):
-        return abs(round_to_n(a-b, sig_figs)) < pow(10, -sig_figs+1)
-    else:
-        raise ValueError(f'Invalid value for a or b in almost_equal (a: {a}, {type(a)}, '+
-                f'b: {b}, {type(b)})')
-        return False
+        return abs(round_to_n(a-b, sig_figs)) < pow(10, 1-sig_figs)
+    raise ValueError(
+        f'Invalid value for a or b in almost_equal (a: {a}, {type(a)}, '
+        f'b: {b}, {type(b)})')
+
 
 def string_to_list(s, split_on_dash=True, remove_duplicates=True, sort=True):
-    """Return a list of numbers by splitting/expanding a string on any combination of
-       commas, whitespaces, or dashes (when split_on_dash=True)
-       e.g: '1, 3, 5-8, 12 ' -> [1, 3, 5, 6, 7, 8, 12]
+    """
+    Return a list of numbers by splitting/expanding a string on any
+    combination of commas, whitespaces, or dashes (when
+    split_on_dash=True).
+    e.g: '1, 3, 5-8, 12 ' -> [1, 3, 5, 6, 7, 8, 12]
     """
     if not isinstance(s, str):
-        illegal_value(s, location='string_to_list')
+        illegal_value(s, 's', location='string_to_list')
         return None
-    if not len(s):
+    if not s:
         return []
     try:
-        ll = [x for x in re_split('\s+,\s+|\s+,|,\s+|\s+|,', s.strip())]
+        list1 = re_split(r'\s+,\s+|\s+,|,\s+|\s+|,', s.strip())
     except (ValueError, TypeError, SyntaxError, MemoryError, RecursionError):
         return None
     if split_on_dash:
         try:
-            l = []
-            for l1 in ll:
-                l2 = [literal_eval(x) for x in re_split('\s+-\s+|\s+-|-\s+|\s+|-', l1)]
-                if len(l2) == 1:
-                    l += l2
-                elif len(l2) == 2 and l2[1] > l2[0]:
-                    l += [i for i in range(l2[0], l2[1]+1)]
+            l_of_i = []
+            for v in list1:
+                list2 = [
+                    literal_eval(x)
+                    for x in re_split(r'\s+-\s+|\s+-|-\s+|\s+|-', v)]
+                if len(list2) == 1:
+                    l_of_i += list2
+                elif len(list2) == 2 and list2[1] > list2[0]:
+                    l_of_i += list(range(list2[0], 1+list2[1]))
                 else:
                     raise ValueError
-        except (ValueError, TypeError, SyntaxError, MemoryError, RecursionError):
+        except (ValueError, TypeError, SyntaxError, MemoryError,
+                RecursionError):
             return None
     else:
-        l = [literal_eval(x) for x in ll]
+        l_of_i = [literal_eval(x) for x in list1]
     if remove_duplicates:
-        l = list(dict.fromkeys(l))
+        l_of_i = list(dict.fromkeys(l_of_i))
     if sort:
-        l = sorted(l)
-    return l
+        l_of_i = sorted(l_of_i)
+    return l_of_i
+
 
 def get_trailing_int(string):
-    indexRegex = re_compile(r'\d+$')
-    mo = indexRegex.search(string)
-    if mo is None:
+    """Get the trailing integer in a string."""
+    index_regex = re_compile(r'\d+$')
+    match = index_regex.search(string)
+    if match is None:
         return None
-    else:
-        return int(mo.group())
+    return int(match.group())
 
-def input_int(s=None, ge=None, gt=None, le=None, lt=None, default=None, inset=None,
+
+def input_int(
+        s=None, ge=None, gt=None, le=None, lt=None, default=None, inset=None,
         raise_error=False, log=True):
-    return _input_int_or_num('int', s, ge, gt, le, lt, default, inset, raise_error, log)
+    """Interactively prompt the user to enter an integer."""
+    return _input_int_or_num(
+        'int', s, ge, gt, le, lt, default, inset, raise_error, log)
 
-def input_num(s=None, ge=None, gt=None, le=None, lt=None, default=None, raise_error=False,
-        log=True):
-    return _input_int_or_num('num', s, ge, gt, le, lt, default, None, raise_error,log)
 
-def _input_int_or_num(type_str, s=None, ge=None, gt=None, le=None, lt=None, default=None,
+def input_num(
+        s=None, ge=None, gt=None, le=None, lt=None, default=None,
+        raise_error=False, log=True):
+    """Interactively prompt the user to enter a number."""
+    return _input_int_or_num(
+        'num', s, ge, gt, le, lt, default, None, raise_error,log)
+
+
+def _input_int_or_num(
+        type_str, s=None, ge=None, gt=None, le=None, lt=None, default=None,
         inset=None, raise_error=False, log=True):
+    """Interactively prompt the user to enter an integer or number."""
     if type_str == 'int':
-        if not test_ge_gt_le_lt(ge, gt, le, lt, is_int, '_input_int_or_num', raise_error, log):
+        if not test_ge_gt_le_lt(
+                ge, gt, le, lt, is_int, '_input_int_or_num', raise_error, log):
             return None
     elif type_str == 'num':
-        if not test_ge_gt_le_lt(ge, gt, le, lt, is_num, '_input_int_or_num', raise_error, log):
+        if not test_ge_gt_le_lt(
+                ge, gt, le, lt, is_num, '_input_int_or_num', raise_error, log):
             return None
     else:
-        illegal_value(type_str, 'type_str', '_input_int_or_num', raise_error, log)
+        illegal_value(
+            type_str, 'type_str', '_input_int_or_num', raise_error, log)
         return None
     if default is not None:
-        if not _is_int_or_num(default, type_str, raise_error=raise_error, log=log):
+        if not _is_int_or_num(
+                default, type_str, raise_error=raise_error, log=log):
             return None
         if ge is not None and default < ge:
-            illegal_combination(ge, 'ge', default, 'default', '_input_int_or_num', raise_error,
+            illegal_combination(
+                ge, 'ge', default, 'default', '_input_int_or_num', raise_error,
                 log)
             return None
         if gt is not None and default <= gt:
-            illegal_combination(gt, 'gt', default, 'default', '_input_int_or_num', raise_error,
+            illegal_combination(
+                gt, 'gt', default, 'default', '_input_int_or_num', raise_error,
                 log)
             return None
         if le is not None and default > le:
-            illegal_combination(le, 'le', default, 'default', '_input_int_or_num', raise_error,
+            illegal_combination(
+                le, 'le', default, 'default', '_input_int_or_num', raise_error,
                 log)
             return None
         if lt is not None and default >= lt:
-            illegal_combination(lt, 'lt', default, 'default', '_input_int_or_num', raise_error,
+            illegal_combination(
+                lt, 'lt', default, 'default', '_input_int_or_num', raise_error,
                 log)
             return None
         default_string = f' [{default}]'
     else:
         default_string = ''
     if inset is not None:
-        if (not isinstance(inset, (tuple, list)) or any(True if not isinstance(i, int) else
-                False for i in inset)):
-            illegal_value(inset, 'inset', '_input_int_or_num', raise_error, log)
+        if (not isinstance(inset, (tuple, list))
+                or any(not isinstance(i, int) for i in inset)):
+            illegal_value(
+                inset, 'inset', '_input_int_or_num', raise_error, log)
             return None
     v_range = f'{range_string_ge_gt_le_lt(ge, gt, le, lt)}'
-    if len(v_range):
+    if v_range:
         v_range = f' {v_range}'
     if s is None:
         if type_str == 'int':
             print(f'Enter an integer{v_range}{default_string}: ')
         else:
             print(f'Enter a number{v_range}{default_string}: ')
     else:
         print(f'{s}{v_range}{default_string}: ')
     try:
         i = input()
-        if isinstance(i, str) and not len(i):
+        if isinstance(i, str) and not i:
             v = default
             print(f'{v}')
         else:
             v = literal_eval(i)
         if inset and v not in inset:
-           raise ValueError(f'{v} not part of the set {inset}')
+            raise ValueError(f'{v} not part of the set {inset}')
     except (ValueError, TypeError, SyntaxError, MemoryError, RecursionError):
         v = None
-    except:
-        if log:
-            logger.error('Unexpected error')
-        if raise_error:
-            raise ValueError('Unexpected error')
     if not _is_int_or_num(v, type_str, ge, gt, le, lt):
-        v = _input_int_or_num(type_str, s, ge, gt, le, lt, default, inset, raise_error, log)
+        v = _input_int_or_num(
+            type_str, s, ge, gt, le, lt, default, inset, raise_error, log)
     return v
 
-def input_int_list(s=None, ge=None, le=None, split_on_dash=True, remove_duplicates=True,
+
+def input_int_list(
+        s=None, ge=None, le=None, split_on_dash=True, remove_duplicates=True,
         sort=True, raise_error=False, log=True):
-    """Prompt the user to input a list of interger and split the entered string on any combination
-       of commas, whitespaces, or dashes (when split_on_dash is True)
-       e.g: '1 3,5-8 , 12 ' -> [1, 3, 5, 6, 7, 8, 12]
-       remove_duplicates: removes duplicates if True (may also change the order)
-       sort: sort in ascending order if True
-       return None upon an illegal input
     """
-    return _input_int_or_num_list('int', s, ge, le, split_on_dash, remove_duplicates, sort,
-        raise_error, log)
-
-def input_num_list(s=None, ge=None, le=None, remove_duplicates=True, sort=True, raise_error=False,
-        log=True):
-    """Prompt the user to input a list of numbers and split the entered string on any combination
-       of commas or whitespaces
-       e.g: '1.0, 3, 5.8, 12 ' -> [1.0, 3.0, 5.8, 12.0]
-       remove_duplicates: removes duplicates if True (may also change the order)
-       sort: sort in ascending order if True
-       return None upon an illegal input
+    Prompt the user to input a list of interger and split the entered
+    string on any combination of commas, whitespaces, or dashes (when
+    split_on_dash is True).
+    e.g: '1 3,5-8 , 12 ' -> [1, 3, 5, 6, 7, 8, 12]
+
+    remove_duplicates: removes duplicates if True (may also change the
+        order)
+    sort: sort in ascending order if True
+    return None upon an illegal input
     """
-    return _input_int_or_num_list('num', s, ge, le, False, remove_duplicates, sort, raise_error,
+    return _input_int_or_num_list(
+        'int', s, ge, le, split_on_dash, remove_duplicates, sort, raise_error,
         log)
 
-def _input_int_or_num_list(type_str, s=None, ge=None, le=None, split_on_dash=True,
+
+def input_num_list(
+        s=None, ge=None, le=None, remove_duplicates=True, sort=True,
+        raise_error=False, log=True):
+    """
+    Prompt the user to input a list of numbers and split the entered
+    string on any combination of commas or whitespaces.
+    e.g: '1.0, 3, 5.8, 12 ' -> [1.0, 3.0, 5.8, 12.0]
+
+    remove_duplicates: removes duplicates if True (may also change the
+        order)
+    sort: sort in ascending order if True
+    return None upon an illegal input
+    """
+    return _input_int_or_num_list(
+        'num', s, ge, le, False, remove_duplicates, sort, raise_error, log)
+
+
+def _input_int_or_num_list(
+        type_str, s=None, ge=None, le=None, split_on_dash=True,
         remove_duplicates=True, sort=True, raise_error=False, log=True):
-    #FIX do we want a limit on max dimension?
+    # RV do we want a limit on max dimension?
     if type_str == 'int':
-        if not test_ge_gt_le_lt(ge, None, le, None, is_int, 'input_int_or_num_list', raise_error,
-                log):
+        if not test_ge_gt_le_lt(
+                ge, None, le, None, is_int, 'input_int_or_num_list',
+                raise_error, log):
             return None
     elif type_str == 'num':
-        if not test_ge_gt_le_lt(ge, None, le, None, is_num, 'input_int_or_num_list', raise_error,
-                log):
+        if not test_ge_gt_le_lt(
+                ge, None, le, None, is_num, 'input_int_or_num_list',
+                raise_error, log):
             return None
     else:
         illegal_value(type_str, 'type_str', '_input_int_or_num_list')
         return None
     v_range = f'{range_string_ge_gt_le_lt(ge=ge, le=le)}'
-    if len(v_range):
+    if v_range:
         v_range = f' (each value in {v_range})'
     if s is None:
         print(f'Enter a series of integers{v_range}: ')
     else:
         print(f'{s}{v_range}: ')
     try:
-        l = string_to_list(input(), split_on_dash, remove_duplicates, sort)
+        _list = string_to_list(input(), split_on_dash, remove_duplicates, sort)
     except (ValueError, TypeError, SyntaxError, MemoryError, RecursionError):
-        l = None
+        _list = None
     except:
         print('Unexpected error')
         raise
-    if (not isinstance(l, list) or
-            any(True if not _is_int_or_num(v, type_str, ge=ge, le=le) else False for v in l)):
+    if (not isinstance(_list, list) or any(
+            not _is_int_or_num(v, type_str, ge=ge, le=le) for v in _list)):
         if split_on_dash:
-            print('Invalid input: enter a valid set of dash/comma/whitespace separated integers '+
-                    'e.g. 1 3,5-8 , 12')
+            print('Invalid input: enter a valid set of dash/comma/whitespace '
+                  'separated integers e.g. 1 3,5-8 , 12')
         else:
-            print('Invalid input: enter a valid set of comma/whitespace separated integers '+
-                    'e.g. 1 3,5 8 , 12')
-        l = _input_int_or_num_list(type_str, s, ge, le, split_on_dash, remove_duplicates, sort,
+            print('Invalid input: enter a valid set of comma/whitespace '
+                  'separated integers e.g. 1 3,5 8 , 12')
+        _list = _input_int_or_num_list(
+            type_str, s, ge, le, split_on_dash, remove_duplicates, sort,
             raise_error, log)
-    return l
+    return _list
+
 
 def input_yesno(s=None, default=None):
+    """Interactively prompt the user to enter a y/n question."""
     if default is not None:
         if not isinstance(default, str):
             illegal_value(default, 'default', 'input_yesno')
             return None
         if default.lower() in 'yes':
             default = 'y'
         elif default.lower() in 'no':
@@ -583,49 +734,53 @@
     else:
         default_string = ''
     if s is None:
         print(f'Enter yes or no{default_string}: ')
     else:
         print(f'{s}{default_string}: ')
     i = input()
-    if isinstance(i, str) and not len(i):
+    if isinstance(i, str) and not i:
         i = default
         print(f'{i}')
     if i is not None and i.lower() in 'yes':
         v = True
     elif i is not None and i.lower() in 'no':
         v = False
     else:
         print('Invalid input, enter yes or no')
         v = input_yesno(s, default)
     return v
 
+
 def input_menu(items, default=None, header=None):
-    if not isinstance(items, (tuple, list)) or any(True if not isinstance(i, str) else False
-            for i in items):
+    """Interactively prompt the user to select from a menu."""
+    if (not isinstance(items, (tuple, list))
+            or any(not isinstance(i, str) for i in items)):
         illegal_value(items, 'items', 'input_menu')
         return None
     if default is not None:
         if not (isinstance(default, str) and default in items):
-            logger.error(f'Invalid value for default ({default}), must be in {items}')
+            logger.error(
+                f'Invalid value for default ({default}), must be in {items}')
             return None
-        default_string = f' [{items.index(default)+1}]'
+        default_string = f' [{1+items.index(default)}]'
     else:
         default_string = ''
     if header is None:
-        print(f'Choose one of the following items (1, {len(items)}){default_string}:')
+        print('Choose one of the following items '
+              f'(1, {len(items)}){default_string}:')
     else:
         print(f'{header} (1, {len(items)}){default_string}:')
     for i, choice in enumerate(items):
         print(f'  {i+1}: {choice}')
     try:
-        choice  = input()
-        if isinstance(choice, str) and not len(choice):
+        choice = input()
+        if isinstance(choice, str) and not choice:
             choice = items.index(default)
-            print(f'{choice+1}')
+            print(f'{1+choice}')
         else:
             choice = literal_eval(choice)
             if isinstance(choice, int) and 1 <= choice <= len(items):
                 choice -= 1
             else:
                 raise ValueError
     except (ValueError, TypeError, SyntaxError, MemoryError, RecursionError):
@@ -634,149 +789,193 @@
         print('Unexpected error')
         raise
     if choice is None:
         print(f'Invalid choice, enter a number between 1 and {len(items)}')
         choice = input_menu(items, default)
     return choice
 
-def assert_no_duplicates_in_list_of_dicts(l: list, raise_error=False) -> list:
-    if not isinstance(l, list):
-        illegal_value(l, 'l', 'assert_no_duplicates_in_list_of_dicts', raise_error)
-        return None
-    if any(True if not isinstance(d, dict) else False for d in l):
-        illegal_value(l, 'l', 'assert_no_duplicates_in_list_of_dicts', raise_error)
+
+def assert_no_duplicates_in_list_of_dicts(_list, raise_error=False):
+    """
+    Assert that there are no duplicates in a list of dictionaries.
+    """
+    if not isinstance(_list, list):
+        illegal_value(
+            _list, '_list', 'assert_no_duplicates_in_list_of_dicts',
+            raise_error)
+        return None
+    if any(not isinstance(d, dict) for d in _list):
+        illegal_value(
+            _list, '_list', 'assert_no_duplicates_in_list_of_dicts',
+            raise_error)
         return None
-    if len(l) != len([dict(t) for t in {tuple(sorted(d.items())) for d in l}]):
+    if (len(_list) != len([dict(_tuple) for _tuple in
+                          {tuple(sorted(d.items())) for d in _list}])):
         if raise_error:
-            raise ValueError(f'Duplicate items found in {l}')
-        else:
-            logger.error(f'Duplicate items found in {l}')
+            raise ValueError(f'Duplicate items found in {_list}')
+        logger.error(f'Duplicate items found in {_list}')
         return None
-    else:
-        return l
+    return _list
+
 
-def assert_no_duplicate_key_in_list_of_dicts(l: list, key: str, raise_error=False) -> list:
+def assert_no_duplicate_key_in_list_of_dicts(_list, key, raise_error=False):
+    """
+    Assert that there are no duplicate keys in a list of dictionaries.
+    """
     if not isinstance(key, str):
-        illegal_value(key, 'key', 'assert_no_duplicate_key_in_list_of_dicts', raise_error)
-        return None
-    if not isinstance(l, list):
-        illegal_value(l, 'l', 'assert_no_duplicate_key_in_list_of_dicts', raise_error)
-        return None
-    if any(True if not isinstance(d, dict) else False for d in l):
-        illegal_value(l, 'l', 'assert_no_duplicates_in_list_of_dicts', raise_error)
+        illegal_value(
+            key, 'key', 'assert_no_duplicate_key_in_list_of_dicts',
+            raise_error)
+        return None
+    if not isinstance(_list, list):
+        illegal_value(
+            _list, '_list', 'assert_no_duplicate_key_in_list_of_dicts',
+            raise_error)
+        return None
+    if any(isinstance(d, dict) for d in _list):
+        illegal_value(
+            _list, '_list', 'assert_no_duplicates_in_list_of_dicts',
+            raise_error)
         return None
-    keys = [d.get(key, None) for d in l]
-    if None in keys or len(set(keys)) != len(l):
+    keys = [d.get(key, None) for d in _list]
+    if None in keys or len(set(keys)) != len(_list):
         if raise_error:
-            raise ValueError(f'Duplicate or missing key ({key}) found in {l}')
-        else:
-            logger.error(f'Duplicate or missing key ({key}) found in {l}')
+            raise ValueError(
+                f'Duplicate or missing key ({key}) found in {_list}')
+        logger.error(f'Duplicate or missing key ({key}) found in {_list}')
         return None
-    else:
-        return l
+    return _list
 
-def assert_no_duplicate_attr_in_list_of_objs(l: list, attr: str, raise_error=False) -> list:
+
+def assert_no_duplicate_attr_in_list_of_objs(_list, attr, raise_error=False):
+    """
+    Assert that there are no duplicate attributes in a list of objects.
+    """
     if not isinstance(attr, str):
-        illegal_value(attr, 'attr', 'assert_no_duplicate_attr_in_list_of_objs', raise_error)
-        return None
-    if not isinstance(l, list):
-        illegal_value(l, 'l', 'assert_no_duplicate_key_in_list_of_objs', raise_error)
+        illegal_value(
+            attr, 'attr', 'assert_no_duplicate_attr_in_list_of_objs',
+            raise_error)
+        return None
+    if not isinstance(_list, list):
+        illegal_value(
+            _list, '_list', 'assert_no_duplicate_key_in_list_of_objs',
+            raise_error)
         return None
-    attrs = [getattr(obj, attr, None) for obj in l]
-    if None in attrs or len(set(attrs)) != len(l):
+    attrs = [getattr(obj, attr, None) for obj in _list]
+    if None in attrs or len(set(attrs)) != len(_list):
         if raise_error:
-            raise ValueError(f'Duplicate or missing attr ({attr}) found in {l}')
-        else:
-            logger.error(f'Duplicate or missing attr ({attr}) found in {l}')
-        return None
-    else:
-        return l
-
-def file_exists_and_readable(path):
-    import os
-    if not os.path.isfile(path):
-        raise ValueError(f'{path} is not a valid file')
-    elif not os.access(path, os.R_OK):
-        raise ValueError(f'{path} is not accessible for reading')
-    else:
-        return path
-
-def draw_mask_1d(ydata, xdata=None, current_index_ranges=None, current_mask=None,
-        select_mask=True, num_index_ranges_max=None, title=None, legend=None, test_mode=False):
-    #FIX make color blind friendly
-    def draw_selections(ax, current_include, current_exclude, selected_index_ranges):
+            raise ValueError(
+                f'Duplicate or missing attr ({attr}) found in {_list}')
+        logger.error(f'Duplicate or missing attr ({attr}) found in {_list}')
+        return None
+    return _list
+
+
+def file_exists_and_readable(f):
+    """Check if a file exists and is readable."""
+    if not os_path.isfile(f):
+        raise ValueError(f'{f} is not a valid file')
+    if not access(f, R_OK):
+        raise ValueError(f'{f} is not accessible for reading')
+    return f
+
+
+def draw_mask_1d(
+        ydata, xdata=None, current_index_ranges=None, current_mask=None,
+        select_mask=True, num_index_ranges_max=None, title=None, legend=None,
+        test_mode=False):
+    """Display a 2D plot and have the user select a mask."""
+    # RV make color blind friendly
+    def draw_selections(
+            ax, current_include, current_exclude, selected_index_ranges):
+        """Draw the selections."""
         ax.clear()
         ax.set_title(title)
         ax.legend([legend])
         ax.plot(xdata, ydata, 'k')
-        for (low, upp) in current_include:
-            xlow = 0.5*(xdata[max(0, low-1)]+xdata[low])
-            xupp = 0.5*(xdata[upp]+xdata[min(num_data-1, upp+1)])
+        for low, upp in current_include:
+            xlow = 0.5 * (xdata[max(0, low-1)]+xdata[low])
+            xupp = 0.5 * (xdata[upp]+xdata[min(num_data-1, 1+upp)])
             ax.axvspan(xlow, xupp, facecolor='green', alpha=0.5)
-        for (low, upp) in current_exclude:
-            xlow = 0.5*(xdata[max(0, low-1)]+xdata[low])
-            xupp = 0.5*(xdata[upp]+xdata[min(num_data-1, upp+1)])
+        for low, upp in current_exclude:
+            xlow = 0.5 * (xdata[max(0, low-1)]+xdata[low])
+            xupp = 0.5 * (xdata[upp]+xdata[min(num_data-1, 1+upp)])
             ax.axvspan(xlow, xupp, facecolor='red', alpha=0.5)
-        for (low, upp) in selected_index_ranges:
-            xlow = 0.5*(xdata[max(0, low-1)]+xdata[low])
-            xupp = 0.5*(xdata[upp]+xdata[min(num_data-1, upp+1)])
+        for low, upp in selected_index_ranges:
+            xlow = 0.5 * (xdata[max(0, low-1)]+xdata[low])
+            xupp = 0.5 * (xdata[upp]+xdata[min(num_data-1, 1+upp)])
             ax.axvspan(xlow, xupp, facecolor=selection_color, alpha=0.5)
         ax.get_figure().canvas.draw()
 
     def onclick(event):
+        """Action taken on clicking the mouse button."""
         if event.inaxes in [fig.axes[0]]:
             selected_index_ranges.append(index_nearest_upp(xdata, event.xdata))
 
     def onrelease(event):
-        if len(selected_index_ranges) > 0:
+        """Action taken on releasing the mouse button."""
+        if selected_index_ranges:
             if isinstance(selected_index_ranges[-1], int):
                 if event.inaxes in [fig.axes[0]]:
                     event.xdata = index_nearest_low(xdata, event.xdata)
                     if selected_index_ranges[-1] <= event.xdata:
-                        selected_index_ranges[-1] = (selected_index_ranges[-1], event.xdata)
+                        selected_index_ranges[-1] = \
+                            (selected_index_ranges[-1], event.xdata)
                     else:
-                        selected_index_ranges[-1] = (event.xdata, selected_index_ranges[-1])
-                    draw_selections(event.inaxes, current_include, current_exclude, selected_index_ranges)
+                        selected_index_ranges[-1] = \
+                            (event.xdata, selected_index_ranges[-1])
+                    draw_selections(
+                        event.inaxes, current_include, current_exclude,
+                        selected_index_ranges)
                 else:
                     selected_index_ranges.pop(-1)
 
     def confirm_selection(event):
+        """Action taken on hitting the confirm button."""
         plt.close()
 
     def clear_last_selection(event):
-        if len(selected_index_ranges):
+        """Action taken on hitting the clear button."""
+        if selected_index_ranges:
             selected_index_ranges.pop(-1)
         else:
-            while len(current_include):
+            while current_include:
                 current_include.pop()
-            while len(current_exclude):
+            while current_exclude:
                 current_exclude.pop()
             selected_mask.fill(False)
-        draw_selections(ax, current_include, current_exclude, selected_index_ranges)
+        draw_selections(
+            ax, current_include, current_exclude, selected_index_ranges)
 
     def update_mask(mask, selected_index_ranges, unselected_index_ranges):
-        for (low, upp) in selected_index_ranges:
-            selected_mask = np.logical_and(xdata >= xdata[low], xdata <= xdata[upp])
+        """Update the plot with the selected mask."""
+        for low, upp in selected_index_ranges:
+            selected_mask = np.logical_and(
+                xdata >= xdata[low], xdata <= xdata[upp])
             mask = np.logical_or(mask, selected_mask)
-        for (low, upp) in unselected_index_ranges:
-            unselected_mask = np.logical_and(xdata >= xdata[low], xdata <= xdata[upp])
+        for low, upp in unselected_index_ranges:
+            unselected_mask = np.logical_and(
+                xdata >= xdata[low], xdata <= xdata[upp])
             mask[unselected_mask] = False
         return mask
 
     def update_index_ranges(mask):
-        # Update the currently included index ranges (where mask is True)
+        """
+        Update the currently included index ranges (where mask = True).
+        """
         current_include = []
         for i, m in enumerate(mask):
-            if m == True:
-                if len(current_include) == 0 or type(current_include[-1]) == tuple:
+            if m:
+                if (not current_include
+                        or isinstance(current_include[-1], tuple)):
                     current_include.append(i)
             else:
-                if len(current_include) > 0 and isinstance(current_include[-1], int):
+                if current_include and isinstance(current_include[-1], int):
                     current_include[-1] = (current_include[-1], i-1)
-        if len(current_include) > 0 and isinstance(current_include[-1], int):
+        if current_include and isinstance(current_include[-1], int):
             current_include[-1] = (current_include[-1], num_data-1)
         return current_include
 
     # Check inputs
     ydata = np.asarray(ydata)
     if ydata.ndim > 1:
         logger.warning(f'Invalid ydata dimension ({ydata.ndim})')
@@ -790,89 +989,95 @@
             logger.warning(f'Invalid xdata shape ({xdata.shape})')
             return None, None
         if not np.all(xdata[:-1] < xdata[1:]):
             logger.warning('Invalid xdata: must be monotonically increasing')
             return None, None
     if current_index_ranges is not None:
         if not isinstance(current_index_ranges, (tuple, list)):
-            logger.warning('Invalid current_index_ranges parameter ({current_index_ranges}, '+
-                    f'{type(current_index_ranges)})')
+            logger.warning(
+                'Invalid current_index_ranges parameter '
+                f'({current_index_ranges}, {type(current_index_ranges)})')
             return None, None
     if not isinstance(select_mask, bool):
-        logger.warning('Invalid select_mask parameter ({select_mask}, {type(select_mask)})')
+        logger.warning(
+            f'Invalid select_mask parameter ({select_mask}, '
+            f'{type(select_mask)})')
         return None, None
     if num_index_ranges_max is not None:
-        logger.warning('num_index_ranges_max input not yet implemented in draw_mask_1d')
+        logger.warning(
+            'num_index_ranges_max input not yet implemented in draw_mask_1d')
     if title is None:
         title = 'select ranges of data'
     elif not isinstance(title, str):
-        illegal(title, 'title')
+        illegal_value(title, 'title')
         title = ''
     if legend is None and not isinstance(title, str):
-        illegal(legend, 'legend')
+        illegal_value(legend, 'legend')
         legend = None
 
     if select_mask:
         title = f'Click and drag to {title} you wish to include'
         selection_color = 'green'
     else:
         title = f'Click and drag to {title} you wish to exclude'
         selection_color = 'red'
 
-    # Set initial selected mask and the selected/unselected index ranges as needed
+    # Set initial selected mask and the selected/unselected index
+    #     ranges as needed
     selected_index_ranges = []
     unselected_index_ranges = []
     selected_mask = np.full(xdata.shape, False, dtype=bool)
     if current_index_ranges is None:
         if current_mask is None:
             if not select_mask:
                 selected_index_ranges = [(0, num_data-1)]
                 selected_mask = np.full(xdata.shape, True, dtype=bool)
         else:
             selected_mask = np.copy(np.asarray(current_mask, dtype=bool))
-    if current_index_ranges is not None and len(current_index_ranges):
-        current_index_ranges = sorted([(low, upp) for (low, upp) in current_index_ranges])
-        for (low, upp) in current_index_ranges:
+    if current_index_ranges is not None and current_index_ranges:
+        current_index_ranges = sorted(list(current_index_ranges))
+        for low, upp in current_index_ranges:
             if low > upp or low >= num_data or upp < 0:
                 continue
-            if low < 0:
-                low = 0
-            if upp >= num_data:
-                upp = num_data-1
+            low = max(low, 0)
+            upp = min(upp, num_data-1)
             selected_index_ranges.append((low, upp))
-        selected_mask = update_mask(selected_mask, selected_index_ranges, unselected_index_ranges)
+        selected_mask = update_mask(
+            selected_mask, selected_index_ranges, unselected_index_ranges)
     if current_index_ranges is not None and current_mask is not None:
         selected_mask = np.logical_and(current_mask, selected_mask)
     if current_mask is not None:
         selected_index_ranges = update_index_ranges(selected_mask)
 
     # Set up range selections for display
     current_include = selected_index_ranges
     current_exclude = []
     selected_index_ranges = []
-    if not len(current_include):
+    if not current_include:
         if select_mask:
             current_exclude = [(0, num_data-1)]
         else:
             current_include = [(0, num_data-1)]
     else:
         if current_include[0][0] > 0:
             current_exclude.append((0, current_include[0][0]-1))
         for i in range(1, len(current_include)):
-            current_exclude.append((current_include[i-1][1]+1, current_include[i][0]-1))
+            current_exclude.append(
+                (1+current_include[i-1][1], current_include[i][0]-1))
         if current_include[-1][1] < num_data-1:
-            current_exclude.append((current_include[-1][1]+1, num_data-1))
+            current_exclude.append((1+current_include[-1][1], num_data-1))
 
     if not test_mode:
 
         # Set up matplotlib figure
         plt.close('all')
         fig, ax = plt.subplots()
         plt.subplots_adjust(bottom=0.2)
-        draw_selections(ax, current_include, current_exclude, selected_index_ranges)
+        draw_selections(
+            ax, current_include, current_exclude, selected_index_ranges)
 
         # Set up event handling for click-and-drag range selection
         cid_click = fig.canvas.mpl_connect('button_press_event', onclick)
         cid_release = fig.canvas.mpl_connect('button_release_event', onrelease)
 
         # Set up confirm / clear range selection buttons
         confirm_b = Button(plt.axes([0.75, 0.05, 0.15, 0.075]), 'Confirm')
@@ -887,208 +1092,255 @@
         fig.canvas.mpl_disconnect(cid_click)
         fig.canvas.mpl_disconnect(cid_release)
         confirm_b.disconnect(cid_confirm)
         clear_b.disconnect(cid_clear)
 
     # Swap selection depending on select_mask
     if not select_mask:
-        selected_index_ranges, unselected_index_ranges = unselected_index_ranges, \
-                selected_index_ranges
+        selected_index_ranges, unselected_index_ranges = \
+            unselected_index_ranges, selected_index_ranges
 
     # Update the mask with the currently selected/unselected x-ranges
-    selected_mask = update_mask(selected_mask, selected_index_ranges, unselected_index_ranges)
+    selected_mask = update_mask(
+        selected_mask, selected_index_ranges, unselected_index_ranges)
 
     # Update the currently included index ranges (where mask is True)
     current_include = update_index_ranges(selected_mask)
 
-def select_image_bounds(a, axis, low=None, upp=None, num_min=None, title='select array bounds',
+    return selected_mask, current_include
+
+
+def select_image_bounds(
+        a, axis, low=None, upp=None, num_min=None, title='select array bounds',
         raise_error=False):
-    """Interactively select the lower and upper data bounds for a 2D numpy array.
+    """
+    Interactively select the lower and upper data bounds for a 2D
+    numpy array.
     """
     a = np.asarray(a)
     if a.ndim != 2:
-        illegal_value(a.ndim, 'array dimension', location='select_image_bounds',
-                raise_error=raise_error)
+        illegal_value(
+            a.ndim, 'array dimension', location='select_image_bounds',
+            raise_error=raise_error)
         return None
     if axis < 0 or axis >= a.ndim:
-        illegal_value(axis, 'axis', location='select_image_bounds', raise_error=raise_error)
+        illegal_value(
+            axis, 'axis', location='select_image_bounds',
+            raise_error=raise_error)
         return None
     low_save = low
     upp_save = upp
     num_min_save = num_min
     if num_min is None:
         num_min = 1
     else:
         if num_min < 2 or num_min > a.shape[axis]:
-            logger.warning('Invalid input for num_min in select_image_bounds, input ignored')
+            logger.warning(
+                'Invalid input for num_min in select_image_bounds, '
+                'input ignored')
             num_min = 1
     if low is None:
         min_ = 0
         max_ = a.shape[axis]
         low_max = a.shape[axis]-num_min
         while True:
             if axis:
-                quick_imshow(a[:,min_:max_], title=title, aspect='auto',
-                        extent=[min_,max_,a.shape[0],0])
+                quick_imshow(
+                    a[:,min_:max_], title=title, aspect='auto',
+                    extent=[min_,max_,a.shape[0],0])
             else:
-                quick_imshow(a[min_:max_,:], title=title, aspect='auto',
-                        extent=[0,a.shape[1], max_,min_])
-            zoom_flag = input_yesno('Set lower data bound (y) or zoom in (n)?', 'y')
+                quick_imshow(
+                    a[min_:max_,:], title=title, aspect='auto',
+                    extent=[0,a.shape[1], max_,min_])
+            zoom_flag = input_yesno(
+                'Set lower data bound (y) or zoom in (n)?', 'y')
             if zoom_flag:
                 low = input_int('    Set lower data bound', ge=0, le=low_max)
                 break
-            else:
-                min_ = input_int('    Set lower zoom index', ge=0, le=low_max)
-                max_ = input_int('    Set upper zoom index', ge=min_+1, le=low_max+1)
+            min_ = input_int('    Set lower zoom index', ge=0, le=low_max)
+            max_ = input_int(
+                '    Set upper zoom index', ge=min_+1, le=low_max+1)
     else:
         if not is_int(low, ge=0, le=a.shape[axis]-num_min):
-            illegal_value(low, 'low', location='select_image_bounds', raise_error=raise_error)
+            illegal_value(
+                low, 'low', location='select_image_bounds',
+                raise_error=raise_error)
             return None
     if upp is None:
         min_ = low+num_min
         max_ = a.shape[axis]
         upp_min = min_
         while True:
             if axis:
-                quick_imshow(a[:,min_:max_], title=title, aspect='auto',
-                        extent=[min_,max_,a.shape[0],0])
+                quick_imshow(
+                    a[:,min_:max_], title=title, aspect='auto',
+                    extent=[min_,max_,a.shape[0],0])
             else:
-                quick_imshow(a[min_:max_,:], title=title, aspect='auto',
-                        extent=[0,a.shape[1], max_,min_])
-            zoom_flag = input_yesno('Set upper data bound (y) or zoom in (n)?', 'y')
+                quick_imshow(
+                    a[min_:max_,:], title=title, aspect='auto',
+                    extent=[0,a.shape[1], max_,min_])
+            zoom_flag = input_yesno(
+                'Set upper data bound (y) or zoom in (n)?', 'y')
             if zoom_flag:
-                upp = input_int('    Set upper data bound', ge=upp_min, le=a.shape[axis])
+                upp = input_int(
+                    '    Set upper data bound', ge=upp_min, le=a.shape[axis])
                 break
-            else:
-                min_ = input_int('    Set upper zoom index', ge=upp_min, le=a.shape[axis]-1)
-                max_ = input_int('    Set upper zoom index', ge=min_+1, le=a.shape[axis])
+            min_ = input_int(
+                '    Set upper zoom index', ge=upp_min, le=a.shape[axis]-1)
+            max_ = input_int(
+                '    Set upper zoom index', ge=min_+1, le=a.shape[axis])
     else:
         if not is_int(upp, ge=low+num_min, le=a.shape[axis]):
-            illegal_value(upp, 'upp', location='select_image_bounds', raise_error=raise_error)
+            illegal_value(
+                upp, 'upp', location='select_image_bounds',
+                raise_error=raise_error)
             return None
     bounds = (low, upp)
     a_tmp = np.copy(a)
     a_tmp_max = a.max()
     if axis:
         a_tmp[:,bounds[0]] = a_tmp_max
         a_tmp[:,bounds[1]-1] = a_tmp_max
     else:
         a_tmp[bounds[0],:] = a_tmp_max
         a_tmp[bounds[1]-1,:] = a_tmp_max
     print(f'lower bound = {low} (inclusive)\nupper bound = {upp} (exclusive)')
     quick_imshow(a_tmp, title=title, aspect='auto')
     del a_tmp
     if not input_yesno('Accept these bounds (y/n)?', 'y'):
-        bounds = select_image_bounds(a, axis, low=low_save, upp=upp_save, num_min=num_min_save,
+        bounds = select_image_bounds(
+            a, axis, low=low_save, upp=upp_save, num_min=num_min_save,
             title=title)
     clear_imshow(title)
     return bounds
 
-def select_one_image_bound(a, axis, bound=None, bound_name=None, title='select array bounds',
+
+def select_one_image_bound(
+        a, axis, bound=None, bound_name=None, title='select array bounds',
         default='y', raise_error=False):
-    """Interactively select a data boundary for a 2D numpy array.
+    """
+    Interactively select a data boundary for a 2D numpy array.
     """
     a = np.asarray(a)
     if a.ndim != 2:
-        illegal_value(a.ndim, 'array dimension', location='select_one_image_bound',
-                raise_error=raise_error)
+        illegal_value(
+            a.ndim, 'array dimension', location='select_one_image_bound',
+            raise_error=raise_error)
         return None
     if axis < 0 or axis >= a.ndim:
-        illegal_value(axis, 'axis', location='select_one_image_bound', raise_error=raise_error)
+        illegal_value(
+            axis, 'axis', location='select_one_image_bound',
+            raise_error=raise_error)
         return None
     if bound_name is None:
         bound_name = 'data bound'
     if bound is None:
         min_ = 0
         max_ = a.shape[axis]
         bound_max = a.shape[axis]-1
         while True:
             if axis:
-                quick_imshow(a[:,min_:max_], title=title, aspect='auto',
-                        extent=[min_,max_,a.shape[0],0])
+                quick_imshow(
+                    a[:,min_:max_], title=title, aspect='auto',
+                    extent=[min_,max_,a.shape[0],0])
             else:
-                quick_imshow(a[min_:max_,:], title=title, aspect='auto',
-                        extent=[0,a.shape[1], max_,min_])
-            zoom_flag = input_yesno(f'Set {bound_name} (y) or zoom in (n)?', 'y')
+                quick_imshow(
+                    a[min_:max_,:], title=title, aspect='auto',
+                    extent=[0,a.shape[1], max_,min_])
+            zoom_flag = input_yesno(
+                f'Set {bound_name} (y) or zoom in (n)?', 'y')
             if zoom_flag:
                 bound = input_int(f'    Set {bound_name}', ge=0, le=bound_max)
                 clear_imshow(title)
                 break
-            else:
-                min_ = input_int('    Set lower zoom index', ge=0, le=bound_max)
-                max_ = input_int('    Set upper zoom index', ge=min_+1, le=bound_max+1)
+            min_ = input_int('    Set lower zoom index', ge=0, le=bound_max)
+            max_ = input_int(
+                '    Set upper zoom index', ge=min_+1, le=bound_max+1)
 
     elif not is_int(bound, ge=0, le=a.shape[axis]-1):
-        illegal_value(bound, 'bound', location='select_one_image_bound', raise_error=raise_error)
+        illegal_value(
+            bound, 'bound', location='select_one_image_bound',
+            raise_error=raise_error)
         return None
     else:
         print(f'Current {bound_name} = {bound}')
     a_tmp = np.copy(a)
     a_tmp_max = a.max()
     if axis:
         a_tmp[:,bound] = a_tmp_max
     else:
         a_tmp[bound,:] = a_tmp_max
     quick_imshow(a_tmp, title=title, aspect='auto')
     del a_tmp
     if not input_yesno(f'Accept this {bound_name} (y/n)?', default):
-        bound = select_one_image_bound(a, axis, bound_name=bound_name, title=title)
+        bound = select_one_image_bound(
+            a, axis, bound_name=bound_name, title=title)
     clear_imshow(title)
     return bound
 
+
 def clear_imshow(title=None):
+    """Clear an image opened by quick_imshow()."""
     plt.ioff()
     if title is None:
         title = 'quick imshow'
     elif not isinstance(title, str):
         raise ValueError(f'Invalid parameter title ({title})')
     plt.close(fig=title)
 
+
 def clear_plot(title=None):
+    """Clear an image opened by quick_plot()."""
     plt.ioff()
     if title is None:
         title = 'quick plot'
     elif not isinstance(title, str):
         raise ValueError(f'Invalid parameter title ({title})')
     plt.close(fig=title)
 
-def quick_imshow(a, title=None, path=None, name=None, save_fig=False, save_only=False,
-            clear=True, extent=None, show_grid=False, grid_color='w', grid_linewidth=1,
-            block=False, **kwargs):
+
+def quick_imshow(
+        a, title=None, path=None, name=None, save_fig=False, save_only=False,
+        clear=True, extent=None, show_grid=False, grid_color='w',
+        grid_linewidth=1, block=False, **kwargs):
+    """Display a 2D image."""
     if title is not None and not isinstance(title, str):
         raise ValueError(f'Invalid parameter title ({title})')
     if path is not None and not isinstance(path, str):
         raise ValueError(f'Invalid parameter path ({path})')
     if not isinstance(save_fig, bool):
         raise ValueError(f'Invalid parameter save_fig ({save_fig})')
     if not isinstance(save_only, bool):
         raise ValueError(f'Invalid parameter save_only ({save_only})')
     if not isinstance(clear, bool):
         raise ValueError(f'Invalid parameter clear ({clear})')
     if not isinstance(block, bool):
         raise ValueError(f'Invalid parameter block ({block})')
     if not title:
-        title='quick imshow'
+        title = 'quick imshow'
     if name is None:
-        ttitle = re_sub(r"\s+", '_', title)
+        ttitle = re_sub(r'\s+', '_', title)
         if path is None:
             path = f'{ttitle}.png'
         else:
             path = f'{path}/{ttitle}.png'
     else:
         if path is None:
             path = name
         else:
             path = f'{path}/{name}'
-    if 'cmap' in kwargs and a.ndim == 3 and (a.shape[2] == 3 or a.shape[2] == 4):
+    if ('cmap' in kwargs and a.ndim == 3
+            and (a.shape[2] == 3 or a.shape[2] == 4)):
         use_cmap = True
         if a.shape[2] == 4 and a[:,:,-1].min() != a[:,:,-1].max():
             use_cmap = False
-        if any(True if a[i,j,0] != a[i,j,1] and a[i,j,0] != a[i,j,2] else False
-                for i in range(a.shape[0]) for j in range(a.shape[1])):
+        if any(
+                a[i,j,0] != a[i,j,1] and a[i,j,0] != a[i,j,2]
+                for i in range(a.shape[0])
+                for j in range(a.shape[1])):
             use_cmap = False
         if use_cmap:
             a = a[:,:,0]
         else:
             logger.warning('Image incompatible with cmap option, ignore cmap')
             kwargs.pop('cmap')
     if extent is None:
@@ -1115,24 +1367,30 @@
         plt.close(fig=title)
     else:
         if save_fig:
             plt.savefig(path)
         if block:
             plt.show(block=block)
 
-def quick_plot(*args, xerr=None, yerr=None, vlines=None, title=None, xlim=None, ylim=None,
-        xlabel=None, ylabel=None, legend=None, path=None, name=None, show_grid=False,
-        save_fig=False, save_only=False, clear=True, block=False, **kwargs):
+
+def quick_plot(
+        *args, xerr=None, yerr=None, vlines=None, title=None, xlim=None,
+        ylim=None, xlabel=None, ylabel=None, legend=None, path=None, name=None,
+        show_grid=False, save_fig=False, save_only=False, clear=True,
+        block=False, **kwargs):
+    """Display a 2D line plot."""
     if title is not None and not isinstance(title, str):
         illegal_value(title, 'title', 'quick_plot')
         title = None
-    if xlim is not None and not isinstance(xlim, (tuple, list)) and len(xlim) != 2:
+    if (xlim is not None and not isinstance(xlim, (tuple, list))
+            and len(xlim) != 2):
         illegal_value(xlim, 'xlim', 'quick_plot')
         xlim = None
-    if ylim is not None and not isinstance(ylim, (tuple, list)) and len(ylim) != 2:
+    if (ylim is not None and not isinstance(ylim, (tuple, list))
+            and len(ylim) != 2):
         illegal_value(ylim, 'ylim', 'quick_plot')
         ylim = None
     if xlabel is not None and not isinstance(xlabel, str):
         illegal_value(xlabel, 'xlabel', 'quick_plot')
         xlabel = None
     if ylabel is not None and not isinstance(ylabel, str):
         illegal_value(ylabel, 'ylabel', 'quick_plot')
@@ -1157,15 +1415,15 @@
         return
     if not isinstance(block, bool):
         illegal_value(block, 'block', 'quick_plot')
         return
     if title is None:
         title = 'quick plot'
     if name is None:
-        ttitle = re_sub(r"\s+", '_', title)
+        ttitle = re_sub(r'\s+', '_', title)
         if path is None:
             path = f'{ttitle}.png'
         else:
             path = f'{path}/{ttitle}.png'
     else:
         if path is None:
             path = name
@@ -1182,44 +1440,43 @@
     if not save_only:
         if block:
             plt.ioff()
         else:
             plt.ion()
     plt.figure(title)
     if depth_tuple(args) > 1:
-       for y in args:
-           plt.plot(*y, **kwargs)
+        for y in args:
+            plt.plot(*y, **kwargs)
     else:
         if xerr is None and yerr is None:
             plt.plot(*args, **kwargs)
         else:
             plt.errorbar(*args, xerr=xerr, yerr=yerr, **kwargs)
     if vlines is not None:
         if isinstance(vlines, (int, float)):
             vlines = [vlines]
         for v in vlines:
             plt.axvline(v, color='r', linestyle='--', **kwargs)
 #    if vlines is not None:
-#        for s in tuple(([x, x], list(plt.gca().get_ylim())) for x in vlines):
+#        for s in tuple(
+#                ([x, x], list(plt.gca().get_ylim())) for x in vlines):
 #            plt.plot(*s, color='red', **kwargs)
     if xlim is not None:
         plt.xlim(xlim)
     if ylim is not None:
         plt.ylim(ylim)
     if xlabel is not None:
         plt.xlabel(xlabel)
     if ylabel is not None:
         plt.ylabel(ylabel)
     if show_grid:
         ax = plt.gca()
-        ax.grid(color='k')#, linewidth=1)
+        ax.grid(color='k')  # , linewidth=1)
     if legend is not None:
         plt.legend(legend)
     if save_only:
         plt.savefig(path)
         plt.close(fig=title)
     else:
         if save_fig:
             plt.savefig(path)
-        if block:
-            plt.show(block=block)
-
+        plt.show(block=block)
```

### Comparing `ChessAnalysisPipeline-0.0.5/CHAP/common/utils/material.py` & `ChessAnalysisPipeline-0.0.6/CHAP/common/utils/material.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,231 +1,268 @@
 #!/usr/bin/env python3
-
 # -*- coding: utf-8 -*-
+#pylint: disable=
 """
-Created on Fri May 27 12:21:25 2022
-
-@author: rv43
+File       : general.py
+Author     : Rolf Verberg <rolfverberg AT gmail dot com>
+Description: Module defining the Material class
 """
 
-import logging
+# System modules
+from logging import getLogger
+from os import path
 
-import os
+# Third party modules
 import numpy as np
 try:
-    import xrayutilities as xu
-    have_xu = True
-except:
-    have_xu = False
-    pass
+    from xrayutilities import materials
+    from xrayutilities import simpack
+    HAVE_XU = True
+except ImportError:
+    HAVE_XU = False
 try:
     from hexrd import material
-    have_hexrd = True
-except:
-    have_hexrd = False
-    pass
-if have_hexrd:
+    HAVE_HEXRD = True
+except ImportError:
+    HAVE_HEXRD = False
+if HAVE_HEXRD:
     try:
         from hexrd.valunits import valWUnit
-    except:
-        have_hexrd = False
-        pass
+    except ImportError:
+        HAVE_HEXRD = False
+
+POEDER_INTENSITY_CUTOFF = 1.e-8
+
+logger = getLogger(__name__)
 
-powder_intensity_cutoff = 1.e-8
 
 class Material:
-    """Base class for materials in an sin2psi or EDD analysis.
-       Right now it assumes a single material
-           extend its ability to do differently when test data is available
     """
-
-    def __init__(self, material_name=None, material_file=None, sgnum=None,
-            lattice_parameters_angstroms=None, atoms=None, pos=None, enrgy=None):
+    Base class for materials in an sin2psi or EDD analysis. Right now
+    it assumes a single material, extend its ability to do differently
+    when test data is available
+    """
+    def __init__(
+            self, material_name=None, material_file=None, sgnum=None,
+            lattice_parameters_angstroms=None, atoms=None, pos=None,
+            enrgy=None):
+        """Initialize Material."""
         self._enrgy = enrgy
         self._materials = []
         self._ds_min = []
         self._ds_unique = None
         self._hkls_unique = None
         if material_name is not None:
-            self.add_material(material_name, material_file, sgnum, lattice_parameters_angstroms,
-                    atoms, pos)
+            self.add_material(
+                material_name, material_file, sgnum,
+                lattice_parameters_angstroms, atoms, pos)
 
-    @property
-    #FIX passing arguments to a property isn't correct?
     def lattice_parameters(self, index=0):
-        """Convert from internal nm units to angstrom
-        """
+        """Convert from internal nm units to angstrom."""
         matl = self._materials[index]
-        if isinstance(matl, xu.materials.material.Crystal):
+        if isinstance(matl, materials.material.Crystal):
             return [matl.a, matl.b, matl.c]
-        elif isinstance(matl, material.Material):
-            return [l.getVal("angstrom") for l in self._materials[index].latticeParameters[0:3]]
-        else:
-            raise ValueError('Illegal material class type')
-            return None
+        if isinstance(matl, material.Material):
+            return [
+                lpars.getVal('angstrom')
+                for lpars in self._materials[index].latticeParameters[0:3]]
+        raise ValueError('Illegal material class type')
 
-    @property
     def ds_unique(self, tth_tol=None, tth_max=None, round_sig=8):
+        """Return the unique lattice spacings."""
         if self._ds_unique is None:
-            self.get_unique_ds(tth_tol, tth_max, round_sig)
+            self.get_ds_unique(tth_tol, tth_max, round_sig)
         return self._ds_unique
 
-    @property
     def hkls_unique(self, tth_tol=None, tth_max=None, round_sig=8):
+        """Return the unique HKLs."""
         if self._hkls_unique is None:
-            self.get_unique_ds(tth_tol, tth_max, round_sig)
+            self.get_ds_unique(tth_tol, tth_max, round_sig)
         return self._hkls_unique
 
-    def add_material(self, material_name, material_file=None, sgnum=None,
-            lattice_parameters_angstroms=None, atoms=None, pos=None, dmin_angstroms=0.6):
+    def add_material(
+            self, material_name, material_file=None, sgnum=None,
+            lattice_parameters_angstroms=None, atoms=None, pos=None,
+            dmin_angstroms=0.6):
+        """Add a material."""
         # At this point only for a single material
-        # Unique energies works for more, but fitting with different materials is not implemented
+        # Unique energies works for more, but fitting with different
+        #     materials is not implemented
         if len(self._materials) == 1:
-            exit('Multiple materials not implemented yet')
+            raise ValueError('Multiple materials not implemented yet')
         self._ds_min.append(dmin_angstroms)
-        self._materials.append(Material.make_material(material_name, material_file, sgnum,
+        self._materials.append(
+            Material.make_material(
+                material_name, material_file, sgnum,
                 lattice_parameters_angstroms, atoms, pos, dmin_angstroms))
 
-    def get_unique_ds(self, tth_tol=None, tth_max=None, round_sig=8):
-        """Get the list of unique lattice spacings from material HKLs
+    def get_ds_unique(self, tth_tol=None, tth_max=None, round_sig=8):
+        """
+        Get the list of unique lattice spacings from material HKLs.
 
         Parameters
         ----------
         tth_tol     : two theta tolerance (in degrees)
         tth_max     : maximum two theta value (in degrees)
         round_sig   : significant digits, passed to round() function
 
         Returns
         -------
-        hkls     : list of hkl's corresponding to the unique lattice spacings
-        ds       : list of the unique lattice spacings
+        hkls: list of hkl's corresponding to the unique lattice spacings
+        ds: list of the unique lattice spacings
         """
         hkls = np.empty((0,3))
         ds = np.empty((0))
-        ids = np.empty((0))
-        for i,m in enumerate(self._materials):
+        ds_index = np.empty((0))
+        for i, m in enumerate(self._materials):
             material_class_valid = False
-            if have_xu:
-                if isinstance(m, xu.materials.material.Crystal):
-                    powder = xu.simpack.PowderDiffraction(m, en=self._enrgy)
-                    hklsi = [hkl for hkl in powder.data if powder.data[hkl]['active']]
-                    dsi = [m.planeDistance(hkl) for hkl in powder.data if powder.data[hkl]['active']]
-                    mask = [True if d > self._ds_min[i] else False for d in dsi]
+            if HAVE_XU:
+                if isinstance(m, materials.material.Crystal):
+                    powder = simpack.PowderDiffraction(m, en=self._enrgy)
+                    hklsi = [hkl for hkl in powder.data
+                             if powder.data[hkl]['active']]
+                    ds_i = [m.planeDistance(hkl) for hkl in powder.data
+                            if powder.data[hkl]['active']]
+                    mask = [d > self._ds_min[i] for d in ds_i]
                     hkls = np.vstack((hkls, np.array(hklsi)[mask,:]))
-                    dsi = np.array(dsi)[mask]
+                    ds_i = np.array(ds_i)[mask]
                     material_class_valid = True
-            if have_hexrd:
+            if HAVE_HEXRD:
                 if isinstance(m, material.Material):
-                    pd = m.planeData
+                    plane_data = m.planeData
                     if tth_tol is not None:
-                        pd.tThWidth = np.radians(tth_tol)
+                        plane_data.tThWidth = np.radians(tth_tol)
                     if tth_max is not None:
-                        pd.exclusions = None
-                        pd.tThMax = np.radians(tth_max)
-                    hkls = np.vstack((hkls, pd.hkls.T))
-                    dsi = pd.getPlaneSpacings()
+                        plane_data.exclusions = None
+                        plane_data.tThMax = np.radians(tth_max)
+                    hkls = np.vstack((hkls, plane_data.hkls.T))
+                    ds_i = plane_data.getPlaneSpacings()
                     material_class_valid = True
             if not material_class_valid:
                 raise ValueError('Illegal material class type')
-            ds = np.hstack((ds, dsi))
-            ids = np.hstack((ids, i*np.ones(len(dsi))))
+            ds = np.hstack((ds, ds_i))
+            ds_index = np.hstack((ds_index, i*np.ones(len(ds_i))))
 
         # Sort lattice spacings in reverse order (use -)
-        ds_unique, ids_unique, _ = np.unique(-ds.round(round_sig), return_index=True,
-                return_counts=True)
+        ds_unique, ds_index_unique, _ = np.unique(
+            -ds.round(round_sig), return_index=True, return_counts=True)
         ds_unique = np.abs(ds_unique)
 
         # Limit the list to unique lattice spacings
-        self._hkls_unique = hkls[ids_unique,:].astype(int)
-        self._ds_unique = ds[ids_unique]
-        hkl_list = np.vstack((np.arange(self._ds_unique.shape[0]), ids[ids_unique],
-                self._hkls_unique.T, self._ds_unique)).T
-        logging.info("Unique d's:")
+        self._hkls_unique = hkls[ds_index_unique,:].astype(int)
+        self._ds_unique = ds[ds_index_unique]
+        hkl_list = np.vstack(
+            (np.arange(self._ds_unique.shape[0]), ds_index[ds_index_unique],
+             self._hkls_unique.T, self._ds_unique)).T
+        logger.info("Unique d's:")
         for hkl in hkl_list:
-            logging.info(f'{hkl[0]:4.0f} {hkl[1]:.0f} {hkl[2]:.0f} {hkl[3]:.0f} {hkl[4]:.0f} '+
-                    f'{hkl[5]:.6f}')
+            logger.info(
+                f'{hkl[0]:4.0f} {hkl[1]:.0f} {hkl[2]:.0f} {hkl[3]:.0f} '
+                f'{hkl[4]:.0f} {hkl[5]:.6f}')
 
         return self._hkls_unique, self._ds_unique
 
     @staticmethod
-    def make_material(material_name, material_file=None, sgnum=None,
-            lattice_parameters_angstroms=None, atoms=None, pos=None, dmin_angstroms=0.6):
-        """ Use HeXRD to get material properties when a materials file is provided
-            Use xrayutilities otherwise
+    def make_material(
+            material_name, material_file=None, sgnum=None,
+            lattice_parameters_angstroms=None, atoms=None, pos=None,
+            dmin_angstroms=0.6):
+        """
+        Use HeXRD to get material properties when a materials file is
+        provided. Use xrayutilities otherwise.
         """
         if not isinstance(material_name, str):
-            raise ValueError(f'Illegal material_name: {material_name} {type(material_name)}')
+            raise ValueError(
+                f'Illegal material_name: {material_name} '
+                f'{type(material_name)}')
         if lattice_parameters_angstroms is not None:
             if material_file is not None:
-                logging.warning('Overwrite lattice_parameters of material_file with input values '+
-                        f'({lattice_parameters_angstroms})')
+                logger.warning(
+                    'Overwrite lattice_parameters of material_file with input '
+                    f'values ({lattice_parameters_angstroms})')
             if isinstance(lattice_parameters_angstroms, (int, float)):
                 lattice_parameters = [lattice_parameters_angstroms]
-            elif isinstance(lattice_parameters_angstroms, (tuple, list, np.ndarray)):
+            elif isinstance(
+                    lattice_parameters_angstroms, (tuple, list, np.ndarray)):
                 lattice_parameters = list(lattice_parameters_angstroms)
             else:
-                raise ValueError(f'Illegal lattice_parameters_angstroms: '+
-                        f'{lattice_parameters_angstroms} {type(lattice_parameters_angstroms)}')
+                raise ValueError(
+                    'Illegal lattice_parameters_angstroms: '
+                    f'{lattice_parameters_angstroms} '
+                    f'{type(lattice_parameters_angstroms)}')
         if material_file is None:
             if not isinstance(sgnum, int):
                 raise ValueError(f'Illegal sgnum: {sgnum} {type(sgnum)}')
-            if sgnum is None or lattice_parameters_angstroms is None or pos is None:
-                raise ValueError('Valid inputs for sgnum and lattice_parameters_angstroms and '+
-                        'pos are required if materials file is not specified')
+            if (sgnum is None or lattice_parameters_angstroms is None
+                    or pos is None):
+                raise ValueError(
+                    'Valid inputs for sgnum, lattice_parameters_angstroms and '
+                    'pos are required if materials file is not specified')
             if isinstance(pos, str):
                 pos = [pos]
             use_xu = True
-            if (np.array(pos).ndim == 1 and isinstance(pos[0], (int, float)) and
-                    np.array(pos).size == 3):
-                if have_hexrd:
+            if (np.array(pos).ndim == 1 and isinstance(pos[0], (int, float))
+                    and np.array(pos).size == 3):
+                if HAVE_HEXRD:
                     pos = np.array([pos])
                     use_xu = False
-            elif (np.array(pos).ndim == 2 and np.array(pos).shape[0] > 0 and
-                    np.array(pos).shape[1] == 3):
-                if have_hexrd:
+            elif (np.array(pos).ndim == 2 and np.array(pos).shape[0] > 0
+                    and np.array(pos).shape[1] == 3):
+                if HAVE_HEXRD:
                     pos = np.array(pos)
                     use_xu = False
-            elif not (np.array(pos).ndim == 1 and isinstance(pos[0], str) and
-                    np.array(pos).size > 0 and have_xu):
-                raise ValueError(f'Illegal pos (have_xu = {have_xu}): {pos} {type(pos)}')
+            elif not (np.array(pos).ndim == 1 and isinstance(pos[0], str)
+                      and np.array(pos).size > 0 and HAVE_XU):
+                raise ValueError(
+                    f'Illegal pos (HAVE_XU = {HAVE_XU}): {pos} {type(pos)}')
             if use_xu:
                 if atoms is None:
                     atoms = [material_name]
-                matl = xu.materials.Crystal(material_name, xu.materials.SGLattice(sgnum,
-                        *lattice_parameters, atoms=atoms, pos=[p for p in np.array(pos)]))
+                matl = materials.Crystal(
+                    material_name,
+                    materials.SGLattice(sgnum, *lattice_parameters,
+                                        atoms=atoms, pos=list(np.array(pos))))
             else:
                 matl = material.Material(material_name)
                 matl.sgnum = sgnum
                 matl.atominfo = np.vstack((pos.T, np.ones(pos.shape[0]))).T
                 matl.latticeParameters = lattice_parameters
-                matl.dmin = valWUnit('lp', 'length',  dmin_angstroms, 'angstrom')
+                matl.dmin = valWUnit(
+                    'lp', 'length', dmin_angstroms, 'angstrom')
                 exclusions = matl.planeData.get_exclusions()
                 powder_intensity = matl.planeData.powder_intensity
-                exclusions = [True if exclusion or i >= len(powder_intensity) or
-                        powder_intensity[i] < powder_intensity_cutoff else False
-                        for i, exclusion in enumerate(exclusions)]
+                exclusions = [
+                    exclusion or i >= len(powder_intensity)
+                    or powder_intensity[i] < POEDER_INTENSITY_CUTOFF
+                    for i, exclusion in enumerate(exclusions)]
                 matl.planeData.set_exclusions(exclusions)
-                logging.debug(f'powder_intensity = {matl.planeData.powder_intensity}')
-                logging.debug(f'exclusions = {matl.planeData.exclusions}')
+                logger.debug(
+                    f'powder_intensity = {matl.planeData.powder_intensity}')
+                logger.debug(f'exclusions = {matl.planeData.exclusions}')
         else:
-            if not have_hexrd:
-                raise ValueError('Illegal inputs: must provide detailed material info when '+
-                        'hexrd package is unavailable')
+            if not HAVE_HEXRD:
+                raise ValueError(
+                    'Illegal inputs: must provide detailed material info when '
+                    'hexrd package is unavailable')
             if sgnum is not None:
-                logging.warning('Ignore sgnum input when material_file is specified')
-            if not (os.path.splitext(material_file)[1] in ('.h5', '.hdf5', '.xtal', '.cif')):
+                logger.warning(
+                    'Ignore sgnum input when material_file is specified')
+            if not (path.splitext(material_file)[1] in
+                    ('.h5', '.hdf5', '.xtal', '.cif')):
                 raise ValueError(f'Illegal material file {material_file}')
-            matl = material.Material(material_name, material_file,
-                    dmin=valWUnit('lp', 'length',  dmin_angstroms, 'angstrom'))
+            matl = material.Material(
+                material_name, material_file,
+                dmin=valWUnit('lp', 'length', dmin_angstroms, 'angstrom'))
             if lattice_parameters_angstroms is not None:
                 matl.latticeParameters = lattice_parameters
             exclusions = matl.planeData.get_exclusions()
             powder_intensity = matl.planeData.powder_intensity
-            exclusions = [True if exclusion or i >= len(powder_intensity) or
-                    powder_intensity[i] < powder_intensity_cutoff else False
-                    for i, exclusion in enumerate(exclusions)]
+            exclusions = [
+                exclusion or i >= len(powder_intensity)
+                or powder_intensity[i] < POEDER_INTENSITY_CUTOFF
+                for i, exclusion in enumerate(exclusions)]
             matl.planeData.set_exclusions(exclusions)
-            logging.debug(f'powder_intensity = {matl.planeData.powder_intensity}')
-            logging.debug(f'exclusions = {matl.planeData.exclusions}')
+            logger.debug(
+                f'powder_intensity = {matl.planeData.powder_intensity}')
+            logger.debug(f'exclusions = {matl.planeData.exclusions}')
 
         return matl
-
```

### Comparing `ChessAnalysisPipeline-0.0.5/CHAP/common/utils/scanparsers.py` & `ChessAnalysisPipeline-0.0.6/CHAP/common/utils/scanparsers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,785 +1,1181 @@
 #!/usr/bin/env python3
 
 # -*- coding: utf-8 -*-
 
 # system modules
-import csv
-import fnmatch
-from functools import cache
-import json
+from csv import reader
+from fnmatch import filter as fnmatch_filter
+from json import load
 import os
 import re
 
-# necessary for the base class, ScanParser:
+# third party modules
 import numpy as np
-from pyspec.file.spec import FileSpec            
+from pyspec.file.spec import FileSpec
+
+
+class ScanParser:
+    """Partial implementation of a class representing a SPEC scan and
+    some of its metadata.
+
+    :param spec_file_name: path to a SPEC file on the CLASSE DAQ
+    :type spec_file_name: str
+    :param scan_number: the number of a scan in the SPEC file provided
+        with `spec_file_name`
+    :type scan_number: int
+    """
 
-class ScanParser(object):
     def __init__(self,
                  spec_file_name:str,
                  scan_number:int):
+        """Constructor method"""
 
         self.spec_file_name = spec_file_name
         self.scan_number = scan_number
-        
+
         self._scan_path = None
         self._scan_name = None
         self._scan_title = None
-        
+
         self._spec_scan = None
         self._spec_command = None
         self._spec_macro = None
         self._spec_args = None
         self._spec_scan_npts = None
         self._spec_scan_data = None
         self._spec_positioner_values = None
-        
+
         self._detector_data_path = None
-        
+
     def __repr__(self):
-        return(f'{self.__class__.__name__}({self.spec_file_name}, {self.scan_number}) -- {self.spec_command}')
-        
+        return (f'{self.__class__.__name__}'
+                f'({self.spec_file_name}, {self.scan_number}) '
+                f'-- {self.spec_command}')
+
     @property
     def spec_file(self):
-        # NB This FileSpec instance is not stored as a private attribute because
-        # it cannot be pickled (and therefore could cause problems for
-        # parallel code that uses ScanParsers).
-        return(FileSpec(self.spec_file_name))
+        # NB This FileSpec instance is not stored as a private
+        # attribute because it cannot be pickled (and therefore could
+        # cause problems for parallel code that uses ScanParsers).
+        return FileSpec(self.spec_file_name)
+
     @property
     def scan_path(self):
         if self._scan_path is None:
             self._scan_path = self.get_scan_path()
         return self._scan_path
+
     @property
     def scan_name(self):
         if self._scan_name is None:
             self._scan_name = self.get_scan_name()
         return self._scan_name
+
     @property
     def scan_title(self):
         if self._scan_title is None:
             self._scan_title = self.get_scan_title()
         return self._scan_title
+
     @property
     def spec_scan(self):
         if self._spec_scan is None:
             self._spec_scan = self.get_spec_scan()
         return self._spec_scan
+
     @property
     def spec_command(self):
         if self._spec_command is None:
             self._spec_command = self.get_spec_command()
         return self._spec_command
+
     @property
     def spec_macro(self):
         if self._spec_macro is None:
             self._spec_macro = self.get_spec_macro()
         return self._spec_macro
+
     @property
     def spec_args(self):
         if self._spec_args is None:
             self._spec_args = self.get_spec_args()
         return self._spec_args
+
     @property
     def spec_scan_npts(self):
         if self._spec_scan_npts is None:
             self._spec_scan_npts = self.get_spec_scan_npts()
         return self._spec_scan_npts
+
     @property
     def spec_scan_data(self):
         if self._spec_scan_data is None:
             self._spec_scan_data = self.get_spec_scan_data()
         return self._spec_scan_data
+
     @property
     def spec_positioner_values(self):
         if self._spec_positioner_values is None:
             self._spec_positioner_values = self.get_spec_positioner_values()
         return self._spec_positioner_values
+
     @property
     def detector_data_path(self):
         if self._detector_data_path is None:
             self._detector_data_path = self.get_detector_data_path()
         return self._detector_data_path
-    
+
     def get_scan_path(self):
-        return(os.path.dirname(self.spec_file_name))
+        """Return the name of the directory containining the SPEC file
+        for this scan.
+
+        :rtype: str
+        """
+        return os.path.dirname(self.spec_file_name)
+
     def get_scan_name(self):
-        return(None)
+        """Return the name of this SPEC scan (not unique to scans
+        within a single spec file).
+
+        :rtype: str
+        """
+        raise NotImplementedError
+
     def get_scan_title(self):
-        return(None)
+        """Return the title of this spec scan (unique to each scan
+        within a spec file).
+
+        :rtype: str
+        """
+        raise NotImplementedError
+
     def get_spec_scan(self):
-        return(self.spec_file.getScanByNumber(self.scan_number))
+        """Return the `pyspec.file.spec.Scan` object parsed from the
+        spec file and scan number provided to the constructor.
+
+        :rtype: pyspec.file.spec.Scan
+        """
+        return self.spec_file.getScanByNumber(self.scan_number)
+
     def get_spec_command(self):
-        return(self.spec_scan.command)
+        """Return the string command of this SPEC scan.
+
+        :rtype: str
+        """
+        return self.spec_scan.command
+
     def get_spec_macro(self):
-        return(self.spec_command.split()[0])
+        """Return the macro used in this scan's SPEC command.
+
+        :rtype: str
+        """
+        return self.spec_command.split()[0]
+
     def get_spec_args(self):
-        return(self.spec_command.split()[1:])
+        """Return a list of the arguments provided to the macro for
+        this SPEC scan.
+
+        :rtype: list[str]
+        """
+        return self.spec_command.split()[1:]
+
     def get_spec_scan_npts(self):
-        raise(NotImplementedError)
+        """Return the number of points collected in this SPEC scan
+
+        :rtype: int
+        """
+        raise NotImplementedError
+
     def get_spec_scan_data(self):
-        return(dict(zip(self.spec_scan.labels, self.spec_scan.data.T)))
+        """Return a dictionary of all the counter data collected by
+        this SPEC scan.
+
+        :rtype: dict[str, numpy.ndarray]
+        """
+        return dict(zip(self.spec_scan.labels, self.spec_scan.data.T))
+
     def get_spec_positioner_values(self):
+        """Return a dictionary of all the SPEC positioner values
+        recorded by SPEC just before the scan began.
+
+        :rtype: dict[str,str]
+        """
         positioner_values = dict(self.spec_scan.motor_positions)
         names = list(positioner_values.keys())
         mnemonics = self.spec_scan.motors
         if mnemonics is not None:
             for name,mnemonic in zip(names,mnemonics):
                 if name != mnemonic:
                     positioner_values[mnemonic] = positioner_values[name]
-        return(positioner_values)
+        return positioner_values
+
     def get_detector_data_path(self):
-        raise(NotImplementedError)
-    
-    def get_detector_data_file(self, detector_prefix, scan_step_index:int):
-        raise(NotImplementedError)
-    def get_detector_data(self, detector_prefix, scan_step_index:int):
-        '''
-        Return a np.ndarray of detector data.
+        """Return the name of the directory containing detector data
+        collected by this scan.
+
+        :rtype: str
+        """
+        raise NotImplementedError
 
-        :param detector_prefix: The detector's name in any data files, often
-        the EPICS macro $(P).
-        :type detector_substring: str
+    def get_detector_data_file(self, detector_prefix, scan_step_index:int):
+        """Return the name of the file containing detector data
+        collected at a certain step of this scan.
 
-        :param scan_step_index: The index of the scan step for which detector
-            data will be returned.
+        :param detector_prefix: the prefix used in filenames for the
+            detector
+        :type detector_prefix: str
+        :param scan_step_index: the index of the point in this scan
+            whose detector file name should be returned.
         :type scan_step_index: int
+        :rtype: str
+        """
+        raise NotImplementedError
+
+    def get_detector_data(self, detector_prefix, scan_step_index:int):
+        """Return the detector data collected at a certain step of
+        this scan.
 
-        :return: The detector data
-        :rtype: np.ndarray
-        '''
-        raise(NotImplementedError)
+        :param detector_prefix: the prefix used in filenames for the
+            detector
+        :type detector_prefix: str
+        :param scan_step_index: the index of the point in this scan
+            whose detector data should be returned.
+        :type scan_step_index: int
+        :rtype: numpy.ndarray
+        """
+        raise NotImplementedError
 
     def get_spec_positioner_value(self, positioner_name):
+        """Return the value of a spec positioner recorded before this
+        scan began.
+
+        :param positioner_name: the name or mnemonic of a SPEC motor
+            whose position should be returned.
+        :raises KeyError: if `positioner_name` is not the name or
+            mnemonic of a SPEC motor recorded for this scan.
+        :raises ValueError: if the recorded string value of the
+            positioner in the SPEC file cannot be converted to a
+            float.
+        :rtype: float
+        """
         try:
             positioner_value = self.spec_positioner_values[positioner_name]
             positioner_value = float(positioner_value)
-            return(positioner_value)
         except KeyError:
-            raise(KeyError(f'{self.scan_title}: motor {positioner_name} not found for this scan'))
+            raise KeyError(f'{self.scan_title}: motor {positioner_name} '
+                           'not found for this scan')
         except ValueError:
-            raise(ValueError(f'{self.scan_title}: ccould not convert value of {positioner_name} to float: {positioner_value}'))
+            raise ValueError(f'{self.scan_title}: could not convert value of'
+                             f' {positioner_name} to float: '
+                             f'{positioner_value}')
+        return positioner_value
 
 
 class FMBScanParser(ScanParser):
-    def __init__(self, spec_file_name, scan_number):
-        super().__init__(spec_file_name, scan_number)
+    """Partial implementation of a class representing a SPEC scan
+    collected at FMB.
+    """
+
     def get_scan_name(self):
-        return(os.path.basename(self.spec_file.abspath))
-    def get_scan_title(self):
-        return(f'{self.scan_name}_{self.scan_number:03d}')
+        return os.path.basename(self.spec_file.abspath)
 
+    def get_scan_title(self):
+        return f'{self.scan_name}_{self.scan_number:03d}'
 
 
 class SMBScanParser(ScanParser):
+    """Partial implementation of a class representing a SPEC scan
+    collected at SMB or FAST.
+    """
+
     def __init__(self, spec_file_name, scan_number):
         super().__init__(spec_file_name, scan_number)
-        
-        self._pars = None # purpose: store values found in the .par file as a dictionary
+
+        self._pars = None
         self.par_file_pattern = f'*-*-{self.scan_name}'
-        
+
     def get_scan_name(self):
-        return(os.path.basename(self.scan_path))
+        return os.path.basename(self.scan_path)
+
     def get_scan_title(self):
-        return(f'{self.scan_name}_{self.scan_number}')
-    
+        return f'{self.scan_name}_{self.scan_number}'
+
     @property
     def pars(self):
         if self._pars is None:
             self._pars = self.get_pars()
-        return(self._pars)
-        
+        return self._pars
+
     def get_pars(self):
+        """Return a dictionary of values recorded in the .par file
+        associated with this SPEC scan.
+
+        :rtype: dict[str,object]
+        """
         # JSON file holds titles for columns in the par file
-        json_files = fnmatch.filter(os.listdir(self.scan_path), f'{self.par_file_pattern}.json')
-        if not len(json_files) == 1:
-            raise(RuntimeError(f'{self.scan_title}: cannot find the .json file to decode the .par file'))
+        json_files = fnmatch_filter(
+            os.listdir(self.scan_path),
+            f'{self.par_file_pattern}.json')
+        if len(json_files) != 1:
+            raise RuntimeError(f'{self.scan_title}: cannot find the '
+                               '.json file to decode the .par file')
         with open(os.path.join(self.scan_path, json_files[0])) as json_file:
-            par_file_cols = json.load(json_file)
+            par_file_cols = load(json_file)
         try:
             par_col_names = list(par_file_cols.values())
             scann_val_idx = par_col_names.index('SCAN_N')
             scann_col_idx = int(list(par_file_cols.keys())[scann_val_idx])
         except:
-            raise(RuntimeError(f'{self.scan_title}: cannot find scan pars without a "SCAN_N" column in the par file'))
-        
-        par_files = fnmatch.filter(os.listdir(self.scan_path), f'{self.par_file_pattern}.par')
-        if not len(par_files) == 1:
-            raise(RuntimeError(f'{self.scan_title}: cannot find the .par file for this scan directory'))
+            raise RuntimeError(f'{self.scan_title}: cannot find scan pars '
+                               'without a "SCAN_N" column in the par file')
+
+        par_files = fnmatch_filter(
+            os.listdir(self.scan_path),
+            f'{self.par_file_pattern}.par')
+        if len(par_files) != 1:
+            raise RuntimeError(f'{self.scan_title}: cannot find the .par '
+                               'file for this scan directory')
+        par_dict = None
         with open(os.path.join(self.scan_path, par_files[0])) as par_file:
-            par_reader = csv.reader(par_file, delimiter=' ')
+            par_reader = reader(par_file, delimiter=' ')
             for row in par_reader:
                 if len(row) == len(par_col_names):
                     row_scann = int(row[scann_col_idx])
                     if row_scann == self.scan_number:
                         par_dict = {}
                         for par_col_idx,par_col_name in par_file_cols.items():
-                            # Convert the string par value from the file to an int or float, if possible.
+                            # Convert the string par value from the
+                            # file to an int or float, if possible.
                             par_value = row[int(par_col_idx)]
                             try:
                                 par_value = int(par_value)
                             except ValueError:
                                 try:
                                     par_value = float(par_value)
                                 except:
                                     pass
                             par_dict[par_col_name] = par_value
-                        return(par_dict)
-        raise(RuntimeError(f'{self.scan_title}: could not find scan pars for scan number {self.scan_number}'))
-            
+
+        if par_dict is None:
+            raise RuntimeError(f'{self.scan_title}: could not find scan pars '
+                               'for scan number {self.scan_number}')
+        return par_dict
+
     def get_counter_gain(self, counter_name):
+        """Return the gain of a counter as recorded in the comments of
+        a scan in a SPEC file converted to nA/V.
+
+        :param counter_name: the name of the counter
+        :type counter_name: str
+        :rtype: str
+        """
+        counter_gain = None
         for comment in self.spec_scan.comments:
-            match = re.search(f'{counter_name} gain: (?P<gain_value>\d+) (?P<unit_prefix>[m|u|n])A/V', comment)
+            match = re.search(
+                f'{counter_name} gain: '  # start of counter gain comments
+                '(?P<gain_value>\d+) '  # gain numerical value
+                '(?P<unit_prefix>[m|u|n])A/V',  # gain units
+                comment)
             if match:
                 unit_prefix = match['unit_prefix']
-                gain_scalar = 1 if unit_prefix == 'n' else 1e3 if unit_prefix == 'u' else 1e6
+                gain_scalar = 1 if unit_prefix == 'n' \
+                    else 1e3 if unit_prefix == 'u' else 1e6
                 counter_gain = f'{float(match["gain_value"])*gain_scalar} nA/V'
-                return(counter_gain)
-        raise(RuntimeError(f'{self.scan_title}: could not get gain for counter {counter_name}'))
+
+        if counter_gain is None:
+            raise RuntimeError(f'{self.scan_title}: could not get gain for '
+                               f'counter {counter_name}')
+        return counter_gain
 
 
 class LinearScanParser(ScanParser):
+    """Partial implementation of a class representing a typical line
+    or mesh scan in SPEC.
+    """
     def __init__(self, spec_file_name, scan_number):
         super().__init__(spec_file_name, scan_number)
-        
+
         self._spec_scan_motor_mnes = None
         self._spec_scan_motor_vals = None
-        self._spec_scan_shape = None        
+        self._spec_scan_shape = None
         self._spec_scan_dwell = None
 
     @property
     def spec_scan_motor_mnes(self):
         if self._spec_scan_motor_mnes is None:
             self._spec_scan_motor_mnes = self.get_spec_scan_motor_mnes()
         return self._spec_scan_motor_mnes
+
     @property
     def spec_scan_motor_vals(self):
         if self._spec_scan_motor_vals is None:
             self._spec_scan_motor_vals = self.get_spec_scan_motor_vals()
         return self._spec_scan_motor_vals
+
     @property
     def spec_scan_shape(self):
         if self._spec_scan_shape is None:
             self._spec_scan_shape = self.get_spec_scan_shape()
         return self._spec_scan_shape
+
     @property
     def spec_scan_dwell(self):
         if self._spec_scan_dwell is None:
             self._spec_scan_dwell = self.get_spec_scan_dwell()
-        return(self._spec_scan_dwell)
+        return self._spec_scan_dwell
+
+    def get_spec_scan_motor_mnes(self):
+        """Return the mnemonics of the SPEC motor(s) provided to the
+        macro for this scan. If there is more than one motor scanned
+        (in a "flymesh" scan, for example), the order of motors in the
+        returned tuple will go from the fastest moving motor first to
+        the slowest moving motor last.
+
+        :rtype: tuple
+        """
+        raise NotImplementedError
 
-    def get_spec_scan_motor_names(self):
-        raise(NotImplementedError)
     def get_spec_scan_motor_vals(self):
-        raise(NotImplementedError)
+        """Return the values visited by each of the scanned motors. If
+        there is more than one motor scanned (in a "flymesh" scan, for
+        example), the order of motor values in the returned tuple will
+        go from the fastest moving motor's values first to the slowest
+        moving motor's values last.
+
+        :rtype: tuple
+        """
+        raise NotImplementedError
+
     def get_spec_scan_shape(self):
-        raise(NotImplementedError)
+        """Return the number of points visited by each of the scanned
+        motors. If there is more than one motor scanned (in a
+        "flymesh" scan, for example), the order of number of motor
+        values in the returned tuple will go from the number of points
+        visited by the fastest moving motor first to the the number of
+        points visited by the slowest moving motor last.
+
+        :rtype: tuple
+        """
+        raise NotImplementedError
+
+    def get_spec_scan_dwell(self):
+        """Return the dwell time for each point in the scan as it
+        appears in the command string.
+
+        :rtype: float
+        """
+        raise NotImplementedError
+
     def get_spec_scan_npts(self):
-        return(np.prod(self.spec_scan_shape))
+        """Return the number of points collected in this SPEC scan.
+
+        :rtype: int
+        """
+        return np.prod(self.spec_scan_shape)
+
     def get_scan_step(self, scan_step_index:int):
+        """Return the index of each motor coordinate corresponding to
+        the index of a single point in the scan. If there is more than
+        one motor scanned (in a "flymesh" scan, for example), the
+        order of indices in the returned tuple will go from the index
+        of the value of the fastest moving motor first to the index of
+        the value of the slowest moving motor last.
+
+        :param scan_step_index: the index of a single point in the
+            scan.
+        :type scan_step_index: int
+        :rtype: tuple
+        """
         scan_steps = np.ndindex(self.spec_scan_shape[::-1])
         i = 0
         while i <= scan_step_index:
             scan_step = next(scan_steps)
             i += 1
-        return(scan_step)
+        return scan_step
+
     def get_scan_step_index(self, scan_step:tuple):
+        """Return the index of a single scan point corresponding to a
+        tuple of indices for each scanned motor coordinate.
+
+        :param scan_step: a tuple of the indices of each scanned motor
+            coordinate. If there is more than one motor scanned (in a
+            "flymesh" scan, for example), the order of indices should
+            go from the index of the value of the fastest moving motor
+            first to the index of the value of the slowest moving
+            motor last.
+        :type scan_step: tuple
+        :trype: int
+        """
         scan_steps = np.ndindex(self.spec_scan_shape[::-1])
         scan_step_found = False
         scan_step_index = -1
         while not scan_step_found:
             next_scan_step = next(scan_steps)
             scan_step_index += 1
             if next_scan_step == scan_step:
                 scan_step_found = True
                 break
-        return(scan_step_index)
+        return scan_step_index
 
 
 class FMBLinearScanParser(LinearScanParser, FMBScanParser):
-    def __init__(self, spec_file_name, scan_number): 
-        super().__init__(spec_file_name, scan_number)
-        
+    """Partial implementation of a class representing a typical line
+    or mesh scan in SPEC collected at FMB.
+    """
+
     def get_spec_scan_motor_mnes(self):
         if self.spec_macro == 'flymesh':
-            return((self.spec_args[0], self.spec_args[5]))
-        elif self.spec_macro == 'flyscan':
-            return((self.spec_args[0],))
-        elif self.spec_macro in ('tseries', 'loopscan'):
-            return(('Time',))
-        else:
-            raise(RuntimeError(f'{self.scan_title}: cannot determine scan motors for scans of type {self.spec_macro}'))
+            return (self.spec_args[0], self.spec_args[5])
+        if self.spec_macro == 'flyscan':
+            return (self.spec_args[0],)
+        if self.spec_macro in ('tseries', 'loopscan'):
+            return ('Time',)
+        raise RuntimeError(f'{self.scan_title}: cannot determine scan motors '
+                           f'for scans of type {self.spec_macro}')
+
     def get_spec_scan_motor_vals(self):
         if self.spec_macro == 'flymesh':
-            fast_mot_vals = np.linspace(float(self.spec_args[1]), float(self.spec_args[2]), int(self.spec_args[3])+1)
-            slow_mot_vals = np.linspace(float(self.spec_args[6]), float(self.spec_args[7]), int(self.spec_args[8])+1)
-            return((fast_mot_vals, slow_mot_vals))
-        elif self.spec_macro == 'flyscan':
-            mot_vals = np.linspace(float(self.spec_args[1]), float(self.spec_args[2]), int(self.spec_args[3])+1)
-            return((mot_vals,))
-        elif self.spec_macro in ('tseries', 'loopscan'):
-            return(self.spec_scan.data[:,0])
-        else:
-            raise(RuntimeError(f'{self.scan_title}: cannot determine scan motors for scans of type {self.spec_macro}'))
+            fast_mot_vals = np.linspace(float(self.spec_args[1]),
+                                        float(self.spec_args[2]),
+                                        int(self.spec_args[3])+1)
+            slow_mot_vals = np.linspace(float(self.spec_args[6]),
+                                        float(self.spec_args[7]),
+                                        int(self.spec_args[8])+1)
+            return (fast_mot_vals, slow_mot_vals)
+        if self.spec_macro == 'flyscan':
+            mot_vals = np.linspace(float(self.spec_args[1]),
+                                   float(self.spec_args[2]),
+                                   int(self.spec_args[3])+1)
+            return (mot_vals,)
+        if self.spec_macro in ('tseries', 'loopscan'):
+            return self.spec_scan.data[:,0]
+        raise RuntimeError(f'{self.scan_title}: cannot determine scan motors '
+                           f'for scans of type {self.spec_macro}')
+
     def get_spec_scan_shape(self):
         if self.spec_macro == 'flymesh':
             fast_mot_npts = int(self.spec_args[3])+1
             slow_mot_npts = int(self.spec_args[8])+1
-            return((fast_mot_npts, slow_mot_npts))
-        elif self.spec_macro == 'flyscan':
+            return (fast_mot_npts, slow_mot_npts)
+        if self.spec_macro == 'flyscan':
             mot_npts = int(self.spec_args[3])+1
-            return((mot_npts,))
-        elif self.spec_macro in ('tseries', 'loopscan'):
-            return(len(np.array(self.spec_scan.data[:,0])))
-        else:
-            raise(RuntimeError(f'{self.scan_title}: cannot determine scan shape for scans of type {self.spec_macro}'))
+            return (mot_npts,)
+        if self.spec_macro in ('tseries', 'loopscan'):
+            return len(np.array(self.spec_scan.data[:,0]))
+        raise RuntimeError(f'{self.scan_title}: cannot determine scan shape '
+                           f'for scans of type {self.spec_macro}')
+
     def get_spec_scan_dwell(self):
         if self.spec_macro in ('flymesh', 'flyscan'):
-            return(float(self.spec_args[4]))
-        elif self.spec_macro in ('tseries', 'loopscan'):
-            return(float(self.spec_args[1]))
-        else:
-            raise(RuntimeError(f'{self.scan_title}: cannot determine dwell for scans of type {self.spec_macro}'))
+            return float(self.spec_args[4])
+        if self.spec_macro in ('tseries', 'loopscan'):
+            return float(self.spec_args[1])
+        raise RuntimeError(f'{self.scan_title}: cannot determine dwell for '
+                           f'scans of type {self.spec_macro}')
+
     def get_detector_data_path(self):
-        return(os.path.join(self.scan_path, self.scan_title))
+        return os.path.join(self.scan_path, self.scan_title)
 
 
 class FMBSAXSWAXSScanParser(FMBLinearScanParser):
-    def __init__(self, spec_file_name, scan_number):
-        super().__init__(spec_file_name, scan_number)
+    """Concrete implementation of a class representing a scan taken
+    with the typical SAXS/WAXS setup at FMB.
+    """
 
     def get_scan_title(self):
-        return(f'{self.scan_name}_{self.scan_number:03d}')
+        return f'{self.scan_name}_{self.scan_number:03d}'
+
     def get_detector_data_file(self, detector_prefix, scan_step_index:int):
         scan_step = self.get_scan_step(scan_step_index)
-        file_indices = [f'{scan_step[i]:03d}' for i in range(len(self.spec_scan_shape)) if self.spec_scan_shape[i] != 1]
-        file_name = f'{self.scan_name}_{detector_prefix}_{self.scan_number:03d}_{"_".join(file_indices)}.tiff'
+        file_indices = [f'{scan_step[i]:03d}'
+                        for i in range(len(self.spec_scan_shape))
+                        if self.spec_scan_shape[i] != 1]
+        file_name = f'{self.scan_name}_{detector_prefix}_' \
+                    f'{self.scan_number:03d}_{"_".join(file_indices)}.tiff'
         file_name_full = os.path.join(self.detector_data_path, file_name)
         if os.path.isfile(file_name_full):
-            return(file_name_full)
-        else:
-            raise(RuntimeError(f'{self.scan_title}: could not find detector image file for detector {detector_prefix} scan step ({scan_step})'))
+            return file_name_full
+        raise RuntimeError(f'{self.scan_title}: could not find detector image '
+                           f'file for detector {detector_prefix} scan step '
+                           f'({scan_step})')
+
     def get_detector_data(self, detector_prefix, scan_step_index:int):
+        # third party modules
         from pyspec.file.tiff import TiffFile
-        image_file = self.get_detector_data_file(detector_prefix, scan_step_index)
+
+        image_file = self.get_detector_data_file(detector_prefix,
+                                                 scan_step_index)
         with TiffFile(image_file) as tiff_file:
             image_data = tiff_file.asarray()
-        return(image_data)
+        return image_data
 
 
 class FMBXRFScanParser(FMBLinearScanParser):
-    def __init__(self, spec_file_name, scan_number):
-        super().__init__(spec_file_name, scan_number)
+    """Concrete implementation of a class representing a scan taken
+    with the typical XRF setup at FMB.
+    """
+
     def get_scan_title(self):
-        return(f'{self.scan_name}_scan{self.scan_number}')        
+        return f'{self.scan_name}_scan{self.scan_number}'
+
     def get_detector_data_file(self, detector_prefix, scan_step_index:int):
         scan_step = self.get_scan_step(scan_step_index)
         file_name = f'scan{self.scan_number}_{scan_step[1]:03d}.hdf5'
         file_name_full = os.path.join(self.detector_data_path, file_name)
         if os.path.isfile(file_name_full):
-            return(file_name_full)
-        else:
-            raise(RuntimeError(f'{self.scan_title}: could not find detector image file for detector {detector_prefix} scan step ({scan_step_index})'))
+            return file_name_full
+        raise RuntimeError(f'{self.scan_title}: could not find detector image '
+                           f'file for detector {detector_prefix} scan step '
+                           f'({scan_step_index})')
+
     def get_detector_data(self, detector_prefix, scan_step_index:int):
-        import h5py
-        detector_file = self.get_detector_data_file(detector_prefix, scan_step_index)
+        # third party modules
+        from h5py import File
+
+        detector_file = self.get_detector_data_file(
+            detector_prefix, scan_step_index)
         scan_step = self.get_scan_step(scan_step_index)
-        with h5py.File(detector_file) as h5_file:
-            detector_data = h5_file['/entry/instrument/detector/data'][scan_step[0]]
-        return(detector_data) 
+        with File(detector_file) as h5_file:
+            detector_data = \
+                h5_file['/entry/instrument/detector/data'][scan_step[0]]
+        return detector_data
 
 
 class SMBLinearScanParser(LinearScanParser, SMBScanParser):
-    def __init__(self, spec_file_name, scan_number):
-        super().__init__(spec_file_name, scan_number)        
+    """Concrete implementation of a class representing a scan taken
+    with the typical powder diffraction setup at SMB.
+    """
+
     def get_spec_scan_motor_mnes(self):
         if self.spec_macro == 'flymesh':
-            return((self.spec_args[0], self.spec_args[5]))
-        elif self.spec_macro == 'flyscan':
-            return((self.spec_args[0],))
-        elif self.spec_macro in ('tseries', 'loopscan'):
-            return(('Time',))
-        else:
-            raise(RuntimeError(f'{self.scan_title}: cannot determine scan motors for scans of type {self.spec_macro}'))
+            return (self.spec_args[0], self.spec_args[5])
+        if self.spec_macro == 'flyscan':
+            return (self.spec_args[0],)
+        if self.spec_macro in ('tseries', 'loopscan'):
+            return ('Time',)
+        raise RuntimeError(f'{self.scan_title}: cannot determine scan motors '
+                           f'for scans of type {self.spec_macro}')
+
     def get_spec_scan_motor_vals(self):
         if self.spec_macro == 'flymesh':
-            fast_mot_vals = np.linspace(float(self.spec_args[1]), float(self.spec_args[2]), int(self.spec_args[3])+1)
-            slow_mot_vals = np.linspace(float(self.spec_args[6]), float(self.spec_args[7]), int(self.spec_args[8])+1)
-            return((fast_mot_vals, slow_mot_vals))
-        elif self.spec_macro == 'flyscan':
-            mot_vals = np.linspace(float(self.spec_args[1]), float(self.spec_args[2]), int(self.spec_args[3])+1)
-            return((mot_vals,))
-        elif self.spec_macro in ('tseries', 'loopscan'):
-            return(self.spec_scan.data[:,0])
-        else:
-            raise(RuntimeError(f'{self.scan_title}: cannot determine scan motors for scans of type {self.spec_macro}'))
+            fast_mot_vals = np.linspace(float(self.spec_args[1]),
+                                        float(self.spec_args[2]),
+                                        int(self.spec_args[3])+1)
+            slow_mot_vals = np.linspace(float(self.spec_args[6]),
+                                        float(self.spec_args[7]),
+                                        int(self.spec_args[8])+1)
+            return (fast_mot_vals, slow_mot_vals)
+        if self.spec_macro == 'flyscan':
+            mot_vals = np.linspace(float(self.spec_args[1]),
+                                   float(self.spec_args[2]),
+                                   int(self.spec_args[3])+1)
+            return (mot_vals,)
+        if self.spec_macro in ('tseries', 'loopscan'):
+            return self.spec_scan.data[:,0]
+        raise RuntimeError(f'{self.scan_title}: cannot determine scan motors '
+                           f'for scans of type {self.spec_macro}')
+
     def get_spec_scan_shape(self):
         if self.spec_macro == 'flymesh':
             fast_mot_npts = int(self.spec_args[3])+1
             slow_mot_npts = int(self.spec_args[8])+1
-            return((fast_mot_npts, slow_mot_npts))
-        elif self.spec_macro == 'flyscan':
+            return (fast_mot_npts, slow_mot_npts)
+        if self.spec_macro == 'flyscan':
             mot_npts = int(self.spec_args[3])+1
-            return((mot_npts,))
-        elif self.spec_macro in ('tseries', 'loopscan'):
-            return(len(np.array(self.spec_scan.data[:,0])))
-        else:
-            raise(RuntimeError(f'{self.scan_title}: cannot determine scan shape for scans of type {self.spec_macro}'))
+            return (mot_npts,)
+        if self.spec_macro in ('tseries', 'loopscan'):
+            return len(np.array(self.spec_scan.data[:,0]))
+        raise RuntimeError(f'{self.scan_title}: cannot determine scan shape '
+                           f'for scans of type {self.spec_macro}')
+
     def get_spec_scan_dwell(self):
         if self.spec_macro == 'flymesh':
-            return(float(self.spec_args[4]))
-        elif self.spec_macro == 'flyscan':
-            return(float(self.spec_args[-1]))
-        else:
-            raise(RuntimeError(f'{self.scan_title}: cannot determine dwell time for scans of type {self.spec_macro}'))
+            return float(self.spec_args[4])
+        if self.spec_macro == 'flyscan':
+            return float(self.spec_args[-1])
+        raise RuntimeError(f'{self.scan_title}: cannot determine dwell time '
+                           f'for scans of type {self.spec_macro}')
+
     def get_detector_data_path(self):
-        return(os.path.join(self.scan_path, str(self.scan_number)))
+        return os.path.join(self.scan_path, str(self.scan_number))
+
     def get_detector_data_file(self, detector_prefix, scan_step_index:int):
         scan_step = self.get_scan_step(scan_step_index)
         if len(scan_step) == 1:
             scan_step = (0, *scan_step)
-        file_name_pattern = f'{detector_prefix}_{self.scan_name}_*_{scan_step[0]}_data_{(scan_step[1]+1):06d}.h5'
-        file_name_matches = fnmatch.filter(os.listdir(self.detector_data_path), file_name_pattern)
+        file_name_pattern = (f'{detector_prefix}_'
+                             f'{self.scan_name}_*_'
+                             f'{scan_step[0]}_data_'
+                             f'{(scan_step[1]+1):06d}.h5')
+        file_name_matches = fnmatch_filter(
+            os.listdir(self.detector_data_path),
+            file_name_pattern)
         if len(file_name_matches) == 1:
-            return(os.path.join(self.detector_data_path, file_name_matches[0]))
-        else:
-            raise(RuntimeError(f'{self.scan_title}: could not find detector image file for detector {detector_prefix} scan step ({scan_step_index})'))
+            return os.path.join(self.detector_data_path, file_name_matches[0])
+        raise RuntimeError(f'{self.scan_title}: could not find detector image '
+                           f'file for detector {detector_prefix} scan step '
+                           f'({scan_step_index})')
+
     def get_detector_data(self, detector_prefix, scan_step_index:int):
-        import h5py
-        image_file = self.get_detector_data_file(detector_prefix, scan_step_index)
-        with h5py.File(image_file) as h5_file:
+        # third party modules
+        from h5py import File
+
+        image_file = self.get_detector_data_file(
+            detector_prefix, scan_step_index)
+        with File(image_file) as h5_file:
             image_data = h5_file['/entry/data/data'][0]
-        return(image_data)
+        return image_data
 
 
 class RotationScanParser(ScanParser):
+    """Partial implementation of a class representing a rotation
+    scan.
+    """
+
     def __init__(self, spec_file_name, scan_number):
         super().__init__(spec_file_name, scan_number)
 
         self._scan_type = None
         self._theta_vals = None
         self._horizontal_shift = None
         self._vertical_shift = None
         self._starting_image_index = None
         self._starting_image_offset = None
 
     @property
     def scan_type(self):
         if self._scan_type is None:
             self._scan_type = self.get_scan_type()
-        return(self._scan_type)
+        return self._scan_type
+
     @property
     def theta_vals(self):
         if self._theta_vals is None:
             self._theta_vals = self.get_theta_vals()
-        return(self._theta_vals)
+        return self._theta_vals
+
     @property
     def horizontal_shift(self):
         if self._horizontal_shift is None:
             self._horizontal_shift = self.get_horizontal_shift()
-        return(self._horizontal_shift)
+        return self._horizontal_shift
+
     @property
     def vertical_shift(self):
         if self._vertical_shift is None:
             self._vertical_shift = self.get_vertical_shift()
-        return(self._vertical_shift)
+        return self._vertical_shift
+
     @property
     def starting_image_index(self):
         if self._starting_image_index is None:
             self._starting_image_index = self.get_starting_image_index()
-        return(self._starting_image_index)
+        return self._starting_image_index
+
     @property
     def starting_image_offset(self):
         if self._starting_image_offset is None:
             self._starting_image_offset = self.get_starting_image_offset()
-        return(self._starting_image_offset)
- 
+        return self._starting_image_offset
+
     def get_scan_type(self):
-        return(None)
+        """Return a string identifier for the type of tomography data
+        being collected by this scan: df1 (dark field), bf1 (bright
+        field), or tf1 (sample tomography data).
+
+        :rtype: typing.Literal['df1', 'bf1', 'tf1']
+        """
+        return None
+
     def get_theta_vals(self):
-        raise(NotImplementedError)
+        """Return a dictionary of information about the angular values
+        visited by the rotating motor at each point in the scan. The
+        dictionary may contain a single key, "num", or three keys:
+        "num", "start", and "end"
+
+        :rtype: dict[str, float]"""
+        raise NotImplementedError
+
     def get_horizontal_shift(self):
-        raise(NotImplementedError)
+        """Return the value of the motor that shifts the sample in the
+        +x direction (hutch frame). Useful when tomography scans are
+        taken in a series of stacks when the sample is wider than the
+        width of the beam.
+
+        :rtype: float
+        """
+        raise NotImplementedError
+
     def get_vertical_shift(self):
-        raise(NotImplementedError)
+        """Return the value of the motor that shifts the sample in the
+        +z direction (hutch frame). Useful when tomography scans are
+        taken in a series of stacks when the sample is taller than the
+        height of the beam.
+
+        :rtype: float
+        """
+        raise NotImplementedError
+
     def get_starting_image_index(self):
-        raise(NotImplementedError)
+        """Return the index of the first frame of detector data
+        collected by this scan.
+
+        :rtype: int
+        """
+        raise NotImplementedError
+
     def get_starting_image_offset(self):
-        raise(NotImplementedError)
+        """Return the offet of the index of the first "good" frame of
+        detector data collected by this scan from the index of the
+        first frame of detector data collected by this scan.
+
+        :rtype: int
+        """
+        raise NotImplementedError
+
     def get_num_image(self, detector_prefix):
-        raise(NotImplementedError)
+        """Return the total number of "good" frames of detector data
+        collected by this scan
+
+        :rtype: int
+        """
+        raise NotImplementedError
 
 
 class FMBRotationScanParser(RotationScanParser, FMBScanParser):
-    def __init__(self, spec_file_name, scan_number):
-        super().__init__(spec_file_name, scan_number)
+    """Concrete implementation of a class representing a scan taken
+    with the typical tomography setup at FMB.
+    """
+
     def get_spec_scan_npts(self):
         if self.spec_macro == 'flyscan':
             if len(self.spec_args) == 2:
                 # Flat field (dark or bright)
-                return(int(self.spec_args[0])+1)
-            elif len(self.spec_args) == 5:
-                return(int(self.spec_args[3])+1)
-            else:
-                raise(RuntimeError(f'{self.scan_title}: cannot obtain number of points from '+
-                        f'{self.spec_macro} with arguments {self.spec_args}'))
-        else:
-            raise(RuntimeError(f'{self.scan_title}: cannot determine number of points for scans '+
-                    f'of type {self.spec_macro}'))
+                return int(self.spec_args[0])+1
+            if len(self.spec_args) == 5:
+                return int(self.spec_args[3])+1
+            raise RuntimeError(f'{self.scan_title}: cannot obtain number of '
+                               f'points from {self.spec_macro} with '
+                               f'arguments {self.spec_args}')
+        raise RuntimeError(f'{self.scan_title}: cannot determine number of '
+                           f'points for scans of type {self.spec_macro}')
+
     def get_theta_vals(self):
         if self.spec_macro == 'flyscan':
             if len(self.spec_args) == 2:
                 # Flat field (dark or bright)
-                return({'num': int(self.spec_args[0])})
-            elif len(self.spec_args) == 5:
-                return({'start': float(self.spec_args[1]), 'end': float(self.spec_args[2]),
-                        'num': int(self.spec_args[3])+1})
-            else:
-                raise(RuntimeError(f'{self.scan_title}: cannot obtain theta values from '+
-                        f'{self.spec_macro} with arguments {self.spec_args}'))
-        else:
-            raise(RuntimeError(f'{self.scan_title}: cannot determine theta values for scans '+
-                    f'of type {self.spec_macro}'))
+                return {'num': int(self.spec_args[0])}
+            if len(self.spec_args) == 5:
+                return {'start': float(self.spec_args[1]),
+                        'end': float(self.spec_args[2]),
+                        'num': int(self.spec_args[3])+1}
+            raise RuntimeError(f'{self.scan_title}: cannot obtain theta values'
+                               f' from {self.spec_macro} with arguments '
+                               f'{self.spec_args}')
+        raise RuntimeError(f'{self.scan_title}: cannot determine theta values '
+                           f'for scans of type {self.spec_macro}')
+
     def get_horizontal_shift(self):
-        return(0.0)
+        return 0.0
+
     def get_vertical_shift(self):
-        return(float(self.get_spec_positioner_value('4C_samz')))
+        return float(self.get_spec_positioner_value('4C_samz'))
+
     def get_starting_image_index(self):
-        return(0)
+        return 0
+
     def get_starting_image_offset(self):
-        return(1)
+        return 1
+
     def get_num_image(self, detector_prefix):
-        import h5py
+        # third party modules
+        from h5py import File
+
         detector_file = self.get_detector_data_file(detector_prefix)
-        with h5py.File(detector_file) as h5_file:
+        with File(detector_file) as h5_file:
             num_image = h5_file['/entry/instrument/detector/data'].shape[0]
-        return(num_image-self.starting_image_offset)
+        return num_image-self.starting_image_offset
+
     def get_detector_data_path(self):
-        return(self.scan_path)
+        return self.scan_path
+
     def get_detector_data_file(self, detector_prefix):
         prefix = detector_prefix.upper()
         file_name = f'{self.scan_name}_{prefix}_{self.scan_number:03d}.h5'
         file_name_full = os.path.join(self.detector_data_path, file_name)
         if os.path.isfile(file_name_full):
-            return(file_name_full)
-        else:
-            raise(RuntimeError(f'{self.scan_title}: could not find detector image file for '+
-                    f'detector {detector_prefix}'))
-    #@cache
-    def get_all_detector_data_in_file(self, detector_prefix, scan_step_index=None):
-        import h5py
+            return file_name_full
+        raise RuntimeError(f'{self.scan_title}: could not find detector image '
+                           f'file for detector {detector_prefix}')
+
+    def get_all_detector_data_in_file(
+            self, detector_prefix, scan_step_index=None):
+        # third party modules
+        from h5py import File
+
         detector_file = self.get_detector_data_file(detector_prefix)
-        with h5py.File(detector_file) as h5_file:
+        with File(detector_file) as h5_file:
             if scan_step_index is None:
                 detector_data = h5_file['/entry/instrument/detector/data'][
-                        self.starting_image_index:]
+                    self.starting_image_index:]
             elif isinstance(scan_step_index, int):
                 detector_data = h5_file['/entry/instrument/detector/data'][
-                        self.starting_image_index+scan_step_index]
-            elif isinstance(scan_step_index, (list, tuple)) and len(scan_step_index) == 2:
+                    self.starting_image_index+scan_step_index]
+            elif (isinstance(scan_step_index, (list, tuple))
+                    and len(scan_step_index) == 2):
                 detector_data = h5_file['/entry/instrument/detector/data'][
-                        self.starting_image_index+scan_step_index[0]:
-                        self.starting_image_index+scan_step_index[1]]
+                    self.starting_image_index+scan_step_index[0]:
+                    self.starting_image_index+scan_step_index[1]]
             else:
-                raise(ValueError(f'Invalid parameter scan_step_index ({scan_step_index})'))
-        return(detector_data)
+                raise ValueError('Invalid parameter scan_step_index '
+                                 f'({scan_step_index})')
+        return detector_data
+
     def get_detector_data(self, detector_prefix, scan_step_index=None):
-        return(self.get_all_detector_data_in_file(detector_prefix, scan_step_index))
+        return self.get_all_detector_data_in_file(
+            detector_prefix, scan_step_index)
 
 
 class SMBRotationScanParser(RotationScanParser, SMBScanParser):
+    """Concrete implementation of a class representing a scan taken
+    with the typical tomography setup at SMB.
+    """
+
     def __init__(self, spec_file_name, scan_number):
         super().__init__(spec_file_name, scan_number)
+
         self.par_file_pattern = f'id*-*tomo*-{self.scan_name}'
+
     def get_spec_scan_npts(self):
-        if self.spec_macro == 'slew_ome' or self.spec_macro == 'rams4_slew_ome':
-            return(int(self.pars['nframes_real']))
-        else:
-            raise(RuntimeError(f'{self.scan_title}: cannot determine number of points for scans of type {self.spec_macro}'))
+        if self.spec_macro in ('slew_ome','rams4_slew_ome'):
+            return int(self.pars['nframes_real'])
+        raise RuntimeError(f'{self.scan_title}: cannot determine number of '
+                           f'points for scans of type {self.spec_macro}')
+
     def get_scan_type(self):
-        try:
-            return(self.pars['tomo_type'])
-        except:
-            try:
-                return(self.pars['tomotype'])
-            except:
-                raise(RuntimeError(f'{self.scan_title}: cannot determine the scan_type'))
+        scan_type = self.pars.get('tomo_type',
+                                  self.pars.get('tomotype', None))
+        if scan_type is None:
+            raise RuntimeError(f'{self.scan_title}: cannot determine '
+                               'the scan_type')
+        return scan_type
+
     def get_theta_vals(self):
-        return({'start': float(self.pars['ome_start_real']),
-                'end': float(self.pars['ome_end_real']), 'num': int(self.pars['nframes_real'])})
+        return {'start': float(self.pars['ome_start_real']),
+                'end': float(self.pars['ome_end_real']),
+                'num': int(self.pars['nframes_real'])}
+
     def get_horizontal_shift(self):
-        try:
-            return(float(self.pars['rams4x']))
-        except:
-            try:
-                return(float(self.pars['ramsx']))
-            except:
-                raise(RuntimeError(f'{self.scan_title}: cannot determine the horizontal shift'))
+        horizontal_shift = self.pars.get(
+            'rams4x', self.pars.get('ramsx', None))
+        if horizontal_shift is None:
+            raise RuntimeError(
+                f'{self.scan_title}: cannot determine the horizontal shift')
+        return horizontal_shift
+
     def get_vertical_shift(self):
-        try:
-            return(float(self.pars['rams4z']))
-        except:
-            try:
-                return(float(self.pars['ramsz']))
-            except:
-                raise(RuntimeError(f'{self.scan_title}: cannot determine the vertical shift'))
+        vertical_shift = self.pars.get(
+            'rams4z', self.pars.get('ramsz', None))
+        if vertical_shift is None:
+            raise RuntimeError(
+                f'{self.scan_title}: cannot determine the vertical shift')
+        return vertical_shift
+
     def get_starting_image_index(self):
         try:
-            return(int(self.pars['junkstart']))
+            return int(self.pars['junkstart'])
         except:
-            raise(RuntimeError(f'{self.scan_title}: cannot determine first detector image index'))
+            raise RuntimeError(f'{self.scan_title}: cannot determine first '
+                               'detector image index')
+
     def get_starting_image_offset(self):
         try:
-            return(int(self.pars['goodstart'])-self.get_starting_image_index())
+            return (int(self.pars['goodstart'])
+                    - self.get_starting_image_index())
         except:
-            raise(RuntimeError(f'{self.scan_title}: cannot determine index offset of first good '+
-                    'detector image'))
+            raise RuntimeError(f'{self.scan_title}: cannot determine index '
+                               'offset of first good detector image')
+
     def get_num_image(self, detector_prefix=None):
         try:
-            return(int(self.pars['nframes_real']))
-#            indexRegex = re.compile(r'\d+')
+            return int(self.pars['nframes_real'])
+#            index_regex = re.compile(r'\d+')
 #            # At this point only tiffs
 #            path = self.get_detector_data_path()
-#            files = sorted([f for f in os.listdir(path) if os.path.isfile(os.path.join(path, f)) and
-#                    f.endswith('.tif') and indexRegex.search(f)])
-#            return(len(files)-self.starting_image_offset)
+#            files = sorted([f for f in os.listdir(path) \
+#                if os.path.isfile(os.path.join(path, f)) \
+#                and f.endswith('.tif') \
+#                and index_regex.search(f)])
+#            return len(files)-self.starting_image_offset
         except:
-            raise(RuntimeError(f'{self.scan_title}: cannot determine the number of good '+
-                    'detector images'))
+            raise RuntimeError(f'{self.scan_title}: cannot determine the '
+                               'number of good detector images')
+
     def get_detector_data_path(self):
-        return(os.path.join(self.scan_path, str(self.scan_number), 'nf'))
+        return os.path.join(self.scan_path, str(self.scan_number), 'nf')
+
     def get_detector_data_file(self, scan_step_index:int):
         file_name = f'nf_{self.starting_image_index+scan_step_index:06d}.tif'
         file_name_full = os.path.join(self.detector_data_path, file_name)
         if os.path.isfile(file_name_full):
-            return(file_name_full)
-        else:
-            raise(RuntimeError(f'{self.scan_title}: could not find detector image file for '+
-                    f'scan step ({scan_step_index})'))
+            return file_name_full
+        raise RuntimeError(f'{self.scan_title}: could not find detector image '
+                           f'file for scan step ({scan_step_index})')
+
     def get_detector_data(self, detector_prefix, scan_step_index=None):
         if scan_step_index is None:
             detector_data = []
             for index in range(len(self.get_num_image(detector_prefix))):
-                detector_data.append(self.get_detector_data(detector_prefix, index))
+                detector_data.append(
+                    self.get_detector_data(detector_prefix, index))
             detector_data = np.asarray(detector_data)
         elif isinstance(scan_step_index, int):
-            image_file = self.get_detector_data_file(scan_step_index)
+            # third party modules
             from pyspec.file.tiff import TiffFile
+
+            image_file = self.get_detector_data_file(scan_step_index)
             with TiffFile(image_file) as tiff_file:
                 detector_data = tiff_file.asarray()
-        elif isinstance(scan_step_index, (list, tuple)) and len(scan_step_index) == 2:
+        elif (isinstance(scan_step_index, (list, tuple))
+                and len(scan_step_index) == 2):
             detector_data = []
             for index in range(scan_step_index[0], scan_step_index[1]):
-                detector_data.append(self.get_detector_data(detector_prefix, index))
+                detector_data.append(
+                    self.get_detector_data(detector_prefix, index))
             detector_data = np.asarray(detector_data)
         else:
-            raise(ValueError(f'Invalid parameter scan_step_index ({scan_step_index})'))
-        return(detector_data)
+            raise ValueError('Invalid parameter scan_step_index '
+                             f'({scan_step_index})')
+        return detector_data
 
 
 class MCAScanParser(ScanParser):
+    """Partial implementation of a class representing a scan taken
+    while collecting SPEC MCA data.
+    """
+
     def __init__(self, spec_file_name, scan_number):
         super().__init__(spec_file_name, scan_number)
-        
+
         self._dwell_time = None
         self._detector_num_bins = None
-        
+
     @property
     def dwell_time(self):
         if self._dwell_time is None:
             self._dwell_time = self.get_dwell_time()
-        return(self._dwell_time)
-    
+        return self._dwell_time
+
     def get_dwell_time(self):
-        raise(NotImplementedError)
-    @cache
+        """Return the dwell time for each scan point as it appears in
+        the SPEC command.
+
+        :rtype: float
+        """
+        raise NotImplementedError
+
     def get_detector_num_bins(self, detector_prefix):
-        raise(NotImplementedError)
+        """Return the number of bins for the detector with the given
+        prefix.
+
+        :param detector_prefix: the detector prefix as used in SPEC
+            MCA data files
+        :type detector_prefix: str
+        :rtype: int
+        """
+        raise NotImplementedError
+
 
 class SMBMCAScanParser(MCAScanParser, SMBScanParser):
-    def __init__(self, spec_file_name, scan_number):
-        super().__init__(spec_file_name, scan_number)
-            
+    """Concrete implementation of a class representing a scan taken
+    with the typical EDD setup at SMB or FAST.
+    """
+
     def get_spec_scan_npts(self):
         if self.spec_macro == 'tseries':
-            return(1)
-        elif self.spec_macro == 'ascan':
-            return(int(self.spec_args[3]))
-        elif self.spec_scan == 'wbslew_scan':
-            return(1)
-        else:
-            raise(RuntimeError(f'{self.scan_title}: cannot determine number of points for scans of type {self.spec_macro}'))
+            return 1
+        if self.spec_macro == 'ascan':
+            return int(self.spec_args[3])
+        if self.spec_scan == 'wbslew_scan':
+            return 1
+        raise RuntimeError(f'{self.scan_title}: cannot determine number of '
+                           f'points for scans of type {self.spec_macro}')
 
     def get_dwell_time(self):
         if self.spec_macro == 'tseries':
-            return(float(self.spec_args[1]))
-        elif self.spec_macro == 'ascan':
-            return(float(self.spec_args[4]))
-        elif self.spec_macro == 'wbslew_scan':
-            return(float(self.spec_args[3]))
-        else:
-            raise(RuntimeError(f'{self.scan_title}: cannot determine dwell time for scans of type {self.spec_macro}'))
+            return float(self.spec_args[1])
+        if self.spec_macro == 'ascan':
+            return float(self.spec_args[4])
+        if self.spec_macro == 'wbslew_scan':
+            return float(self.spec_args[3])
+        raise RuntimeError(f'{self.scan_title}: cannot determine dwell time '
+                           f'for scans of type {self.spec_macro}')
 
     def get_detector_num_bins(self, detector_prefix):
-        with open(self.get_detector_file(detector_prefix)) as detector_file:
+        with open(self.get_detector_data_file(detector_prefix)) \
+             as detector_file:
             lines = detector_file.readlines()
         for line in lines:
             if line.startswith('#@CHANN'):
                 try:
-                    line_prefix, number_saved, first_saved, last_saved, reduction_coef = line.split()
-                    return(int(number_saved))
+                    line_prefix, number_saved, first_saved, last_saved, \
+                        reduction_coef = line.split()
+                    return int(number_saved)
                 except:
                     continue
-        raise(RuntimeError(f'{self.scan_title}: could not find num_bins for detector {detector_prefix}'))
-    
+        raise RuntimeError(f'{self.scan_title}: could not find num_bins for '
+                           f'detector {detector_prefix}')
+
     def get_detector_data_path(self):
-        return(self.scan_path)
+        return self.scan_path
 
-    def get_detector_file(self, detector_prefix, scan_step_index:int=0):
+    def get_detector_data_file(self, detector_prefix, scan_step_index=0):
         file_name = f'spec.log.scan{self.scan_number}.mca1.mca'
         file_name_full = os.path.join(self.detector_data_path, file_name)
         if os.path.isfile(file_name_full):
-            return(file_name_full)
-        else:
-            raise(RuntimeError(f'{self.scan_title}: could not find detector image file'))
+            return file_name_full
+        raise RuntimeError(
+            f'{self.scan_title}: could not find detector image file')
 
-    @cache
     def get_all_detector_data(self, detector_prefix):
-        # This should be easy with pyspec, but there are bugs in pyspec for MCA data.....
-        # or is the 'bug' from a nonstandard implementation of some macro on our end?
-        # According to spec manual and pyspec code, mca data should always begin w/ '@A'
+        # This should be easy with pyspec, but there are bugs in
+        # pyspec for MCA data.....  or is the 'bug' from a nonstandard
+        # implementation of some macro on our end?  According to spec
+        # manual and pyspec code, mca data should always begin w/ '@A'
         # In example scans, it begins with '@mca1' instead
         data = []
-        
-        with open(self.get_detector_file(detector_prefix)) as detector_file:
+
+        with open(self.get_detector_data_file(detector_prefix)) \
+                as detector_file:
             lines = [line.strip("\\\n") for line in detector_file.readlines()]
 
         num_bins = self.get_detector_num_bins(detector_prefix)
 
         counter = 0
         for line in lines:
             a = line.split()
 
             if len(a) > 0:
                 if a[0] == ("@"+detector_prefix):
                     counter = 1
                     spectrum = np.zeros(num_bins)
             if counter == 1:
                 b = np.array(a[1:]).astype('uint16')
-                spectrum[(counter-1)*25:((counter-1)*25+25)] = b
+                spectrum[(counter-1) * 25:((counter-1) * 25 + 25)] = b
                 counter = counter + 1
-            elif counter > 1 and counter <= (np.floor(num_bins/25.)):
+            elif counter > 1 and counter <= (np.floor(num_bins / 25.)):
                 b = np.array(a).astype('uint16')
-                spectrum[(counter-1)*25:((counter-1)*25+25)] = b
-                counter = counter+1
+                spectrum[(counter-1) * 25:((counter-1) * 25 + 25)] = b
+                counter = counter + 1
             elif counter == (np.ceil(num_bins/25.)):
                 b = np.array(a).astype('uint16')
-                spectrum[(counter-1)*25:((counter-1)*25+(np.mod(num_bins,25)))] = b
+                spectrum[(counter-1) * 25:
+                         ((counter-1) * 25 + (np.mod(num_bins, 25)))] = b
                 data.append(spectrum)
                 counter = 0
 
-        return(data)
+        return data
 
     def get_detector_data(self, detector_prefix, scan_step_index:int):
         detector_data = self.get_all_detector_data(detector_prefix)
-        return(detector_data[scan_step_index])
+        return detector_data[scan_step_index]
```

### Comparing `ChessAnalysisPipeline-0.0.5/CHAP/common/writer.py` & `ChessAnalysisPipeline-0.0.6/CHAP/common/writer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,96 +1,102 @@
 #!/usr/bin/env python
-'''
+"""
 File       : writer.py
 Author     : Valentin Kuznetsov <vkuznet AT gmail dot com>
 Description: Module for Writers used in multiple experiment-specific workflows.
-'''
+"""
 
 # system modules
-import argparse
-import json
-import logging
 import os
-import sys
 
 # local modules
 from CHAP import Writer
 
+
 class ExtractArchiveWriter(Writer):
+    """Writer for tar files from binary data"""
     def _write(self, data, filename):
-        '''Take a .tar archive represented as bytes in `data` and write the
-        extracted archive to files.
+        """Take a .tar archive represented as bytes in `data` and
+        write the extracted archive to files.
 
         :param data: the archive data
         :type data: bytes
-        :param filename: the name of a directory to which the archive files will
-            be written
+        :param filename: the name of a directory to which the archive
+            files will be written
         :type filename: str
         :return: the original `data`
         :rtype: bytes
-        '''
+        """
 
         from io import BytesIO
         import tarfile
 
-        tar = tarfile.open(fileobj=BytesIO(data))
-        tar.extractall(path=filename)
+        with tarfile.open(fileobj=BytesIO(data)) as tar:
+            tar.extractall(path=filename)
+
+        return data
 
-        return(data)
 
 class NexusWriter(Writer):
+    """Writer for NeXus files from `NXobject`-s"""
     def _write(self, data, filename, force_overwrite=False):
-        '''Write `data` to a NeXus file
+        """Write `data` to a NeXus file
 
         :param data: the data to write to `filename`.
         :type data: nexusformat.nexus.NXobject
         :param filename: name of the file to write to.
         :param force_overwrite: flag to allow data in `filename` to be
-            overwritten, if it already exists. 
+            overwritten, if it already exists.
         :return: the original input data
-        '''
+        """
 
         from nexusformat.nexus import NXobject
-        
+
         if not isinstance(data, NXobject):
-            raise(TypeError(f'Cannot write object of type {type(data).__name__} to a NeXus file.'))
+            raise TypeError('Cannot write object of type '
+                            f'{type(data).__name__} to a NeXus file.')
 
         mode = 'w' if force_overwrite else 'w-'
         data.save(filename, mode=mode)
 
-        return(data)
+        return data
+
 
 class YAMLWriter(Writer):
+    """Writer for YAML files from `dict`-s"""
     def _write(self, data, filename, force_overwrite=False):
-        '''If `data` is a `dict`, write it to `filename`.
+        """If `data` is a `dict`, write it to `filename`.
 
         :param data: the dictionary to write to `filename`.
         :type data: dict
         :param filename: name of the file to write to.
         :type filename: str
         :param force_overwrite: flag to allow data in `filename` to be
             overwritten if it already exists.
         :type force_overwrite: bool
         :raises TypeError: if `data` is not a `dict`
         :raises RuntimeError: if `filename` already exists and
             `force_overwrite` is `False`.
         :return: the original input data
         :rtype: dict
-        '''
+        """
 
         import yaml
 
         if not isinstance(data, (dict, list)):
-            raise(TypeError(f'{self.__name__}.write: input data must be a dict or list.'))
+            raise TypeError(
+                f'{self.__name__}.write: input data must be a dict or list.')
 
         if not force_overwrite:
             if os.path.isfile(filename):
-                raise(RuntimeError(f'{self.__name__}: {filename} already exists.'))
+                raise RuntimeError(
+                    f'{self.__name__}: {filename} already exists.')
 
         with open(filename, 'w') as outf:
             yaml.dump(data, outf, sort_keys=False)
 
-        return(data)
+        return data
+
 
 if __name__ == '__main__':
     from CHAP.writer import main
     main()
```

### Comparing `ChessAnalysisPipeline-0.0.5/CHAP/edd/models.py` & `ChessAnalysisPipeline-0.0.6/CHAP/edd/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,41 @@
+# third party modules
 import numpy as np
 from pathlib import PosixPath
 from pydantic import (BaseModel,
                       confloat,
                       conint,
                       conlist,
                       constr,
                       FilePath,
                       validator)
 from scipy.interpolate import interp1d
 from typing import Optional
 
 
 class MCACeriaCalibrationConfig(BaseModel):
-    '''Class representing metadata required to perform a Ceria calibration for an
+    """
+    Class representing metadata required to perform a Ceria calibration for an
     MCA detector.
 
     :ivar spec_file: Path to the SPEC file containing the CeO2 scan
     :ivar scan_number: Number of the CeO2 scan in `spec_file`
     :ivar scan_step_index: Index of the scan step to use for calibration,
-        optional. If not specified, the calibration routine will be performed on
-        the average of all MCA spectra for the scan.
+        optional. If not specified, the calibration routine will be performed
+        on the average of all MCA spectra for the scan.
 
     :ivar flux_file: csv file containing station beam energy in eV (column 0)
         and flux (column 1)
 
     :ivar detector_name: name of the MCA to calibrate
     :ivar num_bins: number of channels on the MCA to calibrate
     :ivar max_energy_kev: maximum channel energy of the MCA in keV
 
-    :ivar hexrd_h5_material_file: path to a HEXRD materials.h5 file containing an
-        entry for the material properties.
+    :ivar hexrd_h5_material_file: path to a HEXRD materials.h5 file containing
+        an entry for the material properties.
     :ivar hexrd_h5_material_name: Name of the material entry in
         `hexrd_h5_material_file`, defaults to `'CeO2'`.
     :ivar lattice_parameter_angstrom: lattice spacing in angstrom to use for
         the cubic CeO2 crystal, defaults to `5.41153`.
 
     :ivar tth_max: detector rotation about hutch x axis, defaults to `90`.
     :ivar hkl_tth_tol: minimum resolvable difference in 2&theta between two
@@ -55,30 +57,31 @@
         correction linear slope, defaults to `None`
     :ivar intercept_calibrated: calibrated value for detector channel energy
         correction y-intercept, defaluts to None
 
     :ivar max_iter: maximum number of iterations of the calibration routine,
         defaults to `10`.
     :ivar tune_tth_tol: stop iteratively tuning 2&theta when an iteration
-        produces a change in the tuned value of 2&theta that is smaller than this
-        value, defaults to `1e-8`.
-    '''
+        produces a change in the tuned value of 2&theta that is smaller than
+        this value, defaults to `1e-8`.
+    """
 
     spec_file: FilePath
     scan_number: conint(gt=0)
     scan_step_index: Optional[conint(ge=0)]
 
     flux_file: FilePath
 
     detector_name: constr(strip_whitespace=True, min_length=1)
     num_bins: conint(gt=0)
     max_energy_kev: confloat(gt=0)
 
     hexrd_h5_material_file: FilePath
-    hexrd_h5_material_name: constr(strip_whitespace=True, min_length=1) = 'CeO2'
+    hexrd_h5_material_name: constr(
+        strip_whitespace=True, min_length=1) = 'CeO2'
     lattice_parameter_angstrom: confloat(gt=0) = 5.41153
 
     tth_max: confloat(gt=0, allow_inf_nan=False) = 90.0
     hkl_tth_tol: confloat(gt=0, allow_inf_nan=False) = 0.15
 
     fit_include_bin_ranges: conlist(min_items=1,
                                     item_type=conlist(item_type=conint(ge=0),
@@ -94,122 +97,133 @@
     intercept_calibrated: Optional[confloat(allow_inf_nan=False)]
 
     max_iter: conint(gt=0) = 10
     tune_tth_tol: confloat(ge=0) = 1e-8
 
     @validator('fit_include_bin_ranges', each_item=True)
     def validate_include_bin_range(cls, value, values):
-        '''Ensure no bin ranges are outside the boundary of the detector'''
+        """Ensure no bin ranges are outside the boundary of the detector"""
 
         num_bins = values.get('num_bins')
         value[1] = min(value[1], num_bins)
-        return(value)
+        return value
 
     def mca_data(self):
-        '''Get the 1D array of MCA data to use for calibration.
-        
+        """Get the 1D array of MCA data to use for calibration.
+
         :return: MCA data
         :rtype: np.ndarray
-        '''
+        """
+        # local modules
+        from CHAP.common.utils.scanparsers \
+            import SMBMCAScanParser as ScanParser
 
-        from CHAP.common.utils.scanparsers import SMBMCAScanParser as ScanParser
         scanparser = ScanParser(self.spec_file, self.scan_number)
         if self.scan_step_index is None:
             data = scanparser.get_all_detector_data(self.detector_name)
             if scanparser.spec_scan_npts > 1:
                 data = np.average(data, axis=1)
             else:
                 data = data[0]
         else:
-            data = scanparser.get_detector_data(self.detector_name, self.scan_step_index)
+            data = scanparser.get_detector_data(
+                self.detector_name, self.scan_step_index)
 
-        return(np.array(data))
+        return np.array(data)
 
     def mca_mask(self):
-        '''Get a boolean mask array to use on MCA data before fitting.
+        """Get a boolean mask array to use on MCA data before fitting.
 
         :return: boolean mask array
         :rtype: numpy.ndarray
-        '''
+        """
 
         mask = np.asarray([False]*self.num_bins)
         bin_indices = np.arange(self.num_bins)
         for min_, max_ in self.fit_include_bin_ranges:
-            _mask =  np.logical_and(bin_indices > min_, bin_indices < max_)
+            _mask = np.logical_and(bin_indices > min_, bin_indices < max_)
             mask = np.logical_or(mask, _mask)
 
-        return(mask)
+        return mask
 
     def flux_correction_interpolation_function(self):
-        '''Get an interpolation function to correct MCA data for relative energy
+        """
+        Get an interpolation function to correct MCA data for relative energy
         flux of the incident beam.
 
         :return: energy flux correction interpolation function
         :rtype: scipy.interpolate._polyint._Interpolator1D
-        '''
+        """
 
         flux = np.loadtxt(self.flux_file)
         energies = flux[:,0]/1.e3
         relative_intensities = flux[:,1]/np.max(flux[:,1])
         interpolation_function = interp1d(energies, relative_intensities)
-        return(interpolation_function)
+        return interpolation_function
 
     def material(self):
-        '''Get CeO2 as a `CHAP.common.utils.material.Material` object.
+        """Get CeO2 as a `CHAP.common.utils.material.Material` object.
 
         :return: CeO2 material
         :rtype: CHAP.common.utils.material.Material
-        '''
-
+        """
+        # local modules
         from CHAP.common.utils.material import Material
-        material = Material(material_name=self.hexrd_h5_material_name,
-                            material_file=self.hexrd_h5_material_file,
-                            lattice_parameters_angstroms=self.lattice_parameter_angstrom)
+
+        material = Material(
+            material_name=self.hexrd_h5_material_name,
+            material_file=self.hexrd_h5_material_file,
+            lattice_parameters_angstroms=self.lattice_parameter_angstrom)
         # The following kwargs will be needed if we allow the material to be
         # built using xrayutilities (for now, we only allow hexrd to make the
         # material):
-                            # sgnum=225,
-                            # atoms=['Ce4p', 'O2mdot'],
-                            # pos=[(0.,0.,0.), (0.25,0.75,0.75)],
-                            # enrgy=50000.) # Why do we need to specify an energy to get HKLs when using xrayutilities?
-        return(material)
+        #   sgnum=225,
+        #   atoms=['Ce4p', 'O2mdot'],
+        #   pos=[(0.,0.,0.), (0.25,0.75,0.75)],
+        #   enrgy=50000.)
+        # Why do we need to specify an energy to get HKLs when using
+        # xrayutilities?
+        return material
 
     def unique_ds(self):
-        '''Get a list of unique HKLs and their lattice spacings
-        
+        """Get a list of unique HKLs and their lattice spacings
+
         :return: unique HKLs and their lattice spacings in angstroms
         :rtype: np.ndarray, np.ndarray
-        '''
-        
-        unique_hkls, unique_ds = self.material().get_unique_ds(tth_tol=self.hkl_tth_tol, tth_max=self.tth_max)
+        """
 
-        return(unique_hkls, unique_ds)
+        unique_hkls, unique_ds = self.material().get_ds_unique(
+            tth_tol=self.hkl_tth_tol, tth_max=self.tth_max)
+
+        return unique_hkls, unique_ds
 
     def fit_ds(self):
-        '''Get a list of HKLs and their lattice spacings that will be fit in the
+        """
+        Get a list of HKLs and their lattice spacings that will be fit in the
         calibration routine
-        
+
         :return: HKLs to fit and their lattice spacings in angstroms
         :rtype: np.ndarray, np.ndarray
-        '''
-        
+        """
+
         unique_hkls, unique_ds = self.unique_ds()
 
         fit_hkls = np.array([unique_hkls[i] for i in self.fit_hkls])
         fit_ds = np.array([unique_ds[i] for i in self.fit_hkls])
 
-        return(fit_hkls, fit_ds)
+        return fit_hkls, fit_ds
 
     def dict(self):
-        '''Return a representation of this configuration in a dictionary that is
+        """
+        Return a representation of this configuration in a dictionary that is
         suitable for dumping to a YAML file (one that converts all instances of
         fields with type `PosixPath` to `str`).
 
         :return: dictionary representation of the configuration.
         :rtype: dict
-        '''
+        """
 
         d = super().dict()
         for k,v in d.items():
             if isinstance(v, PosixPath):
                 d[k] = str(v)
-        return(d)
+        return d
```

### Comparing `ChessAnalysisPipeline-0.0.5/CHAP/edd/processor.py` & `ChessAnalysisPipeline-0.0.6/CHAP/edd/processor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,235 +1,250 @@
 #!/usr/bin/env python
 #-*- coding: utf-8 -*-
 #pylint: disable=
-'''
+"""
 File       : processor.py
 Author     : Valentin Kuznetsov <vkuznet AT gmail dot com>
 Description: Module for Processors used only by EDD experiments
-'''
+"""
 
 # system modules
-import json
+from json import dumps
+
+# third party modules
+import numpy as np
 
 # local modules
 from CHAP.processor import Processor
-from CHAP.common import StrainAnalysisProcessor
+
 
 class MCACeriaCalibrationProcessor(Processor):
-    '''A Processor using a CeO2 scan to obtain tuned values for the bragg
-    diffraction angle and linear correction parameters for MCA channel energies
-    for an EDD experimental setup.
-    '''
+    """A Processor using a CeO2 scan to obtain tuned values for the
+    bragg diffraction angle and linear correction parameters for MCA
+    channel energies for an EDD experimental setup.
+    """
 
     def _process(self, data):
-        '''Return tuned values for 2&theta and linear correction parameters for
-        the MCA channel energies.
+        """Return tuned values for 2&theta and linear correction
+        parameters for the MCA channel energies.
 
-        :param data: input configuration for the raw data & tuning procedure
+        :param data: input configuration for the raw data & tuning
+            procedure
         :type data: list[dict[str,object]]
-        :return: original configuration dictionary with tuned values added
+        :return: original configuration dictionary with tuned values
+            added
         :rtype: dict[str,float]
-        '''
+        """
 
         calibration_config = self.get_config(data)
 
         tth, slope, intercept = self.calibrate(calibration_config)
 
         calibration_config.tth_calibrated = tth
         calibration_config.slope_calibrated = slope
         calibration_config.intercept_calibrated = intercept
 
-        return(calibration_config.dict())
+        return calibration_config.dict()
 
     def get_config(self, data):
-        '''Get an instance of the configuration object needed by this
+        """Get an instance of the configuration object needed by this
         `Processor` from a returned value of `Reader.read`
 
-        :param data: Result of `Reader.read` where at least one item has the
-            value `'MCACeriaCalibrationConfig'` for the `'schema'` key.
+        :param data: Result of `Reader.read` where at least one item
+            has the value `'MCACeriaCalibrationConfig'` for the
+            `'schema'` key.
         :type data: list[dict[str,object]]
-        :raises Exception: If a valid config object cannot be constructed from
-            `data`.
-        :return: a valid instance of a configuration object with field values
-            taken from `data`.
+        :raises Exception: If a valid config object cannot be
+            constructed from `data`.
+        :return: a valid instance of a configuration object with field
+            values taken from `data`.
         :rtype: MCACeriaCalibrationConfig
-        '''
-
+        """
+        # local modules
         from CHAP.edd.models import MCACeriaCalibrationConfig
 
         calibration_config = False
         if isinstance(data, list):
             for item in data:
                 if isinstance(item, dict):
                     if item.get('schema') == 'MCACeriaCalibrationConfig':
                         calibration_config = item.get('data')
                         break
 
         if not calibration_config:
-            raise(ValueError('No MCA ceria calibration configuration found in input data'))
+            raise ValueError(
+                'No MCA ceria calibration configuration found in input data')
 
-        return(MCACeriaCalibrationConfig(**calibration_config))
+        return MCACeriaCalibrationConfig(**calibration_config)
 
     def calibrate(self, calibration_config):
-        '''Iteratively calibrate 2&theta by fitting selected peaks of an MCA
-        spectrum until the computed strain is sufficiently small. Use the fitted
-        peak locations to determine linear correction parameters for the MCA's
-        channel energies.
+        """Iteratively calibrate 2&theta by fitting selected peaks of
+        an MCA spectrum until the computed strain is sufficiently
+        small. Use the fitted peak locations to determine linear
+        correction parameters for the MCA's channel energies.
 
-        :param calibration_config: object configuring the CeO2 calibration
-            procedure
+        :param calibration_config: object configuring the CeO2
+            calibration procedure
         :type calibration_config: MCACeriaCalibrationConfig
-        :return: calibrated values of 2&theta and linear correction parameters
-            for MCA channel energies : tth, slope, intercept
+        :return: calibrated values of 2&theta and linear correction
+            parameters for MCA channel energies : tth, slope,
+            intercept
         :rtype: float, float, float
-        '''
+        """
+        # third party modules
+        from scipy.constants import physical_constants
 
+        # local modules
         from CHAP.common.utils.fit import Fit, FitMultipeak
-        import numpy as np
-        from scipy.constants import physical_constants
 
-        hc = (physical_constants['Planck constant in eV/Hz'][0]
-              * physical_constants['speed of light in vacuum'][0]
-              * 1e7) # We'll work in keV and A, not eV and m.
+        # We'll work in keV and A, not eV and m.
+        hc = 1e7 * physical_constants['Planck constant in eV/Hz'][0] \
+            * physical_constants['speed of light in vacuum'][0]
 
         # Collect raw MCA data of interest
         mca_data = calibration_config.mca_data()
-        mca_bin_energies = (np.arange(0, calibration_config.num_bins)
-                            * (calibration_config.max_energy_kev
-                               / calibration_config.num_bins))
+        mca_bin_energies = np.arange(0, calibration_config.num_bins) \
+            * (calibration_config.max_energy_kev/calibration_config.num_bins)
 
         # Mask out the corrected MCA data for fitting
         mca_mask = calibration_config.mca_mask()
         fit_mca_energies = mca_bin_energies[mca_mask]
         fit_mca_intensities = mca_data[mca_mask]
 
         # Correct raw MCA data for variable flux at different energies
-        flux_correct = calibration_config.flux_correction_interpolation_function()
+        flux_correct = \
+            calibration_config.flux_correction_interpolation_function()
         mca_intensity_weights = flux_correct(fit_mca_energies)
-        fit_mca_intensities = fit_mca_intensities / mca_intensity_weights
+        fit_mca_intensities = fit_mca_intensities/mca_intensity_weights
 
-        # Get the HKLs and lattice spacings that will be used for fitting
+        # Get the HKLs and lattice spacings that will be used for
+        # fitting
         tth = calibration_config.tth_initial_guess
         fit_hkls, fit_ds = calibration_config.fit_ds()
         c_1 = fit_hkls[:,0]**2 + fit_hkls[:,1]**2 + fit_hkls[:,2]**2
 
         for iter_i in range(calibration_config.max_iter):
 
-            ### Perform the uniform fit first ###
+            # Perform the uniform fit first
 
-            # Get expected peak energy locations for this iteration's starting
-            # value of tth
-            fit_lambda = 2.0 * fit_ds * np.sin(0.5*np.radians(tth))
+            # Get expected peak energy locations for this iteration's
+            # starting value of tth
+            fit_lambda = 2.0*fit_ds*np.sin(0.5*np.radians(tth))
             fit_E0 = hc / fit_lambda
 
             # Run the uniform fit
             best_fit, residual, best_values, best_errors, redchi, success = \
                 FitMultipeak.fit_multipeak(
                     fit_mca_intensities,
                     fit_E0,
                     x=fit_mca_energies,
                     fit_type='uniform',
                     plot=False)
 
-            # Extract values of interest from the best values for the uniform fit
-            # parameters
-            uniform_fit_centers = [best_values[f'peak{i+1}_center'] for i in range(len(calibration_config.fit_hkls))]
+            # Extract values of interest from the best values for the
+            # uniform fit parameters
+            uniform_fit_centers = [
+                best_values[f'peak{i+1}_center']
+                for i in range(len(calibration_config.fit_hkls))]
             # uniform_a = best_values['scale_factor']
             # uniform_strain = np.log(
-            #     (uniform_a 
+            #     (uniform_a
             #      / calibration_config.lattice_parameter_angstrom))
             # uniform_tth = tth * (1.0 + uniform_strain)
             # uniform_rel_rms_error = (np.linalg.norm(residual)
             #                          / np.linalg.norm(fit_mca_intensities))
 
-            ### Next, perform the unconstrained fit ###
+            # Next, perform the unconstrained fit
 
-            # Use the peak locations found in the uniform fit as the initial
-            # guesses for peak locations in the unconstrained fit
+            # Use the peak locations found in the uniform fit as the
+            # initial guesses for peak locations in the unconstrained
+            # fit
             best_fit, residual, best_values, best_errors, redchi, success = \
                 FitMultipeak.fit_multipeak(
                     fit_mca_intensities,
                     uniform_fit_centers,
                     x=fit_mca_energies,
                     fit_type='unconstrained',
                     plot=False)
 
             # Extract values of interest from the best values for the
             # unconstrained fit parameters
             unconstrained_fit_centers = np.array(
-                [best_values[f'peak{i+1}_center'] for i in range(len(calibration_config.fit_hkls))])
-            unconstrained_a = (0.5 * hc * np.sqrt(c_1)
-                               / (unconstrained_fit_centers
-                                  * abs(np.sin(0.5*np.radians(tth)))))
+                [best_values[f'peak{i+1}_center']
+                 for i in range(len(calibration_config.fit_hkls))])
+            unconstrained_a = 0.5*hc*np.sqrt(c_1) \
+                / (unconstrained_fit_centers*abs(np.sin(0.5*np.radians(tth))))
             unconstrained_strains = np.log(
-                (unconstrained_a
-                 / calibration_config.lattice_parameter_angstrom))
+                unconstrained_a/calibration_config.lattice_parameter_angstrom)
             unconstrained_strain = np.mean(unconstrained_strains)
-            unconstrained_tth = tth * (1.0 + unconstrained_strain)
-            unconstrained_rel_rms_error = (np.linalg.norm(residual)
-                                           / np.linalg.norm(fit_mca_intensities))
-
+            unconstrained_tth = tth * (1.0+unconstrained_strain)
+            unconstrained_rel_rms_error = (
+                np.linalg.norm(residual)/np.linalg.norm(fit_mca_intensities))
 
             # Update tth for the next iteration of tuning
             prev_tth = tth
             tth = unconstrained_tth
 
-            # Stop tuning tth at this iteration if differences are small enough
+            # Stop tuning tth at this iteration if differences are
+            # small enough
             if abs(tth - prev_tth) < calibration_config.tune_tth_tol:
                 break
 
         # Fit line to expected / computed peak locations from the last
         # unconstrained fit.
         fit = Fit.fit_data(
             fit_E0,
             'linear',
             x=unconstrained_fit_centers,
             nan_policy='omit')
         slope = fit.best_values['slope']
         intercept = fit.best_values['intercept']
 
-        return(float(tth), float(slope), float(intercept))
+        return float(tth), float(slope), float(intercept)
+
 
 class MCADataProcessor(Processor):
-    '''A Processor to return data from an MCA, restuctured to incorporate the
-    shape & metadata associated with a map configuration to which the MCA data
-    belongs, and linearly transformed according to the results of a ceria
-    calibration.
-    '''
+    """A Processor to return data from an MCA, restuctured to
+    incorporate the shape & metadata associated with a map
+    configuration to which the MCA data belongs, and linearly
+    transformed according to the results of a ceria calibration.
+    """
 
     def _process(self, data):
-        '''Process configurations for a map and MCA detector(s), and return the
-        calibrated MCA data collected over the map.
+        """Process configurations for a map and MCA detector(s), and
+        return the calibrated MCA data collected over the map.
 
-        :param data: input map configuration and results of ceria calibration
+        :param data: input map configuration and results of ceria
+            calibration
         :type data: list[dict[str,object]]
         :return: calibrated and flux-corrected MCA data
         :rtype: nexusformat.nexus.NXentry
-        '''
+        """
 
         map_config, calibration_config = self.get_configs(data)
         nxroot = self.get_nxroot(map_config, calibration_config)
 
-        return(nxroot)
+        return nxroot
 
     def get_configs(self, data):
-        '''Get instances of the configuration objects needed by this
+        """Get instances of the configuration objects needed by this
         `Processor` from a returned value of `Reader.read`
 
-        :param data: Result of `Reader.read` where at least one item has the
-            value `'MapConfig'` for the `'schema'` key, and at least one item has
-            the value `'MCACeriaCalibrationConfig'` for the `'schema'` key.
+        :param data: Result of `Reader.read` where at least one item
+            has the value `'MapConfig'` for the `'schema'` key, and at
+            least one item has the value `'MCACeriaCalibrationConfig'`
+            for the `'schema'` key.
         :type data: list[dict[str,object]]
-        :raises Exception: If valid config objects cannot be constructed from
-            `data`.
-        :return: valid instances of the configuration objects with field values
-            taken from `data`.
+        :raises Exception: If valid config objects cannot be
+            constructed from `data`.
+        :return: valid instances of the configuration objects with
+            field values taken from `data`.
         :rtype: tuple[MapConfig, MCACeriaCalibrationConfig]
-        '''
-
+        """
+        # local modules
         from CHAP.common.models.map import MapConfig
         from CHAP.edd.models import MCACeriaCalibrationConfig
 
         map_config = False
         calibration_config = False
         if isinstance(data, list):
             for item in data:
@@ -237,61 +252,63 @@
                     schema = item.get('schema')
                     if schema == 'MapConfig':
                         map_config = item.get('data')
                     elif schema == 'MCACeriaCalibrationConfig':
                         calibration_config = item.get('data')
 
         if not map_config:
-            raise(ValueError('No map configuration found in input data'))
+            raise ValueError('No map configuration found in input data')
         if not calibration_config:
-            raise(ValueError('No MCA ceria calibration configuration found in input data'))
+            raise ValueError('No MCA ceria calibration configuration found in '
+                             'input data')
 
-        return(MapConfig(**map_config), MCACeriaCalibrationConfig(**calibration_config))
+        return (MapConfig(**map_config),
+                MCACeriaCalibrationConfig(**calibration_config))
 
     def get_nxroot(self, map_config, calibration_config):
-        '''Get a map of the MCA data collected by the scans in `map_config`. The
-        MCA data will be calibrated and flux-corrected according to the
-        parameters included in `calibration_config`. The data will be returned
-        along with relevant metadata in the form of a NeXus structure.
+        """Get a map of the MCA data collected by the scans in
+        `map_config`. The MCA data will be calibrated and
+        flux-corrected according to the parameters included in
+        `calibration_config`. The data will be returned along with
+        relevant metadata in the form of a NeXus structure.
 
         :param map_config: the map configuration
         :type map_config: MapConfig
         :param calibration_config: the calibration configuration
         :type calibration_config: MCACeriaCalibrationConfig
         :return: a map of the calibrated and flux-corrected MCA data
         :rtype: nexusformat.nexus.NXroot
-        '''
-
-        from CHAP.common import MapProcessor
-
+        """
+        # third party modules
         from nexusformat.nexus import (NXdata,
                                        NXdetector,
-                                       NXentry,
                                        NXinstrument,
                                        NXroot)
-        import numpy as np
+
+        # local modules
+        from CHAP.common import MapProcessor
 
         nxroot = NXroot()
 
         nxroot[map_config.title] = MapProcessor.get_nxentry(map_config)
         nxentry = nxroot[map_config.title]
 
         nxentry.instrument = NXinstrument()
         nxentry.instrument.detector = NXdetector()
-        nxentry.instrument.detector.calibration_configuration = json.dumps(calibration_config.dict())
+        nxentry.instrument.detector.calibration_configuration = dumps(
+            calibration_config.dict())
 
         nxentry.instrument.detector.data = NXdata()
         nxdata = nxentry.instrument.detector.data
         nxdata.raw = np.empty((*map_config.shape, calibration_config.num_bins))
         nxdata.raw.attrs['units'] = 'counts'
-        nxdata.channel_energy = (calibration_config.slope_calibrated
-                                * np.arange(0, calibration_config.num_bins)
-                                * (calibration_config.max_energy_kev
-                                   / calibration_config.num_bins)
-                                + calibration_config.intercept_calibrated)
+        nxdata.channel_energy = calibration_config.slope_calibrated \
+            * np.arange(0, calibration_config.num_bins) \
+            * (calibration_config.max_energy_kev/calibration_config.num_bins) \
+            + calibration_config.intercept_calibrated
         nxdata.channel_energy.attrs['units'] = 'keV'
 
         for scans in map_config.spec_scans:
             for scan_number in scans.scan_numbers:
                 scanparser = scans.get_scanparser(scan_number)
                 for scan_step_index in range(scanparser.spec_scan_npts):
                     map_index = scans.get_index(
@@ -309,15 +326,19 @@
             nxdata.channel_energy,
             name=f'{calibration_config.detector_name}_channel_energy')
         if isinstance(nxentry.data.attrs['axes'], str):
             nxentry.data.attrs['axes'] = [
                 nxentry.data.attrs['axes'],
                 f'{calibration_config.detector_name}_channel_energy']
         else:
-            nxentry.data.attrs['axes'] += [f'{calibration_config.detector_name}_channel_energy']
+            nxentry.data.attrs['axes'] += [
+                f'{calibration_config.detector_name}_channel_energy']
         nxentry.data.attrs['signal'] = calibration_config.detector_name
 
-        return(nxroot)
+        return nxroot
+
 
 if __name__ == '__main__':
+    # local modules
     from CHAP.processor import main
+
     main()
```

### Comparing `ChessAnalysisPipeline-0.0.5/CHAP/inference/processor.py` & `ChessAnalysisPipeline-0.0.6/CHAP/inference/processor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,68 +1,75 @@
-#!/usr/bin/env python                                                                                                       
-#-*- coding: utf-8 -*-                                                                                                      
-#pylint: disable=                                                                                                           
-'''                                                                                                                         
-File       : processor.py                                                                                                   
-Author     : Valentin Kuznetsov <vkuznet AT gmail dot com>                                                                  
-Description: Processor module                                                                                               
-'''
+#!/usr/bin/env python
+#-*- coding: utf-8 -*-
+#pylint: disable=
+"""
+File       : processor.py
+Author     : Valentin Kuznetsov <vkuznet AT gmail dot com>
+Description: Processor module
+"""
 
 # system modules
 from time import time
 
 # local modules
 from CHAP import Processor
 
+
 class TFaaSImageProcessor(Processor):
-    '''
-    A Processor to get predictions from TFaaS inference server.
-    '''
+    """A Processor to get predictions from TFaaS inference server."""
+
     def process(self, data, url, model, verbose=False):
-        '''
-        process data API
-        '''
+        """process data API"""
 
         t0 = time()
         self.logger.info(f'Executing "process" with url {url} model {model}')
 
         data = self._process(data, url, model, verbose)
 
         self.logger.info(f'Finished "process" in {time()-t0:.3f} seconds\n')
 
-        return(data)
+        return data
 
     def _process(self, data, url, model, verbose):
-        '''Print and return the input data.
+        """Print and return the input data.
 
-        :param data: Input image data, either file name or actual image data
+        :param data: Input image data, either file name or actual
+            image data
         :type data: object
         :return: `data`
         :rtype: object
-        '''
+        """
+        # system modules
+        from pathlib import Path
 
+        # local modules
         from MLaaS.tfaas_client import predictImage
-        from pathlib import Path
 
         self.logger.info(f'input data {type(data)}')
         if isinstance(data, str) and Path(data).is_file():
-            imgFile = data
-            data = predictImage(url, imgFile, model, verbose)
+            img_file = data
+            data = predictImage(url, img_file, model, verbose)
         else:
+            # third party modules
+            from requests import Session
+
             rdict = data[0]
-            import requests
             img = rdict['data']
-            session = requests.Session()
+            session = Session()
             rurl = url + '/predict/image'
-            payload = dict(model=model)
-            files = dict(image=img)
-            self.logger.info(f'HTTP request {rurl} with image file and {payload} payload')
-            req = session.post(rurl, files=files, data=payload )
+            payload = {'model': model}
+            files = {'image': img}
+            self.logger.info(
+                f'HTTP request {rurl} with image file and {payload} payload')
+            req = session.post(rurl, files=files, data=payload)
             data = req.content
             data = data.decode('utf-8').replace('\n', '')
             self.logger.info(f'HTTP response {data}')
 
-        return(data)
+        return data
+
 
 if __name__ == '__main__':
+    # local modules
     from CHAP.processor import main
+
     main()
```

### Comparing `ChessAnalysisPipeline-0.0.5/CHAP/pipeline.py` & `ChessAnalysisPipeline-0.0.6/CHAP/pipeline.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,42 @@
 #!/usr/bin/env python
 #-*- coding: utf-8 -*-
 #pylint: disable=
 """
 File       : pipeline.py
 Author     : Valentin Kuznetsov <vkuznet AT gmail dot com>
-Description: 
+Description:
 """
 
 # system modules
 import logging
 from time import time
 
+
 class Pipeline():
-    """
-    Pipeline represent generic Pipeline class
-    """
+    """Pipeline represent generic Pipeline class"""
     def __init__(self, items=None, kwds=None):
-        """
-        Pipeline class constructor
-        
+        """Pipeline class constructor
+
         :param items: list of objects
         :param kwds: list of method args for individual objects
         """
         self.__name__ = self.__class__.__name__
 
         self.items = items
         self.kwds = kwds
 
         self.logger = logging.getLogger(self.__name__)
         self.logger.propagate = False
 
     def execute(self):
-        """
-        execute API
-        """
+        """execute API"""
 
         t0 = time()
-        self.logger.info(f'Executing "execute"\n')
+        self.logger.info('Executing "execute"\n')
 
         data = None
         for item, kwargs in zip(self.items, self.kwds):
             if hasattr(item, 'read'):
                 self.logger.info(f'Calling "read" on {item}')
                 data = item.read(**kwargs)
             if hasattr(item, 'process'):
@@ -48,37 +44,27 @@
                 data = item.process(data, **kwargs)
             if hasattr(item, 'write'):
                 self.logger.info(f'Calling "write" on {item}')
                 data = item.write(data, **kwargs)
 
         self.logger.info(f'Executed "execute" in {time()-t0:.3f} seconds')
 
+
 class PipelineObject():
-    """
-    PipelineObject represent generic Pipeline class
-    """
-    def __init__(self, reader, writer, processor, fitter):
-        """
-        PipelineObject class constructor
-        """
+    """PipelineObject represent generic Pipeline class"""
+    def __init__(self, reader, writer, processor):
+        """PipelineObject class constructor"""
         self.reader = reader
         self.writer = writer
         self.processor = processor
 
     def read(self, filename):
-        """
-        read object API
-        """
+        """read object API"""
         return self.reader.read(filename)
 
     def write(self, data, filename):
-        """
-        write object API
-        """
+        """write object API"""
         return self.writer.write(data, filename)
 
     def process(self, data):
-        """
-        process object API
-        """
+        """process object API"""
         return self.processor.process(data)
-
```

### Comparing `ChessAnalysisPipeline-0.0.5/CHAP/processor.py` & `ChessAnalysisPipeline-0.0.6/CHAP/processor.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,137 +5,106 @@
 File       : processor.py
 Author     : Valentin Kuznetsov <vkuznet AT gmail dot com>
 Description: Processor module
 """
 
 # system modules
 import argparse
-import json
+from inspect import getfullargspec
 import logging
-import sys
+from sys import modules
 from time import time
 
-# local modules
-# from pipeline import PipelineObject
 
 class Processor():
-    """
-    Processor represent generic processor
-    """
+    """Processor represent generic processor"""
     def __init__(self):
-        """
-        Processor constructor
-        """
+        """Processor constructor"""
         self.__name__ = self.__class__.__name__
         self.logger = logging.getLogger(self.__name__)
         self.logger.propagate = False
 
-    def process(self, data):
-        """
-        process data API
+    def process(self, data, **_process_kwargs):
+        """process data API
+
+        :param _process_kwargs: keyword arguments to pass to
+            `self._process`, defaults to `{}`
+        :type _process_kwargs: dict, optional
         """
 
         t0 = time()
         self.logger.info(f'Executing "process" with type(data)={type(data)}')
 
-        data = self._process(data)
+        _valid_process_args = {}
+        allowed_args = getfullargspec(self._process).args \
+            + getfullargspec(self._process).kwonlyargs
+        for k, v in _process_kwargs.items():
+            if k in allowed_args:
+                _valid_process_args[k] = v
+            else:
+                self.logger.warning(f'Ignoring invalid arg to _process: {k}')
+
+        data = self._process(data, **_valid_process_args)
 
         self.logger.info(f'Finished "process" in {time()-t0:.3f} seconds\n')
 
-        return(data)
+        return data
 
     def _process(self, data):
+        """Private method to carry out the mechanics of the specific
+        Processor.
+
+        :param data: input data
+        :return: processed data
+        """
         # If needed, extract data from a returned value of Reader.read
         if isinstance(data, list):
-            if all([isinstance(d,dict) for d in data]):
+            if all(isinstance(d, dict) for d in data):
                 data = data[0]['data']
+        if data is None:
+            return []
         # process operation is a simple print function
         data += "process part\n"
         # and we return data back to pipeline
         return data
 
 
-class TFaaSImageProcessor(Processor):
-    '''
-    A Processor to get predictions from TFaaS inference server.
-    '''
-    def process(self, data, url, model, verbose=False):
-        """
-        process data API
-        """
-
-        t0 = time()
-        self.logger.info(f'Executing "process" with url {url} model {model}')
-
-        data = self._process(data, url, model, verbose)
-
-        self.logger.info(f'Finished "process" in {time()-t0:.3f} seconds\n')
-
-        return(data)
-
-    def _process(self, data, url, model, verbose):
-        '''Print and return the input data.
-
-        :param data: Input image data, either file name or actual image data
-        :type data: object
-        :return: `data`
-        :rtype: object
-        '''
-        from MLaaS.tfaas_client import predictImage
-        from pathlib import Path
-        self.logger.info(f"input data {type(data)}")
-        if isinstance(data, str) and Path(data).is_file():
-            imgFile = data
-            data = predictImage(url, imgFile, model, verbose)
-        else:
-            rdict = data[0]
-            import requests
-            img = rdict['data']
-            session = requests.Session()
-            rurl = url + '/predict/image'
-            payload = dict(model=model)
-            files = dict(image=img)
-            self.logger.info(f"HTTP request {rurl} with image file and {payload} payload")
-            req = session.post(rurl, files=files, data=payload )
-            data = req.content
-            data = data.decode("utf-8").replace('\n', '')
-            self.logger.info(f"HTTP response {data}")
-
-        return(data)
-
 class OptionParser():
-    '''User based option parser'''
+    """User based option parser"""
     def __init__(self):
         self.parser = argparse.ArgumentParser(prog='PROG')
         self.parser.add_argument(
             '--data', action='store',
             dest='data', default='', help='Input data')
         self.parser.add_argument(
             '--processor', action='store',
             dest='processor', default='Processor', help='Processor class name')
         self.parser.add_argument(
             '--log-level', choices=logging._nameToLevel.keys(),
             dest='log_level', default='INFO', help='logging level')
 
+
 def main(opt_parser=OptionParser):
-    '''Main function'''
+    """Main function"""
 
-    optmgr  = opt_parser()
+    optmgr = opt_parser()
     opts = optmgr.parser.parse_args()
-    clsName = opts.processor
+    cls_name = opts.processor
     try:
-        processorCls = getattr(sys.modules[__name__],clsName)
-    except:
-        print(f'Unsupported processor {clsName}')
-        sys.exit(1)
+        processor_cls = getattr(modules[__name__], cls_name)
+    except AttributeError:
+        print(f'Unsupported processor {cls_name}')
+        raise
 
-    processor = processorCls()
+    processor = processor_cls()
     processor.logger.setLevel(getattr(logging, opts.log_level))
     log_handler = logging.StreamHandler()
-    log_handler.setFormatter(logging.Formatter('{name:20}: {message}', style='{'))
+    log_handler.setFormatter(logging.Formatter(
+        '{name:20}: {message}', style='{'))
     processor.logger.addHandler(log_handler)
     data = processor.process(opts.data)
 
-    print(f"Processor {processor} operates on data {data}")
+    print(f'Processor {processor} operates on data {data}')
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `ChessAnalysisPipeline-0.0.5/CHAP/reader.py` & `ChessAnalysisPipeline-0.0.6/CHAP/reader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,114 +1,123 @@
 #!/usr/bin/env python
-'''
+"""
 File       : reader.py
 Author     : Valentin Kuznetsov <vkuznet AT gmail dot com>
 Description: generic Reader module
-'''
+"""
 
 # system modules
 import argparse
-import json
+from inspect import getfullargspec
 import logging
-import sys
+from sys import modules
 from time import time
 
-# local modules
-# from pipeline import PipelineObject
 
 class Reader():
-    '''
-    Reader represent generic file writer
-    '''
+    """Reader represent generic file writer"""
 
     def __init__(self):
-        '''
-        Constructor of Reader class
-        '''
+        """Constructor of Reader class"""
         self.__name__ = self.__class__.__name__
         self.logger = logging.getLogger(self.__name__)
         self.logger.propagate = False
 
     def read(self, type_=None, schema=None, encoding=None, **_read_kwargs):
-        '''Read API
+        """Read API
 
         Wrapper to read, format, and return the data requested.
 
-        :param type_: the expected type of data read from `filename`, defualts
-            to `None`
+        :param type_: the expected type of data read from `filename`,
+            defualts to `None`
         :type type_: type, optional
-        :param schema: the expected schema of the data read from `filename`,
-            defaults to `None`
+        :param schema: the expected schema of the data read from
+            `filename`, defaults to `None`
         :type schema: str, otional
-        :param _read_kwargs: keyword arguments to pass to `self._read`, defaults
-            to `{}`
+        :param _read_kwargs: keyword arguments to pass to
+            `self._read`, defaults to `{}`
         :type _read_kwargs: dict, optional
-        :return: list with one item: a dictionary containing the data read from
-            `filename`, the name of this `Reader`, and the values of `type_` and
-            `schema`.
+        :return: list with one item: a dictionary containing the data
+            read from `filename`, the name of this `Reader`, and the
+            values of `type_` and `schema`.
         :rtype: list[dict[str,object]]
-        '''
+        """
 
         t0 = time()
-        self.logger.info(f'Executing "read" with type={type_}, schema={schema}, kwargs={_read_kwargs}')
+        self.logger.info(f'Executing "read" with type={type_}, '
+                         f'schema={schema}, kwargs={_read_kwargs}')
+
+        _valid_read_args = {}
+        allowed_args = getfullargspec(self._read).args \
+            + getfullargspec(self._read).kwonlyargs
+        for k, v in _read_kwargs.items():
+            if k in allowed_args:
+                _valid_read_args[k] = v
+            else:
+                self.logger.warning(f'Ignoring invalid arg to _read: {k}')
 
         data = [{'name': self.__name__,
-                 'data': self._read(**_read_kwargs),
+                 'data': self._read(**_valid_read_args),
                  'type': type_,
                  'schema': schema,
                  'encoding': encoding}]
 
         self.logger.info(f'Finished "read" in {time()-t0:.3f} seconds\n')
-        return(data)
+        return data
 
     def _read(self, filename):
-        '''Read and return the data from requested from `filename`
+        """Read and return the data from requested from `filename`
 
         :param filename: Name of file to read from
         :return: specific number of bytes from a file
-        '''
+        """
 
         if not filename:
-            self.logger.warning('No file name is given, will skip read operation')
+            self.logger.warning(
+                'No file name is given, will skip read operation')
             return None
 
         with open(filename) as file:
             data = file.read()
-        return(data)
+        return data
+
 
 class OptionParser():
-    '''User based option parser'''
+    """User based option parser"""
     def __init__(self):
         self.parser = argparse.ArgumentParser(prog='PROG')
         self.parser.add_argument(
             '--filename', action='store',
             dest='filename', default='', help='Input file')
         self.parser.add_argument(
             '--reader', action='store',
             dest='reader', default='Reader', help='Reader class name')
         self.parser.add_argument(
             '--log-level', choices=logging._nameToLevel.keys(),
             dest='log_level', default='INFO', help='logging level')
 
+
 def main(opt_parser=OptionParser):
-    '''Main function'''
+    """Main function"""
 
-    optmgr  = opt_parser()
+    optmgr = opt_parser()
     opts = optmgr.parser.parse_args()
-    clsName = opts.reader
+    cls_name = opts.reader
     try:
-        readerCls = getattr(sys.modules[__name__],clsName)
-    except:
-        print(f'Unsupported reader {clsName}')
-        sys.exit(1)
+        reader_cls = getattr(modules[__name__], cls_name)
+    except AttributeError:
+        print(f'Unsupported reader {cls_name}')
+        raise
 
-    reader = readerCls()
+    reader = reader_cls()
     reader.logger.setLevel(getattr(logging, opts.log_level))
     log_handler = logging.StreamHandler()
-    log_handler.setFormatter(logging.Formatter('{name:20}: {message}', style='{'))
+    log_handler.setFormatter(logging.Formatter(
+        '{name:20}: {message}', style='{'))
     reader.logger.addHandler(log_handler)
     data = reader.read(filename=opts.filename)
 
     print(f'Reader {reader} reads from {opts.filename}, data {data}')
 
+
 if __name__ == '__main__':
     main()
```

### Comparing `ChessAnalysisPipeline-0.0.5/CHAP/tomo/models.py` & `ChessAnalysisPipeline-0.0.6/CHAP/tomo/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,77 +1,91 @@
-# system modules
+"""Tomography Pydantic model classes"""
 
-# third party imports
+# Third party imports
+from typing import (
+    Literal,
+    Optional,
+)
 from pydantic import (
-        BaseModel,
-        StrictBool,
-        conint,
-        conlist,
-        confloat,
-        constr,
+    BaseModel,
+    StrictBool,
+    conint,
+    conlist,
+    confloat,
+    constr,
 )
-from typing import Literal, Optional
 
 
 class Detector(BaseModel):
     """
     Detector class to represent the detector used in the experiment.
-    
+
     :ivar prefix: Prefix of the detector in the SPEC file.
     :type prefix: str
     :ivar rows: Number of pixel rows on the detector
     :type rows: int
     :ivar columns: Number of pixel columns on the detector
     :type columns: int
     :ivar pixel_size: Pixel size of the detector in mm
     :type pixel_size: int or list[int]
     :ivar lens_magnification: Lens magnification for the detector
-    :type lens_magnification: float, optional
+    :type lens_magnification: float, optional [1.0]
     """
     prefix: constr(strip_whitespace=True, min_length=1)
     rows: conint(gt=0)
     columns: conint(gt=0)
-    pixel_size: conlist(item_type=confloat(gt=0, allow_inf_nan=False), min_items=1, max_items=2)
+    pixel_size: conlist(
+        item_type=confloat(gt=0, allow_inf_nan=False),
+        min_items=1, max_items=2)
     lens_magnification: confloat(gt=0, allow_inf_nan=False) = 1.0
 
 
 class TomoSetupConfig(BaseModel):
     """
-    Class representing the configuration for the tomography reconstruction setup.
+    Class representing the configuration for the tomography
+    reconstruction setup.
 
     :ivar detectors: Detector used in the tomography experiment
     :type detectors: Detector
+    :ivar include_raw_data: Flag to designate whether raw data will be
+        included (True) or not (False)
+    :type include_raw_data: bool, optional [False]
     """
     detector: Detector.construct()
     include_raw_data: Optional[StrictBool] = False
 
 
 class TomoReduceConfig(BaseModel):
     """
-    Class representing the configuration for tomography image reductions.
+    Class representing the configuration for tomography image
+    reductions.
 
-    :ivar tool_type: Type of tomography reconstruction tool; always set to "reduce_data"
+    :ivar tool_type: Type of tomography reconstruction tool; always set
+        to "reduce_data"
     :type tool_type: str, optional
     :ivar detectors: Detector used in the tomography experiment
     :type detectors: Detector
     :ivar img_x_bounds: Detector image bounds in the x-direction
     :type img_x_bounds: list[int], optional
     """
     tool_type: Literal['reduce_data'] = 'reduce_data'
     detector: Detector = Detector.construct()
-    img_x_bounds: Optional[conlist(item_type=conint(ge=0), min_items=2, max_items=2)]
+    img_x_bounds: Optional[
+        conlist(item_type=conint(ge=0), min_items=2, max_items=2)]
 
 
 class TomoFindCenterConfig(BaseModel):
     """
     Class representing the configuration for tomography find center axis.
 
-    :ivar tool_type: Type of tomography reconstruction tool; always set to "find_center"
+    :ivar tool_type: Type of tomography reconstruction tool; always set
+        to "find_center"
     :type tool_type: str, optional
-    :ivar center_stack_index: Stack index of tomography set to find center axis (offset 1)
+    :ivar center_stack_index: Stack index of tomography set to find
+        center axis (offset 1)
     :type center_stack_index: int, optional
     :ivar lower_row: Lower row index for center finding
     :type lower_row: int, optional
     :ivar lower_center_offset: Center at lower row index
     :type lower_center_offset: float, optional
     :ivar upper_row: Upper row index for center finding
     :type upper_row: int, optional
@@ -84,42 +98,50 @@
     lower_center_offset: Optional[confloat(allow_inf_nan=False)]
     upper_row: Optional[conint(ge=-1)]
     upper_center_offset: Optional[confloat(allow_inf_nan=False)]
 
 
 class TomoReconstructConfig(BaseModel):
     """
-    Class representing the configuration for tomography image reconstruction.
+    Class representing the configuration for tomography image
+    reconstruction.
 
-    :ivar tool_type: Type of tomography reconstruction tool; always set to "reconstruct_data"
+    :ivar tool_type: Type of tomography reconstruction tool; always set
+        to "reconstruct_data"
     :type tool_type: str, optional
     :ivar x_bounds: Reconstructed image bounds in the x-direction
     :type x_bounds: list[int], optional
     :ivar y_bounds: Reconstructed image bounds in the y-direction
     :type y_bounds: list[int], optional
     :ivar z_bounds: Reconstructed image bounds in the z-direction
     :type z_bounds: list[int], optional
     """
     tool_type: Literal['reconstruct_data'] = 'reconstruct_data'
-    x_bounds: Optional[conlist(item_type=conint(ge=-1), min_items=2, max_items=2)]
-    y_bounds: Optional[conlist(item_type=conint(ge=-1), min_items=2, max_items=2)]
-    z_bounds: Optional[conlist(item_type=conint(ge=-1), min_items=2, max_items=2)]
+    x_bounds: Optional[
+        conlist(item_type=conint(ge=-1), min_items=2, max_items=2)]
+    y_bounds: Optional[
+        conlist(item_type=conint(ge=-1), min_items=2, max_items=2)]
+    z_bounds: Optional[
+        conlist(item_type=conint(ge=-1), min_items=2, max_items=2)]
 
 
 class TomoCombineConfig(BaseModel):
     """
     Class representing the configuration for combined tomography stacks.
 
-    :ivar tool_type: Type of tomography reconstruction tool; always set to "combine_data"
+    :ivar tool_type: Type of tomography reconstruction tool; always set
+        to "combine_data"
     :type tool_type: str, optional
-    :ivar x_bounds: Reconstructed image bounds in the x-direction
+    :ivar x_bounds: Combined image bounds in the x-direction
     :type x_bounds: list[int], optional
-    :ivar y_bounds: Reconstructed image bounds in the y-direction
+    :ivar y_bounds: Combined image bounds in the y-direction
     :type y_bounds: list[int], optional
-    :ivar z_bounds: Reconstructed image bounds in the z-direction
+    :ivar z_bounds: Combined image bounds in the z-direction
     :type z_bounds: list[int], optional
     """
     tool_type: Literal['combine_data'] = 'combine_data'
-    x_bounds: Optional[conlist(item_type=conint(ge=-1), min_items=2, max_items=2)]
-    y_bounds: Optional[conlist(item_type=conint(ge=-1), min_items=2, max_items=2)]
-    z_bounds: Optional[conlist(item_type=conint(ge=-1), min_items=2, max_items=2)]
-
+    x_bounds: Optional[
+        conlist(item_type=conint(ge=-1), min_items=2, max_items=2)]
+    y_bounds: Optional[
+        conlist(item_type=conint(ge=-1), min_items=2, max_items=2)]
+    z_bounds: Optional[
+        conlist(item_type=conint(ge=-1), min_items=2, max_items=2)]
```

### Comparing `ChessAnalysisPipeline-0.0.5/CHAP/tomo/processor.py` & `ChessAnalysisPipeline-0.0.6/CHAP/tomo/processor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,173 +1,289 @@
 #!/usr/bin/env python
 #-*- coding: utf-8 -*-
 #pylint: disable=
-'''
+"""
 File       : processor.py
 Author     : Rolf Verberg <rolfverberg AT gmail dot com>
 Description: Module for Processors used only by tomography experiments
-'''
+"""
 
-# system modules
+# System modules
 from os import mkdir
 from os import path as os_path
+from sys import exit as sys_exit
 from time import time
 
-# third party modules
-from nexusformat.nexus import NXobject
+# Third party modules
 import numpy as np
 
-# local modules
-from CHAP.common.utils.general import clear_plot, clear_imshow, quick_plot, quick_imshow
+# Local modules
+from CHAP.common.utils.general import (
+    is_num,
+    input_int,
+    input_yesno,
+    select_image_bounds,
+    select_one_image_bound,
+    draw_mask_1d,
+    clear_plot,
+    clear_imshow,
+    quick_plot,
+    quick_imshow,
+)
+#    input_num,
+from CHAP.common.utils.fit import Fit
 from CHAP.processor import Processor
+from CHAP.reader import main
 
-num_core_tomopy_limit = 24
+NUM_CORE_TOMOPY_LIMIT = 24
 
 
 class TomoDataProcessor(Processor):
-    '''Class representing the processes to reconstruct a set of Tomographic images returning
-    either a dictionary or a `nexusformat.nexus.NXroot` object containing the (meta) data after
-    processing each individual step.
-    '''
-
-    def _process(self, data):
-        '''Process the output of a `Reader` that contains a map or a `nexusformat.nexus.NXroot`
-        object and one that contains the step specific instructions and return either a dictionary
-        or a `nexusformat.nexus.NXroot` returning the processed result.
-
-        :param data: Result of `Reader.read` where at least one item is of type
-            `nexusformat.nexus.NXroot` or has the value `'MapConfig'` for the `'schema'` key,
-            and at least one item has the value `'TomoReduceConfig'` for the `'schema'` key.
+    """
+    Class representing the processes to reconstruct a set of Tomographic
+    images returning either a dictionary or a `nexusformat.nexus.NXroot`
+    object containing the (meta) data after processing each individual
+    step.
+    """
+
+    def _process(
+            self, data, interactive=False, reduce_data=False,
+            find_center=False, reconstruct_data=False, combine_data=False,
+            output_folder='.', save_figs=None, **kwargs):
+        """
+        Process the output of a `Reader` that contains a map or a
+        `nexusformat.nexus.NXroot` object and one that contains the step
+        specific instructions and return either a dictionary or a
+        `nexusformat.nexus.NXroot` returning the processed result.
+
+        :param data: Result of `Reader.read`
         :type data: list[dict[str,object]]
+        :param interactive: Allows interactive actions
+        :type bool, optional [False]
+        :param reduce_data: Generate reduced tomography images
+        :type bool, optional [False]
+        :param find_center: Find the calibrated center axis info
+        :type bool, optional [False]
+        :param reconstruct_data: Reconstruct the tomography data
+        :type bool, optional [False]
+        :param combine_data: Combine the reconstructed tomography stacks
+        :type bool, optional [False]
+        :param output_folder: Output folder name
+        :type str, optional ['.']
+        :param save_figs: Display and/or save figures to file
+        :type str, optional
         :return: processed (meta)data
         :rtype: dict or nexusformat.nexus.NXroot
-        '''
+        """
 
-        tomo = Tomo(save_figs='only')
+        if not isinstance(reduce_data, bool):
+            raise ValueError(f'Invalid parameter reduce_data ({reduce_data})')
+        if not isinstance(find_center, bool):
+            raise ValueError(f'Invalid parameter find_center ({find_center})')
+        if not isinstance(reconstruct_data, bool):
+            raise ValueError(
+                f'Invalid parameter reconstruct_data ({reconstruct_data})')
+        if not isinstance(combine_data, bool):
+            raise ValueError(
+                f'Invalid parameter combine_data ({combine_data})')
+
+        tomo = Tomo(
+            interactive=interactive, output_folder=output_folder,
+            save_figs=save_figs)
         nxroot = None
         center_config = None
 
         # Get and validate the relevant configuration objects in data
         configs = self.get_configs(data)
 
         # Setup the pipeline for a tomography reconstruction
         if 'setup' in configs:
             configs.pop('nxroot', None)
             nxroot = self.get_nxroot(configs.pop('map'), configs.pop('setup'))
         else:
             nxroot = configs.pop('nxroot', None)
 
         # Reduce tomography images
-        if 'reduce' in configs:
-            tool_config = configs.pop('reduce')
+        if reduce_data or 'reduce' in configs:
+            if 'reduce' in configs:
+                tool_config = configs.pop('reduce')
+                img_x_bounds = tool_config.img_x_bounds
+            else:
+                img_x_bounds = None
+                if nxroot is None:
+                    raise RuntimeError(
+                        'Unable to reduce the data without providing a '
+                        + 'reduced_data config file')
             if nxroot is None:
                 map_config = configs.pop('map')
                 nxroot = self.get_nxroot(map_config, tool_config)
-            nxroot = tomo.gen_reduced_data(nxroot, img_x_bounds=tool_config.img_x_bounds)
+            nxroot = tomo.gen_reduced_data(nxroot, img_x_bounds=img_x_bounds)
 
         # Find rotation axis centers for the tomography stacks
-        # Pass tool_config directly to tomo.find_centers?
-        if 'find_center' in configs:
-            tool_config = configs.pop('find_center')
-            center_rows = [tool_config.lower_row, tool_config.upper_row]
-            if (None in center_rows or tool_config.lower_center_offset is None or
-                    tool_config.upper_center_offset is None):
-                center_config = tomo.find_centers(nxroot, center_rows=center_rows,
-                        center_stack_index=tool_config.center_stack_index)
+        # RV pass tool_config directly to tomo.find_centers?
+        if find_center or 'find_center' in configs:
+            if 'find_center' in configs:
+                tool_config = configs.pop('find_center')
+                center_rows = (tool_config.lower_row, tool_config.upper_row)
+                lower_center_offset = tool_config.lower_center_offset
+                upper_center_offset = tool_config.upper_center_offset
+                center_stack_index = tool_config.center_stack_index
+            else:
+                center_rows = (None, None)
+                lower_center_offset = None
+                upper_center_offset = None
+                center_stack_index = None
+            if (None in center_rows or lower_center_offset is None
+                    or upper_center_offset is None):
+                center_config = tomo.find_centers(
+                    nxroot, center_rows=center_rows,
+                    center_stack_index=center_stack_index)
             else:
-                #RV make a convert to dict in basemodel?
-                center_config = {'lower_row': tool_config.lower_row,
-                        'lower_center_offset': tool_config.lower_center_offset,
-                        'upper_row': tool_config.upper_row,
-                        'upper_center_offset': tool_config.upper_center_offset}
+                # RV make a convert to dict in basemodel?
+                center_config = {
+                    'lower_row': tool_config.lower_row,
+                    'lower_center_offset': tool_config.lower_center_offset,
+                    'upper_row': tool_config.upper_row,
+                    'upper_center_offset': tool_config.upper_center_offset,
+                    'center_stack_index': tool_config.center_stack_index,
+                }
 
         # Reconstruct tomography stacks
-        # Pass tool_config and center_config directly to tomo.reconstruct_data
-        if 'reconstruct' in configs:
-            tool_config = configs.pop('reconstruct')
-            nxroot = tomo.reconstruct_data(nxroot, center_config, x_bounds=tool_config.x_bounds,
-                    y_bounds=tool_config.y_bounds, z_bounds=tool_config.z_bounds)
+        # RV pass tool_config and center_config directly to
+        #     tomo.reconstruct_data?
+        if reconstruct_data or 'reconstruct' in configs:
+            if 'reconstruct' in configs:
+                tool_config = configs.pop('reconstruct')
+                x_bounds = tool_config.x_bounds
+                y_bounds = tool_config.y_bounds
+                z_bounds = tool_config.z_bounds
+            else:
+                x_bounds = None
+                y_bounds = None
+                z_bounds = None
+            nxroot = tomo.reconstruct_data(
+                nxroot, center_config, x_bounds=x_bounds, y_bounds=y_bounds,
+                z_bounds=z_bounds)
             center_config = None
 
         # Combine reconstructed tomography stacks
-        if 'combine' in configs:
-            tool_config = configs.pop('combine')
-            nxroot = tomo.combine_data(nxroot, x_bounds=tool_config.x_bounds,
-                    y_bounds=tool_config.y_bounds, z_bounds=tool_config.z_bounds)
+        if combine_data or 'combine' in configs:
+            if 'combine' in configs:
+                tool_config = configs.pop('combine')
+                x_bounds = tool_config.x_bounds
+                y_bounds = tool_config.y_bounds
+                z_bounds = tool_config.z_bounds
+            else:
+                x_bounds = None
+                y_bounds = None
+                z_bounds = None
+            nxroot = tomo.combine_data(
+                nxroot, x_bounds=x_bounds, y_bounds=y_bounds,
+                z_bounds=z_bounds)
 
         if center_config is not None:
             return center_config
-        else:
-            return nxroot
+        return nxroot
 
     def get_configs(self, data):
-        '''Get instances of the configuration objects needed by this
+        """
+        Get instances of the configuration objects needed by this
         `Processor` from a returned value of `Reader.read`
 
         :param data: Result of `Reader.read` where at least one item
             is of type `nexusformat.nexus.NXroot` or has the value
             `'MapConfig'` for the `'schema'` key, and at least one item
             has the value `'TomoSetupConfig'`, or `'TomoReduceConfig'`,
             or `'TomoFindCenterConfig'`, or `'TomoReconstructConfig'`,
             or `'TomoCombineConfig'` for the `'schema'` key.
         :type data: list[dict[str,object]]
         :raises Exception: If valid config objects cannot be constructed
             from `data`.
         :return: valid instances of the configuration objects with field
             values taken from `data`.
         :rtype: dict
-        '''
-        #:rtype: dict{'map': MapConfig, 'reduce': TomoReduceConfig} RV: Is there a way to denote optional items?
-        from CHAP.common.models.map import MapConfig
-        from CHAP.tomo.models import TomoSetupConfig, TomoReduceConfig, TomoFindCenterConfig, \
-                TomoReconstructConfig, TomoCombineConfig
+        """
+        # :rtype: dict{'map': MapConfig, 'reduce': TomoReduceConfig}
+        # RV is there a way to denote optional items?
+        # Third party modules
         from nexusformat.nexus import NXroot
 
+        # Local modules
+        from CHAP.common.models.map import MapConfig
+        from CHAP.tomo.models import (
+            TomoSetupConfig,
+            TomoReduceConfig,
+            TomoFindCenterConfig,
+            TomoReconstructConfig,
+            TomoCombineConfig,
+        )
+
         configs = {}
         if isinstance(data, list):
             for item in data:
-                if isinstance(item, dict):
+                if isinstance(item, dict) and item.get('data') is not None:
                     schema = item.get('schema')
                     if isinstance(item.get('data'), NXroot):
                         configs['nxroot'] = item.get('data')
                     if schema == 'MapConfig':
                         configs['map'] = MapConfig(**(item.get('data')))
                     if schema == 'TomoSetupConfig':
-                        configs['setup'] = TomoSetupConfig(**(item.get('data')))
+                        configs['setup'] = TomoSetupConfig(
+                            **(item.get('data')))
                     if schema == 'TomoReduceConfig':
-                        configs['reduce'] = TomoReduceConfig(**(item.get('data')))
+                        configs['reduce'] = TomoReduceConfig(
+                            **(item.get('data')))
                     elif schema == 'TomoFindCenterConfig':
-                        configs['find_center'] = TomoFindCenterConfig(**(item.get('data')))
+                        configs['find_center'] = TomoFindCenterConfig(
+                            **(item.get('data')))
                     elif schema == 'TomoReconstructConfig':
-                        configs['reconstruct'] = TomoReconstructConfig(**(item.get('data')))
+                        configs['reconstruct'] = TomoReconstructConfig(
+                            **(item.get('data')))
                     elif schema == 'TomoCombineConfig':
-                        configs['combine'] = TomoCombineConfig(**(item.get('data')))
+                        configs['combine'] = TomoCombineConfig(
+                            **(item.get('data')))
 
         return configs
 
     def get_nxroot(self, map_config, tool_config):
-        '''Get a map of the collected tomography data from the scans in `map_config`. The
-        data will be reduced based on additional parameters included in `tool_config`.
-        The data will be returned along with relevant metadata in the form of a NeXus structure.
+        """
+        Get a map of the collected tomography data from the scans in
+        `map_config`. The data will be reduced based on additional
+        parameters included in `tool_config`. The data will be returned
+        along with relevant metadata in the form of a NeXus structure.
 
         :param map_config: the map configuration
         :type map_config: MapConfig
         :param tool_config: the tomography image reduction configuration
         :type tool_config: TomoReduceConfig
-        :return: a map of the collected tomography data along with the data reduction configuration
+        :return: a map of the collected tomography data along with the
+        data reduction configuration
         :rtype: nexusformat.nexus.NXroot
-        '''
+        """
+        # System modules
+        from copy import deepcopy
+
+        # Third party modules
+        from nexusformat.nexus import (
+            NXcollection,
+            NXdata,
+            NXdetector,
+            NXinstrument,
+            NXroot,
+            NXsample,
+            NXsource,
+            NXsubentry,
+        )
+
+        # Local modules
         from CHAP.common import MapProcessor
         from CHAP.common.models.map import import_scanparser
         from CHAP.common.utils.general import index_nearest
-        from copy import deepcopy
-        from nexusformat.nexus import NXcollection, NXdata, NXdetector, NXinstrument, NXsample, \
-                NXsource, NXsubentry, NXroot
 
-        include_raw_data = getattr(tool_config, "include_raw_data", False)
+        include_raw_data = getattr(tool_config, 'include_raw_data', False)
 
         # Construct NXroot
         nxroot = NXroot()
 
         # Construct base NXentry and add to NXroot
         nxentry = MapProcessor.get_nxentry(map_config)
         nxroot[map_config.title] = nxentry
@@ -189,37 +305,45 @@
 
         # Tag the NXsource with the runinfo (as an attribute)
 #        nxsource.attrs['cycle'] = map_config.cycle
 #        nxsource.attrs['btr'] = map_config.btr
         nxsource.attrs['station'] = map_config.station
         nxsource.attrs['experiment_type'] = map_config.experiment_type
 
-        # Add an NXdetector to the NXinstrument (don't fill in data fields yet)
+        # Add an NXdetector to the NXinstrument
+        # (do not fill in data fields yet)
         nxdetector = NXdetector()
         nxinstrument.detector = nxdetector
         nxdetector.local_name = tool_config.detector.prefix
         pixel_size = tool_config.detector.pixel_size
         if len(pixel_size) == 1:
-            nxdetector.x_pixel_size = pixel_size[0]/tool_config.detector.lens_magnification
-            nxdetector.y_pixel_size = pixel_size[0]/tool_config.detector.lens_magnification
-        else:
-            nxdetector.x_pixel_size = pixel_size[0]/tool_config.detector.lens_magnification
-            nxdetector.y_pixel_size = pixel_size[1]/tool_config.detector.lens_magnification
+            nxdetector.x_pixel_size = \
+                pixel_size[0]/tool_config.detector.lens_magnification
+            nxdetector.y_pixel_size = \
+                pixel_size[0]/tool_config.detector.lens_magnification
+        else:
+            nxdetector.x_pixel_size = \
+                pixel_size[0]/tool_config.detector.lens_magnification
+            nxdetector.y_pixel_size = \
+                pixel_size[1]/tool_config.detector.lens_magnification
         nxdetector.x_pixel_size.attrs['units'] = 'mm'
         nxdetector.y_pixel_size.attrs['units'] = 'mm'
 
         if include_raw_data:
-            # Add an NXsample to NXentry (don't fill in data fields yet)
+            # Add an NXsample to NXentry
+            # (do not fill in data fields yet)
             nxsample = NXsample()
             nxentry.sample = nxsample
             nxsample.name = map_config.sample.name
             nxsample.description = map_config.sample.description
 
-        # Add NXcollection's to NXentry to hold metadata about the spec scans in the map
-        # Also obtain the data fields in NXsample and NXdetector if requested
+        # Add NXcollection's to NXentry to hold metadata about the spec
+        #     scans in the map
+        # Also obtain the data fields in NXsample and NXdetector if
+        #     requested
         import_scanparser(map_config.station, map_config.experiment_type)
         image_keys = []
         sequence_numbers = []
         image_stacks = []
         rotation_angles = []
         x_translations = []
         z_translations = []
@@ -240,60 +364,68 @@
                     else:
                         raise RuntimeError('Invalid scan type: {scan_type}')
                 elif map_config.station in ('id3b'):
                     if scans.spec_file.endswith('_dark'):
                         image_key = 2
                         field_name = 'dark_field'
                     elif scans.spec_file.endswith('_flat'):
-                        #RV not yet tested with an actual fmb run
+                        # RV not yet tested with an actual fmb run
                         image_key = 1
                         field_name = 'bright_field'
                     else:
                         image_key = 0
                         field_name = 'tomo_fields'
                 else:
-                    raise RuntimeError(f'Invalid station: {station}')
+                    raise RuntimeError(
+                        f'Invalid station in map_config: {map_config.station}')
 
                 # Create an NXcollection for each field type
                 if field_name in nxentry.spec_scans:
                     nxcollection = nxentry.spec_scans[field_name]
                     if nxcollection.attrs['spec_file'] != str(scans.spec_file):
-                        raise RuntimeError(f'Multiple SPEC files for a single field type not yet '+
-                                f'implemented; field name: {field_name}, '+
-                                f'SPEC file: {str(scans.spec_file)}')
+                        raise RuntimeError(
+                            'Multiple SPEC files for a single field type not '
+                            + f'yet implemented; field name: {field_name}, '
+                            + f'SPEC file: {str(scans.spec_file)}')
                 else:
                     nxcollection = NXcollection()
                     nxentry.spec_scans[field_name] = nxcollection
                     nxcollection.attrs['spec_file'] = str(scans.spec_file)
                     nxcollection.attrs['date'] = scanparser.spec_scan.file_date
 
                 # Get thetas
                 image_offset = scanparser.starting_image_offset
                 if map_config.station in ('id1a3', 'id3a'):
                     theta_vals = scanparser.theta_vals
-                    thetas = np.linspace(theta_vals.get('start'), theta_vals.get('end'),
-                            theta_vals.get('num'))
+                    thetas = np.linspace(
+                        theta_vals.get('start'), theta_vals.get('end'),
+                        theta_vals.get('num'))
                 else:
                     if len(scans.scan_numbers) != 1:
-                        raise RuntimeError('Multiple scans not yet implemented for '+
-                                f'{map_config.station}')
+                        raise RuntimeError(
+                            'Multiple scans not yet implemented for '
+                            + f'{map_config.station}')
                     scan_number = scans.scan_numbers[0]
                     thetas = []
                     for dim in map_config.independent_dimensions:
                         if dim.label != 'theta':
                             continue
                         for index in range(scanparser.spec_scan_npts):
-                            thetas.append(dim.get_value(scans, scan_number, index))
-                    if not len(thetas):
-                        raise RuntimeError(f'Unable to obtain thetas for {field_name}')
+                            thetas.append(
+                                dim.get_value(scans, scan_number, index))
+                    if not thetas:
+                        raise RuntimeError(
+                            f'Unable to obtain thetas for {field_name}')
                     if thetas[image_offset] <= 0.0 and thetas[-1] >= 180.0:
                         image_offset = index_nearest(thetas, 0.0)
-                        thetas = thetas[image_offset:index_nearest(thetas, 180.0)]
+                        image_end = index_nearest(thetas, 180.0)
+                        thetas = thetas[image_offset:image_end]
                     elif thetas[-1]-thetas[image_offset] >= 180:
-                        thetas = thetas[image_offset:index_nearest(thetas, thetas[0]+180.0)]
+                        image_end = index_nearest(thetas, thetas[0]+180.0)
+                        thetas = thetas[image_offset:image_end]
                     else:
                         thetas = thetas[image_offset:]
 
                 # x and z translations
                 x_translation = scanparser.horizontal_shift
                 z_translation = scanparser.vertical_shift
 
@@ -301,42 +433,47 @@
                 entry_name = f'scan_{scan_number}'
                 nxsubentry = NXsubentry()
                 nxcollection[entry_name] = nxsubentry
                 nxsubentry.start_time = scanparser.spec_scan.date
                 nxsubentry.spec_command = scanparser.spec_command
                 # Add an NXinstrument to the scan's NXsubentry
                 nxsubentry.instrument = NXinstrument()
-                # Add an NXdetector to the NXinstrument to the scan's NXsubentry
+                # Add an NXdetector to the NXinstrument to the scan's
+                #     NXsubentry
                 nxsubentry.instrument.detector = deepcopy(nxdetector)
-                nxsubentry.instrument.detector.frame_start_number = image_offset
+                nxsubentry.instrument.detector.frame_start_number = \
+                    image_offset
                 nxsubentry.instrument.detector.image_key = image_key
                 # Add an NXsample to the scan's NXsubentry
                 nxsubentry.sample = NXsample()
                 nxsubentry.sample.rotation_angle = thetas
                 nxsubentry.sample.rotation_angle.units = 'degrees'
                 nxsubentry.sample.x_translation = x_translation
                 nxsubentry.sample.x_translation.units = 'mm'
                 nxsubentry.sample.z_translation = z_translation
                 nxsubentry.sample.z_translation.units = 'mm'
 
                 if include_raw_data:
                     num_image = len(thetas)
                     image_keys += num_image*[image_key]
                     sequence_numbers += list(range(num_image))
-                    image_stacks.append(scanparser.get_detector_data(tool_config.detector.prefix,
-                            scan_step_index=(image_offset, image_offset+num_image)))
+                    image_stacks.append(
+                        scanparser.get_detector_data(
+                            tool_config.detector.prefix,
+                            scan_step_index=(image_offset,
+                                             image_offset+num_image)))
                     rotation_angles += list(thetas)
                     x_translations += num_image*[x_translation]
                     z_translations += num_image*[z_translation]
 
         if include_raw_data:
             # Add image data to NXdetector
             nxinstrument.detector.image_key = image_keys
             nxinstrument.detector.sequence_number = sequence_numbers
-            nxinstrument.detector.data = np.concatenate([image for image in image_stacks])
+            nxinstrument.detector.data = np.concatenate(image_stacks)
 
             # Add image data to NXsample
             nxsample.rotation_angle = rotation_angles
             nxsample.rotation_angle.attrs['units'] = 'degrees'
             nxsample.x_translation = x_translations
             nxsample.x_translation.attrs['units'] = 'mm'
             nxsample.z_translation = z_translations
@@ -351,206 +488,205 @@
             nxdata.makelink(nxentry.sample.x_translation)
             nxdata.makelink(nxentry.sample.z_translation)
 #            nxdata.attrs['axes'] = ['field', 'row', 'column']
 #            nxdata.attrs['field_indices'] = 0
 #            nxdata.attrs['row_indices'] = 1
 #            nxdata.attrs['column_indices'] = 2
 
-        return(nxroot)
+        return nxroot
 
 
-def nxcopy(nxobject:NXobject, exclude_nxpaths:list[str]=[], nxpath_prefix:str='') -> NXobject:
-    '''Function that returns a copy of a nexus object, optionally exluding certain child items.
+def nxcopy(nxobject, exclude_nxpaths=None, nxpath_prefix=''):
+    """
+    Function that returns a copy of a nexus object, optionally exluding
+    certain child items.
 
     :param nxobject: the original nexus object to return a "copy" of
     :type nxobject: nexusformat.nexus.NXobject
     :param exlude_nxpaths: a list of paths to child nexus objects that
         should be exluded from the returned "copy", defaults to `[]`
     :type exclude_nxpaths: list[str], optional
     :param nxpath_prefix: For use in recursive calls from inside this
         function only!
     :type nxpath_prefix: str
     :return: a copy of `nxobject` with some children optionally exluded.
     :rtype: NXobject
-    '''
+    """
+    # Third party modules
     from nexusformat.nexus import NXgroup
 
     nxobject_copy = nxobject.__class__()
-    if not len(nxpath_prefix):
+    if not nxpath_prefix:
         if 'default' in nxobject.attrs:
             nxobject_copy.attrs['default'] = nxobject.attrs['default']
     else:
         for k, v in nxobject.attrs.items():
             nxobject_copy.attrs[k] = v
 
+    if exclude_nxpaths is None:
+        exclude_nxpaths = []
     for k, v in nxobject.items():
         nxpath = os_path.join(nxpath_prefix, k)
 
         if nxpath in exclude_nxpaths:
             continue
 
         if isinstance(v, NXgroup):
-            nxobject_copy[k] = nxcopy(v, exclude_nxpaths=exclude_nxpaths,
-                    nxpath_prefix=os_path.join(nxpath_prefix, k))
+            nxobject_copy[k] = nxcopy(
+                v, exclude_nxpaths=exclude_nxpaths,
+                nxpath_prefix=os_path.join(nxpath_prefix, k))
         else:
             nxobject_copy[k] = v
 
-    return(nxobject_copy)
+    return nxobject_copy
 
 
-class set_numexpr_threads:
+class SetNumexprThreads:
+    """
+    Class that sets and keeps track of the number of processors used by
+    the code in general and by the num_expr package specifically.
+
+    :ivar num_core: Number of processors used by the num_expr package
+    :type num_core: int
+    """
+
     def __init__(self, num_core):
+        """Initialize SetNumexprThreads."""
+        # System modules
         from multiprocessing import cpu_count
 
         if num_core is None or num_core < 1 or num_core > cpu_count():
-            self.num_core = cpu_count()
+            self._num_core = cpu_count()
         else:
-            self.num_core = num_core
+            self._num_core = num_core
+        self._num_core_org = self._num_core
 
     def __enter__(self):
-        import numexpr as ne
+        # Third party modules
+        from numexpr import (
+            MAX_THREADS,
+            set_num_threads,
+        )
 
-        self.num_core_org = ne.set_num_threads(min(self.num_core, ne.MAX_THREADS))
+        self._num_core_org = set_num_threads(
+            min(self._num_core, MAX_THREADS))
 
     def __exit__(self, exc_type, exc_value, traceback):
-        import numexpr as ne
+        # Third party modules
+        from numexpr import set_num_threads
 
-        ne.set_num_threads(self.num_core_org)
+        set_num_threads(self._num_core_org)
 
 
 class Tomo:
-    """Processing tomography data with misalignment.
-    """
-    def __init__(self, galaxy_flag=False, num_core=-1, output_folder='.', save_figs=None,
-            test_mode=False):
-        """Initialize with optional config input file or dictionary
-        """
-        from logging import getLogger
+    """Reconstruct a set of Tomographic images."""
 
+    def __init__(
+            self, interactive=False, num_core=-1, output_folder='.',
+            save_figs=None, test_mode=False):
+        """Initialize Tomo."""
+        # System modules
+        from logging import getLogger
         from multiprocessing import cpu_count
 
         self.__name__ = self.__class__.__name__
-        self.logger = getLogger(self.__name__)
-        self.logger.propagate = False
+        self._logger = getLogger(self.__name__)
+        self._logger.propagate = False
 
-        if not isinstance(galaxy_flag, bool):
-            raise ValueError(f'Invalid parameter galaxy_flag ({galaxy_flag})')
-        self.galaxy_flag = galaxy_flag
-        self.num_core = num_core
-        if self.galaxy_flag:
-            if output_folder != '.':
-                self.logger.warning('Ignoring output_folder in galaxy mode')
-            self.output_folder = '.'
-            if test_mode != False:
-                self.logger.warning('Ignoring test_mode in galaxy mode')
-            self.test_mode = False
-            if save_figs is not None:
-                self.logger.warning('Ignoring save_figs in galaxy mode')
-            save_figs = 'only'
+        if not isinstance(interactive, bool):
+            raise ValueError(f'Invalid parameter interactive ({interactive})')
+        self._interactive = interactive
+        self._num_core = num_core
+        self._output_folder = os_path.abspath(output_folder)
+        if not os_path.isdir(output_folder):
+            mkdir(os_path.abspath(output_folder))
+        if self._interactive:
+            self._test_mode = False
         else:
-            self.output_folder = os_path.abspath(output_folder)
-            if not os_path.isdir(output_folder):
-                mkdir(os_path.abspath(output_folder))
             if not isinstance(test_mode, bool):
                 raise ValueError(f'Invalid parameter test_mode ({test_mode})')
-            self.test_mode = test_mode
+            self._test_mode = test_mode
             if save_figs is None:
                 save_figs = 'no'
-        self.test_config = {}
-        if self.test_mode:
+        self._test_config = {}
+        if self._test_mode:
             if save_figs != 'only':
-                self.logger.warning('Ignoring save_figs in test mode')
+                self._logger.warning('Ignoring save_figs in test mode')
             save_figs = 'only'
         if save_figs == 'only':
-            self.save_only = True
-            self.save_figs = True
+            self._save_only = True
+            self._save_figs = True
         elif save_figs == 'yes':
-            self.save_only = False
-            self.save_figs = True
+            self._save_only = False
+            self._save_figs = True
         elif save_figs == 'no':
-            self.save_only = False
-            self.save_figs = False
+            self._save_only = False
+            self._save_figs = False
         else:
             raise ValueError(f'Invalid parameter save_figs ({save_figs})')
-        if self.save_only:
-            self.block = False
+        if self._save_only:
+            self._block = False
         else:
-            self.block = True
-        if self.num_core == -1:
-            self.num_core = cpu_count()
-        if not isinstance(self.num_core, int) or self.num_core < 0:
+            self._block = True
+        if self._num_core == -1:
+            self._num_core = cpu_count()
+        if not isinstance(self._num_core, int) or self._num_core < 0:
             raise ValueError(f'Invalid parameter num_core ({num_core})')
-        if self.num_core > cpu_count():
-            self.logger.warning(f'num_core = {self.num_core} is larger than the number of '
-                    f'available processors and reduced to {cpu_count()}')
-            self.num_core= cpu_count()
-
-    def read(self, filename):
-        extension = os_path.splitext(filename)[1]
-        if extension == '.yml' or extension == '.yaml':
-            with open(filename, 'r') as f:
-                config = safe_load(f)
-#            if len(config) > 1:
-#                raise ValueError(f'Multiple root entries in {filename} not yet implemented')
-#            if len(list(config.values())[0]) > 1:
-#                raise ValueError(f'Multiple sample maps in {filename} not yet implemented')
-            return(config)
-        elif extension == '.nxs':
-            with NXFile(filename, mode='r') as nxfile:
-                nxroot = nxfile.readfile()
-            return(nxroot)
-        else:
-            raise ValueError(f'Invalid filename extension ({extension})')
-
-    def write(self, data, filename):
-        extension = os_path.splitext(filename)[1]
-        if extension == '.yml' or extension == '.yaml':
-            with open(filename, 'w') as f:
-                safe_dump(data, f)
-        elif extension == '.nxs':
-            data.save(filename, mode='w')
-        elif extension == '.nc':
-            data.to_netcdf(os_path=filename)
-        else:
-            raise ValueError(f'Invalid filename extension ({extension})')
+        if self._num_core > cpu_count():
+            self._logger.warning(
+                f'num_core = {self._num_core} is larger than the number '
+                + f'of available processors and reduced to {cpu_count()}')
+            self._num_core = cpu_count()
 
     def gen_reduced_data(self, data, img_x_bounds=None):
-        """Generate the reduced tomography images.
         """
-        from nexusformat.nexus import NXdata, NXprocess, NXroot
+        Generate the reduced tomography images.
 
-        from CHAP.common.models.map import import_scanparser
+        :param data: Data object containing the raw data info and
+            metadata required for a tomography data reduction
+        :type data: nexusformat.nexus.NXroot
+        :param img_x_bounds: Detector image bounds in the x-direction
+        :type img_x_bounds: tuple(int, int), list[int], optional
+        :return: Reduced tomography data
+        :rtype: nexusformat.nexus.NXroot
+        """
+        # Third party modules
+        from nexusformat.nexus import (
+            NXdata,
+            NXprocess,
+            NXroot,
+        )
 
-        self.logger.info('Generate the reduced tomography images')
+        self._logger.info('Generate the reduced tomography images')
         if img_x_bounds is not None:
             if not isinstance(img_x_bounds, (tuple, list)):
-                raise ValueError(f'Invalid parameter img_x_bounds ({img_x_bounds})')
+                raise ValueError(
+                    f'Invalid parameter img_x_bounds ({img_x_bounds})')
             img_x_bounds = tuple(img_x_bounds)
 
-        # Create plot galaxy path directory if needed
-        if self.galaxy_flag and not os_path.exists('tomo_reduce_plots'):
-            mkdir('tomo_reduce_plots')
-
-        if isinstance(data, dict):
-            # Create Nexus format object from input dictionary
-            wf = TomoWorkflow(**data)
-            if len(wf.sample_maps) > 1:
-                raise ValueError(f'Multiple sample maps not yet implemented')
-            nxroot = NXroot()
-            t0 = time()
-            for sample_map in wf.sample_maps:
-                self.logger.info(f'Start constructing the {sample_map.title} map.')
-                import_scanparser(sample_map.station)
-                sample_map.construct_nxentry(nxroot, include_raw_data=False)
-            self.logger.info(f'Constructed all sample maps in {time()-t0:.2f} seconds.')
-            nxentry = nxroot[nxroot.attrs['default']]
-            # Get test mode configuration info
-            if self.test_mode:
-                self.test_config = data['sample_maps'][0]['test_mode']
-        elif isinstance(data, NXroot):
+#        if isinstance(data, dict):
+#            # Create Nexus format object from input dictionary
+#            wf = TomoWorkflow(**data)
+#            if len(wf.sample_maps) > 1:
+#                raise ValueError('Multiple sample maps not yet implemented')
+#            nxroot = NXroot()
+#            t0 = time()
+#            for sample_map in wf.sample_maps:
+#                self._logger.info(
+#                    f'Start constructing the {sample_map.title} map')
+#                import_scanparser(sample_map.station)
+#                sample_map.construct_nxentry(nxroot, include_raw_data=False)
+#            self._logger.info(
+#                f'Constructed all sample maps in {time()-t0:.2f} seconds')
+#            nxentry = nxroot[nxroot.attrs['default']]
+#            # Get test mode configuration info
+#            if self._test_mode:
+#                self._test_config = data['sample_maps'][0]['test_mode']
+#        elif isinstance(data, NXroot):
+        if isinstance(data, NXroot):
             nxentry = data[data.attrs['default']]
         else:
             raise ValueError(f'Invalid parameter data ({data})')
 
         # Create an NXprocess to store data reduction (meta)data
         reduced_data = NXprocess()
 
@@ -558,235 +694,288 @@
         if 'dark_field' in nxentry['spec_scans']:
             reduced_data = self._gen_dark(nxentry, reduced_data)
 
         # Generate bright field
         reduced_data = self._gen_bright(nxentry, reduced_data)
 
         # Set vertical detector bounds for image stack
-        img_x_bounds = self._set_detector_bounds(nxentry, reduced_data, img_x_bounds=img_x_bounds)
-        self.logger.info(f'img_x_bounds = {img_x_bounds}')
+        img_x_bounds = self._set_detector_bounds(
+            nxentry, reduced_data, img_x_bounds=img_x_bounds)
+        self._logger.info(f'img_x_bounds = {img_x_bounds}')
         reduced_data['img_x_bounds'] = img_x_bounds
 
         # Set zoom and/or theta skip to reduce memory the requirement
         zoom_perc, num_theta_skip = self._set_zoom_or_skip()
         if zoom_perc is not None:
             reduced_data.attrs['zoom_perc'] = zoom_perc
         if num_theta_skip is not None:
             reduced_data.attrs['num_theta_skip'] = num_theta_skip
 
         # Generate reduced tomography fields
         reduced_data = self._gen_tomo(nxentry, reduced_data)
 
-        # Create a copy of the input Nexus object and remove raw and any existing reduced data
+        # Create a copy of the input Nexus object and remove raw and
+        #     any existing reduced data
         if isinstance(data, NXroot):
-            exclude_items = [f'{nxentry._name}/reduced_data/data',
-                    f'{nxentry._name}/instrument/detector/data',
-                    f'{nxentry._name}/instrument/detector/image_key',
-                    f'{nxentry._name}/instrument/detector/sequence_number',
-                    f'{nxentry._name}/sample/rotation_angle',
-                    f'{nxentry._name}/sample/x_translation',
-                    f'{nxentry._name}/sample/z_translation',
-                    f'{nxentry._name}/data/data',
-                    f'{nxentry._name}/data/image_key',
-                    f'{nxentry._name}/data/rotation_angle',
-                    f'{nxentry._name}/data/x_translation',
-                    f'{nxentry._name}/data/z_translation']
+            exclude_items = [
+                f'{nxentry.nxname}/reduced_data/data',
+                f'{nxentry.nxname}/instrument/detector/data',
+                f'{nxentry.nxname}/instrument/detector/image_key',
+                f'{nxentry.nxname}/instrument/detector/sequence_number',
+                f'{nxentry.nxname}/sample/rotation_angle',
+                f'{nxentry.nxname}/sample/x_translation',
+                f'{nxentry.nxname}/sample/z_translation',
+                f'{nxentry.nxname}/data/data',
+                f'{nxentry.nxname}/data/image_key',
+                f'{nxentry.nxname}/data/rotation_angle',
+                f'{nxentry.nxname}/data/x_translation',
+                f'{nxentry.nxname}/data/z_translation',
+            ]
             nxroot = nxcopy(data, exclude_nxpaths=exclude_items)
             nxentry = nxroot[nxroot.attrs['default']]
 
         # Add the reduced data NXprocess
         nxentry.reduced_data = reduced_data
 
         if 'data' not in nxentry:
             nxentry.data = NXdata()
         nxentry.attrs['default'] = 'data'
-        nxentry.data.makelink(nxentry.reduced_data.data.tomo_fields, name='reduced_data')
-        nxentry.data.makelink(nxentry.reduced_data.rotation_angle, name='rotation_angle')
+        nxentry.data.makelink(
+            nxentry.reduced_data.data.tomo_fields, name='reduced_data')
+        nxentry.data.makelink(
+            nxentry.reduced_data.rotation_angle, name='rotation_angle')
         nxentry.data.attrs['signal'] = 'reduced_data'
- 
-        return(nxroot)
+
+        return nxroot
 
     def find_centers(self, nxroot, center_rows=None, center_stack_index=None):
-        """Find the calibrated center axis info
         """
-        from nexusformat.nexus import NXentry, NXroot
+        Find the calibrated center axis info
 
-        from CHAP.common.utils.general import is_int_pair
+        :param nxroot: Data object containing the reduced data and
+            metadata required to find the calibrated center axis info
+        :type data: nexusformat.nexus.NXroot
+        :param center_rows: Lower and upper row indices for center
+            finding
+        :type center_rows: tuple(int, int), list[int], optional
+        :return: Calibrated center axis info
+        :rtype: dict
+        """
+        # Third party modules
+        from nexusformat.nexus import (
+            NXentry,
+            NXroot,
+        )
+        from yaml import safe_dump
 
-        self.logger.info('Find the calibrated center axis info')
+        self._logger.info('Find the calibrated center axis info')
 
         if not isinstance(nxroot, NXroot):
             raise ValueError(f'Invalid parameter nxroot ({nxroot})')
         nxentry = nxroot[nxroot.attrs['default']]
         if not isinstance(nxentry, NXentry):
             raise ValueError(f'Invalid nxentry ({nxentry})')
-        if self.galaxy_flag:
-            if center_rows is not None:
-                center_rows = tuple(center_rows)
-                if not is_int_pair(center_rows):
-                    raise ValueError(f'Invalid parameter center_rows ({center_rows})')
-        elif center_rows is not None:
-#            self.logger.warning(f'Ignoring parameter center_rows ({center_rows})')
-#            center_rows = None
-             if not isinstance(center_rows, (tuple, list)) or len(center_rows) != 2:
-                raise ValueError(f'Invalid parameter center_rows ({center_rows})')
-        if self.galaxy_flag:
-            if center_stack_index is not None and (not isinstance(center_stack_index, int) or
-                    center_stack_index < 0):
-                raise ValueError(f'Invalid parameter center_stack_index ({center_stack_index})')
-
-        # Create plot galaxy path directory and path if needed
-        if self.galaxy_flag:
-            if not os_path.exists('tomo_find_centers_plots'):
-                mkdir('tomo_find_centers_plots')
-            path = 'tomo_find_centers_plots'
-        else:
-            path = self.output_folder
+        if (center_rows is not None
+                and (not isinstance(center_rows, (tuple, list))
+                     or len(center_rows) != 2)):
+            raise ValueError(f'Invalid parameter center_rows ({center_rows})')
+        if (not self._interactive
+                and (center_rows is None
+                     or (center_rows[0] is None and center_rows[1] is None))):
+            self._logger.warning(
+                'center_rows unspecified, find centers at reduced data bounds')
+        if (center_stack_index is not None
+                and (not isinstance(center_stack_index, int)
+                     or center_stack_index < 0)):
+            raise ValueError(
+                'Invalid parameter center_stack_index '
+                + f'({center_stack_index})')
 
         # Check if reduced data is available
-        if ('reduced_data' not in nxentry or 'reduced_data' not in nxentry.data):
+        if ('reduced_data' not in nxentry
+                or 'reduced_data' not in nxentry.data):
             raise KeyError(f'Unable to find valid reduced data in {nxentry}.')
 
         # Select the image stack to calibrate the center axis
-        #   reduced data axes order: stack,theta,row,column
-        #   Note: Nexus cannot follow a link if the data it points to is too big,
-        #         so get the data from the actual place, not from nxentry.data
+        #     reduced data axes order: stack,theta,row,column
+        # Note: Nexus can't follow a link if the data it points to is
+        #     too big get the data from the actual place, not from
+        #     nxentry.data
         tomo_fields_shape = nxentry.reduced_data.data.tomo_fields.shape
-        if len(tomo_fields_shape) != 4 or any(True for dim in tomo_fields_shape if not dim):
-            raise KeyError('Unable to load the required reduced tomography stack')
+        if (len(tomo_fields_shape) != 4
+                or any(True for dim in tomo_fields_shape if not dim)):
+            raise KeyError(
+                'Unable to load the required reduced tomography stack')
         num_tomo_stacks = tomo_fields_shape[0]
         if num_tomo_stacks == 1:
             center_stack_index = 0
             default = 'n'
         else:
-            if self.test_mode:
-                center_stack_index = self.test_config['center_stack_index']-1 # make offset 0
-            elif self.galaxy_flag:
+            if self._test_mode:
+                # Convert input value to offset 0
+                center_stack_index = self._test_config['center_stack_index']-1
+            elif self._interactive:
                 if center_stack_index is None:
-                    center_stack_index = int(num_tomo_stacks/2)
-                if center_stack_index >= num_tomo_stacks:
-                    raise ValueError(f'Invalid parameter center_stack_index ({center_stack_index})')
+                    center_stack_index = input_int(
+                        '\nEnter tomography stack index to calibrate the '
+                        + 'center axis', ge=1, le=num_tomo_stacks,
+                        default=int(1 + num_tomo_stacks/2))
+                center_stack_index -= 1
             else:
                 if center_stack_index is None:
-                    center_stack_index = input_int('\nEnter tomography stack index to calibrate '
-                            'the center axis', ge=1, le=num_tomo_stacks,
-                            default=int(1+num_tomo_stacks/2))
-                else:
-                    if (not isinstance(center_stack_index, int) or
-                            not 0 < center_stack_index <= num_tomo_stacks):
-                        raise ValueError('Invalid parameter center_stack_index '+
-                                f'({center_stack_index})')
-                center_stack_index -= 1
+                    center_stack_index = int(num_tomo_stacks/2)
+                    self._logger.warning(
+                        'center_stack_index unspecified, use stack '
+                        + f'{center_stack_index+1} to find centers')
             default = 'y'
 
         # Get thetas (in degrees)
         thetas = np.asarray(nxentry.reduced_data.rotation_angle)
 
         # Get effective pixel_size
         if 'zoom_perc' in nxentry.reduced_data:
-            eff_pixel_size = 100.*(nxentry.instrument.detector.x_pixel_size/
-                nxentry.reduced_data.attrs['zoom_perc'])
+            eff_pixel_size = \
+                100.0 * (nxentry.instrument.detector.x_pixel_size
+                         / nxentry.reduced_data.attrs['zoom_perc'])
         else:
             eff_pixel_size = nxentry.instrument.detector.x_pixel_size
 
         # Get cross sectional diameter
         cross_sectional_dim = tomo_fields_shape[3]*eff_pixel_size
-        self.logger.debug(f'cross_sectional_dim = {cross_sectional_dim}')
+        self._logger.debug(f'cross_sectional_dim = {cross_sectional_dim}')
 
         # Determine center offset at sample row boundaries
-        self.logger.info('Determine center offset at sample row boundaries')
+        self._logger.info('Determine center offset at sample row boundaries')
 
         # Lower row center
-        if self.test_mode:
-            lower_row = self.test_config['lower_row']
-        elif self.galaxy_flag:
-            if center_rows is None:
-                lower_row = 0
-            else:
-                lower_row = min(center_rows)
-                if not 0 <= lower_row < tomo_fields_shape[2]-1:
-                    raise ValueError(f'Invalid parameter center_rows ({center_rows})')
-        else:
+        if self._test_mode:
+            lower_row = self._test_config['lower_row']
+        elif self._interactive:
             if center_rows is not None and center_rows[0] is not None:
                 lower_row = center_rows[0]
                 if lower_row == -1:
                     lower_row = 0
                 if not 0 <= lower_row < tomo_fields_shape[2]-1:
-                    raise ValueError(f'Invalid parameter center_rows ({center_rows})')
+                    raise ValueError(
+                        f'Invalid parameter center_rows ({center_rows})')
             else:
                 lower_row = select_one_image_bound(
-                        nxentry.reduced_data.data.tomo_fields[center_stack_index,0,:,:],
-                        0, bound=0, title=f'theta={round(thetas[0], 2)+0}',
-                        bound_name='row index to find lower center', default=default,
-                        raise_error=True)
-        self.logger.debug('Finding center...')
+                    nxentry.reduced_data.data.tomo_fields[
+                        center_stack_index,0,:,:],
+                    0, bound=0, title=f'theta={round(thetas[0], 2)+0}',
+                    bound_name='row index to find lower center',
+                    default=default, raise_error=True)
+        else:
+            if center_rows is None or center_rows[0] is None:
+                lower_row = 0
+            else:
+                lower_row = center_rows[0]
+                if lower_row == -1:
+                    lower_row = 0
+                if not 0 <= lower_row < tomo_fields_shape[2]-1:
+                    raise ValueError(
+                        f'Invalid parameter center_rows ({center_rows})')
         t0 = time()
         lower_center_offset = self._find_center_one_plane(
-                #np.asarray(nxentry.reduced_data.data.tomo_fields[center_stack_index,:,lower_row,:]),
-                nxentry.reduced_data.data.tomo_fields[center_stack_index,:,lower_row,:],
-                lower_row, thetas, eff_pixel_size, cross_sectional_dim, path=path,
-                num_core=self.num_core)
-        self.logger.debug(f'... done in {time()-t0:.2f} seconds')
-        self.logger.debug(f'lower_row = {lower_row:.2f}')
-        self.logger.debug(f'lower_center_offset = {lower_center_offset:.2f}')
+            nxentry.reduced_data.data.tomo_fields[
+                center_stack_index,:,lower_row,:],
+            lower_row, thetas, eff_pixel_size, cross_sectional_dim,
+            path=self._output_folder, num_core=self._num_core)
+        self._logger.info(f'Finding center took {time()-t0:.2f} seconds')
+        self._logger.debug(f'lower_row = {lower_row:.2f}')
+        self._logger.debug(f'lower_center_offset = {lower_center_offset:.2f}')
 
         # Upper row center
-        if self.test_mode:
-            upper_row = self.test_config['upper_row']
-        elif self.galaxy_flag:
-            if center_rows is None:
-                upper_row = tomo_fields_shape[2]-1
-            else:
-                upper_row = max(center_rows)
-                if not lower_row < upper_row < tomo_fields_shape[2]:
-                    raise ValueError(f'Invalid parameter center_rows ({center_rows})')
-        else:
+        if self._test_mode:
+            upper_row = self._test_config['upper_row']
+        elif self._interactive:
             if center_rows is not None and center_rows[1] is not None:
                 upper_row = center_rows[1]
                 if upper_row == -1:
                     upper_row = tomo_fields_shape[2]-1
                 if not lower_row < upper_row < tomo_fields_shape[2]:
-                    raise ValueError(f'Invalid parameter center_rows ({center_rows})')
+                    raise ValueError(
+                        f'Invalid parameter center_rows ({center_rows})')
             else:
                 upper_row = select_one_image_bound(
-                        nxentry.reduced_data.data.tomo_fields[center_stack_index,0,:,:],
-                        0, bound=tomo_fields_shape[2]-1, title=f'theta={round(thetas[0], 2)+0}',
-                        bound_name='row index to find upper center', default=default,
-                        raise_error=True)
-        self.logger.debug('Finding center...')
+                    nxentry.reduced_data.data.tomo_fields[
+                        center_stack_index,0,:,:],
+                    0, bound=tomo_fields_shape[2]-1,
+                    title=f'theta = {round(thetas[0], 2)+0}',
+                    bound_name='row index to find upper center',
+                    default=default, raise_error=True)
+        else:
+            if center_rows is None or center_rows[1] is None:
+                upper_row = tomo_fields_shape[2]-1
+            else:
+                upper_row = center_rows[1]
+                if upper_row == -1:
+                    upper_row = tomo_fields_shape[2]-1
+                if not lower_row < upper_row < tomo_fields_shape[2]:
+                    raise ValueError(
+                        f'Invalid parameter center_rows ({center_rows})')
         t0 = time()
         upper_center_offset = self._find_center_one_plane(
-                #np.asarray(nxentry.reduced_data.data.tomo_fields[center_stack_index,:,upper_row,:]),
-                nxentry.reduced_data.data.tomo_fields[center_stack_index,:,upper_row,:],
-                upper_row, thetas, eff_pixel_size, cross_sectional_dim, path=path,
-                num_core=self.num_core)
-        self.logger.debug(f'... done in {time()-t0:.2f} seconds')
-        self.logger.debug(f'upper_row = {upper_row:.2f}')
-        self.logger.debug(f'upper_center_offset = {upper_center_offset:.2f}')
-
-        center_config = {'lower_row': lower_row, 'lower_center_offset': lower_center_offset,
-                'upper_row': upper_row, 'upper_center_offset': upper_center_offset}
+            nxentry.reduced_data.data.tomo_fields[
+                center_stack_index,:,upper_row,:],
+            upper_row, thetas, eff_pixel_size, cross_sectional_dim,
+            path=self._output_folder, num_core=self._num_core)
+        self._logger.info(f'Finding center took {time()-t0:.2f} seconds')
+        self._logger.debug(f'upper_row = {upper_row:.2f}')
+        self._logger.debug(f'upper_center_offset = {upper_center_offset:.2f}')
+
+        center_config = {
+            'lower_row': lower_row,
+            'lower_center_offset': lower_center_offset,
+            'upper_row': upper_row,
+            'upper_center_offset': upper_center_offset,
+        }
         if num_tomo_stacks > 1:
-            center_config['center_stack_index'] = center_stack_index+1 # save as offset 1
+            # Save as offset 1
+            center_config['center_stack_index'] = center_stack_index+1
 
         # Save test data to file
-        if self.test_mode:
-            with open(f'{self.output_folder}/center_config.yaml', 'w') as f:
+        if self._test_mode:
+            with open(f'{self._output_folder}/center_config.yaml', 'w',
+                      encoding='utf8') as f:
                 safe_dump(center_config, f)
 
-        return(center_config)
+        return center_config
 
-    def reconstruct_data(self, nxroot, center_info, x_bounds=None, y_bounds=None, z_bounds=None):
-        """Reconstruct the tomography data.
+    def reconstruct_data(
+            self, nxroot, center_info, x_bounds=None, y_bounds=None,
+            z_bounds=None):
         """
-        from nexusformat.nexus import NXdata, NXentry, NXprocess, NXroot
+        Reconstruct the tomography data.
 
+        :param nxroot: Reduced data
+        :type data: nexusformat.nexus.NXroot
+        :param center_info: Calibrated center axis info
+        :type center_info: dict
+        :param x_bounds: Reconstructed image bounds in the x-direction
+        :type x_bounds: tuple(int, int), list[int], optional
+        :param y_bounds: Reconstructed image bounds in the y-direction
+        :type y_bounds: tuple(int, int), list[int], optional
+        :param z_bounds: Reconstructed image bounds in the z-direction
+        :type z_bounds: tuple(int, int), list[int], optional
+        :return: Reconstructed tomography data
+        :rtype: dict
+        """
+        # Third party modules
+        from nexusformat.nexus import (
+            NXdata,
+            NXentry,
+            NXprocess,
+            NXroot,
+        )
+
+        # Local modules
         from CHAP.common.utils.general import is_int_pair
 
-        self.logger.info('Reconstruct the tomography data')
+        self._logger.info('Reconstruct the tomography data')
 
         if not isinstance(nxroot, NXroot):
             raise ValueError(f'Invalid parameter nxroot ({nxroot})')
         nxentry = nxroot[nxroot.attrs['default']]
         if not isinstance(nxentry, NXentry):
             raise ValueError(f'Invalid nxentry ({nxentry})')
         if not isinstance(center_info, dict):
@@ -800,176 +989,220 @@
                 raise ValueError(f'Invalid parameter y_bounds ({y_bounds})')
             y_bounds = tuple(y_bounds)
         if z_bounds is not None:
             if not isinstance(z_bounds, (tuple, list)):
                 raise ValueError(f'Invalid parameter z_bounds ({z_bounds})')
             z_bounds = tuple(z_bounds)
 
-        # Create plot galaxy path directory and path if needed
-        if self.galaxy_flag:
-            if not os_path.exists('tomo_reconstruct_plots'):
-                mkdir('tomo_reconstruct_plots')
-            path = 'tomo_reconstruct_plots'
-        else:
-            path = self.output_folder
-
         # Check if reduced data is available
-        if ('reduced_data' not in nxentry or 'reduced_data' not in nxentry.data):
+        if ('reduced_data' not in nxentry
+                or 'reduced_data' not in nxentry.data):
             raise KeyError(f'Unable to find valid reduced data in {nxentry}.')
 
         # Create an NXprocess to store image reconstruction (meta)data
         nxprocess = NXprocess()
 
         # Get rotation axis rows and centers
         lower_row = center_info.get('lower_row')
         lower_center_offset = center_info.get('lower_center_offset')
         upper_row = center_info.get('upper_row')
         upper_center_offset = center_info.get('upper_center_offset')
-        if (lower_row is None or lower_center_offset is None or upper_row is None or
-                upper_center_offset is None):
-            raise KeyError(f'Unable to find valid calibrated center axis info in {center_info}.')
-        center_slope = (upper_center_offset-lower_center_offset)/(upper_row-lower_row)
+        if (lower_row is None or lower_center_offset is None
+                or upper_row is None or upper_center_offset is None):
+            raise KeyError(
+                'Unable to find valid calibrated center axis info in '
+                + f'{center_info}.')
+        center_slope = (upper_center_offset-lower_center_offset) \
+            / (upper_row-lower_row)
 
         # Get thetas (in degrees)
         thetas = np.asarray(nxentry.reduced_data.rotation_angle)
 
         # Reconstruct tomography data
-        #   reduced data axes order: stack,theta,row,column
-        #   reconstructed data order in each stack: row/z,x,y
-        #   Note: Nexus cannot follow a link if the data it points to is too big,
-        #         so get the data from the actual place, not from nxentry.data
+        #     reduced data axes order: stack,theta,row,column
+        #     reconstructed data order in each stack: row/z,x,y
+        # Note: Nexus can't follow a link if the data it points to is
+        #     too big get the data from the actual place, not from
+        #     nxentry.data
         if 'zoom_perc' in nxentry.reduced_data:
             res_title = f'{nxentry.reduced_data.attrs["zoom_perc"]}p'
         else:
             res_title = 'fullres'
-        load_error = False
         num_tomo_stacks = nxentry.reduced_data.data.tomo_fields.shape[0]
         tomo_recon_stacks = num_tomo_stacks*[np.array([])]
         for i in range(num_tomo_stacks):
-            # Convert reduced data stack from theta,row,column to row,theta,column
-            self.logger.debug(f'Reading reduced data stack {i+1}...')
+            # Convert reduced data stack from theta,row,column to
+            #     row,theta,column
             t0 = time()
             tomo_stack = np.asarray(nxentry.reduced_data.data.tomo_fields[i])
-            self.logger.debug(f'... done in {time()-t0:.2f} seconds')
-            if len(tomo_stack.shape) != 3 or any(True for dim in tomo_stack.shape if not dim):
-                raise ValueError(f'Unable to load tomography stack {i+1} for reconstruction')
+            self._logger.info(
+                f'Reading reduced data stack {i+1} took {time()-t0:.2f} '
+                + 'seconds')
+            if (len(tomo_stack.shape) != 3
+                    or any(True for dim in tomo_stack.shape if not dim)):
+                raise RuntimeError(
+                    f'Unable to load tomography stack {i+1} for '
+                    + 'reconstruction')
             tomo_stack = np.swapaxes(tomo_stack, 0, 1)
-            assert(len(thetas) == tomo_stack.shape[1])
-            assert(0 <= lower_row < upper_row < tomo_stack.shape[0])
-            center_offsets = [lower_center_offset-lower_row*center_slope,
-                    upper_center_offset+(tomo_stack.shape[0]-1-upper_row)*center_slope]
+            assert len(thetas) == tomo_stack.shape[1]
+            assert 0 <= lower_row < upper_row < tomo_stack.shape[0]
+            center_offsets = [
+                lower_center_offset-lower_row*center_slope,
+                upper_center_offset + center_slope * (
+                    tomo_stack.shape[0]-1-upper_row),
+            ]
             t0 = time()
-            self.logger.debug(f'Running _reconstruct_one_tomo_stack on {self.num_core} cores ...')
-            tomo_recon_stack = self._reconstruct_one_tomo_stack(tomo_stack, thetas,
-                    center_offsets=center_offsets, num_core=self.num_core, algorithm='gridrec')
-            self.logger.debug(f'... done in {time()-t0:.2f} seconds')
-            self.logger.info(f'Reconstruction of stack {i+1} took {time()-t0:.2f} seconds')
+            tomo_recon_stack = self._reconstruct_one_tomo_stack(
+                tomo_stack, thetas, center_offsets=center_offsets,
+                num_core=self._num_core, algorithm='gridrec')
+            self._logger.info(
+                f'Reconstruction of stack {i+1} took {time()-t0:.2f} seconds')
 
             # Combine stacks
             tomo_recon_stacks[i] = tomo_recon_stack
 
         # Resize the reconstructed tomography data
-        #   reconstructed data order in each stack: row/z,x,y
-        if self.test_mode:
-            x_bounds = tuple(self.test_config.get('x_bounds'))
-            y_bounds = tuple(self.test_config.get('y_bounds'))
+        #     reconstructed data order in each stack: row/z,x,y
+        if self._test_mode:
+            x_bounds = tuple(self._test_config.get('x_bounds'))
+            y_bounds = tuple(self._test_config.get('y_bounds'))
             z_bounds = None
-        elif self.galaxy_flag:
-            if x_bounds is not None and not is_int_pair(x_bounds, ge=0,
-                    lt=tomo_recon_stacks[0].shape[1]):
+        elif self._interactive:
+            x_bounds, y_bounds, z_bounds = self._resize_reconstructed_data(
+                tomo_recon_stacks, x_bounds=x_bounds, y_bounds=y_bounds,
+                z_bounds=z_bounds)
+        else:
+            if x_bounds is None:
+                self._logger.warning(
+                    'x_bounds unspecified, reconstruct data for full x-range')
+            elif not is_int_pair(x_bounds, ge=0,
+                                 lt=tomo_recon_stacks[0].shape[1]):
                 raise ValueError(f'Invalid parameter x_bounds ({x_bounds})')
-            if y_bounds is not None and not is_int_pair(y_bounds, ge=0,
-                    lt=tomo_recon_stacks[0].shape[1]):
+            if y_bounds is None:
+                self._logger.warning(
+                    'y_bounds unspecified, reconstruct data for full y-range')
+            elif not is_int_pair(
+                    y_bounds, ge=0, lt=tomo_recon_stacks[0].shape[2]):
                 raise ValueError(f'Invalid parameter y_bounds ({y_bounds})')
             z_bounds = None
-        else:
-            x_bounds, y_bounds, z_bounds = self._resize_reconstructed_data(tomo_recon_stacks,
-                   x_bounds=x_bounds, y_bounds=y_bounds, z_bounds=z_bounds)
         if x_bounds is None:
             x_range = (0, tomo_recon_stacks[0].shape[1])
             x_slice = int(x_range[1]/2)
         else:
             x_range = (min(x_bounds), max(x_bounds))
-            x_slice = int((x_bounds[0]+x_bounds[1])/2)
+            x_slice = int((x_bounds[0]+x_bounds[1]) / 2)
         if y_bounds is None:
             y_range = (0, tomo_recon_stacks[0].shape[2])
-            y_slice = int(y_range[1]/2)
+            y_slice = int(y_range[1] / 2)
         else:
             y_range = (min(y_bounds), max(y_bounds))
-            y_slice = int((y_bounds[0]+y_bounds[1])/2)
+            y_slice = int((y_bounds[0]+y_bounds[1]) / 2)
         if z_bounds is None:
             z_range = (0, tomo_recon_stacks[0].shape[0])
-            z_slice = int(z_range[1]/2)
+            z_slice = int(z_range[1] / 2)
         else:
             z_range = (min(z_bounds), max(z_bounds))
-            z_slice = int((z_bounds[0]+z_bounds[1])/2)
+            z_slice = int((z_bounds[0]+z_bounds[1]) / 2)
 
         # Plot a few reconstructed image slices
-        if self.save_figs:
+        if self._save_figs:
             for i, stack in enumerate(tomo_recon_stacks):
                 if num_tomo_stacks == 1:
                     basetitle = 'recon'
                 else:
                     basetitle = f'recon stack {i+1}'
                 title = f'{basetitle} {res_title} xslice{x_slice}'
-                quick_imshow(stack[z_range[0]:z_range[1],x_slice,y_range[0]:y_range[1]],
-                        title=title, path=path, save_fig=True, save_only=True)
+                quick_imshow(
+                    stack[z_range[0]:z_range[1],x_slice,y_range[0]:y_range[1]],
+                    title=title, path=self._output_folder, save_fig=True,
+                    save_only=True)
                 title = f'{basetitle} {res_title} yslice{y_slice}'
-                quick_imshow(stack[z_range[0]:z_range[1],x_range[0]:x_range[1],y_slice],
-                        title=title, path=path, save_fig=True, save_only=True)
+                quick_imshow(
+                    stack[z_range[0]:z_range[1],x_range[0]:x_range[1],y_slice],
+                    title=title, path=self._output_folder, save_fig=True,
+                    save_only=True)
                 title = f'{basetitle} {res_title} zslice{z_slice}'
-                quick_imshow(stack[z_slice,x_range[0]:x_range[1],y_range[0]:y_range[1]],
-                        title=title, path=path, save_fig=True, save_only=True)
+                quick_imshow(
+                    stack[z_slice,x_range[0]:x_range[1],y_range[0]:y_range[1]],
+                    title=title, path=self._output_folder, save_fig=True,
+                    save_only=True)
 
         # Save test data to file
-        #   reconstructed data order in each stack: row/z,x,y
-        if self.test_mode:
+        #     reconstructed data order in each stack: row/z,x,y
+        if self._test_mode:
             for i, stack in enumerate(tomo_recon_stacks):
-                np.savetxt(f'{self.output_folder}/recon_stack_{i+1}.txt',
-                        stack[z_slice,x_range[0]:x_range[1],y_range[0]:y_range[1]], fmt='%.6e')
+                np.savetxt(
+                    f'{self._output_folder}/recon_stack_{i+1}.txt',
+                    stack[z_slice,x_range[0]:x_range[1],y_range[0]:y_range[1]],
+                    fmt='%.6e')
 
         # Add image reconstruction to reconstructed data NXprocess
-        #   reconstructed data order in each stack: row/z,x,y
+        #     reconstructed data order in each stack: row/z,x,y
         nxprocess.data = NXdata()
         nxprocess.attrs['default'] = 'data'
         for k, v in center_info.items():
             nxprocess[k] = v
         if x_bounds is not None:
             nxprocess.x_bounds = x_bounds
         if y_bounds is not None:
             nxprocess.y_bounds = y_bounds
         if z_bounds is not None:
             nxprocess.z_bounds = z_bounds
-        nxprocess.data['reconstructed_data'] = np.asarray([stack[z_range[0]:z_range[1],
-                x_range[0]:x_range[1],y_range[0]:y_range[1]] for stack in tomo_recon_stacks])
+        nxprocess.data['reconstructed_data'] = np.asarray(
+            [stack[z_range[0]:z_range[1],x_range[0]:x_range[1],
+             y_range[0]:y_range[1]] for stack in tomo_recon_stacks])
         nxprocess.data.attrs['signal'] = 'reconstructed_data'
 
-        # Create a copy of the input Nexus object and remove reduced data
-        exclude_items = [f'{nxentry._name}/reduced_data/data', f'{nxentry._name}/data/reduced_data']
+        # Create a copy of the input Nexus object and remove reduced
+        #     data
+        exclude_items = [
+            f'{nxentry.nxname}/reduced_data/data',
+            f'{nxentry.nxname}/data/reduced_data',
+        ]
         nxroot_copy = nxcopy(nxroot, exclude_nxpaths=exclude_items)
 
         # Add the reconstructed data NXprocess to the new Nexus object
         nxentry_copy = nxroot_copy[nxroot_copy.attrs['default']]
         nxentry_copy.reconstructed_data = nxprocess
         if 'data' not in nxentry_copy:
             nxentry_copy.data = NXdata()
         nxentry_copy.attrs['default'] = 'data'
-        nxentry_copy.data.makelink(nxprocess.data.reconstructed_data, name='reconstructed_data')
+        nxentry_copy.data.makelink(
+            nxprocess.data.reconstructed_data, name='reconstructed_data')
         nxentry_copy.data.attrs['signal'] = 'reconstructed_data'
 
-        return(nxroot_copy)
+        return nxroot_copy
 
-    def combine_data(self, nxroot, x_bounds=None, y_bounds=None, z_bounds=None):
+    def combine_data(
+            self, nxroot, x_bounds=None, y_bounds=None, z_bounds=None):
         """Combine the reconstructed tomography stacks.
+
+        :param nxroot: A stack of reconstructed tomography datasets
+        :type data: nexusformat.nexus.NXroot
+        :param x_bounds: Combined image bounds in the x-direction
+        :type x_bounds: tuple(int, int), list[int], optional
+        :param y_bounds: Combined image bounds in the y-direction
+        :type y_bounds: tuple(int, int), list[int], optional
+        :param z_bounds: Combined image bounds in the z-direction
+        :type z_bounds: tuple(int, int), list[int], optional
+        :return: Combined reconstructed tomography data
+        :rtype: dict
         """
-        from nexusformat.nexus import NXdata, NXentry, NXprocess, NXroot
+        # Third party modules
+        from nexusformat.nexus import (
+            NXdata,
+            NXentry,
+            NXprocess,
+            NXroot,
+        )
 
+        # Local modules
         from CHAP.common.utils.general import is_int_pair
 
-        self.logger.info('Combine the reconstructed tomography stacks')
+        self._logger.info('Combine the reconstructed tomography stacks')
 
         if not isinstance(nxroot, NXroot):
             raise ValueError(f'Invalid parameter nxroot ({nxroot})')
         nxentry = nxroot[nxroot.attrs['default']]
         if not isinstance(nxentry, NXentry):
             raise ValueError(f'Invalid nxentry ({nxentry})')
         if x_bounds is not None:
@@ -981,1027 +1214,1220 @@
                 raise ValueError(f'Invalid parameter y_bounds ({y_bounds})')
             y_bounds = tuple(y_bounds)
         if z_bounds is not None:
             if not isinstance(z_bounds, (tuple, list)):
                 raise ValueError(f'Invalid parameter z_bounds ({z_bounds})')
             z_bounds = tuple(z_bounds)
 
-        # Create plot galaxy path directory and path if needed
-        if self.galaxy_flag:
-            if not os_path.exists('tomo_combine_plots'):
-                mkdir('tomo_combine_plots')
-            path = 'tomo_combine_plots'
-        else:
-            path = self.output_folder
-
         # Check if reconstructed image data is available
-        if ('reconstructed_data' not in nxentry or 'reconstructed_data' not in nxentry.data):
-            raise KeyError(f'Unable to find valid reconstructed image data in {nxentry}.')
+        if ('reconstructed_data' not in nxentry
+                or 'reconstructed_data' not in nxentry.data):
+            raise KeyError(
+                f'Unable to find valid reconstructed image data in {nxentry}')
 
-        # Create an NXprocess to store combined image reconstruction (meta)data
+        # Create an NXprocess to store combined image reconstruction
+        #     (meta)data
         nxprocess = NXprocess()
 
         # Get the reconstructed data
-        #   reconstructed data order: stack,row(z),x,y
-        #   Note: Nexus cannot follow a link if the data it points to is too big,
-        #         so get the data from the actual place, not from nxentry.data
-        num_tomo_stacks = nxentry.reconstructed_data.data.reconstructed_data.shape[0]
+        #     reconstructed data order: stack,row(z),x,y
+        # Note: Nexus can't follow a link if the data it points to is
+        #     too big get the data from the actual place, not from
+        #     nxentry.data
+        num_tomo_stacks = \
+            nxentry.reconstructed_data.data.reconstructed_data.shape[0]
         if num_tomo_stacks == 1:
-            self.logger.info('Only one stack available: leaving combine_data')
-            return(None)
+            self._logger.info('Only one stack available: leaving combine_data')
+            return None
 
         # Combine the reconstructed stacks
-        # (load one stack at a time to reduce risk of hitting Nexus data access limit)
+        # (load one stack at a time to reduce risk of hitting Nexus
+        #     data access limit)
         t0 = time()
-        self.logger.debug(f'Combining the reconstructed stacks ...')
-        tomo_recon_combined = np.asarray(nxentry.reconstructed_data.data.reconstructed_data[0])
+        tomo_recon_combined = np.asarray(
+            nxentry.reconstructed_data.data.reconstructed_data[0])
         if num_tomo_stacks > 2:
-            tomo_recon_combined = np.concatenate([tomo_recon_combined]+
-                    [nxentry.reconstructed_data.data.reconstructed_data[i]
-                    for i in range(1, num_tomo_stacks-1)])
+            tomo_recon_combined = np.concatenate(
+                [tomo_recon_combined]
+                + [nxentry.reconstructed_data.data.reconstructed_data[i]
+                   for i in range(1, num_tomo_stacks-1)])
         if num_tomo_stacks > 1:
-            tomo_recon_combined = np.concatenate([tomo_recon_combined]+
-                    [nxentry.reconstructed_data.data.reconstructed_data[num_tomo_stacks-1]])
-        self.logger.debug(f'... done in {time()-t0:.2f} seconds')
-        self.logger.info(f'Combining the reconstructed stacks took {time()-t0:.2f} seconds')
+            tomo_recon_combined = np.concatenate(
+                [tomo_recon_combined]
+                + [nxentry.reconstructed_data.data.reconstructed_data[
+                   num_tomo_stacks-1]])
+        self._logger.info(
+            f'Combining the reconstructed stacks took {time()-t0:.2f} seconds')
 
         # Resize the combined tomography data stacks
-        #   combined data order: row/z,x,y
-        if self.test_mode:
+        #     combined data order: row/z,x,y
+        if self._test_mode:
             x_bounds = None
             y_bounds = None
-            z_bounds = tuple(self.test_config.get('z_bounds'))
-        elif self.galaxy_flag:
-            if x_bounds is not None and not is_int_pair(x_bounds, ge=0,
-                    lt=tomo_recon_stacks[0].shape[1]):
-                raise ValueError(f'Invalid parameter x_bounds ({x_bounds})')
-            if y_bounds is not None and not is_int_pair(y_bounds, ge=0,
-                    lt=tomo_recon_stacks[0].shape[1]):
-                raise ValueError(f'Invalid parameter y_bounds ({y_bounds})')
-            z_bounds = None
-        else:
+            z_bounds = tuple(self._test_config.get('z_bounds'))
+        elif self._interactive:
             if x_bounds is None and x_bounds in nxentry.reconstructed_data:
                 x_bounds = (-1, -1)
             if y_bounds is None and y_bounds in nxentry.reconstructed_data:
                 y_bounds = (-1, -1)
-            x_bounds, y_bounds, z_bounds = self._resize_reconstructed_data(tomo_recon_combined,
-                    z_only=True)
+            x_bounds, y_bounds, z_bounds = self._resize_reconstructed_data(
+                tomo_recon_combined, z_only=True)
+        else:
+            if x_bounds is None:
+                self._logger.warning(
+                    'x_bounds unspecified, reconstruct data for full x-range')
+            elif not is_int_pair(
+                    x_bounds, ge=0, lt=tomo_recon_combined.shape[1]):
+                raise ValueError(f'Invalid parameter x_bounds ({x_bounds})')
+            if y_bounds is None:
+                self._logger.warning(
+                    'y_bounds unspecified, reconstruct data for full y-range')
+            elif not is_int_pair(
+                    y_bounds, ge=0, lt=tomo_recon_combined.shape[2]):
+                raise ValueError(f'Invalid parameter y_bounds ({y_bounds})')
+            z_bounds = None
         if x_bounds is None:
             x_range = (0, tomo_recon_combined.shape[1])
             x_slice = int(x_range[1]/2)
         else:
             x_range = x_bounds
-            x_slice = int((x_bounds[0]+x_bounds[1])/2)
+            x_slice = int((x_bounds[0]+x_bounds[1]) / 2)
         if y_bounds is None:
             y_range = (0, tomo_recon_combined.shape[2])
             y_slice = int(y_range[1]/2)
         else:
             y_range = y_bounds
-            y_slice = int((y_bounds[0]+y_bounds[1])/2)
+            y_slice = int((y_bounds[0]+y_bounds[1]) / 2)
         if z_bounds is None:
             z_range = (0, tomo_recon_combined.shape[0])
             z_slice = int(z_range[1]/2)
         else:
             z_range = z_bounds
-            z_slice = int((z_bounds[0]+z_bounds[1])/2)
+            z_slice = int((z_bounds[0]+z_bounds[1]) / 2)
 
         # Plot a few combined image slices
-        if self.save_figs:
-            quick_imshow(tomo_recon_combined[z_range[0]:z_range[1],x_slice,y_range[0]:y_range[1]],
-                    title=f'recon combined xslice{x_slice}', path=path, save_fig=True,
-                    save_only=True)
-            quick_imshow(tomo_recon_combined[z_range[0]:z_range[1],x_range[0]:x_range[1],y_slice],
-                    title=f'recon combined yslice{y_slice}', path=path, save_fig=True,
-                    save_only=True)
-            quick_imshow(tomo_recon_combined[z_slice,x_range[0]:x_range[1],y_range[0]:y_range[1]],
-                    title=f'recon combined zslice{z_slice}', path=path, save_fig=True,
-                    save_only=True)
+        if self._save_figs:
+            quick_imshow(
+                tomo_recon_combined[
+                    z_range[0]:z_range[1],x_slice,y_range[0]:y_range[1]],
+                title=f'recon combined xslice{x_slice}',
+                path=self._output_folder, save_fig=True, save_only=True)
+            quick_imshow(
+                tomo_recon_combined[
+                    z_range[0]:z_range[1],x_range[0]:x_range[1],y_slice],
+                title=f'recon combined yslice{y_slice}',
+                path=self._output_folder, save_fig=True, save_only=True)
+            quick_imshow(
+                tomo_recon_combined[
+                    z_slice,x_range[0]:x_range[1],y_range[0]:y_range[1]],
+                title=f'recon combined zslice{z_slice}',
+                path=self._output_folder, save_fig=True, save_only=True)
 
         # Save test data to file
-        #   combined data order: row/z,x,y
-        if self.test_mode:
-            np.savetxt(f'{self.output_folder}/recon_combined.txt', tomo_recon_combined[
-                    z_slice,x_range[0]:x_range[1],y_range[0]:y_range[1]], fmt='%.6e')
+        #     combined data order: row/z,x,y
+        if self._test_mode:
+            np.savetxt(
+                f'{self._output_folder}/recon_combined.txt',
+                tomo_recon_combined[
+                    z_slice,x_range[0]:x_range[1],y_range[0]:y_range[1]],
+                fmt='%.6e')
 
         # Add image reconstruction to reconstructed data NXprocess
-        #   combined data order: row/z,x,y
+        #     combined data order: row/z,x,y
         nxprocess.data = NXdata()
         nxprocess.attrs['default'] = 'data'
         if x_bounds is not None:
             nxprocess.x_bounds = x_bounds
         if y_bounds is not None:
             nxprocess.y_bounds = y_bounds
         if z_bounds is not None:
             nxprocess.z_bounds = z_bounds
         nxprocess.data['combined_data'] = tomo_recon_combined[
-                z_range[0]:z_range[1],x_range[0]:x_range[1],y_range[0]:y_range[1]]
+            z_range[0]:z_range[1],x_range[0]:x_range[1],y_range[0]:y_range[1]]
         nxprocess.data.attrs['signal'] = 'combined_data'
 
-        # Create a copy of the input Nexus object and remove reconstructed data
-        exclude_items = [f'{nxentry._name}/reconstructed_data/data',
-                f'{nxentry._name}/data/reconstructed_data']
+        # Create a copy of the input Nexus object and remove
+        #     reconstructed data
+        exclude_items = [
+            f'{nxentry.nxname}/reconstructed_data/data',
+            f'{nxentry.nxname}/data/reconstructed_data',
+        ]
         nxroot_copy = nxcopy(nxroot, exclude_nxpaths=exclude_items)
 
         # Add the combined data NXprocess to the new Nexus object
         nxentry_copy = nxroot_copy[nxroot_copy.attrs['default']]
         nxentry_copy.combined_data = nxprocess
         if 'data' not in nxentry_copy:
             nxentry_copy.data = NXdata()
         nxentry_copy.attrs['default'] = 'data'
-        nxentry_copy.data.makelink(nxprocess.data.combined_data, name='combined_data')
+        nxentry_copy.data.makelink(
+            nxprocess.data.combined_data, name='combined_data')
         nxentry_copy.data.attrs['signal'] = 'combined_data'
 
-        return(nxroot_copy)
+        return nxroot_copy
 
     def _gen_dark(self, nxentry, reduced_data):
-        """Generate dark field.
-        """
+        """Generate dark field."""
+        # Third party modules
         from nexusformat.nexus import NXdata
 
-        from CHAP.common.models.map import get_scanparser, import_scanparser
+        # Local modules
+        from CHAP.common.models.map import (
+            get_scanparser,
+            import_scanparser,
+        )
 
         # Get the dark field images
         image_key = nxentry.instrument.detector.get('image_key', None)
         if image_key and 'data' in nxentry.instrument.detector:
-            field_indices = [index for index, key in enumerate(image_key) if key == 2]
+            field_indices = [
+                index for index, key in enumerate(image_key) if key == 2]
             tdf_stack = nxentry.instrument.detector.data[field_indices,:,:]
-            # RV the default NXtomo form does not accomodate bright or dark field stacks
+            # RV the default NXtomo form does not accomodate dark field
+            #     stacks
         else:
-            import_scanparser(nxentry.instrument.source.attrs['station'],
-                    nxentry.instrument.source.attrs['experiment_type'])
+            import_scanparser(
+                nxentry.instrument.source.attrs['station'],
+                nxentry.instrument.source.attrs['experiment_type'])
             dark_field_scans = nxentry.spec_scans.dark_field
             detector_prefix = str(nxentry.instrument.detector.local_name)
             tdf_stack = []
             for nxsubentry_name, nxsubentry in dark_field_scans.items():
                 scan_number = int(nxsubentry_name.split('_')[-1])
-                scanparser = get_scanparser(dark_field_scans.attrs['spec_file'], scan_number)
-                image_offset = int(nxsubentry.instrument.detector.frame_start_number)
+                scanparser = get_scanparser(
+                    dark_field_scans.attrs['spec_file'], scan_number)
+                image_offset = int(
+                    nxsubentry.instrument.detector.frame_start_number)
                 num_image = len(nxsubentry.sample.rotation_angle)
-                tdf_stack.append(scanparser.get_detector_data(detector_prefix,
+                tdf_stack.append(
+                    scanparser.get_detector_data(
+                        detector_prefix,
                         (image_offset, image_offset+num_image)))
             if isinstance(tdf_stack, list):
-                assert(len(tdf_stack) == 1) # TODO
+                assert len(tdf_stack) == 1  # RV
                 tdf_stack = tdf_stack[0]
 
         # Take median
         if tdf_stack.ndim == 2:
             tdf = tdf_stack
         elif tdf_stack.ndim == 3:
             tdf = np.median(tdf_stack, axis=0)
             del tdf_stack
         else:
-           raise ValueError(f'Invalid tdf_stack shape ({tdf_stack.shape})')
+            raise RuntimeError(f'Invalid tdf_stack shape ({tdf_stack.shape})')
 
         # Remove dark field intensities above the cutoff
-#RV        tdf_cutoff = None
-        tdf_cutoff = tdf.min()+2*(np.median(tdf)-tdf.min())
-        self.logger.debug(f'tdf_cutoff = {tdf_cutoff}')
+#        tdf_cutoff = None
+        tdf_cutoff = tdf.min() + 2 * (np.median(tdf)-tdf.min())
+        self._logger.debug(f'tdf_cutoff = {tdf_cutoff}')
         if tdf_cutoff is not None:
             if not isinstance(tdf_cutoff, (int, float)) or tdf_cutoff < 0:
-                self.logger.warning(f'Ignoring illegal value of tdf_cutoff {tdf_cutoff}')
+                self._logger.warning(
+                    f'Ignoring illegal value of tdf_cutoff {tdf_cutoff}')
             else:
                 tdf[tdf > tdf_cutoff] = np.nan
-                self.logger.debug(f'tdf_cutoff = {tdf_cutoff}')
+                self._logger.debug(f'tdf_cutoff = {tdf_cutoff}')
 
         # Remove nans
         tdf_mean = np.nanmean(tdf)
-        self.logger.debug(f'tdf_mean = {tdf_mean}')
-        np.nan_to_num(tdf, copy=False, nan=tdf_mean, posinf=tdf_mean, neginf=0.)
+        self._logger.debug(f'tdf_mean = {tdf_mean}')
+        np.nan_to_num(
+            tdf, copy=False, nan=tdf_mean, posinf=tdf_mean, neginf=0.0)
 
         # Plot dark field
-        if self.save_figs:
-            if self.galaxy_flag:
-                quick_imshow(tdf, title='dark field', path='tomo_reduce_plots', save_fig=True,
-                        save_only=True)
-            else:
-                quick_imshow(tdf, title='dark field', path=self.output_folder, save_fig=True,
-                        save_only=True)
+        if self._save_figs:
+            quick_imshow(
+                tdf, title='dark field', path=self._output_folder,
+                save_fig=True, save_only=True)
 
         # Add dark field to reduced data NXprocess
         reduced_data.data = NXdata()
         reduced_data.data['dark_field'] = tdf
 
-        return(reduced_data)
+        return reduced_data
 
     def _gen_bright(self, nxentry, reduced_data):
-        """Generate bright field.
-        """
+        """Generate bright field."""
+        # Third party modules
         from nexusformat.nexus import NXdata
 
-        from CHAP.common.models.map import get_scanparser, import_scanparser
+        # Local modules
+        from CHAP.common.models.map import (
+            get_scanparser,
+            import_scanparser,
+        )
 
         # Get the bright field images
         image_key = nxentry.instrument.detector.get('image_key', None)
         if image_key and 'data' in nxentry.instrument.detector:
-            field_indices = [index for index, key in enumerate(image_key) if key == 1]
+            field_indices = [
+                index for index, key in enumerate(image_key) if key == 1]
             tbf_stack = nxentry.instrument.detector.data[field_indices,:,:]
-            # RV the default NXtomo form does not accomodate bright or dark field stacks
+            # RV the default NXtomo form does not accomodate bright
+            #     field stacks
         else:
-            import_scanparser(nxentry.instrument.source.attrs['station'],
-                    nxentry.instrument.source.attrs['experiment_type'])
+            import_scanparser(
+                nxentry.instrument.source.attrs['station'],
+                nxentry.instrument.source.attrs['experiment_type'])
             bright_field_scans = nxentry.spec_scans.bright_field
             detector_prefix = str(nxentry.instrument.detector.local_name)
             tbf_stack = []
             for nxsubentry_name, nxsubentry in bright_field_scans.items():
                 scan_number = int(nxsubentry_name.split('_')[-1])
-                scanparser = get_scanparser(bright_field_scans.attrs['spec_file'], scan_number)
-                image_offset = int(nxsubentry.instrument.detector.frame_start_number)
+                scanparser = get_scanparser(
+                    bright_field_scans.attrs['spec_file'], scan_number)
+                image_offset = int(
+                    nxsubentry.instrument.detector.frame_start_number)
                 num_image = len(nxsubentry.sample.rotation_angle)
-                tbf_stack.append(scanparser.get_detector_data(detector_prefix,
+                tbf_stack.append(
+                    scanparser.get_detector_data(
+                        detector_prefix,
                         (image_offset, image_offset+num_image)))
             if isinstance(tbf_stack, list):
-                assert(len(tbf_stack) == 1) # TODO
+                assert len(tbf_stack) == 1  # RV
                 tbf_stack = tbf_stack[0]
 
         # Take median if more than one image
-        """Median or mean: It may be best to try the median because of some image 
-           artifacts that arise due to crinkles in the upstream kapton tape windows 
-           causing some phase contrast images to appear on the detector.
-           One thing that also may be useful in a future implementation is to do a 
-           brightfield adjustment on EACH frame of the tomo based on a ROI in the 
-           corner of the frame where there is no sample but there is the direct X-ray 
-           beam because there is frame to frame fluctuations from the incoming beam. 
-           We don’t typically account for them but potentially could.
-        """
-        from nexusformat.nexus import NXdata
-
+        #
+        # Median or mean: It may be best to try the median because of
+        # some image artifacts that arise due to crinkles in the
+        # upstream kapton tape windows causing some phase contrast
+        # images to appear on the detector.
+        #
+        # One thing that also may be useful in a future implementation
+        # is to do a brightfield adjustment on EACH frame of the tomo
+        # based on a ROI in the corner of the frame where there is no
+        # sample but there is the direct X-ray beam because there is
+        # frame to frame fluctuations from the incoming beam. We don’t
+        # typically account for them but potentially could.
         if tbf_stack.ndim == 2:
             tbf = tbf_stack
         elif tbf_stack.ndim == 3:
             tbf = np.median(tbf_stack, axis=0)
             del tbf_stack
         else:
-           raise ValueError(f'Invalid tbf_stack shape ({tbf_stacks.shape})')
+            raise RuntimeError(f'Invalid tbf_stack shape ({tbf_stack.shape})')
 
         # Subtract dark field
         if 'data' in reduced_data and 'dark_field' in reduced_data.data:
             tbf -= reduced_data.data.dark_field
         else:
-            self.logger.warning('Dark field unavailable')
+            self._logger.warning('Dark field unavailable')
 
         # Set any non-positive values to one
         # (avoid negative bright field values for spikes in dark field)
         tbf[tbf < 1] = 1
 
         # Plot bright field
-        if self.save_figs:
-            if self.galaxy_flag:
-                quick_imshow(tbf, title='bright field', path='tomo_reduce_plots', save_fig=True,
-                        save_only=True)
-            else:
-                quick_imshow(tbf, title='bright field', path=self.output_folder, save_fig=True,
-                        save_only=True)
+        if self._save_figs:
+            quick_imshow(
+                tbf, title='bright field', path=self._output_folder,
+                save_fig=True, save_only=True)
 
         # Add bright field to reduced data NXprocess
-        if 'data' not in reduced_data: 
+        if 'data' not in reduced_data:
             reduced_data.data = NXdata()
         reduced_data.data['bright_field'] = tbf
 
-        return(reduced_data)
+        return reduced_data
 
     def _set_detector_bounds(self, nxentry, reduced_data, img_x_bounds=None):
-        """Set vertical detector bounds for each image stack.
-        Right now the range is the same for each set in the image stack.
         """
-        from CHAP.common.models.map import get_scanparser, import_scanparser
+        Set vertical detector bounds for each image stack.Right now the
+        range is the same for each set in the image stack.
+        """
+        # Local modules
+        from CHAP.common.models.map import (
+            get_scanparser,
+            import_scanparser,
+        )
         from CHAP.common.utils.general import is_index_range
 
-        if self.test_mode:
-            return(tuple(self.test_config['img_x_bounds']))
+        if self._test_mode:
+            return tuple(self._test_config['img_x_bounds'])
 
         # Get the first tomography image and the reference heights
         image_key = nxentry.instrument.detector.get('image_key', None)
         if image_key and 'data' in nxentry.instrument.detector:
-            field_indices = [index for index, key in enumerate(image_key) if key == 0]
-            first_image = np.asarray(nxentry.instrument.detector.data[field_indices[0],:,:])
+            field_indices = [
+                index for index, key in enumerate(image_key) if key == 0]
+            first_image = np.asarray(
+                nxentry.instrument.detector.data[field_indices[0],:,:])
             theta = float(nxentry.sample.rotation_angle[field_indices[0]])
             z_translation_all = nxentry.sample.z_translation[field_indices]
             vertical_shifts = sorted(list(set(z_translation_all)))
             num_tomo_stacks = len(vertical_shifts)
         else:
-            import_scanparser(nxentry.instrument.source.attrs['station'],
-                    nxentry.instrument.source.attrs['experiment_type'])
+            import_scanparser(
+                nxentry.instrument.source.attrs['station'],
+                nxentry.instrument.source.attrs['experiment_type'])
             tomo_field_scans = nxentry.spec_scans.tomo_fields
             num_tomo_stacks = len(tomo_field_scans.keys())
             center_stack_index = int(num_tomo_stacks/2)
             detector_prefix = str(nxentry.instrument.detector.local_name)
             vertical_shifts = []
             for i, nxsubentry in enumerate(tomo_field_scans.items()):
                 scan_number = int(nxsubentry[0].split('_')[-1])
-                scanparser = get_scanparser(tomo_field_scans.attrs['spec_file'], scan_number)
-                image_offset = int(nxsubentry[1].instrument.detector.frame_start_number)
+                scanparser = get_scanparser(
+                    tomo_field_scans.attrs['spec_file'], scan_number)
+                image_offset = int(
+                    nxsubentry[1].instrument.detector.frame_start_number)
                 vertical_shifts.append(nxsubentry[1].sample.z_translation)
                 if i == center_stack_index:
-                    first_image = scanparser.get_detector_data(detector_prefix, image_offset)
+                    first_image = scanparser.get_detector_data(
+                        detector_prefix, image_offset)
                     theta = float(nxsubentry[1].sample.rotation_angle[0])
 
         # Select image bounds
-        title = f'tomography image at theta={round(theta, 2)+0}'
+        title = f'tomography image at theta = {round(theta, 2)+0}'
         if img_x_bounds is not None:
-            if not is_index_range(img_x_bounds, ge=0, le=first_image.shape[0]):
-                raise ValueError(f'Invalid parameter img_x_bounds ({img_x_bounds})')
-            #RV TODO make interactive upon request?
-            return(img_x_bounds)
+            if is_index_range(img_x_bounds, ge=0, le=first_image.shape[0]):
+                return img_x_bounds
+            if self._interactive:
+                self._logger.warning(
+                    f'Invalid parameter img_x_bounds ({img_x_bounds}), '
+                    + 'ignoring img_x_bounds')
+                img_x_bounds = None
+            else:
+                raise ValueError(
+                    f'Invalid parameter img_x_bounds ({img_x_bounds})')
         if nxentry.instrument.source.attrs['station'] in ('id1a3', 'id3a'):
             pixel_size = nxentry.instrument.detector.x_pixel_size
             # Try to get a fit from the bright field
             tbf = np.asarray(reduced_data.data.bright_field)
             tbf_shape = tbf.shape
             x_sum = np.sum(tbf, 1)
             x_sum_min = x_sum.min()
             x_sum_max = x_sum.max()
-            fit = Fit.fit_data(x_sum, 'rectangle', x=np.array(range(len(x_sum))), form='atan',
-                    guess=True)
+            fit = Fit.fit_data(
+                x_sum, 'rectangle', x=np.array(range(len(x_sum))),
+                form='atan', guess=True)
             parameters = fit.best_values
             x_low_fit = parameters.get('center1', None)
             x_upp_fit = parameters.get('center2', None)
             sig_low = parameters.get('sigma1', None)
             sig_upp = parameters.get('sigma2', None)
-            have_fit = fit.success and x_low_fit is not None and x_upp_fit is not None and \
-                    sig_low is not None and sig_upp is not None and \
-                    0 <= x_low_fit < x_upp_fit <= x_sum.size and \
-                    (sig_low+sig_upp)/(x_upp_fit-x_low_fit) < 0.1
+            have_fit = (fit.success and x_low_fit is not None
+                        and x_upp_fit is not None and sig_low is not None
+                        and sig_upp is not None
+                        and 0 <= x_low_fit < x_upp_fit <= x_sum.size
+                        and (sig_low+sig_upp) / (x_upp_fit-x_low_fit) < 0.1)
             if have_fit:
                 # Set a 5% margin on each side
-                margin = 0.05*(x_upp_fit-x_low_fit)
+                margin = 0.05 * (x_upp_fit-x_low_fit)
                 x_low_fit = max(0, x_low_fit-margin)
                 x_upp_fit = min(tbf_shape[0], x_upp_fit+margin)
             if num_tomo_stacks == 1:
                 if have_fit:
-                    # Set the default range to enclose the full fitted window
+                    # Set the default range to enclose the full fitted
+                    #     window
                     x_low = int(x_low_fit)
                     x_upp = int(x_upp_fit)
                 else:
-                    # Center a default range of 1 mm (RV: can we get this from the slits?)
-                    num_x_min = int((1.0-0.5*pixel_size)/pixel_size)
-                    x_low = int(0.5*(tbf_shape[0]-num_x_min))
+                    # Center a default range of 1 mm
+                    # RV can we get this from the slits?
+                    num_x_min = int((1.0 - 0.5*pixel_size) / pixel_size)
+                    x_low = int((tbf_shape[0]-num_x_min) / 2)
                     x_upp = x_low+num_x_min
             else:
                 # Get the default range from the reference heights
                 delta_z = vertical_shifts[1]-vertical_shifts[0]
                 for i in range(2, num_tomo_stacks):
-                    delta_z = min(delta_z, vertical_shifts[i]-vertical_shifts[i-1])
-                self.logger.debug(f'delta_z = {delta_z}')
-                num_x_min = int((delta_z-0.5*pixel_size)/pixel_size)
-                self.logger.debug(f'num_x_min = {num_x_min}')
+                    delta_z = min(
+                        delta_z, vertical_shifts[i]-vertical_shifts[i-1])
+                self._logger.debug(f'delta_z = {delta_z}')
+                num_x_min = int((delta_z - 0.5*pixel_size) / pixel_size)
+                self._logger.debug(f'num_x_min = {num_x_min}')
                 if num_x_min > tbf_shape[0]:
-                    self.logger.warning('Image bounds and pixel size prevent seamless stacking')
+                    self._logger.warning(
+                        'Image bounds and pixel size prevent seamless '
+                        + 'stacking')
                 if have_fit:
-                    # Center the default range relative to the fitted window
-                    x_low = int(0.5*(x_low_fit+x_upp_fit-num_x_min))
+                    # Center the default range relative to the fitted
+                    #     window
+                    x_low = int((x_low_fit+x_upp_fit-num_x_min) / 2)
                     x_upp = x_low+num_x_min
                 else:
                     # Center the default range
-                    x_low = int(0.5*(tbf_shape[0]-num_x_min))
+                    x_low = int((tbf_shape[0]-num_x_min) / 2)
                     x_upp = x_low+num_x_min
-            if self.galaxy_flag:
+            if not self._interactive:
                 img_x_bounds = (x_low, x_upp)
             else:
                 tmp = np.copy(tbf)
                 tmp_max = tmp.max()
                 tmp[x_low,:] = tmp_max
                 tmp[x_upp-1,:] = tmp_max
                 quick_imshow(tmp, title='bright field')
                 tmp = np.copy(first_image)
                 tmp_max = tmp.max()
                 tmp[x_low,:] = tmp_max
                 tmp[x_upp-1,:] = tmp_max
                 quick_imshow(tmp, title=title)
                 del tmp
-                quick_plot((range(x_sum.size), x_sum),
-                        ([x_low, x_low], [x_sum_min, x_sum_max], 'r-'),
-                        ([x_upp, x_upp], [x_sum_min, x_sum_max], 'r-'),
-                        title='sum over theta and y')
+                quick_plot(
+                    (range(x_sum.size), x_sum),
+                    ([x_low, x_low], [x_sum_min, x_sum_max], 'r-'),
+                    ([x_upp, x_upp], [x_sum_min, x_sum_max], 'r-'),
+                    title='sum over theta and y')
                 print(f'lower bound = {x_low} (inclusive)')
                 print(f'upper bound = {x_upp} (exclusive)]')
-                accept =  input_yesno('Accept these bounds (y/n)?', 'y')
+                accept = input_yesno('Accept these bounds (y/n)?', 'y')
                 clear_imshow('bright field')
                 clear_imshow(title)
                 clear_plot('sum over theta and y')
                 if accept:
                     img_x_bounds = (x_low, x_upp)
                 else:
                     while True:
-                        mask, img_x_bounds = draw_mask_1d(x_sum, title='select x data range',
-                                legend='sum over theta and y')
+                        _, img_x_bounds = draw_mask_1d(
+                            x_sum, title='select x data range',
+                            legend='sum over theta and y')
                         if len(img_x_bounds) == 1:
                             break
-                        else:
-                            print(f'Choose a single connected data range')
+                        print('Choose a single connected data range')
                     img_x_bounds = tuple(img_x_bounds[0])
-            if (num_tomo_stacks > 1 and img_x_bounds[1]-img_x_bounds[0]+1 < 
-                    int((delta_z-0.5*pixel_size)/pixel_size)):
-                self.logger.warning('Image bounds and pixel size prevent seamless stacking')
+            if (num_tomo_stacks > 1
+                    and (img_x_bounds[1]-img_x_bounds[0]+1)
+                    < int((delta_z - 0.5*pixel_size) / pixel_size)):
+                self._logger.warning(
+                    'Image bounds and pixel size prevent seamless stacking')
         else:
             if num_tomo_stacks > 1:
-                raise NotImplementedError('Selecting image bounds for multiple stacks on FMB')
+                raise NotImplementedError(
+                    'Selecting image bounds for multiple stacks on FMB')
             # For FMB: use the first tomography image to select range
-            # RV: revisit if they do tomography with multiple stacks
+            # RV revisit if they do tomography with multiple stacks
             x_sum = np.sum(first_image, 1)
             x_sum_min = x_sum.min()
             x_sum_max = x_sum.max()
-            if self.galaxy_flag:
+            if self._interactive:
+                print(
+                    'Select vertical data reduction range from first '
+                    + 'tomography image')
+                img_x_bounds = select_image_bounds(first_image, 0, title=title)
                 if img_x_bounds is None:
-                    img_x_bounds = (0, first_image.shape[0])
+                    raise RuntimeError('Unable to select image bounds')
             else:
-                print('Select vertical data reduction range from first tomography image')
-                img_x_bounds = select_image_bounds(first_image, 0, title=title)
                 if img_x_bounds is None:
-                    raise ValueError('Unable to select image bounds')
+                    self._logger.warning(
+                        'img_x_bounds unspecified, reduce data for entire '
+                        + 'detector range')
+                    img_x_bounds = (0, first_image.shape[0])
 
         # Plot results
-        if self.save_figs:
-            if self.galaxy_flag:
-                path = 'tomo_reduce_plots'
-            else:
-                path = self.output_folder
+        if self._save_figs:
             x_low = img_x_bounds[0]
             x_upp = img_x_bounds[1]
             tmp = np.copy(first_image)
             tmp_max = tmp.max()
             tmp[x_low,:] = tmp_max
             tmp[x_upp-1,:] = tmp_max
-            quick_imshow(tmp, title=title, path=path, save_fig=True, save_only=True)
-            quick_plot((range(x_sum.size), x_sum),
-                    ([x_low, x_low], [x_sum_min, x_sum_max], 'r-'),
-                    ([x_upp, x_upp], [x_sum_min, x_sum_max], 'r-'),
-                    title='sum over theta and y', path=path, save_fig=True, save_only=True)
+            quick_imshow(
+                tmp, title=title, path=self._output_folder, save_fig=True,
+                save_only=True)
+            quick_plot(
+                (range(x_sum.size), x_sum),
+                ([x_low, x_low], [x_sum_min, x_sum_max], 'r-'),
+                ([x_upp, x_upp], [x_sum_min, x_sum_max], 'r-'),
+                title='sum over theta and y', path=self._output_folder,
+                save_fig=True, save_only=True)
             del tmp
 
-        return(img_x_bounds)
+        return img_x_bounds
 
     def _set_zoom_or_skip(self):
-        """Set zoom and/or theta skip to reduce memory the requirement for the analysis.
         """
-#        if input_yesno('\nDo you want to zoom in to reduce memory requirement (y/n)?', 'n'):
-#            zoom_perc = input_int('    Enter zoom percentage', ge=1, le=100)
+        Set zoom and/or theta skip to reduce memory the requirement
+        for the analysis.
+        """
+#        if input_yesno(
+#                '\nDo you want to zoom in to reduce memory '
+#                + 'requirement (y/n)?', 'n'):
+#            zoom_perc = input_int(
+#                '    Enter zoom percentage', ge=1, le=100)
 #        else:
 #            zoom_perc = None
         zoom_perc = None
-#        if input_yesno('Do you want to skip thetas to reduce memory requirement (y/n)?', 'n'):
-#            num_theta_skip = input_int('    Enter the number skip theta interval', ge=0,
-#                    lt=num_theta)
+#        if input_yesno(
+#                'Do you want to skip thetas to reduce memory '
+#                + 'requirement (y/n)?', 'n'):
+#            num_theta_skip = input_int(
+#                '    Enter the number skip theta interval',
+#                ge=0, lt=num_theta)
 #        else:
 #            num_theta_skip = None
         num_theta_skip = None
-        self.logger.debug(f'zoom_perc = {zoom_perc}')
-        self.logger.debug(f'num_theta_skip = {num_theta_skip}')
+        self._logger.debug(f'zoom_perc = {zoom_perc}')
+        self._logger.debug(f'num_theta_skip = {num_theta_skip}')
 
-        return(zoom_perc, num_theta_skip)
+        return zoom_perc, num_theta_skip
 
     def _gen_tomo(self, nxentry, reduced_data):
-        """Generate tomography fields.
-        """
-        import numexpr as ne
-        import scipy.ndimage as spi
-
-        from CHAP.common.models.map import get_scanparser, import_scanparser
+        """Generate tomography fields."""
+        # Third party modules
+        from numexpr import evaluate
+        from scipy.ndimage import zoom
+
+        # Local modules
+        from CHAP.common.models.map import (
+            get_scanparser,
+            import_scanparser,
+        )
 
         # Get full bright field
         tbf = np.asarray(reduced_data.data.bright_field)
         tbf_shape = tbf.shape
 
         # Get image bounds
-        img_x_bounds = tuple(reduced_data.get('img_x_bounds', (0, tbf_shape[0])))
-        img_y_bounds = tuple(reduced_data.get('img_y_bounds', (0, tbf_shape[1])))
+        img_x_bounds = tuple(
+            reduced_data.get('img_x_bounds', (0, tbf_shape[0])))
+        img_y_bounds = tuple(
+            reduced_data.get('img_y_bounds', (0, tbf_shape[1])))
 
         # Get resized dark field
 #        if 'dark_field' in data:
-#            tbf = np.asarray(reduced_data.data.dark_field[
-#                    img_x_bounds[0]:img_x_bounds[1],img_y_bounds[0]:img_y_bounds[1]])
+#            tbf = np.asarray(
+#                reduced_data.data.dark_field[
+#                    img_x_bounds[0]:img_x_bounds[1],
+#                    img_y_bounds[0]:img_y_bounds[1]])
 #        else:
-#            self.logger.warning('Dark field unavailable')
+#            self._logger.warning('Dark field unavailable')
 #            tdf = None
         tdf = None
 
         # Resize bright field
-        if img_x_bounds != (0, tbf.shape[0]) or img_y_bounds != (0, tbf.shape[1]):
-            tbf = tbf[img_x_bounds[0]:img_x_bounds[1],img_y_bounds[0]:img_y_bounds[1]]
+        if (img_x_bounds != (0, tbf.shape[0])
+                or img_y_bounds != (0, tbf.shape[1])):
+            tbf = tbf[
+                img_x_bounds[0]:img_x_bounds[1],
+                img_y_bounds[0]:img_y_bounds[1]]
 
         # Get the tomography images
         image_key = nxentry.instrument.detector.get('image_key', None)
         if image_key and 'data' in nxentry.instrument.detector:
-            field_indices_all = [index for index, key in enumerate(image_key) if key == 0]
+            field_indices_all = [
+                index for index, key in enumerate(image_key) if key == 0]
             z_translation_all = nxentry.sample.z_translation[field_indices_all]
             z_translation_levels = sorted(list(set(z_translation_all)))
             num_tomo_stacks = len(z_translation_levels)
             tomo_stacks = num_tomo_stacks*[np.array([])]
             horizontal_shifts = []
             vertical_shifts = []
             thetas = None
             tomo_stacks = []
             for i, z_translation in enumerate(z_translation_levels):
-                field_indices = [field_indices_all[index]
-                        for index, z in enumerate(z_translation_all) if z == z_translation]
-                horizontal_shift = list(set(nxentry.sample.x_translation[field_indices]))
-                assert(len(horizontal_shift) == 1)
+                field_indices = [
+                    field_indices_all[index]
+                    for index, z in enumerate(z_translation_all)
+                    if z == z_translation]
+                horizontal_shift = list(
+                    set(nxentry.sample.x_translation[field_indices]))
+                assert len(horizontal_shift) == 1
                 horizontal_shifts += horizontal_shift
-                vertical_shift = list(set(nxentry.sample.z_translation[field_indices]))
-                assert(len(vertical_shift) == 1)
+                vertical_shift = list(
+                    set(nxentry.sample.z_translation[field_indices]))
+                assert len(vertical_shift) == 1
                 vertical_shifts += vertical_shift
-                sequence_numbers = nxentry.instrument.detector.sequence_number[field_indices]
+                sequence_numbers = nxentry.instrument.detector.sequence_number[
+                    field_indices]
                 if thetas is None:
-                    thetas = np.asarray(nxentry.sample.rotation_angle[field_indices]) \
-                             [sequence_numbers]
+                    thetas = np.asarray(
+                        nxentry.sample.rotation_angle[
+                            field_indices])[sequence_numbers]
                 else:
-                    assert(all(thetas[i] == nxentry.sample.rotation_angle[field_indices[index]]
-                            for i, index in enumerate(sequence_numbers)))
-                assert(list(set(sequence_numbers)) == [i for i in range(len(sequence_numbers))])
-                if list(sequence_numbers) == [i for i in range(len(sequence_numbers))]:
-                    tomo_stack = np.asarray(nxentry.instrument.detector.data[field_indices])
+                    assert all(
+                        thetas[i] == nxentry.sample.rotation_angle[
+                            field_indices[index]]
+                        for i, index in enumerate(sequence_numbers))
+                assert (list(set(sequence_numbers))
+                        == list(np.arange(0, (len(sequence_numbers)))))
+                if (list(sequence_numbers)
+                        == list(np.arange(0, (len(sequence_numbers))))):
+                    tomo_stack = np.asarray(
+                        nxentry.instrument.detector.data[field_indices])
                 else:
-                    raise ValueError('Unable to load the tomography images')
+                    raise RuntimeError('Unable to load the tomography images')
                 tomo_stacks.append(tomo_stack)
         else:
-            import_scanparser(nxentry.instrument.source.attrs['station'],
-                    nxentry.instrument.source.attrs['experiment_type'])
+            import_scanparser(
+                nxentry.instrument.source.attrs['station'],
+                nxentry.instrument.source.attrs['experiment_type'])
             tomo_field_scans = nxentry.spec_scans.tomo_fields
             num_tomo_stacks = len(tomo_field_scans.keys())
-            center_stack_index = int(num_tomo_stacks/2)
             detector_prefix = str(nxentry.instrument.detector.local_name)
             thetas = None
             tomo_stacks = []
             horizontal_shifts = []
             vertical_shifts = []
             for nxsubentry_name, nxsubentry in tomo_field_scans.items():
                 scan_number = int(nxsubentry_name.split('_')[-1])
-                scanparser = get_scanparser(tomo_field_scans.attrs['spec_file'], scan_number)
-                image_offset = int(nxsubentry.instrument.detector.frame_start_number)
+                scanparser = get_scanparser(
+                    tomo_field_scans.attrs['spec_file'], scan_number)
+                image_offset = int(
+                    nxsubentry.instrument.detector.frame_start_number)
                 if thetas is None:
                     thetas = np.asarray(nxsubentry.sample.rotation_angle)
                 num_image = len(thetas)
-                tomo_stacks.append(scanparser.get_detector_data(detector_prefix,
+                tomo_stacks.append(
+                    scanparser.get_detector_data(
+                        detector_prefix,
                         (image_offset, image_offset+num_image)))
                 horizontal_shifts.append(nxsubentry.sample.x_translation)
                 vertical_shifts.append(nxsubentry.sample.z_translation)
 
         reduced_tomo_stacks = []
-        if self.galaxy_flag:
-            path = 'tomo_reduce_plots'
-        else:
-            path = self.output_folder
         for i, tomo_stack in enumerate(tomo_stacks):
             # Resize the tomography images
-            # Right now the range is the same for each set in the image stack.
-            if img_x_bounds != (0, tbf.shape[0]) or img_y_bounds != (0, tbf.shape[1]):
-                t0 = time()
-                tomo_stack = tomo_stack[:,img_x_bounds[0]:img_x_bounds[1],
-                        img_y_bounds[0]:img_y_bounds[1]].astype('float64')
-                self.logger.debug(f'Resizing tomography images took {time()-t0:.2f} seconds')
+            # Right now the range is the same for each set in the stack
+            if (img_x_bounds != (0, tbf.shape[0])
+                    or img_y_bounds != (0, tbf.shape[1])):
+                tomo_stack = tomo_stack[
+                    :,img_x_bounds[0]:img_x_bounds[1],
+                    img_y_bounds[0]:img_y_bounds[1]].astype('float64')
 
             # Subtract dark field
             if tdf is not None:
-                t0 = time()
-                with set_numexpr_threads(self.num_core):
-                    ne.evaluate('tomo_stack-tdf', out=tomo_stack)
-                self.logger.debug(f'Subtracting dark field took {time()-t0:.2f} seconds')
+                try:
+                    with SetNumexprThreads(self._num_core):
+                        evaluate('tomo_stack-tdf', out=tomo_stack)
+                except TypeError as e:
+                    sys_exit(
+                        f'\nA {type(e).__name__} occured while subtracting '
+                        + 'the dark field with num_expr.evaluate()'
+                        + '\nTry reducing the detector range'
+                        + f'\n(currently img_x_bounds = {img_x_bounds}, and '
+                        + f'img_y_bounds = {img_y_bounds})\n')
 
             # Normalize
-            t0 = time()
-            with set_numexpr_threads(self.num_core):
-                ne.evaluate('tomo_stack/tbf', out=tomo_stack, truediv=True)
-            self.logger.debug(f'Normalizing took {time()-t0:.2f} seconds')
+            try:
+                with SetNumexprThreads(self._num_core):
+                    evaluate('tomo_stack/tbf', out=tomo_stack, truediv=True)
+            except TypeError as e:
+                sys_exit(
+                    f'\nA {type(e).__name__} occured while normalizing the '
+                    + 'tomography data with num_expr.evaluate()'
+                    + '\nTry reducing the detector range'
+                    + f'\n(currently img_x_bounds = {img_x_bounds}, and '
+                    + f'img_y_bounds = {img_y_bounds})\n')
 
             # Remove non-positive values and linearize data
-            t0 = time()
-            cutoff = 1.e-6
-            with set_numexpr_threads(self.num_core):
-                ne.evaluate('where(tomo_stack<cutoff, cutoff, tomo_stack)', out=tomo_stack)
-            with set_numexpr_threads(self.num_core):
-                ne.evaluate('-log(tomo_stack)', out=tomo_stack)
-            self.logger.debug('Removing non-positive values and linearizing data took '+
-                    f'{time()-t0:.2f} seconds')
+            # RV make input argument? cutoff = 1.e-6
+            with SetNumexprThreads(self._num_core):
+                evaluate(
+                    'where(tomo_stack < 1.e-6, 1.e-6, tomo_stack)',
+                    out=tomo_stack)
+            with SetNumexprThreads(self._num_core):
+                evaluate('-log(tomo_stack)', out=tomo_stack)
 
             # Get rid of nans/infs that may be introduced by normalization
-            t0 = time()
             np.where(np.isfinite(tomo_stack), tomo_stack, 0.)
-            self.logger.debug(f'Remove nans/infs took {time()-t0:.2f} seconds')
 
             # Downsize tomography stack to smaller size
-            # TODO use theta_skip as well
+            # RV use theta_skip as well
             tomo_stack = tomo_stack.astype('float32')
-            if not self.test_mode:
+            if not self._test_mode:
                 if len(tomo_stacks) == 1:
                     title = f'red fullres theta {round(thetas[0], 2)+0}'
                 else:
-                    title = f'red stack {i+1} fullres theta {round(thetas[0], 2)+0}'
-                quick_imshow(tomo_stack[0,:,:], title=title, path=path, save_fig=self.save_figs,
-                        save_only=self.save_only, block=self.block)
-#                if not self.block:
+                    title = f'red stack {i+1} fullres theta ' \
+                        + f'{round(thetas[0], 2)+0}'
+                quick_imshow(
+                    tomo_stack[0,:,:], title=title, path=self._output_folder,
+                    save_fig=self._save_figs, save_only=self._save_only,
+                    block=self._block)
+#                if not self._block:
 #                    clear_imshow(title)
-            if False and zoom_perc != 100:
+            zoom_perc = 100
+            if zoom_perc != 100:
                 t0 = time()
-                self.logger.debug(f'Zooming in ...')
+                self._logger.debug('Zooming in ...')
                 tomo_zoom_list = []
                 for j in range(tomo_stack.shape[0]):
-                    tomo_zoom = spi.zoom(tomo_stack[j,:,:], 0.01*zoom_perc)
+                    tomo_zoom = zoom(tomo_stack[j,:,:], 0.01*zoom_perc)
                     tomo_zoom_list.append(tomo_zoom)
-                tomo_stack = np.stack([tomo_zoom for tomo_zoom in tomo_zoom_list])
-                self.logger.debug(f'... done in {time()-t0:.2f} seconds')
-                self.logger.info(f'Zooming in took {time()-t0:.2f} seconds')
+                tomo_stack = np.stack(tomo_zoom_list)
+                self._logger.info(f'Zooming in took {time()-t0:.2f} seconds')
                 del tomo_zoom_list
-                if not self.test_mode:
-                    title = f'red stack {zoom_perc}p theta {round(thetas[0], 2)+0}'
-                    quick_imshow(tomo_stack[0,:,:], title=title, path=path, save_fig=self.save_figs,
-                            save_only=self.save_only, block=self.block)
-#                    if not self.block:
+                if not self._test_mode:
+                    title = f'red stack {zoom_perc}p theta ' \
+                        + f'{round(thetas[0], 2)+0}'
+                    quick_imshow(
+                        tomo_stack[0,:,:], title=title,
+                        path=self._output_folder, save_fig=self._save_figs,
+                        save_only=self._save_only, block=self._block)
+#                    if not self._block:
 #                        clear_imshow(title)
 
             # Save test data to file
-            if self.test_mode:
-#                row_index = int(tomo_stack.shape[0]/2)
-#                np.savetxt(f'{self.output_folder}/red_stack_{i+1}.txt', tomo_stack[row_index,:,:],
-#                        fmt='%.6e')
+            if self._test_mode:
                 row_index = int(tomo_stack.shape[1]/2)
-                np.savetxt(f'{self.output_folder}/red_stack_{i+1}.txt', tomo_stack[:,row_index,:],
-                        fmt='%.6e')
+                np.savetxt(
+                    f'{self._output_folder}/red_stack_{i+1}.txt',
+                    tomo_stack[:,row_index,:], fmt='%.6e')
 
             # Combine resized stacks
             reduced_tomo_stacks.append(tomo_stack)
 
         # Add tomo field info to reduced data NXprocess
         reduced_data['rotation_angle'] = thetas
         reduced_data['x_translation'] = np.asarray(horizontal_shifts)
         reduced_data['z_translation'] = np.asarray(vertical_shifts)
         reduced_data.data['tomo_fields'] = np.asarray(reduced_tomo_stacks)
 
         if tdf is not None:
             del tdf
         del tbf
 
-        return(reduced_data)
+        return reduced_data
 
-    def _find_center_one_plane(self, sinogram, row, thetas, eff_pixel_size, cross_sectional_dim,
-            path=None, tol=0.1, num_core=1):
-        """Find center for a single tomography plane.
-        """
-        import tomopy
+    def _find_center_one_plane(
+            self, sinogram, row, thetas, eff_pixel_size, cross_sectional_dim,
+            path=None, num_core=1):  # , tol=0.1):
+        """Find center for a single tomography plane."""
+        from tomopy import find_center_vo
 
         # Try automatic center finding routines for initial value
         # sinogram index order: theta,column
         # need column,theta for iradon, so take transpose
         sinogram = np.asarray(sinogram)
-        sinogram_T = sinogram.T
+        sinogram_t = sinogram.T
         center = sinogram.shape[1]/2
 
         # Try using Nghia Vo’s method
         t0 = time()
-        if num_core > num_core_tomopy_limit:
-            self.logger.debug(f'Running find_center_vo on {num_core_tomopy_limit} cores ...')
-            tomo_center = tomopy.find_center_vo(sinogram, ncore=num_core_tomopy_limit)
-        else:
-            self.logger.debug(f'Running find_center_vo on {num_core} cores ...')
-            tomo_center = tomopy.find_center_vo(sinogram, ncore=num_core)
-        self.logger.debug(f'... done in {time()-t0:.2f} seconds')
-        self.logger.info(f'Finding the center using Nghia Vo’s method took {time()-t0:.2f} seconds')
+        if num_core > NUM_CORE_TOMOPY_LIMIT:
+            self._logger.debug(
+                f'Running find_center_vo on {NUM_CORE_TOMOPY_LIMIT} cores ...')
+            tomo_center = find_center_vo(
+                sinogram, ncore=NUM_CORE_TOMOPY_LIMIT)
+        else:
+            tomo_center = find_center_vo(sinogram, ncore=num_core)
+        self._logger.info(
+            f'Finding center using Nghia Vo’s method took {time()-t0:.2f} '
+            + 'seconds')
         center_offset_vo = tomo_center-center
-        self.logger.info(f'Center at row {row} using Nghia Vo’s method = {center_offset_vo:.2f}')
+        self._logger.info(
+            f'Center at row {row} using Nghia Vo’s method = '
+            + f'{center_offset_vo:.2f}')
         t0 = time()
-        self.logger.debug(f'Running _reconstruct_one_plane on {self.num_core} cores ...')
-        recon_plane = self._reconstruct_one_plane(sinogram_T, tomo_center, thetas,
-                eff_pixel_size, cross_sectional_dim, False, num_core)
-        self.logger.debug(f'... done in {time()-t0:.2f} seconds')
-        self.logger.info(f'Reconstructing row {row} took {time()-t0:.2f} seconds')
+        recon_plane = self._reconstruct_one_plane(
+            sinogram_t, tomo_center, thetas, eff_pixel_size,
+            cross_sectional_dim, False, num_core)
+        self._logger.info(
+            f'Reconstructing row {row} took {time()-t0:.2f} seconds')
 
         title = f'edges row{row} center offset{center_offset_vo:.2f} Vo'
         self._plot_edges_one_plane(recon_plane, title, path=path)
 
         # Try using phase correlation method
-#        if input_yesno('Try finding center using phase correlation (y/n)?', 'n'):
+#        if input_yesno('
+#                Try finding center using phase correlation (y/n)?',
+#                'n'):
 #            t0 = time()
-#            self.logger.debug(f'Running find_center_pc ...')
-#            tomo_center = tomopy.find_center_pc(sinogram, sinogram, tol=0.1, rotc_guess=tomo_center)
+#            tomo_center = find_center_pc(
+#                sinogram, sinogram, tol=0.1, rotc_guess=tomo_center)
 #            error = 1.
 #            while error > tol:
 #                prev = tomo_center
-#                tomo_center = tomopy.find_center_pc(sinogram, sinogram, tol=tol,
-#                        rotc_guess=tomo_center)
+#                tomo_center = find_center_pc(
+#                    sinogram, sinogram, tol=tol, rotc_guess=tomo_center)
 #                error = np.abs(tomo_center-prev)
-#            self.logger.debug(f'... done in {time()-t0:.2f} seconds')
-#            self.logger.info('Finding the center using the phase correlation method took '+
-#                    f'{time()-t0:.2f} seconds')
+#            self._logger.info(
+#                'Finding center using the phase correlation method '
+#                + f'took {time()-t0:.2f} seconds')
 #            center_offset = tomo_center-center
-#            print(f'Center at row {row} using phase correlation = {center_offset:.2f}')
+#            print(
+#                f'Center at row {row} using phase correlation = '
+#                + f'{center_offset:.2f}')
 #            t0 = time()
-#            self.logger.debug(f'Running _reconstruct_one_plane on {self.num_core} cores ...')
-#            recon_plane = self._reconstruct_one_plane(sinogram_T, tomo_center, thetas,
-#                    eff_pixel_size, cross_sectional_dim, False, num_core)
-#            self.logger.debug(f'... done in {time()-t0:.2f} seconds')
-#            self.logger.info(f'Reconstructing row {row} took {time()-t0:.2f} seconds')
+#            recon_plane = self._reconstruct_one_plane(
+#                sinogram_t, tomo_center, thetas, eff_pixel_size,
+#                cross_sectional_dim, False, num_core)
+#            self._logger.info(
+#                f'Reconstructing row {row} took {time()-t0:.2f} seconds')
 #
-#            title = f'edges row{row} center_offset{center_offset:.2f} PC'
+#            title = \
+#                f'edges row{row} center_offset{center_offset:.2f} PC'
 #            self._plot_edges_one_plane(recon_plane, title, path=path)
 
         # Select center location
-#        if input_yesno('Accept a center location (y) or continue search (n)?', 'y'):
-        if True:
-#            center_offset = input_num('    Enter chosen center offset', ge=-center, le=center,
-#                    default=center_offset_vo)
-            center_offset = center_offset_vo
-            del sinogram_T
-            del recon_plane
-            return float(center_offset)
-
-        # perform center finding search
-        while True:
-            center_offset_low = input_int('\nEnter lower bound for center offset', ge=-center,
-                    le=center)
-            center_offset_upp = input_int('Enter upper bound for center offset',
-                    ge=center_offset_low, le=center)
-            if center_offset_upp == center_offset_low:
-                center_offset_step = 1
-            else:
-                center_offset_step = input_int('Enter step size for center offset search', ge=1,
-                        le=center_offset_upp-center_offset_low)
-            num_center_offset = 1+int((center_offset_upp-center_offset_low)/center_offset_step)
-            center_offsets = np.linspace(center_offset_low, center_offset_upp, num_center_offset)
-            for center_offset in center_offsets:
-                if center_offset == center_offset_vo:
-                    continue
-                t0 = time()
-                self.logger.debug(f'Running _reconstruct_one_plane on {num_core} cores ...')
-                recon_plane = self._reconstruct_one_plane(sinogram_T, center_offset+center, thetas,
-                        eff_pixel_size, cross_sectional_dim, False, num_core)
-                self.logger.debug(f'... done in {time()-t0:.2f} seconds')
-                self.logger.info(f'Reconstructing center_offset {center_offset} took '+
-                        f'{time()-t0:.2f} seconds')
-                title = f'edges row{row} center_offset{center_offset:.2f}'
-                self._plot_edges_one_plane(recon_plane, title, path=path)
-            if input_int('\nContinue (0) or end the search (1)', ge=0, le=1):
-                break
+#        if input_yesno(
+#            'Accept a center location (y) or continue search (n)?',
+#            'y'):
+#            center_offset = input_num('    Enter chosen center offset',
+#                    ge=-center, le=center, default=center_offset_vo)
+#            return float(center_offset)
+
+        # Perform center finding search
+#        while True:
+#            center_offset_low = input_int(
+#                '\nEnter lower bound for center offset', ge=-center,le=center)
+#            center_offset_upp = input_int(
+#                'Enter upper bound for center offset', ge=center_offset_low,
+#                le=center)
+#            if center_offset_upp == center_offset_low:
+#                center_offset_step = 1
+#            else:
+#                center_offset_step = input_int(
+#                    'Enter step size for center offset search', ge=1,
+#                        le=center_offset_upp-center_offset_low)
+#            num_center_offset = 1 + int(
+#                (center_offset_upp-center_offset_low) / center_offset_step)
+#            center_offsets = np.linspace(
+#                center_offset_low, center_offset_upp, num_center_offset)
+#            for center_offset in center_offsets:
+#                if center_offset == center_offset_vo:
+#                    continue
+#                t0 = time()
+#                recon_plane = self._reconstruct_one_plane(
+#                    sinogram_t, center_offset+center, thetas, eff_pixel_size,
+#                    cross_sectional_dim, False, num_core)
+#                self._logger.info(
+#                    f'Reconstructing center_offset {center_offset} took '
+#                    + 'f{time()-t0:.2f} seconds')
+#                title = f'edges row{row} center_offset{center_offset:.2f}'
+#                self._plot_edges_one_plane(recon_plane, title, path=path)
+#            if input_int('\nContinue (0) or end the search (1)', ge=0, le=1):
+#                break
 
-        del sinogram_T
+        del sinogram_t
         del recon_plane
-        center_offset = input_num('    Enter chosen center offset', ge=-center, le=center)
+#        center_offset = input_num(
+#            '    Enter chosen center offset', ge=-center, le=center)
+        center_offset = center_offset_vo
+
         return float(center_offset)
 
-    def _reconstruct_one_plane(self, tomo_plane_T, center, thetas, eff_pixel_size,
+    def _reconstruct_one_plane(
+            self, tomo_plane_t, center, thetas, eff_pixel_size,
             cross_sectional_dim, plot_sinogram=True, num_core=1):
-        """Invert the sinogram for a single tomography plane.
-        """
-        import scipy.ndimage as spi
+        """Invert the sinogram for a single tomography plane."""
+        from scipy.ndimage import gaussian_filter
         from skimage.transform import iradon
-        import tomopy
+        from tomopy import misc
 
-        # tomo_plane_T index order: column,theta
-        assert(0 <= center < tomo_plane_T.shape[0])
-        center_offset = center-tomo_plane_T.shape[0]/2
-        two_offset = 2*int(np.round(center_offset))
+        # tomo_plane_t index order: column,theta
+        assert 0 <= center < tomo_plane_t.shape[0]
+        center_offset = center-tomo_plane_t.shape[0]/2
+        two_offset = 2 * int(np.round(center_offset))
         two_offset_abs = np.abs(two_offset)
-        max_rad = int(0.55*(cross_sectional_dim/eff_pixel_size)) # 10% slack to avoid edge effects
-        if max_rad > 0.5*tomo_plane_T.shape[0]:
-            max_rad = 0.5*tomo_plane_T.shape[0]
-        dist_from_edge = max(1, int(np.floor((tomo_plane_T.shape[0]-two_offset_abs)/2.)-max_rad))
+        # Add 10% slack to max_rad to avoid edge effects
+        max_rad = int(0.55 * (cross_sectional_dim/eff_pixel_size))
+        if max_rad > 0.5*tomo_plane_t.shape[0]:
+            max_rad = 0.5*tomo_plane_t.shape[0]
+        dist_from_edge = max(1, int(np.floor(
+            (tomo_plane_t.shape[0] - two_offset_abs) / 2.0) - max_rad))
         if two_offset >= 0:
-            self.logger.debug(f'sinogram range = [{two_offset+dist_from_edge}, {-dist_from_edge}]')
-            sinogram = tomo_plane_T[two_offset+dist_from_edge:-dist_from_edge,:]
-        else:
-            self.logger.debug(f'sinogram range = [{dist_from_edge}, {two_offset-dist_from_edge}]')
-            sinogram = tomo_plane_T[dist_from_edge:two_offset-dist_from_edge,:]
-        if not self.galaxy_flag and plot_sinogram:
-            quick_imshow(sinogram.T, f'sinogram center offset{center_offset:.2f}', aspect='auto',
-                    path=self.output_folder, save_fig=self.save_figs, save_only=self.save_only,
-                    block=self.block)
+            self._logger.debug(
+                f'sinogram range = [{two_offset+dist_from_edge}, '
+                + f'{-dist_from_edge}]')
+            sinogram = tomo_plane_t[
+                two_offset+dist_from_edge:-dist_from_edge,:]
+        else:
+            self._logger.debug(
+                f'sinogram range = [{dist_from_edge}, '
+                + f'{two_offset-dist_from_edge}]')
+            sinogram = tomo_plane_t[dist_from_edge:two_offset-dist_from_edge,:]
+        if plot_sinogram:
+            quick_imshow(
+                sinogram.T, f'sinogram center offset{center_offset:.2f}',
+                aspect='auto', path=self._output_folder,
+                save_fig=self._save_figs, save_only=self._save_only,
+                block=self._block)
 
         # Inverting sinogram
         t0 = time()
         recon_sinogram = iradon(sinogram, theta=thetas, circle=True)
-        self.logger.debug(f'Inverting sinogram took {time()-t0:.2f} seconds')
+        self._logger.info(f'Inverting sinogram took {time()-t0:.2f} seconds')
         del sinogram
 
         # Performing Gaussian filtering and removing ring artifacts
-        recon_parameters = None#self.config.get('recon_parameters')
+        recon_parameters = None  # self._config.get('recon_parameters')
         if recon_parameters is None:
             sigma = 1.0
             ring_width = 15
         else:
             sigma = recon_parameters.get('gaussian_sigma', 1.0)
             if not is_num(sigma, ge=0.0):
-                self.logger.warning(f'Invalid gaussian_sigma ({sigma}) in _reconstruct_one_plane, '+
-                        'set to a default value of 1.0')
+                self._logger.warning(
+                    f'Invalid gaussian_sigma ({sigma}) in '
+                    + '_reconstruct_one_plane, set to a default of 1.0')
                 sigma = 1.0
             ring_width = recon_parameters.get('ring_width', 15)
             if not isinstance(ring_width, int) or ring_width < 0:
-                self.logger.warning(f'Invalid ring_width ({ring_width}) in '+
-                        '_reconstruct_one_plane, set to a default value of 15')
+                self._logger.warning(
+                    f'Invalid ring_width ({ring_width}) in '
+                    + '_reconstruct_one_plane, set to a default of 15')
                 ring_width = 15
-        t0 = time()
-        recon_sinogram = spi.gaussian_filter(recon_sinogram, sigma, mode='nearest')
+        recon_sinogram = gaussian_filter(
+            recon_sinogram, sigma, mode='nearest')
         recon_clean = np.expand_dims(recon_sinogram, axis=0)
         del recon_sinogram
-        recon_clean = tomopy.misc.corr.remove_ring(recon_clean, rwidth=ring_width, ncore=num_core)
-        self.logger.debug(f'Filtering and removing ring artifacts took {time()-t0:.2f} seconds')
+        recon_clean = misc.corr.remove_ring(
+            recon_clean, rwidth=ring_width, ncore=num_core)
 
         return recon_clean
 
     def _plot_edges_one_plane(self, recon_plane, title, path=None):
+        """
+        Create an "edges plot" for a singled reconstructed tomography
+        data plane.
+        """
         from skimage.restoration import denoise_tv_chambolle
 
-        vis_parameters = None#self.config.get('vis_parameters')
+        vis_parameters = None  # self._config.get('vis_parameters')
         if vis_parameters is None:
             weight = 0.1
         else:
             weight = vis_parameters.get('denoise_weight', 0.1)
             if not is_num(weight, ge=0.0):
-                self.logger.warning(f'Invalid weight ({weight}) in _plot_edges_one_plane, '+
-                        'set to a default value of 0.1')
+                self._logger.warning(
+                    f'Invalid weight ({weight}) in _plot_edges_one_plane, '
+                    + 'set to a default of 0.1')
                 weight = 0.1
         edges = denoise_tv_chambolle(recon_plane, weight=weight)
         vmax = np.max(edges[0,:,:])
         vmin = -vmax
         if path is None:
-            path = self.output_folder
-        quick_imshow(edges[0,:,:], f'{title} coolwarm', path=path, cmap='coolwarm',
-                save_fig=self.save_figs, save_only=self.save_only, block=self.block)
-        quick_imshow(edges[0,:,:], f'{title} gray', path=path, cmap='gray', vmin=vmin, vmax=vmax,
-                save_fig=self.save_figs, save_only=self.save_only, block=self.block)
+            path = self._output_folder
+        quick_imshow(
+            edges[0,:,:], f'{title} coolwarm', path=path, cmap='coolwarm',
+            save_fig=self._save_figs, save_only=self._save_only,
+            block=self._block)
+        quick_imshow(
+            edges[0,:,:], f'{title} gray', path=path, cmap='gray', vmin=vmin,
+            vmax=vmax, save_fig=self._save_figs, save_only=self._save_only,
+            block=self._block)
         del edges
 
-    def _reconstruct_one_tomo_stack(self, tomo_stack, thetas, center_offsets=[], num_core=1,
+    def _reconstruct_one_tomo_stack(
+            self, tomo_stack, thetas, center_offsets=None, num_core=1,
             algorithm='gridrec'):
-        """Reconstruct a single tomography stack.
-        """
-        import tomopy
+        """Reconstruct a single tomography stack."""
+        # Third party modules
+        from tomopy import (
+            astra,
+            misc,
+            prep,
+            recon,
+        )
 
         # tomo_stack order: row,theta,column
-        # input thetas must be in degrees 
-        # centers_offset: tomography axis shift in pixels relative to column center
+        # input thetas must be in degrees
+        # centers_offset: tomography axis shift in pixels relative
+        #     to column center
         # RV should we remove stripes?
         # https://tomopy.readthedocs.io/en/latest/api/tomopy.prep.stripe.html
         # RV should we remove rings?
         # https://tomopy.readthedocs.io/en/latest/api/tomopy.misc.corr.html
-        # RV: Add an option to do (extra) secondary iterations later or to do some sort of convergence test?
-        if not len(center_offsets):
+        # RV add an option to do (extra) secondary iterations later or
+        #     to do some sort of convergence test?
+        if center_offsets is None:
             centers = np.zeros((tomo_stack.shape[0]))
         elif len(center_offsets) == 2:
-            centers = np.linspace(center_offsets[0], center_offsets[1], tomo_stack.shape[0])
+            centers = np.linspace(
+                center_offsets[0], center_offsets[1], tomo_stack.shape[0])
         else:
             if center_offsets.size != tomo_stack.shape[0]:
-                raise ValueError('center_offsets dimension mismatch in reconstruct_one_tomo_stack')
+                raise RuntimeError(
+                    'center_offsets dimension mismatch in '
+                    + 'reconstruct_one_tomo_stack')
             centers = center_offsets
         centers += tomo_stack.shape[2]/2
 
         # Get reconstruction parameters
-        recon_parameters = None#self.config.get('recon_parameters')
+        recon_parameters = None  # self._config.get('recon_parameters')
         if recon_parameters is None:
             sigma = 2.0
             secondary_iters = 0
             ring_width = 15
         else:
             sigma = recon_parameters.get('stripe_fw_sigma', 2.0)
             if not is_num(sigma, ge=0):
-                self.logger.warning(f'Invalid stripe_fw_sigma ({sigma}) in '+
-                        '_reconstruct_one_tomo_stack, set to a default value of 2.0')
+                self._logger.warning(
+                    f'Invalid stripe_fw_sigma ({sigma}) in '
+                    + '_reconstruct_one_tomo_stack, set to a default of 2.0')
                 ring_width = 15
             secondary_iters = recon_parameters.get('secondary_iters', 0)
             if not isinstance(secondary_iters, int) or secondary_iters < 0:
-                self.logger.warning(f'Invalid secondary_iters ({secondary_iters}) in '+
-                        '_reconstruct_one_tomo_stack, set to a default value of 0 (skip them)')
+                self._logger.warning(
+                    f'Invalid secondary_iters ({secondary_iters}) in '
+                    + '_reconstruct_one_tomo_stack, set to a default of 0 '
+                    + '(i.e., skip them)')
                 ring_width = 0
             ring_width = recon_parameters.get('ring_width', 15)
             if not isinstance(ring_width, int) or ring_width < 0:
-                self.logger.warning(f'Invalid ring_width ({ring_width}) in '+
-                        '_reconstruct_one_plane, set to a default value of 15')
+                self._logger.warning(
+                    f'Invalid ring_width ({ring_width}) in '
+                    + '_reconstruct_one_plane, set to a default of 15')
                 ring_width = 15
 
         # Remove horizontal stripe
-        t0 = time()
-        if num_core > num_core_tomopy_limit:
-            self.logger.debug('Running remove_stripe_fw on {num_core_tomopy_limit} cores ...')
-            tomo_stack = tomopy.prep.stripe.remove_stripe_fw(tomo_stack, sigma=sigma,
-                    ncore=num_core_tomopy_limit)
-        else:
-            self.logger.debug(f'Running remove_stripe_fw on {num_core} cores ...')
-            tomo_stack = tomopy.prep.stripe.remove_stripe_fw(tomo_stack, sigma=sigma,
-                    ncore=num_core)
-        self.logger.debug(f'... tomopy.prep.stripe.remove_stripe_fw took {time()-t0:.2f} seconds')
+        if num_core > NUM_CORE_TOMOPY_LIMIT:
+            tomo_stack = prep.stripe.remove_stripe_fw(
+                tomo_stack, sigma=sigma, ncore=NUM_CORE_TOMOPY_LIMIT)
+        else:
+            tomo_stack = prep.stripe.remove_stripe_fw(
+                tomo_stack, sigma=sigma, ncore=num_core)
 
         # Perform initial image reconstruction
-        self.logger.debug('Performing initial image reconstruction')
+        self._logger.debug('Performing initial image reconstruction')
         t0 = time()
-        self.logger.debug(f'Running recon on {num_core} cores ...')
-        tomo_recon_stack = tomopy.recon(tomo_stack, np.radians(thetas), centers,
-                sinogram_order=True, algorithm=algorithm, ncore=num_core)
-        self.logger.debug(f'... done in {time()-t0:.2f} seconds')
-        self.logger.info(f'Performing initial image reconstruction took {time()-t0:.2f} seconds')
+        tomo_recon_stack = recon(
+            tomo_stack, np.radians(thetas), centers, sinogram_order=True,
+            algorithm=algorithm, ncore=num_core)
+        self._logger.info(
+            f'Performing initial image reconstruction took {time()-t0:.2f} '
+            + 'seconds')
 
         # Run optional secondary iterations
         if secondary_iters > 0:
-            self.logger.debug(f'Running {secondary_iters} secondary iterations')
-            #options = {'method':'SIRT_CUDA', 'proj_type':'cuda', 'num_iter':secondary_iters}
-            #RV: doesn't work for me:
-            #"Error: CUDA error 803: system has unsupported display driver/cuda driver combination."
-            #options = {'method':'SIRT', 'proj_type':'linear', 'MinConstraint': 0, 'num_iter':secondary_iters}
-            #SIRT did not finish while running overnight
-            #options = {'method':'SART', 'proj_type':'linear', 'num_iter':secondary_iters}
-            options = {'method':'SART', 'proj_type':'linear', 'MinConstraint': 0,
-                    'num_iter':secondary_iters}
+            self._logger.debug(
+                'Running {secondary_iters} secondary iterations')
+#            options = {
+#                'method': 'SIRT_CUDA',
+#                'proj_type': 'cuda',
+#                'num_iter': secondary_iters
+#            }
+# RV doesn't work for me:
+# "Error: CUDA error 803: system has unsupported display driver/cuda driver
+#     combination."
+#            options = {
+#                'method': 'SIRT',
+#                'proj_type': 'linear',
+#                'MinConstraint': 0,
+#                'num_iter':secondary_iters
+#            }
+# SIRT did not finish while running overnight
+#            options = {
+#                'method': 'SART',
+#                'proj_type': 'linear',
+#                'num_iter':secondary_iters
+#            }
+            options = {
+                'method': 'SART',
+                'proj_type': 'linear',
+                'MinConstraint': 0,
+                'num_iter': secondary_iters,
+            }
             t0 = time()
-            self.logger.debug(f'Running recon on {num_core} cores ...')
-            tomo_recon_stack  = tomopy.recon(tomo_stack, np.radians(thetas), centers,
-                    init_recon=tomo_recon_stack, options=options, sinogram_order=True,
-                    algorithm=tomopy.astra, ncore=num_core)
-            self.logger.debug(f'... done in {time()-t0:.2f} seconds')
-            self.logger.info(f'Performing secondary iterations took {time()-t0:.2f} seconds')
+            tomo_recon_stack = recon(
+                tomo_stack, np.radians(thetas), centers,
+                init_recon=tomo_recon_stack, options=options,
+                sinogram_order=True, algorithm=astra, ncore=num_core)
+            self._logger.info(
+                f'Performing secondary iterations took {time()-t0:.2f} '
+                + 'seconds')
 
         # Remove ring artifacts
-        t0 = time()
-        tomopy.misc.corr.remove_ring(tomo_recon_stack, rwidth=ring_width, out=tomo_recon_stack,
-                ncore=num_core)
-        self.logger.debug(f'Removing ring artifacts took {time()-t0:.2f} seconds')
+        misc.corr.remove_ring(
+            tomo_recon_stack, rwidth=ring_width, out=tomo_recon_stack,
+            ncore=num_core)
 
         return tomo_recon_stack
 
-    def _resize_reconstructed_data(self, data, x_bounds=None, y_bounds=None, z_bounds=None,
+    def _resize_reconstructed_data(
+            self, data, x_bounds=None, y_bounds=None, z_bounds=None,
             z_only=False):
-        """Resize the reconstructed tomography data.
-        """
+        """Resize the reconstructed tomography data."""
         # Data order: row(z),x,y or stack,row(z),x,y
         if isinstance(data, list):
             for stack in data:
-                assert(stack.ndim == 3)
+                assert stack.ndim == 3
             num_tomo_stacks = len(data)
             tomo_recon_stacks = data
         else:
-            assert(data.ndim == 3)
+            assert data.ndim == 3
             num_tomo_stacks = 1
             tomo_recon_stacks = [data]
 
         if x_bounds == (-1, -1):
             x_bounds = None
         elif not z_only and x_bounds is None:
             # Selecting x bounds (in yz-plane)
             tomosum = 0
-            [tomosum := tomosum+np.sum(tomo_recon_stacks[i], axis=(0,2))
-                    for i in range(num_tomo_stacks)]
-            select_x_bounds = input_yesno('\nDo you want to change the image x-bounds (y/n)?', 'y')
+            for i in range(num_tomo_stacks):
+                tomosum = tomosum + np.sum(tomo_recon_stacks[i], axis=(0,2))
+            select_x_bounds = input_yesno(
+                '\nDo you want to change the image x-bounds (y/n)?', 'y')
             if not select_x_bounds:
                 x_bounds = None
             else:
                 accept = False
                 index_ranges = None
                 while not accept:
-                    mask, x_bounds = draw_mask_1d(tomosum, current_index_ranges=index_ranges,
-                            title='select x data range', legend='recon stack sum yz')
+                    _, x_bounds = draw_mask_1d(
+                        tomosum, current_index_ranges=index_ranges,
+                        title='select x data range',
+                        legend='recon stack sum yz')
                     while len(x_bounds) != 1:
                         print('Please select exactly one continuous range')
-                        mask, x_bounds = draw_mask_1d(tomosum, title='select x data range',
-                                legend='recon stack sum yz')
+                        _, x_bounds = draw_mask_1d(
+                            tomosum, title='select x data range',
+                            legend='recon stack sum yz')
                     x_bounds = x_bounds[0]
                     accept = True
-            self.logger.debug(f'x_bounds = {x_bounds}')
+            self._logger.debug(f'x_bounds = {x_bounds}')
 
         if y_bounds == (-1, -1):
             y_bounds = None
         elif not z_only and y_bounds is None:
             # Selecting y bounds (in xz-plane)
             tomosum = 0
-            [tomosum := tomosum+np.sum(tomo_recon_stacks[i], axis=(0,1))
-                    for i in range(num_tomo_stacks)]
-            select_y_bounds = input_yesno('\nDo you want to change the image y-bounds (y/n)?', 'y')
+            for i in range(num_tomo_stacks):
+                tomosum = tomosum + np.sum(tomo_recon_stacks[i], axis=(0,1))
+            select_y_bounds = input_yesno(
+                '\nDo you want to change the image y-bounds (y/n)?', 'y')
             if not select_y_bounds:
                 y_bounds = None
             else:
                 accept = False
                 index_ranges = None
                 while not accept:
-                    mask, y_bounds = draw_mask_1d(tomosum, current_index_ranges=index_ranges,
-                            title='select x data range', legend='recon stack sum xz')
+                    _, y_bounds = draw_mask_1d(
+                        tomosum, current_index_ranges=index_ranges,
+                        title='select x data range',
+                        legend='recon stack sum xz')
                     while len(y_bounds) != 1:
                         print('Please select exactly one continuous range')
-                        mask, y_bounds = draw_mask_1d(tomosum, title='select x data range',
-                                legend='recon stack sum xz')
+                        _, y_bounds = draw_mask_1d(
+                            tomosum, title='select x data range',
+                            legend='recon stack sum xz')
                     y_bounds = y_bounds[0]
                     accept = True
-            self.logger.debug(f'y_bounds = {y_bounds}')
+            self._logger.debug(f'y_bounds = {y_bounds}')
 
-        # Selecting z bounds (in xy-plane) (only valid for a single image stack)
+        # Selecting z bounds (in xy-plane)
+        # (only valid for a single image stack)
         if z_bounds == (-1, -1):
             z_bounds = None
         elif z_bounds is None and num_tomo_stacks != 1:
             tomosum = 0
-            [tomosum := tomosum+np.sum(tomo_recon_stacks[i], axis=(1,2))
-                    for i in range(num_tomo_stacks)]
-            select_z_bounds = input_yesno('Do you want to change the image z-bounds (y/n)?', 'n')
+            for i in range(num_tomo_stacks):
+                tomosum = tomosum + np.sum(tomo_recon_stacks[i], axis=(1,2))
+            select_z_bounds = input_yesno(
+                'Do you want to change the image z-bounds (y/n)?', 'n')
             if not select_z_bounds:
                 z_bounds = None
             else:
                 accept = False
                 index_ranges = None
                 while not accept:
-                    mask, z_bounds = draw_mask_1d(tomosum, current_index_ranges=index_ranges,
-                            title='select x data range', legend='recon stack sum xy')
+                    _, z_bounds = draw_mask_1d(
+                        tomosum, current_index_ranges=index_ranges,
+                        title='select x data range',
+                        legend='recon stack sum xy')
                     while len(z_bounds) != 1:
                         print('Please select exactly one continuous range')
-                        mask, z_bounds = draw_mask_1d(tomosum, title='select x data range',
-                                legend='recon stack sum xy')
+                        _, z_bounds = draw_mask_1d(
+                            tomosum, title='select x data range',
+                            legend='recon stack sum xy')
                     z_bounds = z_bounds[0]
                     accept = True
-            self.logger.debug(f'z_bounds = {z_bounds}')
+            self._logger.debug(f'z_bounds = {z_bounds}')
 
-        return(x_bounds, y_bounds, z_bounds)
+        return x_bounds, y_bounds, z_bounds
 
 
 if __name__ == '__main__':
-    from CHAP.processor import main
     main()
-
```

### Comparing `ChessAnalysisPipeline-0.0.5/CHAP/writer.py` & `ChessAnalysisPipeline-0.0.6/CHAP/writer.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,91 +3,97 @@
 File       : writer.py
 Author     : Valentin Kuznetsov <vkuznet AT gmail dot com>
 Description: generic Writer module
 """
 
 # system modules
 import argparse
-import json
+from inspect import getfullargspec
 import logging
-import os
-import sys
+from sys import modules
 from time import time
 
-# local modules
-# from pipeline import PipelineObject
 
 class Writer():
-    """
-    Writer represent generic file writer
-    """
+    """Writer represent generic file writer"""
 
     def __init__(self):
-        """
-        Constructor of Writer class
-        """
+        """Constructor of Writer class"""
         self.__name__ = self.__class__.__name__
         self.logger = logging.getLogger(self.__name__)
         self.logger.propagate = False
 
     def write(self, data, filename, **_write_kwargs):
-        """
-        write API
+        """write API
 
         :param filename: Name of file to write to
         :param data: data to write to file
         :return: data written to file
         """
 
         t0 = time()
-        self.logger.info(f'Executing "write" with filename={filename}, type(data)={type(data)}, kwargs={_write_kwargs}')
+        self.logger.info(f'Executing "write" with filename={filename}, '
+                         f'type(data)={type(data)}, kwargs={_write_kwargs}')
+
+        _valid_write_args = {}
+        allowed_args = getfullargspec(self._write).args \
+            + getfullargspec(self._write).kwonlyargs
+        for k, v in _write_kwargs.items():
+            if k in allowed_args:
+                _valid_write_args[k] = v
+            else:
+                self.logger.warning(f'Ignoring invalid arg to _write: {k}')
 
-        data = self._write(data, filename, **_write_kwargs)
+        data = self._write(data, filename, **_valid_write_args)
 
         self.logger.info(f'Finished "write" in {time()-t0:.3f} seconds\n')
 
-        return(data)
+        return data
 
     def _write(self, data, filename):
         with open(filename, 'a') as file:
             file.write(data)
-        return(data)
+        return data
+
 
 class OptionParser():
-        '''User based option parser'''
-        def __init__(self):
-            self.parser = argparse.ArgumentParser(prog='PROG')
-            self.parser.add_argument(
-                '--data', action='store',
-                dest='data', default='', help='Input data')
-            self.parser.add_argument(
-                '--filename', action='store',
-                        dest='filename', default='', help='Output file')
-            self.parser.add_argument(
-                '--writer', action='store',
-                dest='writer', default='Writer', help='Writer class name')
-            self.parser.add_argument(
-                '--log-level', choices=logging._nameToLevel.keys(),
+    """User based option parser"""
+    def __init__(self):
+        self.parser = argparse.ArgumentParser(prog='PROG')
+        self.parser.add_argument(
+            '--data', action='store',
+            dest='data', default='', help='Input data')
+        self.parser.add_argument(
+            '--filename', action='store',
+            dest='filename', default='', help='Output file')
+        self.parser.add_argument(
+            '--writer', action='store',
+            dest='writer', default='Writer', help='Writer class name')
+        self.parser.add_argument(
+            '--log-level', choices=logging._nameToLevel.keys(),
             dest='log_level', default='INFO', help='logging level')
 
+
 def main(opt_parser=OptionParser):
-    '''Main function'''
+    """Main function"""
 
-    optmgr  = opt_parser()
+    optmgr = opt_parser()
     opts = optmgr.parser.parse_args()
-    clsName = opts.writer
+    cls_name = opts.writer
     try:
-        writerCls = getattr(sys.modules[__name__],clsName)
-    except:
-        print(f'Unsupported writer {clsName}')
-        sys.exit(1)
+        writer_cls = getattr(modules[__name__], cls_name)
+    except AttributeError:
+        print(f'Unsupported writer {cls_name}')
+        raise
 
-    writer = writerCls()
+    writer = writer_cls()
     writer.logger.setLevel(getattr(logging, opts.log_level))
     log_handler = logging.StreamHandler()
-    log_handler.setFormatter(logging.Formatter('{name:20}: {message}', style='{'))
+    log_handler.setFormatter(logging.Formatter(
+        '{name:20}: {message}', style='{'))
     writer.logger.addHandler(log_handler)
     data = writer.write(opts.data, opts.filename)
-    print(f"Writer {writer} writes to {opts.filename}, data {data}")
+    print(f'Writer {writer} writes to {opts.filename}, data {data}')
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `ChessAnalysisPipeline-0.0.5/ChessAnalysisPipeline.egg-info/PKG-INFO` & `ChessAnalysisPipeline-0.0.6/ChessAnalysisPipeline.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChessAnalysisPipeline
-Version: 0.0.5
+Version: 0.0.6
 Summary: CHESS analysis pipeline framework
 Home-page: https://github.com/CHESSComputing/ChessAnalysisPipeline
 Author: Keara Soloway, Rolf Verberg, Valentin Kuznetsov
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ChessAnalysisPipeline-0.0.5/ChessAnalysisPipeline.egg-info/SOURCES.txt` & `ChessAnalysisPipeline-0.0.6/ChessAnalysisPipeline.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 LICENSE
 README.md
 setup.py
+CHAP/TaskManager.py
 CHAP/__init__.py
 CHAP/pipeline.py
 CHAP/processor.py
 CHAP/reader.py
 CHAP/runner.py
+CHAP/server.py
 CHAP/writer.py
 CHAP/common/__init__.py
 CHAP/common/processor.py
 CHAP/common/reader.py
 CHAP/common/writer.py
 CHAP/common/models/__init__.py
 CHAP/common/models/integration.py
```

### Comparing `ChessAnalysisPipeline-0.0.5/LICENSE` & `ChessAnalysisPipeline-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.5/MLaaS/ktrain.py` & `ChessAnalysisPipeline-0.0.6/MLaaS/ktrain.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.5/MLaaS/mnist_img.py` & `ChessAnalysisPipeline-0.0.6/MLaaS/mnist_img.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.5/MLaaS/tfaas_client.py` & `ChessAnalysisPipeline-0.0.6/MLaaS/tfaas_client.py`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.5/PKG-INFO` & `ChessAnalysisPipeline-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChessAnalysisPipeline
-Version: 0.0.5
+Version: 0.0.6
 Summary: CHESS analysis pipeline framework
 Home-page: https://github.com/CHESSComputing/ChessAnalysisPipeline
 Author: Keara Soloway, Rolf Verberg, Valentin Kuznetsov
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ChessAnalysisPipeline-0.0.5/README.md` & `ChessAnalysisPipeline-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ChessAnalysisPipeline-0.0.5/setup.py` & `ChessAnalysisPipeline-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 to build doc : python setup.py doc
 to run tests : python setup.py test
 """
 
 import os
 import setuptools
 
-version = 'v0.0.5'
+version = 'v0.0.6'
 
 def datafiles(idir, pattern=None):
     """Return list of data files in provided relative dir"""
     files = []
     for dirname, dirnames, filenames in os.walk(idir):
         for subdirname in dirnames:
             files.append(os.path.join(dirname, subdirname))
```


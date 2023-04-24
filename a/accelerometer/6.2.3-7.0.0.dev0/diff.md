# Comparing `tmp/accelerometer-6.2.3.tar.gz` & `tmp/accelerometer-7.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/accelerometer-6.2.3.tar", last modified: Tue Mar 28 06:13:58 2023, max compression
+gzip compressed data, was "accelerometer-7.0.0.dev0.tar", last modified: Mon Apr 24 18:09:04 2023, max compression
```

## Comparing `accelerometer-6.2.3.tar` & `accelerometer-7.0.0.dev0.tar`

### file list

```diff
@@ -1,60 +1,64 @@
-drwxr-xr-x   0 shing     (1000) shing     (1000)        0 2023-03-28 06:13:58.000000 accelerometer-6.2.3/
--rw-r--r--   0 shing     (1000) shing     (1000)     8045 2023-02-25 21:02:41.000000 accelerometer-6.2.3/LICENSE.md
--rw-r--r--   0 shing     (1000) shing     (1000)      264 2022-07-22 18:09:42.000000 accelerometer-6.2.3/MANIFEST.in
--rw-r--r--   0 shing     (1000) shing     (1000)     4379 2023-03-28 06:13:58.000000 accelerometer-6.2.3/PKG-INFO
--rw-r--r--   0 shing     (1000) shing     (1000)     3579 2023-02-25 21:02:41.000000 accelerometer-6.2.3/README.md
-drwxr-xr-x   0 shing     (1000) shing     (1000)        0 2023-03-28 06:13:58.000000 accelerometer-6.2.3/accelerometer/
--rw-r--r--   0 shing     (1000) shing     (1000)      273 2023-03-28 06:11:39.000000 accelerometer-6.2.3/accelerometer/__init__.py
--rw-r--r--   0 shing     (1000) shing     (1000)      402 2022-07-22 18:09:42.000000 accelerometer-6.2.3/accelerometer/accCollateSummary.py
--rw-r--r--   0 shing     (1000) shing     (1000)     9133 2023-02-25 21:02:41.000000 accelerometer-6.2.3/accelerometer/accPlot.py
--rw-r--r--   0 shing     (1000) shing     (1000)    20172 2022-07-22 18:09:42.000000 accelerometer-6.2.3/accelerometer/accProcess.py
--rw-r--r--   0 shing     (1000) shing     (1000)      805 2022-07-22 18:09:42.000000 accelerometer-6.2.3/accelerometer/accWriteCmds.py
-drwxr-xr-x   0 shing     (1000) shing     (1000)        0 2023-03-28 06:13:58.000000 accelerometer-6.2.3/accelerometer/activityModels/
--rw-r--r--   0 shing     (1000) shing     (1000)       58 2022-07-22 18:09:42.000000 accelerometer-6.2.3/accelerometer/activityModels/README.md
--rw-r--r--   0 shing     (1000) shing     (1000)     4929 2022-07-22 18:09:42.000000 accelerometer-6.2.3/accelerometer/circadian.py
--rw-r--r--   0 shing     (1000) shing     (1000)    19110 2023-02-25 21:02:41.000000 accelerometer-6.2.3/accelerometer/classification.py
--rw-r--r--   0 shing     (1000) shing     (1000)    22477 2023-03-28 05:44:48.000000 accelerometer-6.2.3/accelerometer/device.py
-drwxr-xr-x   0 shing     (1000) shing     (1000)        0 2023-03-28 06:13:58.000000 accelerometer-6.2.3/accelerometer/java/
--rw-r--r--   0 shing     (1000) shing     (1000)     5339 2023-03-28 06:13:57.000000 accelerometer-6.2.3/accelerometer/java/AccStats.class
--rw-r--r--   0 shing     (1000) shing     (1000)    11339 2023-02-25 21:02:41.000000 accelerometer-6.2.3/accelerometer/java/AccStats.java
--rw-r--r--   0 shing     (1000) shing     (1000)     7628 2023-03-28 06:13:57.000000 accelerometer-6.2.3/accelerometer/java/AccelerometerParser.class
--rw-r--r--   0 shing     (1000) shing     (1000)    10305 2023-02-25 21:02:41.000000 accelerometer-6.2.3/accelerometer/java/AccelerometerParser.java
--rw-r--r--   0 shing     (1000) shing     (1000)    11961 2023-03-28 06:13:57.000000 accelerometer-6.2.3/accelerometer/java/ActigraphReader.class
--rw-r--r--   0 shing     (1000) shing     (1000)    29730 2023-02-25 21:02:41.000000 accelerometer-6.2.3/accelerometer/java/ActigraphReader.java
--rw-r--r--   0 shing     (1000) shing     (1000)     6683 2023-03-28 06:13:57.000000 accelerometer-6.2.3/accelerometer/java/AxivityReader.class
--rw-r--r--   0 shing     (1000) shing     (1000)    16174 2023-03-03 17:16:43.000000 accelerometer-6.2.3/accelerometer/java/AxivityReader.java
--rw-r--r--   0 shing     (1000) shing     (1000)     2649 2023-03-28 06:13:57.000000 accelerometer-6.2.3/accelerometer/java/BandpassFilter.class
--rw-r--r--   0 shing     (1000) shing     (1000)     4412 2023-02-25 21:02:41.000000 accelerometer-6.2.3/accelerometer/java/BandpassFilter.java
--rw-r--r--   0 shing     (1000) shing     (1000)     2793 2023-03-28 06:13:57.000000 accelerometer-6.2.3/accelerometer/java/CsvReader.class
--rw-r--r--   0 shing     (1000) shing     (1000)     3226 2023-02-25 21:02:41.000000 accelerometer-6.2.3/accelerometer/java/CsvReader.java
--rw-r--r--   0 shing     (1000) shing     (1000)     5360 2023-03-28 06:13:57.000000 accelerometer-6.2.3/accelerometer/java/DeviceReader.class
--rw-r--r--   0 shing     (1000) shing     (1000)     6890 2023-03-03 17:16:46.000000 accelerometer-6.2.3/accelerometer/java/DeviceReader.java
--rw-r--r--   0 shing     (1000) shing     (1000)    11537 2023-03-28 06:13:57.000000 accelerometer-6.2.3/accelerometer/java/EpochWriter.class
--rw-r--r--   0 shing     (1000) shing     (1000)    15684 2022-07-22 18:09:42.000000 accelerometer-6.2.3/accelerometer/java/EpochWriter.java
--rw-r--r--   0 shing     (1000) shing     (1000)     8376 2023-03-28 06:13:57.000000 accelerometer-6.2.3/accelerometer/java/Features.class
--rw-r--r--   0 shing     (1000) shing     (1000)    24365 2023-02-25 21:02:41.000000 accelerometer-6.2.3/accelerometer/java/Features.java
--rw-r--r--   0 shing     (1000) shing     (1000)     1021 2023-03-28 06:13:57.000000 accelerometer-6.2.3/accelerometer/java/Filter.class
--rw-r--r--   0 shing     (1000) shing     (1000)     1426 2023-02-25 21:02:41.000000 accelerometer-6.2.3/accelerometer/java/Filter.java
--rw-r--r--   0 shing     (1000) shing     (1000)     4273 2023-03-28 06:13:58.000000 accelerometer-6.2.3/accelerometer/java/GENEActivReader.class
--rw-r--r--   0 shing     (1000) shing     (1000)     7859 2023-03-03 17:31:54.000000 accelerometer-6.2.3/accelerometer/java/GENEActivReader.java
--rw-r--r--   0 shing     (1000) shing     (1000)  1501730 2022-07-22 18:09:42.000000 accelerometer-6.2.3/accelerometer/java/JTransforms-3.1-with-dependencies.jar
--rw-r--r--   0 shing     (1000) shing     (1000)     2617 2023-03-28 06:13:58.000000 accelerometer-6.2.3/accelerometer/java/LowpassFilter.class
--rw-r--r--   0 shing     (1000) shing     (1000)     4366 2023-02-25 21:02:41.000000 accelerometer-6.2.3/accelerometer/java/LowpassFilter.java
--rw-r--r--   0 shing     (1000) shing     (1000)     6391 2023-03-28 06:13:57.000000 accelerometer-6.2.3/accelerometer/java/NpyWriter.class
--rw-r--r--   0 shing     (1000) shing     (1000)     6967 2022-07-22 18:09:42.000000 accelerometer-6.2.3/accelerometer/java/NpyWriter.java
--rw-r--r--   0 shing     (1000) shing     (1000)       44 2022-07-22 18:09:42.000000 accelerometer-6.2.3/accelerometer/java/README.md
--rw-r--r--   0 shing     (1000) shing     (1000)     2852 2023-03-28 06:13:58.000000 accelerometer-6.2.3/accelerometer/java/Resample.class
--rw-r--r--   0 shing     (1000) shing     (1000)     4560 2022-07-22 18:09:42.000000 accelerometer-6.2.3/accelerometer/java/Resample.java
--rw-r--r--   0 shing     (1000) shing     (1000)      326 2022-07-22 18:09:42.000000 accelerometer-6.2.3/accelerometer/java/logging.properties
--rw-r--r--   0 shing     (1000) shing     (1000)      860 2023-03-03 16:09:51.000000 accelerometer-6.2.3/accelerometer/models.py
--rw-r--r--   0 shing     (1000) shing     (1000)    17888 2023-03-28 05:48:29.000000 accelerometer-6.2.3/accelerometer/summarisation.py
--rw-r--r--   0 shing     (1000) shing     (1000)    15015 2023-03-03 16:09:51.000000 accelerometer-6.2.3/accelerometer/utils.py
-drwxr-xr-x   0 shing     (1000) shing     (1000)        0 2023-03-28 06:13:58.000000 accelerometer-6.2.3/accelerometer.egg-info/
--rw-r--r--   0 shing     (1000) shing     (1000)     4379 2023-03-28 06:13:58.000000 accelerometer-6.2.3/accelerometer.egg-info/PKG-INFO
--rw-r--r--   0 shing     (1000) shing     (1000)     1767 2023-03-28 06:13:58.000000 accelerometer-6.2.3/accelerometer.egg-info/SOURCES.txt
--rw-r--r--   0 shing     (1000) shing     (1000)        1 2023-03-28 06:13:58.000000 accelerometer-6.2.3/accelerometer.egg-info/dependency_links.txt
--rw-r--r--   0 shing     (1000) shing     (1000)      202 2023-03-28 06:13:58.000000 accelerometer-6.2.3/accelerometer.egg-info/entry_points.txt
--rw-r--r--   0 shing     (1000) shing     (1000)      304 2023-03-28 06:13:58.000000 accelerometer-6.2.3/accelerometer.egg-info/requires.txt
--rw-r--r--   0 shing     (1000) shing     (1000)       14 2023-03-28 06:13:58.000000 accelerometer-6.2.3/accelerometer.egg-info/top_level.txt
--rw-r--r--   0 shing     (1000) shing     (1000)       38 2023-03-28 06:13:58.000000 accelerometer-6.2.3/setup.cfg
--rw-r--r--   0 shing     (1000) shing     (1000)     2352 2023-03-03 16:09:51.000000 accelerometer-6.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:09:04.028379 accelerometer-7.0.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-04-24 18:09:04.028379 accelerometer-7.0.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 18:09:04.028379 accelerometer-7.0.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:09:04.012379 accelerometer-7.0.0.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:09:04.028379 accelerometer-7.0.0.dev0/src/accelerometer/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-24 18:09:04.028379 accelerometer-7.0.0.dev0/src/accelerometer/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/accCollateSummary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/accPlot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20172 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/accProcess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/accWriteCmds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:09:04.016379 accelerometer-7.0.0.dev0/src/accelerometer/activityModels/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/activityModels/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/circadian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19110 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22477 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:09:04.024379 accelerometer-7.0.0.dev0/src/accelerometer/java/
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-04-24 18:08:50.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/AccStats.class
+-rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/AccStats.java
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-24 18:08:50.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/AccelerometerParser.class
+-rw-r--r--   0 runner    (1001) docker     (123)    10305 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/AccelerometerParser.java
+-rw-r--r--   0 runner    (1001) docker     (123)    11988 2023-04-24 18:08:50.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/ActigraphReader.class
+-rw-r--r--   0 runner    (1001) docker     (123)    29730 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/ActigraphReader.java
+-rw-r--r--   0 runner    (1001) docker     (123)     7007 2023-04-24 18:08:51.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/AxivityReader.class
+-rw-r--r--   0 runner    (1001) docker     (123)    16174 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/AxivityReader.java
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-24 18:08:51.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/BandpassFilter.class
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/BandpassFilter.java
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-24 18:08:51.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/CsvReader.class
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/CsvReader.java
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-04-24 18:08:50.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/DeviceReader.class
+-rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/DeviceReader.java
+-rw-r--r--   0 runner    (1001) docker     (123)    11569 2023-04-24 18:08:50.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/EpochWriter.class
+-rw-r--r--   0 runner    (1001) docker     (123)    15684 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/EpochWriter.java
+-rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-04-24 18:08:51.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/Features.class
+-rw-r--r--   0 runner    (1001) docker     (123)    24365 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/Features.java
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-24 18:08:50.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/Filter.class
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/Filter.java
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-04-24 18:08:51.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/GENEActivReader.class
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/GENEActivReader.java
+-rw-r--r--   0 runner    (1001) docker     (123)  1501730 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/JTransforms-3.1-with-dependencies.jar
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-24 18:08:51.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/LowpassFilter.class
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/LowpassFilter.java
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-04-24 18:08:50.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/NpyWriter.class
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/NpyWriter.java
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-24 18:08:51.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/Resample.class
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/Resample.java
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/java/logging.properties
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/summarisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15015 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/src/accelerometer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:09:04.016379 accelerometer-7.0.0.dev0/src/accelerometer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-04-24 18:09:03.000000 accelerometer-7.0.0.dev0/src/accelerometer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-24 18:09:03.000000 accelerometer-7.0.0.dev0/src/accelerometer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 18:09:03.000000 accelerometer-7.0.0.dev0/src/accelerometer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-24 18:09:03.000000 accelerometer-7.0.0.dev0/src/accelerometer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-24 18:09:03.000000 accelerometer-7.0.0.dev0/src/accelerometer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-24 18:09:03.000000 accelerometer-7.0.0.dev0/src/accelerometer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-04-24 18:08:45.000000 accelerometer-7.0.0.dev0/versioneer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `accelerometer-6.2.3/LICENSE.md` & `accelerometer-7.0.0.dev0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `accelerometer-6.2.3/PKG-INFO` & `accelerometer-7.0.0.dev0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 Metadata-Version: 2.1
 Name: accelerometer
-Version: 6.2.3
+Version: 7.0.0.dev0
 Summary: A package to extract meaningful health information from large accelerometer datasets e.g. how much time individuals spend in sleep, sedentary behaviour, walking and moderate intensity physical activity
 Home-page: https://github.com/activityMonitoring/biobankAccelerometerAnalysis
+Download-URL: https://github.com/activityMonitoring/biobankAccelerometerAnalysis
 Author: Aiden Doherty, Shing Chan, Rosemary Walmsley, Hang Yuan
-Author-email: aiden.doherty@ndph.ox.ac.uk, shing.chan@ndph.ox.ac.uk, rosemary.walmsley@gtc.ox.ac.uk, hang.yuan@keble.ox.ac.uk
+Maintainer: Shing Chan
+Maintainer-email: shing.chan@ndph.ox.ac.uk
+License: See LICENSE.md
+Keywords: wearables,accelerometer,health data science,human activity recognition
 Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Unix
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE.md
 
 ![Accelerometer data processing overview](docs/source/accelerometerLogo.png)
```

### Comparing `accelerometer-6.2.3/README.md` & `accelerometer-7.0.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `accelerometer-6.2.3/accelerometer/accPlot.py` & `accelerometer-7.0.0.dev0/src/accelerometer/accPlot.py`

 * *Files identical despite different names*

### Comparing `accelerometer-6.2.3/accelerometer/accProcess.py` & `accelerometer-7.0.0.dev0/src/accelerometer/accProcess.py`

 * *Files identical despite different names*

### Comparing `accelerometer-6.2.3/accelerometer/accWriteCmds.py` & `accelerometer-7.0.0.dev0/src/accelerometer/accWriteCmds.py`

 * *Files identical despite different names*

### Comparing `accelerometer-6.2.3/accelerometer/circadian.py` & `accelerometer-7.0.0.dev0/src/accelerometer/circadian.py`

 * *Files identical despite different names*

### Comparing `accelerometer-6.2.3/accelerometer/classification.py` & `accelerometer-7.0.0.dev0/src/accelerometer/classification.py`

 * *Files identical despite different names*

### Comparing `accelerometer-6.2.3/accelerometer/device.py` & `accelerometer-7.0.0.dev0/src/accelerometer/device.py`

 * *Files identical despite different names*

### Comparing `accelerometer-6.2.3/accelerometer/java/AccStats.class` & `accelerometer-7.0.0.dev0/src/accelerometer/java/AccStats.class`

 * *Files 4% similar despite different names*

#### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 52853834eb55d0f928cb09e99728d33d9fbbfc57ec61eb40dd46272ff18d044f
+  SHA-256 checksum b573442e4d77c04820d0a999c7a6db38a8962a5117ec23dc693e226f74ae1585
   Compiled from "AccStats.java"
 public class AccStats
   minor version: 0
   major version: 52
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #53                         // AccStats
   super_class: #54                        // java/lang/Object
@@ -10,69 +10,69 @@
 Constant pool:
     #1 = Methodref          #54.#97       // java/lang/Object."<init>":()V
     #2 = Methodref          #53.#98       // AccStats.mean:([D)D
     #3 = Methodref          #53.#99       // AccStats.range:([D)D
     #4 = Methodref          #53.#100      // AccStats.std:([DD)D
     #5 = Methodref          #53.#101      // AccStats.covariance:([D[DDDI)D
     #6 = Methodref          #53.#102      // AccStats.getENMO:([D[D[D)[D
-    #7 = Methodref          #62.#103      // Filter.filter:([D)V
-    #8 = Methodref          #53.#104      // AccStats.trunc:([D)[D
-    #9 = Methodref          #53.#105      // AccStats.abs:([D)[D
-   #10 = Methodref          #63.#106      // java/lang/Boolean.booleanValue:()Z
-   #11 = Methodref          #107.#108     // Features.getFeatures:([D[D[D[DI)[D
-   #12 = Methodref          #53.#109      // AccStats.combineArrays:([D[D)[D
-   #13 = String             #110          // enmoTrunc,enmoAbs
-   #14 = Class              #111          // java/lang/StringBuilder
+    #7 = Methodref          #103.#104     // Filter.filter:([D)V
+    #8 = Methodref          #53.#105      // AccStats.trunc:([D)[D
+    #9 = Methodref          #53.#106      // AccStats.abs:([D)[D
+   #10 = Methodref          #107.#108     // java/lang/Boolean.booleanValue:()Z
+   #11 = Methodref          #109.#110     // Features.getFeatures:([D[D[D[DI)[D
+   #12 = Methodref          #53.#111      // AccStats.combineArrays:([D[D)[D
+   #13 = String             #112          // enmoTrunc,enmoAbs
+   #14 = Class              #113          // java/lang/StringBuilder
    #15 = Methodref          #14.#97       // java/lang/StringBuilder."<init>":()V
-   #16 = Methodref          #14.#112      // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-   #17 = String             #113          // ,xMean,yMean,zMean
-   #18 = Methodref          #14.#114      // java/lang/StringBuilder.toString:()Ljava/lang/String;
-   #19 = String             #115          // ,xRange,yRange,zRange,xStd,yStd,zStd
-   #20 = String             #116          // ,xyCov,xzCov,yzCov
-   #21 = String             #117          // ,
-   #22 = Methodref          #107.#118     // Features.getFeaturesHeader:()Ljava/lang/String;
-   #23 = Methodref          #53.#119      // AccStats.getVectorMagnitude:(DDD)D
-   #24 = Methodref          #120.#121     // java/lang/Math.sqrt:(D)D
-   #25 = Methodref          #120.#122     // java/lang/Math.abs:(D)D
-   #26 = Class              #123          // java/lang/Double
+   #16 = Methodref          #14.#114      // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+   #17 = String             #115          // ,xMean,yMean,zMean
+   #18 = Methodref          #14.#116      // java/lang/StringBuilder.toString:()Ljava/lang/String;
+   #19 = String             #117          // ,xRange,yRange,zRange,xStd,yStd,zStd
+   #20 = String             #118          // ,xyCov,xzCov,yzCov
+   #21 = String             #119          // ,
+   #22 = Methodref          #109.#120     // Features.getFeaturesHeader:()Ljava/lang/String;
+   #23 = Methodref          #53.#121      // AccStats.getVectorMagnitude:(DDD)D
+   #24 = Methodref          #122.#123     // java/lang/Math.sqrt:(D)D
+   #25 = Methodref          #122.#124     // java/lang/Math.abs:(D)D
+   #26 = Class              #125          // java/lang/Double
    #27 = Double             NaNd
-   #29 = Methodref          #124.#125     // java/util/Arrays.fill:([DD)V
-   #30 = Methodref          #126.#127     // "[D".clone:()Ljava/lang/Object;
-   #31 = Class              #128          // "[D"
-   #32 = Methodref          #124.#129     // java/util/Arrays.sort:([D)V
-   #33 = Methodref          #120.#130     // java/lang/Math.floor:(D)D
-   #34 = Methodref          #120.#131     // java/lang/Math.atan2:(DD)D
+   #29 = Methodref          #126.#127     // java/util/Arrays.fill:([DD)V
+   #30 = Methodref          #128.#129     // "[D".clone:()Ljava/lang/Object;
+   #31 = Class              #130          // "[D"
+   #32 = Methodref          #126.#131     // java/util/Arrays.sort:([D)V
+   #33 = Methodref          #122.#132     // java/lang/Math.floor:(D)D
+   #34 = Methodref          #122.#133     // java/lang/Math.atan2:(DD)D
    #35 = Double             2.0d
-   #37 = Methodref          #120.#132     // java/lang/Math.pow:(DD)D
-   #38 = Methodref          #120.#133     // java/lang/Math.abs:(I)I
-   #39 = Methodref          #26.#134      // java/lang/Double.isNaN:(D)Z
-   #40 = Methodref          #53.#135      // AccStats.correlation:([D[DI)D
-   #41 = Methodref          #120.#136     // java/lang/Math.max:(DD)D
-   #42 = InterfaceMethodref #137.#138     // java/util/List.size:()I
-   #43 = InterfaceMethodref #137.#139     // java/util/List.get:(I)Ljava/lang/Object;
-   #44 = Methodref          #26.#140      // java/lang/Double.doubleValue:()D
-   #45 = Methodref          #53.#141      // AccStats.sum:([D)D
-   #46 = Methodref          #53.#142      // AccStats.sum:(Ljava/util/List;)D
+   #37 = Methodref          #122.#134     // java/lang/Math.pow:(DD)D
+   #38 = Methodref          #122.#135     // java/lang/Math.abs:(I)I
+   #39 = Methodref          #26.#136      // java/lang/Double.isNaN:(D)Z
+   #40 = Methodref          #53.#137      // AccStats.correlation:([D[DI)D
+   #41 = Methodref          #122.#138     // java/lang/Math.max:(DD)D
+   #42 = InterfaceMethodref #139.#140     // java/util/List.size:()I
+   #43 = InterfaceMethodref #139.#141     // java/util/List.get:(I)Ljava/lang/Object;
+   #44 = Methodref          #26.#142      // java/lang/Double.doubleValue:()D
+   #45 = Methodref          #53.#143      // AccStats.sum:([D)D
+   #46 = Methodref          #53.#144      // AccStats.sum:(Ljava/util/List;)D
    #47 = Double             1.7976931348623157E308d
    #49 = Double             -1.7976931348623157E308d
    #51 = Double             1.5d
-   #53 = Class              #143          // AccStats
-   #54 = Class              #144          // java/lang/Object
+   #53 = Class              #145          // AccStats
+   #54 = Class              #146          // java/lang/Object
    #55 = Utf8               <init>
    #56 = Utf8               ()V
    #57 = Utf8               Code
    #58 = Utf8               LineNumberTable
    #59 = Utf8               getAccStats
    #60 = Utf8               ([D[D[DLFilter;Ljava/lang/Boolean;I)[D
    #61 = Utf8               StackMapTable
-   #62 = Class              #145          // Filter
-   #63 = Class              #146          // java/lang/Boolean
+   #62 = Class              #147          // Filter
+   #63 = Class              #148          // java/lang/Boolean
    #64 = Utf8               getStatsHeader
    #65 = Utf8               (Ljava/lang/Boolean;)Ljava/lang/String;
-   #66 = Class              #147          // java/lang/String
+   #66 = Class              #149          // java/lang/String
    #67 = Utf8               getENMO
    #68 = Utf8               ([D[D[D)[D
    #69 = Utf8               getVectorMagnitude
    #70 = Utf8               (DDD)D
    #71 = Utf8               abs
    #72 = Utf8               ([D)[D
    #73 = Utf8               trunc
@@ -101,95 +101,97 @@
    #96 = Utf8               AccStats.java
    #97 = NameAndType        #55:#56       // "<init>":()V
    #98 = NameAndType        #87:#83       // mean:([D)D
    #99 = NameAndType        #88:#83       // range:([D)D
   #100 = NameAndType        #89:#90       // std:([DD)D
   #101 = NameAndType        #77:#78       // covariance:([D[DDDI)D
   #102 = NameAndType        #67:#68       // getENMO:([D[D[D)[D
-  #103 = NameAndType        #148:#149     // filter:([D)V
-  #104 = NameAndType        #73:#72       // trunc:([D)[D
-  #105 = NameAndType        #71:#72       // abs:([D)[D
-  #106 = NameAndType        #150:#151     // booleanValue:()Z
-  #107 = Class              #152          // Features
-  #108 = NameAndType        #153:#154     // getFeatures:([D[D[D[DI)[D
-  #109 = NameAndType        #94:#75       // combineArrays:([D[D)[D
-  #110 = Utf8               enmoTrunc,enmoAbs
-  #111 = Utf8               java/lang/StringBuilder
-  #112 = NameAndType        #155:#156     // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #113 = Utf8               ,xMean,yMean,zMean
-  #114 = NameAndType        #157:#158     // toString:()Ljava/lang/String;
-  #115 = Utf8               ,xRange,yRange,zRange,xStd,yStd,zStd
-  #116 = Utf8               ,xyCov,xzCov,yzCov
-  #117 = Utf8               ,
-  #118 = NameAndType        #159:#158     // getFeaturesHeader:()Ljava/lang/String;
-  #119 = NameAndType        #69:#70       // getVectorMagnitude:(DDD)D
-  #120 = Class              #160          // java/lang/Math
-  #121 = NameAndType        #161:#162     // sqrt:(D)D
-  #122 = NameAndType        #71:#162      // abs:(D)D
-  #123 = Utf8               java/lang/Double
-  #124 = Class              #163          // java/util/Arrays
-  #125 = NameAndType        #164:#165     // fill:([DD)V
-  #126 = Class              #128          // "[D"
-  #127 = NameAndType        #166:#167     // clone:()Ljava/lang/Object;
-  #128 = Utf8               [D
-  #129 = NameAndType        #168:#149     // sort:([D)V
-  #130 = NameAndType        #169:#162     // floor:(D)D
-  #131 = NameAndType        #170:#171     // atan2:(DD)D
-  #132 = NameAndType        #172:#171     // pow:(DD)D
-  #133 = NameAndType        #71:#173      // abs:(I)I
-  #134 = NameAndType        #174:#175     // isNaN:(D)Z
-  #135 = NameAndType        #79:#81       // correlation:([D[DI)D
-  #136 = NameAndType        #176:#171     // max:(DD)D
-  #137 = Class              #177          // java/util/List
-  #138 = NameAndType        #178:#179     // size:()I
-  #139 = NameAndType        #180:#181     // get:(I)Ljava/lang/Object;
-  #140 = NameAndType        #182:#183     // doubleValue:()D
-  #141 = NameAndType        #82:#83       // sum:([D)D
-  #142 = NameAndType        #82:#84       // sum:(Ljava/util/List;)D
-  #143 = Utf8               AccStats
-  #144 = Utf8               java/lang/Object
-  #145 = Utf8               Filter
-  #146 = Utf8               java/lang/Boolean
-  #147 = Utf8               java/lang/String
-  #148 = Utf8               filter
-  #149 = Utf8               ([D)V
-  #150 = Utf8               booleanValue
-  #151 = Utf8               ()Z
-  #152 = Utf8               Features
-  #153 = Utf8               getFeatures
-  #154 = Utf8               ([D[D[D[DI)[D
-  #155 = Utf8               append
-  #156 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #157 = Utf8               toString
-  #158 = Utf8               ()Ljava/lang/String;
-  #159 = Utf8               getFeaturesHeader
-  #160 = Utf8               java/lang/Math
-  #161 = Utf8               sqrt
-  #162 = Utf8               (D)D
-  #163 = Utf8               java/util/Arrays
-  #164 = Utf8               fill
-  #165 = Utf8               ([DD)V
-  #166 = Utf8               clone
-  #167 = Utf8               ()Ljava/lang/Object;
-  #168 = Utf8               sort
-  #169 = Utf8               floor
-  #170 = Utf8               atan2
-  #171 = Utf8               (DD)D
-  #172 = Utf8               pow
-  #173 = Utf8               (I)I
-  #174 = Utf8               isNaN
-  #175 = Utf8               (D)Z
-  #176 = Utf8               max
-  #177 = Utf8               java/util/List
-  #178 = Utf8               size
-  #179 = Utf8               ()I
-  #180 = Utf8               get
-  #181 = Utf8               (I)Ljava/lang/Object;
-  #182 = Utf8               doubleValue
-  #183 = Utf8               ()D
+  #103 = Class              #147          // Filter
+  #104 = NameAndType        #150:#151     // filter:([D)V
+  #105 = NameAndType        #73:#72       // trunc:([D)[D
+  #106 = NameAndType        #71:#72       // abs:([D)[D
+  #107 = Class              #148          // java/lang/Boolean
+  #108 = NameAndType        #152:#153     // booleanValue:()Z
+  #109 = Class              #154          // Features
+  #110 = NameAndType        #155:#156     // getFeatures:([D[D[D[DI)[D
+  #111 = NameAndType        #94:#75       // combineArrays:([D[D)[D
+  #112 = Utf8               enmoTrunc,enmoAbs
+  #113 = Utf8               java/lang/StringBuilder
+  #114 = NameAndType        #157:#158     // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #115 = Utf8               ,xMean,yMean,zMean
+  #116 = NameAndType        #159:#160     // toString:()Ljava/lang/String;
+  #117 = Utf8               ,xRange,yRange,zRange,xStd,yStd,zStd
+  #118 = Utf8               ,xyCov,xzCov,yzCov
+  #119 = Utf8               ,
+  #120 = NameAndType        #161:#160     // getFeaturesHeader:()Ljava/lang/String;
+  #121 = NameAndType        #69:#70       // getVectorMagnitude:(DDD)D
+  #122 = Class              #162          // java/lang/Math
+  #123 = NameAndType        #163:#164     // sqrt:(D)D
+  #124 = NameAndType        #71:#164      // abs:(D)D
+  #125 = Utf8               java/lang/Double
+  #126 = Class              #165          // java/util/Arrays
+  #127 = NameAndType        #166:#167     // fill:([DD)V
+  #128 = Class              #130          // "[D"
+  #129 = NameAndType        #168:#169     // clone:()Ljava/lang/Object;
+  #130 = Utf8               [D
+  #131 = NameAndType        #170:#151     // sort:([D)V
+  #132 = NameAndType        #171:#164     // floor:(D)D
+  #133 = NameAndType        #172:#173     // atan2:(DD)D
+  #134 = NameAndType        #174:#173     // pow:(DD)D
+  #135 = NameAndType        #71:#175      // abs:(I)I
+  #136 = NameAndType        #176:#177     // isNaN:(D)Z
+  #137 = NameAndType        #79:#81       // correlation:([D[DI)D
+  #138 = NameAndType        #178:#173     // max:(DD)D
+  #139 = Class              #179          // java/util/List
+  #140 = NameAndType        #180:#181     // size:()I
+  #141 = NameAndType        #182:#183     // get:(I)Ljava/lang/Object;
+  #142 = NameAndType        #184:#185     // doubleValue:()D
+  #143 = NameAndType        #82:#83       // sum:([D)D
+  #144 = NameAndType        #82:#84       // sum:(Ljava/util/List;)D
+  #145 = Utf8               AccStats
+  #146 = Utf8               java/lang/Object
+  #147 = Utf8               Filter
+  #148 = Utf8               java/lang/Boolean
+  #149 = Utf8               java/lang/String
+  #150 = Utf8               filter
+  #151 = Utf8               ([D)V
+  #152 = Utf8               booleanValue
+  #153 = Utf8               ()Z
+  #154 = Utf8               Features
+  #155 = Utf8               getFeatures
+  #156 = Utf8               ([D[D[D[DI)[D
+  #157 = Utf8               append
+  #158 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #159 = Utf8               toString
+  #160 = Utf8               ()Ljava/lang/String;
+  #161 = Utf8               getFeaturesHeader
+  #162 = Utf8               java/lang/Math
+  #163 = Utf8               sqrt
+  #164 = Utf8               (D)D
+  #165 = Utf8               java/util/Arrays
+  #166 = Utf8               fill
+  #167 = Utf8               ([DD)V
+  #168 = Utf8               clone
+  #169 = Utf8               ()Ljava/lang/Object;
+  #170 = Utf8               sort
+  #171 = Utf8               floor
+  #172 = Utf8               atan2
+  #173 = Utf8               (DD)D
+  #174 = Utf8               pow
+  #175 = Utf8               (I)I
+  #176 = Utf8               isNaN
+  #177 = Utf8               (D)Z
+  #178 = Utf8               max
+  #179 = Utf8               java/util/List
+  #180 = Utf8               size
+  #181 = Utf8               ()I
+  #182 = Utf8               get
+  #183 = Utf8               (I)Ljava/lang/Object;
+  #184 = Utf8               doubleValue
+  #185 = Utf8               ()D
 {
   public AccStats();
     descriptor: ()V
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
```

### Comparing `accelerometer-6.2.3/accelerometer/java/AccStats.java` & `accelerometer-7.0.0.dev0/src/accelerometer/java/AccStats.java`

 * *Files identical despite different names*

### Comparing `accelerometer-6.2.3/accelerometer/java/AccelerometerParser.class` & `accelerometer-7.0.0.dev0/src/accelerometer/java/AccelerometerParser.class`

 * *Files 13% similar despite different names*

#### javap -verbose -constants -s -l -private {}

```diff
@@ -1,401 +1,409 @@
-  SHA-256 checksum a1981867602b404f7fe72ec529f73623198bfdb699eb390ddf84b20ccc14f9fd
+  SHA-256 checksum 48b96b2ed4a3249012d9b6247e05837e37f80d36f6556b5cd03b79bec3cb00fe
   Compiled from "AccelerometerParser.java"
 public class AccelerometerParser
   minor version: 0
   major version: 52
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #131                        // AccelerometerParser
   super_class: #132                       // java/lang/Object
   interfaces: 0, fields: 3, methods: 4, attributes: 1
 Constant pool:
-    #1 = Methodref          #132.#155     // java/lang/Object."<init>":()V
-    #2 = Class              #156          // java/lang/String
-    #3 = String             #157          //
-    #4 = String             #158          // Europe/London
-    #5 = Methodref          #144.#159     // java/lang/Boolean.valueOf:(Z)Ljava/lang/Boolean;
-    #6 = Fieldref           #131.#160     // AccelerometerParser.DF6:Ljava/text/DecimalFormat;
-    #7 = Fieldref           #161.#162     // java/math/RoundingMode.CEILING:Ljava/math/RoundingMode;
-    #8 = Methodref          #126.#163     // java/text/DecimalFormat.setRoundingMode:(Ljava/math/RoundingMode;)V
-    #9 = Fieldref           #131.#164     // AccelerometerParser.DF2:Ljava/text/DecimalFormat;
-   #10 = Fieldref           #131.#165     // AccelerometerParser.DF3:Ljava/text/DecimalFormat;
-   #11 = Fieldref           #161.#166     // java/math/RoundingMode.HALF_UP:Ljava/math/RoundingMode;
-   #12 = String             #167          // yyyy-MM-dd HH:mm:ss.SSSxxxx \'[\'VV\']\'
-   #13 = Methodref          #145.#168     // java/time/format/DateTimeFormatter.ofPattern:(Ljava/lang/String;)Ljava/time/format/DateTimeFormatter;
+    #1 = Methodref          #132.#159     // java/lang/Object."<init>":()V
+    #2 = Class              #160          // java/lang/String
+    #3 = String             #161          //
+    #4 = String             #162          // Europe/London
+    #5 = Methodref          #163.#164     // java/lang/Boolean.valueOf:(Z)Ljava/lang/Boolean;
+    #6 = Fieldref           #131.#165     // AccelerometerParser.DF6:Ljava/text/DecimalFormat;
+    #7 = Fieldref           #166.#167     // java/math/RoundingMode.CEILING:Ljava/math/RoundingMode;
+    #8 = Methodref          #126.#168     // java/text/DecimalFormat.setRoundingMode:(Ljava/math/RoundingMode;)V
+    #9 = Fieldref           #131.#169     // AccelerometerParser.DF2:Ljava/text/DecimalFormat;
+   #10 = Fieldref           #131.#170     // AccelerometerParser.DF3:Ljava/text/DecimalFormat;
+   #11 = Fieldref           #166.#171     // java/math/RoundingMode.HALF_UP:Ljava/math/RoundingMode;
+   #12 = String             #172          // yyyy-MM-dd HH:mm:ss.SSSxxxx \'[\'VV\']\'
+   #13 = Methodref          #173.#174     // java/time/format/DateTimeFormatter.ofPattern:(Ljava/lang/String;)Ljava/time/format/DateTimeFormatter;
    #14 = Double             0.013d
-   #16 = String             #169          // linear
+   #16 = String             #175          // linear
    #17 = Long               -1l
-   #19 = Class              #170          // java/lang/Integer
-   #20 = Methodref          #19.#171      // java/lang/Integer.valueOf:(I)Ljava/lang/Integer;
-   #21 = Methodref          #172.#173     // java/util/Arrays.asList:([Ljava/lang/Object;)Ljava/util/List;
-   #22 = String             #174          // Invalid input,
-   #23 = Class              #175          // java/lang/StringBuilder
-   #24 = Methodref          #23.#155      // java/lang/StringBuilder."<init>":()V
-   #25 = Methodref          #23.#176      // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-   #26 = String             #177          // please enter at least 1 parameter, e.g.\n
-   #27 = Methodref          #23.#178      // java/lang/StringBuilder.toString:()Ljava/lang/String;
-   #28 = String             #179          // java AccelerometerParser inputFile.cwa.gz
-   #29 = Fieldref           #180.#181     // java/lang/System.out:Ljava/io/PrintStream;
-   #30 = Methodref          #182.#183     // java/io/PrintStream.println:(Ljava/lang/String;)V
-   #31 = Methodref          #180.#184     // java/lang/System.exit:(I)V
-   #32 = String             #185          // \\.
-   #33 = Methodref          #2.#186       // java/lang/String.split:(Ljava/lang/String;)[Ljava/lang/String;
-   #34 = String             #187          // Epoch.csv
-   #35 = Methodref          #172.#188     // java/util/Arrays.copyOfRange:([Ljava/lang/Object;II)[Ljava/lang/Object;
-   #36 = Class              #189          // "[Ljava/lang/String;"
-   #37 = Class              #190          // java/text/SimpleDateFormat
-   #38 = String             #191          // yyyy-M-d\'T\'H:m
-   #39 = Methodref          #37.#192      // java/text/SimpleDateFormat."<init>":(Ljava/lang/String;)V
-   #40 = String             #193          // UTC
-   #41 = Methodref          #194.#195     // java/util/TimeZone.getTimeZone:(Ljava/lang/String;)Ljava/util/TimeZone;
-   #42 = Methodref          #37.#196      // java/text/SimpleDateFormat.setTimeZone:(Ljava/util/TimeZone;)V
-   #43 = String             #197          // :
-   #44 = Methodref          #2.#198       // java/lang/String.indexOf:(Ljava/lang/String;)I
-   #45 = Methodref          #2.#199       // java/lang/String.substring:(I)Ljava/lang/String;
-   #46 = String             #200          // timeZone
-   #47 = Methodref          #2.#201       // java/lang/String.equals:(Ljava/lang/Object;)Z
-   #48 = String             #202          // timeShift
-   #49 = Methodref          #19.#203      // java/lang/Integer.parseInt:(Ljava/lang/String;)I
-   #50 = String             #204          // outputFile
-   #51 = String             #205          // verbose
-   #52 = Methodref          #2.#206       // java/lang/String.toLowerCase:()Ljava/lang/String;
-   #53 = Methodref          #144.#207     // java/lang/Boolean.parseBoolean:(Ljava/lang/String;)Z
-   #54 = String             #208          // epochPeriod
-   #55 = String             #209          // filter
-   #56 = String             #210          // getStationaryBouts
-   #57 = String             #211          // stationaryStd
-   #58 = Methodref          #212.#213     // java/lang/Double.parseDouble:(Ljava/lang/String;)D
-   #59 = String             #214          // xIntercept
-   #60 = String             #215          // yIntercept
-   #61 = String             #216          // zIntercept
-   #62 = String             #217          // xSlope
-   #63 = String             #218          // ySlope
-   #64 = String             #219          // zSlope
-   #65 = String             #220          // xSlopeT
-   #66 = String             #221          // ySlopeT
-   #67 = String             #222          // zSlopeT
-   #68 = String             #223          // sampleRate
-   #69 = String             #224          // resampleMethod
-   #70 = String             #225          // range
-   #71 = String             #226          // rawOutput
-   #72 = String             #227          // rawFile
-   #73 = String             #228          // npyOutput
-   #74 = String             #229          // npyFile
-   #75 = String             #230          // startTime
-   #76 = String             #231          // endTime
-   #77 = String             #232          // csvTimeXYZTempColsIndex
-   #78 = String             #233          // ,
-   #79 = Fieldref           #180.#234     // java/lang/System.err:Ljava/io/PrintStream;
-   #80 = String             #235          // error parsing csvTimeXYZTempColsIndex:
-   #81 = Methodref          #132.#178     // java/lang/Object.toString:()Ljava/lang/String;
-   #82 = String             #236          // \n must be 4 or 5 comma separated integers
-   #83 = Class              #237          // java/util/LinkedList
-   #84 = Methodref          #83.#155      // java/util/LinkedList."<init>":()V
-   #85 = InterfaceMethodref #147.#238     // java/util/List.add:(Ljava/lang/Object;)Z
-   #86 = String             #239          // csvStartRow
-   #87 = String             #240          // getFeatures
-   #88 = String             #241          // csvTimeFormat
-   #89 = String             #242          // unknown parameter
-   #90 = Methodref          #2.#243       // java/lang/String.isEmpty:()Z
-   #91 = Methodref          #37.#244      // java/text/SimpleDateFormat.parse:(Ljava/lang/String;)Ljava/util/Date;
-   #92 = Methodref          #245.#246     // java/util/Date.getTime:()J
-   #93 = Class              #247          // java/text/ParseException
-   #94 = String             #248          // error parsing startTime:\'
-   #95 = String             #249          // \', must be in format: 1996-7-30T13:59
-   #96 = String             #250          // error parsing endTime:\'
-   #97 = String             #251          // Intermediate file:
-   #98 = Methodref          #144.#252     // java/lang/Boolean.booleanValue:()Z
-   #99 = Methodref          #253.#254     // DeviceReader.setupEpochWriter:(Ljava/lang/String;ZZLjava/lang/String;ZLjava/lang/String;ZLjava/time/format/DateTimeFormatter;Ljava/lang/String;IILjava/lang/String;I[D[D[DZDJJZ)LEpochWriter;
-  #100 = String             #255          // .cwa
-  #101 = Methodref          #2.#256       // java/lang/String.endsWith:(Ljava/lang/String;)Z
-  #102 = Methodref          #257.#258     // AxivityReader.readCwaEpochs:(Ljava/lang/String;Ljava/lang/String;ILEpochWriter;Ljava/lang/Boolean;)V
-  #103 = String             #259          // .cwa.gz
-  #104 = Methodref          #257.#260     // AxivityReader.readCwaGzEpochs:(Ljava/lang/String;Ljava/lang/String;ILEpochWriter;Ljava/lang/Boolean;)V
-  #105 = String             #261          // .bin
-  #106 = Methodref          #262.#263     // GENEActivReader.readGeneaEpochs:(Ljava/lang/String;Ljava/lang/String;ILEpochWriter;Ljava/lang/Boolean;)V
-  #107 = String             #264          // .gt3x
-  #108 = Methodref          #265.#266     // ActigraphReader.readG3TXEpochs:(Ljava/lang/String;LEpochWriter;Ljava/lang/Boolean;)V
-  #109 = String             #267          // .csv
-  #110 = String             #268          // .csv.gz
-  #111 = Methodref          #269.#270     // CsvReader.readCSVEpochs:(Ljava/lang/String;LEpochWriter;ILjava/util/List;Ljava/time/format/DateTimeFormatter;Ljava/lang/Boolean;)V
-  #112 = String             #271          // Unrecognised file format for:
-  #113 = Methodref          #148.#272     // EpochWriter.closeWriters:()V
-  #114 = Class              #273          // java/lang/Exception
-  #115 = Methodref          #114.#274     // java/lang/Exception.printStackTrace:(Ljava/io/PrintStream;)V
-  #116 = String             #275          // error reading/writing file
-  #117 = String             #276          // :
-  #118 = Methodref          #114.#178     // java/lang/Exception.toString:()Ljava/lang/String;
+   #19 = Class              #176          // java/lang/Integer
+   #20 = Methodref          #19.#177      // java/lang/Integer.valueOf:(I)Ljava/lang/Integer;
+   #21 = Methodref          #178.#179     // java/util/Arrays.asList:([Ljava/lang/Object;)Ljava/util/List;
+   #22 = String             #180          // Invalid input,
+   #23 = Class              #181          // java/lang/StringBuilder
+   #24 = Methodref          #23.#159      // java/lang/StringBuilder."<init>":()V
+   #25 = Methodref          #23.#182      // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+   #26 = String             #183          // please enter at least 1 parameter, e.g.\n
+   #27 = Methodref          #23.#184      // java/lang/StringBuilder.toString:()Ljava/lang/String;
+   #28 = String             #185          // java AccelerometerParser inputFile.cwa.gz
+   #29 = Fieldref           #186.#187     // java/lang/System.out:Ljava/io/PrintStream;
+   #30 = Methodref          #188.#189     // java/io/PrintStream.println:(Ljava/lang/String;)V
+   #31 = Methodref          #186.#190     // java/lang/System.exit:(I)V
+   #32 = String             #191          // \\.
+   #33 = Methodref          #2.#192       // java/lang/String.split:(Ljava/lang/String;)[Ljava/lang/String;
+   #34 = String             #193          // Epoch.csv
+   #35 = Methodref          #178.#194     // java/util/Arrays.copyOfRange:([Ljava/lang/Object;II)[Ljava/lang/Object;
+   #36 = Class              #195          // "[Ljava/lang/String;"
+   #37 = Class              #196          // java/text/SimpleDateFormat
+   #38 = String             #197          // yyyy-M-d\'T\'H:m
+   #39 = Methodref          #37.#198      // java/text/SimpleDateFormat."<init>":(Ljava/lang/String;)V
+   #40 = String             #199          // UTC
+   #41 = Methodref          #200.#201     // java/util/TimeZone.getTimeZone:(Ljava/lang/String;)Ljava/util/TimeZone;
+   #42 = Methodref          #37.#202      // java/text/SimpleDateFormat.setTimeZone:(Ljava/util/TimeZone;)V
+   #43 = String             #203          // :
+   #44 = Methodref          #2.#204       // java/lang/String.indexOf:(Ljava/lang/String;)I
+   #45 = Methodref          #2.#205       // java/lang/String.substring:(I)Ljava/lang/String;
+   #46 = String             #206          // timeZone
+   #47 = Methodref          #2.#207       // java/lang/String.equals:(Ljava/lang/Object;)Z
+   #48 = String             #208          // timeShift
+   #49 = Methodref          #19.#209      // java/lang/Integer.parseInt:(Ljava/lang/String;)I
+   #50 = String             #210          // outputFile
+   #51 = String             #211          // verbose
+   #52 = Methodref          #2.#212       // java/lang/String.toLowerCase:()Ljava/lang/String;
+   #53 = Methodref          #163.#213     // java/lang/Boolean.parseBoolean:(Ljava/lang/String;)Z
+   #54 = String             #214          // epochPeriod
+   #55 = String             #215          // filter
+   #56 = String             #216          // getStationaryBouts
+   #57 = String             #217          // stationaryStd
+   #58 = Methodref          #218.#219     // java/lang/Double.parseDouble:(Ljava/lang/String;)D
+   #59 = String             #220          // xIntercept
+   #60 = String             #221          // yIntercept
+   #61 = String             #222          // zIntercept
+   #62 = String             #223          // xSlope
+   #63 = String             #224          // ySlope
+   #64 = String             #225          // zSlope
+   #65 = String             #226          // xSlopeT
+   #66 = String             #227          // ySlopeT
+   #67 = String             #228          // zSlopeT
+   #68 = String             #229          // sampleRate
+   #69 = String             #230          // resampleMethod
+   #70 = String             #231          // range
+   #71 = String             #232          // rawOutput
+   #72 = String             #233          // rawFile
+   #73 = String             #234          // npyOutput
+   #74 = String             #235          // npyFile
+   #75 = String             #236          // startTime
+   #76 = String             #237          // endTime
+   #77 = String             #238          // csvTimeXYZTempColsIndex
+   #78 = String             #239          // ,
+   #79 = Fieldref           #186.#240     // java/lang/System.err:Ljava/io/PrintStream;
+   #80 = String             #241          // error parsing csvTimeXYZTempColsIndex:
+   #81 = Methodref          #132.#184     // java/lang/Object.toString:()Ljava/lang/String;
+   #82 = String             #242          // \n must be 4 or 5 comma separated integers
+   #83 = Class              #243          // java/util/LinkedList
+   #84 = Methodref          #83.#159      // java/util/LinkedList."<init>":()V
+   #85 = InterfaceMethodref #244.#245     // java/util/List.add:(Ljava/lang/Object;)Z
+   #86 = String             #246          // csvStartRow
+   #87 = String             #247          // getFeatures
+   #88 = String             #248          // csvTimeFormat
+   #89 = String             #249          // unknown parameter
+   #90 = Methodref          #2.#250       // java/lang/String.isEmpty:()Z
+   #91 = Methodref          #37.#251      // java/text/SimpleDateFormat.parse:(Ljava/lang/String;)Ljava/util/Date;
+   #92 = Methodref          #252.#253     // java/util/Date.getTime:()J
+   #93 = Class              #254          // java/text/ParseException
+   #94 = String             #255          // error parsing startTime:\'
+   #95 = String             #256          // \', must be in format: 1996-7-30T13:59
+   #96 = String             #257          // error parsing endTime:\'
+   #97 = String             #258          // Intermediate file:
+   #98 = Methodref          #163.#259     // java/lang/Boolean.booleanValue:()Z
+   #99 = Methodref          #260.#261     // DeviceReader.setupEpochWriter:(Ljava/lang/String;ZZLjava/lang/String;ZLjava/lang/String;ZLjava/time/format/DateTimeFormatter;Ljava/lang/String;IILjava/lang/String;I[D[D[DZDJJZ)LEpochWriter;
+  #100 = String             #262          // .cwa
+  #101 = Methodref          #2.#263       // java/lang/String.endsWith:(Ljava/lang/String;)Z
+  #102 = Methodref          #264.#265     // AxivityReader.readCwaEpochs:(Ljava/lang/String;Ljava/lang/String;ILEpochWriter;Ljava/lang/Boolean;)V
+  #103 = String             #266          // .cwa.gz
+  #104 = Methodref          #264.#267     // AxivityReader.readCwaGzEpochs:(Ljava/lang/String;Ljava/lang/String;ILEpochWriter;Ljava/lang/Boolean;)V
+  #105 = String             #268          // .bin
+  #106 = Methodref          #269.#270     // GENEActivReader.readGeneaEpochs:(Ljava/lang/String;Ljava/lang/String;ILEpochWriter;Ljava/lang/Boolean;)V
+  #107 = String             #271          // .gt3x
+  #108 = Methodref          #272.#273     // ActigraphReader.readG3TXEpochs:(Ljava/lang/String;LEpochWriter;Ljava/lang/Boolean;)V
+  #109 = String             #274          // .csv
+  #110 = String             #275          // .csv.gz
+  #111 = Methodref          #276.#277     // CsvReader.readCSVEpochs:(Ljava/lang/String;LEpochWriter;ILjava/util/List;Ljava/time/format/DateTimeFormatter;Ljava/lang/Boolean;)V
+  #112 = String             #278          // Unrecognised file format for:
+  #113 = Methodref          #279.#280     // EpochWriter.closeWriters:()V
+  #114 = Class              #281          // java/lang/Exception
+  #115 = Methodref          #114.#282     // java/lang/Exception.printStackTrace:(Ljava/io/PrintStream;)V
+  #116 = String             #283          // error reading/writing file
+  #117 = String             #284          // :
+  #118 = Methodref          #114.#184     // java/lang/Exception.toString:()Ljava/lang/String;
   #119 = Long               1000l
-  #121 = Methodref          #277.#278     // java/lang/Math.floor:(D)D
-  #122 = Fieldref           #279.#280     // java/util/concurrent/TimeUnit.MILLISECONDS:Ljava/util/concurrent/TimeUnit;
-  #123 = Methodref          #279.#281     // java/util/concurrent/TimeUnit.toNanos:(J)J
-  #124 = Fieldref           #282.#283     // java/time/ZoneOffset.UTC:Ljava/time/ZoneOffset;
-  #125 = Methodref          #284.#285     // java/time/LocalDateTime.ofEpochSecond:(JILjava/time/ZoneOffset;)Ljava/time/LocalDateTime;
-  #126 = Class              #286          // java/text/DecimalFormat
-  #127 = String             #287          // 0.000000
-  #128 = Methodref          #126.#192     // java/text/DecimalFormat."<init>":(Ljava/lang/String;)V
-  #129 = String             #288          // 0.000
-  #130 = String             #289          // 0.00
-  #131 = Class              #290          // AccelerometerParser
-  #132 = Class              #291          // java/lang/Object
+  #121 = Methodref          #285.#286     // java/lang/Math.floor:(D)D
+  #122 = Fieldref           #287.#288     // java/util/concurrent/TimeUnit.MILLISECONDS:Ljava/util/concurrent/TimeUnit;
+  #123 = Methodref          #287.#289     // java/util/concurrent/TimeUnit.toNanos:(J)J
+  #124 = Fieldref           #290.#291     // java/time/ZoneOffset.UTC:Ljava/time/ZoneOffset;
+  #125 = Methodref          #292.#293     // java/time/LocalDateTime.ofEpochSecond:(JILjava/time/ZoneOffset;)Ljava/time/LocalDateTime;
+  #126 = Class              #294          // java/text/DecimalFormat
+  #127 = String             #295          // 0.000000
+  #128 = Methodref          #126.#198     // java/text/DecimalFormat."<init>":(Ljava/lang/String;)V
+  #129 = String             #296          // 0.000
+  #130 = String             #297          // 0.00
+  #131 = Class              #298          // AccelerometerParser
+  #132 = Class              #299          // java/lang/Object
   #133 = Utf8               DF6
   #134 = Utf8               Ljava/text/DecimalFormat;
   #135 = Utf8               DF3
   #136 = Utf8               DF2
   #137 = Utf8               <init>
   #138 = Utf8               ()V
   #139 = Utf8               Code
   #140 = Utf8               LineNumberTable
   #141 = Utf8               main
   #142 = Utf8               ([Ljava/lang/String;)V
   #143 = Utf8               StackMapTable
-  #144 = Class              #292          // java/lang/Boolean
-  #145 = Class              #293          // java/time/format/DateTimeFormatter
-  #146 = Class              #294          // "[D"
-  #147 = Class              #295          // java/util/List
-  #148 = Class              #296          // EpochWriter
-  #149 = Class              #297          // java/lang/Throwable
-  #150 = Utf8               epochMillisToLocalDateTime
-  #151 = Utf8               (J)Ljava/time/LocalDateTime;
-  #152 = Utf8               <clinit>
-  #153 = Utf8               SourceFile
-  #154 = Utf8               AccelerometerParser.java
-  #155 = NameAndType        #137:#138     // "<init>":()V
-  #156 = Utf8               java/lang/String
-  #157 = Utf8
-  #158 = Utf8               Europe/London
-  #159 = NameAndType        #298:#299     // valueOf:(Z)Ljava/lang/Boolean;
-  #160 = NameAndType        #133:#134     // DF6:Ljava/text/DecimalFormat;
-  #161 = Class              #300          // java/math/RoundingMode
-  #162 = NameAndType        #301:#302     // CEILING:Ljava/math/RoundingMode;
-  #163 = NameAndType        #303:#304     // setRoundingMode:(Ljava/math/RoundingMode;)V
-  #164 = NameAndType        #136:#134     // DF2:Ljava/text/DecimalFormat;
-  #165 = NameAndType        #135:#134     // DF3:Ljava/text/DecimalFormat;
-  #166 = NameAndType        #305:#302     // HALF_UP:Ljava/math/RoundingMode;
-  #167 = Utf8               yyyy-MM-dd HH:mm:ss.SSSxxxx \'[\'VV\']\'
-  #168 = NameAndType        #306:#307     // ofPattern:(Ljava/lang/String;)Ljava/time/format/DateTimeFormatter;
-  #169 = Utf8               linear
-  #170 = Utf8               java/lang/Integer
-  #171 = NameAndType        #298:#308     // valueOf:(I)Ljava/lang/Integer;
-  #172 = Class              #309          // java/util/Arrays
-  #173 = NameAndType        #310:#311     // asList:([Ljava/lang/Object;)Ljava/util/List;
-  #174 = Utf8               Invalid input,
-  #175 = Utf8               java/lang/StringBuilder
-  #176 = NameAndType        #312:#313     // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #177 = Utf8               please enter at least 1 parameter, e.g.\n
-  #178 = NameAndType        #314:#315     // toString:()Ljava/lang/String;
-  #179 = Utf8               java AccelerometerParser inputFile.cwa.gz
-  #180 = Class              #316          // java/lang/System
-  #181 = NameAndType        #317:#318     // out:Ljava/io/PrintStream;
-  #182 = Class              #319          // java/io/PrintStream
-  #183 = NameAndType        #320:#321     // println:(Ljava/lang/String;)V
-  #184 = NameAndType        #322:#323     // exit:(I)V
-  #185 = Utf8               \\.
-  #186 = NameAndType        #324:#325     // split:(Ljava/lang/String;)[Ljava/lang/String;
-  #187 = Utf8               Epoch.csv
-  #188 = NameAndType        #326:#327     // copyOfRange:([Ljava/lang/Object;II)[Ljava/lang/Object;
-  #189 = Utf8               [Ljava/lang/String;
-  #190 = Utf8               java/text/SimpleDateFormat
-  #191 = Utf8               yyyy-M-d\'T\'H:m
-  #192 = NameAndType        #137:#321     // "<init>":(Ljava/lang/String;)V
-  #193 = Utf8               UTC
-  #194 = Class              #328          // java/util/TimeZone
-  #195 = NameAndType        #329:#330     // getTimeZone:(Ljava/lang/String;)Ljava/util/TimeZone;
-  #196 = NameAndType        #331:#332     // setTimeZone:(Ljava/util/TimeZone;)V
-  #197 = Utf8               :
-  #198 = NameAndType        #333:#334     // indexOf:(Ljava/lang/String;)I
-  #199 = NameAndType        #335:#336     // substring:(I)Ljava/lang/String;
-  #200 = Utf8               timeZone
-  #201 = NameAndType        #337:#338     // equals:(Ljava/lang/Object;)Z
-  #202 = Utf8               timeShift
-  #203 = NameAndType        #339:#334     // parseInt:(Ljava/lang/String;)I
-  #204 = Utf8               outputFile
-  #205 = Utf8               verbose
-  #206 = NameAndType        #340:#315     // toLowerCase:()Ljava/lang/String;
-  #207 = NameAndType        #341:#342     // parseBoolean:(Ljava/lang/String;)Z
-  #208 = Utf8               epochPeriod
-  #209 = Utf8               filter
-  #210 = Utf8               getStationaryBouts
-  #211 = Utf8               stationaryStd
-  #212 = Class              #343          // java/lang/Double
-  #213 = NameAndType        #344:#345     // parseDouble:(Ljava/lang/String;)D
-  #214 = Utf8               xIntercept
-  #215 = Utf8               yIntercept
-  #216 = Utf8               zIntercept
-  #217 = Utf8               xSlope
-  #218 = Utf8               ySlope
-  #219 = Utf8               zSlope
-  #220 = Utf8               xSlopeT
-  #221 = Utf8               ySlopeT
-  #222 = Utf8               zSlopeT
-  #223 = Utf8               sampleRate
-  #224 = Utf8               resampleMethod
-  #225 = Utf8               range
-  #226 = Utf8               rawOutput
-  #227 = Utf8               rawFile
-  #228 = Utf8               npyOutput
-  #229 = Utf8               npyFile
-  #230 = Utf8               startTime
-  #231 = Utf8               endTime
-  #232 = Utf8               csvTimeXYZTempColsIndex
-  #233 = Utf8               ,
-  #234 = NameAndType        #346:#318     // err:Ljava/io/PrintStream;
-  #235 = Utf8               error parsing csvTimeXYZTempColsIndex:
-  #236 = Utf8               \n must be 4 or 5 comma separated integers
-  #237 = Utf8               java/util/LinkedList
-  #238 = NameAndType        #347:#338     // add:(Ljava/lang/Object;)Z
-  #239 = Utf8               csvStartRow
-  #240 = Utf8               getFeatures
-  #241 = Utf8               csvTimeFormat
-  #242 = Utf8               unknown parameter
-  #243 = NameAndType        #348:#349     // isEmpty:()Z
-  #244 = NameAndType        #350:#351     // parse:(Ljava/lang/String;)Ljava/util/Date;
-  #245 = Class              #352          // java/util/Date
-  #246 = NameAndType        #353:#354     // getTime:()J
-  #247 = Utf8               java/text/ParseException
-  #248 = Utf8               error parsing startTime:\'
-  #249 = Utf8               \', must be in format: 1996-7-30T13:59
-  #250 = Utf8               error parsing endTime:\'
-  #251 = Utf8               Intermediate file:
-  #252 = NameAndType        #355:#349     // booleanValue:()Z
-  #253 = Class              #356          // DeviceReader
-  #254 = NameAndType        #357:#358     // setupEpochWriter:(Ljava/lang/String;ZZLjava/lang/String;ZLjava/lang/String;ZLjava/time/format/DateTimeFormatter;Ljava/lang/String;IILjava/lang/String;I[D[D[DZDJJZ)LEpochWriter;
-  #255 = Utf8               .cwa
-  #256 = NameAndType        #359:#342     // endsWith:(Ljava/lang/String;)Z
-  #257 = Class              #360          // AxivityReader
-  #258 = NameAndType        #361:#362     // readCwaEpochs:(Ljava/lang/String;Ljava/lang/String;ILEpochWriter;Ljava/lang/Boolean;)V
-  #259 = Utf8               .cwa.gz
-  #260 = NameAndType        #363:#362     // readCwaGzEpochs:(Ljava/lang/String;Ljava/lang/String;ILEpochWriter;Ljava/lang/Boolean;)V
-  #261 = Utf8               .bin
-  #262 = Class              #364          // GENEActivReader
-  #263 = NameAndType        #365:#362     // readGeneaEpochs:(Ljava/lang/String;Ljava/lang/String;ILEpochWriter;Ljava/lang/Boolean;)V
-  #264 = Utf8               .gt3x
-  #265 = Class              #366          // ActigraphReader
-  #266 = NameAndType        #367:#368     // readG3TXEpochs:(Ljava/lang/String;LEpochWriter;Ljava/lang/Boolean;)V
-  #267 = Utf8               .csv
-  #268 = Utf8               .csv.gz
-  #269 = Class              #369          // CsvReader
-  #270 = NameAndType        #370:#371     // readCSVEpochs:(Ljava/lang/String;LEpochWriter;ILjava/util/List;Ljava/time/format/DateTimeFormatter;Ljava/lang/Boolean;)V
-  #271 = Utf8               Unrecognised file format for:
-  #272 = NameAndType        #372:#138     // closeWriters:()V
-  #273 = Utf8               java/lang/Exception
-  #274 = NameAndType        #373:#374     // printStackTrace:(Ljava/io/PrintStream;)V
-  #275 = Utf8               error reading/writing file
-  #276 = Utf8               :
-  #277 = Class              #375          // java/lang/Math
-  #278 = NameAndType        #376:#377     // floor:(D)D
-  #279 = Class              #378          // java/util/concurrent/TimeUnit
-  #280 = NameAndType        #379:#380     // MILLISECONDS:Ljava/util/concurrent/TimeUnit;
-  #281 = NameAndType        #381:#382     // toNanos:(J)J
-  #282 = Class              #383          // java/time/ZoneOffset
-  #283 = NameAndType        #193:#384     // UTC:Ljava/time/ZoneOffset;
-  #284 = Class              #385          // java/time/LocalDateTime
-  #285 = NameAndType        #386:#387     // ofEpochSecond:(JILjava/time/ZoneOffset;)Ljava/time/LocalDateTime;
-  #286 = Utf8               java/text/DecimalFormat
-  #287 = Utf8               0.000000
-  #288 = Utf8               0.000
-  #289 = Utf8               0.00
-  #290 = Utf8               AccelerometerParser
-  #291 = Utf8               java/lang/Object
-  #292 = Utf8               java/lang/Boolean
-  #293 = Utf8               java/time/format/DateTimeFormatter
-  #294 = Utf8               [D
-  #295 = Utf8               java/util/List
-  #296 = Utf8               EpochWriter
-  #297 = Utf8               java/lang/Throwable
-  #298 = Utf8               valueOf
-  #299 = Utf8               (Z)Ljava/lang/Boolean;
-  #300 = Utf8               java/math/RoundingMode
-  #301 = Utf8               CEILING
-  #302 = Utf8               Ljava/math/RoundingMode;
-  #303 = Utf8               setRoundingMode
-  #304 = Utf8               (Ljava/math/RoundingMode;)V
-  #305 = Utf8               HALF_UP
-  #306 = Utf8               ofPattern
-  #307 = Utf8               (Ljava/lang/String;)Ljava/time/format/DateTimeFormatter;
-  #308 = Utf8               (I)Ljava/lang/Integer;
-  #309 = Utf8               java/util/Arrays
-  #310 = Utf8               asList
-  #311 = Utf8               ([Ljava/lang/Object;)Ljava/util/List;
-  #312 = Utf8               append
-  #313 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #314 = Utf8               toString
-  #315 = Utf8               ()Ljava/lang/String;
-  #316 = Utf8               java/lang/System
-  #317 = Utf8               out
-  #318 = Utf8               Ljava/io/PrintStream;
-  #319 = Utf8               java/io/PrintStream
-  #320 = Utf8               println
-  #321 = Utf8               (Ljava/lang/String;)V
-  #322 = Utf8               exit
-  #323 = Utf8               (I)V
-  #324 = Utf8               split
-  #325 = Utf8               (Ljava/lang/String;)[Ljava/lang/String;
-  #326 = Utf8               copyOfRange
-  #327 = Utf8               ([Ljava/lang/Object;II)[Ljava/lang/Object;
-  #328 = Utf8               java/util/TimeZone
-  #329 = Utf8               getTimeZone
-  #330 = Utf8               (Ljava/lang/String;)Ljava/util/TimeZone;
-  #331 = Utf8               setTimeZone
-  #332 = Utf8               (Ljava/util/TimeZone;)V
-  #333 = Utf8               indexOf
-  #334 = Utf8               (Ljava/lang/String;)I
-  #335 = Utf8               substring
-  #336 = Utf8               (I)Ljava/lang/String;
-  #337 = Utf8               equals
-  #338 = Utf8               (Ljava/lang/Object;)Z
-  #339 = Utf8               parseInt
-  #340 = Utf8               toLowerCase
-  #341 = Utf8               parseBoolean
-  #342 = Utf8               (Ljava/lang/String;)Z
-  #343 = Utf8               java/lang/Double
-  #344 = Utf8               parseDouble
-  #345 = Utf8               (Ljava/lang/String;)D
-  #346 = Utf8               err
-  #347 = Utf8               add
-  #348 = Utf8               isEmpty
-  #349 = Utf8               ()Z
-  #350 = Utf8               parse
-  #351 = Utf8               (Ljava/lang/String;)Ljava/util/Date;
-  #352 = Utf8               java/util/Date
-  #353 = Utf8               getTime
-  #354 = Utf8               ()J
-  #355 = Utf8               booleanValue
-  #356 = Utf8               DeviceReader
-  #357 = Utf8               setupEpochWriter
-  #358 = Utf8               (Ljava/lang/String;ZZLjava/lang/String;ZLjava/lang/String;ZLjava/time/format/DateTimeFormatter;Ljava/lang/String;IILjava/lang/String;I[D[D[DZDJJZ)LEpochWriter;
-  #359 = Utf8               endsWith
-  #360 = Utf8               AxivityReader
-  #361 = Utf8               readCwaEpochs
-  #362 = Utf8               (Ljava/lang/String;Ljava/lang/String;ILEpochWriter;Ljava/lang/Boolean;)V
-  #363 = Utf8               readCwaGzEpochs
-  #364 = Utf8               GENEActivReader
-  #365 = Utf8               readGeneaEpochs
-  #366 = Utf8               ActigraphReader
-  #367 = Utf8               readG3TXEpochs
-  #368 = Utf8               (Ljava/lang/String;LEpochWriter;Ljava/lang/Boolean;)V
-  #369 = Utf8               CsvReader
-  #370 = Utf8               readCSVEpochs
-  #371 = Utf8               (Ljava/lang/String;LEpochWriter;ILjava/util/List;Ljava/time/format/DateTimeFormatter;Ljava/lang/Boolean;)V
-  #372 = Utf8               closeWriters
-  #373 = Utf8               printStackTrace
-  #374 = Utf8               (Ljava/io/PrintStream;)V
-  #375 = Utf8               java/lang/Math
-  #376 = Utf8               floor
-  #377 = Utf8               (D)D
-  #378 = Utf8               java/util/concurrent/TimeUnit
-  #379 = Utf8               MILLISECONDS
-  #380 = Utf8               Ljava/util/concurrent/TimeUnit;
-  #381 = Utf8               toNanos
-  #382 = Utf8               (J)J
-  #383 = Utf8               java/time/ZoneOffset
-  #384 = Utf8               Ljava/time/ZoneOffset;
-  #385 = Utf8               java/time/LocalDateTime
-  #386 = Utf8               ofEpochSecond
-  #387 = Utf8               (JILjava/time/ZoneOffset;)Ljava/time/LocalDateTime;
+  #144 = Class              #160          // java/lang/String
+  #145 = Class              #300          // java/lang/Boolean
+  #146 = Class              #301          // java/time/format/DateTimeFormatter
+  #147 = Class              #302          // "[D"
+  #148 = Class              #303          // java/util/List
+  #149 = Class              #196          // java/text/SimpleDateFormat
+  #150 = Class              #254          // java/text/ParseException
+  #151 = Class              #304          // EpochWriter
+  #152 = Class              #281          // java/lang/Exception
+  #153 = Class              #305          // java/lang/Throwable
+  #154 = Utf8               epochMillisToLocalDateTime
+  #155 = Utf8               (J)Ljava/time/LocalDateTime;
+  #156 = Utf8               <clinit>
+  #157 = Utf8               SourceFile
+  #158 = Utf8               AccelerometerParser.java
+  #159 = NameAndType        #137:#138     // "<init>":()V
+  #160 = Utf8               java/lang/String
+  #161 = Utf8
+  #162 = Utf8               Europe/London
+  #163 = Class              #300          // java/lang/Boolean
+  #164 = NameAndType        #306:#307     // valueOf:(Z)Ljava/lang/Boolean;
+  #165 = NameAndType        #133:#134     // DF6:Ljava/text/DecimalFormat;
+  #166 = Class              #308          // java/math/RoundingMode
+  #167 = NameAndType        #309:#310     // CEILING:Ljava/math/RoundingMode;
+  #168 = NameAndType        #311:#312     // setRoundingMode:(Ljava/math/RoundingMode;)V
+  #169 = NameAndType        #136:#134     // DF2:Ljava/text/DecimalFormat;
+  #170 = NameAndType        #135:#134     // DF3:Ljava/text/DecimalFormat;
+  #171 = NameAndType        #313:#310     // HALF_UP:Ljava/math/RoundingMode;
+  #172 = Utf8               yyyy-MM-dd HH:mm:ss.SSSxxxx \'[\'VV\']\'
+  #173 = Class              #301          // java/time/format/DateTimeFormatter
+  #174 = NameAndType        #314:#315     // ofPattern:(Ljava/lang/String;)Ljava/time/format/DateTimeFormatter;
+  #175 = Utf8               linear
+  #176 = Utf8               java/lang/Integer
+  #177 = NameAndType        #306:#316     // valueOf:(I)Ljava/lang/Integer;
+  #178 = Class              #317          // java/util/Arrays
+  #179 = NameAndType        #318:#319     // asList:([Ljava/lang/Object;)Ljava/util/List;
+  #180 = Utf8               Invalid input,
+  #181 = Utf8               java/lang/StringBuilder
+  #182 = NameAndType        #320:#321     // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #183 = Utf8               please enter at least 1 parameter, e.g.\n
+  #184 = NameAndType        #322:#323     // toString:()Ljava/lang/String;
+  #185 = Utf8               java AccelerometerParser inputFile.cwa.gz
+  #186 = Class              #324          // java/lang/System
+  #187 = NameAndType        #325:#326     // out:Ljava/io/PrintStream;
+  #188 = Class              #327          // java/io/PrintStream
+  #189 = NameAndType        #328:#329     // println:(Ljava/lang/String;)V
+  #190 = NameAndType        #330:#331     // exit:(I)V
+  #191 = Utf8               \\.
+  #192 = NameAndType        #332:#333     // split:(Ljava/lang/String;)[Ljava/lang/String;
+  #193 = Utf8               Epoch.csv
+  #194 = NameAndType        #334:#335     // copyOfRange:([Ljava/lang/Object;II)[Ljava/lang/Object;
+  #195 = Utf8               [Ljava/lang/String;
+  #196 = Utf8               java/text/SimpleDateFormat
+  #197 = Utf8               yyyy-M-d\'T\'H:m
+  #198 = NameAndType        #137:#329     // "<init>":(Ljava/lang/String;)V
+  #199 = Utf8               UTC
+  #200 = Class              #336          // java/util/TimeZone
+  #201 = NameAndType        #337:#338     // getTimeZone:(Ljava/lang/String;)Ljava/util/TimeZone;
+  #202 = NameAndType        #339:#340     // setTimeZone:(Ljava/util/TimeZone;)V
+  #203 = Utf8               :
+  #204 = NameAndType        #341:#342     // indexOf:(Ljava/lang/String;)I
+  #205 = NameAndType        #343:#344     // substring:(I)Ljava/lang/String;
+  #206 = Utf8               timeZone
+  #207 = NameAndType        #345:#346     // equals:(Ljava/lang/Object;)Z
+  #208 = Utf8               timeShift
+  #209 = NameAndType        #347:#342     // parseInt:(Ljava/lang/String;)I
+  #210 = Utf8               outputFile
+  #211 = Utf8               verbose
+  #212 = NameAndType        #348:#323     // toLowerCase:()Ljava/lang/String;
+  #213 = NameAndType        #349:#350     // parseBoolean:(Ljava/lang/String;)Z
+  #214 = Utf8               epochPeriod
+  #215 = Utf8               filter
+  #216 = Utf8               getStationaryBouts
+  #217 = Utf8               stationaryStd
+  #218 = Class              #351          // java/lang/Double
+  #219 = NameAndType        #352:#353     // parseDouble:(Ljava/lang/String;)D
+  #220 = Utf8               xIntercept
+  #221 = Utf8               yIntercept
+  #222 = Utf8               zIntercept
+  #223 = Utf8               xSlope
+  #224 = Utf8               ySlope
+  #225 = Utf8               zSlope
+  #226 = Utf8               xSlopeT
+  #227 = Utf8               ySlopeT
+  #228 = Utf8               zSlopeT
+  #229 = Utf8               sampleRate
+  #230 = Utf8               resampleMethod
+  #231 = Utf8               range
+  #232 = Utf8               rawOutput
+  #233 = Utf8               rawFile
+  #234 = Utf8               npyOutput
+  #235 = Utf8               npyFile
+  #236 = Utf8               startTime
+  #237 = Utf8               endTime
+  #238 = Utf8               csvTimeXYZTempColsIndex
+  #239 = Utf8               ,
+  #240 = NameAndType        #354:#326     // err:Ljava/io/PrintStream;
+  #241 = Utf8               error parsing csvTimeXYZTempColsIndex:
+  #242 = Utf8               \n must be 4 or 5 comma separated integers
+  #243 = Utf8               java/util/LinkedList
+  #244 = Class              #303          // java/util/List
+  #245 = NameAndType        #355:#346     // add:(Ljava/lang/Object;)Z
+  #246 = Utf8               csvStartRow
+  #247 = Utf8               getFeatures
+  #248 = Utf8               csvTimeFormat
+  #249 = Utf8               unknown parameter
+  #250 = NameAndType        #356:#357     // isEmpty:()Z
+  #251 = NameAndType        #358:#359     // parse:(Ljava/lang/String;)Ljava/util/Date;
+  #252 = Class              #360          // java/util/Date
+  #253 = NameAndType        #361:#362     // getTime:()J
+  #254 = Utf8               java/text/ParseException
+  #255 = Utf8               error parsing startTime:\'
+  #256 = Utf8               \', must be in format: 1996-7-30T13:59
+  #257 = Utf8               error parsing endTime:\'
+  #258 = Utf8               Intermediate file:
+  #259 = NameAndType        #363:#357     // booleanValue:()Z
+  #260 = Class              #364          // DeviceReader
+  #261 = NameAndType        #365:#366     // setupEpochWriter:(Ljava/lang/String;ZZLjava/lang/String;ZLjava/lang/String;ZLjava/time/format/DateTimeFormatter;Ljava/lang/String;IILjava/lang/String;I[D[D[DZDJJZ)LEpochWriter;
+  #262 = Utf8               .cwa
+  #263 = NameAndType        #367:#350     // endsWith:(Ljava/lang/String;)Z
+  #264 = Class              #368          // AxivityReader
+  #265 = NameAndType        #369:#370     // readCwaEpochs:(Ljava/lang/String;Ljava/lang/String;ILEpochWriter;Ljava/lang/Boolean;)V
+  #266 = Utf8               .cwa.gz
+  #267 = NameAndType        #371:#370     // readCwaGzEpochs:(Ljava/lang/String;Ljava/lang/String;ILEpochWriter;Ljava/lang/Boolean;)V
+  #268 = Utf8               .bin
+  #269 = Class              #372          // GENEActivReader
+  #270 = NameAndType        #373:#370     // readGeneaEpochs:(Ljava/lang/String;Ljava/lang/String;ILEpochWriter;Ljava/lang/Boolean;)V
+  #271 = Utf8               .gt3x
+  #272 = Class              #374          // ActigraphReader
+  #273 = NameAndType        #375:#376     // readG3TXEpochs:(Ljava/lang/String;LEpochWriter;Ljava/lang/Boolean;)V
+  #274 = Utf8               .csv
+  #275 = Utf8               .csv.gz
+  #276 = Class              #377          // CsvReader
+  #277 = NameAndType        #378:#379     // readCSVEpochs:(Ljava/lang/String;LEpochWriter;ILjava/util/List;Ljava/time/format/DateTimeFormatter;Ljava/lang/Boolean;)V
+  #278 = Utf8               Unrecognised file format for:
+  #279 = Class              #304          // EpochWriter
+  #280 = NameAndType        #380:#138     // closeWriters:()V
+  #281 = Utf8               java/lang/Exception
+  #282 = NameAndType        #381:#382     // printStackTrace:(Ljava/io/PrintStream;)V
+  #283 = Utf8               error reading/writing file
+  #284 = Utf8               :
+  #285 = Class              #383          // java/lang/Math
+  #286 = NameAndType        #384:#385     // floor:(D)D
+  #287 = Class              #386          // java/util/concurrent/TimeUnit
+  #288 = NameAndType        #387:#388     // MILLISECONDS:Ljava/util/concurrent/TimeUnit;
+  #289 = NameAndType        #389:#390     // toNanos:(J)J
+  #290 = Class              #391          // java/time/ZoneOffset
+  #291 = NameAndType        #199:#392     // UTC:Ljava/time/ZoneOffset;
+  #292 = Class              #393          // java/time/LocalDateTime
+  #293 = NameAndType        #394:#395     // ofEpochSecond:(JILjava/time/ZoneOffset;)Ljava/time/LocalDateTime;
+  #294 = Utf8               java/text/DecimalFormat
+  #295 = Utf8               0.000000
+  #296 = Utf8               0.000
+  #297 = Utf8               0.00
+  #298 = Utf8               AccelerometerParser
+  #299 = Utf8               java/lang/Object
+  #300 = Utf8               java/lang/Boolean
+  #301 = Utf8               java/time/format/DateTimeFormatter
+  #302 = Utf8               [D
+  #303 = Utf8               java/util/List
+  #304 = Utf8               EpochWriter
+  #305 = Utf8               java/lang/Throwable
+  #306 = Utf8               valueOf
+  #307 = Utf8               (Z)Ljava/lang/Boolean;
+  #308 = Utf8               java/math/RoundingMode
+  #309 = Utf8               CEILING
+  #310 = Utf8               Ljava/math/RoundingMode;
+  #311 = Utf8               setRoundingMode
+  #312 = Utf8               (Ljava/math/RoundingMode;)V
+  #313 = Utf8               HALF_UP
+  #314 = Utf8               ofPattern
+  #315 = Utf8               (Ljava/lang/String;)Ljava/time/format/DateTimeFormatter;
+  #316 = Utf8               (I)Ljava/lang/Integer;
+  #317 = Utf8               java/util/Arrays
+  #318 = Utf8               asList
+  #319 = Utf8               ([Ljava/lang/Object;)Ljava/util/List;
+  #320 = Utf8               append
+  #321 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #322 = Utf8               toString
+  #323 = Utf8               ()Ljava/lang/String;
+  #324 = Utf8               java/lang/System
+  #325 = Utf8               out
+  #326 = Utf8               Ljava/io/PrintStream;
+  #327 = Utf8               java/io/PrintStream
+  #328 = Utf8               println
+  #329 = Utf8               (Ljava/lang/String;)V
+  #330 = Utf8               exit
+  #331 = Utf8               (I)V
+  #332 = Utf8               split
+  #333 = Utf8               (Ljava/lang/String;)[Ljava/lang/String;
+  #334 = Utf8               copyOfRange
+  #335 = Utf8               ([Ljava/lang/Object;II)[Ljava/lang/Object;
+  #336 = Utf8               java/util/TimeZone
+  #337 = Utf8               getTimeZone
+  #338 = Utf8               (Ljava/lang/String;)Ljava/util/TimeZone;
+  #339 = Utf8               setTimeZone
+  #340 = Utf8               (Ljava/util/TimeZone;)V
+  #341 = Utf8               indexOf
+  #342 = Utf8               (Ljava/lang/String;)I
+  #343 = Utf8               substring
+  #344 = Utf8               (I)Ljava/lang/String;
+  #345 = Utf8               equals
+  #346 = Utf8               (Ljava/lang/Object;)Z
+  #347 = Utf8               parseInt
+  #348 = Utf8               toLowerCase
+  #349 = Utf8               parseBoolean
+  #350 = Utf8               (Ljava/lang/String;)Z
+  #351 = Utf8               java/lang/Double
+  #352 = Utf8               parseDouble
+  #353 = Utf8               (Ljava/lang/String;)D
+  #354 = Utf8               err
+  #355 = Utf8               add
+  #356 = Utf8               isEmpty
+  #357 = Utf8               ()Z
+  #358 = Utf8               parse
+  #359 = Utf8               (Ljava/lang/String;)Ljava/util/Date;
+  #360 = Utf8               java/util/Date
+  #361 = Utf8               getTime
+  #362 = Utf8               ()J
+  #363 = Utf8               booleanValue
+  #364 = Utf8               DeviceReader
+  #365 = Utf8               setupEpochWriter
+  #366 = Utf8               (Ljava/lang/String;ZZLjava/lang/String;ZLjava/lang/String;ZLjava/time/format/DateTimeFormatter;Ljava/lang/String;IILjava/lang/String;I[D[D[DZDJJZ)LEpochWriter;
+  #367 = Utf8               endsWith
+  #368 = Utf8               AxivityReader
+  #369 = Utf8               readCwaEpochs
+  #370 = Utf8               (Ljava/lang/String;Ljava/lang/String;ILEpochWriter;Ljava/lang/Boolean;)V
+  #371 = Utf8               readCwaGzEpochs
+  #372 = Utf8               GENEActivReader
+  #373 = Utf8               readGeneaEpochs
+  #374 = Utf8               ActigraphReader
+  #375 = Utf8               readG3TXEpochs
+  #376 = Utf8               (Ljava/lang/String;LEpochWriter;Ljava/lang/Boolean;)V
+  #377 = Utf8               CsvReader
+  #378 = Utf8               readCSVEpochs
+  #379 = Utf8               (Ljava/lang/String;LEpochWriter;ILjava/util/List;Ljava/time/format/DateTimeFormatter;Ljava/lang/Boolean;)V
+  #380 = Utf8               closeWriters
+  #381 = Utf8               printStackTrace
+  #382 = Utf8               (Ljava/io/PrintStream;)V
+  #383 = Utf8               java/lang/Math
+  #384 = Utf8               floor
+  #385 = Utf8               (D)D
+  #386 = Utf8               java/util/concurrent/TimeUnit
+  #387 = Utf8               MILLISECONDS
+  #388 = Utf8               Ljava/util/concurrent/TimeUnit;
+  #389 = Utf8               toNanos
+  #390 = Utf8               (J)J
+  #391 = Utf8               java/time/ZoneOffset
+  #392 = Utf8               Ljava/time/ZoneOffset;
+  #393 = Utf8               java/time/LocalDateTime
+  #394 = Utf8               ofEpochSecond
+  #395 = Utf8               (JILjava/time/ZoneOffset;)Ljava/time/LocalDateTime;
 {
   private static final java.text.DecimalFormat DF6;
     descriptor: Ljava/text/DecimalFormat;
     flags: (0x001a) ACC_PRIVATE, ACC_STATIC, ACC_FINAL
 
   private static final java.text.DecimalFormat DF3;
     descriptor: Ljava/text/DecimalFormat;
```

### Comparing `accelerometer-6.2.3/accelerometer/java/AccelerometerParser.java` & `accelerometer-7.0.0.dev0/src/accelerometer/java/AccelerometerParser.java`

 * *Files identical despite different names*

### Comparing `accelerometer-6.2.3/accelerometer/java/ActigraphReader.class` & `accelerometer-7.0.0.dev0/src/accelerometer/java/ActigraphReader.class`

 * *Files 10% similar despite different names*

#### javap -verbose -constants -s -l -private {}

```diff
@@ -1,173 +1,173 @@
-  SHA-256 checksum 331285793d9b78fbe3d40b16012eaa54bbb97cac06a09fa0be3d97f6a866810a
+  SHA-256 checksum f04c521276ba85f50906453c8fa0e7c695d3224db327000f126982d212743762
   Compiled from "ActigraphReader.java"
 public class ActigraphReader extends DeviceReader
   minor version: 0
   major version: 52
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #29                         // ActigraphReader
   super_class: #170                       // DeviceReader
   interfaces: 0, fields: 5, methods: 17, attributes: 1
 Constant pool:
-    #1 = Methodref          #170.#231     // DeviceReader."<init>":()V
-    #2 = Class              #232          // java/util/zip/ZipFile
-    #3 = Class              #233          // java/io/File
-    #4 = Methodref          #3.#234       // java/io/File."<init>":(Ljava/lang/String;)V
-    #5 = Methodref          #2.#235       // java/util/zip/ZipFile."<init>":(Ljava/io/File;I)V
-    #6 = Methodref          #29.#236      // ActigraphReader.getGT3XVersion:(Ljava/util/zip/ZipFile;)I
-    #7 = Fieldref           #237.#238     // java/lang/System.err:Ljava/io/PrintStream;
-    #8 = Class              #239          // java/lang/StringBuilder
-    #9 = Methodref          #8.#231       // java/lang/StringBuilder."<init>":()V
-   #10 = String             #240          // file
-   #11 = Methodref          #8.#241       // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-   #12 = String             #242          //  is not a valid V1 or V2 g3tx file
-   #13 = Methodref          #8.#243       // java/lang/StringBuilder.toString:()Ljava/lang/String;
-   #14 = Methodref          #244.#245     // java/io/PrintStream.println:(Ljava/lang/String;)V
-   #15 = Methodref          #237.#246     // java/lang/System.exit:(I)V
-   #16 = Methodref          #2.#247       // java/util/zip/ZipFile.entries:()Ljava/util/Enumeration;
-   #17 = InterfaceMethodref #194.#248     // java/util/Enumeration.hasMoreElements:()Z
-   #18 = InterfaceMethodref #194.#249     // java/util/Enumeration.nextElement:()Ljava/lang/Object;
-   #19 = Class              #250          // java/util/zip/ZipEntry
-   #20 = Methodref          #19.#243      // java/util/zip/ZipEntry.toString:()Ljava/lang/String;
-   #21 = String             #251          // info.txt
-   #22 = Methodref          #190.#252     // java/lang/String.equals:(Ljava/lang/Object;)Z
-   #23 = Class              #253          // java/io/BufferedReader
-   #24 = Class              #254          // java/io/InputStreamReader
-   #25 = Methodref          #2.#255       // java/util/zip/ZipFile.getInputStream:(Ljava/util/zip/ZipEntry;)Ljava/io/InputStream;
-   #26 = Methodref          #24.#256      // java/io/InputStreamReader."<init>":(Ljava/io/InputStream;)V
-   #27 = Methodref          #23.#257      // java/io/BufferedReader."<init>":(Ljava/io/Reader;)V
-   #28 = String             #258          // activity.bin
-   #29 = Class              #259          // ActigraphReader
-   #30 = String             #260          // log.bin
+    #1 = Methodref          #170.#236     // DeviceReader."<init>":()V
+    #2 = Class              #237          // java/util/zip/ZipFile
+    #3 = Class              #238          // java/io/File
+    #4 = Methodref          #3.#239       // java/io/File."<init>":(Ljava/lang/String;)V
+    #5 = Methodref          #2.#240       // java/util/zip/ZipFile."<init>":(Ljava/io/File;I)V
+    #6 = Methodref          #29.#241      // ActigraphReader.getGT3XVersion:(Ljava/util/zip/ZipFile;)I
+    #7 = Fieldref           #242.#243     // java/lang/System.err:Ljava/io/PrintStream;
+    #8 = Class              #244          // java/lang/StringBuilder
+    #9 = Methodref          #8.#236       // java/lang/StringBuilder."<init>":()V
+   #10 = String             #245          // file
+   #11 = Methodref          #8.#246       // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+   #12 = String             #247          //  is not a valid V1 or V2 g3tx file
+   #13 = Methodref          #8.#248       // java/lang/StringBuilder.toString:()Ljava/lang/String;
+   #14 = Methodref          #249.#250     // java/io/PrintStream.println:(Ljava/lang/String;)V
+   #15 = Methodref          #242.#251     // java/lang/System.exit:(I)V
+   #16 = Methodref          #2.#252       // java/util/zip/ZipFile.entries:()Ljava/util/Enumeration;
+   #17 = InterfaceMethodref #253.#254     // java/util/Enumeration.hasMoreElements:()Z
+   #18 = InterfaceMethodref #253.#255     // java/util/Enumeration.nextElement:()Ljava/lang/Object;
+   #19 = Class              #256          // java/util/zip/ZipEntry
+   #20 = Methodref          #19.#248      // java/util/zip/ZipEntry.toString:()Ljava/lang/String;
+   #21 = String             #257          // info.txt
+   #22 = Methodref          #258.#259     // java/lang/String.equals:(Ljava/lang/Object;)Z
+   #23 = Class              #260          // java/io/BufferedReader
+   #24 = Class              #261          // java/io/InputStreamReader
+   #25 = Methodref          #2.#262       // java/util/zip/ZipFile.getInputStream:(Ljava/util/zip/ZipEntry;)Ljava/io/InputStream;
+   #26 = Methodref          #24.#263      // java/io/InputStreamReader."<init>":(Ljava/io/InputStream;)V
+   #27 = Methodref          #23.#264      // java/io/BufferedReader."<init>":(Ljava/io/Reader;)V
+   #28 = String             #265          // activity.bin
+   #29 = Class              #266          // ActigraphReader
+   #30 = String             #267          // log.bin
    #31 = Double             -1.0d
    #33 = Long               -1l
-   #35 = String             #261          //
-   #36 = String             #262          // 00:00:00
-   #37 = Methodref          #23.#263      // java/io/BufferedReader.ready:()Z
-   #38 = Methodref          #23.#264      // java/io/BufferedReader.readLine:()Ljava/lang/String;
-   #39 = String             #265          // :
-   #40 = Methodref          #190.#266     // java/lang/String.split:(Ljava/lang/String;)[Ljava/lang/String;
-   #41 = Methodref          #190.#267     // java/lang/String.trim:()Ljava/lang/String;
-   #42 = String             #268          // Sample Rate
-   #43 = Methodref          #141.#269     // java/lang/Integer.parseInt:(Ljava/lang/String;)I
-   #44 = String             #270          // Start Date
-   #45 = Methodref          #271.#272     // java/lang/Long.parseLong:(Ljava/lang/String;)J
-   #46 = Methodref          #29.#273      // ActigraphReader.GT3XfromTickToMillisecond:(J)J
-   #47 = String             #274          // Acceleration Scale
-   #48 = Methodref          #275.#276     // java/lang/Double.parseDouble:(Ljava/lang/String;)D
-   #49 = String             #277          // Acceleration Min
-   #50 = String             #278          // Acceleration Max
-   #51 = String             #279          // Stop Date
-   #52 = String             #280          // Serial Number
-   #53 = String             #281          // TimeZone
-   #54 = Fieldref           #237.#282     // java/lang/System.out:Ljava/io/PrintStream;
-   #55 = String             #283          // Device\'s initial offset:
-   #56 = String             #284          // Start date (local UNIX):
-   #57 = Methodref          #8.#285       // java/lang/StringBuilder.append:(J)Ljava/lang/StringBuilder;
-   #58 = String             #286          // Stop date (local UNIX):
-   #59 = Methodref          #29.#287      // ActigraphReader.setAccelerationScale:(Ljava/lang/String;)D
-   #60 = String             #288          // error parsing
-   #61 = String             #289          // , info.txt must contain \'Sample Rate\', \' Start Date\', and (usually) \'Acceleration Scale\'.
-   #62 = Methodref          #29.#290      // ActigraphReader.setSampleDelta:(D)D
-   #63 = Methodref          #29.#291      // ActigraphReader.readG3TXV1EpochPairs:(Ljava/io/InputStream;Ljava/lang/String;DDDJLEpochWriter;)V
-   #64 = Methodref          #29.#292      // ActigraphReader.readG3TXV2Epoch:(Ljava/io/InputStream;Ljava/lang/String;DDDLEpochWriter;)V
-   #65 = Methodref          #2.#293       // java/util/zip/ZipFile.close:()V
-   #66 = Methodref          #193.#293     // java/io/InputStream.close:()V
-   #67 = Methodref          #23.#293      // java/io/BufferedReader.close:()V
-   #68 = Class              #294          // java/lang/Exception
-   #69 = Class              #295          // java/io/IOException
-   #70 = Methodref          #69.#296      // java/io/IOException.printStackTrace:(Ljava/io/PrintStream;)V
-   #71 = String             #297          // error reading/writing file
-   #72 = Methodref          #69.#243      // java/io/IOException.toString:()Ljava/lang/String;
-   #73 = Methodref          #193.#298     // java/io/InputStream.read:()I
-   #74 = Fieldref           #29.#299      // ActigraphReader.logger:Ljava/util/logging/Logger;
-   #75 = Fieldref           #300.#301     // java/util/logging/Level.FINER:Ljava/util/logging/Level;
-   #76 = String             #302          // \nHeader info\ntype:
-   #77 = Methodref          #8.#303       // java/lang/StringBuilder.append:(I)Ljava/lang/StringBuilder;
-   #78 = String             #304          // \nDate 0x%08X:
-   #79 = Class              #305          // java/lang/Object
-   #80 = Methodref          #271.#306     // java/lang/Long.valueOf:(J)Ljava/lang/Long;
-   #81 = Methodref          #190.#307     // java/lang/String.format:(Ljava/lang/String;[Ljava/lang/Object;)Ljava/lang/String;
-   #82 = String             #308          // \nsize:
-   #83 = String             #309          // \nStarting index:
-   #84 = Methodref          #310.#311     // java/util/logging/Logger.log:(Ljava/util/logging/Level;Ljava/lang/String;)V
-   #85 = Methodref          #29.#312      // ActigraphReader.isPayload:(III)Z
-   #86 = Fieldref           #300.#313     // java/util/logging/Level.INFO:Ljava/util/logging/Level;
-   #87 = String             #314          // Processing parameter packet...
-   #88 = Methodref          #29.#315      // ActigraphReader.isAccelScale:([B)Z
-   #89 = Methodref          #29.#316      // ActigraphReader.decodePara:(I)D
-   #90 = String             #317          // accelerationScale changed to
-   #91 = Methodref          #8.#318       // java/lang/StringBuilder.append:(D)Ljava/lang/StringBuilder;
-   #92 = Methodref          #29.#319      // ActigraphReader.processActivity:(Ljava/lang/String;DJBIIIIDLjava/io/InputStream;LEpochWriter;)[I
-   #93 = Methodref          #29.#320      // ActigraphReader.processActivity2:(Ljava/lang/String;DJBIIIIDLjava/io/InputStream;LEpochWriter;)[I
-   #94 = Methodref          #29.#321      // ActigraphReader.checkChecksum:(IIIIJII)V
-   #95 = String             #322          // Done processing
-   #96 = String             #323          //  packets.
-   #97 = String             #324          // End of .g3tx file reached
-   #98 = Methodref          #29.#325      // ActigraphReader.readAccelPair:([BD)[D
+   #35 = String             #268          //
+   #36 = String             #269          // 00:00:00
+   #37 = Methodref          #23.#270      // java/io/BufferedReader.ready:()Z
+   #38 = Methodref          #23.#271      // java/io/BufferedReader.readLine:()Ljava/lang/String;
+   #39 = String             #272          // :
+   #40 = Methodref          #258.#273     // java/lang/String.split:(Ljava/lang/String;)[Ljava/lang/String;
+   #41 = Methodref          #258.#274     // java/lang/String.trim:()Ljava/lang/String;
+   #42 = String             #275          // Sample Rate
+   #43 = Methodref          #141.#276     // java/lang/Integer.parseInt:(Ljava/lang/String;)I
+   #44 = String             #277          // Start Date
+   #45 = Methodref          #278.#279     // java/lang/Long.parseLong:(Ljava/lang/String;)J
+   #46 = Methodref          #29.#280      // ActigraphReader.GT3XfromTickToMillisecond:(J)J
+   #47 = String             #281          // Acceleration Scale
+   #48 = Methodref          #282.#283     // java/lang/Double.parseDouble:(Ljava/lang/String;)D
+   #49 = String             #284          // Acceleration Min
+   #50 = String             #285          // Acceleration Max
+   #51 = String             #286          // Stop Date
+   #52 = String             #287          // Serial Number
+   #53 = String             #288          // TimeZone
+   #54 = Fieldref           #242.#289     // java/lang/System.out:Ljava/io/PrintStream;
+   #55 = String             #290          // Device\'s initial offset:
+   #56 = String             #291          // Start date (local UNIX):
+   #57 = Methodref          #8.#292       // java/lang/StringBuilder.append:(J)Ljava/lang/StringBuilder;
+   #58 = String             #293          // Stop date (local UNIX):
+   #59 = Methodref          #29.#294      // ActigraphReader.setAccelerationScale:(Ljava/lang/String;)D
+   #60 = String             #295          // error parsing
+   #61 = String             #296          // , info.txt must contain \'Sample Rate\', \' Start Date\', and (usually) \'Acceleration Scale\'.
+   #62 = Methodref          #29.#297      // ActigraphReader.setSampleDelta:(D)D
+   #63 = Methodref          #29.#298      // ActigraphReader.readG3TXV1EpochPairs:(Ljava/io/InputStream;Ljava/lang/String;DDDJLEpochWriter;)V
+   #64 = Methodref          #29.#299      // ActigraphReader.readG3TXV2Epoch:(Ljava/io/InputStream;Ljava/lang/String;DDDLEpochWriter;)V
+   #65 = Methodref          #2.#300       // java/util/zip/ZipFile.close:()V
+   #66 = Methodref          #301.#300     // java/io/InputStream.close:()V
+   #67 = Methodref          #23.#300      // java/io/BufferedReader.close:()V
+   #68 = Class              #302          // java/lang/Exception
+   #69 = Class              #303          // java/io/IOException
+   #70 = Methodref          #69.#304      // java/io/IOException.printStackTrace:(Ljava/io/PrintStream;)V
+   #71 = String             #305          // error reading/writing file
+   #72 = Methodref          #69.#248      // java/io/IOException.toString:()Ljava/lang/String;
+   #73 = Methodref          #301.#306     // java/io/InputStream.read:()I
+   #74 = Fieldref           #29.#307      // ActigraphReader.logger:Ljava/util/logging/Logger;
+   #75 = Fieldref           #308.#309     // java/util/logging/Level.FINER:Ljava/util/logging/Level;
+   #76 = String             #310          // \nHeader info\ntype:
+   #77 = Methodref          #8.#311       // java/lang/StringBuilder.append:(I)Ljava/lang/StringBuilder;
+   #78 = String             #312          // \nDate 0x%08X:
+   #79 = Class              #313          // java/lang/Object
+   #80 = Methodref          #278.#314     // java/lang/Long.valueOf:(J)Ljava/lang/Long;
+   #81 = Methodref          #258.#315     // java/lang/String.format:(Ljava/lang/String;[Ljava/lang/Object;)Ljava/lang/String;
+   #82 = String             #316          // \nsize:
+   #83 = String             #317          // \nStarting index:
+   #84 = Methodref          #318.#319     // java/util/logging/Logger.log:(Ljava/util/logging/Level;Ljava/lang/String;)V
+   #85 = Methodref          #29.#320      // ActigraphReader.isPayload:(III)Z
+   #86 = Fieldref           #308.#321     // java/util/logging/Level.INFO:Ljava/util/logging/Level;
+   #87 = String             #322          // Processing parameter packet...
+   #88 = Methodref          #29.#323      // ActigraphReader.isAccelScale:([B)Z
+   #89 = Methodref          #29.#324      // ActigraphReader.decodePara:(I)D
+   #90 = String             #325          // accelerationScale changed to
+   #91 = Methodref          #8.#326       // java/lang/StringBuilder.append:(D)Ljava/lang/StringBuilder;
+   #92 = Methodref          #29.#327      // ActigraphReader.processActivity:(Ljava/lang/String;DJBIIIIDLjava/io/InputStream;LEpochWriter;)[I
+   #93 = Methodref          #29.#328      // ActigraphReader.processActivity2:(Ljava/lang/String;DJBIIIIDLjava/io/InputStream;LEpochWriter;)[I
+   #94 = Methodref          #29.#329      // ActigraphReader.checkChecksum:(IIIIJII)V
+   #95 = String             #330          // Done processing
+   #96 = String             #331          //  packets.
+   #97 = String             #332          // End of .g3tx file reached
+   #98 = Methodref          #29.#333      // ActigraphReader.readAccelPair:([BD)[D
    #99 = Double             1000.0d
-  #101 = Methodref          #326.#327     // java/lang/Math.round:(D)J
-  #102 = Methodref          #29.#328      // ActigraphReader.getTrueUnixTime:(JLjava/lang/String;)J
-  #103 = Methodref          #191.#329     // EpochWriter.newValues:(JDDDD[I)Z
+  #101 = Methodref          #334.#335     // java/lang/Math.round:(D)J
+  #102 = Methodref          #29.#336      // ActigraphReader.getTrueUnixTime:(JLjava/lang/String;)J
+  #103 = Methodref          #337.#338     // EpochWriter.newValues:(JDDDD[I)Z
   #104 = Integer            61440
-  #105 = String             #330          // i:
-  #106 = String             #331          // x y z:
-  #107 = String             #332          //
+  #105 = String             #339          // i:
+  #106 = String             #340          // x y z:
+  #107 = String             #341          //
   #108 = Long               1000l
-  #110 = String             #333          // error when reading activity at byte
-  #111 = Methodref          #190.#334     // java/lang/String.charAt:(I)C
-  #112 = Methodref          #190.#335     // java/lang/String.substring:(I)Ljava/lang/String;
-  #113 = Methodref          #336.#337     // java/time/LocalTime.parse:(Ljava/lang/CharSequence;)Ljava/time/LocalTime;
-  #114 = Methodref          #336.#338     // java/time/LocalTime.getHour:()I
-  #115 = Methodref          #336.#339     // java/time/LocalTime.getMinute:()I
-  #116 = String             #340          // \nx y z:
-  #117 = String             #341          // \nTime:
+  #110 = String             #342          // error when reading activity at byte
+  #111 = Methodref          #258.#343     // java/lang/String.charAt:(I)C
+  #112 = Methodref          #258.#344     // java/lang/String.substring:(I)Ljava/lang/String;
+  #113 = Methodref          #345.#346     // java/time/LocalTime.parse:(Ljava/lang/CharSequence;)Ljava/time/LocalTime;
+  #114 = Methodref          #345.#347     // java/time/LocalTime.getHour:()I
+  #115 = Methodref          #345.#348     // java/time/LocalTime.getMinute:()I
+  #116 = String             #349          // \nx y z:
+  #117 = String             #350          // \nTime:
   #118 = Long               255l
-  #120 = Fieldref           #300.#342     // java/util/logging/Level.SEVERE:Ljava/util/logging/Level;
-  #121 = String             #343          // Packet parsing failed at byte
-  #122 = String             #344          // \nChecksum does not match!
-  #123 = String             #345          // \nExpected 0x%08X
-  #124 = Methodref          #141.#346     // java/lang/Integer.valueOf:(I)Ljava/lang/Integer;
-  #125 = String             #347          // \nObtained 0x%08X
-  #126 = String             #348          // Verification succeeds
+  #120 = Fieldref           #308.#351     // java/util/logging/Level.SEVERE:Ljava/util/logging/Level;
+  #121 = String             #352          // Packet parsing failed at byte
+  #122 = String             #353          // \nChecksum does not match!
+  #123 = String             #354          // \nExpected 0x%08X
+  #124 = Methodref          #141.#355     // java/lang/Integer.valueOf:(I)Ljava/lang/Integer;
+  #125 = String             #356          // \nObtained 0x%08X
+  #126 = String             #357          // Verification succeeds
   #127 = Double             341.0d
   #129 = Double             256.0d
-  #131 = String             #349          // NEO
-  #132 = Methodref          #190.#350     // java/lang/String.startsWith:(Ljava/lang/String;)Z
-  #133 = String             #351          // CLE
-  #134 = String             #352          // MOS
-  #135 = String             #353          // sampleFreq:
+  #131 = String             #358          // NEO
+  #132 = Methodref          #258.#359     // java/lang/String.startsWith:(Ljava/lang/String;)Z
+  #133 = String             #360          // CLE
+  #134 = String             #361          // MOS
+  #135 = String             #362          // sampleFreq:
   #136 = Double             100.0d
-  #138 = String             #354          // sampleDelta before rounding:
-  #139 = String             #355          // sampleDelta after rounding:
+  #138 = String             #363          // sampleDelta before rounding:
+  #139 = String             #364          // sampleDelta after rounding:
   #140 = Integer            8388607
-  #141 = Class              #356          // java/lang/Integer
+  #141 = Class              #365          // java/lang/Integer
   #142 = Double             2.147483647E9d
   #144 = Double             -2.147483647E9d
   #146 = Integer            -16777216
   #147 = Integer            16777215
   #148 = Integer            8388608
   #149 = Double             8388608.0d
   #151 = Double             2.0d
-  #153 = Methodref          #326.#357     // java/lang/Math.pow:(DD)D
-  #154 = Class              #358          // java/util/Date
+  #153 = Methodref          #334.#366     // java/lang/Math.pow:(DD)D
+  #154 = Class              #367          // java/util/Date
   #155 = Long               621355968000000000l
   #157 = Long               10000l
-  #159 = Methodref          #154.#359     // java/util/Date."<init>":(J)V
-  #160 = Methodref          #154.#360     // java/util/Date.getTime:()J
-  #161 = String             #361          // lux.bin
-  #162 = Methodref          #362.#363     // java/lang/Class.getClassLoader:()Ljava/lang/ClassLoader;
-  #163 = String             #364          // logging.properties
-  #164 = Methodref          #365.#366     // java/lang/ClassLoader.getResource:(Ljava/lang/String;)Ljava/net/URL;
-  #165 = Methodref          #367.#368     // java/net/URL.getFile:()Ljava/lang/String;
-  #166 = String             #369          // java.util.logging.config.file
-  #167 = Methodref          #237.#370     // java/lang/System.setProperty:(Ljava/lang/String;Ljava/lang/String;)Ljava/lang/String;
-  #168 = Methodref          #362.#371     // java/lang/Class.getName:()Ljava/lang/String;
-  #169 = Methodref          #310.#372     // java/util/logging/Logger.getLogger:(Ljava/lang/String;)Ljava/util/logging/Logger;
-  #170 = Class              #373          // DeviceReader
+  #159 = Methodref          #154.#368     // java/util/Date."<init>":(J)V
+  #160 = Methodref          #154.#369     // java/util/Date.getTime:()J
+  #161 = String             #370          // lux.bin
+  #162 = Methodref          #371.#372     // java/lang/Class.getClassLoader:()Ljava/lang/ClassLoader;
+  #163 = String             #373          // logging.properties
+  #164 = Methodref          #374.#375     // java/lang/ClassLoader.getResource:(Ljava/lang/String;)Ljava/net/URL;
+  #165 = Methodref          #376.#377     // java/net/URL.getFile:()Ljava/lang/String;
+  #166 = String             #378          // java.util.logging.config.file
+  #167 = Methodref          #242.#379     // java/lang/System.setProperty:(Ljava/lang/String;Ljava/lang/String;)Ljava/lang/String;
+  #168 = Methodref          #371.#380     // java/lang/Class.getName:()Ljava/lang/String;
+  #169 = Methodref          #318.#381     // java/util/logging/Logger.getLogger:(Ljava/lang/String;)Ljava/util/logging/Logger;
+  #170 = Class              #382          // DeviceReader
   #171 = Utf8               INVALID_GT3_FILE
   #172 = Utf8               I
   #173 = Utf8               ConstantValue
   #174 = Integer            0
   #175 = Utf8               VALID_GT3_V1_FILE
   #176 = Integer            1
   #177 = Utf8               VALID_GT3_V2_FILE
@@ -179,301 +179,310 @@
   #183 = Utf8               <init>
   #184 = Utf8               ()V
   #185 = Utf8               Code
   #186 = Utf8               LineNumberTable
   #187 = Utf8               readG3TXEpochs
   #188 = Utf8               (Ljava/lang/String;LEpochWriter;Ljava/lang/Boolean;)V
   #189 = Utf8               StackMapTable
-  #190 = Class              #374          // java/lang/String
-  #191 = Class              #375          // EpochWriter
-  #192 = Class              #376          // java/lang/Boolean
-  #193 = Class              #377          // java/io/InputStream
-  #194 = Class              #378          // java/util/Enumeration
-  #195 = Class              #379          // "[Ljava/lang/String;"
-  #196 = Class              #380          // java/lang/Throwable
-  #197 = Utf8               readG3TXV2Epoch
-  #198 = Utf8               (Ljava/io/InputStream;Ljava/lang/String;DDDLEpochWriter;)V
-  #199 = Class              #381          // "[I"
-  #200 = Class              #382          // "[B"
-  #201 = Utf8               readG3TXV1EpochPairs
-  #202 = Utf8               (Ljava/io/InputStream;Ljava/lang/String;DDDJLEpochWriter;)V
-  #203 = Class              #383          // "[D"
-  #204 = Utf8               processActivity
-  #205 = Utf8               (Ljava/lang/String;DJBIIIIDLjava/io/InputStream;LEpochWriter;)[I
-  #206 = Utf8               getTrueUnixTime
-  #207 = Utf8               (JLjava/lang/String;)J
-  #208 = Utf8               processActivity2
-  #209 = Utf8               readAccelPair
-  #210 = Utf8               ([BD)[D
-  #211 = Utf8               checkChecksum
-  #212 = Utf8               (IIIIJII)V
-  #213 = Utf8               setAccelerationScale
-  #214 = Utf8               (Ljava/lang/String;)D
-  #215 = Utf8               setSampleDelta
-  #216 = Utf8               (D)D
-  #217 = Utf8               isPayload
-  #218 = Utf8               (III)Z
-  #219 = Utf8               decodePara
-  #220 = Utf8               (I)D
-  #221 = Utf8               isAccelScale
-  #222 = Utf8               ([B)Z
-  #223 = Utf8               GT3XfromTickToMillisecond
-  #224 = Utf8               (J)J
-  #225 = Utf8               getGT3XVersion
-  #226 = Utf8               (Ljava/util/zip/ZipFile;)I
-  #227 = Utf8               Exceptions
-  #228 = Utf8               <clinit>
-  #229 = Utf8               SourceFile
-  #230 = Utf8               ActigraphReader.java
-  #231 = NameAndType        #183:#184     // "<init>":()V
-  #232 = Utf8               java/util/zip/ZipFile
-  #233 = Utf8               java/io/File
-  #234 = NameAndType        #183:#384     // "<init>":(Ljava/lang/String;)V
-  #235 = NameAndType        #183:#385     // "<init>":(Ljava/io/File;I)V
-  #236 = NameAndType        #225:#226     // getGT3XVersion:(Ljava/util/zip/ZipFile;)I
-  #237 = Class              #386          // java/lang/System
-  #238 = NameAndType        #387:#388     // err:Ljava/io/PrintStream;
-  #239 = Utf8               java/lang/StringBuilder
-  #240 = Utf8               file
-  #241 = NameAndType        #389:#390     // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #242 = Utf8                is not a valid V1 or V2 g3tx file
-  #243 = NameAndType        #391:#392     // toString:()Ljava/lang/String;
-  #244 = Class              #393          // java/io/PrintStream
-  #245 = NameAndType        #394:#384     // println:(Ljava/lang/String;)V
-  #246 = NameAndType        #395:#396     // exit:(I)V
-  #247 = NameAndType        #397:#398     // entries:()Ljava/util/Enumeration;
-  #248 = NameAndType        #399:#400     // hasMoreElements:()Z
-  #249 = NameAndType        #401:#402     // nextElement:()Ljava/lang/Object;
-  #250 = Utf8               java/util/zip/ZipEntry
-  #251 = Utf8               info.txt
-  #252 = NameAndType        #403:#404     // equals:(Ljava/lang/Object;)Z
-  #253 = Utf8               java/io/BufferedReader
-  #254 = Utf8               java/io/InputStreamReader
-  #255 = NameAndType        #405:#406     // getInputStream:(Ljava/util/zip/ZipEntry;)Ljava/io/InputStream;
-  #256 = NameAndType        #183:#407     // "<init>":(Ljava/io/InputStream;)V
-  #257 = NameAndType        #183:#408     // "<init>":(Ljava/io/Reader;)V
-  #258 = Utf8               activity.bin
-  #259 = Utf8               ActigraphReader
-  #260 = Utf8               log.bin
-  #261 = Utf8
-  #262 = Utf8               00:00:00
-  #263 = NameAndType        #409:#400     // ready:()Z
-  #264 = NameAndType        #410:#392     // readLine:()Ljava/lang/String;
-  #265 = Utf8               :
-  #266 = NameAndType        #411:#412     // split:(Ljava/lang/String;)[Ljava/lang/String;
-  #267 = NameAndType        #413:#392     // trim:()Ljava/lang/String;
-  #268 = Utf8               Sample Rate
-  #269 = NameAndType        #414:#415     // parseInt:(Ljava/lang/String;)I
-  #270 = Utf8               Start Date
-  #271 = Class              #416          // java/lang/Long
-  #272 = NameAndType        #417:#418     // parseLong:(Ljava/lang/String;)J
-  #273 = NameAndType        #223:#224     // GT3XfromTickToMillisecond:(J)J
-  #274 = Utf8               Acceleration Scale
-  #275 = Class              #419          // java/lang/Double
-  #276 = NameAndType        #420:#214     // parseDouble:(Ljava/lang/String;)D
-  #277 = Utf8               Acceleration Min
-  #278 = Utf8               Acceleration Max
-  #279 = Utf8               Stop Date
-  #280 = Utf8               Serial Number
-  #281 = Utf8               TimeZone
-  #282 = NameAndType        #421:#388     // out:Ljava/io/PrintStream;
-  #283 = Utf8               Device\'s initial offset:
-  #284 = Utf8               Start date (local UNIX):
-  #285 = NameAndType        #389:#422     // append:(J)Ljava/lang/StringBuilder;
-  #286 = Utf8               Stop date (local UNIX):
-  #287 = NameAndType        #213:#214     // setAccelerationScale:(Ljava/lang/String;)D
-  #288 = Utf8               error parsing
-  #289 = Utf8               , info.txt must contain \'Sample Rate\', \' Start Date\', and (usually) \'Acceleration Scale\'.
-  #290 = NameAndType        #215:#216     // setSampleDelta:(D)D
-  #291 = NameAndType        #201:#202     // readG3TXV1EpochPairs:(Ljava/io/InputStream;Ljava/lang/String;DDDJLEpochWriter;)V
-  #292 = NameAndType        #197:#198     // readG3TXV2Epoch:(Ljava/io/InputStream;Ljava/lang/String;DDDLEpochWriter;)V
-  #293 = NameAndType        #423:#184     // close:()V
-  #294 = Utf8               java/lang/Exception
-  #295 = Utf8               java/io/IOException
-  #296 = NameAndType        #424:#425     // printStackTrace:(Ljava/io/PrintStream;)V
-  #297 = Utf8               error reading/writing file
-  #298 = NameAndType        #426:#427     // read:()I
-  #299 = NameAndType        #181:#182     // logger:Ljava/util/logging/Logger;
-  #300 = Class              #428          // java/util/logging/Level
-  #301 = NameAndType        #429:#430     // FINER:Ljava/util/logging/Level;
-  #302 = Utf8               \nHeader info\ntype:
-  #303 = NameAndType        #389:#431     // append:(I)Ljava/lang/StringBuilder;
-  #304 = Utf8               \nDate 0x%08X:
-  #305 = Utf8               java/lang/Object
-  #306 = NameAndType        #432:#433     // valueOf:(J)Ljava/lang/Long;
-  #307 = NameAndType        #434:#435     // format:(Ljava/lang/String;[Ljava/lang/Object;)Ljava/lang/String;
-  #308 = Utf8               \nsize:
-  #309 = Utf8               \nStarting index:
-  #310 = Class              #436          // java/util/logging/Logger
-  #311 = NameAndType        #437:#438     // log:(Ljava/util/logging/Level;Ljava/lang/String;)V
-  #312 = NameAndType        #217:#218     // isPayload:(III)Z
-  #313 = NameAndType        #439:#430     // INFO:Ljava/util/logging/Level;
-  #314 = Utf8               Processing parameter packet...
-  #315 = NameAndType        #221:#222     // isAccelScale:([B)Z
-  #316 = NameAndType        #219:#220     // decodePara:(I)D
-  #317 = Utf8               accelerationScale changed to
-  #318 = NameAndType        #389:#440     // append:(D)Ljava/lang/StringBuilder;
-  #319 = NameAndType        #204:#205     // processActivity:(Ljava/lang/String;DJBIIIIDLjava/io/InputStream;LEpochWriter;)[I
-  #320 = NameAndType        #208:#205     // processActivity2:(Ljava/lang/String;DJBIIIIDLjava/io/InputStream;LEpochWriter;)[I
-  #321 = NameAndType        #211:#212     // checkChecksum:(IIIIJII)V
-  #322 = Utf8               Done processing
-  #323 = Utf8                packets.
-  #324 = Utf8               End of .g3tx file reached
-  #325 = NameAndType        #209:#210     // readAccelPair:([BD)[D
-  #326 = Class              #441          // java/lang/Math
-  #327 = NameAndType        #442:#443     // round:(D)J
-  #328 = NameAndType        #206:#207     // getTrueUnixTime:(JLjava/lang/String;)J
-  #329 = NameAndType        #444:#445     // newValues:(JDDDD[I)Z
-  #330 = Utf8               i:
-  #331 = Utf8               x y z:
-  #332 = Utf8
-  #333 = Utf8               error when reading activity at byte
-  #334 = NameAndType        #446:#447     // charAt:(I)C
-  #335 = NameAndType        #448:#449     // substring:(I)Ljava/lang/String;
-  #336 = Class              #450          // java/time/LocalTime
-  #337 = NameAndType        #451:#452     // parse:(Ljava/lang/CharSequence;)Ljava/time/LocalTime;
-  #338 = NameAndType        #453:#427     // getHour:()I
-  #339 = NameAndType        #454:#427     // getMinute:()I
-  #340 = Utf8               \nx y z:
-  #341 = Utf8               \nTime:
-  #342 = NameAndType        #455:#430     // SEVERE:Ljava/util/logging/Level;
-  #343 = Utf8               Packet parsing failed at byte
-  #344 = Utf8               \nChecksum does not match!
-  #345 = Utf8               \nExpected 0x%08X
-  #346 = NameAndType        #432:#456     // valueOf:(I)Ljava/lang/Integer;
-  #347 = Utf8               \nObtained 0x%08X
-  #348 = Utf8               Verification succeeds
-  #349 = Utf8               NEO
-  #350 = NameAndType        #457:#458     // startsWith:(Ljava/lang/String;)Z
-  #351 = Utf8               CLE
-  #352 = Utf8               MOS
-  #353 = Utf8               sampleFreq:
-  #354 = Utf8               sampleDelta before rounding:
-  #355 = Utf8               sampleDelta after rounding:
-  #356 = Utf8               java/lang/Integer
-  #357 = NameAndType        #459:#460     // pow:(DD)D
-  #358 = Utf8               java/util/Date
-  #359 = NameAndType        #183:#461     // "<init>":(J)V
-  #360 = NameAndType        #462:#463     // getTime:()J
-  #361 = Utf8               lux.bin
-  #362 = Class              #464          // java/lang/Class
-  #363 = NameAndType        #465:#466     // getClassLoader:()Ljava/lang/ClassLoader;
-  #364 = Utf8               logging.properties
-  #365 = Class              #467          // java/lang/ClassLoader
-  #366 = NameAndType        #468:#469     // getResource:(Ljava/lang/String;)Ljava/net/URL;
-  #367 = Class              #470          // java/net/URL
-  #368 = NameAndType        #471:#392     // getFile:()Ljava/lang/String;
-  #369 = Utf8               java.util.logging.config.file
-  #370 = NameAndType        #472:#473     // setProperty:(Ljava/lang/String;Ljava/lang/String;)Ljava/lang/String;
-  #371 = NameAndType        #474:#392     // getName:()Ljava/lang/String;
-  #372 = NameAndType        #475:#476     // getLogger:(Ljava/lang/String;)Ljava/util/logging/Logger;
-  #373 = Utf8               DeviceReader
-  #374 = Utf8               java/lang/String
-  #375 = Utf8               EpochWriter
-  #376 = Utf8               java/lang/Boolean
-  #377 = Utf8               java/io/InputStream
-  #378 = Utf8               java/util/Enumeration
-  #379 = Utf8               [Ljava/lang/String;
-  #380 = Utf8               java/lang/Throwable
-  #381 = Utf8               [I
-  #382 = Utf8               [B
-  #383 = Utf8               [D
-  #384 = Utf8               (Ljava/lang/String;)V
-  #385 = Utf8               (Ljava/io/File;I)V
-  #386 = Utf8               java/lang/System
-  #387 = Utf8               err
-  #388 = Utf8               Ljava/io/PrintStream;
-  #389 = Utf8               append
-  #390 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #391 = Utf8               toString
-  #392 = Utf8               ()Ljava/lang/String;
-  #393 = Utf8               java/io/PrintStream
-  #394 = Utf8               println
-  #395 = Utf8               exit
-  #396 = Utf8               (I)V
-  #397 = Utf8               entries
-  #398 = Utf8               ()Ljava/util/Enumeration;
-  #399 = Utf8               hasMoreElements
-  #400 = Utf8               ()Z
-  #401 = Utf8               nextElement
-  #402 = Utf8               ()Ljava/lang/Object;
-  #403 = Utf8               equals
-  #404 = Utf8               (Ljava/lang/Object;)Z
-  #405 = Utf8               getInputStream
-  #406 = Utf8               (Ljava/util/zip/ZipEntry;)Ljava/io/InputStream;
-  #407 = Utf8               (Ljava/io/InputStream;)V
-  #408 = Utf8               (Ljava/io/Reader;)V
-  #409 = Utf8               ready
-  #410 = Utf8               readLine
-  #411 = Utf8               split
-  #412 = Utf8               (Ljava/lang/String;)[Ljava/lang/String;
-  #413 = Utf8               trim
-  #414 = Utf8               parseInt
-  #415 = Utf8               (Ljava/lang/String;)I
-  #416 = Utf8               java/lang/Long
-  #417 = Utf8               parseLong
-  #418 = Utf8               (Ljava/lang/String;)J
-  #419 = Utf8               java/lang/Double
-  #420 = Utf8               parseDouble
-  #421 = Utf8               out
-  #422 = Utf8               (J)Ljava/lang/StringBuilder;
-  #423 = Utf8               close
-  #424 = Utf8               printStackTrace
-  #425 = Utf8               (Ljava/io/PrintStream;)V
-  #426 = Utf8               read
-  #427 = Utf8               ()I
-  #428 = Utf8               java/util/logging/Level
-  #429 = Utf8               FINER
-  #430 = Utf8               Ljava/util/logging/Level;
-  #431 = Utf8               (I)Ljava/lang/StringBuilder;
-  #432 = Utf8               valueOf
-  #433 = Utf8               (J)Ljava/lang/Long;
-  #434 = Utf8               format
-  #435 = Utf8               (Ljava/lang/String;[Ljava/lang/Object;)Ljava/lang/String;
-  #436 = Utf8               java/util/logging/Logger
-  #437 = Utf8               log
-  #438 = Utf8               (Ljava/util/logging/Level;Ljava/lang/String;)V
-  #439 = Utf8               INFO
-  #440 = Utf8               (D)Ljava/lang/StringBuilder;
-  #441 = Utf8               java/lang/Math
-  #442 = Utf8               round
-  #443 = Utf8               (D)J
-  #444 = Utf8               newValues
-  #445 = Utf8               (JDDDD[I)Z
-  #446 = Utf8               charAt
-  #447 = Utf8               (I)C
-  #448 = Utf8               substring
-  #449 = Utf8               (I)Ljava/lang/String;
-  #450 = Utf8               java/time/LocalTime
-  #451 = Utf8               parse
-  #452 = Utf8               (Ljava/lang/CharSequence;)Ljava/time/LocalTime;
-  #453 = Utf8               getHour
-  #454 = Utf8               getMinute
-  #455 = Utf8               SEVERE
-  #456 = Utf8               (I)Ljava/lang/Integer;
-  #457 = Utf8               startsWith
-  #458 = Utf8               (Ljava/lang/String;)Z
-  #459 = Utf8               pow
-  #460 = Utf8               (DD)D
-  #461 = Utf8               (J)V
-  #462 = Utf8               getTime
-  #463 = Utf8               ()J
-  #464 = Utf8               java/lang/Class
-  #465 = Utf8               getClassLoader
-  #466 = Utf8               ()Ljava/lang/ClassLoader;
-  #467 = Utf8               java/lang/ClassLoader
-  #468 = Utf8               getResource
-  #469 = Utf8               (Ljava/lang/String;)Ljava/net/URL;
-  #470 = Utf8               java/net/URL
-  #471 = Utf8               getFile
-  #472 = Utf8               setProperty
-  #473 = Utf8               (Ljava/lang/String;Ljava/lang/String;)Ljava/lang/String;
-  #474 = Utf8               getName
-  #475 = Utf8               getLogger
-  #476 = Utf8               (Ljava/lang/String;)Ljava/util/logging/Logger;
+  #190 = Class              #383          // java/lang/String
+  #191 = Class              #384          // EpochWriter
+  #192 = Class              #385          // java/lang/Boolean
+  #193 = Class              #237          // java/util/zip/ZipFile
+  #194 = Class              #260          // java/io/BufferedReader
+  #195 = Class              #386          // java/io/InputStream
+  #196 = Class              #387          // java/util/Enumeration
+  #197 = Class              #256          // java/util/zip/ZipEntry
+  #198 = Class              #388          // "[Ljava/lang/String;"
+  #199 = Class              #302          // java/lang/Exception
+  #200 = Class              #303          // java/io/IOException
+  #201 = Class              #389          // java/lang/Throwable
+  #202 = Utf8               readG3TXV2Epoch
+  #203 = Utf8               (Ljava/io/InputStream;Ljava/lang/String;DDDLEpochWriter;)V
+  #204 = Class              #390          // "[I"
+  #205 = Class              #391          // "[B"
+  #206 = Utf8               readG3TXV1EpochPairs
+  #207 = Utf8               (Ljava/io/InputStream;Ljava/lang/String;DDDJLEpochWriter;)V
+  #208 = Class              #392          // "[D"
+  #209 = Utf8               processActivity
+  #210 = Utf8               (Ljava/lang/String;DJBIIIIDLjava/io/InputStream;LEpochWriter;)[I
+  #211 = Utf8               getTrueUnixTime
+  #212 = Utf8               (JLjava/lang/String;)J
+  #213 = Utf8               processActivity2
+  #214 = Utf8               readAccelPair
+  #215 = Utf8               ([BD)[D
+  #216 = Utf8               checkChecksum
+  #217 = Utf8               (IIIIJII)V
+  #218 = Utf8               setAccelerationScale
+  #219 = Utf8               (Ljava/lang/String;)D
+  #220 = Utf8               setSampleDelta
+  #221 = Utf8               (D)D
+  #222 = Utf8               isPayload
+  #223 = Utf8               (III)Z
+  #224 = Utf8               decodePara
+  #225 = Utf8               (I)D
+  #226 = Utf8               isAccelScale
+  #227 = Utf8               ([B)Z
+  #228 = Utf8               GT3XfromTickToMillisecond
+  #229 = Utf8               (J)J
+  #230 = Utf8               getGT3XVersion
+  #231 = Utf8               (Ljava/util/zip/ZipFile;)I
+  #232 = Utf8               Exceptions
+  #233 = Utf8               <clinit>
+  #234 = Utf8               SourceFile
+  #235 = Utf8               ActigraphReader.java
+  #236 = NameAndType        #183:#184     // "<init>":()V
+  #237 = Utf8               java/util/zip/ZipFile
+  #238 = Utf8               java/io/File
+  #239 = NameAndType        #183:#393     // "<init>":(Ljava/lang/String;)V
+  #240 = NameAndType        #183:#394     // "<init>":(Ljava/io/File;I)V
+  #241 = NameAndType        #230:#231     // getGT3XVersion:(Ljava/util/zip/ZipFile;)I
+  #242 = Class              #395          // java/lang/System
+  #243 = NameAndType        #396:#397     // err:Ljava/io/PrintStream;
+  #244 = Utf8               java/lang/StringBuilder
+  #245 = Utf8               file
+  #246 = NameAndType        #398:#399     // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #247 = Utf8                is not a valid V1 or V2 g3tx file
+  #248 = NameAndType        #400:#401     // toString:()Ljava/lang/String;
+  #249 = Class              #402          // java/io/PrintStream
+  #250 = NameAndType        #403:#393     // println:(Ljava/lang/String;)V
+  #251 = NameAndType        #404:#405     // exit:(I)V
+  #252 = NameAndType        #406:#407     // entries:()Ljava/util/Enumeration;
+  #253 = Class              #387          // java/util/Enumeration
+  #254 = NameAndType        #408:#409     // hasMoreElements:()Z
+  #255 = NameAndType        #410:#411     // nextElement:()Ljava/lang/Object;
+  #256 = Utf8               java/util/zip/ZipEntry
+  #257 = Utf8               info.txt
+  #258 = Class              #383          // java/lang/String
+  #259 = NameAndType        #412:#413     // equals:(Ljava/lang/Object;)Z
+  #260 = Utf8               java/io/BufferedReader
+  #261 = Utf8               java/io/InputStreamReader
+  #262 = NameAndType        #414:#415     // getInputStream:(Ljava/util/zip/ZipEntry;)Ljava/io/InputStream;
+  #263 = NameAndType        #183:#416     // "<init>":(Ljava/io/InputStream;)V
+  #264 = NameAndType        #183:#417     // "<init>":(Ljava/io/Reader;)V
+  #265 = Utf8               activity.bin
+  #266 = Utf8               ActigraphReader
+  #267 = Utf8               log.bin
+  #268 = Utf8
+  #269 = Utf8               00:00:00
+  #270 = NameAndType        #418:#409     // ready:()Z
+  #271 = NameAndType        #419:#401     // readLine:()Ljava/lang/String;
+  #272 = Utf8               :
+  #273 = NameAndType        #420:#421     // split:(Ljava/lang/String;)[Ljava/lang/String;
+  #274 = NameAndType        #422:#401     // trim:()Ljava/lang/String;
+  #275 = Utf8               Sample Rate
+  #276 = NameAndType        #423:#424     // parseInt:(Ljava/lang/String;)I
+  #277 = Utf8               Start Date
+  #278 = Class              #425          // java/lang/Long
+  #279 = NameAndType        #426:#427     // parseLong:(Ljava/lang/String;)J
+  #280 = NameAndType        #228:#229     // GT3XfromTickToMillisecond:(J)J
+  #281 = Utf8               Acceleration Scale
+  #282 = Class              #428          // java/lang/Double
+  #283 = NameAndType        #429:#219     // parseDouble:(Ljava/lang/String;)D
+  #284 = Utf8               Acceleration Min
+  #285 = Utf8               Acceleration Max
+  #286 = Utf8               Stop Date
+  #287 = Utf8               Serial Number
+  #288 = Utf8               TimeZone
+  #289 = NameAndType        #430:#397     // out:Ljava/io/PrintStream;
+  #290 = Utf8               Device\'s initial offset:
+  #291 = Utf8               Start date (local UNIX):
+  #292 = NameAndType        #398:#431     // append:(J)Ljava/lang/StringBuilder;
+  #293 = Utf8               Stop date (local UNIX):
+  #294 = NameAndType        #218:#219     // setAccelerationScale:(Ljava/lang/String;)D
+  #295 = Utf8               error parsing
+  #296 = Utf8               , info.txt must contain \'Sample Rate\', \' Start Date\', and (usually) \'Acceleration Scale\'.
+  #297 = NameAndType        #220:#221     // setSampleDelta:(D)D
+  #298 = NameAndType        #206:#207     // readG3TXV1EpochPairs:(Ljava/io/InputStream;Ljava/lang/String;DDDJLEpochWriter;)V
+  #299 = NameAndType        #202:#203     // readG3TXV2Epoch:(Ljava/io/InputStream;Ljava/lang/String;DDDLEpochWriter;)V
+  #300 = NameAndType        #432:#184     // close:()V
+  #301 = Class              #386          // java/io/InputStream
+  #302 = Utf8               java/lang/Exception
+  #303 = Utf8               java/io/IOException
+  #304 = NameAndType        #433:#434     // printStackTrace:(Ljava/io/PrintStream;)V
+  #305 = Utf8               error reading/writing file
+  #306 = NameAndType        #435:#436     // read:()I
+  #307 = NameAndType        #181:#182     // logger:Ljava/util/logging/Logger;
+  #308 = Class              #437          // java/util/logging/Level
+  #309 = NameAndType        #438:#439     // FINER:Ljava/util/logging/Level;
+  #310 = Utf8               \nHeader info\ntype:
+  #311 = NameAndType        #398:#440     // append:(I)Ljava/lang/StringBuilder;
+  #312 = Utf8               \nDate 0x%08X:
+  #313 = Utf8               java/lang/Object
+  #314 = NameAndType        #441:#442     // valueOf:(J)Ljava/lang/Long;
+  #315 = NameAndType        #443:#444     // format:(Ljava/lang/String;[Ljava/lang/Object;)Ljava/lang/String;
+  #316 = Utf8               \nsize:
+  #317 = Utf8               \nStarting index:
+  #318 = Class              #445          // java/util/logging/Logger
+  #319 = NameAndType        #446:#447     // log:(Ljava/util/logging/Level;Ljava/lang/String;)V
+  #320 = NameAndType        #222:#223     // isPayload:(III)Z
+  #321 = NameAndType        #448:#439     // INFO:Ljava/util/logging/Level;
+  #322 = Utf8               Processing parameter packet...
+  #323 = NameAndType        #226:#227     // isAccelScale:([B)Z
+  #324 = NameAndType        #224:#225     // decodePara:(I)D
+  #325 = Utf8               accelerationScale changed to
+  #326 = NameAndType        #398:#449     // append:(D)Ljava/lang/StringBuilder;
+  #327 = NameAndType        #209:#210     // processActivity:(Ljava/lang/String;DJBIIIIDLjava/io/InputStream;LEpochWriter;)[I
+  #328 = NameAndType        #213:#210     // processActivity2:(Ljava/lang/String;DJBIIIIDLjava/io/InputStream;LEpochWriter;)[I
+  #329 = NameAndType        #216:#217     // checkChecksum:(IIIIJII)V
+  #330 = Utf8               Done processing
+  #331 = Utf8                packets.
+  #332 = Utf8               End of .g3tx file reached
+  #333 = NameAndType        #214:#215     // readAccelPair:([BD)[D
+  #334 = Class              #450          // java/lang/Math
+  #335 = NameAndType        #451:#452     // round:(D)J
+  #336 = NameAndType        #211:#212     // getTrueUnixTime:(JLjava/lang/String;)J
+  #337 = Class              #384          // EpochWriter
+  #338 = NameAndType        #453:#454     // newValues:(JDDDD[I)Z
+  #339 = Utf8               i:
+  #340 = Utf8               x y z:
+  #341 = Utf8
+  #342 = Utf8               error when reading activity at byte
+  #343 = NameAndType        #455:#456     // charAt:(I)C
+  #344 = NameAndType        #457:#458     // substring:(I)Ljava/lang/String;
+  #345 = Class              #459          // java/time/LocalTime
+  #346 = NameAndType        #460:#461     // parse:(Ljava/lang/CharSequence;)Ljava/time/LocalTime;
+  #347 = NameAndType        #462:#436     // getHour:()I
+  #348 = NameAndType        #463:#436     // getMinute:()I
+  #349 = Utf8               \nx y z:
+  #350 = Utf8               \nTime:
+  #351 = NameAndType        #464:#439     // SEVERE:Ljava/util/logging/Level;
+  #352 = Utf8               Packet parsing failed at byte
+  #353 = Utf8               \nChecksum does not match!
+  #354 = Utf8               \nExpected 0x%08X
+  #355 = NameAndType        #441:#465     // valueOf:(I)Ljava/lang/Integer;
+  #356 = Utf8               \nObtained 0x%08X
+  #357 = Utf8               Verification succeeds
+  #358 = Utf8               NEO
+  #359 = NameAndType        #466:#467     // startsWith:(Ljava/lang/String;)Z
+  #360 = Utf8               CLE
+  #361 = Utf8               MOS
+  #362 = Utf8               sampleFreq:
+  #363 = Utf8               sampleDelta before rounding:
+  #364 = Utf8               sampleDelta after rounding:
+  #365 = Utf8               java/lang/Integer
+  #366 = NameAndType        #468:#469     // pow:(DD)D
+  #367 = Utf8               java/util/Date
+  #368 = NameAndType        #183:#470     // "<init>":(J)V
+  #369 = NameAndType        #471:#472     // getTime:()J
+  #370 = Utf8               lux.bin
+  #371 = Class              #473          // java/lang/Class
+  #372 = NameAndType        #474:#475     // getClassLoader:()Ljava/lang/ClassLoader;
+  #373 = Utf8               logging.properties
+  #374 = Class              #476          // java/lang/ClassLoader
+  #375 = NameAndType        #477:#478     // getResource:(Ljava/lang/String;)Ljava/net/URL;
+  #376 = Class              #479          // java/net/URL
+  #377 = NameAndType        #480:#401     // getFile:()Ljava/lang/String;
+  #378 = Utf8               java.util.logging.config.file
+  #379 = NameAndType        #481:#482     // setProperty:(Ljava/lang/String;Ljava/lang/String;)Ljava/lang/String;
+  #380 = NameAndType        #483:#401     // getName:()Ljava/lang/String;
+  #381 = NameAndType        #484:#485     // getLogger:(Ljava/lang/String;)Ljava/util/logging/Logger;
+  #382 = Utf8               DeviceReader
+  #383 = Utf8               java/lang/String
+  #384 = Utf8               EpochWriter
+  #385 = Utf8               java/lang/Boolean
+  #386 = Utf8               java/io/InputStream
+  #387 = Utf8               java/util/Enumeration
+  #388 = Utf8               [Ljava/lang/String;
+  #389 = Utf8               java/lang/Throwable
+  #390 = Utf8               [I
+  #391 = Utf8               [B
+  #392 = Utf8               [D
+  #393 = Utf8               (Ljava/lang/String;)V
+  #394 = Utf8               (Ljava/io/File;I)V
+  #395 = Utf8               java/lang/System
+  #396 = Utf8               err
+  #397 = Utf8               Ljava/io/PrintStream;
+  #398 = Utf8               append
+  #399 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #400 = Utf8               toString
+  #401 = Utf8               ()Ljava/lang/String;
+  #402 = Utf8               java/io/PrintStream
+  #403 = Utf8               println
+  #404 = Utf8               exit
+  #405 = Utf8               (I)V
+  #406 = Utf8               entries
+  #407 = Utf8               ()Ljava/util/Enumeration;
+  #408 = Utf8               hasMoreElements
+  #409 = Utf8               ()Z
+  #410 = Utf8               nextElement
+  #411 = Utf8               ()Ljava/lang/Object;
+  #412 = Utf8               equals
+  #413 = Utf8               (Ljava/lang/Object;)Z
+  #414 = Utf8               getInputStream
+  #415 = Utf8               (Ljava/util/zip/ZipEntry;)Ljava/io/InputStream;
+  #416 = Utf8               (Ljava/io/InputStream;)V
+  #417 = Utf8               (Ljava/io/Reader;)V
+  #418 = Utf8               ready
+  #419 = Utf8               readLine
+  #420 = Utf8               split
+  #421 = Utf8               (Ljava/lang/String;)[Ljava/lang/String;
+  #422 = Utf8               trim
+  #423 = Utf8               parseInt
+  #424 = Utf8               (Ljava/lang/String;)I
+  #425 = Utf8               java/lang/Long
+  #426 = Utf8               parseLong
+  #427 = Utf8               (Ljava/lang/String;)J
+  #428 = Utf8               java/lang/Double
+  #429 = Utf8               parseDouble
+  #430 = Utf8               out
+  #431 = Utf8               (J)Ljava/lang/StringBuilder;
+  #432 = Utf8               close
+  #433 = Utf8               printStackTrace
+  #434 = Utf8               (Ljava/io/PrintStream;)V
+  #435 = Utf8               read
+  #436 = Utf8               ()I
+  #437 = Utf8               java/util/logging/Level
+  #438 = Utf8               FINER
+  #439 = Utf8               Ljava/util/logging/Level;
+  #440 = Utf8               (I)Ljava/lang/StringBuilder;
+  #441 = Utf8               valueOf
+  #442 = Utf8               (J)Ljava/lang/Long;
+  #443 = Utf8               format
+  #444 = Utf8               (Ljava/lang/String;[Ljava/lang/Object;)Ljava/lang/String;
+  #445 = Utf8               java/util/logging/Logger
+  #446 = Utf8               log
+  #447 = Utf8               (Ljava/util/logging/Level;Ljava/lang/String;)V
+  #448 = Utf8               INFO
+  #449 = Utf8               (D)Ljava/lang/StringBuilder;
+  #450 = Utf8               java/lang/Math
+  #451 = Utf8               round
+  #452 = Utf8               (D)J
+  #453 = Utf8               newValues
+  #454 = Utf8               (JDDDD[I)Z
+  #455 = Utf8               charAt
+  #456 = Utf8               (I)C
+  #457 = Utf8               substring
+  #458 = Utf8               (I)Ljava/lang/String;
+  #459 = Utf8               java/time/LocalTime
+  #460 = Utf8               parse
+  #461 = Utf8               (Ljava/lang/CharSequence;)Ljava/time/LocalTime;
+  #462 = Utf8               getHour
+  #463 = Utf8               getMinute
+  #464 = Utf8               SEVERE
+  #465 = Utf8               (I)Ljava/lang/Integer;
+  #466 = Utf8               startsWith
+  #467 = Utf8               (Ljava/lang/String;)Z
+  #468 = Utf8               pow
+  #469 = Utf8               (DD)D
+  #470 = Utf8               (J)V
+  #471 = Utf8               getTime
+  #472 = Utf8               ()J
+  #473 = Utf8               java/lang/Class
+  #474 = Utf8               getClassLoader
+  #475 = Utf8               ()Ljava/lang/ClassLoader;
+  #476 = Utf8               java/lang/ClassLoader
+  #477 = Utf8               getResource
+  #478 = Utf8               (Ljava/lang/String;)Ljava/net/URL;
+  #479 = Utf8               java/net/URL
+  #480 = Utf8               getFile
+  #481 = Utf8               setProperty
+  #482 = Utf8               (Ljava/lang/String;Ljava/lang/String;)Ljava/lang/String;
+  #483 = Utf8               getName
+  #484 = Utf8               getLogger
+  #485 = Utf8               (Ljava/lang/String;)Ljava/util/logging/Logger;
 {
   private static final int INVALID_GT3_FILE = 0;
     descriptor: I
     flags: (0x001a) ACC_PRIVATE, ACC_STATIC, ACC_FINAL
     ConstantValue: int 0
 
   private static final int VALID_GT3_V1_FILE = 1;
```

### Comparing `accelerometer-6.2.3/accelerometer/java/ActigraphReader.java` & `accelerometer-7.0.0.dev0/src/accelerometer/java/ActigraphReader.java`

 * *Files identical despite different names*

### Comparing `accelerometer-6.2.3/accelerometer/java/AxivityReader.class` & `accelerometer-7.0.0.dev0/src/accelerometer/java/AxivityReader.class`

 * *Files 9% similar despite different names*

#### javap -verbose -constants -s -l -private {}

```diff
@@ -1,296 +1,307 @@
-  SHA-256 checksum 92994b8ad8189cc7cc5c631f2e9dd372858ee0675fbf1532cc0c804275684a21
+  SHA-256 checksum 8035345656b506993c29ebe8ae00fe08a92290e5c486e64b62863b1f0cfeb73f
   Compiled from "AxivityReader.java"
 public class AxivityReader extends DeviceReader
   minor version: 0
   major version: 52
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #95                         // AxivityReader
   super_class: #96                        // DeviceReader
   interfaces: 0, fields: 0, methods: 6, attributes: 1
 Constant pool:
-    #1 = Methodref          #96.#121      // DeviceReader."<init>":()V
-    #2 = Methodref          #95.#122      // AxivityReader.setTimeSettings:(Ljava/lang/String;I)V
-    #3 = Class              #123          // java/time/LocalDateTime
-    #4 = String             #124          //
-    #5 = Methodref          #109.#125     // java/nio/ByteBuffer.allocate:(I)Ljava/nio/ByteBuffer;
-    #6 = Class              #126          // java/io/FileInputStream
-    #7 = Methodref          #6.#127       // java/io/FileInputStream."<init>":(Ljava/lang/String;)V
-    #8 = Methodref          #6.#128       // java/io/FileInputStream.getChannel:()Ljava/nio/channels/FileChannel;
-    #9 = Methodref          #110.#129     // java/nio/channels/FileChannel.size:()J
-   #10 = Methodref          #110.#130     // java/nio/channels/FileChannel.read:(Ljava/nio/ByteBuffer;)I
-   #11 = Methodref          #95.#131      // AxivityReader.readCwaBuffer:(Ljava/nio/ByteBuffer;Z[Ljava/time/LocalDateTime;[ILjava/lang/String;[ILEpochWriter;)V
-   #12 = Methodref          #109.#132     // java/nio/ByteBuffer.clear:()Ljava/nio/Buffer;
-   #13 = Methodref          #106.#133     // java/lang/Boolean.booleanValue:()Z
-   #14 = Fieldref           #134.#135     // java/lang/System.out:Ljava/io/PrintStream;
-   #15 = Class              #136          // java/lang/StringBuilder
-   #16 = Methodref          #15.#121      // java/lang/StringBuilder."<init>":()V
-   #17 = Methodref          #15.#137      // java/lang/StringBuilder.append:(J)Ljava/lang/StringBuilder;
-   #18 = String             #138          // %\t
-   #19 = Methodref          #15.#139      // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-   #20 = Methodref          #15.#140      // java/lang/StringBuilder.toString:()Ljava/lang/String;
-   #21 = Methodref          #141.#142     // java/io/PrintStream.print:(Ljava/lang/String;)V
-   #22 = Methodref          #110.#143     // java/nio/channels/FileChannel.close:()V
-   #23 = Methodref          #6.#143       // java/io/FileInputStream.close:()V
-   #24 = Class              #144          // java/lang/Throwable
-   #25 = Methodref          #24.#145      // java/lang/Throwable.addSuppressed:(Ljava/lang/Throwable;)V
-   #26 = Class              #146          // java/lang/Exception
-   #27 = Fieldref           #134.#147     // java/lang/System.err:Ljava/io/PrintStream;
-   #28 = Methodref          #26.#148      // java/lang/Exception.printStackTrace:(Ljava/io/PrintStream;)V
-   #29 = String             #149          // error reading/writing file
-   #30 = String             #150          // :
-   #31 = Methodref          #26.#140      // java/lang/Exception.toString:()Ljava/lang/String;
-   #32 = Methodref          #141.#151     // java/io/PrintStream.println:(Ljava/lang/String;)V
-   #33 = Methodref          #134.#152     // java/lang/System.exit:(I)V
-   #34 = Class              #153          // java/util/zip/GZIPInputStream
-   #35 = Methodref          #34.#154      // java/util/zip/GZIPInputStream."<init>":(Ljava/io/InputStream;)V
-   #36 = Methodref          #155.#156     // java/nio/channels/Channels.newChannel:(Ljava/io/InputStream;)Ljava/nio/channels/ReadableByteChannel;
-   #37 = Methodref          #95.#157      // AxivityReader.getUncompressedSizeofGzipFile:(Ljava/lang/String;)J
-   #38 = InterfaceMethodref #112.#130     // java/nio/channels/ReadableByteChannel.read:(Ljava/nio/ByteBuffer;)I
-   #39 = InterfaceMethodref #112.#143     // java/nio/channels/ReadableByteChannel.close:()V
-   #40 = Methodref          #109.#158     // java/nio/ByteBuffer.flip:()Ljava/nio/Buffer;
-   #41 = Fieldref           #159.#160     // java/nio/ByteOrder.LITTLE_ENDIAN:Ljava/nio/ByteOrder;
-   #42 = Methodref          #109.#161     // java/nio/ByteBuffer.order:(Ljava/nio/ByteOrder;)Ljava/nio/ByteBuffer;
-   #43 = Methodref          #109.#162     // java/nio/ByteBuffer.get:()B
-   #44 = Methodref          #15.#163      // java/lang/StringBuilder.append:(C)Ljava/lang/StringBuilder;
-   #45 = String             #164          // MD
-   #46 = Methodref          #104.#165     // java/lang/String.equals:(Ljava/lang/Object;)Z
-   #47 = Methodref          #95.#166      // AxivityReader.cwaHeaderLoggingStartTime:(Ljava/nio/ByteBuffer;)Ljava/time/LocalDateTime;
-   #48 = Methodref          #95.#167      // AxivityReader.setSessionStart:(Ljava/time/LocalDateTime;)V
-   #49 = String             #168          // Device was programmed with delayed start time
-   #50 = String             #169          // Session start:
-   #51 = Fieldref           #95.#170      // AxivityReader.sessionStart:Ljava/time/ZonedDateTime;
-   #52 = Methodref          #15.#171      // java/lang/StringBuilder.append:(Ljava/lang/Object;)Ljava/lang/StringBuilder;
-   #53 = String             #172          // AX
-   #54 = Methodref          #95.#173      // AxivityReader.getUnsignedInt:(Ljava/nio/ByteBuffer;I)J
-   #55 = Methodref          #95.#174      // AxivityReader.getUnsignedShort:(Ljava/nio/ByteBuffer;I)I
+    #1 = Methodref          #96.#126      // DeviceReader."<init>":()V
+    #2 = Methodref          #95.#127      // AxivityReader.setTimeSettings:(Ljava/lang/String;I)V
+    #3 = Class              #128          // java/time/LocalDateTime
+    #4 = String             #129          //
+    #5 = Methodref          #130.#131     // java/nio/ByteBuffer.allocate:(I)Ljava/nio/ByteBuffer;
+    #6 = Class              #132          // java/io/FileInputStream
+    #7 = Methodref          #6.#133       // java/io/FileInputStream."<init>":(Ljava/lang/String;)V
+    #8 = Methodref          #6.#134       // java/io/FileInputStream.getChannel:()Ljava/nio/channels/FileChannel;
+    #9 = Methodref          #135.#136     // java/nio/channels/FileChannel.size:()J
+   #10 = Methodref          #135.#137     // java/nio/channels/FileChannel.read:(Ljava/nio/ByteBuffer;)I
+   #11 = Methodref          #95.#138      // AxivityReader.readCwaBuffer:(Ljava/nio/ByteBuffer;Z[Ljava/time/LocalDateTime;[ILjava/lang/String;[ILEpochWriter;)V
+   #12 = Methodref          #130.#139     // java/nio/ByteBuffer.clear:()Ljava/nio/Buffer;
+   #13 = Methodref          #140.#141     // java/lang/Boolean.booleanValue:()Z
+   #14 = Fieldref           #142.#143     // java/lang/System.out:Ljava/io/PrintStream;
+   #15 = Class              #144          // java/lang/StringBuilder
+   #16 = Methodref          #15.#126      // java/lang/StringBuilder."<init>":()V
+   #17 = Methodref          #15.#145      // java/lang/StringBuilder.append:(J)Ljava/lang/StringBuilder;
+   #18 = String             #146          // %\t
+   #19 = Methodref          #15.#147      // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+   #20 = Methodref          #15.#148      // java/lang/StringBuilder.toString:()Ljava/lang/String;
+   #21 = Methodref          #149.#150     // java/io/PrintStream.print:(Ljava/lang/String;)V
+   #22 = Methodref          #135.#151     // java/nio/channels/FileChannel.close:()V
+   #23 = Methodref          #6.#151       // java/io/FileInputStream.close:()V
+   #24 = Class              #152          // java/lang/Throwable
+   #25 = Methodref          #24.#153      // java/lang/Throwable.addSuppressed:(Ljava/lang/Throwable;)V
+   #26 = Class              #154          // java/lang/Exception
+   #27 = Fieldref           #142.#155     // java/lang/System.err:Ljava/io/PrintStream;
+   #28 = Methodref          #26.#156      // java/lang/Exception.printStackTrace:(Ljava/io/PrintStream;)V
+   #29 = String             #157          // error reading/writing file
+   #30 = String             #158          // :
+   #31 = Methodref          #26.#148      // java/lang/Exception.toString:()Ljava/lang/String;
+   #32 = Methodref          #149.#159     // java/io/PrintStream.println:(Ljava/lang/String;)V
+   #33 = Methodref          #142.#160     // java/lang/System.exit:(I)V
+   #34 = Class              #161          // java/util/zip/GZIPInputStream
+   #35 = Methodref          #34.#162      // java/util/zip/GZIPInputStream."<init>":(Ljava/io/InputStream;)V
+   #36 = Methodref          #163.#164     // java/nio/channels/Channels.newChannel:(Ljava/io/InputStream;)Ljava/nio/channels/ReadableByteChannel;
+   #37 = Methodref          #95.#165      // AxivityReader.getUncompressedSizeofGzipFile:(Ljava/lang/String;)J
+   #38 = InterfaceMethodref #166.#137     // java/nio/channels/ReadableByteChannel.read:(Ljava/nio/ByteBuffer;)I
+   #39 = InterfaceMethodref #166.#151     // java/nio/channels/ReadableByteChannel.close:()V
+   #40 = Methodref          #130.#167     // java/nio/ByteBuffer.flip:()Ljava/nio/Buffer;
+   #41 = Fieldref           #168.#169     // java/nio/ByteOrder.LITTLE_ENDIAN:Ljava/nio/ByteOrder;
+   #42 = Methodref          #130.#170     // java/nio/ByteBuffer.order:(Ljava/nio/ByteOrder;)Ljava/nio/ByteBuffer;
+   #43 = Methodref          #130.#171     // java/nio/ByteBuffer.get:()B
+   #44 = Methodref          #15.#172      // java/lang/StringBuilder.append:(C)Ljava/lang/StringBuilder;
+   #45 = String             #173          // MD
+   #46 = Methodref          #174.#175     // java/lang/String.equals:(Ljava/lang/Object;)Z
+   #47 = Methodref          #95.#176      // AxivityReader.cwaHeaderLoggingStartTime:(Ljava/nio/ByteBuffer;)Ljava/time/LocalDateTime;
+   #48 = Methodref          #95.#177      // AxivityReader.setSessionStart:(Ljava/time/LocalDateTime;)V
+   #49 = String             #178          // Device was programmed with delayed start time
+   #50 = String             #179          // Session start:
+   #51 = Fieldref           #95.#180      // AxivityReader.sessionStart:Ljava/time/ZonedDateTime;
+   #52 = Methodref          #15.#181      // java/lang/StringBuilder.append:(Ljava/lang/Object;)Ljava/lang/StringBuilder;
+   #53 = String             #182          // AX
+   #54 = Methodref          #95.#183      // AxivityReader.getUnsignedInt:(Ljava/nio/ByteBuffer;I)J
+   #55 = Methodref          #95.#184      // AxivityReader.getUnsignedShort:(Ljava/nio/ByteBuffer;I)I
    #56 = Double             150.0d
    #58 = Double             20500.0d
    #60 = Double             1000.0d
-   #62 = Methodref          #109.#175     // java/nio/ByteBuffer.get:(I)B
-   #63 = Methodref          #109.#176     // java/nio/ByteBuffer.getShort:(I)S
+   #62 = Methodref          #130.#185     // java/nio/ByteBuffer.get:(I)B
+   #63 = Methodref          #130.#186     // java/nio/ByteBuffer.getShort:(I)S
    #64 = Integer            32768
    #65 = Double             3200.0d
-   #67 = Methodref          #95.#177      // AxivityReader.getCwaTimestamp:(II)Ljava/time/LocalDateTime;
-   #68 = Methodref          #178.#179     // java/time/Duration.between:(Ljava/time/temporal/Temporal;Ljava/time/temporal/Temporal;)Ljava/time/Duration;
-   #69 = Methodref          #178.#180     // java/time/Duration.toNanos:()J
+   #67 = Methodref          #95.#187      // AxivityReader.getCwaTimestamp:(II)Ljava/time/LocalDateTime;
+   #68 = Methodref          #188.#189     // java/time/Duration.between:(Ljava/time/temporal/Temporal;Ljava/time/temporal/Temporal;)Ljava/time/Duration;
+   #69 = Methodref          #188.#190     // java/time/Duration.toNanos:()J
    #70 = Double             2.0E9d
-   #72 = Methodref          #95.#181      // AxivityReader.secs2Nanos:(D)J
-   #73 = Methodref          #3.#182       // java/time/LocalDateTime.plusNanos:(J)Ljava/time/LocalDateTime;
-   #74 = String             #183          // xyz reading err:
+   #72 = Methodref          #95.#191      // AxivityReader.secs2Nanos:(D)J
+   #73 = Methodref          #3.#192       // java/time/LocalDateTime.plusNanos:(J)Ljava/time/LocalDateTime;
+   #74 = String             #193          // xyz reading err:
    #75 = Long               -64l
    #77 = Long               6l
    #79 = Long               3l
-   #81 = String             #184          // xyz read err:
+   #81 = String             #194          // xyz read err:
    #82 = Double             256.0d
-   #84 = Methodref          #95.#185      // AxivityReader.zonedWithDSTCorrection:(Ljava/time/LocalDateTime;)Ljava/time/ZonedDateTime;
-   #85 = Methodref          #186.#187     // java/time/ZonedDateTime.toInstant:()Ljava/time/Instant;
-   #86 = Methodref          #188.#189     // java/time/Instant.toEpochMilli:()J
-   #87 = Methodref          #105.#190     // EpochWriter.newValues:(JDDDD[I)Z
-   #88 = String             #191          // block err @
-   #89 = Methodref          #186.#140     // java/time/ZonedDateTime.toString:()Ljava/lang/String;
-   #90 = Methodref          #3.#192       // java/time/LocalDateTime.of:(IIIIII)Ljava/time/LocalDateTime;
+   #84 = Methodref          #95.#195      // AxivityReader.zonedWithDSTCorrection:(Ljava/time/LocalDateTime;)Ljava/time/ZonedDateTime;
+   #85 = Methodref          #196.#197     // java/time/ZonedDateTime.toInstant:()Ljava/time/Instant;
+   #86 = Methodref          #198.#199     // java/time/Instant.toEpochMilli:()J
+   #87 = Methodref          #200.#201     // EpochWriter.newValues:(JDDDD[I)Z
+   #88 = String             #202          // block err @
+   #89 = Methodref          #196.#148     // java/time/ZonedDateTime.toString:()Ljava/lang/String;
+   #90 = Methodref          #3.#203       // java/time/LocalDateTime.of:(IIIIII)Ljava/time/LocalDateTime;
    #91 = Double             65536.0d
-   #93 = Fieldref           #95.#193      // AxivityReader.timeShift:I
-   #94 = Methodref          #3.#194       // java/time/LocalDateTime.plusMinutes:(J)Ljava/time/LocalDateTime;
-   #95 = Class              #195          // AxivityReader
-   #96 = Class              #196          // DeviceReader
+   #93 = Fieldref           #95.#204      // AxivityReader.timeShift:I
+   #94 = Methodref          #3.#205       // java/time/LocalDateTime.plusMinutes:(J)Ljava/time/LocalDateTime;
+   #95 = Class              #206          // AxivityReader
+   #96 = Class              #207          // DeviceReader
    #97 = Utf8               <init>
    #98 = Utf8               ()V
    #99 = Utf8               Code
   #100 = Utf8               LineNumberTable
   #101 = Utf8               readCwaEpochs
   #102 = Utf8               (Ljava/lang/String;Ljava/lang/String;ILEpochWriter;Ljava/lang/Boolean;)V
   #103 = Utf8               StackMapTable
-  #104 = Class              #197          // java/lang/String
-  #105 = Class              #198          // EpochWriter
-  #106 = Class              #199          // java/lang/Boolean
-  #107 = Class              #200          // "[I"
-  #108 = Class              #201          // "[Ljava/time/LocalDateTime;"
-  #109 = Class              #202          // java/nio/ByteBuffer
-  #110 = Class              #203          // java/nio/channels/FileChannel
-  #111 = Utf8               readCwaGzEpochs
-  #112 = Class              #204          // java/nio/channels/ReadableByteChannel
-  #113 = Utf8               readCwaBuffer
-  #114 = Utf8               (Ljava/nio/ByteBuffer;Z[Ljava/time/LocalDateTime;[ILjava/lang/String;[ILEpochWriter;)V
-  #115 = Utf8               getCwaTimestamp
-  #116 = Utf8               (II)Ljava/time/LocalDateTime;
-  #117 = Utf8               cwaHeaderLoggingStartTime
-  #118 = Utf8               (Ljava/nio/ByteBuffer;)Ljava/time/LocalDateTime;
-  #119 = Utf8               SourceFile
-  #120 = Utf8               AxivityReader.java
-  #121 = NameAndType        #97:#98       // "<init>":()V
-  #122 = NameAndType        #205:#206     // setTimeSettings:(Ljava/lang/String;I)V
-  #123 = Utf8               java/time/LocalDateTime
-  #124 = Utf8
-  #125 = NameAndType        #207:#208     // allocate:(I)Ljava/nio/ByteBuffer;
-  #126 = Utf8               java/io/FileInputStream
-  #127 = NameAndType        #97:#209      // "<init>":(Ljava/lang/String;)V
-  #128 = NameAndType        #210:#211     // getChannel:()Ljava/nio/channels/FileChannel;
-  #129 = NameAndType        #212:#213     // size:()J
-  #130 = NameAndType        #214:#215     // read:(Ljava/nio/ByteBuffer;)I
-  #131 = NameAndType        #113:#114     // readCwaBuffer:(Ljava/nio/ByteBuffer;Z[Ljava/time/LocalDateTime;[ILjava/lang/String;[ILEpochWriter;)V
-  #132 = NameAndType        #216:#217     // clear:()Ljava/nio/Buffer;
-  #133 = NameAndType        #218:#219     // booleanValue:()Z
-  #134 = Class              #220          // java/lang/System
-  #135 = NameAndType        #221:#222     // out:Ljava/io/PrintStream;
-  #136 = Utf8               java/lang/StringBuilder
-  #137 = NameAndType        #223:#224     // append:(J)Ljava/lang/StringBuilder;
-  #138 = Utf8               %\t
-  #139 = NameAndType        #223:#225     // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #140 = NameAndType        #226:#227     // toString:()Ljava/lang/String;
-  #141 = Class              #228          // java/io/PrintStream
-  #142 = NameAndType        #229:#209     // print:(Ljava/lang/String;)V
-  #143 = NameAndType        #230:#98      // close:()V
-  #144 = Utf8               java/lang/Throwable
-  #145 = NameAndType        #231:#232     // addSuppressed:(Ljava/lang/Throwable;)V
-  #146 = Utf8               java/lang/Exception
-  #147 = NameAndType        #233:#222     // err:Ljava/io/PrintStream;
-  #148 = NameAndType        #234:#235     // printStackTrace:(Ljava/io/PrintStream;)V
-  #149 = Utf8               error reading/writing file
-  #150 = Utf8               :
-  #151 = NameAndType        #236:#209     // println:(Ljava/lang/String;)V
-  #152 = NameAndType        #237:#238     // exit:(I)V
-  #153 = Utf8               java/util/zip/GZIPInputStream
-  #154 = NameAndType        #97:#239      // "<init>":(Ljava/io/InputStream;)V
-  #155 = Class              #240          // java/nio/channels/Channels
-  #156 = NameAndType        #241:#242     // newChannel:(Ljava/io/InputStream;)Ljava/nio/channels/ReadableByteChannel;
-  #157 = NameAndType        #243:#244     // getUncompressedSizeofGzipFile:(Ljava/lang/String;)J
-  #158 = NameAndType        #245:#217     // flip:()Ljava/nio/Buffer;
-  #159 = Class              #246          // java/nio/ByteOrder
-  #160 = NameAndType        #247:#248     // LITTLE_ENDIAN:Ljava/nio/ByteOrder;
-  #161 = NameAndType        #249:#250     // order:(Ljava/nio/ByteOrder;)Ljava/nio/ByteBuffer;
-  #162 = NameAndType        #251:#252     // get:()B
-  #163 = NameAndType        #223:#253     // append:(C)Ljava/lang/StringBuilder;
-  #164 = Utf8               MD
-  #165 = NameAndType        #254:#255     // equals:(Ljava/lang/Object;)Z
-  #166 = NameAndType        #117:#118     // cwaHeaderLoggingStartTime:(Ljava/nio/ByteBuffer;)Ljava/time/LocalDateTime;
-  #167 = NameAndType        #256:#257     // setSessionStart:(Ljava/time/LocalDateTime;)V
-  #168 = Utf8               Device was programmed with delayed start time
-  #169 = Utf8               Session start:
-  #170 = NameAndType        #258:#259     // sessionStart:Ljava/time/ZonedDateTime;
-  #171 = NameAndType        #223:#260     // append:(Ljava/lang/Object;)Ljava/lang/StringBuilder;
-  #172 = Utf8               AX
-  #173 = NameAndType        #261:#262     // getUnsignedInt:(Ljava/nio/ByteBuffer;I)J
-  #174 = NameAndType        #263:#264     // getUnsignedShort:(Ljava/nio/ByteBuffer;I)I
-  #175 = NameAndType        #251:#265     // get:(I)B
-  #176 = NameAndType        #266:#267     // getShort:(I)S
-  #177 = NameAndType        #115:#116     // getCwaTimestamp:(II)Ljava/time/LocalDateTime;
-  #178 = Class              #268          // java/time/Duration
-  #179 = NameAndType        #269:#270     // between:(Ljava/time/temporal/Temporal;Ljava/time/temporal/Temporal;)Ljava/time/Duration;
-  #180 = NameAndType        #271:#213     // toNanos:()J
-  #181 = NameAndType        #272:#273     // secs2Nanos:(D)J
-  #182 = NameAndType        #274:#275     // plusNanos:(J)Ljava/time/LocalDateTime;
-  #183 = Utf8               xyz reading err:
-  #184 = Utf8               xyz read err:
-  #185 = NameAndType        #276:#277     // zonedWithDSTCorrection:(Ljava/time/LocalDateTime;)Ljava/time/ZonedDateTime;
-  #186 = Class              #278          // java/time/ZonedDateTime
-  #187 = NameAndType        #279:#280     // toInstant:()Ljava/time/Instant;
-  #188 = Class              #281          // java/time/Instant
-  #189 = NameAndType        #282:#213     // toEpochMilli:()J
-  #190 = NameAndType        #283:#284     // newValues:(JDDDD[I)Z
-  #191 = Utf8               block err @
-  #192 = NameAndType        #285:#286     // of:(IIIIII)Ljava/time/LocalDateTime;
-  #193 = NameAndType        #287:#288     // timeShift:I
-  #194 = NameAndType        #289:#275     // plusMinutes:(J)Ljava/time/LocalDateTime;
-  #195 = Utf8               AxivityReader
-  #196 = Utf8               DeviceReader
-  #197 = Utf8               java/lang/String
-  #198 = Utf8               EpochWriter
-  #199 = Utf8               java/lang/Boolean
-  #200 = Utf8               [I
-  #201 = Utf8               [Ljava/time/LocalDateTime;
-  #202 = Utf8               java/nio/ByteBuffer
-  #203 = Utf8               java/nio/channels/FileChannel
-  #204 = Utf8               java/nio/channels/ReadableByteChannel
-  #205 = Utf8               setTimeSettings
-  #206 = Utf8               (Ljava/lang/String;I)V
-  #207 = Utf8               allocate
-  #208 = Utf8               (I)Ljava/nio/ByteBuffer;
-  #209 = Utf8               (Ljava/lang/String;)V
-  #210 = Utf8               getChannel
-  #211 = Utf8               ()Ljava/nio/channels/FileChannel;
-  #212 = Utf8               size
-  #213 = Utf8               ()J
-  #214 = Utf8               read
-  #215 = Utf8               (Ljava/nio/ByteBuffer;)I
-  #216 = Utf8               clear
-  #217 = Utf8               ()Ljava/nio/Buffer;
-  #218 = Utf8               booleanValue
-  #219 = Utf8               ()Z
-  #220 = Utf8               java/lang/System
-  #221 = Utf8               out
-  #222 = Utf8               Ljava/io/PrintStream;
-  #223 = Utf8               append
-  #224 = Utf8               (J)Ljava/lang/StringBuilder;
-  #225 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #226 = Utf8               toString
-  #227 = Utf8               ()Ljava/lang/String;
-  #228 = Utf8               java/io/PrintStream
-  #229 = Utf8               print
-  #230 = Utf8               close
-  #231 = Utf8               addSuppressed
-  #232 = Utf8               (Ljava/lang/Throwable;)V
-  #233 = Utf8               err
-  #234 = Utf8               printStackTrace
-  #235 = Utf8               (Ljava/io/PrintStream;)V
-  #236 = Utf8               println
-  #237 = Utf8               exit
-  #238 = Utf8               (I)V
-  #239 = Utf8               (Ljava/io/InputStream;)V
-  #240 = Utf8               java/nio/channels/Channels
-  #241 = Utf8               newChannel
-  #242 = Utf8               (Ljava/io/InputStream;)Ljava/nio/channels/ReadableByteChannel;
-  #243 = Utf8               getUncompressedSizeofGzipFile
-  #244 = Utf8               (Ljava/lang/String;)J
-  #245 = Utf8               flip
-  #246 = Utf8               java/nio/ByteOrder
-  #247 = Utf8               LITTLE_ENDIAN
-  #248 = Utf8               Ljava/nio/ByteOrder;
-  #249 = Utf8               order
-  #250 = Utf8               (Ljava/nio/ByteOrder;)Ljava/nio/ByteBuffer;
-  #251 = Utf8               get
-  #252 = Utf8               ()B
-  #253 = Utf8               (C)Ljava/lang/StringBuilder;
-  #254 = Utf8               equals
-  #255 = Utf8               (Ljava/lang/Object;)Z
-  #256 = Utf8               setSessionStart
-  #257 = Utf8               (Ljava/time/LocalDateTime;)V
-  #258 = Utf8               sessionStart
-  #259 = Utf8               Ljava/time/ZonedDateTime;
-  #260 = Utf8               (Ljava/lang/Object;)Ljava/lang/StringBuilder;
-  #261 = Utf8               getUnsignedInt
-  #262 = Utf8               (Ljava/nio/ByteBuffer;I)J
-  #263 = Utf8               getUnsignedShort
-  #264 = Utf8               (Ljava/nio/ByteBuffer;I)I
-  #265 = Utf8               (I)B
-  #266 = Utf8               getShort
-  #267 = Utf8               (I)S
-  #268 = Utf8               java/time/Duration
-  #269 = Utf8               between
-  #270 = Utf8               (Ljava/time/temporal/Temporal;Ljava/time/temporal/Temporal;)Ljava/time/Duration;
-  #271 = Utf8               toNanos
-  #272 = Utf8               secs2Nanos
-  #273 = Utf8               (D)J
-  #274 = Utf8               plusNanos
-  #275 = Utf8               (J)Ljava/time/LocalDateTime;
-  #276 = Utf8               zonedWithDSTCorrection
-  #277 = Utf8               (Ljava/time/LocalDateTime;)Ljava/time/ZonedDateTime;
-  #278 = Utf8               java/time/ZonedDateTime
-  #279 = Utf8               toInstant
-  #280 = Utf8               ()Ljava/time/Instant;
-  #281 = Utf8               java/time/Instant
-  #282 = Utf8               toEpochMilli
-  #283 = Utf8               newValues
-  #284 = Utf8               (JDDDD[I)Z
-  #285 = Utf8               of
-  #286 = Utf8               (IIIIII)Ljava/time/LocalDateTime;
-  #287 = Utf8               timeShift
-  #288 = Utf8               I
-  #289 = Utf8               plusMinutes
+  #104 = Class              #208          // java/lang/String
+  #105 = Class              #209          // EpochWriter
+  #106 = Class              #210          // java/lang/Boolean
+  #107 = Class              #211          // "[I"
+  #108 = Class              #212          // "[Ljava/time/LocalDateTime;"
+  #109 = Class              #213          // java/nio/ByteBuffer
+  #110 = Class              #132          // java/io/FileInputStream
+  #111 = Class              #152          // java/lang/Throwable
+  #112 = Class              #214          // java/nio/channels/FileChannel
+  #113 = Class              #154          // java/lang/Exception
+  #114 = Utf8               readCwaGzEpochs
+  #115 = Class              #161          // java/util/zip/GZIPInputStream
+  #116 = Class              #215          // java/nio/channels/ReadableByteChannel
+  #117 = Utf8               readCwaBuffer
+  #118 = Utf8               (Ljava/nio/ByteBuffer;Z[Ljava/time/LocalDateTime;[ILjava/lang/String;[ILEpochWriter;)V
+  #119 = Class              #128          // java/time/LocalDateTime
+  #120 = Utf8               getCwaTimestamp
+  #121 = Utf8               (II)Ljava/time/LocalDateTime;
+  #122 = Utf8               cwaHeaderLoggingStartTime
+  #123 = Utf8               (Ljava/nio/ByteBuffer;)Ljava/time/LocalDateTime;
+  #124 = Utf8               SourceFile
+  #125 = Utf8               AxivityReader.java
+  #126 = NameAndType        #97:#98       // "<init>":()V
+  #127 = NameAndType        #216:#217     // setTimeSettings:(Ljava/lang/String;I)V
+  #128 = Utf8               java/time/LocalDateTime
+  #129 = Utf8
+  #130 = Class              #213          // java/nio/ByteBuffer
+  #131 = NameAndType        #218:#219     // allocate:(I)Ljava/nio/ByteBuffer;
+  #132 = Utf8               java/io/FileInputStream
+  #133 = NameAndType        #97:#220      // "<init>":(Ljava/lang/String;)V
+  #134 = NameAndType        #221:#222     // getChannel:()Ljava/nio/channels/FileChannel;
+  #135 = Class              #214          // java/nio/channels/FileChannel
+  #136 = NameAndType        #223:#224     // size:()J
+  #137 = NameAndType        #225:#226     // read:(Ljava/nio/ByteBuffer;)I
+  #138 = NameAndType        #117:#118     // readCwaBuffer:(Ljava/nio/ByteBuffer;Z[Ljava/time/LocalDateTime;[ILjava/lang/String;[ILEpochWriter;)V
+  #139 = NameAndType        #227:#228     // clear:()Ljava/nio/Buffer;
+  #140 = Class              #210          // java/lang/Boolean
+  #141 = NameAndType        #229:#230     // booleanValue:()Z
+  #142 = Class              #231          // java/lang/System
+  #143 = NameAndType        #232:#233     // out:Ljava/io/PrintStream;
+  #144 = Utf8               java/lang/StringBuilder
+  #145 = NameAndType        #234:#235     // append:(J)Ljava/lang/StringBuilder;
+  #146 = Utf8               %\t
+  #147 = NameAndType        #234:#236     // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #148 = NameAndType        #237:#238     // toString:()Ljava/lang/String;
+  #149 = Class              #239          // java/io/PrintStream
+  #150 = NameAndType        #240:#220     // print:(Ljava/lang/String;)V
+  #151 = NameAndType        #241:#98      // close:()V
+  #152 = Utf8               java/lang/Throwable
+  #153 = NameAndType        #242:#243     // addSuppressed:(Ljava/lang/Throwable;)V
+  #154 = Utf8               java/lang/Exception
+  #155 = NameAndType        #244:#233     // err:Ljava/io/PrintStream;
+  #156 = NameAndType        #245:#246     // printStackTrace:(Ljava/io/PrintStream;)V
+  #157 = Utf8               error reading/writing file
+  #158 = Utf8               :
+  #159 = NameAndType        #247:#220     // println:(Ljava/lang/String;)V
+  #160 = NameAndType        #248:#249     // exit:(I)V
+  #161 = Utf8               java/util/zip/GZIPInputStream
+  #162 = NameAndType        #97:#250      // "<init>":(Ljava/io/InputStream;)V
+  #163 = Class              #251          // java/nio/channels/Channels
+  #164 = NameAndType        #252:#253     // newChannel:(Ljava/io/InputStream;)Ljava/nio/channels/ReadableByteChannel;
+  #165 = NameAndType        #254:#255     // getUncompressedSizeofGzipFile:(Ljava/lang/String;)J
+  #166 = Class              #215          // java/nio/channels/ReadableByteChannel
+  #167 = NameAndType        #256:#228     // flip:()Ljava/nio/Buffer;
+  #168 = Class              #257          // java/nio/ByteOrder
+  #169 = NameAndType        #258:#259     // LITTLE_ENDIAN:Ljava/nio/ByteOrder;
+  #170 = NameAndType        #260:#261     // order:(Ljava/nio/ByteOrder;)Ljava/nio/ByteBuffer;
+  #171 = NameAndType        #262:#263     // get:()B
+  #172 = NameAndType        #234:#264     // append:(C)Ljava/lang/StringBuilder;
+  #173 = Utf8               MD
+  #174 = Class              #208          // java/lang/String
+  #175 = NameAndType        #265:#266     // equals:(Ljava/lang/Object;)Z
+  #176 = NameAndType        #122:#123     // cwaHeaderLoggingStartTime:(Ljava/nio/ByteBuffer;)Ljava/time/LocalDateTime;
+  #177 = NameAndType        #267:#268     // setSessionStart:(Ljava/time/LocalDateTime;)V
+  #178 = Utf8               Device was programmed with delayed start time
+  #179 = Utf8               Session start:
+  #180 = NameAndType        #269:#270     // sessionStart:Ljava/time/ZonedDateTime;
+  #181 = NameAndType        #234:#271     // append:(Ljava/lang/Object;)Ljava/lang/StringBuilder;
+  #182 = Utf8               AX
+  #183 = NameAndType        #272:#273     // getUnsignedInt:(Ljava/nio/ByteBuffer;I)J
+  #184 = NameAndType        #274:#275     // getUnsignedShort:(Ljava/nio/ByteBuffer;I)I
+  #185 = NameAndType        #262:#276     // get:(I)B
+  #186 = NameAndType        #277:#278     // getShort:(I)S
+  #187 = NameAndType        #120:#121     // getCwaTimestamp:(II)Ljava/time/LocalDateTime;
+  #188 = Class              #279          // java/time/Duration
+  #189 = NameAndType        #280:#281     // between:(Ljava/time/temporal/Temporal;Ljava/time/temporal/Temporal;)Ljava/time/Duration;
+  #190 = NameAndType        #282:#224     // toNanos:()J
+  #191 = NameAndType        #283:#284     // secs2Nanos:(D)J
+  #192 = NameAndType        #285:#286     // plusNanos:(J)Ljava/time/LocalDateTime;
+  #193 = Utf8               xyz reading err:
+  #194 = Utf8               xyz read err:
+  #195 = NameAndType        #287:#288     // zonedWithDSTCorrection:(Ljava/time/LocalDateTime;)Ljava/time/ZonedDateTime;
+  #196 = Class              #289          // java/time/ZonedDateTime
+  #197 = NameAndType        #290:#291     // toInstant:()Ljava/time/Instant;
+  #198 = Class              #292          // java/time/Instant
+  #199 = NameAndType        #293:#224     // toEpochMilli:()J
+  #200 = Class              #209          // EpochWriter
+  #201 = NameAndType        #294:#295     // newValues:(JDDDD[I)Z
+  #202 = Utf8               block err @
+  #203 = NameAndType        #296:#297     // of:(IIIIII)Ljava/time/LocalDateTime;
+  #204 = NameAndType        #298:#299     // timeShift:I
+  #205 = NameAndType        #300:#286     // plusMinutes:(J)Ljava/time/LocalDateTime;
+  #206 = Utf8               AxivityReader
+  #207 = Utf8               DeviceReader
+  #208 = Utf8               java/lang/String
+  #209 = Utf8               EpochWriter
+  #210 = Utf8               java/lang/Boolean
+  #211 = Utf8               [I
+  #212 = Utf8               [Ljava/time/LocalDateTime;
+  #213 = Utf8               java/nio/ByteBuffer
+  #214 = Utf8               java/nio/channels/FileChannel
+  #215 = Utf8               java/nio/channels/ReadableByteChannel
+  #216 = Utf8               setTimeSettings
+  #217 = Utf8               (Ljava/lang/String;I)V
+  #218 = Utf8               allocate
+  #219 = Utf8               (I)Ljava/nio/ByteBuffer;
+  #220 = Utf8               (Ljava/lang/String;)V
+  #221 = Utf8               getChannel
+  #222 = Utf8               ()Ljava/nio/channels/FileChannel;
+  #223 = Utf8               size
+  #224 = Utf8               ()J
+  #225 = Utf8               read
+  #226 = Utf8               (Ljava/nio/ByteBuffer;)I
+  #227 = Utf8               clear
+  #228 = Utf8               ()Ljava/nio/Buffer;
+  #229 = Utf8               booleanValue
+  #230 = Utf8               ()Z
+  #231 = Utf8               java/lang/System
+  #232 = Utf8               out
+  #233 = Utf8               Ljava/io/PrintStream;
+  #234 = Utf8               append
+  #235 = Utf8               (J)Ljava/lang/StringBuilder;
+  #236 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #237 = Utf8               toString
+  #238 = Utf8               ()Ljava/lang/String;
+  #239 = Utf8               java/io/PrintStream
+  #240 = Utf8               print
+  #241 = Utf8               close
+  #242 = Utf8               addSuppressed
+  #243 = Utf8               (Ljava/lang/Throwable;)V
+  #244 = Utf8               err
+  #245 = Utf8               printStackTrace
+  #246 = Utf8               (Ljava/io/PrintStream;)V
+  #247 = Utf8               println
+  #248 = Utf8               exit
+  #249 = Utf8               (I)V
+  #250 = Utf8               (Ljava/io/InputStream;)V
+  #251 = Utf8               java/nio/channels/Channels
+  #252 = Utf8               newChannel
+  #253 = Utf8               (Ljava/io/InputStream;)Ljava/nio/channels/ReadableByteChannel;
+  #254 = Utf8               getUncompressedSizeofGzipFile
+  #255 = Utf8               (Ljava/lang/String;)J
+  #256 = Utf8               flip
+  #257 = Utf8               java/nio/ByteOrder
+  #258 = Utf8               LITTLE_ENDIAN
+  #259 = Utf8               Ljava/nio/ByteOrder;
+  #260 = Utf8               order
+  #261 = Utf8               (Ljava/nio/ByteOrder;)Ljava/nio/ByteBuffer;
+  #262 = Utf8               get
+  #263 = Utf8               ()B
+  #264 = Utf8               (C)Ljava/lang/StringBuilder;
+  #265 = Utf8               equals
+  #266 = Utf8               (Ljava/lang/Object;)Z
+  #267 = Utf8               setSessionStart
+  #268 = Utf8               (Ljava/time/LocalDateTime;)V
+  #269 = Utf8               sessionStart
+  #270 = Utf8               Ljava/time/ZonedDateTime;
+  #271 = Utf8               (Ljava/lang/Object;)Ljava/lang/StringBuilder;
+  #272 = Utf8               getUnsignedInt
+  #273 = Utf8               (Ljava/nio/ByteBuffer;I)J
+  #274 = Utf8               getUnsignedShort
+  #275 = Utf8               (Ljava/nio/ByteBuffer;I)I
+  #276 = Utf8               (I)B
+  #277 = Utf8               getShort
+  #278 = Utf8               (I)S
+  #279 = Utf8               java/time/Duration
+  #280 = Utf8               between
+  #281 = Utf8               (Ljava/time/temporal/Temporal;Ljava/time/temporal/Temporal;)Ljava/time/Duration;
+  #282 = Utf8               toNanos
+  #283 = Utf8               secs2Nanos
+  #284 = Utf8               (D)J
+  #285 = Utf8               plusNanos
+  #286 = Utf8               (J)Ljava/time/LocalDateTime;
+  #287 = Utf8               zonedWithDSTCorrection
+  #288 = Utf8               (Ljava/time/LocalDateTime;)Ljava/time/ZonedDateTime;
+  #289 = Utf8               java/time/ZonedDateTime
+  #290 = Utf8               toInstant
+  #291 = Utf8               ()Ljava/time/Instant;
+  #292 = Utf8               java/time/Instant
+  #293 = Utf8               toEpochMilli
+  #294 = Utf8               newValues
+  #295 = Utf8               (JDDDD[I)Z
+  #296 = Utf8               of
+  #297 = Utf8               (IIIIII)Ljava/time/LocalDateTime;
+  #298 = Utf8               timeShift
+  #299 = Utf8               I
+  #300 = Utf8               plusMinutes
 {
   public AxivityReader();
     descriptor: ()V
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
@@ -299,15 +310,15 @@
       LineNumberTable:
         line 20: 0
 
   public static void readCwaEpochs(java.lang.String, java.lang.String, int, EpochWriter, java.lang.Boolean);
     descriptor: (Ljava/lang/String;Ljava/lang/String;ILEpochWriter;Ljava/lang/Boolean;)V
     flags: (0x0009) ACC_PUBLIC, ACC_STATIC
     Code:
-      stack=7, locals=17, args_size=5
+      stack=7, locals=20, args_size=5
          0: aload_1
          1: iload_2
          2: invokestatic  #2                  // Method setTimeSettings:(Ljava/lang/String;I)V
          5: iconst_1
          6: newarray       int
          8: dup
          9: iconst_0
@@ -336,165 +347,203 @@
         44: invokestatic  #5                  // Method java/nio/ByteBuffer.allocate:(I)Ljava/nio/ByteBuffer;
         47: astore        10
         49: new           #6                  // class java/io/FileInputStream
         52: dup
         53: aload_0
         54: invokespecial #7                  // Method java/io/FileInputStream."<init>":(Ljava/lang/String;)V
         57: astore        11
-        59: aload         11
-        61: invokevirtual #8                  // Method java/io/FileInputStream.getChannel:()Ljava/nio/channels/FileChannel;
-        64: astore        12
-        66: iconst_0
-        67: istore        13
-        69: aload         12
-        71: invokevirtual #9                  // Method java/nio/channels/FileChannel.size:()J
-        74: iload         9
-        76: i2l
-        77: ldiv
-        78: lstore        14
-        80: iconst_1
-        81: istore        16
-        83: aload         12
-        85: aload         10
-        87: invokevirtual #10                 // Method java/nio/channels/FileChannel.read:(Ljava/nio/ByteBuffer;)I
-        90: iconst_m1
-        91: if_icmpeq     172
-        94: aload         10
-        96: iload         16
-        98: aload         6
-       100: aload         7
-       102: aload         8
-       104: aload         5
-       106: aload_3
-       107: invokestatic  #11                 // Method readCwaBuffer:(Ljava/nio/ByteBuffer;Z[Ljava/time/LocalDateTime;[ILjava/lang/String;[ILEpochWriter;)V
-       110: aload         10
-       112: invokevirtual #12                 // Method java/nio/ByteBuffer.clear:()Ljava/nio/Buffer;
-       115: pop
-       116: iinc          13, 1
-       119: aload         4
-       121: invokevirtual #13                 // Method java/lang/Boolean.booleanValue:()Z
-       124: ifeq          83
-       127: iload         13
-       129: sipush        10000
-       132: irem
-       133: ifne          83
-       136: getstatic     #14                 // Field java/lang/System.out:Ljava/io/PrintStream;
-       139: new           #15                 // class java/lang/StringBuilder
-       142: dup
-       143: invokespecial #16                 // Method java/lang/StringBuilder."<init>":()V
-       146: iload         13
-       148: bipush        100
-       150: imul
-       151: i2l
-       152: lload         14
-       154: ldiv
-       155: invokevirtual #17                 // Method java/lang/StringBuilder.append:(J)Ljava/lang/StringBuilder;
-       158: ldc           #18                 // String %\t
-       160: invokevirtual #19                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-       163: invokevirtual #20                 // Method java/lang/StringBuilder.toString:()Ljava/lang/String;
-       166: invokevirtual #21                 // Method java/io/PrintStream.print:(Ljava/lang/String;)V
-       169: goto          83
-       172: aload         12
-       174: invokevirtual #22                 // Method java/nio/channels/FileChannel.close:()V
-       177: aload         11
-       179: invokevirtual #23                 // Method java/io/FileInputStream.close:()V
-       182: goto          207
-       185: astore        12
-       187: aload         11
-       189: invokevirtual #23                 // Method java/io/FileInputStream.close:()V
-       192: goto          204
-       195: astore        13
-       197: aload         12
-       199: aload         13
-       201: invokevirtual #25                 // Method java/lang/Throwable.addSuppressed:(Ljava/lang/Throwable;)V
-       204: aload         12
-       206: athrow
-       207: goto          263
-       210: astore        11
-       212: aload         11
-       214: getstatic     #27                 // Field java/lang/System.err:Ljava/io/PrintStream;
-       217: invokevirtual #28                 // Method java/lang/Exception.printStackTrace:(Ljava/io/PrintStream;)V
-       220: getstatic     #27                 // Field java/lang/System.err:Ljava/io/PrintStream;
-       223: new           #15                 // class java/lang/StringBuilder
-       226: dup
-       227: invokespecial #16                 // Method java/lang/StringBuilder."<init>":()V
-       230: ldc           #29                 // String error reading/writing file
-       232: invokevirtual #19                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-       235: aload_0
-       236: invokevirtual #19                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-       239: ldc           #30                 // String :
-       241: invokevirtual #19                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-       244: aload         11
-       246: invokevirtual #31                 // Method java/lang/Exception.toString:()Ljava/lang/String;
-       249: invokevirtual #19                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-       252: invokevirtual #20                 // Method java/lang/StringBuilder.toString:()Ljava/lang/String;
-       255: invokevirtual #32                 // Method java/io/PrintStream.println:(Ljava/lang/String;)V
-       258: bipush        -2
-       260: invokestatic  #33                 // Method java/lang/System.exit:(I)V
-       263: return
+        59: aconst_null
+        60: astore        12
+        62: aload         11
+        64: invokevirtual #8                  // Method java/io/FileInputStream.getChannel:()Ljava/nio/channels/FileChannel;
+        67: astore        13
+        69: iconst_0
+        70: istore        14
+        72: aload         13
+        74: invokevirtual #9                  // Method java/nio/channels/FileChannel.size:()J
+        77: iload         9
+        79: i2l
+        80: ldiv
+        81: lstore        15
+        83: iconst_1
+        84: istore        17
+        86: aload         13
+        88: aload         10
+        90: invokevirtual #10                 // Method java/nio/channels/FileChannel.read:(Ljava/nio/ByteBuffer;)I
+        93: iconst_m1
+        94: if_icmpeq     175
+        97: aload         10
+        99: iload         17
+       101: aload         6
+       103: aload         7
+       105: aload         8
+       107: aload         5
+       109: aload_3
+       110: invokestatic  #11                 // Method readCwaBuffer:(Ljava/nio/ByteBuffer;Z[Ljava/time/LocalDateTime;[ILjava/lang/String;[ILEpochWriter;)V
+       113: aload         10
+       115: invokevirtual #12                 // Method java/nio/ByteBuffer.clear:()Ljava/nio/Buffer;
+       118: pop
+       119: iinc          14, 1
+       122: aload         4
+       124: invokevirtual #13                 // Method java/lang/Boolean.booleanValue:()Z
+       127: ifeq          86
+       130: iload         14
+       132: sipush        10000
+       135: irem
+       136: ifne          86
+       139: getstatic     #14                 // Field java/lang/System.out:Ljava/io/PrintStream;
+       142: new           #15                 // class java/lang/StringBuilder
+       145: dup
+       146: invokespecial #16                 // Method java/lang/StringBuilder."<init>":()V
+       149: iload         14
+       151: bipush        100
+       153: imul
+       154: i2l
+       155: lload         15
+       157: ldiv
+       158: invokevirtual #17                 // Method java/lang/StringBuilder.append:(J)Ljava/lang/StringBuilder;
+       161: ldc           #18                 // String %\t
+       163: invokevirtual #19                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+       166: invokevirtual #20                 // Method java/lang/StringBuilder.toString:()Ljava/lang/String;
+       169: invokevirtual #21                 // Method java/io/PrintStream.print:(Ljava/lang/String;)V
+       172: goto          86
+       175: aload         13
+       177: invokevirtual #22                 // Method java/nio/channels/FileChannel.close:()V
+       180: aload         11
+       182: ifnull        267
+       185: aload         12
+       187: ifnull        210
+       190: aload         11
+       192: invokevirtual #23                 // Method java/io/FileInputStream.close:()V
+       195: goto          267
+       198: astore        13
+       200: aload         12
+       202: aload         13
+       204: invokevirtual #25                 // Method java/lang/Throwable.addSuppressed:(Ljava/lang/Throwable;)V
+       207: goto          267
+       210: aload         11
+       212: invokevirtual #23                 // Method java/io/FileInputStream.close:()V
+       215: goto          267
+       218: astore        13
+       220: aload         13
+       222: astore        12
+       224: aload         13
+       226: athrow
+       227: astore        18
+       229: aload         11
+       231: ifnull        264
+       234: aload         12
+       236: ifnull        259
+       239: aload         11
+       241: invokevirtual #23                 // Method java/io/FileInputStream.close:()V
+       244: goto          264
+       247: astore        19
+       249: aload         12
+       251: aload         19
+       253: invokevirtual #25                 // Method java/lang/Throwable.addSuppressed:(Ljava/lang/Throwable;)V
+       256: goto          264
+       259: aload         11
+       261: invokevirtual #23                 // Method java/io/FileInputStream.close:()V
+       264: aload         18
+       266: athrow
+       267: goto          323
+       270: astore        11
+       272: aload         11
+       274: getstatic     #27                 // Field java/lang/System.err:Ljava/io/PrintStream;
+       277: invokevirtual #28                 // Method java/lang/Exception.printStackTrace:(Ljava/io/PrintStream;)V
+       280: getstatic     #27                 // Field java/lang/System.err:Ljava/io/PrintStream;
+       283: new           #15                 // class java/lang/StringBuilder
+       286: dup
+       287: invokespecial #16                 // Method java/lang/StringBuilder."<init>":()V
+       290: ldc           #29                 // String error reading/writing file
+       292: invokevirtual #19                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+       295: aload_0
+       296: invokevirtual #19                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+       299: ldc           #30                 // String :
+       301: invokevirtual #19                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+       304: aload         11
+       306: invokevirtual #31                 // Method java/lang/Exception.toString:()Ljava/lang/String;
+       309: invokevirtual #19                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+       312: invokevirtual #20                 // Method java/lang/StringBuilder.toString:()Ljava/lang/String;
+       315: invokevirtual #32                 // Method java/io/PrintStream.println:(Ljava/lang/String;)V
+       318: bipush        -2
+       320: invokestatic  #33                 // Method java/lang/System.exit:(I)V
+       323: return
       Exception table:
          from    to  target type
-            59   177   185   Class java/lang/Throwable
-           187   192   195   Class java/lang/Throwable
-            49   207   210   Class java/lang/Exception
+           190   195   198   Class java/lang/Throwable
+            62   180   218   Class java/lang/Throwable
+            62   180   227   any
+           239   244   247   Class java/lang/Throwable
+           218   229   227   any
+            49   267   270   Class java/lang/Exception
       LineNumberTable:
         line 33: 0
         line 35: 5
         line 38: 14
         line 39: 24
         line 42: 33
         line 44: 37
         line 45: 42
         line 46: 49
-        line 47: 59
-        line 50: 66
-        line 51: 69
-        line 52: 80
-        line 56: 83
-        line 57: 94
-        line 60: 110
-        line 62: 116
-        line 63: 119
-        line 64: 136
-        line 67: 172
-        line 68: 177
-        line 46: 185
-        line 72: 207
-        line 68: 210
-        line 69: 212
-        line 70: 220
-        line 71: 258
-        line 73: 263
-      StackMapTable: number_of_entries = 8
+        line 47: 62
+        line 50: 69
+        line 51: 72
+        line 52: 83
+        line 56: 86
+        line 57: 97
+        line 60: 113
+        line 62: 119
+        line 63: 122
+        line 64: 139
+        line 67: 175
+        line 68: 180
+        line 46: 218
+        line 68: 227
+        line 72: 267
+        line 68: 270
+        line 69: 272
+        line 70: 280
+        line 71: 318
+        line 73: 323
+      StackMapTable: number_of_entries = 12
         frame_type = 255 /* full_frame */
-          offset_delta = 83
-          locals = [ class java/lang/String, class java/lang/String, int, class EpochWriter, class java/lang/Boolean, class "[I", class "[Ljava/time/LocalDateTime;", class "[I", class java/lang/String, int, class java/nio/ByteBuffer, class java/io/FileInputStream, class java/nio/channels/FileChannel, int, long, int ]
+          offset_delta = 86
+          locals = [ class java/lang/String, class java/lang/String, int, class EpochWriter, class java/lang/Boolean, class "[I", class "[Ljava/time/LocalDateTime;", class "[I", class java/lang/String, int, class java/nio/ByteBuffer, class java/io/FileInputStream, class java/lang/Throwable, class java/nio/channels/FileChannel, int, long, int ]
           stack = []
         frame_type = 251 /* same_frame_extended */
           offset_delta = 88
         frame_type = 255 /* full_frame */
-          offset_delta = 12
-          locals = [ class java/lang/String, class java/lang/String, int, class EpochWriter, class java/lang/Boolean, class "[I", class "[Ljava/time/LocalDateTime;", class "[I", class java/lang/String, int, class java/nio/ByteBuffer, class java/io/FileInputStream ]
+          offset_delta = 22
+          locals = [ class java/lang/String, class java/lang/String, int, class EpochWriter, class java/lang/Boolean, class "[I", class "[Ljava/time/LocalDateTime;", class "[I", class java/lang/String, int, class java/nio/ByteBuffer, class java/io/FileInputStream, class java/lang/Throwable ]
+          stack = [ class java/lang/Throwable ]
+        frame_type = 11 /* same */
+        frame_type = 71 /* same_locals_1_stack_item */
+          stack = [ class java/lang/Throwable ]
+        frame_type = 72 /* same_locals_1_stack_item */
           stack = [ class java/lang/Throwable ]
         frame_type = 255 /* full_frame */
-          offset_delta = 9
-          locals = [ class java/lang/String, class java/lang/String, int, class EpochWriter, class java/lang/Boolean, class "[I", class "[Ljava/time/LocalDateTime;", class "[I", class java/lang/String, int, class java/nio/ByteBuffer, class java/io/FileInputStream, class java/lang/Throwable ]
+          offset_delta = 19
+          locals = [ class java/lang/String, class java/lang/String, int, class EpochWriter, class java/lang/Boolean, class "[I", class "[Ljava/time/LocalDateTime;", class "[I", class java/lang/String, int, class java/nio/ByteBuffer, class java/io/FileInputStream, class java/lang/Throwable, top, top, top, top, top, class java/lang/Throwable ]
           stack = [ class java/lang/Throwable ]
-        frame_type = 8 /* same */
-        frame_type = 249 /* chop */
+        frame_type = 11 /* same */
+        frame_type = 4 /* same */
+        frame_type = 255 /* full_frame */
           offset_delta = 2
+          locals = [ class java/lang/String, class java/lang/String, int, class EpochWriter, class java/lang/Boolean, class "[I", class "[Ljava/time/LocalDateTime;", class "[I", class java/lang/String, int, class java/nio/ByteBuffer ]
+          stack = []
         frame_type = 66 /* same_locals_1_stack_item */
           stack = [ class java/lang/Exception ]
         frame_type = 52 /* same */
 
   public static void readCwaGzEpochs(java.lang.String, java.lang.String, int, EpochWriter, java.lang.Boolean);
     descriptor: (Ljava/lang/String;Ljava/lang/String;ILEpochWriter;Ljava/lang/Boolean;)V
     flags: (0x0009) ACC_PUBLIC, ACC_STATIC
     Code:
-      stack=7, locals=18, args_size=5
+      stack=7, locals=21, args_size=5
          0: aload_1
          1: iload_2
          2: invokestatic  #2                  // Method setTimeSettings:(Ljava/lang/String;I)V
          5: iconst_1
          6: newarray       int
          8: dup
          9: iconst_0
@@ -523,162 +572,200 @@
         44: invokestatic  #5                  // Method java/nio/ByteBuffer.allocate:(I)Ljava/nio/ByteBuffer;
         47: astore        10
         49: new           #6                  // class java/io/FileInputStream
         52: dup
         53: aload_0
         54: invokespecial #7                  // Method java/io/FileInputStream."<init>":(Ljava/lang/String;)V
         57: astore        11
-        59: new           #34                 // class java/util/zip/GZIPInputStream
-        62: dup
-        63: aload         11
-        65: invokespecial #35                 // Method java/util/zip/GZIPInputStream."<init>":(Ljava/io/InputStream;)V
-        68: astore        12
-        70: aload         12
-        72: invokestatic  #36                 // Method java/nio/channels/Channels.newChannel:(Ljava/io/InputStream;)Ljava/nio/channels/ReadableByteChannel;
-        75: astore        13
-        77: iconst_0
-        78: istore        14
-        80: aload_0
-        81: invokestatic  #37                 // Method getUncompressedSizeofGzipFile:(Ljava/lang/String;)J
-        84: iload         9
-        86: i2l
-        87: ldiv
-        88: lstore        15
-        90: iconst_1
-        91: istore        17
-        93: aload         13
-        95: aload         10
-        97: invokeinterface #38,  2           // InterfaceMethod java/nio/channels/ReadableByteChannel.read:(Ljava/nio/ByteBuffer;)I
-       102: iconst_m1
-       103: if_icmpeq     184
-       106: aload         10
-       108: iload         17
-       110: aload         6
-       112: aload         7
-       114: aload         8
-       116: aload         5
-       118: aload_3
-       119: invokestatic  #11                 // Method readCwaBuffer:(Ljava/nio/ByteBuffer;Z[Ljava/time/LocalDateTime;[ILjava/lang/String;[ILEpochWriter;)V
-       122: aload         10
-       124: invokevirtual #12                 // Method java/nio/ByteBuffer.clear:()Ljava/nio/Buffer;
-       127: pop
-       128: iinc          14, 1
-       131: aload         4
-       133: invokevirtual #13                 // Method java/lang/Boolean.booleanValue:()Z
-       136: ifeq          93
-       139: iload         14
-       141: sipush        10000
-       144: irem
-       145: ifne          93
-       148: getstatic     #14                 // Field java/lang/System.out:Ljava/io/PrintStream;
-       151: new           #15                 // class java/lang/StringBuilder
-       154: dup
-       155: invokespecial #16                 // Method java/lang/StringBuilder."<init>":()V
-       158: iload         14
-       160: bipush        100
-       162: imul
-       163: i2l
-       164: lload         15
-       166: ldiv
-       167: invokevirtual #17                 // Method java/lang/StringBuilder.append:(J)Ljava/lang/StringBuilder;
-       170: ldc           #18                 // String %\t
-       172: invokevirtual #19                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-       175: invokevirtual #20                 // Method java/lang/StringBuilder.toString:()Ljava/lang/String;
-       178: invokevirtual #21                 // Method java/io/PrintStream.print:(Ljava/lang/String;)V
-       181: goto          93
-       184: aload         13
-       186: invokeinterface #39,  1           // InterfaceMethod java/nio/channels/ReadableByteChannel.close:()V
-       191: aload         11
-       193: invokevirtual #23                 // Method java/io/FileInputStream.close:()V
-       196: goto          221
-       199: astore        12
-       201: aload         11
-       203: invokevirtual #23                 // Method java/io/FileInputStream.close:()V
-       206: goto          218
-       209: astore        13
-       211: aload         12
-       213: aload         13
-       215: invokevirtual #25                 // Method java/lang/Throwable.addSuppressed:(Ljava/lang/Throwable;)V
-       218: aload         12
-       220: athrow
-       221: goto          277
-       224: astore        11
-       226: aload         11
-       228: getstatic     #27                 // Field java/lang/System.err:Ljava/io/PrintStream;
-       231: invokevirtual #28                 // Method java/lang/Exception.printStackTrace:(Ljava/io/PrintStream;)V
-       234: getstatic     #27                 // Field java/lang/System.err:Ljava/io/PrintStream;
-       237: new           #15                 // class java/lang/StringBuilder
-       240: dup
-       241: invokespecial #16                 // Method java/lang/StringBuilder."<init>":()V
-       244: ldc           #29                 // String error reading/writing file
-       246: invokevirtual #19                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-       249: aload_0
-       250: invokevirtual #19                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-       253: ldc           #30                 // String :
-       255: invokevirtual #19                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-       258: aload         11
-       260: invokevirtual #31                 // Method java/lang/Exception.toString:()Ljava/lang/String;
-       263: invokevirtual #19                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-       266: invokevirtual #20                 // Method java/lang/StringBuilder.toString:()Ljava/lang/String;
-       269: invokevirtual #32                 // Method java/io/PrintStream.println:(Ljava/lang/String;)V
-       272: bipush        -2
-       274: invokestatic  #33                 // Method java/lang/System.exit:(I)V
-       277: return
+        59: aconst_null
+        60: astore        12
+        62: new           #34                 // class java/util/zip/GZIPInputStream
+        65: dup
+        66: aload         11
+        68: invokespecial #35                 // Method java/util/zip/GZIPInputStream."<init>":(Ljava/io/InputStream;)V
+        71: astore        13
+        73: aload         13
+        75: invokestatic  #36                 // Method java/nio/channels/Channels.newChannel:(Ljava/io/InputStream;)Ljava/nio/channels/ReadableByteChannel;
+        78: astore        14
+        80: iconst_0
+        81: istore        15
+        83: aload_0
+        84: invokestatic  #37                 // Method getUncompressedSizeofGzipFile:(Ljava/lang/String;)J
+        87: iload         9
+        89: i2l
+        90: ldiv
+        91: lstore        16
+        93: iconst_1
+        94: istore        18
+        96: aload         14
+        98: aload         10
+       100: invokeinterface #38,  2           // InterfaceMethod java/nio/channels/ReadableByteChannel.read:(Ljava/nio/ByteBuffer;)I
+       105: iconst_m1
+       106: if_icmpeq     187
+       109: aload         10
+       111: iload         18
+       113: aload         6
+       115: aload         7
+       117: aload         8
+       119: aload         5
+       121: aload_3
+       122: invokestatic  #11                 // Method readCwaBuffer:(Ljava/nio/ByteBuffer;Z[Ljava/time/LocalDateTime;[ILjava/lang/String;[ILEpochWriter;)V
+       125: aload         10
+       127: invokevirtual #12                 // Method java/nio/ByteBuffer.clear:()Ljava/nio/Buffer;
+       130: pop
+       131: iinc          15, 1
+       134: aload         4
+       136: invokevirtual #13                 // Method java/lang/Boolean.booleanValue:()Z
+       139: ifeq          96
+       142: iload         15
+       144: sipush        10000
+       147: irem
+       148: ifne          96
+       151: getstatic     #14                 // Field java/lang/System.out:Ljava/io/PrintStream;
+       154: new           #15                 // class java/lang/StringBuilder
+       157: dup
+       158: invokespecial #16                 // Method java/lang/StringBuilder."<init>":()V
+       161: iload         15
+       163: bipush        100
+       165: imul
+       166: i2l
+       167: lload         16
+       169: ldiv
+       170: invokevirtual #17                 // Method java/lang/StringBuilder.append:(J)Ljava/lang/StringBuilder;
+       173: ldc           #18                 // String %\t
+       175: invokevirtual #19                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+       178: invokevirtual #20                 // Method java/lang/StringBuilder.toString:()Ljava/lang/String;
+       181: invokevirtual #21                 // Method java/io/PrintStream.print:(Ljava/lang/String;)V
+       184: goto          96
+       187: aload         14
+       189: invokeinterface #39,  1           // InterfaceMethod java/nio/channels/ReadableByteChannel.close:()V
+       194: aload         11
+       196: ifnull        281
+       199: aload         12
+       201: ifnull        224
+       204: aload         11
+       206: invokevirtual #23                 // Method java/io/FileInputStream.close:()V
+       209: goto          281
+       212: astore        13
+       214: aload         12
+       216: aload         13
+       218: invokevirtual #25                 // Method java/lang/Throwable.addSuppressed:(Ljava/lang/Throwable;)V
+       221: goto          281
+       224: aload         11
+       226: invokevirtual #23                 // Method java/io/FileInputStream.close:()V
+       229: goto          281
+       232: astore        13
+       234: aload         13
+       236: astore        12
+       238: aload         13
+       240: athrow
+       241: astore        19
+       243: aload         11
+       245: ifnull        278
+       248: aload         12
+       250: ifnull        273
+       253: aload         11
+       255: invokevirtual #23                 // Method java/io/FileInputStream.close:()V
+       258: goto          278
+       261: astore        20
+       263: aload         12
+       265: aload         20
+       267: invokevirtual #25                 // Method java/lang/Throwable.addSuppressed:(Ljava/lang/Throwable;)V
+       270: goto          278
+       273: aload         11
+       275: invokevirtual #23                 // Method java/io/FileInputStream.close:()V
+       278: aload         19
+       280: athrow
+       281: goto          337
+       284: astore        11
+       286: aload         11
+       288: getstatic     #27                 // Field java/lang/System.err:Ljava/io/PrintStream;
+       291: invokevirtual #28                 // Method java/lang/Exception.printStackTrace:(Ljava/io/PrintStream;)V
+       294: getstatic     #27                 // Field java/lang/System.err:Ljava/io/PrintStream;
+       297: new           #15                 // class java/lang/StringBuilder
+       300: dup
+       301: invokespecial #16                 // Method java/lang/StringBuilder."<init>":()V
+       304: ldc           #29                 // String error reading/writing file
+       306: invokevirtual #19                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+       309: aload_0
+       310: invokevirtual #19                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+       313: ldc           #30                 // String :
+       315: invokevirtual #19                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+       318: aload         11
+       320: invokevirtual #31                 // Method java/lang/Exception.toString:()Ljava/lang/String;
+       323: invokevirtual #19                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+       326: invokevirtual #20                 // Method java/lang/StringBuilder.toString:()Ljava/lang/String;
+       329: invokevirtual #32                 // Method java/io/PrintStream.println:(Ljava/lang/String;)V
+       332: bipush        -2
+       334: invokestatic  #33                 // Method java/lang/System.exit:(I)V
+       337: return
       Exception table:
          from    to  target type
-            59   191   199   Class java/lang/Throwable
-           201   206   209   Class java/lang/Throwable
-            49   221   224   Class java/lang/Exception
+           204   209   212   Class java/lang/Throwable
+            62   194   232   Class java/lang/Throwable
+            62   194   241   any
+           253   258   261   Class java/lang/Throwable
+           232   243   241   any
+            49   281   284   Class java/lang/Exception
       LineNumberTable:
         line 87: 0
         line 89: 5
         line 92: 14
         line 93: 24
         line 96: 33
         line 98: 37
         line 99: 42
         line 100: 49
-        line 101: 59
-        line 102: 70
-        line 105: 77
-        line 106: 80
-        line 107: 90
-        line 111: 93
-        line 112: 106
-        line 115: 122
-        line 117: 128
-        line 118: 131
-        line 119: 148
-        line 122: 184
-        line 123: 191
-        line 100: 199
-        line 127: 221
-        line 123: 224
-        line 124: 226
-        line 125: 234
-        line 126: 272
-        line 128: 277
-      StackMapTable: number_of_entries = 8
+        line 101: 62
+        line 102: 73
+        line 105: 80
+        line 106: 83
+        line 107: 93
+        line 111: 96
+        line 112: 109
+        line 115: 125
+        line 117: 131
+        line 118: 134
+        line 119: 151
+        line 122: 187
+        line 123: 194
+        line 100: 232
+        line 123: 241
+        line 127: 281
+        line 123: 284
+        line 124: 286
+        line 125: 294
+        line 126: 332
+        line 128: 337
+      StackMapTable: number_of_entries = 12
         frame_type = 255 /* full_frame */
-          offset_delta = 93
-          locals = [ class java/lang/String, class java/lang/String, int, class EpochWriter, class java/lang/Boolean, class "[I", class "[Ljava/time/LocalDateTime;", class "[I", class java/lang/String, int, class java/nio/ByteBuffer, class java/io/FileInputStream, class java/util/zip/GZIPInputStream, class java/nio/channels/ReadableByteChannel, int, long, int ]
+          offset_delta = 96
+          locals = [ class java/lang/String, class java/lang/String, int, class EpochWriter, class java/lang/Boolean, class "[I", class "[Ljava/time/LocalDateTime;", class "[I", class java/lang/String, int, class java/nio/ByteBuffer, class java/io/FileInputStream, class java/lang/Throwable, class java/util/zip/GZIPInputStream, class java/nio/channels/ReadableByteChannel, int, long, int ]
           stack = []
         frame_type = 251 /* same_frame_extended */
           offset_delta = 90
         frame_type = 255 /* full_frame */
-          offset_delta = 14
-          locals = [ class java/lang/String, class java/lang/String, int, class EpochWriter, class java/lang/Boolean, class "[I", class "[Ljava/time/LocalDateTime;", class "[I", class java/lang/String, int, class java/nio/ByteBuffer, class java/io/FileInputStream ]
+          offset_delta = 24
+          locals = [ class java/lang/String, class java/lang/String, int, class EpochWriter, class java/lang/Boolean, class "[I", class "[Ljava/time/LocalDateTime;", class "[I", class java/lang/String, int, class java/nio/ByteBuffer, class java/io/FileInputStream, class java/lang/Throwable ]
+          stack = [ class java/lang/Throwable ]
+        frame_type = 11 /* same */
+        frame_type = 71 /* same_locals_1_stack_item */
+          stack = [ class java/lang/Throwable ]
+        frame_type = 72 /* same_locals_1_stack_item */
           stack = [ class java/lang/Throwable ]
         frame_type = 255 /* full_frame */
-          offset_delta = 9
-          locals = [ class java/lang/String, class java/lang/String, int, class EpochWriter, class java/lang/Boolean, class "[I", class "[Ljava/time/LocalDateTime;", class "[I", class java/lang/String, int, class java/nio/ByteBuffer, class java/io/FileInputStream, class java/lang/Throwable ]
+          offset_delta = 19
+          locals = [ class java/lang/String, class java/lang/String, int, class EpochWriter, class java/lang/Boolean, class "[I", class "[Ljava/time/LocalDateTime;", class "[I", class java/lang/String, int, class java/nio/ByteBuffer, class java/io/FileInputStream, class java/lang/Throwable, top, top, top, top, top, top, class java/lang/Throwable ]
           stack = [ class java/lang/Throwable ]
-        frame_type = 8 /* same */
-        frame_type = 249 /* chop */
+        frame_type = 11 /* same */
+        frame_type = 4 /* same */
+        frame_type = 255 /* full_frame */
           offset_delta = 2
+          locals = [ class java/lang/String, class java/lang/String, int, class EpochWriter, class java/lang/Boolean, class "[I", class "[Ljava/time/LocalDateTime;", class "[I", class java/lang/String, int, class java/nio/ByteBuffer ]
+          stack = []
         frame_type = 66 /* same_locals_1_stack_item */
           stack = [ class java/lang/Exception ]
         frame_type = 52 /* same */
 
   private static void readCwaBuffer(java.nio.ByteBuffer, boolean, java.time.LocalDateTime[], int[], java.lang.String, int[], EpochWriter);
     descriptor: (Ljava/nio/ByteBuffer;Z[Ljava/time/LocalDateTime;[ILjava/lang/String;[ILEpochWriter;)V
     flags: (0x000a) ACC_PRIVATE, ACC_STATIC
```

### Comparing `accelerometer-6.2.3/accelerometer/java/AxivityReader.java` & `accelerometer-7.0.0.dev0/src/accelerometer/java/AxivityReader.java`

 * *Files identical despite different names*

### Comparing `accelerometer-6.2.3/accelerometer/java/BandpassFilter.class` & `accelerometer-7.0.0.dev0/src/accelerometer/java/BandpassFilter.class`

 * *Files 20% similar despite different names*

#### javap -verbose -constants -s -l -private {}

```diff
@@ -1,110 +1,112 @@
-  SHA-256 checksum 4a9c535cb7ef59159b116ff3ad85261c0f5c2afe622b644de77a583818b6f153
+  SHA-256 checksum a99bff49b51ded545066a06a9b221649ffa387542dc591cf7296bb4965a3c780
   Compiled from "BandpassFilter.java"
 public class BandpassFilter extends Filter
   minor version: 0
   major version: 52
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #33                         // BandpassFilter
   super_class: #4                         // Filter
   interfaces: 0, fields: 0, methods: 2, attributes: 1
 Constant pool:
-   #1 = Methodref          #4.#46         // Filter."<init>":()V
-   #2 = Double             2.0d
-   #4 = Class              #47            // Filter
-   #5 = Fieldref           #33.#48        // BandpassFilter.BUTTERWORTH4_NUM_COEFFICIENTS:I
-   #6 = Fieldref           #33.#49        // BandpassFilter.B:[D
-   #7 = Fieldref           #33.#50        // BandpassFilter.A:[D
-   #8 = Methodref          #33.#51        // BandpassFilter.CoefficientsButterworth4BP:(DD[D[D)V
-   #9 = Methodref          #39.#52        // java/lang/Boolean.booleanValue:()Z
-  #10 = Fieldref           #53.#54        // java/lang/System.out:Ljava/io/PrintStream;
-  #11 = Class              #55            // java/lang/StringBuilder
-  #12 = Methodref          #11.#46        // java/lang/StringBuilder."<init>":()V
-  #13 = String             #56            // B =
-  #14 = Methodref          #11.#57        // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #15 = Methodref          #58.#59        // java/util/Arrays.toString:([D)Ljava/lang/String;
-  #16 = Methodref          #11.#60        // java/lang/StringBuilder.toString:()Ljava/lang/String;
-  #17 = Methodref          #61.#62        // java/io/PrintStream.println:(Ljava/lang/String;)V
-  #18 = String             #63            // A =
-  #19 = Fieldref           #33.#64        // BandpassFilter.z:[D
-  #20 = Methodref          #33.#65        // BandpassFilter.reset:()V
-  #21 = Class              #66            // java/lang/Math
-  #22 = Double             3.141592653589793d
-  #24 = Methodref          #21.#67        // java/lang/Math.tan:(D)D
-  #25 = Double             8.0d
-  #27 = Methodref          #21.#68        // java/lang/Math.sin:(D)D
-  #28 = Methodref          #21.#69        // java/lang/Math.cos:(D)D
-  #29 = Double             -1.0d
-  #31 = Double             -2.0d
-  #33 = Class              #70            // BandpassFilter
-  #34 = Utf8               <init>
-  #35 = Utf8               (DDDLjava/lang/Boolean;)V
-  #36 = Utf8               Code
-  #37 = Utf8               LineNumberTable
-  #38 = Utf8               StackMapTable
-  #39 = Class              #71            // java/lang/Boolean
-  #40 = Utf8               CoefficientsButterworth4BP
-  #41 = Utf8               (DD[D[D)V
-  #42 = Class              #72            // "[D"
-  #43 = Class              #73            // "[I"
-  #44 = Utf8               SourceFile
-  #45 = Utf8               BandpassFilter.java
-  #46 = NameAndType        #34:#74        // "<init>":()V
-  #47 = Utf8               Filter
-  #48 = NameAndType        #75:#76        // BUTTERWORTH4_NUM_COEFFICIENTS:I
-  #49 = NameAndType        #77:#72        // B:[D
-  #50 = NameAndType        #78:#72        // A:[D
-  #51 = NameAndType        #40:#41        // CoefficientsButterworth4BP:(DD[D[D)V
-  #52 = NameAndType        #79:#80        // booleanValue:()Z
-  #53 = Class              #81            // java/lang/System
-  #54 = NameAndType        #82:#83        // out:Ljava/io/PrintStream;
-  #55 = Utf8               java/lang/StringBuilder
-  #56 = Utf8               B =
-  #57 = NameAndType        #84:#85        // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #58 = Class              #86            // java/util/Arrays
-  #59 = NameAndType        #87:#88        // toString:([D)Ljava/lang/String;
-  #60 = NameAndType        #87:#89        // toString:()Ljava/lang/String;
-  #61 = Class              #90            // java/io/PrintStream
-  #62 = NameAndType        #91:#92        // println:(Ljava/lang/String;)V
-  #63 = Utf8               A =
-  #64 = NameAndType        #93:#72        // z:[D
-  #65 = NameAndType        #94:#74        // reset:()V
-  #66 = Utf8               java/lang/Math
-  #67 = NameAndType        #95:#96        // tan:(D)D
-  #68 = NameAndType        #97:#96        // sin:(D)D
-  #69 = NameAndType        #98:#96        // cos:(D)D
-  #70 = Utf8               BandpassFilter
-  #71 = Utf8               java/lang/Boolean
-  #72 = Utf8               [D
-  #73 = Utf8               [I
-  #74 = Utf8               ()V
-  #75 = Utf8               BUTTERWORTH4_NUM_COEFFICIENTS
-  #76 = Utf8               I
-  #77 = Utf8               B
-  #78 = Utf8               A
-  #79 = Utf8               booleanValue
-  #80 = Utf8               ()Z
-  #81 = Utf8               java/lang/System
-  #82 = Utf8               out
-  #83 = Utf8               Ljava/io/PrintStream;
-  #84 = Utf8               append
-  #85 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #86 = Utf8               java/util/Arrays
-  #87 = Utf8               toString
-  #88 = Utf8               ([D)Ljava/lang/String;
-  #89 = Utf8               ()Ljava/lang/String;
-  #90 = Utf8               java/io/PrintStream
-  #91 = Utf8               println
-  #92 = Utf8               (Ljava/lang/String;)V
-  #93 = Utf8               z
-  #94 = Utf8               reset
-  #95 = Utf8               tan
-  #96 = Utf8               (D)D
-  #97 = Utf8               sin
-  #98 = Utf8               cos
+    #1 = Methodref          #4.#47        // Filter."<init>":()V
+    #2 = Double             2.0d
+    #4 = Class              #48           // Filter
+    #5 = Fieldref           #33.#49       // BandpassFilter.BUTTERWORTH4_NUM_COEFFICIENTS:I
+    #6 = Fieldref           #33.#50       // BandpassFilter.B:[D
+    #7 = Fieldref           #33.#51       // BandpassFilter.A:[D
+    #8 = Methodref          #33.#52       // BandpassFilter.CoefficientsButterworth4BP:(DD[D[D)V
+    #9 = Methodref          #53.#54       // java/lang/Boolean.booleanValue:()Z
+   #10 = Fieldref           #55.#56       // java/lang/System.out:Ljava/io/PrintStream;
+   #11 = Class              #57           // java/lang/StringBuilder
+   #12 = Methodref          #11.#47       // java/lang/StringBuilder."<init>":()V
+   #13 = String             #58           // B =
+   #14 = Methodref          #11.#59       // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+   #15 = Methodref          #60.#61       // java/util/Arrays.toString:([D)Ljava/lang/String;
+   #16 = Methodref          #11.#62       // java/lang/StringBuilder.toString:()Ljava/lang/String;
+   #17 = Methodref          #63.#64       // java/io/PrintStream.println:(Ljava/lang/String;)V
+   #18 = String             #65           // A =
+   #19 = Fieldref           #33.#66       // BandpassFilter.z:[D
+   #20 = Methodref          #33.#67       // BandpassFilter.reset:()V
+   #21 = Class              #68           // java/lang/Math
+   #22 = Double             3.141592653589793d
+   #24 = Methodref          #21.#69       // java/lang/Math.tan:(D)D
+   #25 = Double             8.0d
+   #27 = Methodref          #21.#70       // java/lang/Math.sin:(D)D
+   #28 = Methodref          #21.#71       // java/lang/Math.cos:(D)D
+   #29 = Double             -1.0d
+   #31 = Double             -2.0d
+   #33 = Class              #72           // BandpassFilter
+   #34 = Utf8               <init>
+   #35 = Utf8               (DDDLjava/lang/Boolean;)V
+   #36 = Utf8               Code
+   #37 = Utf8               LineNumberTable
+   #38 = Utf8               StackMapTable
+   #39 = Class              #72           // BandpassFilter
+   #40 = Class              #73           // java/lang/Boolean
+   #41 = Utf8               CoefficientsButterworth4BP
+   #42 = Utf8               (DD[D[D)V
+   #43 = Class              #74           // "[D"
+   #44 = Class              #75           // "[I"
+   #45 = Utf8               SourceFile
+   #46 = Utf8               BandpassFilter.java
+   #47 = NameAndType        #34:#76       // "<init>":()V
+   #48 = Utf8               Filter
+   #49 = NameAndType        #77:#78       // BUTTERWORTH4_NUM_COEFFICIENTS:I
+   #50 = NameAndType        #79:#74       // B:[D
+   #51 = NameAndType        #80:#74       // A:[D
+   #52 = NameAndType        #41:#42       // CoefficientsButterworth4BP:(DD[D[D)V
+   #53 = Class              #73           // java/lang/Boolean
+   #54 = NameAndType        #81:#82       // booleanValue:()Z
+   #55 = Class              #83           // java/lang/System
+   #56 = NameAndType        #84:#85       // out:Ljava/io/PrintStream;
+   #57 = Utf8               java/lang/StringBuilder
+   #58 = Utf8               B =
+   #59 = NameAndType        #86:#87       // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+   #60 = Class              #88           // java/util/Arrays
+   #61 = NameAndType        #89:#90       // toString:([D)Ljava/lang/String;
+   #62 = NameAndType        #89:#91       // toString:()Ljava/lang/String;
+   #63 = Class              #92           // java/io/PrintStream
+   #64 = NameAndType        #93:#94       // println:(Ljava/lang/String;)V
+   #65 = Utf8               A =
+   #66 = NameAndType        #95:#74       // z:[D
+   #67 = NameAndType        #96:#76       // reset:()V
+   #68 = Utf8               java/lang/Math
+   #69 = NameAndType        #97:#98       // tan:(D)D
+   #70 = NameAndType        #99:#98       // sin:(D)D
+   #71 = NameAndType        #100:#98      // cos:(D)D
+   #72 = Utf8               BandpassFilter
+   #73 = Utf8               java/lang/Boolean
+   #74 = Utf8               [D
+   #75 = Utf8               [I
+   #76 = Utf8               ()V
+   #77 = Utf8               BUTTERWORTH4_NUM_COEFFICIENTS
+   #78 = Utf8               I
+   #79 = Utf8               B
+   #80 = Utf8               A
+   #81 = Utf8               booleanValue
+   #82 = Utf8               ()Z
+   #83 = Utf8               java/lang/System
+   #84 = Utf8               out
+   #85 = Utf8               Ljava/io/PrintStream;
+   #86 = Utf8               append
+   #87 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
+   #88 = Utf8               java/util/Arrays
+   #89 = Utf8               toString
+   #90 = Utf8               ([D)Ljava/lang/String;
+   #91 = Utf8               ()Ljava/lang/String;
+   #92 = Utf8               java/io/PrintStream
+   #93 = Utf8               println
+   #94 = Utf8               (Ljava/lang/String;)V
+   #95 = Utf8               z
+   #96 = Utf8               reset
+   #97 = Utf8               tan
+   #98 = Utf8               (D)D
+   #99 = Utf8               sin
+  #100 = Utf8               cos
 {
   public BandpassFilter(double, double, double, java.lang.Boolean);
     descriptor: (DDDLjava/lang/Boolean;)V
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=7, locals=12, args_size=5
          0: aload_0
```

### Comparing `accelerometer-6.2.3/accelerometer/java/BandpassFilter.java` & `accelerometer-7.0.0.dev0/src/accelerometer/java/BandpassFilter.java`

 * *Files identical despite different names*

### Comparing `accelerometer-6.2.3/accelerometer/java/CsvReader.class` & `accelerometer-7.0.0.dev0/src/accelerometer/java/CsvReader.class`

 * *Files 18% similar despite different names*

#### javap -verbose -constants -s -l -private {}

```diff
@@ -1,168 +1,173 @@
-  SHA-256 checksum 25af4d222d9326833b5325150441ef136ccfd92af63d7ab2ea93a6feb2585f53
+  SHA-256 checksum 3f08ee2f695e44f976e09676a53a407d8b525e6cc40528fec255e6826e8c3e2d
   Compiled from "CsvReader.java"
 public class CsvReader extends DeviceReader
   minor version: 0
   major version: 52
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #44                         // CsvReader
   super_class: #45                        // DeviceReader
   interfaces: 0, fields: 1, methods: 3, attributes: 1
 Constant pool:
-    #1 = Methodref          #45.#66       // DeviceReader."<init>":()V
-    #2 = Methodref          #55.#67       // java/lang/String.toLowerCase:()Ljava/lang/String;
-    #3 = String             #68           // .csv.gz
-    #4 = Methodref          #55.#69       // java/lang/String.endsWith:(Ljava/lang/String;)Z
-    #5 = Class              #70           // java/io/FileInputStream
-    #6 = Methodref          #5.#71        // java/io/FileInputStream."<init>":(Ljava/lang/String;)V
-    #7 = Class              #72           // java/util/zip/GZIPInputStream
-    #8 = Methodref          #7.#73        // java/util/zip/GZIPInputStream."<init>":(Ljava/io/InputStream;)V
-    #9 = Class              #74           // java/io/InputStreamReader
-   #10 = Methodref          #9.#73        // java/io/InputStreamReader."<init>":(Ljava/io/InputStream;)V
-   #11 = Class              #75           // java/io/BufferedReader
-   #12 = Methodref          #11.#76       // java/io/BufferedReader."<init>":(Ljava/io/Reader;)V
-   #13 = Class              #77           // java/io/FileReader
-   #14 = Methodref          #13.#71       // java/io/FileReader."<init>":(Ljava/lang/String;)V
-   #15 = String             #78           //
-   #16 = String             #79           // ,
-   #17 = InterfaceMethodref #57.#80       // java/util/List.get:(I)Ljava/lang/Object;
-   #18 = Class              #81           // java/lang/Integer
-   #19 = Methodref          #18.#82       // java/lang/Integer.intValue:()I
-   #20 = Fieldref           #44.#83       // CsvReader.NO_TEMPERATURE:I
-   #21 = InterfaceMethodref #57.#84       // java/util/List.size:()I
-   #22 = Class              #85           // java/lang/Long
+    #1 = Methodref          #45.#68       // DeviceReader."<init>":()V
+    #2 = Methodref          #69.#70       // java/lang/String.toLowerCase:()Ljava/lang/String;
+    #3 = String             #71           // .csv.gz
+    #4 = Methodref          #69.#72       // java/lang/String.endsWith:(Ljava/lang/String;)Z
+    #5 = Class              #73           // java/io/FileInputStream
+    #6 = Methodref          #5.#74        // java/io/FileInputStream."<init>":(Ljava/lang/String;)V
+    #7 = Class              #75           // java/util/zip/GZIPInputStream
+    #8 = Methodref          #7.#76        // java/util/zip/GZIPInputStream."<init>":(Ljava/io/InputStream;)V
+    #9 = Class              #77           // java/io/InputStreamReader
+   #10 = Methodref          #9.#76        // java/io/InputStreamReader."<init>":(Ljava/io/InputStream;)V
+   #11 = Class              #78           // java/io/BufferedReader
+   #12 = Methodref          #11.#79       // java/io/BufferedReader."<init>":(Ljava/io/Reader;)V
+   #13 = Class              #80           // java/io/FileReader
+   #14 = Methodref          #13.#74       // java/io/FileReader."<init>":(Ljava/lang/String;)V
+   #15 = String             #81           //
+   #16 = String             #82           // ,
+   #17 = InterfaceMethodref #83.#84       // java/util/List.get:(I)Ljava/lang/Object;
+   #18 = Class              #85           // java/lang/Integer
+   #19 = Methodref          #18.#86       // java/lang/Integer.intValue:()I
+   #20 = Fieldref           #44.#87       // CsvReader.NO_TEMPERATURE:I
+   #21 = InterfaceMethodref #83.#88       // java/util/List.size:()I
+   #22 = Class              #89           // java/lang/Long
    #23 = Long               -9223372036854775808l
-   #25 = Methodref          #11.#86       // java/io/BufferedReader.readLine:()Ljava/lang/String;
-   #26 = Methodref          #11.#87       // java/io/BufferedReader.close:()V
-   #27 = Methodref          #55.#88       // java/lang/String.split:(Ljava/lang/String;)[Ljava/lang/String;
-   #28 = Methodref          #89.#90       // java/time/LocalDateTime.parse:(Ljava/lang/CharSequence;Ljava/time/format/DateTimeFormatter;)Ljava/time/LocalDateTime;
-   #29 = Methodref          #44.#91       // CsvReader.getEpochMillis:(Ljava/time/LocalDateTime;)J
-   #30 = Methodref          #92.#93       // java/lang/Double.parseDouble:(Ljava/lang/String;)D
-   #31 = Methodref          #56.#94       // EpochWriter.newValues:(JDDDD[I)Z
-   #32 = Class              #95           // java/lang/Exception
-   #33 = Fieldref           #96.#97       // java/lang/System.err:Ljava/io/PrintStream;
-   #34 = Methodref          #32.#98       // java/lang/Exception.printStackTrace:(Ljava/io/PrintStream;)V
-   #35 = Class              #99           // java/lang/StringBuilder
-   #36 = Methodref          #35.#66       // java/lang/StringBuilder."<init>":()V
-   #37 = String             #100          // error reading/writing file
-   #38 = Methodref          #35.#101      // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-   #39 = String             #102          // :
-   #40 = Methodref          #32.#103      // java/lang/Exception.toString:()Ljava/lang/String;
-   #41 = Methodref          #35.#103      // java/lang/StringBuilder.toString:()Ljava/lang/String;
-   #42 = Methodref          #104.#105     // java/io/PrintStream.println:(Ljava/lang/String;)V
-   #43 = Methodref          #96.#106      // java/lang/System.exit:(I)V
-   #44 = Class              #107          // CsvReader
-   #45 = Class              #108          // DeviceReader
+   #25 = Methodref          #11.#90       // java/io/BufferedReader.readLine:()Ljava/lang/String;
+   #26 = Methodref          #11.#91       // java/io/BufferedReader.close:()V
+   #27 = Methodref          #69.#92       // java/lang/String.split:(Ljava/lang/String;)[Ljava/lang/String;
+   #28 = Methodref          #93.#94       // java/time/LocalDateTime.parse:(Ljava/lang/CharSequence;Ljava/time/format/DateTimeFormatter;)Ljava/time/LocalDateTime;
+   #29 = Methodref          #44.#95       // CsvReader.getEpochMillis:(Ljava/time/LocalDateTime;)J
+   #30 = Methodref          #96.#97       // java/lang/Double.parseDouble:(Ljava/lang/String;)D
+   #31 = Methodref          #98.#99       // EpochWriter.newValues:(JDDDD[I)Z
+   #32 = Class              #100          // java/lang/Exception
+   #33 = Fieldref           #101.#102     // java/lang/System.err:Ljava/io/PrintStream;
+   #34 = Methodref          #32.#103      // java/lang/Exception.printStackTrace:(Ljava/io/PrintStream;)V
+   #35 = Class              #104          // java/lang/StringBuilder
+   #36 = Methodref          #35.#68       // java/lang/StringBuilder."<init>":()V
+   #37 = String             #105          // error reading/writing file
+   #38 = Methodref          #35.#106      // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+   #39 = String             #107          // :
+   #40 = Methodref          #32.#108      // java/lang/Exception.toString:()Ljava/lang/String;
+   #41 = Methodref          #35.#108      // java/lang/StringBuilder.toString:()Ljava/lang/String;
+   #42 = Methodref          #109.#110     // java/io/PrintStream.println:(Ljava/lang/String;)V
+   #43 = Methodref          #101.#111     // java/lang/System.exit:(I)V
+   #44 = Class              #112          // CsvReader
+   #45 = Class              #113          // DeviceReader
    #46 = Utf8               NO_TEMPERATURE
    #47 = Utf8               I
    #48 = Utf8               <init>
    #49 = Utf8               ()V
    #50 = Utf8               Code
    #51 = Utf8               LineNumberTable
    #52 = Utf8               readCSVEpochs
    #53 = Utf8               (Ljava/lang/String;LEpochWriter;ILjava/util/List;Ljava/time/format/DateTimeFormatter;Ljava/lang/Boolean;)V
    #54 = Utf8               StackMapTable
-   #55 = Class              #109          // java/lang/String
-   #56 = Class              #110          // EpochWriter
-   #57 = Class              #111          // java/util/List
-   #58 = Class              #112          // java/time/format/DateTimeFormatter
-   #59 = Class              #113          // java/lang/Boolean
-   #60 = Class              #114          // "[Ljava/lang/String;"
-   #61 = Utf8               Signature
-   #62 = Utf8               (Ljava/lang/String;LEpochWriter;ILjava/util/List<Ljava/lang/Integer;>;Ljava/time/format/DateTimeFormatter;Ljava/lang/Boolean;)V
-   #63 = Utf8               <clinit>
-   #64 = Utf8               SourceFile
-   #65 = Utf8               CsvReader.java
-   #66 = NameAndType        #48:#49       // "<init>":()V
-   #67 = NameAndType        #115:#116     // toLowerCase:()Ljava/lang/String;
-   #68 = Utf8               .csv.gz
-   #69 = NameAndType        #117:#118     // endsWith:(Ljava/lang/String;)Z
-   #70 = Utf8               java/io/FileInputStream
-   #71 = NameAndType        #48:#119      // "<init>":(Ljava/lang/String;)V
-   #72 = Utf8               java/util/zip/GZIPInputStream
-   #73 = NameAndType        #48:#120      // "<init>":(Ljava/io/InputStream;)V
-   #74 = Utf8               java/io/InputStreamReader
-   #75 = Utf8               java/io/BufferedReader
-   #76 = NameAndType        #48:#121      // "<init>":(Ljava/io/Reader;)V
-   #77 = Utf8               java/io/FileReader
-   #78 = Utf8
-   #79 = Utf8               ,
-   #80 = NameAndType        #122:#123     // get:(I)Ljava/lang/Object;
-   #81 = Utf8               java/lang/Integer
-   #82 = NameAndType        #124:#125     // intValue:()I
-   #83 = NameAndType        #46:#47       // NO_TEMPERATURE:I
-   #84 = NameAndType        #126:#125     // size:()I
-   #85 = Utf8               java/lang/Long
-   #86 = NameAndType        #127:#116     // readLine:()Ljava/lang/String;
-   #87 = NameAndType        #128:#49      // close:()V
-   #88 = NameAndType        #129:#130     // split:(Ljava/lang/String;)[Ljava/lang/String;
-   #89 = Class              #131          // java/time/LocalDateTime
-   #90 = NameAndType        #132:#133     // parse:(Ljava/lang/CharSequence;Ljava/time/format/DateTimeFormatter;)Ljava/time/LocalDateTime;
-   #91 = NameAndType        #134:#135     // getEpochMillis:(Ljava/time/LocalDateTime;)J
-   #92 = Class              #136          // java/lang/Double
-   #93 = NameAndType        #137:#138     // parseDouble:(Ljava/lang/String;)D
-   #94 = NameAndType        #139:#140     // newValues:(JDDDD[I)Z
-   #95 = Utf8               java/lang/Exception
-   #96 = Class              #141          // java/lang/System
-   #97 = NameAndType        #142:#143     // err:Ljava/io/PrintStream;
-   #98 = NameAndType        #144:#145     // printStackTrace:(Ljava/io/PrintStream;)V
-   #99 = Utf8               java/lang/StringBuilder
-  #100 = Utf8               error reading/writing file
-  #101 = NameAndType        #146:#147     // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #102 = Utf8               :
-  #103 = NameAndType        #148:#116     // toString:()Ljava/lang/String;
-  #104 = Class              #149          // java/io/PrintStream
-  #105 = NameAndType        #150:#119     // println:(Ljava/lang/String;)V
-  #106 = NameAndType        #151:#152     // exit:(I)V
-  #107 = Utf8               CsvReader
-  #108 = Utf8               DeviceReader
-  #109 = Utf8               java/lang/String
-  #110 = Utf8               EpochWriter
-  #111 = Utf8               java/util/List
-  #112 = Utf8               java/time/format/DateTimeFormatter
-  #113 = Utf8               java/lang/Boolean
-  #114 = Utf8               [Ljava/lang/String;
-  #115 = Utf8               toLowerCase
-  #116 = Utf8               ()Ljava/lang/String;
-  #117 = Utf8               endsWith
-  #118 = Utf8               (Ljava/lang/String;)Z
-  #119 = Utf8               (Ljava/lang/String;)V
-  #120 = Utf8               (Ljava/io/InputStream;)V
-  #121 = Utf8               (Ljava/io/Reader;)V
-  #122 = Utf8               get
-  #123 = Utf8               (I)Ljava/lang/Object;
-  #124 = Utf8               intValue
-  #125 = Utf8               ()I
-  #126 = Utf8               size
-  #127 = Utf8               readLine
-  #128 = Utf8               close
-  #129 = Utf8               split
-  #130 = Utf8               (Ljava/lang/String;)[Ljava/lang/String;
-  #131 = Utf8               java/time/LocalDateTime
-  #132 = Utf8               parse
-  #133 = Utf8               (Ljava/lang/CharSequence;Ljava/time/format/DateTimeFormatter;)Ljava/time/LocalDateTime;
-  #134 = Utf8               getEpochMillis
-  #135 = Utf8               (Ljava/time/LocalDateTime;)J
-  #136 = Utf8               java/lang/Double
-  #137 = Utf8               parseDouble
-  #138 = Utf8               (Ljava/lang/String;)D
-  #139 = Utf8               newValues
-  #140 = Utf8               (JDDDD[I)Z
-  #141 = Utf8               java/lang/System
-  #142 = Utf8               err
-  #143 = Utf8               Ljava/io/PrintStream;
-  #144 = Utf8               printStackTrace
-  #145 = Utf8               (Ljava/io/PrintStream;)V
-  #146 = Utf8               append
-  #147 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #148 = Utf8               toString
-  #149 = Utf8               java/io/PrintStream
-  #150 = Utf8               println
-  #151 = Utf8               exit
-  #152 = Utf8               (I)V
+   #55 = Class              #78           // java/io/BufferedReader
+   #56 = Class              #114          // java/lang/String
+   #57 = Class              #115          // EpochWriter
+   #58 = Class              #116          // java/util/List
+   #59 = Class              #117          // java/time/format/DateTimeFormatter
+   #60 = Class              #118          // java/lang/Boolean
+   #61 = Class              #119          // "[Ljava/lang/String;"
+   #62 = Class              #100          // java/lang/Exception
+   #63 = Utf8               Signature
+   #64 = Utf8               (Ljava/lang/String;LEpochWriter;ILjava/util/List<Ljava/lang/Integer;>;Ljava/time/format/DateTimeFormatter;Ljava/lang/Boolean;)V
+   #65 = Utf8               <clinit>
+   #66 = Utf8               SourceFile
+   #67 = Utf8               CsvReader.java
+   #68 = NameAndType        #48:#49       // "<init>":()V
+   #69 = Class              #114          // java/lang/String
+   #70 = NameAndType        #120:#121     // toLowerCase:()Ljava/lang/String;
+   #71 = Utf8               .csv.gz
+   #72 = NameAndType        #122:#123     // endsWith:(Ljava/lang/String;)Z
+   #73 = Utf8               java/io/FileInputStream
+   #74 = NameAndType        #48:#124      // "<init>":(Ljava/lang/String;)V
+   #75 = Utf8               java/util/zip/GZIPInputStream
+   #76 = NameAndType        #48:#125      // "<init>":(Ljava/io/InputStream;)V
+   #77 = Utf8               java/io/InputStreamReader
+   #78 = Utf8               java/io/BufferedReader
+   #79 = NameAndType        #48:#126      // "<init>":(Ljava/io/Reader;)V
+   #80 = Utf8               java/io/FileReader
+   #81 = Utf8
+   #82 = Utf8               ,
+   #83 = Class              #116          // java/util/List
+   #84 = NameAndType        #127:#128     // get:(I)Ljava/lang/Object;
+   #85 = Utf8               java/lang/Integer
+   #86 = NameAndType        #129:#130     // intValue:()I
+   #87 = NameAndType        #46:#47       // NO_TEMPERATURE:I
+   #88 = NameAndType        #131:#130     // size:()I
+   #89 = Utf8               java/lang/Long
+   #90 = NameAndType        #132:#121     // readLine:()Ljava/lang/String;
+   #91 = NameAndType        #133:#49      // close:()V
+   #92 = NameAndType        #134:#135     // split:(Ljava/lang/String;)[Ljava/lang/String;
+   #93 = Class              #136          // java/time/LocalDateTime
+   #94 = NameAndType        #137:#138     // parse:(Ljava/lang/CharSequence;Ljava/time/format/DateTimeFormatter;)Ljava/time/LocalDateTime;
+   #95 = NameAndType        #139:#140     // getEpochMillis:(Ljava/time/LocalDateTime;)J
+   #96 = Class              #141          // java/lang/Double
+   #97 = NameAndType        #142:#143     // parseDouble:(Ljava/lang/String;)D
+   #98 = Class              #115          // EpochWriter
+   #99 = NameAndType        #144:#145     // newValues:(JDDDD[I)Z
+  #100 = Utf8               java/lang/Exception
+  #101 = Class              #146          // java/lang/System
+  #102 = NameAndType        #147:#148     // err:Ljava/io/PrintStream;
+  #103 = NameAndType        #149:#150     // printStackTrace:(Ljava/io/PrintStream;)V
+  #104 = Utf8               java/lang/StringBuilder
+  #105 = Utf8               error reading/writing file
+  #106 = NameAndType        #151:#152     // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #107 = Utf8               :
+  #108 = NameAndType        #153:#121     // toString:()Ljava/lang/String;
+  #109 = Class              #154          // java/io/PrintStream
+  #110 = NameAndType        #155:#124     // println:(Ljava/lang/String;)V
+  #111 = NameAndType        #156:#157     // exit:(I)V
+  #112 = Utf8               CsvReader
+  #113 = Utf8               DeviceReader
+  #114 = Utf8               java/lang/String
+  #115 = Utf8               EpochWriter
+  #116 = Utf8               java/util/List
+  #117 = Utf8               java/time/format/DateTimeFormatter
+  #118 = Utf8               java/lang/Boolean
+  #119 = Utf8               [Ljava/lang/String;
+  #120 = Utf8               toLowerCase
+  #121 = Utf8               ()Ljava/lang/String;
+  #122 = Utf8               endsWith
+  #123 = Utf8               (Ljava/lang/String;)Z
+  #124 = Utf8               (Ljava/lang/String;)V
+  #125 = Utf8               (Ljava/io/InputStream;)V
+  #126 = Utf8               (Ljava/io/Reader;)V
+  #127 = Utf8               get
+  #128 = Utf8               (I)Ljava/lang/Object;
+  #129 = Utf8               intValue
+  #130 = Utf8               ()I
+  #131 = Utf8               size
+  #132 = Utf8               readLine
+  #133 = Utf8               close
+  #134 = Utf8               split
+  #135 = Utf8               (Ljava/lang/String;)[Ljava/lang/String;
+  #136 = Utf8               java/time/LocalDateTime
+  #137 = Utf8               parse
+  #138 = Utf8               (Ljava/lang/CharSequence;Ljava/time/format/DateTimeFormatter;)Ljava/time/LocalDateTime;
+  #139 = Utf8               getEpochMillis
+  #140 = Utf8               (Ljava/time/LocalDateTime;)J
+  #141 = Utf8               java/lang/Double
+  #142 = Utf8               parseDouble
+  #143 = Utf8               (Ljava/lang/String;)D
+  #144 = Utf8               newValues
+  #145 = Utf8               (JDDDD[I)Z
+  #146 = Utf8               java/lang/System
+  #147 = Utf8               err
+  #148 = Utf8               Ljava/io/PrintStream;
+  #149 = Utf8               printStackTrace
+  #150 = Utf8               (Ljava/io/PrintStream;)V
+  #151 = Utf8               append
+  #152 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #153 = Utf8               toString
+  #154 = Utf8               java/io/PrintStream
+  #155 = Utf8               println
+  #156 = Utf8               exit
+  #157 = Utf8               (I)V
 {
   private static int NO_TEMPERATURE;
     descriptor: I
     flags: (0x000a) ACC_PRIVATE, ACC_STATIC
 
   public CsvReader();
     descriptor: ()V
@@ -415,15 +420,15 @@
           locals = [ class java/lang/String, class EpochWriter, int, class java/util/List, class java/time/format/DateTimeFormatter, class java/lang/Boolean, class java/io/BufferedReader ]
           stack = []
         frame_type = 255 /* full_frame */
           offset_delta = 2
           locals = [ class java/lang/String, class EpochWriter, int, class java/util/List, class java/time/format/DateTimeFormatter, class java/lang/Boolean ]
           stack = [ class java/lang/Exception ]
         frame_type = 52 /* same */
-    Signature: #62                          // (Ljava/lang/String;LEpochWriter;ILjava/util/List<Ljava/lang/Integer;>;Ljava/time/format/DateTimeFormatter;Ljava/lang/Boolean;)V
+    Signature: #64                          // (Ljava/lang/String;LEpochWriter;ILjava/util/List<Ljava/lang/Integer;>;Ljava/time/format/DateTimeFormatter;Ljava/lang/Boolean;)V
 
   static {};
     descriptor: ()V
     flags: (0x0008) ACC_STATIC
     Code:
       stack=1, locals=0, args_size=0
          0: bipush        -99
```

### Comparing `accelerometer-6.2.3/accelerometer/java/CsvReader.java` & `accelerometer-7.0.0.dev0/src/accelerometer/java/CsvReader.java`

 * *Files identical despite different names*

### Comparing `accelerometer-6.2.3/accelerometer/java/DeviceReader.class` & `accelerometer-7.0.0.dev0/src/accelerometer/java/DeviceReader.class`

 * *Files 9% similar despite different names*

#### javap -verbose -constants -s -l -private {}

```diff
@@ -1,97 +1,97 @@
-  SHA-256 checksum a44ff2c1bf47b14ef1a28c363bd2b44cb66d993dc702300f65c1a50080140b0d
+  SHA-256 checksum 6f5c769a331f8b378c08a9033d7cb14711be991a18fdf4404af6d2f0b4a56f58
   Compiled from "DeviceReader.java"
 public class DeviceReader
   minor version: 0
   major version: 52
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #84                         // DeviceReader
   super_class: #85                        // java/lang/Object
   interfaces: 0, fields: 5, methods: 12, attributes: 1
 Constant pool:
-    #1 = Methodref          #85.#128      // java/lang/Object."<init>":()V
-    #2 = String             #129          // .gz
-    #3 = Methodref          #103.#130     // java/lang/String.endsWith:(Ljava/lang/String;)Z
-    #4 = Class              #131          // java/util/zip/GZIPOutputStream
-    #5 = Class              #132          // java/io/FileOutputStream
-    #6 = Class              #133          // java/io/File
-    #7 = Methodref          #6.#134       // java/io/File."<init>":(Ljava/lang/String;)V
-    #8 = Methodref          #5.#135       // java/io/FileOutputStream."<init>":(Ljava/io/File;)V
-    #9 = Methodref          #4.#136       // java/util/zip/GZIPOutputStream."<init>":(Ljava/io/OutputStream;)V
-   #10 = Class              #137          // java/io/BufferedWriter
-   #11 = Class              #138          // java/io/OutputStreamWriter
-   #12 = String             #139          // UTF-8
-   #13 = Methodref          #11.#140      // java/io/OutputStreamWriter."<init>":(Ljava/io/OutputStream;Ljava/lang/String;)V
-   #14 = Methodref          #10.#141      // java/io/BufferedWriter."<init>":(Ljava/io/Writer;)V
-   #15 = Class              #142          // java/io/FileWriter
-   #16 = Methodref          #15.#134      // java/io/FileWriter."<init>":(Ljava/lang/String;)V
-   #17 = Class              #143          // LowpassFilter
+    #1 = Methodref          #85.#134      // java/lang/Object."<init>":()V
+    #2 = String             #135          // .gz
+    #3 = Methodref          #136.#137     // java/lang/String.endsWith:(Ljava/lang/String;)Z
+    #4 = Class              #138          // java/util/zip/GZIPOutputStream
+    #5 = Class              #139          // java/io/FileOutputStream
+    #6 = Class              #140          // java/io/File
+    #7 = Methodref          #6.#141       // java/io/File."<init>":(Ljava/lang/String;)V
+    #8 = Methodref          #5.#142       // java/io/FileOutputStream."<init>":(Ljava/io/File;)V
+    #9 = Methodref          #4.#143       // java/util/zip/GZIPOutputStream."<init>":(Ljava/io/OutputStream;)V
+   #10 = Class              #144          // java/io/BufferedWriter
+   #11 = Class              #145          // java/io/OutputStreamWriter
+   #12 = String             #146          // UTF-8
+   #13 = Methodref          #11.#147      // java/io/OutputStreamWriter."<init>":(Ljava/io/OutputStream;Ljava/lang/String;)V
+   #14 = Methodref          #10.#148      // java/io/BufferedWriter."<init>":(Ljava/io/Writer;)V
+   #15 = Class              #149          // java/io/FileWriter
+   #16 = Methodref          #15.#141      // java/io/FileWriter."<init>":(Ljava/lang/String;)V
+   #17 = Class              #150          // LowpassFilter
    #18 = Double             20.0d
-   #20 = Methodref          #144.#145     // java/lang/Boolean.valueOf:(Z)Ljava/lang/Boolean;
-   #21 = Methodref          #17.#146      // LowpassFilter."<init>":(DDLjava/lang/Boolean;)V
-   #22 = Methodref          #103.#147     // java/lang/String.trim:()Ljava/lang/String;
-   #23 = Methodref          #103.#148     // java/lang/String.length:()I
-   #24 = Class              #149          // java/lang/StringBuilder
-   #25 = Methodref          #24.#128      // java/lang/StringBuilder."<init>":()V
-   #26 = Methodref          #103.#150     // java/lang/String.toLowerCase:()Ljava/lang/String;
-   #27 = String             #151          // .csv.gz
-   #28 = Methodref          #103.#152     // java/lang/String.substring:(II)Ljava/lang/String;
-   #29 = Methodref          #24.#153      // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-   #30 = String             #154          // _raw.csv.gz
-   #31 = Methodref          #24.#155      // java/lang/StringBuilder.toString:()Ljava/lang/String;
-   #32 = String             #156          // _raw.npy
-   #33 = Class              #157          // NpyWriter
-   #34 = Methodref          #33.#134      // NpyWriter."<init>":(Ljava/lang/String;)V
-   #35 = Class              #158          // EpochWriter
-   #36 = Methodref          #35.#159      // EpochWriter."<init>":(Ljava/io/BufferedWriter;Ljava/io/BufferedWriter;LNpyWriter;Ljava/time/format/DateTimeFormatter;Ljava/lang/String;IILjava/lang/String;I[D[D[DLjava/lang/Boolean;DLFilter;JJZ)V
-   #37 = Class              #160          // java/io/IOException
-   #38 = Fieldref           #161.#162     // java/lang/System.err:Ljava/io/PrintStream;
-   #39 = Methodref          #37.#163      // java/io/IOException.printStackTrace:(Ljava/io/PrintStream;)V
-   #40 = String             #164          // error closing file writer:
-   #41 = Methodref          #37.#155      // java/io/IOException.toString:()Ljava/lang/String;
-   #42 = Methodref          #165.#166     // java/io/PrintStream.println:(Ljava/lang/String;)V
-   #43 = Methodref          #161.#167     // java/lang/System.exit:(I)V
+   #20 = Methodref          #151.#152     // java/lang/Boolean.valueOf:(Z)Ljava/lang/Boolean;
+   #21 = Methodref          #17.#153      // LowpassFilter."<init>":(DDLjava/lang/Boolean;)V
+   #22 = Methodref          #136.#154     // java/lang/String.trim:()Ljava/lang/String;
+   #23 = Methodref          #136.#155     // java/lang/String.length:()I
+   #24 = Class              #156          // java/lang/StringBuilder
+   #25 = Methodref          #24.#134      // java/lang/StringBuilder."<init>":()V
+   #26 = Methodref          #136.#157     // java/lang/String.toLowerCase:()Ljava/lang/String;
+   #27 = String             #158          // .csv.gz
+   #28 = Methodref          #136.#159     // java/lang/String.substring:(II)Ljava/lang/String;
+   #29 = Methodref          #24.#160      // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+   #30 = String             #161          // _raw.csv.gz
+   #31 = Methodref          #24.#162      // java/lang/StringBuilder.toString:()Ljava/lang/String;
+   #32 = String             #163          // _raw.npy
+   #33 = Class              #164          // NpyWriter
+   #34 = Methodref          #33.#141      // NpyWriter."<init>":(Ljava/lang/String;)V
+   #35 = Class              #165          // EpochWriter
+   #36 = Methodref          #35.#166      // EpochWriter."<init>":(Ljava/io/BufferedWriter;Ljava/io/BufferedWriter;LNpyWriter;Ljava/time/format/DateTimeFormatter;Ljava/lang/String;IILjava/lang/String;I[D[D[DLjava/lang/Boolean;DLFilter;JJZ)V
+   #37 = Class              #167          // java/io/IOException
+   #38 = Fieldref           #168.#169     // java/lang/System.err:Ljava/io/PrintStream;
+   #39 = Methodref          #37.#170      // java/io/IOException.printStackTrace:(Ljava/io/PrintStream;)V
+   #40 = String             #171          // error closing file writer:
+   #41 = Methodref          #37.#162      // java/io/IOException.toString:()Ljava/lang/String;
+   #42 = Methodref          #172.#173     // java/io/PrintStream.println:(Ljava/lang/String;)V
+   #43 = Methodref          #168.#174     // java/lang/System.exit:(I)V
    #44 = Long               500000l
-   #46 = Class              #168          // java/io/RandomAccessFile
-   #47 = String             #169          // r
-   #48 = Methodref          #46.#170      // java/io/RandomAccessFile."<init>":(Ljava/lang/String;Ljava/lang/String;)V
-   #49 = Methodref          #46.#171      // java/io/RandomAccessFile.length:()J
-   #50 = Class              #172          // java/lang/Integer
+   #46 = Class              #175          // java/io/RandomAccessFile
+   #47 = String             #176          // r
+   #48 = Methodref          #46.#177      // java/io/RandomAccessFile."<init>":(Ljava/lang/String;Ljava/lang/String;)V
+   #49 = Methodref          #46.#178      // java/io/RandomAccessFile.length:()J
+   #50 = Class              #179          // java/lang/Integer
    #51 = Long               4l
-   #53 = Methodref          #46.#173      // java/io/RandomAccessFile.seek:(J)V
-   #54 = Methodref          #46.#174      // java/io/RandomAccessFile.readInt:()I
-   #55 = Methodref          #50.#175      // java/lang/Integer.reverseBytes:(I)I
-   #56 = Methodref          #50.#176      // java/lang/Integer.toUnsignedLong:(I)J
-   #57 = String             #177          // error reading gz size of file
-   #58 = String             #178          // :
-   #59 = Fieldref           #179.#180     // java/time/ZoneOffset.UTC:Ljava/time/ZoneOffset;
-   #60 = Methodref          #181.#182     // java/time/LocalDateTime.toInstant:(Ljava/time/ZoneOffset;)Ljava/time/Instant;
-   #61 = Methodref          #183.#184     // java/time/Instant.toEpochMilli:()J
-   #62 = Fieldref           #185.#186     // java/util/concurrent/TimeUnit.SECONDS:Ljava/util/concurrent/TimeUnit;
-   #63 = Methodref          #185.#187     // java/util/concurrent/TimeUnit.toNanos:(J)J
-   #64 = Methodref          #188.#189     // java/nio/ByteBuffer.getInt:(I)I
+   #53 = Methodref          #46.#180      // java/io/RandomAccessFile.seek:(J)V
+   #54 = Methodref          #46.#181      // java/io/RandomAccessFile.readInt:()I
+   #55 = Methodref          #50.#182      // java/lang/Integer.reverseBytes:(I)I
+   #56 = Methodref          #50.#183      // java/lang/Integer.toUnsignedLong:(I)J
+   #57 = String             #184          // error reading gz size of file
+   #58 = String             #185          // :
+   #59 = Fieldref           #186.#187     // java/time/ZoneOffset.UTC:Ljava/time/ZoneOffset;
+   #60 = Methodref          #188.#189     // java/time/LocalDateTime.toInstant:(Ljava/time/ZoneOffset;)Ljava/time/Instant;
+   #61 = Methodref          #190.#191     // java/time/Instant.toEpochMilli:()J
+   #62 = Fieldref           #192.#193     // java/util/concurrent/TimeUnit.SECONDS:Ljava/util/concurrent/TimeUnit;
+   #63 = Methodref          #192.#194     // java/util/concurrent/TimeUnit.toNanos:(J)J
+   #64 = Methodref          #195.#196     // java/nio/ByteBuffer.getInt:(I)I
    #65 = Long               4294967295l
-   #67 = Methodref          #188.#190     // java/nio/ByteBuffer.getShort:(I)S
+   #67 = Methodref          #195.#197     // java/nio/ByteBuffer.getShort:(I)S
    #68 = Integer            65535
-   #69 = Methodref          #50.#191      // java/lang/Integer.parseInt:(Ljava/lang/String;I)I
-   #70 = Methodref          #192.#193     // java/time/ZoneId.of:(Ljava/lang/String;)Ljava/time/ZoneId;
-   #71 = Fieldref           #84.#194      // DeviceReader.zoneId:Ljava/time/ZoneId;
-   #72 = Methodref          #192.#195     // java/time/ZoneId.getRules:()Ljava/time/zone/ZoneRules;
-   #73 = Fieldref           #84.#196      // DeviceReader.rules:Ljava/time/zone/ZoneRules;
-   #74 = Fieldref           #84.#197      // DeviceReader.timeShift:I
-   #75 = Methodref          #181.#198     // java/time/LocalDateTime.atZone:(Ljava/time/ZoneId;)Ljava/time/ZonedDateTime;
-   #76 = Fieldref           #84.#199      // DeviceReader.sessionStart:Ljava/time/ZonedDateTime;
-   #77 = Methodref          #124.#200     // java/time/ZonedDateTime.toInstant:()Ljava/time/Instant;
-   #78 = Methodref          #201.#202     // java/time/zone/ZoneRules.isDaylightSavings:(Ljava/time/Instant;)Z
-   #79 = Fieldref           #84.#203      // DeviceReader.sessionStartDST:Z
-   #80 = Methodref          #181.#204     // java/time/LocalDateTime.plusHours:(J)Ljava/time/LocalDateTime;
+   #69 = Methodref          #50.#198      // java/lang/Integer.parseInt:(Ljava/lang/String;I)I
+   #70 = Methodref          #199.#200     // java/time/ZoneId.of:(Ljava/lang/String;)Ljava/time/ZoneId;
+   #71 = Fieldref           #84.#201      // DeviceReader.zoneId:Ljava/time/ZoneId;
+   #72 = Methodref          #199.#202     // java/time/ZoneId.getRules:()Ljava/time/zone/ZoneRules;
+   #73 = Fieldref           #84.#203      // DeviceReader.rules:Ljava/time/zone/ZoneRules;
+   #74 = Fieldref           #84.#204      // DeviceReader.timeShift:I
+   #75 = Methodref          #188.#205     // java/time/LocalDateTime.atZone:(Ljava/time/ZoneId;)Ljava/time/ZonedDateTime;
+   #76 = Fieldref           #84.#206      // DeviceReader.sessionStart:Ljava/time/ZonedDateTime;
+   #77 = Methodref          #207.#208     // java/time/ZonedDateTime.toInstant:()Ljava/time/Instant;
+   #78 = Methodref          #209.#210     // java/time/zone/ZoneRules.isDaylightSavings:(Ljava/time/Instant;)Z
+   #79 = Fieldref           #84.#211      // DeviceReader.sessionStartDST:Z
+   #80 = Methodref          #188.#212     // java/time/LocalDateTime.plusHours:(J)Ljava/time/LocalDateTime;
    #81 = Long               -1l
-   #83 = Methodref          #124.#205     // java/time/ZonedDateTime.plusHours:(J)Ljava/time/ZonedDateTime;
-   #84 = Class              #206          // DeviceReader
-   #85 = Class              #207          // java/lang/Object
+   #83 = Methodref          #207.#213     // java/time/ZonedDateTime.plusHours:(J)Ljava/time/ZonedDateTime;
+   #84 = Class              #214          // DeviceReader
+   #85 = Class              #215          // java/lang/Object
    #86 = Utf8               sessionStart
    #87 = Utf8               Ljava/time/ZonedDateTime;
    #88 = Utf8               sessionStartDST
    #89 = Utf8               Z
    #90 = Utf8               zoneId
    #91 = Utf8               Ljava/time/ZoneId;
    #92 = Utf8               rules
@@ -101,196 +101,204 @@
    #96 = Utf8               <init>
    #97 = Utf8               ()V
    #98 = Utf8               Code
    #99 = Utf8               LineNumberTable
   #100 = Utf8               setupEpochWriter
   #101 = Utf8               (Ljava/lang/String;ZZLjava/lang/String;ZLjava/lang/String;ZLjava/time/format/DateTimeFormatter;Ljava/lang/String;IILjava/lang/String;I[D[D[DZDJJZ)LEpochWriter;
   #102 = Utf8               StackMapTable
-  #103 = Class              #208          // java/lang/String
-  #104 = Class              #209          // java/time/format/DateTimeFormatter
-  #105 = Class              #210          // "[D"
-  #106 = Utf8               getUncompressedSizeofGzipFile
-  #107 = Utf8               (Ljava/lang/String;)J
-  #108 = Utf8               getEpochMillis
-  #109 = Utf8               (Ljava/time/LocalDateTime;)J
-  #110 = Utf8               secs2Nanos
-  #111 = Utf8               (D)J
-  #112 = Utf8               getUnsignedInt
-  #113 = Utf8               (Ljava/nio/ByteBuffer;I)J
-  #114 = Utf8               getUnsignedShort
-  #115 = Utf8               (Ljava/nio/ByteBuffer;I)I
-  #116 = Utf8               getSignedIntFromHex
-  #117 = Utf8               (Ljava/lang/String;II)I
-  #118 = Utf8               setTimeSettings
-  #119 = Utf8               (Ljava/lang/String;I)V
-  #120 = Utf8               setSessionStart
-  #121 = Utf8               (Ljava/time/LocalDateTime;)V
-  #122 = Utf8               zonedWithDSTCorrection
-  #123 = Utf8               (Ljava/time/LocalDateTime;)Ljava/time/ZonedDateTime;
-  #124 = Class              #211          // java/time/ZonedDateTime
-  #125 = Utf8               <clinit>
-  #126 = Utf8               SourceFile
-  #127 = Utf8               DeviceReader.java
-  #128 = NameAndType        #96:#97       // "<init>":()V
-  #129 = Utf8               .gz
-  #130 = NameAndType        #212:#213     // endsWith:(Ljava/lang/String;)Z
-  #131 = Utf8               java/util/zip/GZIPOutputStream
-  #132 = Utf8               java/io/FileOutputStream
-  #133 = Utf8               java/io/File
-  #134 = NameAndType        #96:#214      // "<init>":(Ljava/lang/String;)V
-  #135 = NameAndType        #96:#215      // "<init>":(Ljava/io/File;)V
-  #136 = NameAndType        #96:#216      // "<init>":(Ljava/io/OutputStream;)V
-  #137 = Utf8               java/io/BufferedWriter
-  #138 = Utf8               java/io/OutputStreamWriter
-  #139 = Utf8               UTF-8
-  #140 = NameAndType        #96:#217      // "<init>":(Ljava/io/OutputStream;Ljava/lang/String;)V
-  #141 = NameAndType        #96:#218      // "<init>":(Ljava/io/Writer;)V
-  #142 = Utf8               java/io/FileWriter
-  #143 = Utf8               LowpassFilter
-  #144 = Class              #219          // java/lang/Boolean
-  #145 = NameAndType        #220:#221     // valueOf:(Z)Ljava/lang/Boolean;
-  #146 = NameAndType        #96:#222      // "<init>":(DDLjava/lang/Boolean;)V
-  #147 = NameAndType        #223:#224     // trim:()Ljava/lang/String;
-  #148 = NameAndType        #225:#226     // length:()I
-  #149 = Utf8               java/lang/StringBuilder
-  #150 = NameAndType        #227:#224     // toLowerCase:()Ljava/lang/String;
-  #151 = Utf8               .csv.gz
-  #152 = NameAndType        #228:#229     // substring:(II)Ljava/lang/String;
-  #153 = NameAndType        #230:#231     // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #154 = Utf8               _raw.csv.gz
-  #155 = NameAndType        #232:#224     // toString:()Ljava/lang/String;
-  #156 = Utf8               _raw.npy
-  #157 = Utf8               NpyWriter
-  #158 = Utf8               EpochWriter
-  #159 = NameAndType        #96:#233      // "<init>":(Ljava/io/BufferedWriter;Ljava/io/BufferedWriter;LNpyWriter;Ljava/time/format/DateTimeFormatter;Ljava/lang/String;IILjava/lang/String;I[D[D[DLjava/lang/Boolean;DLFilter;JJZ)V
-  #160 = Utf8               java/io/IOException
-  #161 = Class              #234          // java/lang/System
-  #162 = NameAndType        #235:#236     // err:Ljava/io/PrintStream;
-  #163 = NameAndType        #237:#238     // printStackTrace:(Ljava/io/PrintStream;)V
-  #164 = Utf8               error closing file writer:
-  #165 = Class              #239          // java/io/PrintStream
-  #166 = NameAndType        #240:#214     // println:(Ljava/lang/String;)V
-  #167 = NameAndType        #241:#242     // exit:(I)V
-  #168 = Utf8               java/io/RandomAccessFile
-  #169 = Utf8               r
-  #170 = NameAndType        #96:#243      // "<init>":(Ljava/lang/String;Ljava/lang/String;)V
-  #171 = NameAndType        #225:#244     // length:()J
-  #172 = Utf8               java/lang/Integer
-  #173 = NameAndType        #245:#246     // seek:(J)V
-  #174 = NameAndType        #247:#226     // readInt:()I
-  #175 = NameAndType        #248:#249     // reverseBytes:(I)I
-  #176 = NameAndType        #250:#251     // toUnsignedLong:(I)J
-  #177 = Utf8               error reading gz size of file
-  #178 = Utf8               :
-  #179 = Class              #252          // java/time/ZoneOffset
-  #180 = NameAndType        #253:#254     // UTC:Ljava/time/ZoneOffset;
-  #181 = Class              #255          // java/time/LocalDateTime
-  #182 = NameAndType        #256:#257     // toInstant:(Ljava/time/ZoneOffset;)Ljava/time/Instant;
-  #183 = Class              #258          // java/time/Instant
-  #184 = NameAndType        #259:#244     // toEpochMilli:()J
-  #185 = Class              #260          // java/util/concurrent/TimeUnit
-  #186 = NameAndType        #261:#262     // SECONDS:Ljava/util/concurrent/TimeUnit;
-  #187 = NameAndType        #263:#264     // toNanos:(J)J
-  #188 = Class              #265          // java/nio/ByteBuffer
-  #189 = NameAndType        #266:#249     // getInt:(I)I
-  #190 = NameAndType        #267:#268     // getShort:(I)S
-  #191 = NameAndType        #269:#270     // parseInt:(Ljava/lang/String;I)I
-  #192 = Class              #271          // java/time/ZoneId
-  #193 = NameAndType        #272:#273     // of:(Ljava/lang/String;)Ljava/time/ZoneId;
-  #194 = NameAndType        #90:#91       // zoneId:Ljava/time/ZoneId;
-  #195 = NameAndType        #274:#275     // getRules:()Ljava/time/zone/ZoneRules;
-  #196 = NameAndType        #92:#93       // rules:Ljava/time/zone/ZoneRules;
-  #197 = NameAndType        #94:#95       // timeShift:I
-  #198 = NameAndType        #276:#277     // atZone:(Ljava/time/ZoneId;)Ljava/time/ZonedDateTime;
-  #199 = NameAndType        #86:#87       // sessionStart:Ljava/time/ZonedDateTime;
-  #200 = NameAndType        #256:#278     // toInstant:()Ljava/time/Instant;
-  #201 = Class              #279          // java/time/zone/ZoneRules
-  #202 = NameAndType        #280:#281     // isDaylightSavings:(Ljava/time/Instant;)Z
-  #203 = NameAndType        #88:#89       // sessionStartDST:Z
-  #204 = NameAndType        #282:#283     // plusHours:(J)Ljava/time/LocalDateTime;
-  #205 = NameAndType        #282:#284     // plusHours:(J)Ljava/time/ZonedDateTime;
-  #206 = Utf8               DeviceReader
-  #207 = Utf8               java/lang/Object
-  #208 = Utf8               java/lang/String
-  #209 = Utf8               java/time/format/DateTimeFormatter
-  #210 = Utf8               [D
-  #211 = Utf8               java/time/ZonedDateTime
-  #212 = Utf8               endsWith
-  #213 = Utf8               (Ljava/lang/String;)Z
-  #214 = Utf8               (Ljava/lang/String;)V
-  #215 = Utf8               (Ljava/io/File;)V
-  #216 = Utf8               (Ljava/io/OutputStream;)V
-  #217 = Utf8               (Ljava/io/OutputStream;Ljava/lang/String;)V
-  #218 = Utf8               (Ljava/io/Writer;)V
-  #219 = Utf8               java/lang/Boolean
-  #220 = Utf8               valueOf
-  #221 = Utf8               (Z)Ljava/lang/Boolean;
-  #222 = Utf8               (DDLjava/lang/Boolean;)V
-  #223 = Utf8               trim
-  #224 = Utf8               ()Ljava/lang/String;
-  #225 = Utf8               length
-  #226 = Utf8               ()I
-  #227 = Utf8               toLowerCase
-  #228 = Utf8               substring
-  #229 = Utf8               (II)Ljava/lang/String;
-  #230 = Utf8               append
-  #231 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #232 = Utf8               toString
-  #233 = Utf8               (Ljava/io/BufferedWriter;Ljava/io/BufferedWriter;LNpyWriter;Ljava/time/format/DateTimeFormatter;Ljava/lang/String;IILjava/lang/String;I[D[D[DLjava/lang/Boolean;DLFilter;JJZ)V
-  #234 = Utf8               java/lang/System
-  #235 = Utf8               err
-  #236 = Utf8               Ljava/io/PrintStream;
-  #237 = Utf8               printStackTrace
-  #238 = Utf8               (Ljava/io/PrintStream;)V
-  #239 = Utf8               java/io/PrintStream
-  #240 = Utf8               println
-  #241 = Utf8               exit
-  #242 = Utf8               (I)V
-  #243 = Utf8               (Ljava/lang/String;Ljava/lang/String;)V
-  #244 = Utf8               ()J
-  #245 = Utf8               seek
-  #246 = Utf8               (J)V
-  #247 = Utf8               readInt
-  #248 = Utf8               reverseBytes
-  #249 = Utf8               (I)I
-  #250 = Utf8               toUnsignedLong
-  #251 = Utf8               (I)J
-  #252 = Utf8               java/time/ZoneOffset
-  #253 = Utf8               UTC
-  #254 = Utf8               Ljava/time/ZoneOffset;
-  #255 = Utf8               java/time/LocalDateTime
-  #256 = Utf8               toInstant
-  #257 = Utf8               (Ljava/time/ZoneOffset;)Ljava/time/Instant;
-  #258 = Utf8               java/time/Instant
-  #259 = Utf8               toEpochMilli
-  #260 = Utf8               java/util/concurrent/TimeUnit
-  #261 = Utf8               SECONDS
-  #262 = Utf8               Ljava/util/concurrent/TimeUnit;
-  #263 = Utf8               toNanos
-  #264 = Utf8               (J)J
-  #265 = Utf8               java/nio/ByteBuffer
-  #266 = Utf8               getInt
-  #267 = Utf8               getShort
-  #268 = Utf8               (I)S
-  #269 = Utf8               parseInt
-  #270 = Utf8               (Ljava/lang/String;I)I
-  #271 = Utf8               java/time/ZoneId
-  #272 = Utf8               of
-  #273 = Utf8               (Ljava/lang/String;)Ljava/time/ZoneId;
-  #274 = Utf8               getRules
-  #275 = Utf8               ()Ljava/time/zone/ZoneRules;
-  #276 = Utf8               atZone
-  #277 = Utf8               (Ljava/time/ZoneId;)Ljava/time/ZonedDateTime;
-  #278 = Utf8               ()Ljava/time/Instant;
-  #279 = Utf8               java/time/zone/ZoneRules
-  #280 = Utf8               isDaylightSavings
-  #281 = Utf8               (Ljava/time/Instant;)Z
-  #282 = Utf8               plusHours
-  #283 = Utf8               (J)Ljava/time/LocalDateTime;
-  #284 = Utf8               (J)Ljava/time/ZonedDateTime;
+  #103 = Class              #216          // java/lang/String
+  #104 = Class              #217          // java/time/format/DateTimeFormatter
+  #105 = Class              #218          // "[D"
+  #106 = Class              #165          // EpochWriter
+  #107 = Class              #144          // java/io/BufferedWriter
+  #108 = Class              #164          // NpyWriter
+  #109 = Class              #150          // LowpassFilter
+  #110 = Class              #156          // java/lang/StringBuilder
+  #111 = Class              #167          // java/io/IOException
+  #112 = Utf8               getUncompressedSizeofGzipFile
+  #113 = Utf8               (Ljava/lang/String;)J
+  #114 = Utf8               getEpochMillis
+  #115 = Utf8               (Ljava/time/LocalDateTime;)J
+  #116 = Utf8               secs2Nanos
+  #117 = Utf8               (D)J
+  #118 = Utf8               getUnsignedInt
+  #119 = Utf8               (Ljava/nio/ByteBuffer;I)J
+  #120 = Utf8               getUnsignedShort
+  #121 = Utf8               (Ljava/nio/ByteBuffer;I)I
+  #122 = Utf8               getSignedIntFromHex
+  #123 = Utf8               (Ljava/lang/String;II)I
+  #124 = Utf8               setTimeSettings
+  #125 = Utf8               (Ljava/lang/String;I)V
+  #126 = Utf8               setSessionStart
+  #127 = Utf8               (Ljava/time/LocalDateTime;)V
+  #128 = Utf8               zonedWithDSTCorrection
+  #129 = Utf8               (Ljava/time/LocalDateTime;)Ljava/time/ZonedDateTime;
+  #130 = Class              #219          // java/time/ZonedDateTime
+  #131 = Utf8               <clinit>
+  #132 = Utf8               SourceFile
+  #133 = Utf8               DeviceReader.java
+  #134 = NameAndType        #96:#97       // "<init>":()V
+  #135 = Utf8               .gz
+  #136 = Class              #216          // java/lang/String
+  #137 = NameAndType        #220:#221     // endsWith:(Ljava/lang/String;)Z
+  #138 = Utf8               java/util/zip/GZIPOutputStream
+  #139 = Utf8               java/io/FileOutputStream
+  #140 = Utf8               java/io/File
+  #141 = NameAndType        #96:#222      // "<init>":(Ljava/lang/String;)V
+  #142 = NameAndType        #96:#223      // "<init>":(Ljava/io/File;)V
+  #143 = NameAndType        #96:#224      // "<init>":(Ljava/io/OutputStream;)V
+  #144 = Utf8               java/io/BufferedWriter
+  #145 = Utf8               java/io/OutputStreamWriter
+  #146 = Utf8               UTF-8
+  #147 = NameAndType        #96:#225      // "<init>":(Ljava/io/OutputStream;Ljava/lang/String;)V
+  #148 = NameAndType        #96:#226      // "<init>":(Ljava/io/Writer;)V
+  #149 = Utf8               java/io/FileWriter
+  #150 = Utf8               LowpassFilter
+  #151 = Class              #227          // java/lang/Boolean
+  #152 = NameAndType        #228:#229     // valueOf:(Z)Ljava/lang/Boolean;
+  #153 = NameAndType        #96:#230      // "<init>":(DDLjava/lang/Boolean;)V
+  #154 = NameAndType        #231:#232     // trim:()Ljava/lang/String;
+  #155 = NameAndType        #233:#234     // length:()I
+  #156 = Utf8               java/lang/StringBuilder
+  #157 = NameAndType        #235:#232     // toLowerCase:()Ljava/lang/String;
+  #158 = Utf8               .csv.gz
+  #159 = NameAndType        #236:#237     // substring:(II)Ljava/lang/String;
+  #160 = NameAndType        #238:#239     // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #161 = Utf8               _raw.csv.gz
+  #162 = NameAndType        #240:#232     // toString:()Ljava/lang/String;
+  #163 = Utf8               _raw.npy
+  #164 = Utf8               NpyWriter
+  #165 = Utf8               EpochWriter
+  #166 = NameAndType        #96:#241      // "<init>":(Ljava/io/BufferedWriter;Ljava/io/BufferedWriter;LNpyWriter;Ljava/time/format/DateTimeFormatter;Ljava/lang/String;IILjava/lang/String;I[D[D[DLjava/lang/Boolean;DLFilter;JJZ)V
+  #167 = Utf8               java/io/IOException
+  #168 = Class              #242          // java/lang/System
+  #169 = NameAndType        #243:#244     // err:Ljava/io/PrintStream;
+  #170 = NameAndType        #245:#246     // printStackTrace:(Ljava/io/PrintStream;)V
+  #171 = Utf8               error closing file writer:
+  #172 = Class              #247          // java/io/PrintStream
+  #173 = NameAndType        #248:#222     // println:(Ljava/lang/String;)V
+  #174 = NameAndType        #249:#250     // exit:(I)V
+  #175 = Utf8               java/io/RandomAccessFile
+  #176 = Utf8               r
+  #177 = NameAndType        #96:#251      // "<init>":(Ljava/lang/String;Ljava/lang/String;)V
+  #178 = NameAndType        #233:#252     // length:()J
+  #179 = Utf8               java/lang/Integer
+  #180 = NameAndType        #253:#254     // seek:(J)V
+  #181 = NameAndType        #255:#234     // readInt:()I
+  #182 = NameAndType        #256:#257     // reverseBytes:(I)I
+  #183 = NameAndType        #258:#259     // toUnsignedLong:(I)J
+  #184 = Utf8               error reading gz size of file
+  #185 = Utf8               :
+  #186 = Class              #260          // java/time/ZoneOffset
+  #187 = NameAndType        #261:#262     // UTC:Ljava/time/ZoneOffset;
+  #188 = Class              #263          // java/time/LocalDateTime
+  #189 = NameAndType        #264:#265     // toInstant:(Ljava/time/ZoneOffset;)Ljava/time/Instant;
+  #190 = Class              #266          // java/time/Instant
+  #191 = NameAndType        #267:#252     // toEpochMilli:()J
+  #192 = Class              #268          // java/util/concurrent/TimeUnit
+  #193 = NameAndType        #269:#270     // SECONDS:Ljava/util/concurrent/TimeUnit;
+  #194 = NameAndType        #271:#272     // toNanos:(J)J
+  #195 = Class              #273          // java/nio/ByteBuffer
+  #196 = NameAndType        #274:#257     // getInt:(I)I
+  #197 = NameAndType        #275:#276     // getShort:(I)S
+  #198 = NameAndType        #277:#278     // parseInt:(Ljava/lang/String;I)I
+  #199 = Class              #279          // java/time/ZoneId
+  #200 = NameAndType        #280:#281     // of:(Ljava/lang/String;)Ljava/time/ZoneId;
+  #201 = NameAndType        #90:#91       // zoneId:Ljava/time/ZoneId;
+  #202 = NameAndType        #282:#283     // getRules:()Ljava/time/zone/ZoneRules;
+  #203 = NameAndType        #92:#93       // rules:Ljava/time/zone/ZoneRules;
+  #204 = NameAndType        #94:#95       // timeShift:I
+  #205 = NameAndType        #284:#285     // atZone:(Ljava/time/ZoneId;)Ljava/time/ZonedDateTime;
+  #206 = NameAndType        #86:#87       // sessionStart:Ljava/time/ZonedDateTime;
+  #207 = Class              #219          // java/time/ZonedDateTime
+  #208 = NameAndType        #264:#286     // toInstant:()Ljava/time/Instant;
+  #209 = Class              #287          // java/time/zone/ZoneRules
+  #210 = NameAndType        #288:#289     // isDaylightSavings:(Ljava/time/Instant;)Z
+  #211 = NameAndType        #88:#89       // sessionStartDST:Z
+  #212 = NameAndType        #290:#291     // plusHours:(J)Ljava/time/LocalDateTime;
+  #213 = NameAndType        #290:#292     // plusHours:(J)Ljava/time/ZonedDateTime;
+  #214 = Utf8               DeviceReader
+  #215 = Utf8               java/lang/Object
+  #216 = Utf8               java/lang/String
+  #217 = Utf8               java/time/format/DateTimeFormatter
+  #218 = Utf8               [D
+  #219 = Utf8               java/time/ZonedDateTime
+  #220 = Utf8               endsWith
+  #221 = Utf8               (Ljava/lang/String;)Z
+  #222 = Utf8               (Ljava/lang/String;)V
+  #223 = Utf8               (Ljava/io/File;)V
+  #224 = Utf8               (Ljava/io/OutputStream;)V
+  #225 = Utf8               (Ljava/io/OutputStream;Ljava/lang/String;)V
+  #226 = Utf8               (Ljava/io/Writer;)V
+  #227 = Utf8               java/lang/Boolean
+  #228 = Utf8               valueOf
+  #229 = Utf8               (Z)Ljava/lang/Boolean;
+  #230 = Utf8               (DDLjava/lang/Boolean;)V
+  #231 = Utf8               trim
+  #232 = Utf8               ()Ljava/lang/String;
+  #233 = Utf8               length
+  #234 = Utf8               ()I
+  #235 = Utf8               toLowerCase
+  #236 = Utf8               substring
+  #237 = Utf8               (II)Ljava/lang/String;
+  #238 = Utf8               append
+  #239 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #240 = Utf8               toString
+  #241 = Utf8               (Ljava/io/BufferedWriter;Ljava/io/BufferedWriter;LNpyWriter;Ljava/time/format/DateTimeFormatter;Ljava/lang/String;IILjava/lang/String;I[D[D[DLjava/lang/Boolean;DLFilter;JJZ)V
+  #242 = Utf8               java/lang/System
+  #243 = Utf8               err
+  #244 = Utf8               Ljava/io/PrintStream;
+  #245 = Utf8               printStackTrace
+  #246 = Utf8               (Ljava/io/PrintStream;)V
+  #247 = Utf8               java/io/PrintStream
+  #248 = Utf8               println
+  #249 = Utf8               exit
+  #250 = Utf8               (I)V
+  #251 = Utf8               (Ljava/lang/String;Ljava/lang/String;)V
+  #252 = Utf8               ()J
+  #253 = Utf8               seek
+  #254 = Utf8               (J)V
+  #255 = Utf8               readInt
+  #256 = Utf8               reverseBytes
+  #257 = Utf8               (I)I
+  #258 = Utf8               toUnsignedLong
+  #259 = Utf8               (I)J
+  #260 = Utf8               java/time/ZoneOffset
+  #261 = Utf8               UTC
+  #262 = Utf8               Ljava/time/ZoneOffset;
+  #263 = Utf8               java/time/LocalDateTime
+  #264 = Utf8               toInstant
+  #265 = Utf8               (Ljava/time/ZoneOffset;)Ljava/time/Instant;
+  #266 = Utf8               java/time/Instant
+  #267 = Utf8               toEpochMilli
+  #268 = Utf8               java/util/concurrent/TimeUnit
+  #269 = Utf8               SECONDS
+  #270 = Utf8               Ljava/util/concurrent/TimeUnit;
+  #271 = Utf8               toNanos
+  #272 = Utf8               (J)J
+  #273 = Utf8               java/nio/ByteBuffer
+  #274 = Utf8               getInt
+  #275 = Utf8               getShort
+  #276 = Utf8               (I)S
+  #277 = Utf8               parseInt
+  #278 = Utf8               (Ljava/lang/String;I)I
+  #279 = Utf8               java/time/ZoneId
+  #280 = Utf8               of
+  #281 = Utf8               (Ljava/lang/String;)Ljava/time/ZoneId;
+  #282 = Utf8               getRules
+  #283 = Utf8               ()Ljava/time/zone/ZoneRules;
+  #284 = Utf8               atZone
+  #285 = Utf8               (Ljava/time/ZoneId;)Ljava/time/ZonedDateTime;
+  #286 = Utf8               ()Ljava/time/Instant;
+  #287 = Utf8               java/time/zone/ZoneRules
+  #288 = Utf8               isDaylightSavings
+  #289 = Utf8               (Ljava/time/Instant;)Z
+  #290 = Utf8               plusHours
+  #291 = Utf8               (J)Ljava/time/LocalDateTime;
+  #292 = Utf8               (J)Ljava/time/ZonedDateTime;
 {
   protected static java.time.ZonedDateTime sessionStart;
     descriptor: Ljava/time/ZonedDateTime;
     flags: (0x000c) ACC_PROTECTED, ACC_STATIC
 
   protected static boolean sessionStartDST;
     descriptor: Z
@@ -519,21 +527,21 @@
         line 71: 68
         line 73: 85
         line 74: 88
         line 75: 92
         line 77: 112
         line 78: 116
         line 79: 126
-        line 80: 145
+        line 80: 148
         line 82: 176
         line 84: 200
         line 86: 220
         line 87: 225
         line 88: 236
-        line 89: 255
+        line 89: 258
         line 91: 287
         line 93: 298
         line 106: 328
         line 116: 346
         line 112: 349
         line 113: 351
         line 114: 359
```

### Comparing `accelerometer-6.2.3/accelerometer/java/DeviceReader.java` & `accelerometer-7.0.0.dev0/src/accelerometer/java/DeviceReader.java`

 * *Files identical despite different names*

### Comparing `accelerometer-6.2.3/accelerometer/java/EpochWriter.class` & `accelerometer-7.0.0.dev0/src/accelerometer/java/EpochWriter.class`

 * *Files 13% similar despite different names*

#### javap -verbose -constants -s -l -private {}

```diff
@@ -1,169 +1,169 @@
-  SHA-256 checksum 5477d418b26b6584007f2c7b3ba0bf6f440e73b9cc3bbfc7d36f7078f8376462
+  SHA-256 checksum 07acbb90e0d5f69a1e944a0ba1d948d53b93dfd919434bb87faa1ee5c81b6c39
   Compiled from "EpochWriter.java"
 public class EpochWriter
   minor version: 0
   major version: 52
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #18                         // EpochWriter
   super_class: #155                       // java/lang/Object
   interfaces: 0, fields: 34, methods: 13, attributes: 1
 Constant pool:
-    #1 = Methodref          #155.#251     // java/lang/Object."<init>":()V
+    #1 = Methodref          #155.#255     // java/lang/Object."<init>":()V
     #2 = Long               -1l
-    #4 = Fieldref           #18.#252      // EpochWriter.UNUSED_DATE:J
-    #5 = Class              #253          // java/util/ArrayList
-    #6 = Methodref          #5.#251       // java/util/ArrayList."<init>":()V
-    #7 = Fieldref           #18.#254      // EpochWriter.timeVals:Ljava/util/List;
-    #8 = Fieldref           #18.#255      // EpochWriter.xVals:Ljava/util/List;
-    #9 = Fieldref           #18.#256      // EpochWriter.yVals:Ljava/util/List;
-   #10 = Fieldref           #18.#257      // EpochWriter.zVals:Ljava/util/List;
-   #11 = Fieldref           #18.#258      // EpochWriter.temperatureVals:Ljava/util/List;
-   #12 = Fieldref           #18.#259      // EpochWriter.minSamplesForEpoch:I
-   #13 = Fieldref           #18.#260      // EpochWriter.prevTimeVal:J
+    #4 = Fieldref           #18.#256      // EpochWriter.UNUSED_DATE:J
+    #5 = Class              #257          // java/util/ArrayList
+    #6 = Methodref          #5.#255       // java/util/ArrayList."<init>":()V
+    #7 = Fieldref           #18.#258      // EpochWriter.timeVals:Ljava/util/List;
+    #8 = Fieldref           #18.#259      // EpochWriter.xVals:Ljava/util/List;
+    #9 = Fieldref           #18.#260      // EpochWriter.yVals:Ljava/util/List;
+   #10 = Fieldref           #18.#261      // EpochWriter.zVals:Ljava/util/List;
+   #11 = Fieldref           #18.#262      // EpochWriter.temperatureVals:Ljava/util/List;
+   #12 = Fieldref           #18.#263      // EpochWriter.minSamplesForEpoch:I
+   #13 = Fieldref           #18.#264      // EpochWriter.prevTimeVal:J
    #14 = Double             -1.0d
-   #16 = Fieldref           #18.#261      // EpochWriter.prevXYZT:[D
-   #17 = Fieldref           #18.#262      // EpochWriter.edgeInterpolation:Z
-   #18 = Class              #263          // EpochWriter
-   #19 = Fieldref           #18.#264      // EpochWriter.epochStartTime:J
-   #20 = Fieldref           #18.#265      // EpochWriter.epochFileWriter:Ljava/io/BufferedWriter;
-   #21 = Fieldref           #18.#266      // EpochWriter.rawWriter:Ljava/io/BufferedWriter;
-   #22 = Fieldref           #18.#267      // EpochWriter.npyWriter:LNpyWriter;
-   #23 = Fieldref           #18.#268      // EpochWriter.timeFormat:Ljava/time/format/DateTimeFormatter;
-   #24 = Fieldref           #18.#269      // EpochWriter.epochPeriod:I
-   #25 = Fieldref           #18.#270      // EpochWriter.intendedSampleRate:I
-   #26 = Fieldref           #18.#271      // EpochWriter.resampleMethod:Ljava/lang/String;
-   #27 = Fieldref           #18.#272      // EpochWriter.range:I
-   #28 = Fieldref           #18.#273      // EpochWriter.xyzIntercept:[D
-   #29 = Fieldref           #18.#274      // EpochWriter.xyzSlope:[D
-   #30 = Fieldref           #18.#275      // EpochWriter.xyzSlopeT:[D
-   #31 = Methodref          #219.#276     // java/lang/Boolean.booleanValue:()Z
-   #32 = Fieldref           #18.#277      // EpochWriter.getStationaryBouts:Z
-   #33 = Fieldref           #18.#278      // EpochWriter.stationaryStd:D
-   #34 = Fieldref           #18.#279      // EpochWriter.filter:LFilter;
-   #35 = Fieldref           #18.#280      // EpochWriter.startTime:J
-   #36 = Fieldref           #18.#281      // EpochWriter.endTime:J
-   #37 = Fieldref           #18.#282      // EpochWriter.getFeatures:Z
-   #38 = Methodref          #283.#284     // java/time/ZoneId.of:(Ljava/lang/String;)Ljava/time/ZoneId;
-   #39 = Fieldref           #18.#285      // EpochWriter.zoneId:Ljava/time/ZoneId;
-   #40 = Fieldref           #18.#286      // EpochWriter.decimalFormatSymbol:Ljava/text/DecimalFormatSymbols;
-   #41 = String             #287          // NaN
-   #42 = Methodref          #147.#288     // java/text/DecimalFormatSymbols.setNaN:(Ljava/lang/String;)V
-   #43 = String             #289          // inf
-   #44 = Methodref          #147.#290     // java/text/DecimalFormatSymbols.setInfinity:(Ljava/lang/String;)V
-   #45 = Fieldref           #18.#291      // EpochWriter.DF6:Ljava/text/DecimalFormat;
-   #46 = Methodref          #150.#292     // java/text/DecimalFormat.setDecimalFormatSymbols:(Ljava/text/DecimalFormatSymbols;)V
-   #47 = Fieldref           #18.#293      // EpochWriter.DF3:Ljava/text/DecimalFormat;
-   #48 = Fieldref           #18.#294      // EpochWriter.DF2:Ljava/text/DecimalFormat;
-   #49 = Fieldref           #295.#296     // java/math/RoundingMode.CEILING:Ljava/math/RoundingMode;
-   #50 = Methodref          #150.#297     // java/text/DecimalFormat.setRoundingMode:(Ljava/math/RoundingMode;)V
-   #51 = Fieldref           #295.#298     // java/math/RoundingMode.HALF_UP:Ljava/math/RoundingMode;
-   #52 = String             #299          // time
-   #53 = Class              #300          // java/lang/StringBuilder
-   #54 = Methodref          #53.#251      // java/lang/StringBuilder."<init>":()V
-   #55 = Methodref          #53.#301      // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-   #56 = String             #302          // ,
-   #57 = Methodref          #219.#303     // java/lang/Boolean.valueOf:(Z)Ljava/lang/Boolean;
-   #58 = Methodref          #304.#305     // AccStats.getStatsHeader:(Ljava/lang/Boolean;)Ljava/lang/String;
-   #59 = Methodref          #53.#306      // java/lang/StringBuilder.toString:()Ljava/lang/String;
-   #60 = String             #307          // ,temp,samples
-   #61 = String             #308          // ,dataErrors,clipsBeforeCalibr,clipsAfterCalibr,rawSamples
-   #62 = Methodref          #18.#309      // EpochWriter.writeLine:(Ljava/io/BufferedWriter;Ljava/lang/String;)V
-   #63 = String             #310          // time,x,y,z
-   #64 = Fieldref           #311.#312     // java/lang/System.out:Ljava/io/PrintStream;
-   #65 = String             #313          // first epochtime set to startTime
-   #66 = String             #314          //  +
-   #67 = Methodref          #53.#315      // java/lang/StringBuilder.append:(I)Ljava/lang/StringBuilder;
-   #68 = String             #316          //  epochs
-   #69 = String             #317          //
-   #70 = String             #318          //  at
-   #71 = Methodref          #18.#319      // EpochWriter.millisToZonedDateTime:(J)Ljava/time/ZonedDateTime;
-   #72 = Methodref          #53.#320      // java/lang/StringBuilder.append:(Ljava/lang/Object;)Ljava/lang/StringBuilder;
-   #73 = Methodref          #224.#321     // java/io/PrintStream.println:(Ljava/lang/String;)V
-   #74 = Fieldref           #311.#322     // java/lang/System.err:Ljava/io/PrintStream;
-   #75 = String             #323          // Interrupt of length:
+   #16 = Fieldref           #18.#265      // EpochWriter.prevXYZT:[D
+   #17 = Fieldref           #18.#266      // EpochWriter.edgeInterpolation:Z
+   #18 = Class              #267          // EpochWriter
+   #19 = Fieldref           #18.#268      // EpochWriter.epochStartTime:J
+   #20 = Fieldref           #18.#269      // EpochWriter.epochFileWriter:Ljava/io/BufferedWriter;
+   #21 = Fieldref           #18.#270      // EpochWriter.rawWriter:Ljava/io/BufferedWriter;
+   #22 = Fieldref           #18.#271      // EpochWriter.npyWriter:LNpyWriter;
+   #23 = Fieldref           #18.#272      // EpochWriter.timeFormat:Ljava/time/format/DateTimeFormatter;
+   #24 = Fieldref           #18.#273      // EpochWriter.epochPeriod:I
+   #25 = Fieldref           #18.#274      // EpochWriter.intendedSampleRate:I
+   #26 = Fieldref           #18.#275      // EpochWriter.resampleMethod:Ljava/lang/String;
+   #27 = Fieldref           #18.#276      // EpochWriter.range:I
+   #28 = Fieldref           #18.#277      // EpochWriter.xyzIntercept:[D
+   #29 = Fieldref           #18.#278      // EpochWriter.xyzSlope:[D
+   #30 = Fieldref           #18.#279      // EpochWriter.xyzSlopeT:[D
+   #31 = Methodref          #280.#281     // java/lang/Boolean.booleanValue:()Z
+   #32 = Fieldref           #18.#282      // EpochWriter.getStationaryBouts:Z
+   #33 = Fieldref           #18.#283      // EpochWriter.stationaryStd:D
+   #34 = Fieldref           #18.#284      // EpochWriter.filter:LFilter;
+   #35 = Fieldref           #18.#285      // EpochWriter.startTime:J
+   #36 = Fieldref           #18.#286      // EpochWriter.endTime:J
+   #37 = Fieldref           #18.#287      // EpochWriter.getFeatures:Z
+   #38 = Methodref          #288.#289     // java/time/ZoneId.of:(Ljava/lang/String;)Ljava/time/ZoneId;
+   #39 = Fieldref           #18.#290      // EpochWriter.zoneId:Ljava/time/ZoneId;
+   #40 = Fieldref           #18.#291      // EpochWriter.decimalFormatSymbol:Ljava/text/DecimalFormatSymbols;
+   #41 = String             #292          // NaN
+   #42 = Methodref          #147.#293     // java/text/DecimalFormatSymbols.setNaN:(Ljava/lang/String;)V
+   #43 = String             #294          // inf
+   #44 = Methodref          #147.#295     // java/text/DecimalFormatSymbols.setInfinity:(Ljava/lang/String;)V
+   #45 = Fieldref           #18.#296      // EpochWriter.DF6:Ljava/text/DecimalFormat;
+   #46 = Methodref          #150.#297     // java/text/DecimalFormat.setDecimalFormatSymbols:(Ljava/text/DecimalFormatSymbols;)V
+   #47 = Fieldref           #18.#298      // EpochWriter.DF3:Ljava/text/DecimalFormat;
+   #48 = Fieldref           #18.#299      // EpochWriter.DF2:Ljava/text/DecimalFormat;
+   #49 = Fieldref           #300.#301     // java/math/RoundingMode.CEILING:Ljava/math/RoundingMode;
+   #50 = Methodref          #150.#302     // java/text/DecimalFormat.setRoundingMode:(Ljava/math/RoundingMode;)V
+   #51 = Fieldref           #300.#303     // java/math/RoundingMode.HALF_UP:Ljava/math/RoundingMode;
+   #52 = String             #304          // time
+   #53 = Class              #305          // java/lang/StringBuilder
+   #54 = Methodref          #53.#255      // java/lang/StringBuilder."<init>":()V
+   #55 = Methodref          #53.#306      // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+   #56 = String             #307          // ,
+   #57 = Methodref          #280.#308     // java/lang/Boolean.valueOf:(Z)Ljava/lang/Boolean;
+   #58 = Methodref          #309.#310     // AccStats.getStatsHeader:(Ljava/lang/Boolean;)Ljava/lang/String;
+   #59 = Methodref          #53.#311      // java/lang/StringBuilder.toString:()Ljava/lang/String;
+   #60 = String             #312          // ,temp,samples
+   #61 = String             #313          // ,dataErrors,clipsBeforeCalibr,clipsAfterCalibr,rawSamples
+   #62 = Methodref          #18.#314      // EpochWriter.writeLine:(Ljava/io/BufferedWriter;Ljava/lang/String;)V
+   #63 = String             #315          // time,x,y,z
+   #64 = Fieldref           #316.#317     // java/lang/System.out:Ljava/io/PrintStream;
+   #65 = String             #318          // first epochtime set to startTime
+   #66 = String             #319          //  +
+   #67 = Methodref          #53.#320      // java/lang/StringBuilder.append:(I)Ljava/lang/StringBuilder;
+   #68 = String             #321          //  epochs
+   #69 = String             #322          //
+   #70 = String             #323          //  at
+   #71 = Methodref          #18.#324      // EpochWriter.millisToZonedDateTime:(J)Ljava/time/ZonedDateTime;
+   #72 = Methodref          #53.#325      // java/lang/StringBuilder.append:(Ljava/lang/Object;)Ljava/lang/StringBuilder;
+   #73 = Methodref          #326.#327     // java/io/PrintStream.println:(Ljava/lang/String;)V
+   #74 = Fieldref           #316.#328     // java/lang/System.err:Ljava/io/PrintStream;
+   #75 = String             #329          // Interrupt of length:
    #76 = Double             1000.0d
-   #78 = Methodref          #53.#324      // java/lang/StringBuilder.append:(D)Ljava/lang/StringBuilder;
-   #79 = String             #325          // s, at epoch
-   #80 = String             #326          //  \n from:
-   #81 = String             #327          // \n to  :
-   #82 = InterfaceMethodref #228.#328     // java/util/List.size:()I
-   #83 = Methodref          #18.#329      // EpochWriter.writeEpochSummary:(Ljava/time/ZonedDateTime;Ljava/util/List;Ljava/util/List;Ljava/util/List;Ljava/util/List;Ljava/util/List;[I)V
-   #84 = String             #330          // not enough samples for an epoch.. discarding
-   #85 = String             #331          //  samples
-   #86 = InterfaceMethodref #228.#332     // java/util/List.clear:()V
-   #87 = Methodref          #333.#334     // java/lang/Long.valueOf:(J)Ljava/lang/Long;
-   #88 = InterfaceMethodref #228.#335     // java/util/List.add:(Ljava/lang/Object;)Z
-   #89 = Methodref          #97.#336      // java/lang/Double.valueOf:(D)Ljava/lang/Double;
-   #90 = String             #337          // reached endTime at sample:
-   #91 = Methodref          #214.#338     // java/io/BufferedWriter.close:()V
-   #92 = Methodref          #215.#338     // NpyWriter.close:()V
-   #93 = Class              #339          // java/lang/Exception
-   #94 = String             #340          // error closing output files
-   #95 = Methodref          #311.#341     // java/lang/System.exit:(I)V
-   #96 = InterfaceMethodref #228.#342     // java/util/List.get:(I)Ljava/lang/Object;
-   #97 = Class              #343          // java/lang/Double
-   #98 = Methodref          #97.#344      // java/lang/Double.doubleValue:()D
-   #99 = Methodref          #345.#346     // java/lang/Math.abs:(D)D
-  #100 = InterfaceMethodref #228.#347     // java/util/List.set:(ILjava/lang/Object;)Ljava/lang/Object;
-  #101 = Methodref          #345.#348     // java/lang/Math.round:(D)J
-  #102 = String             #349          // linear
-  #103 = Methodref          #217.#350     // java/lang/String.equalsIgnoreCase:(Ljava/lang/String;)Z
-  #104 = Methodref          #351.#352     // Resample.interpLinear:(Ljava/util/List;Ljava/util/List;Ljava/util/List;Ljava/util/List;[J[D[D[D)V
-  #105 = String             #353          // nearest
-  #106 = Methodref          #351.#354     // Resample.interpNearest:(Ljava/util/List;Ljava/util/List;Ljava/util/List;Ljava/util/List;[J[D[D[D)V
-  #107 = String             #355          // Unknown resample method:
-  #108 = Fieldref           #356.#357     // java/time/temporal/ChronoUnit.MILLIS:Ljava/time/temporal/ChronoUnit;
-  #109 = Methodref          #227.#358     // java/time/ZonedDateTime.plus:(JLjava/time/temporal/TemporalUnit;)Ljava/time/ZonedDateTime;
-  #110 = Methodref          #216.#359     // java/time/format/DateTimeFormatter.format:(Ljava/time/temporal/TemporalAccessor;)Ljava/lang/String;
-  #111 = Methodref          #150.#360     // java/text/DecimalFormat.format:(D)Ljava/lang/String;
-  #112 = Methodref          #18.#361      // EpochWriter.toNanos:(Ljava/time/ZonedDateTime;)J
-  #113 = Methodref          #18.#362      // EpochWriter.writeNpyLine:(LNpyWriter;JDDD)V
-  #114 = Methodref          #304.#363     // AccStats.getAccStats:([D[D[DLFilter;Ljava/lang/Boolean;I)[D
-  #115 = Methodref          #304.#364     // AccStats.countStuckVals:([D[D[D)I
-  #116 = Methodref          #304.#365     // AccStats.mean:(Ljava/util/List;)D
-  #117 = String             #366          // \n
-  #118 = Methodref          #214.#367     // java/io/BufferedWriter.write:(Ljava/lang/String;)V
-  #119 = String             #368          // line write error:
-  #120 = Methodref          #93.#306      // java/lang/Exception.toString:()Ljava/lang/String;
-  #121 = Methodref          #97.#369      // java/lang/Double.isNaN:(D)Z
-  #122 = String             #370          // NaN at
-  #123 = Methodref          #53.#371      // java/lang/StringBuilder.append:(J)Ljava/lang/StringBuilder;
-  #124 = Methodref          #372.#373     // java/lang/Float.valueOf:(F)Ljava/lang/Float;
-  #125 = Methodref          #215.#374     // NpyWriter.writeData:(JLjava/lang/Float;Ljava/lang/Float;Ljava/lang/Float;)V
-  #126 = Class              #375          // java/io/IOException
-  #127 = Methodref          #126.#376     // java/io/IOException.printStackTrace:(Ljava/io/PrintStream;)V
-  #128 = String             #377          // error closing file writer:
-  #129 = Methodref          #126.#306     // java/io/IOException.toString:()Ljava/lang/String;
-  #130 = Class              #378          // java/util/Date
-  #131 = Methodref          #130.#379     // java/util/Date."<init>":(J)V
-  #132 = Methodref          #130.#380     // java/util/Date.toInstant:()Ljava/time/Instant;
-  #133 = Fieldref           #381.#382     // java/time/ZoneOffset.UTC:Ljava/time/ZoneOffset;
-  #134 = Methodref          #383.#384     // java/time/LocalDateTime.ofInstant:(Ljava/time/Instant;Ljava/time/ZoneId;)Ljava/time/LocalDateTime;
-  #135 = String             #385          // UTC
-  #136 = Methodref          #383.#386     // java/time/LocalDateTime.atZone:(Ljava/time/ZoneId;)Ljava/time/ZonedDateTime;
-  #137 = Methodref          #227.#380     // java/time/ZonedDateTime.toInstant:()Ljava/time/Instant;
-  #138 = Methodref          #387.#388     // java/time/Instant.toEpochMilli:()J
-  #139 = Methodref          #387.#389     // java/time/Instant.ofEpochMilli:(J)Ljava/time/Instant;
-  #140 = Methodref          #18.#390      // EpochWriter.millisToInstant:(J)Ljava/time/Instant;
-  #141 = Methodref          #387.#386     // java/time/Instant.atZone:(Ljava/time/ZoneId;)Ljava/time/ZonedDateTime;
-  #142 = Fieldref           #391.#392     // java/util/concurrent/TimeUnit.SECONDS:Ljava/util/concurrent/TimeUnit;
-  #143 = Methodref          #387.#393     // java/time/Instant.getEpochSecond:()J
-  #144 = Methodref          #391.#394     // java/util/concurrent/TimeUnit.toNanos:(J)J
-  #145 = Methodref          #387.#395     // java/time/Instant.getNano:()I
-  #146 = Methodref          #18.#396      // EpochWriter.toNanos:(Ljava/time/Instant;)J
-  #147 = Class              #397          // java/text/DecimalFormatSymbols
-  #148 = Fieldref           #398.#399     // java/util/Locale.ENGLISH:Ljava/util/Locale;
-  #149 = Methodref          #147.#400     // java/text/DecimalFormatSymbols."<init>":(Ljava/util/Locale;)V
-  #150 = Class              #401          // java/text/DecimalFormat
-  #151 = String             #402          // 0.000000
-  #152 = Methodref          #150.#403     // java/text/DecimalFormat."<init>":(Ljava/lang/String;Ljava/text/DecimalFormatSymbols;)V
-  #153 = String             #404          // 0.000
-  #154 = String             #405          // 0.00
-  #155 = Class              #406          // java/lang/Object
+   #78 = Methodref          #53.#330      // java/lang/StringBuilder.append:(D)Ljava/lang/StringBuilder;
+   #79 = String             #331          // s, at epoch
+   #80 = String             #332          //  \n from:
+   #81 = String             #333          // \n to  :
+   #82 = InterfaceMethodref #334.#335     // java/util/List.size:()I
+   #83 = Methodref          #18.#336      // EpochWriter.writeEpochSummary:(Ljava/time/ZonedDateTime;Ljava/util/List;Ljava/util/List;Ljava/util/List;Ljava/util/List;Ljava/util/List;[I)V
+   #84 = String             #337          // not enough samples for an epoch.. discarding
+   #85 = String             #338          //  samples
+   #86 = InterfaceMethodref #334.#339     // java/util/List.clear:()V
+   #87 = Methodref          #340.#341     // java/lang/Long.valueOf:(J)Ljava/lang/Long;
+   #88 = InterfaceMethodref #334.#342     // java/util/List.add:(Ljava/lang/Object;)Z
+   #89 = Methodref          #97.#343      // java/lang/Double.valueOf:(D)Ljava/lang/Double;
+   #90 = String             #344          // reached endTime at sample:
+   #91 = Methodref          #345.#346     // java/io/BufferedWriter.close:()V
+   #92 = Methodref          #347.#346     // NpyWriter.close:()V
+   #93 = Class              #348          // java/lang/Exception
+   #94 = String             #349          // error closing output files
+   #95 = Methodref          #316.#350     // java/lang/System.exit:(I)V
+   #96 = InterfaceMethodref #334.#351     // java/util/List.get:(I)Ljava/lang/Object;
+   #97 = Class              #352          // java/lang/Double
+   #98 = Methodref          #97.#353      // java/lang/Double.doubleValue:()D
+   #99 = Methodref          #354.#355     // java/lang/Math.abs:(D)D
+  #100 = InterfaceMethodref #334.#356     // java/util/List.set:(ILjava/lang/Object;)Ljava/lang/Object;
+  #101 = Methodref          #354.#357     // java/lang/Math.round:(D)J
+  #102 = String             #358          // linear
+  #103 = Methodref          #359.#360     // java/lang/String.equalsIgnoreCase:(Ljava/lang/String;)Z
+  #104 = Methodref          #361.#362     // Resample.interpLinear:(Ljava/util/List;Ljava/util/List;Ljava/util/List;Ljava/util/List;[J[D[D[D)V
+  #105 = String             #363          // nearest
+  #106 = Methodref          #361.#364     // Resample.interpNearest:(Ljava/util/List;Ljava/util/List;Ljava/util/List;Ljava/util/List;[J[D[D[D)V
+  #107 = String             #365          // Unknown resample method:
+  #108 = Fieldref           #366.#367     // java/time/temporal/ChronoUnit.MILLIS:Ljava/time/temporal/ChronoUnit;
+  #109 = Methodref          #368.#369     // java/time/ZonedDateTime.plus:(JLjava/time/temporal/TemporalUnit;)Ljava/time/ZonedDateTime;
+  #110 = Methodref          #370.#371     // java/time/format/DateTimeFormatter.format:(Ljava/time/temporal/TemporalAccessor;)Ljava/lang/String;
+  #111 = Methodref          #150.#372     // java/text/DecimalFormat.format:(D)Ljava/lang/String;
+  #112 = Methodref          #18.#373      // EpochWriter.toNanos:(Ljava/time/ZonedDateTime;)J
+  #113 = Methodref          #18.#374      // EpochWriter.writeNpyLine:(LNpyWriter;JDDD)V
+  #114 = Methodref          #309.#375     // AccStats.getAccStats:([D[D[DLFilter;Ljava/lang/Boolean;I)[D
+  #115 = Methodref          #309.#376     // AccStats.countStuckVals:([D[D[D)I
+  #116 = Methodref          #309.#377     // AccStats.mean:(Ljava/util/List;)D
+  #117 = String             #378          // \n
+  #118 = Methodref          #345.#379     // java/io/BufferedWriter.write:(Ljava/lang/String;)V
+  #119 = String             #380          // line write error:
+  #120 = Methodref          #93.#311      // java/lang/Exception.toString:()Ljava/lang/String;
+  #121 = Methodref          #97.#381      // java/lang/Double.isNaN:(D)Z
+  #122 = String             #382          // NaN at
+  #123 = Methodref          #53.#383      // java/lang/StringBuilder.append:(J)Ljava/lang/StringBuilder;
+  #124 = Methodref          #384.#385     // java/lang/Float.valueOf:(F)Ljava/lang/Float;
+  #125 = Methodref          #347.#386     // NpyWriter.writeData:(JLjava/lang/Float;Ljava/lang/Float;Ljava/lang/Float;)V
+  #126 = Class              #387          // java/io/IOException
+  #127 = Methodref          #126.#388     // java/io/IOException.printStackTrace:(Ljava/io/PrintStream;)V
+  #128 = String             #389          // error closing file writer:
+  #129 = Methodref          #126.#311     // java/io/IOException.toString:()Ljava/lang/String;
+  #130 = Class              #390          // java/util/Date
+  #131 = Methodref          #130.#391     // java/util/Date."<init>":(J)V
+  #132 = Methodref          #130.#392     // java/util/Date.toInstant:()Ljava/time/Instant;
+  #133 = Fieldref           #393.#394     // java/time/ZoneOffset.UTC:Ljava/time/ZoneOffset;
+  #134 = Methodref          #395.#396     // java/time/LocalDateTime.ofInstant:(Ljava/time/Instant;Ljava/time/ZoneId;)Ljava/time/LocalDateTime;
+  #135 = String             #397          // UTC
+  #136 = Methodref          #395.#398     // java/time/LocalDateTime.atZone:(Ljava/time/ZoneId;)Ljava/time/ZonedDateTime;
+  #137 = Methodref          #368.#392     // java/time/ZonedDateTime.toInstant:()Ljava/time/Instant;
+  #138 = Methodref          #399.#400     // java/time/Instant.toEpochMilli:()J
+  #139 = Methodref          #399.#401     // java/time/Instant.ofEpochMilli:(J)Ljava/time/Instant;
+  #140 = Methodref          #18.#402      // EpochWriter.millisToInstant:(J)Ljava/time/Instant;
+  #141 = Methodref          #399.#398     // java/time/Instant.atZone:(Ljava/time/ZoneId;)Ljava/time/ZonedDateTime;
+  #142 = Fieldref           #403.#404     // java/util/concurrent/TimeUnit.SECONDS:Ljava/util/concurrent/TimeUnit;
+  #143 = Methodref          #399.#405     // java/time/Instant.getEpochSecond:()J
+  #144 = Methodref          #403.#406     // java/util/concurrent/TimeUnit.toNanos:(J)J
+  #145 = Methodref          #399.#407     // java/time/Instant.getNano:()I
+  #146 = Methodref          #18.#408      // EpochWriter.toNanos:(Ljava/time/Instant;)J
+  #147 = Class              #409          // java/text/DecimalFormatSymbols
+  #148 = Fieldref           #410.#411     // java/util/Locale.ENGLISH:Ljava/util/Locale;
+  #149 = Methodref          #147.#412     // java/text/DecimalFormatSymbols."<init>":(Ljava/util/Locale;)V
+  #150 = Class              #413          // java/text/DecimalFormat
+  #151 = String             #414          // 0.000000
+  #152 = Methodref          #150.#415     // java/text/DecimalFormat."<init>":(Ljava/lang/String;Ljava/text/DecimalFormatSymbols;)V
+  #153 = String             #416          // 0.000
+  #154 = String             #417          // 0.00
+  #155 = Class              #418          // java/lang/Object
   #156 = Utf8               decimalFormatSymbol
   #157 = Utf8               Ljava/text/DecimalFormatSymbols;
   #158 = Utf8               DF6
   #159 = Utf8               Ljava/text/DecimalFormat;
   #160 = Utf8               DF3
   #161 = Utf8               DF2
   #162 = Utf8               UNUSED_DATE
@@ -214,328 +214,340 @@
   #207 = Utf8               zoneId
   #208 = Utf8               Ljava/time/ZoneId;
   #209 = Utf8               <init>
   #210 = Utf8               (Ljava/io/BufferedWriter;Ljava/io/BufferedWriter;LNpyWriter;Ljava/time/format/DateTimeFormatter;Ljava/lang/String;IILjava/lang/String;I[D[D[DLjava/lang/Boolean;DLFilter;JJZ)V
   #211 = Utf8               Code
   #212 = Utf8               LineNumberTable
   #213 = Utf8               StackMapTable
-  #214 = Class              #407          // java/io/BufferedWriter
-  #215 = Class              #408          // NpyWriter
-  #216 = Class              #409          // java/time/format/DateTimeFormatter
-  #217 = Class              #410          // java/lang/String
-  #218 = Class              #179          // "[D"
-  #219 = Class              #411          // java/lang/Boolean
-  #220 = Class              #412          // Filter
-  #221 = Utf8               newValues
-  #222 = Utf8               (JDDDD[I)Z
-  #223 = Class              #413          // "[I"
-  #224 = Class              #414          // java/io/PrintStream
-  #225 = Utf8               writeEpochSummary
-  #226 = Utf8               (Ljava/time/ZonedDateTime;Ljava/util/List;Ljava/util/List;Ljava/util/List;Ljava/util/List;Ljava/util/List;[I)V
-  #227 = Class              #415          // java/time/ZonedDateTime
-  #228 = Class              #416          // java/util/List
-  #229 = Class              #417          // "[J"
-  #230 = Utf8               (Ljava/time/ZonedDateTime;Ljava/util/List<Ljava/lang/Long;>;Ljava/util/List<Ljava/lang/Double;>;Ljava/util/List<Ljava/lang/Double;>;Ljava/util/List<Ljava/lang/Double;>;Ljava/util/List<Ljava/lang/Double;>;[I)V
-  #231 = Utf8               writeLine
-  #232 = Utf8               (Ljava/io/BufferedWriter;Ljava/lang/String;)V
-  #233 = Utf8               writeNpyLine
-  #234 = Utf8               (LNpyWriter;JDDD)V
-  #235 = Utf8               closeWriters
-  #236 = Utf8               ()V
-  #237 = Utf8               millisToTimestamp
-  #238 = Utf8               (D)Ljava/time/LocalDateTime;
-  #239 = Utf8               timestampToMillis
-  #240 = Utf8               (Ljava/time/LocalDateTime;)D
-  #241 = Utf8               millisToInstant
-  #242 = Utf8               (J)Ljava/time/Instant;
-  #243 = Utf8               millisToZonedDateTime
-  #244 = Utf8               (J)Ljava/time/ZonedDateTime;
-  #245 = Utf8               toNanos
-  #246 = Utf8               (Ljava/time/Instant;)J
-  #247 = Utf8               (Ljava/time/ZonedDateTime;)J
-  #248 = Utf8               <clinit>
-  #249 = Utf8               SourceFile
-  #250 = Utf8               EpochWriter.java
-  #251 = NameAndType        #209:#236     // "<init>":()V
-  #252 = NameAndType        #162:#163     // UNUSED_DATE:J
-  #253 = Utf8               java/util/ArrayList
-  #254 = NameAndType        #165:#166     // timeVals:Ljava/util/List;
-  #255 = NameAndType        #169:#166     // xVals:Ljava/util/List;
-  #256 = NameAndType        #171:#166     // yVals:Ljava/util/List;
-  #257 = NameAndType        #172:#166     // zVals:Ljava/util/List;
-  #258 = NameAndType        #173:#166     // temperatureVals:Ljava/util/List;
-  #259 = NameAndType        #174:#175     // minSamplesForEpoch:I
-  #260 = NameAndType        #177:#163     // prevTimeVal:J
-  #261 = NameAndType        #178:#179     // prevXYZT:[D
-  #262 = NameAndType        #180:#181     // edgeInterpolation:Z
-  #263 = Utf8               EpochWriter
-  #264 = NameAndType        #182:#163     // epochStartTime:J
-  #265 = NameAndType        #202:#203     // epochFileWriter:Ljava/io/BufferedWriter;
-  #266 = NameAndType        #204:#203     // rawWriter:Ljava/io/BufferedWriter;
-  #267 = NameAndType        #205:#206     // npyWriter:LNpyWriter;
-  #268 = NameAndType        #184:#185     // timeFormat:Ljava/time/format/DateTimeFormatter;
-  #269 = NameAndType        #183:#175     // epochPeriod:I
-  #270 = NameAndType        #194:#175     // intendedSampleRate:I
-  #271 = NameAndType        #195:#187     // resampleMethod:Ljava/lang/String;
-  #272 = NameAndType        #196:#175     // range:I
-  #273 = NameAndType        #191:#179     // xyzIntercept:[D
-  #274 = NameAndType        #192:#179     // xyzSlope:[D
-  #275 = NameAndType        #193:#179     // xyzSlopeT:[D
-  #276 = NameAndType        #418:#419     // booleanValue:()Z
-  #277 = NameAndType        #188:#181     // getStationaryBouts:Z
-  #278 = NameAndType        #189:#190     // stationaryStd:D
-  #279 = NameAndType        #197:#198     // filter:LFilter;
-  #280 = NameAndType        #199:#163     // startTime:J
-  #281 = NameAndType        #200:#163     // endTime:J
-  #282 = NameAndType        #201:#181     // getFeatures:Z
-  #283 = Class              #420          // java/time/ZoneId
-  #284 = NameAndType        #421:#422     // of:(Ljava/lang/String;)Ljava/time/ZoneId;
-  #285 = NameAndType        #207:#208     // zoneId:Ljava/time/ZoneId;
-  #286 = NameAndType        #156:#157     // decimalFormatSymbol:Ljava/text/DecimalFormatSymbols;
-  #287 = Utf8               NaN
-  #288 = NameAndType        #423:#424     // setNaN:(Ljava/lang/String;)V
-  #289 = Utf8               inf
-  #290 = NameAndType        #425:#424     // setInfinity:(Ljava/lang/String;)V
-  #291 = NameAndType        #158:#159     // DF6:Ljava/text/DecimalFormat;
-  #292 = NameAndType        #426:#427     // setDecimalFormatSymbols:(Ljava/text/DecimalFormatSymbols;)V
-  #293 = NameAndType        #160:#159     // DF3:Ljava/text/DecimalFormat;
-  #294 = NameAndType        #161:#159     // DF2:Ljava/text/DecimalFormat;
-  #295 = Class              #428          // java/math/RoundingMode
-  #296 = NameAndType        #429:#430     // CEILING:Ljava/math/RoundingMode;
-  #297 = NameAndType        #431:#432     // setRoundingMode:(Ljava/math/RoundingMode;)V
-  #298 = NameAndType        #433:#430     // HALF_UP:Ljava/math/RoundingMode;
-  #299 = Utf8               time
-  #300 = Utf8               java/lang/StringBuilder
-  #301 = NameAndType        #434:#435     // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #302 = Utf8               ,
-  #303 = NameAndType        #436:#437     // valueOf:(Z)Ljava/lang/Boolean;
-  #304 = Class              #438          // AccStats
-  #305 = NameAndType        #439:#440     // getStatsHeader:(Ljava/lang/Boolean;)Ljava/lang/String;
-  #306 = NameAndType        #441:#442     // toString:()Ljava/lang/String;
-  #307 = Utf8               ,temp,samples
-  #308 = Utf8               ,dataErrors,clipsBeforeCalibr,clipsAfterCalibr,rawSamples
-  #309 = NameAndType        #231:#232     // writeLine:(Ljava/io/BufferedWriter;Ljava/lang/String;)V
-  #310 = Utf8               time,x,y,z
-  #311 = Class              #443          // java/lang/System
-  #312 = NameAndType        #444:#445     // out:Ljava/io/PrintStream;
-  #313 = Utf8               first epochtime set to startTime
-  #314 = Utf8                +
-  #315 = NameAndType        #434:#446     // append:(I)Ljava/lang/StringBuilder;
-  #316 = Utf8                epochs
-  #317 = Utf8
-  #318 = Utf8                at
-  #319 = NameAndType        #243:#244     // millisToZonedDateTime:(J)Ljava/time/ZonedDateTime;
-  #320 = NameAndType        #434:#447     // append:(Ljava/lang/Object;)Ljava/lang/StringBuilder;
-  #321 = NameAndType        #448:#424     // println:(Ljava/lang/String;)V
-  #322 = NameAndType        #449:#445     // err:Ljava/io/PrintStream;
-  #323 = Utf8               Interrupt of length:
-  #324 = NameAndType        #434:#450     // append:(D)Ljava/lang/StringBuilder;
-  #325 = Utf8               s, at epoch
-  #326 = Utf8                \n from:
-  #327 = Utf8               \n to  :
-  #328 = NameAndType        #451:#452     // size:()I
-  #329 = NameAndType        #225:#226     // writeEpochSummary:(Ljava/time/ZonedDateTime;Ljava/util/List;Ljava/util/List;Ljava/util/List;Ljava/util/List;Ljava/util/List;[I)V
-  #330 = Utf8               not enough samples for an epoch.. discarding
-  #331 = Utf8                samples
-  #332 = NameAndType        #453:#236     // clear:()V
-  #333 = Class              #454          // java/lang/Long
-  #334 = NameAndType        #436:#455     // valueOf:(J)Ljava/lang/Long;
-  #335 = NameAndType        #456:#457     // add:(Ljava/lang/Object;)Z
-  #336 = NameAndType        #436:#458     // valueOf:(D)Ljava/lang/Double;
-  #337 = Utf8               reached endTime at sample:
-  #338 = NameAndType        #459:#236     // close:()V
-  #339 = Utf8               java/lang/Exception
-  #340 = Utf8               error closing output files
-  #341 = NameAndType        #460:#461     // exit:(I)V
-  #342 = NameAndType        #462:#463     // get:(I)Ljava/lang/Object;
-  #343 = Utf8               java/lang/Double
-  #344 = NameAndType        #464:#465     // doubleValue:()D
-  #345 = Class              #466          // java/lang/Math
-  #346 = NameAndType        #467:#468     // abs:(D)D
-  #347 = NameAndType        #469:#470     // set:(ILjava/lang/Object;)Ljava/lang/Object;
-  #348 = NameAndType        #471:#472     // round:(D)J
-  #349 = Utf8               linear
-  #350 = NameAndType        #473:#474     // equalsIgnoreCase:(Ljava/lang/String;)Z
-  #351 = Class              #475          // Resample
-  #352 = NameAndType        #476:#477     // interpLinear:(Ljava/util/List;Ljava/util/List;Ljava/util/List;Ljava/util/List;[J[D[D[D)V
-  #353 = Utf8               nearest
-  #354 = NameAndType        #478:#477     // interpNearest:(Ljava/util/List;Ljava/util/List;Ljava/util/List;Ljava/util/List;[J[D[D[D)V
-  #355 = Utf8               Unknown resample method:
-  #356 = Class              #479          // java/time/temporal/ChronoUnit
-  #357 = NameAndType        #480:#481     // MILLIS:Ljava/time/temporal/ChronoUnit;
-  #358 = NameAndType        #482:#483     // plus:(JLjava/time/temporal/TemporalUnit;)Ljava/time/ZonedDateTime;
-  #359 = NameAndType        #484:#485     // format:(Ljava/time/temporal/TemporalAccessor;)Ljava/lang/String;
-  #360 = NameAndType        #484:#486     // format:(D)Ljava/lang/String;
-  #361 = NameAndType        #245:#247     // toNanos:(Ljava/time/ZonedDateTime;)J
-  #362 = NameAndType        #233:#234     // writeNpyLine:(LNpyWriter;JDDD)V
-  #363 = NameAndType        #487:#488     // getAccStats:([D[D[DLFilter;Ljava/lang/Boolean;I)[D
-  #364 = NameAndType        #489:#490     // countStuckVals:([D[D[D)I
-  #365 = NameAndType        #491:#492     // mean:(Ljava/util/List;)D
-  #366 = Utf8               \n
-  #367 = NameAndType        #493:#424     // write:(Ljava/lang/String;)V
-  #368 = Utf8               line write error:
-  #369 = NameAndType        #494:#495     // isNaN:(D)Z
-  #370 = Utf8               NaN at
-  #371 = NameAndType        #434:#496     // append:(J)Ljava/lang/StringBuilder;
-  #372 = Class              #497          // java/lang/Float
-  #373 = NameAndType        #436:#498     // valueOf:(F)Ljava/lang/Float;
-  #374 = NameAndType        #499:#500     // writeData:(JLjava/lang/Float;Ljava/lang/Float;Ljava/lang/Float;)V
-  #375 = Utf8               java/io/IOException
-  #376 = NameAndType        #501:#502     // printStackTrace:(Ljava/io/PrintStream;)V
-  #377 = Utf8               error closing file writer:
-  #378 = Utf8               java/util/Date
-  #379 = NameAndType        #209:#503     // "<init>":(J)V
-  #380 = NameAndType        #504:#505     // toInstant:()Ljava/time/Instant;
-  #381 = Class              #506          // java/time/ZoneOffset
-  #382 = NameAndType        #385:#507     // UTC:Ljava/time/ZoneOffset;
-  #383 = Class              #508          // java/time/LocalDateTime
-  #384 = NameAndType        #509:#510     // ofInstant:(Ljava/time/Instant;Ljava/time/ZoneId;)Ljava/time/LocalDateTime;
-  #385 = Utf8               UTC
-  #386 = NameAndType        #511:#512     // atZone:(Ljava/time/ZoneId;)Ljava/time/ZonedDateTime;
-  #387 = Class              #513          // java/time/Instant
-  #388 = NameAndType        #514:#515     // toEpochMilli:()J
-  #389 = NameAndType        #516:#242     // ofEpochMilli:(J)Ljava/time/Instant;
-  #390 = NameAndType        #241:#242     // millisToInstant:(J)Ljava/time/Instant;
-  #391 = Class              #517          // java/util/concurrent/TimeUnit
-  #392 = NameAndType        #518:#519     // SECONDS:Ljava/util/concurrent/TimeUnit;
-  #393 = NameAndType        #520:#515     // getEpochSecond:()J
-  #394 = NameAndType        #245:#521     // toNanos:(J)J
-  #395 = NameAndType        #522:#452     // getNano:()I
-  #396 = NameAndType        #245:#246     // toNanos:(Ljava/time/Instant;)J
-  #397 = Utf8               java/text/DecimalFormatSymbols
-  #398 = Class              #523          // java/util/Locale
-  #399 = NameAndType        #524:#525     // ENGLISH:Ljava/util/Locale;
-  #400 = NameAndType        #209:#526     // "<init>":(Ljava/util/Locale;)V
-  #401 = Utf8               java/text/DecimalFormat
-  #402 = Utf8               0.000000
-  #403 = NameAndType        #209:#527     // "<init>":(Ljava/lang/String;Ljava/text/DecimalFormatSymbols;)V
-  #404 = Utf8               0.000
-  #405 = Utf8               0.00
-  #406 = Utf8               java/lang/Object
-  #407 = Utf8               java/io/BufferedWriter
-  #408 = Utf8               NpyWriter
-  #409 = Utf8               java/time/format/DateTimeFormatter
-  #410 = Utf8               java/lang/String
-  #411 = Utf8               java/lang/Boolean
-  #412 = Utf8               Filter
-  #413 = Utf8               [I
-  #414 = Utf8               java/io/PrintStream
-  #415 = Utf8               java/time/ZonedDateTime
-  #416 = Utf8               java/util/List
-  #417 = Utf8               [J
-  #418 = Utf8               booleanValue
-  #419 = Utf8               ()Z
-  #420 = Utf8               java/time/ZoneId
-  #421 = Utf8               of
-  #422 = Utf8               (Ljava/lang/String;)Ljava/time/ZoneId;
-  #423 = Utf8               setNaN
-  #424 = Utf8               (Ljava/lang/String;)V
-  #425 = Utf8               setInfinity
-  #426 = Utf8               setDecimalFormatSymbols
-  #427 = Utf8               (Ljava/text/DecimalFormatSymbols;)V
-  #428 = Utf8               java/math/RoundingMode
-  #429 = Utf8               CEILING
-  #430 = Utf8               Ljava/math/RoundingMode;
-  #431 = Utf8               setRoundingMode
-  #432 = Utf8               (Ljava/math/RoundingMode;)V
-  #433 = Utf8               HALF_UP
-  #434 = Utf8               append
-  #435 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #436 = Utf8               valueOf
-  #437 = Utf8               (Z)Ljava/lang/Boolean;
-  #438 = Utf8               AccStats
-  #439 = Utf8               getStatsHeader
-  #440 = Utf8               (Ljava/lang/Boolean;)Ljava/lang/String;
-  #441 = Utf8               toString
-  #442 = Utf8               ()Ljava/lang/String;
-  #443 = Utf8               java/lang/System
-  #444 = Utf8               out
-  #445 = Utf8               Ljava/io/PrintStream;
-  #446 = Utf8               (I)Ljava/lang/StringBuilder;
-  #447 = Utf8               (Ljava/lang/Object;)Ljava/lang/StringBuilder;
-  #448 = Utf8               println
-  #449 = Utf8               err
-  #450 = Utf8               (D)Ljava/lang/StringBuilder;
-  #451 = Utf8               size
-  #452 = Utf8               ()I
-  #453 = Utf8               clear
-  #454 = Utf8               java/lang/Long
-  #455 = Utf8               (J)Ljava/lang/Long;
-  #456 = Utf8               add
-  #457 = Utf8               (Ljava/lang/Object;)Z
-  #458 = Utf8               (D)Ljava/lang/Double;
-  #459 = Utf8               close
-  #460 = Utf8               exit
-  #461 = Utf8               (I)V
-  #462 = Utf8               get
-  #463 = Utf8               (I)Ljava/lang/Object;
-  #464 = Utf8               doubleValue
-  #465 = Utf8               ()D
-  #466 = Utf8               java/lang/Math
-  #467 = Utf8               abs
-  #468 = Utf8               (D)D
-  #469 = Utf8               set
-  #470 = Utf8               (ILjava/lang/Object;)Ljava/lang/Object;
-  #471 = Utf8               round
-  #472 = Utf8               (D)J
-  #473 = Utf8               equalsIgnoreCase
-  #474 = Utf8               (Ljava/lang/String;)Z
-  #475 = Utf8               Resample
-  #476 = Utf8               interpLinear
-  #477 = Utf8               (Ljava/util/List;Ljava/util/List;Ljava/util/List;Ljava/util/List;[J[D[D[D)V
-  #478 = Utf8               interpNearest
-  #479 = Utf8               java/time/temporal/ChronoUnit
-  #480 = Utf8               MILLIS
-  #481 = Utf8               Ljava/time/temporal/ChronoUnit;
-  #482 = Utf8               plus
-  #483 = Utf8               (JLjava/time/temporal/TemporalUnit;)Ljava/time/ZonedDateTime;
-  #484 = Utf8               format
-  #485 = Utf8               (Ljava/time/temporal/TemporalAccessor;)Ljava/lang/String;
-  #486 = Utf8               (D)Ljava/lang/String;
-  #487 = Utf8               getAccStats
-  #488 = Utf8               ([D[D[DLFilter;Ljava/lang/Boolean;I)[D
-  #489 = Utf8               countStuckVals
-  #490 = Utf8               ([D[D[D)I
-  #491 = Utf8               mean
-  #492 = Utf8               (Ljava/util/List;)D
-  #493 = Utf8               write
-  #494 = Utf8               isNaN
-  #495 = Utf8               (D)Z
-  #496 = Utf8               (J)Ljava/lang/StringBuilder;
-  #497 = Utf8               java/lang/Float
-  #498 = Utf8               (F)Ljava/lang/Float;
-  #499 = Utf8               writeData
-  #500 = Utf8               (JLjava/lang/Float;Ljava/lang/Float;Ljava/lang/Float;)V
-  #501 = Utf8               printStackTrace
-  #502 = Utf8               (Ljava/io/PrintStream;)V
-  #503 = Utf8               (J)V
-  #504 = Utf8               toInstant
-  #505 = Utf8               ()Ljava/time/Instant;
-  #506 = Utf8               java/time/ZoneOffset
-  #507 = Utf8               Ljava/time/ZoneOffset;
-  #508 = Utf8               java/time/LocalDateTime
-  #509 = Utf8               ofInstant
-  #510 = Utf8               (Ljava/time/Instant;Ljava/time/ZoneId;)Ljava/time/LocalDateTime;
-  #511 = Utf8               atZone
-  #512 = Utf8               (Ljava/time/ZoneId;)Ljava/time/ZonedDateTime;
-  #513 = Utf8               java/time/Instant
-  #514 = Utf8               toEpochMilli
-  #515 = Utf8               ()J
-  #516 = Utf8               ofEpochMilli
-  #517 = Utf8               java/util/concurrent/TimeUnit
-  #518 = Utf8               SECONDS
-  #519 = Utf8               Ljava/util/concurrent/TimeUnit;
-  #520 = Utf8               getEpochSecond
-  #521 = Utf8               (J)J
-  #522 = Utf8               getNano
-  #523 = Utf8               java/util/Locale
-  #524 = Utf8               ENGLISH
-  #525 = Utf8               Ljava/util/Locale;
-  #526 = Utf8               (Ljava/util/Locale;)V
-  #527 = Utf8               (Ljava/lang/String;Ljava/text/DecimalFormatSymbols;)V
+  #214 = Class              #267          // EpochWriter
+  #215 = Class              #419          // java/io/BufferedWriter
+  #216 = Class              #420          // NpyWriter
+  #217 = Class              #421          // java/time/format/DateTimeFormatter
+  #218 = Class              #422          // java/lang/String
+  #219 = Class              #179          // "[D"
+  #220 = Class              #423          // java/lang/Boolean
+  #221 = Class              #424          // Filter
+  #222 = Utf8               newValues
+  #223 = Utf8               (JDDDD[I)Z
+  #224 = Class              #425          // "[I"
+  #225 = Class              #426          // java/io/PrintStream
+  #226 = Class              #305          // java/lang/StringBuilder
+  #227 = Class              #348          // java/lang/Exception
+  #228 = Utf8               writeEpochSummary
+  #229 = Utf8               (Ljava/time/ZonedDateTime;Ljava/util/List;Ljava/util/List;Ljava/util/List;Ljava/util/List;Ljava/util/List;[I)V
+  #230 = Class              #427          // java/time/ZonedDateTime
+  #231 = Class              #428          // java/util/List
+  #232 = Class              #429          // "[J"
+  #233 = Utf8               (Ljava/time/ZonedDateTime;Ljava/util/List<Ljava/lang/Long;>;Ljava/util/List<Ljava/lang/Double;>;Ljava/util/List<Ljava/lang/Double;>;Ljava/util/List<Ljava/lang/Double;>;Ljava/util/List<Ljava/lang/Double;>;[I)V
+  #234 = Utf8               writeLine
+  #235 = Utf8               (Ljava/io/BufferedWriter;Ljava/lang/String;)V
+  #236 = Utf8               writeNpyLine
+  #237 = Utf8               (LNpyWriter;JDDD)V
+  #238 = Utf8               closeWriters
+  #239 = Utf8               ()V
+  #240 = Class              #387          // java/io/IOException
+  #241 = Utf8               millisToTimestamp
+  #242 = Utf8               (D)Ljava/time/LocalDateTime;
+  #243 = Utf8               timestampToMillis
+  #244 = Utf8               (Ljava/time/LocalDateTime;)D
+  #245 = Utf8               millisToInstant
+  #246 = Utf8               (J)Ljava/time/Instant;
+  #247 = Utf8               millisToZonedDateTime
+  #248 = Utf8               (J)Ljava/time/ZonedDateTime;
+  #249 = Utf8               toNanos
+  #250 = Utf8               (Ljava/time/Instant;)J
+  #251 = Utf8               (Ljava/time/ZonedDateTime;)J
+  #252 = Utf8               <clinit>
+  #253 = Utf8               SourceFile
+  #254 = Utf8               EpochWriter.java
+  #255 = NameAndType        #209:#239     // "<init>":()V
+  #256 = NameAndType        #162:#163     // UNUSED_DATE:J
+  #257 = Utf8               java/util/ArrayList
+  #258 = NameAndType        #165:#166     // timeVals:Ljava/util/List;
+  #259 = NameAndType        #169:#166     // xVals:Ljava/util/List;
+  #260 = NameAndType        #171:#166     // yVals:Ljava/util/List;
+  #261 = NameAndType        #172:#166     // zVals:Ljava/util/List;
+  #262 = NameAndType        #173:#166     // temperatureVals:Ljava/util/List;
+  #263 = NameAndType        #174:#175     // minSamplesForEpoch:I
+  #264 = NameAndType        #177:#163     // prevTimeVal:J
+  #265 = NameAndType        #178:#179     // prevXYZT:[D
+  #266 = NameAndType        #180:#181     // edgeInterpolation:Z
+  #267 = Utf8               EpochWriter
+  #268 = NameAndType        #182:#163     // epochStartTime:J
+  #269 = NameAndType        #202:#203     // epochFileWriter:Ljava/io/BufferedWriter;
+  #270 = NameAndType        #204:#203     // rawWriter:Ljava/io/BufferedWriter;
+  #271 = NameAndType        #205:#206     // npyWriter:LNpyWriter;
+  #272 = NameAndType        #184:#185     // timeFormat:Ljava/time/format/DateTimeFormatter;
+  #273 = NameAndType        #183:#175     // epochPeriod:I
+  #274 = NameAndType        #194:#175     // intendedSampleRate:I
+  #275 = NameAndType        #195:#187     // resampleMethod:Ljava/lang/String;
+  #276 = NameAndType        #196:#175     // range:I
+  #277 = NameAndType        #191:#179     // xyzIntercept:[D
+  #278 = NameAndType        #192:#179     // xyzSlope:[D
+  #279 = NameAndType        #193:#179     // xyzSlopeT:[D
+  #280 = Class              #423          // java/lang/Boolean
+  #281 = NameAndType        #430:#431     // booleanValue:()Z
+  #282 = NameAndType        #188:#181     // getStationaryBouts:Z
+  #283 = NameAndType        #189:#190     // stationaryStd:D
+  #284 = NameAndType        #197:#198     // filter:LFilter;
+  #285 = NameAndType        #199:#163     // startTime:J
+  #286 = NameAndType        #200:#163     // endTime:J
+  #287 = NameAndType        #201:#181     // getFeatures:Z
+  #288 = Class              #432          // java/time/ZoneId
+  #289 = NameAndType        #433:#434     // of:(Ljava/lang/String;)Ljava/time/ZoneId;
+  #290 = NameAndType        #207:#208     // zoneId:Ljava/time/ZoneId;
+  #291 = NameAndType        #156:#157     // decimalFormatSymbol:Ljava/text/DecimalFormatSymbols;
+  #292 = Utf8               NaN
+  #293 = NameAndType        #435:#436     // setNaN:(Ljava/lang/String;)V
+  #294 = Utf8               inf
+  #295 = NameAndType        #437:#436     // setInfinity:(Ljava/lang/String;)V
+  #296 = NameAndType        #158:#159     // DF6:Ljava/text/DecimalFormat;
+  #297 = NameAndType        #438:#439     // setDecimalFormatSymbols:(Ljava/text/DecimalFormatSymbols;)V
+  #298 = NameAndType        #160:#159     // DF3:Ljava/text/DecimalFormat;
+  #299 = NameAndType        #161:#159     // DF2:Ljava/text/DecimalFormat;
+  #300 = Class              #440          // java/math/RoundingMode
+  #301 = NameAndType        #441:#442     // CEILING:Ljava/math/RoundingMode;
+  #302 = NameAndType        #443:#444     // setRoundingMode:(Ljava/math/RoundingMode;)V
+  #303 = NameAndType        #445:#442     // HALF_UP:Ljava/math/RoundingMode;
+  #304 = Utf8               time
+  #305 = Utf8               java/lang/StringBuilder
+  #306 = NameAndType        #446:#447     // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #307 = Utf8               ,
+  #308 = NameAndType        #448:#449     // valueOf:(Z)Ljava/lang/Boolean;
+  #309 = Class              #450          // AccStats
+  #310 = NameAndType        #451:#452     // getStatsHeader:(Ljava/lang/Boolean;)Ljava/lang/String;
+  #311 = NameAndType        #453:#454     // toString:()Ljava/lang/String;
+  #312 = Utf8               ,temp,samples
+  #313 = Utf8               ,dataErrors,clipsBeforeCalibr,clipsAfterCalibr,rawSamples
+  #314 = NameAndType        #234:#235     // writeLine:(Ljava/io/BufferedWriter;Ljava/lang/String;)V
+  #315 = Utf8               time,x,y,z
+  #316 = Class              #455          // java/lang/System
+  #317 = NameAndType        #456:#457     // out:Ljava/io/PrintStream;
+  #318 = Utf8               first epochtime set to startTime
+  #319 = Utf8                +
+  #320 = NameAndType        #446:#458     // append:(I)Ljava/lang/StringBuilder;
+  #321 = Utf8                epochs
+  #322 = Utf8
+  #323 = Utf8                at
+  #324 = NameAndType        #247:#248     // millisToZonedDateTime:(J)Ljava/time/ZonedDateTime;
+  #325 = NameAndType        #446:#459     // append:(Ljava/lang/Object;)Ljava/lang/StringBuilder;
+  #326 = Class              #426          // java/io/PrintStream
+  #327 = NameAndType        #460:#436     // println:(Ljava/lang/String;)V
+  #328 = NameAndType        #461:#457     // err:Ljava/io/PrintStream;
+  #329 = Utf8               Interrupt of length:
+  #330 = NameAndType        #446:#462     // append:(D)Ljava/lang/StringBuilder;
+  #331 = Utf8               s, at epoch
+  #332 = Utf8                \n from:
+  #333 = Utf8               \n to  :
+  #334 = Class              #428          // java/util/List
+  #335 = NameAndType        #463:#464     // size:()I
+  #336 = NameAndType        #228:#229     // writeEpochSummary:(Ljava/time/ZonedDateTime;Ljava/util/List;Ljava/util/List;Ljava/util/List;Ljava/util/List;Ljava/util/List;[I)V
+  #337 = Utf8               not enough samples for an epoch.. discarding
+  #338 = Utf8                samples
+  #339 = NameAndType        #465:#239     // clear:()V
+  #340 = Class              #466          // java/lang/Long
+  #341 = NameAndType        #448:#467     // valueOf:(J)Ljava/lang/Long;
+  #342 = NameAndType        #468:#469     // add:(Ljava/lang/Object;)Z
+  #343 = NameAndType        #448:#470     // valueOf:(D)Ljava/lang/Double;
+  #344 = Utf8               reached endTime at sample:
+  #345 = Class              #419          // java/io/BufferedWriter
+  #346 = NameAndType        #471:#239     // close:()V
+  #347 = Class              #420          // NpyWriter
+  #348 = Utf8               java/lang/Exception
+  #349 = Utf8               error closing output files
+  #350 = NameAndType        #472:#473     // exit:(I)V
+  #351 = NameAndType        #474:#475     // get:(I)Ljava/lang/Object;
+  #352 = Utf8               java/lang/Double
+  #353 = NameAndType        #476:#477     // doubleValue:()D
+  #354 = Class              #478          // java/lang/Math
+  #355 = NameAndType        #479:#480     // abs:(D)D
+  #356 = NameAndType        #481:#482     // set:(ILjava/lang/Object;)Ljava/lang/Object;
+  #357 = NameAndType        #483:#484     // round:(D)J
+  #358 = Utf8               linear
+  #359 = Class              #422          // java/lang/String
+  #360 = NameAndType        #485:#486     // equalsIgnoreCase:(Ljava/lang/String;)Z
+  #361 = Class              #487          // Resample
+  #362 = NameAndType        #488:#489     // interpLinear:(Ljava/util/List;Ljava/util/List;Ljava/util/List;Ljava/util/List;[J[D[D[D)V
+  #363 = Utf8               nearest
+  #364 = NameAndType        #490:#489     // interpNearest:(Ljava/util/List;Ljava/util/List;Ljava/util/List;Ljava/util/List;[J[D[D[D)V
+  #365 = Utf8               Unknown resample method:
+  #366 = Class              #491          // java/time/temporal/ChronoUnit
+  #367 = NameAndType        #492:#493     // MILLIS:Ljava/time/temporal/ChronoUnit;
+  #368 = Class              #427          // java/time/ZonedDateTime
+  #369 = NameAndType        #494:#495     // plus:(JLjava/time/temporal/TemporalUnit;)Ljava/time/ZonedDateTime;
+  #370 = Class              #421          // java/time/format/DateTimeFormatter
+  #371 = NameAndType        #496:#497     // format:(Ljava/time/temporal/TemporalAccessor;)Ljava/lang/String;
+  #372 = NameAndType        #496:#498     // format:(D)Ljava/lang/String;
+  #373 = NameAndType        #249:#251     // toNanos:(Ljava/time/ZonedDateTime;)J
+  #374 = NameAndType        #236:#237     // writeNpyLine:(LNpyWriter;JDDD)V
+  #375 = NameAndType        #499:#500     // getAccStats:([D[D[DLFilter;Ljava/lang/Boolean;I)[D
+  #376 = NameAndType        #501:#502     // countStuckVals:([D[D[D)I
+  #377 = NameAndType        #503:#504     // mean:(Ljava/util/List;)D
+  #378 = Utf8               \n
+  #379 = NameAndType        #505:#436     // write:(Ljava/lang/String;)V
+  #380 = Utf8               line write error:
+  #381 = NameAndType        #506:#507     // isNaN:(D)Z
+  #382 = Utf8               NaN at
+  #383 = NameAndType        #446:#508     // append:(J)Ljava/lang/StringBuilder;
+  #384 = Class              #509          // java/lang/Float
+  #385 = NameAndType        #448:#510     // valueOf:(F)Ljava/lang/Float;
+  #386 = NameAndType        #511:#512     // writeData:(JLjava/lang/Float;Ljava/lang/Float;Ljava/lang/Float;)V
+  #387 = Utf8               java/io/IOException
+  #388 = NameAndType        #513:#514     // printStackTrace:(Ljava/io/PrintStream;)V
+  #389 = Utf8               error closing file writer:
+  #390 = Utf8               java/util/Date
+  #391 = NameAndType        #209:#515     // "<init>":(J)V
+  #392 = NameAndType        #516:#517     // toInstant:()Ljava/time/Instant;
+  #393 = Class              #518          // java/time/ZoneOffset
+  #394 = NameAndType        #397:#519     // UTC:Ljava/time/ZoneOffset;
+  #395 = Class              #520          // java/time/LocalDateTime
+  #396 = NameAndType        #521:#522     // ofInstant:(Ljava/time/Instant;Ljava/time/ZoneId;)Ljava/time/LocalDateTime;
+  #397 = Utf8               UTC
+  #398 = NameAndType        #523:#524     // atZone:(Ljava/time/ZoneId;)Ljava/time/ZonedDateTime;
+  #399 = Class              #525          // java/time/Instant
+  #400 = NameAndType        #526:#527     // toEpochMilli:()J
+  #401 = NameAndType        #528:#246     // ofEpochMilli:(J)Ljava/time/Instant;
+  #402 = NameAndType        #245:#246     // millisToInstant:(J)Ljava/time/Instant;
+  #403 = Class              #529          // java/util/concurrent/TimeUnit
+  #404 = NameAndType        #530:#531     // SECONDS:Ljava/util/concurrent/TimeUnit;
+  #405 = NameAndType        #532:#527     // getEpochSecond:()J
+  #406 = NameAndType        #249:#533     // toNanos:(J)J
+  #407 = NameAndType        #534:#464     // getNano:()I
+  #408 = NameAndType        #249:#250     // toNanos:(Ljava/time/Instant;)J
+  #409 = Utf8               java/text/DecimalFormatSymbols
+  #410 = Class              #535          // java/util/Locale
+  #411 = NameAndType        #536:#537     // ENGLISH:Ljava/util/Locale;
+  #412 = NameAndType        #209:#538     // "<init>":(Ljava/util/Locale;)V
+  #413 = Utf8               java/text/DecimalFormat
+  #414 = Utf8               0.000000
+  #415 = NameAndType        #209:#539     // "<init>":(Ljava/lang/String;Ljava/text/DecimalFormatSymbols;)V
+  #416 = Utf8               0.000
+  #417 = Utf8               0.00
+  #418 = Utf8               java/lang/Object
+  #419 = Utf8               java/io/BufferedWriter
+  #420 = Utf8               NpyWriter
+  #421 = Utf8               java/time/format/DateTimeFormatter
+  #422 = Utf8               java/lang/String
+  #423 = Utf8               java/lang/Boolean
+  #424 = Utf8               Filter
+  #425 = Utf8               [I
+  #426 = Utf8               java/io/PrintStream
+  #427 = Utf8               java/time/ZonedDateTime
+  #428 = Utf8               java/util/List
+  #429 = Utf8               [J
+  #430 = Utf8               booleanValue
+  #431 = Utf8               ()Z
+  #432 = Utf8               java/time/ZoneId
+  #433 = Utf8               of
+  #434 = Utf8               (Ljava/lang/String;)Ljava/time/ZoneId;
+  #435 = Utf8               setNaN
+  #436 = Utf8               (Ljava/lang/String;)V
+  #437 = Utf8               setInfinity
+  #438 = Utf8               setDecimalFormatSymbols
+  #439 = Utf8               (Ljava/text/DecimalFormatSymbols;)V
+  #440 = Utf8               java/math/RoundingMode
+  #441 = Utf8               CEILING
+  #442 = Utf8               Ljava/math/RoundingMode;
+  #443 = Utf8               setRoundingMode
+  #444 = Utf8               (Ljava/math/RoundingMode;)V
+  #445 = Utf8               HALF_UP
+  #446 = Utf8               append
+  #447 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #448 = Utf8               valueOf
+  #449 = Utf8               (Z)Ljava/lang/Boolean;
+  #450 = Utf8               AccStats
+  #451 = Utf8               getStatsHeader
+  #452 = Utf8               (Ljava/lang/Boolean;)Ljava/lang/String;
+  #453 = Utf8               toString
+  #454 = Utf8               ()Ljava/lang/String;
+  #455 = Utf8               java/lang/System
+  #456 = Utf8               out
+  #457 = Utf8               Ljava/io/PrintStream;
+  #458 = Utf8               (I)Ljava/lang/StringBuilder;
+  #459 = Utf8               (Ljava/lang/Object;)Ljava/lang/StringBuilder;
+  #460 = Utf8               println
+  #461 = Utf8               err
+  #462 = Utf8               (D)Ljava/lang/StringBuilder;
+  #463 = Utf8               size
+  #464 = Utf8               ()I
+  #465 = Utf8               clear
+  #466 = Utf8               java/lang/Long
+  #467 = Utf8               (J)Ljava/lang/Long;
+  #468 = Utf8               add
+  #469 = Utf8               (Ljava/lang/Object;)Z
+  #470 = Utf8               (D)Ljava/lang/Double;
+  #471 = Utf8               close
+  #472 = Utf8               exit
+  #473 = Utf8               (I)V
+  #474 = Utf8               get
+  #475 = Utf8               (I)Ljava/lang/Object;
+  #476 = Utf8               doubleValue
+  #477 = Utf8               ()D
+  #478 = Utf8               java/lang/Math
+  #479 = Utf8               abs
+  #480 = Utf8               (D)D
+  #481 = Utf8               set
+  #482 = Utf8               (ILjava/lang/Object;)Ljava/lang/Object;
+  #483 = Utf8               round
+  #484 = Utf8               (D)J
+  #485 = Utf8               equalsIgnoreCase
+  #486 = Utf8               (Ljava/lang/String;)Z
+  #487 = Utf8               Resample
+  #488 = Utf8               interpLinear
+  #489 = Utf8               (Ljava/util/List;Ljava/util/List;Ljava/util/List;Ljava/util/List;[J[D[D[D)V
+  #490 = Utf8               interpNearest
+  #491 = Utf8               java/time/temporal/ChronoUnit
+  #492 = Utf8               MILLIS
+  #493 = Utf8               Ljava/time/temporal/ChronoUnit;
+  #494 = Utf8               plus
+  #495 = Utf8               (JLjava/time/temporal/TemporalUnit;)Ljava/time/ZonedDateTime;
+  #496 = Utf8               format
+  #497 = Utf8               (Ljava/time/temporal/TemporalAccessor;)Ljava/lang/String;
+  #498 = Utf8               (D)Ljava/lang/String;
+  #499 = Utf8               getAccStats
+  #500 = Utf8               ([D[D[DLFilter;Ljava/lang/Boolean;I)[D
+  #501 = Utf8               countStuckVals
+  #502 = Utf8               ([D[D[D)I
+  #503 = Utf8               mean
+  #504 = Utf8               (Ljava/util/List;)D
+  #505 = Utf8               write
+  #506 = Utf8               isNaN
+  #507 = Utf8               (D)Z
+  #508 = Utf8               (J)Ljava/lang/StringBuilder;
+  #509 = Utf8               java/lang/Float
+  #510 = Utf8               (F)Ljava/lang/Float;
+  #511 = Utf8               writeData
+  #512 = Utf8               (JLjava/lang/Float;Ljava/lang/Float;Ljava/lang/Float;)V
+  #513 = Utf8               printStackTrace
+  #514 = Utf8               (Ljava/io/PrintStream;)V
+  #515 = Utf8               (J)V
+  #516 = Utf8               toInstant
+  #517 = Utf8               ()Ljava/time/Instant;
+  #518 = Utf8               java/time/ZoneOffset
+  #519 = Utf8               Ljava/time/ZoneOffset;
+  #520 = Utf8               java/time/LocalDateTime
+  #521 = Utf8               ofInstant
+  #522 = Utf8               (Ljava/time/Instant;Ljava/time/ZoneId;)Ljava/time/LocalDateTime;
+  #523 = Utf8               atZone
+  #524 = Utf8               (Ljava/time/ZoneId;)Ljava/time/ZonedDateTime;
+  #525 = Utf8               java/time/Instant
+  #526 = Utf8               toEpochMilli
+  #527 = Utf8               ()J
+  #528 = Utf8               ofEpochMilli
+  #529 = Utf8               java/util/concurrent/TimeUnit
+  #530 = Utf8               SECONDS
+  #531 = Utf8               Ljava/util/concurrent/TimeUnit;
+  #532 = Utf8               getEpochSecond
+  #533 = Utf8               (J)J
+  #534 = Utf8               getNano
+  #535 = Utf8               java/util/Locale
+  #536 = Utf8               ENGLISH
+  #537 = Utf8               Ljava/util/Locale;
+  #538 = Utf8               (Ljava/util/Locale;)V
+  #539 = Utf8               (Ljava/lang/String;Ljava/text/DecimalFormatSymbols;)V
 {
   private static final java.text.DecimalFormatSymbols decimalFormatSymbol;
     descriptor: Ljava/text/DecimalFormatSymbols;
     flags: (0x001a) ACC_PRIVATE, ACC_STATIC, ACC_FINAL
 
   private static java.text.DecimalFormat DF6;
     descriptor: Ljava/text/DecimalFormat;
@@ -1410,15 +1422,14 @@
         line 147: 44
         line 150: 52
         line 151: 60
         line 152: 63
         line 153: 82
         line 154: 100
         line 156: 106
-        line 157: 121
         line 158: 169
         line 156: 178
         line 162: 181
         line 163: 201
         line 164: 209
         line 167: 211
         line 168: 243
@@ -2275,15 +2286,15 @@
           locals = [ class "[D", class java/lang/String, int ]
         frame_type = 250 /* chop */
           offset_delta = 49
         frame_type = 254 /* append */
           offset_delta = 205
           locals = [ double, double, double ]
         frame_type = 8 /* same */
-    Signature: #230                         // (Ljava/time/ZonedDateTime;Ljava/util/List<Ljava/lang/Long;>;Ljava/util/List<Ljava/lang/Double;>;Ljava/util/List<Ljava/lang/Double;>;Ljava/util/List<Ljava/lang/Double;>;Ljava/util/List<Ljava/lang/Double;>;[I)V
+    Signature: #233                         // (Ljava/time/ZonedDateTime;Ljava/util/List<Ljava/lang/Long;>;Ljava/util/List<Ljava/lang/Double;>;Ljava/util/List<Ljava/lang/Double;>;Ljava/util/List<Ljava/lang/Double;>;Ljava/util/List<Ljava/lang/Double;>;[I)V
 
   private static void writeLine(java.io.BufferedWriter, java.lang.String);
     descriptor: (Ljava/io/BufferedWriter;Ljava/lang/String;)V
     flags: (0x000a) ACC_PRIVATE, ACC_STATIC
     Code:
       stack=3, locals=3, args_size=2
          0: aload_0
```

### Comparing `accelerometer-6.2.3/accelerometer/java/EpochWriter.java` & `accelerometer-7.0.0.dev0/src/accelerometer/java/EpochWriter.java`

 * *Files identical despite different names*

### Comparing `accelerometer-6.2.3/accelerometer/java/Features.class` & `accelerometer-7.0.0.dev0/src/accelerometer/java/Features.class`

 * *Files 7% similar despite different names*

#### javap -verbose -constants -s -l -private {}

```diff
@@ -1,274 +1,276 @@
-  SHA-256 checksum 18b7c8552e77121330627e0f05365dae9246c1911385afe96e576fdb840977d9
+  SHA-256 checksum 9e8e03fab2cb91cd328fd35e03d4b2c3a1693e1772bca1c7933a99688067cde7
   Compiled from "Features.java"
 public class Features
   minor version: 0
   major version: 52
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #110                        // Features
   super_class: #111                       // java/lang/Object
   interfaces: 0, fields: 0, methods: 24, attributes: 1
 Constant pool:
-    #1 = Methodref          #111.#151     // java/lang/Object."<init>":()V
-    #2 = Methodref          #110.#152     // Features.calculateSanDiegoFeatures:([D[D[DI)[D
-    #3 = Methodref          #110.#153     // Features.calculateMADFeatures:([D[D[D)[D
-    #4 = Methodref          #110.#154     // Features.calculateArmFeatures:([D[D[DI)[D
-    #5 = Methodref          #110.#155     // Features.unileverFeatures:([DI)[D
-    #6 = Methodref          #156.#157     // AccStats.combineArrays:([D[D)[D
-    #7 = Methodref          #110.#158     // Features.getSanDiegoFeaturesHeader:()Ljava/lang/String;
-    #8 = Class              #159          // java/lang/StringBuilder
-    #9 = Methodref          #8.#151       // java/lang/StringBuilder."<init>":()V
-   #10 = Methodref          #8.#160       // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-   #11 = String             #161          // ,
-   #12 = Methodref          #110.#162     // Features.getMADFeaturesHeader:()Ljava/lang/String;
-   #13 = Methodref          #8.#163       // java/lang/StringBuilder.toString:()Ljava/lang/String;
-   #14 = Methodref          #110.#164     // Features.getArmFeaturesHeader:()Ljava/lang/String;
-   #15 = Methodref          #110.#165     // Features.getUnileverFeaturesHeader:()Ljava/lang/String;
-   #16 = Methodref          #110.#166     // Features.sanDiegoGetAvgGravity:([D[D[DI)[D
-   #17 = Methodref          #156.#167     // AccStats.getVectorMagnitude:(DDD)D
-   #18 = Methodref          #156.#168     // AccStats.mean:([D)D
-   #19 = Methodref          #156.#169     // AccStats.stdR:([DD)D
+    #1 = Methodref          #111.#152     // java/lang/Object."<init>":()V
+    #2 = Methodref          #110.#153     // Features.calculateSanDiegoFeatures:([D[D[DI)[D
+    #3 = Methodref          #110.#154     // Features.calculateMADFeatures:([D[D[D)[D
+    #4 = Methodref          #110.#155     // Features.calculateArmFeatures:([D[D[DI)[D
+    #5 = Methodref          #110.#156     // Features.unileverFeatures:([DI)[D
+    #6 = Methodref          #157.#158     // AccStats.combineArrays:([D[D)[D
+    #7 = Methodref          #110.#159     // Features.getSanDiegoFeaturesHeader:()Ljava/lang/String;
+    #8 = Class              #160          // java/lang/StringBuilder
+    #9 = Methodref          #8.#152       // java/lang/StringBuilder."<init>":()V
+   #10 = Methodref          #8.#161       // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+   #11 = String             #162          // ,
+   #12 = Methodref          #110.#163     // Features.getMADFeaturesHeader:()Ljava/lang/String;
+   #13 = Methodref          #8.#164       // java/lang/StringBuilder.toString:()Ljava/lang/String;
+   #14 = Methodref          #110.#165     // Features.getArmFeaturesHeader:()Ljava/lang/String;
+   #15 = Methodref          #110.#166     // Features.getUnileverFeaturesHeader:()Ljava/lang/String;
+   #16 = Methodref          #110.#167     // Features.sanDiegoGetAvgGravity:([D[D[DI)[D
+   #17 = Methodref          #157.#168     // AccStats.getVectorMagnitude:(DDD)D
+   #18 = Methodref          #157.#169     // AccStats.mean:([D)D
+   #19 = Methodref          #157.#170     // AccStats.stdR:([DD)D
    #20 = Double             0.25d
    #22 = Double             0.5d
    #24 = Double             0.75d
-   #26 = Methodref          #156.#170     // AccStats.percentiles:([D[D)[D
-   #27 = Methodref          #110.#171     // Features.correlation:([D[DI)D
-   #28 = Methodref          #110.#172     // Features.correlation:([D[D)D
-   #29 = Methodref          #156.#173     // AccStats.angleAvgStd:([D[D)[D
-   #30 = Methodref          #71.#174      // java/lang/Math.atan2:(DD)D
-   #31 = Methodref          #110.#175     // Features.sanDiegoFFT:([DI)[D
-   #32 = String             #176          // mean,sd,coefvariation
-   #33 = String             #177          // ,median,min,max,25thp,75thp
-   #34 = String             #178          // ,autocorr,corrxy,corrxz,corryz
-   #35 = String             #179          // ,avgroll,avgpitch,avgyaw
-   #36 = String             #180          // ,sdroll,sdpitch,sdyaw
-   #37 = String             #181          // ,rollg,pitchg,yawg
-   #38 = Methodref          #110.#182     // Features.getSanDiegoFFTHeader:()Ljava/lang/String;
+   #26 = Methodref          #157.#171     // AccStats.percentiles:([D[D)[D
+   #27 = Methodref          #110.#172     // Features.correlation:([D[DI)D
+   #28 = Methodref          #110.#173     // Features.correlation:([D[D)D
+   #29 = Methodref          #157.#174     // AccStats.angleAvgStd:([D[D)[D
+   #30 = Methodref          #71.#175      // java/lang/Math.atan2:(DD)D
+   #31 = Methodref          #110.#176     // Features.sanDiegoFFT:([DI)[D
+   #32 = String             #177          // mean,sd,coefvariation
+   #33 = String             #178          // ,median,min,max,25thp,75thp
+   #34 = String             #179          // ,autocorr,corrxy,corrxz,corryz
+   #35 = String             #180          // ,avgroll,avgpitch,avgyaw
+   #36 = String             #181          // ,sdroll,sdpitch,sdyaw
+   #37 = String             #182          // ,rollg,pitchg,yawg
+   #38 = Methodref          #110.#183     // Features.getSanDiegoFFTHeader:()Ljava/lang/String;
    #39 = Double             0.9d
-   #41 = Methodref          #110.#183     // Features.HanningWindow:([DI)[D
-   #42 = Class              #184          // org/jtransforms/fft/DoubleFFT_1D
-   #43 = Methodref          #42.#185      // org/jtransforms/fft/DoubleFFT_1D."<init>":(J)V
-   #44 = Methodref          #42.#186      // org/jtransforms/fft/DoubleFFT_1D.realForward:([D)V
-   #45 = Methodref          #110.#187     // Features.getFFTpower:([D)[D
-   #46 = Methodref          #156.#188     // AccStats.sum:([D)D
+   #41 = Methodref          #110.#184     // Features.HanningWindow:([DI)[D
+   #42 = Class              #185          // org/jtransforms/fft/DoubleFFT_1D
+   #43 = Methodref          #42.#186      // org/jtransforms/fft/DoubleFFT_1D."<init>":(J)V
+   #44 = Methodref          #42.#187      // org/jtransforms/fft/DoubleFFT_1D.realForward:([D)V
+   #45 = Methodref          #110.#188     // Features.getFFTpower:([D)[D
+   #46 = Methodref          #157.#189     // AccStats.sum:([D)D
    #47 = Double             1.0E-8d
-   #49 = Methodref          #71.#189      // java/lang/Math.log:(D)D
+   #49 = Methodref          #71.#190      // java/lang/Math.log:(D)D
    #50 = Double             -1.0d
    #52 = Double             0.3d
    #54 = Double             3.0d
-   #56 = Methodref          #110.#190     // Features.getFFTmagnitude:([D)[D
-   #57 = String             #191          // fmax,pmax,fmaxband,pmaxband,entropy
-   #58 = String             #192          // ,fft
-   #59 = Methodref          #8.#193       // java/lang/StringBuilder.append:(I)Ljava/lang/StringBuilder;
-   #60 = Methodref          #101.#194     // java/lang/Double.isNaN:(D)Z
-   #61 = Methodref          #156.#195     // AccStats.std:([DD)D
-   #62 = Methodref          #71.#196      // java/lang/Math.abs:(D)D
+   #56 = Methodref          #110.#191     // Features.getFFTmagnitude:([D)[D
+   #57 = String             #192          // fmax,pmax,fmaxband,pmaxband,entropy
+   #58 = String             #193          // ,fft
+   #59 = Methodref          #8.#194       // java/lang/StringBuilder.append:(I)Ljava/lang/StringBuilder;
+   #60 = Methodref          #101.#195     // java/lang/Double.isNaN:(D)Z
+   #61 = Methodref          #157.#196     // AccStats.std:([DD)D
+   #62 = Methodref          #71.#197      // java/lang/Math.abs:(D)D
    #63 = Double             1.5d
-   #65 = Methodref          #71.#197      // java/lang/Math.pow:(DD)D
+   #65 = Methodref          #71.#198      // java/lang/Math.pow:(DD)D
    #66 = Double             4.0d
    #68 = Double             2.0d
-   #70 = String             #198          // MAD,MPD,skew,kurt
-   #71 = Class              #199          // java/lang/Math
+   #70 = String             #199          // MAD,MPD,skew,kurt
+   #71 = Class              #200          // java/lang/Math
    #72 = Double             6.283185307179586d
-   #74 = Methodref          #71.#200      // java/lang/Math.cos:(D)D
-   #75 = Methodref          #110.#201     // Features.getFFTmagnitude:([DZ)[D
-   #76 = Methodref          #110.#202     // Features.getFFTpower:([DZ)[D
-   #77 = Methodref          #71.#203      // java/lang/Math.sqrt:(D)D
-   #78 = Methodref          #71.#204      // java/lang/Math.ceil:(D)D
+   #74 = Methodref          #71.#201      // java/lang/Math.cos:(D)D
+   #75 = Methodref          #110.#202     // Features.getFFTmagnitude:([DZ)[D
+   #76 = Methodref          #110.#203     // Features.getFFTpower:([DZ)[D
+   #77 = Methodref          #71.#204      // java/lang/Math.sqrt:(D)D
+   #78 = Methodref          #71.#205      // java/lang/Math.ceil:(D)D
    #79 = Double             15.0d
    #81 = Double             0.6d
    #83 = Double             2.5d
-   #85 = String             #205          // f1,p1,f2,p2,f625,p625,totalPower
-   #86 = Methodref          #110.#206     // Features.medianSlidingWindow:([DI)[D
-   #87 = Methodref          #71.#207      // java/lang/Math.atan:(D)D
+   #85 = String             #206          // f1,p1,f2,p2,f625,p625,totalPower
+   #86 = Methodref          #110.#207     // Features.medianSlidingWindow:([DI)[D
+   #87 = Methodref          #71.#208      // java/lang/Math.atan:(D)D
    #88 = Double             180.0d
    #90 = Double             3.141592653589793d
-   #92 = Methodref          #110.#208     // Features.computeFiveSecAvg:([DI)[D
-   #93 = Methodref          #110.#209     // Features.computeAbsoluteDiff:([D)[D
-   #94 = String             #210          // avgArmAngel,avgArmAngelAbsDiff
-   #95 = Class              #211          // java/util/ArrayList
-   #96 = Methodref          #95.#151      // java/util/ArrayList."<init>":()V
-   #97 = Methodref          #101.#212     // java/lang/Double.valueOf:(D)Ljava/lang/Double;
-   #98 = InterfaceMethodref #143.#213     // java/util/List.add:(Ljava/lang/Object;)Z
-   #99 = Methodref          #214.#215     // java/util/Collections.sort:(Ljava/util/List;)V
-  #100 = InterfaceMethodref #143.#216     // java/util/List.get:(I)Ljava/lang/Object;
-  #101 = Class              #217          // java/lang/Double
-  #102 = Methodref          #101.#218     // java/lang/Double.doubleValue:()D
-  #103 = Methodref          #214.#219     // java/util/Collections.binarySearch:(Ljava/util/List;Ljava/lang/Object;)I
-  #104 = InterfaceMethodref #143.#220     // java/util/List.add:(ILjava/lang/Object;)V
-  #105 = InterfaceMethodref #143.#221     // java/util/List.remove:(I)Ljava/lang/Object;
+   #92 = Methodref          #110.#209     // Features.computeFiveSecAvg:([DI)[D
+   #93 = Methodref          #110.#210     // Features.computeAbsoluteDiff:([D)[D
+   #94 = String             #211          // avgArmAngel,avgArmAngelAbsDiff
+   #95 = Class              #212          // java/util/ArrayList
+   #96 = Methodref          #95.#152      // java/util/ArrayList."<init>":()V
+   #97 = Methodref          #101.#213     // java/lang/Double.valueOf:(D)Ljava/lang/Double;
+   #98 = InterfaceMethodref #214.#215     // java/util/List.add:(Ljava/lang/Object;)Z
+   #99 = Methodref          #216.#217     // java/util/Collections.sort:(Ljava/util/List;)V
+  #100 = InterfaceMethodref #214.#218     // java/util/List.get:(I)Ljava/lang/Object;
+  #101 = Class              #219          // java/lang/Double
+  #102 = Methodref          #101.#220     // java/lang/Double.doubleValue:()D
+  #103 = Methodref          #216.#221     // java/util/Collections.binarySearch:(Ljava/util/List;Ljava/lang/Object;)I
+  #104 = InterfaceMethodref #214.#222     // java/util/List.add:(ILjava/lang/Object;)V
+  #105 = InterfaceMethodref #214.#223     // java/util/List.remove:(I)Ljava/lang/Object;
   #106 = Double             5.0d
-  #108 = Methodref          #156.#171     // AccStats.correlation:([D[DI)D
-  #109 = Methodref          #101.#222     // java/lang/Double.isFinite:(D)Z
-  #110 = Class              #223          // Features
-  #111 = Class              #224          // java/lang/Object
+  #108 = Methodref          #157.#172     // AccStats.correlation:([D[DI)D
+  #109 = Methodref          #101.#224     // java/lang/Double.isFinite:(D)Z
+  #110 = Class              #225          // Features
+  #111 = Class              #226          // java/lang/Object
   #112 = Utf8               <init>
   #113 = Utf8               ()V
   #114 = Utf8               Code
   #115 = Utf8               LineNumberTable
   #116 = Utf8               getFeatures
   #117 = Utf8               ([D[D[D[DI)[D
   #118 = Utf8               getFeaturesHeader
   #119 = Utf8               ()Ljava/lang/String;
   #120 = Utf8               calculateSanDiegoFeatures
   #121 = Utf8               ([D[D[DI)[D
   #122 = Utf8               StackMapTable
-  #123 = Class              #225          // "[D"
+  #123 = Class              #227          // "[D"
   #124 = Utf8               getSanDiegoFeaturesHeader
   #125 = Utf8               sanDiegoGetAvgGravity
   #126 = Utf8               sanDiegoFFT
   #127 = Utf8               ([DI)[D
-  #128 = Utf8               getSanDiegoFFTHeader
-  #129 = Class              #226          // java/lang/String
-  #130 = Utf8               calculateMADFeatures
-  #131 = Utf8               ([D[D[D)[D
-  #132 = Utf8               getMADFeaturesHeader
-  #133 = Utf8               HanningWindow
-  #134 = Utf8               getFFTmagnitude
-  #135 = Utf8               ([D)[D
-  #136 = Utf8               ([DZ)[D
-  #137 = Utf8               getFFTpower
-  #138 = Utf8               unileverFeatures
-  #139 = Utf8               getUnileverFeaturesHeader
-  #140 = Utf8               calculateArmFeatures
-  #141 = Utf8               getArmFeaturesHeader
-  #142 = Utf8               medianSlidingWindow
-  #143 = Class              #227          // java/util/List
-  #144 = Utf8               computeFiveSecAvg
-  #145 = Utf8               computeAbsoluteDiff
-  #146 = Utf8               correlation
-  #147 = Utf8               ([D[DI)D
-  #148 = Utf8               ([D[D)D
-  #149 = Utf8               SourceFile
-  #150 = Utf8               Features.java
-  #151 = NameAndType        #112:#113     // "<init>":()V
-  #152 = NameAndType        #120:#121     // calculateSanDiegoFeatures:([D[D[DI)[D
-  #153 = NameAndType        #130:#131     // calculateMADFeatures:([D[D[D)[D
-  #154 = NameAndType        #140:#121     // calculateArmFeatures:([D[D[DI)[D
-  #155 = NameAndType        #138:#127     // unileverFeatures:([DI)[D
-  #156 = Class              #228          // AccStats
-  #157 = NameAndType        #229:#230     // combineArrays:([D[D)[D
-  #158 = NameAndType        #124:#119     // getSanDiegoFeaturesHeader:()Ljava/lang/String;
-  #159 = Utf8               java/lang/StringBuilder
-  #160 = NameAndType        #231:#232     // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #161 = Utf8               ,
-  #162 = NameAndType        #132:#119     // getMADFeaturesHeader:()Ljava/lang/String;
-  #163 = NameAndType        #233:#119     // toString:()Ljava/lang/String;
-  #164 = NameAndType        #141:#119     // getArmFeaturesHeader:()Ljava/lang/String;
-  #165 = NameAndType        #139:#119     // getUnileverFeaturesHeader:()Ljava/lang/String;
-  #166 = NameAndType        #125:#121     // sanDiegoGetAvgGravity:([D[D[DI)[D
-  #167 = NameAndType        #234:#235     // getVectorMagnitude:(DDD)D
-  #168 = NameAndType        #236:#237     // mean:([D)D
-  #169 = NameAndType        #238:#239     // stdR:([DD)D
-  #170 = NameAndType        #240:#230     // percentiles:([D[D)[D
-  #171 = NameAndType        #146:#147     // correlation:([D[DI)D
-  #172 = NameAndType        #146:#148     // correlation:([D[D)D
-  #173 = NameAndType        #241:#230     // angleAvgStd:([D[D)[D
-  #174 = NameAndType        #242:#243     // atan2:(DD)D
-  #175 = NameAndType        #126:#127     // sanDiegoFFT:([DI)[D
-  #176 = Utf8               mean,sd,coefvariation
-  #177 = Utf8               ,median,min,max,25thp,75thp
-  #178 = Utf8               ,autocorr,corrxy,corrxz,corryz
-  #179 = Utf8               ,avgroll,avgpitch,avgyaw
-  #180 = Utf8               ,sdroll,sdpitch,sdyaw
-  #181 = Utf8               ,rollg,pitchg,yawg
-  #182 = NameAndType        #128:#119     // getSanDiegoFFTHeader:()Ljava/lang/String;
-  #183 = NameAndType        #133:#127     // HanningWindow:([DI)[D
-  #184 = Utf8               org/jtransforms/fft/DoubleFFT_1D
-  #185 = NameAndType        #112:#244     // "<init>":(J)V
-  #186 = NameAndType        #245:#246     // realForward:([D)V
-  #187 = NameAndType        #137:#135     // getFFTpower:([D)[D
-  #188 = NameAndType        #247:#237     // sum:([D)D
-  #189 = NameAndType        #248:#249     // log:(D)D
-  #190 = NameAndType        #134:#135     // getFFTmagnitude:([D)[D
-  #191 = Utf8               fmax,pmax,fmaxband,pmaxband,entropy
-  #192 = Utf8               ,fft
-  #193 = NameAndType        #231:#250     // append:(I)Ljava/lang/StringBuilder;
-  #194 = NameAndType        #251:#252     // isNaN:(D)Z
-  #195 = NameAndType        #253:#239     // std:([DD)D
-  #196 = NameAndType        #254:#249     // abs:(D)D
-  #197 = NameAndType        #255:#243     // pow:(DD)D
-  #198 = Utf8               MAD,MPD,skew,kurt
-  #199 = Utf8               java/lang/Math
-  #200 = NameAndType        #256:#249     // cos:(D)D
-  #201 = NameAndType        #134:#136     // getFFTmagnitude:([DZ)[D
-  #202 = NameAndType        #137:#136     // getFFTpower:([DZ)[D
-  #203 = NameAndType        #257:#249     // sqrt:(D)D
-  #204 = NameAndType        #258:#249     // ceil:(D)D
-  #205 = Utf8               f1,p1,f2,p2,f625,p625,totalPower
-  #206 = NameAndType        #142:#127     // medianSlidingWindow:([DI)[D
-  #207 = NameAndType        #259:#249     // atan:(D)D
-  #208 = NameAndType        #144:#127     // computeFiveSecAvg:([DI)[D
-  #209 = NameAndType        #145:#135     // computeAbsoluteDiff:([D)[D
-  #210 = Utf8               avgArmAngel,avgArmAngelAbsDiff
-  #211 = Utf8               java/util/ArrayList
-  #212 = NameAndType        #260:#261     // valueOf:(D)Ljava/lang/Double;
-  #213 = NameAndType        #262:#263     // add:(Ljava/lang/Object;)Z
-  #214 = Class              #264          // java/util/Collections
-  #215 = NameAndType        #265:#266     // sort:(Ljava/util/List;)V
-  #216 = NameAndType        #267:#268     // get:(I)Ljava/lang/Object;
-  #217 = Utf8               java/lang/Double
-  #218 = NameAndType        #269:#270     // doubleValue:()D
-  #219 = NameAndType        #271:#272     // binarySearch:(Ljava/util/List;Ljava/lang/Object;)I
-  #220 = NameAndType        #262:#273     // add:(ILjava/lang/Object;)V
-  #221 = NameAndType        #274:#268     // remove:(I)Ljava/lang/Object;
-  #222 = NameAndType        #275:#252     // isFinite:(D)Z
-  #223 = Utf8               Features
-  #224 = Utf8               java/lang/Object
-  #225 = Utf8               [D
-  #226 = Utf8               java/lang/String
-  #227 = Utf8               java/util/List
-  #228 = Utf8               AccStats
-  #229 = Utf8               combineArrays
-  #230 = Utf8               ([D[D)[D
-  #231 = Utf8               append
-  #232 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #233 = Utf8               toString
-  #234 = Utf8               getVectorMagnitude
-  #235 = Utf8               (DDD)D
-  #236 = Utf8               mean
-  #237 = Utf8               ([D)D
-  #238 = Utf8               stdR
-  #239 = Utf8               ([DD)D
-  #240 = Utf8               percentiles
-  #241 = Utf8               angleAvgStd
-  #242 = Utf8               atan2
-  #243 = Utf8               (DD)D
-  #244 = Utf8               (J)V
-  #245 = Utf8               realForward
-  #246 = Utf8               ([D)V
-  #247 = Utf8               sum
-  #248 = Utf8               log
-  #249 = Utf8               (D)D
-  #250 = Utf8               (I)Ljava/lang/StringBuilder;
-  #251 = Utf8               isNaN
-  #252 = Utf8               (D)Z
-  #253 = Utf8               std
-  #254 = Utf8               abs
-  #255 = Utf8               pow
-  #256 = Utf8               cos
-  #257 = Utf8               sqrt
-  #258 = Utf8               ceil
-  #259 = Utf8               atan
-  #260 = Utf8               valueOf
-  #261 = Utf8               (D)Ljava/lang/Double;
-  #262 = Utf8               add
-  #263 = Utf8               (Ljava/lang/Object;)Z
-  #264 = Utf8               java/util/Collections
-  #265 = Utf8               sort
-  #266 = Utf8               (Ljava/util/List;)V
-  #267 = Utf8               get
-  #268 = Utf8               (I)Ljava/lang/Object;
-  #269 = Utf8               doubleValue
-  #270 = Utf8               ()D
-  #271 = Utf8               binarySearch
-  #272 = Utf8               (Ljava/util/List;Ljava/lang/Object;)I
-  #273 = Utf8               (ILjava/lang/Object;)V
-  #274 = Utf8               remove
-  #275 = Utf8               isFinite
+  #128 = Class              #185          // org/jtransforms/fft/DoubleFFT_1D
+  #129 = Utf8               getSanDiegoFFTHeader
+  #130 = Class              #228          // java/lang/String
+  #131 = Utf8               calculateMADFeatures
+  #132 = Utf8               ([D[D[D)[D
+  #133 = Utf8               getMADFeaturesHeader
+  #134 = Utf8               HanningWindow
+  #135 = Utf8               getFFTmagnitude
+  #136 = Utf8               ([D)[D
+  #137 = Utf8               ([DZ)[D
+  #138 = Utf8               getFFTpower
+  #139 = Utf8               unileverFeatures
+  #140 = Utf8               getUnileverFeaturesHeader
+  #141 = Utf8               calculateArmFeatures
+  #142 = Utf8               getArmFeaturesHeader
+  #143 = Utf8               medianSlidingWindow
+  #144 = Class              #229          // java/util/List
+  #145 = Utf8               computeFiveSecAvg
+  #146 = Utf8               computeAbsoluteDiff
+  #147 = Utf8               correlation
+  #148 = Utf8               ([D[DI)D
+  #149 = Utf8               ([D[D)D
+  #150 = Utf8               SourceFile
+  #151 = Utf8               Features.java
+  #152 = NameAndType        #112:#113     // "<init>":()V
+  #153 = NameAndType        #120:#121     // calculateSanDiegoFeatures:([D[D[DI)[D
+  #154 = NameAndType        #131:#132     // calculateMADFeatures:([D[D[D)[D
+  #155 = NameAndType        #141:#121     // calculateArmFeatures:([D[D[DI)[D
+  #156 = NameAndType        #139:#127     // unileverFeatures:([DI)[D
+  #157 = Class              #230          // AccStats
+  #158 = NameAndType        #231:#232     // combineArrays:([D[D)[D
+  #159 = NameAndType        #124:#119     // getSanDiegoFeaturesHeader:()Ljava/lang/String;
+  #160 = Utf8               java/lang/StringBuilder
+  #161 = NameAndType        #233:#234     // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #162 = Utf8               ,
+  #163 = NameAndType        #133:#119     // getMADFeaturesHeader:()Ljava/lang/String;
+  #164 = NameAndType        #235:#119     // toString:()Ljava/lang/String;
+  #165 = NameAndType        #142:#119     // getArmFeaturesHeader:()Ljava/lang/String;
+  #166 = NameAndType        #140:#119     // getUnileverFeaturesHeader:()Ljava/lang/String;
+  #167 = NameAndType        #125:#121     // sanDiegoGetAvgGravity:([D[D[DI)[D
+  #168 = NameAndType        #236:#237     // getVectorMagnitude:(DDD)D
+  #169 = NameAndType        #238:#239     // mean:([D)D
+  #170 = NameAndType        #240:#241     // stdR:([DD)D
+  #171 = NameAndType        #242:#232     // percentiles:([D[D)[D
+  #172 = NameAndType        #147:#148     // correlation:([D[DI)D
+  #173 = NameAndType        #147:#149     // correlation:([D[D)D
+  #174 = NameAndType        #243:#232     // angleAvgStd:([D[D)[D
+  #175 = NameAndType        #244:#245     // atan2:(DD)D
+  #176 = NameAndType        #126:#127     // sanDiegoFFT:([DI)[D
+  #177 = Utf8               mean,sd,coefvariation
+  #178 = Utf8               ,median,min,max,25thp,75thp
+  #179 = Utf8               ,autocorr,corrxy,corrxz,corryz
+  #180 = Utf8               ,avgroll,avgpitch,avgyaw
+  #181 = Utf8               ,sdroll,sdpitch,sdyaw
+  #182 = Utf8               ,rollg,pitchg,yawg
+  #183 = NameAndType        #129:#119     // getSanDiegoFFTHeader:()Ljava/lang/String;
+  #184 = NameAndType        #134:#127     // HanningWindow:([DI)[D
+  #185 = Utf8               org/jtransforms/fft/DoubleFFT_1D
+  #186 = NameAndType        #112:#246     // "<init>":(J)V
+  #187 = NameAndType        #247:#248     // realForward:([D)V
+  #188 = NameAndType        #138:#136     // getFFTpower:([D)[D
+  #189 = NameAndType        #249:#239     // sum:([D)D
+  #190 = NameAndType        #250:#251     // log:(D)D
+  #191 = NameAndType        #135:#136     // getFFTmagnitude:([D)[D
+  #192 = Utf8               fmax,pmax,fmaxband,pmaxband,entropy
+  #193 = Utf8               ,fft
+  #194 = NameAndType        #233:#252     // append:(I)Ljava/lang/StringBuilder;
+  #195 = NameAndType        #253:#254     // isNaN:(D)Z
+  #196 = NameAndType        #255:#241     // std:([DD)D
+  #197 = NameAndType        #256:#251     // abs:(D)D
+  #198 = NameAndType        #257:#245     // pow:(DD)D
+  #199 = Utf8               MAD,MPD,skew,kurt
+  #200 = Utf8               java/lang/Math
+  #201 = NameAndType        #258:#251     // cos:(D)D
+  #202 = NameAndType        #135:#137     // getFFTmagnitude:([DZ)[D
+  #203 = NameAndType        #138:#137     // getFFTpower:([DZ)[D
+  #204 = NameAndType        #259:#251     // sqrt:(D)D
+  #205 = NameAndType        #260:#251     // ceil:(D)D
+  #206 = Utf8               f1,p1,f2,p2,f625,p625,totalPower
+  #207 = NameAndType        #143:#127     // medianSlidingWindow:([DI)[D
+  #208 = NameAndType        #261:#251     // atan:(D)D
+  #209 = NameAndType        #145:#127     // computeFiveSecAvg:([DI)[D
+  #210 = NameAndType        #146:#136     // computeAbsoluteDiff:([D)[D
+  #211 = Utf8               avgArmAngel,avgArmAngelAbsDiff
+  #212 = Utf8               java/util/ArrayList
+  #213 = NameAndType        #262:#263     // valueOf:(D)Ljava/lang/Double;
+  #214 = Class              #229          // java/util/List
+  #215 = NameAndType        #264:#265     // add:(Ljava/lang/Object;)Z
+  #216 = Class              #266          // java/util/Collections
+  #217 = NameAndType        #267:#268     // sort:(Ljava/util/List;)V
+  #218 = NameAndType        #269:#270     // get:(I)Ljava/lang/Object;
+  #219 = Utf8               java/lang/Double
+  #220 = NameAndType        #271:#272     // doubleValue:()D
+  #221 = NameAndType        #273:#274     // binarySearch:(Ljava/util/List;Ljava/lang/Object;)I
+  #222 = NameAndType        #264:#275     // add:(ILjava/lang/Object;)V
+  #223 = NameAndType        #276:#270     // remove:(I)Ljava/lang/Object;
+  #224 = NameAndType        #277:#254     // isFinite:(D)Z
+  #225 = Utf8               Features
+  #226 = Utf8               java/lang/Object
+  #227 = Utf8               [D
+  #228 = Utf8               java/lang/String
+  #229 = Utf8               java/util/List
+  #230 = Utf8               AccStats
+  #231 = Utf8               combineArrays
+  #232 = Utf8               ([D[D)[D
+  #233 = Utf8               append
+  #234 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #235 = Utf8               toString
+  #236 = Utf8               getVectorMagnitude
+  #237 = Utf8               (DDD)D
+  #238 = Utf8               mean
+  #239 = Utf8               ([D)D
+  #240 = Utf8               stdR
+  #241 = Utf8               ([DD)D
+  #242 = Utf8               percentiles
+  #243 = Utf8               angleAvgStd
+  #244 = Utf8               atan2
+  #245 = Utf8               (DD)D
+  #246 = Utf8               (J)V
+  #247 = Utf8               realForward
+  #248 = Utf8               ([D)V
+  #249 = Utf8               sum
+  #250 = Utf8               log
+  #251 = Utf8               (D)D
+  #252 = Utf8               (I)Ljava/lang/StringBuilder;
+  #253 = Utf8               isNaN
+  #254 = Utf8               (D)Z
+  #255 = Utf8               std
+  #256 = Utf8               abs
+  #257 = Utf8               pow
+  #258 = Utf8               cos
+  #259 = Utf8               sqrt
+  #260 = Utf8               ceil
+  #261 = Utf8               atan
+  #262 = Utf8               valueOf
+  #263 = Utf8               (D)Ljava/lang/Double;
+  #264 = Utf8               add
+  #265 = Utf8               (Ljava/lang/Object;)Z
+  #266 = Utf8               java/util/Collections
+  #267 = Utf8               sort
+  #268 = Utf8               (Ljava/util/List;)V
+  #269 = Utf8               get
+  #270 = Utf8               (I)Ljava/lang/Object;
+  #271 = Utf8               doubleValue
+  #272 = Utf8               ()D
+  #273 = Utf8               binarySearch
+  #274 = Utf8               (Ljava/util/List;Ljava/lang/Object;)I
+  #275 = Utf8               (ILjava/lang/Object;)V
+  #276 = Utf8               remove
+  #277 = Utf8               isFinite
 {
   public Features();
     descriptor: ()V
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
```

### Comparing `accelerometer-6.2.3/accelerometer/java/Features.java` & `accelerometer-7.0.0.dev0/src/accelerometer/java/Features.java`

 * *Files identical despite different names*

### Comparing `accelerometer-6.2.3/accelerometer/java/Filter.class` & `accelerometer-7.0.0.dev0/src/accelerometer/java/Filter.class`

 * *Files identical despite different names*

### Comparing `accelerometer-6.2.3/accelerometer/java/Filter.java` & `accelerometer-7.0.0.dev0/src/accelerometer/java/Filter.java`

 * *Files identical despite different names*

### Comparing `accelerometer-6.2.3/accelerometer/java/GENEActivReader.class` & `accelerometer-7.0.0.dev0/src/accelerometer/java/GENEActivReader.class`

 * *Files 11% similar despite different names*

#### javap -verbose -constants -s -l -private {}

```diff
@@ -1,217 +1,224 @@
-  SHA-256 checksum 875779abfeb9b1db514c9aa1b4992c927e19aae4f1a2947b94453ff389cf98eb
+  SHA-256 checksum db274b633b8ca7c6cc78f62c2d019562db12f2de7c9a0a94e972559c14d892c6
   Compiled from "GENEActivReader.java"
 public class GENEActivReader extends DeviceReader
   minor version: 0
   major version: 52
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #55                         // GENEActivReader
   super_class: #56                        // DeviceReader
   interfaces: 0, fields: 0, methods: 4, attributes: 1
 Constant pool:
-    #1 = Methodref          #56.#77       // DeviceReader."<init>":()V
-    #2 = Methodref          #55.#78       // GENEActivReader.setTimeSettings:(Ljava/lang/String;I)V
-    #3 = Class              #79           // java/io/BufferedReader
-    #4 = Class              #80           // java/io/FileReader
-    #5 = Methodref          #4.#81        // java/io/FileReader."<init>":(Ljava/lang/String;)V
-    #6 = Methodref          #3.#82        // java/io/BufferedReader."<init>":(Ljava/io/Reader;)V
-    #7 = Methodref          #55.#83       // GENEActivReader.parseBinFileHeader:(Ljava/io/BufferedReader;II[D[I)I
-    #8 = Methodref          #69.#84       // java/time/LocalDateTime.of:(IIIIII)Ljava/time/LocalDateTime;
-    #9 = String             #85           // yyyy-MM-dd HH:mm:ss:SSS
-   #10 = Methodref          #70.#86       // java/time/format/DateTimeFormatter.ofPattern:(Ljava/lang/String;)Ljava/time/format/DateTimeFormatter;
-   #11 = Methodref          #55.#87       // GENEActivReader.readLine:(Ljava/io/BufferedReader;)Ljava/lang/String;
-   #12 = String             #88           // Time:
-   #13 = Methodref          #64.#89       // java/lang/String.split:(Ljava/lang/String;)[Ljava/lang/String;
-   #14 = Methodref          #69.#90       // java/time/LocalDateTime.parse:(Ljava/lang/CharSequence;Ljava/time/format/DateTimeFormatter;)Ljava/time/LocalDateTime;
-   #15 = Methodref          #69.#91       // java/time/LocalDateTime.plusMinutes:(J)Ljava/time/LocalDateTime;
-   #16 = Methodref          #55.#92       // GENEActivReader.setSessionStart:(Ljava/time/LocalDateTime;)V
-   #17 = Fieldref           #93.#94       // java/lang/System.out:Ljava/io/PrintStream;
-   #18 = Class              #95           // java/lang/StringBuilder
-   #19 = Methodref          #18.#77       // java/lang/StringBuilder."<init>":()V
-   #20 = String             #96           // Session start:
-   #21 = Methodref          #18.#97       // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-   #22 = Fieldref           #55.#98       // GENEActivReader.sessionStart:Ljava/time/ZonedDateTime;
-   #23 = Methodref          #18.#99       // java/lang/StringBuilder.append:(Ljava/lang/Object;)Ljava/lang/StringBuilder;
-   #24 = Methodref          #18.#100      // java/lang/StringBuilder.toString:()Ljava/lang/String;
-   #25 = Methodref          #101.#102     // java/io/PrintStream.println:(Ljava/lang/String;)V
-   #26 = String             #103          // :
-   #27 = Methodref          #104.#105     // java/lang/Double.parseDouble:(Ljava/lang/String;)D
-   #28 = Class              #106          // java/lang/Exception
-   #29 = Fieldref           #93.#107      // java/lang/System.err:Ljava/io/PrintStream;
-   #30 = Methodref          #28.#100      // java/lang/Exception.toString:()Ljava/lang/String;
-   #31 = Methodref          #64.#108      // java/lang/String.length:()I
-   #32 = Methodref          #55.#109      // GENEActivReader.getSignedIntFromHex:(Ljava/lang/String;II)I
-   #33 = String             #110          // block err @
-   #34 = Methodref          #69.#100      // java/time/LocalDateTime.toString:()Ljava/lang/String;
-   #35 = String             #111          // :
+    #1 = Methodref          #56.#79       // DeviceReader."<init>":()V
+    #2 = Methodref          #55.#80       // GENEActivReader.setTimeSettings:(Ljava/lang/String;I)V
+    #3 = Class              #81           // java/io/BufferedReader
+    #4 = Class              #82           // java/io/FileReader
+    #5 = Methodref          #4.#83        // java/io/FileReader."<init>":(Ljava/lang/String;)V
+    #6 = Methodref          #3.#84        // java/io/BufferedReader."<init>":(Ljava/io/Reader;)V
+    #7 = Methodref          #55.#85       // GENEActivReader.parseBinFileHeader:(Ljava/io/BufferedReader;II[D[I)I
+    #8 = Methodref          #86.#87       // java/time/LocalDateTime.of:(IIIIII)Ljava/time/LocalDateTime;
+    #9 = String             #88           // yyyy-MM-dd HH:mm:ss:SSS
+   #10 = Methodref          #89.#90       // java/time/format/DateTimeFormatter.ofPattern:(Ljava/lang/String;)Ljava/time/format/DateTimeFormatter;
+   #11 = Methodref          #55.#91       // GENEActivReader.readLine:(Ljava/io/BufferedReader;)Ljava/lang/String;
+   #12 = String             #92           // Time:
+   #13 = Methodref          #93.#94       // java/lang/String.split:(Ljava/lang/String;)[Ljava/lang/String;
+   #14 = Methodref          #86.#95       // java/time/LocalDateTime.parse:(Ljava/lang/CharSequence;Ljava/time/format/DateTimeFormatter;)Ljava/time/LocalDateTime;
+   #15 = Methodref          #86.#96       // java/time/LocalDateTime.plusMinutes:(J)Ljava/time/LocalDateTime;
+   #16 = Methodref          #55.#97       // GENEActivReader.setSessionStart:(Ljava/time/LocalDateTime;)V
+   #17 = Fieldref           #98.#99       // java/lang/System.out:Ljava/io/PrintStream;
+   #18 = Class              #100          // java/lang/StringBuilder
+   #19 = Methodref          #18.#79       // java/lang/StringBuilder."<init>":()V
+   #20 = String             #101          // Session start:
+   #21 = Methodref          #18.#102      // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+   #22 = Fieldref           #55.#103      // GENEActivReader.sessionStart:Ljava/time/ZonedDateTime;
+   #23 = Methodref          #18.#104      // java/lang/StringBuilder.append:(Ljava/lang/Object;)Ljava/lang/StringBuilder;
+   #24 = Methodref          #18.#105      // java/lang/StringBuilder.toString:()Ljava/lang/String;
+   #25 = Methodref          #106.#107     // java/io/PrintStream.println:(Ljava/lang/String;)V
+   #26 = String             #108          // :
+   #27 = Methodref          #109.#110     // java/lang/Double.parseDouble:(Ljava/lang/String;)D
+   #28 = Class              #111          // java/lang/Exception
+   #29 = Fieldref           #98.#112      // java/lang/System.err:Ljava/io/PrintStream;
+   #30 = Methodref          #28.#105      // java/lang/Exception.toString:()Ljava/lang/String;
+   #31 = Methodref          #93.#113      // java/lang/String.length:()I
+   #32 = Methodref          #55.#114      // GENEActivReader.getSignedIntFromHex:(Ljava/lang/String;II)I
+   #33 = String             #115          // block err @
+   #34 = Methodref          #86.#105      // java/time/LocalDateTime.toString:()Ljava/lang/String;
+   #35 = String             #116          // :
    #36 = Double             100.0d
-   #38 = Methodref          #55.#112      // GENEActivReader.zonedWithDSTCorrection:(Ljava/time/LocalDateTime;)Ljava/time/ZonedDateTime;
-   #39 = Methodref          #113.#114     // java/time/ZonedDateTime.toInstant:()Ljava/time/Instant;
-   #40 = Methodref          #115.#116     // java/time/Instant.toEpochMilli:()J
-   #41 = Methodref          #65.#117      // EpochWriter.newValues:(JDDDD[I)Z
-   #42 = Methodref          #55.#118      // GENEActivReader.secs2Nanos:(D)J
-   #43 = Methodref          #69.#119      // java/time/LocalDateTime.plusNanos:(J)Ljava/time/LocalDateTime;
-   #44 = Methodref          #66.#120      // java/lang/Boolean.booleanValue:()Z
-   #45 = Methodref          #18.#121      // java/lang/StringBuilder.append:(I)Ljava/lang/StringBuilder;
-   #46 = String             #122          // %\t
-   #47 = Methodref          #101.#123     // java/io/PrintStream.print:(Ljava/lang/String;)V
-   #48 = Methodref          #3.#124       // java/io/BufferedReader.close:()V
-   #49 = Methodref          #28.#125      // java/lang/Exception.printStackTrace:(Ljava/io/PrintStream;)V
-   #50 = String             #126          // error reading/writing file
-   #51 = Methodref          #93.#127      // java/lang/System.exit:(I)V
-   #52 = Methodref          #128.#129     // java/lang/Integer.parseInt:(Ljava/lang/String;)I
-   #53 = String             #130          //
-   #54 = Methodref          #3.#131       // java/io/BufferedReader.readLine:()Ljava/lang/String;
-   #55 = Class              #132          // GENEActivReader
-   #56 = Class              #133          // DeviceReader
+   #38 = Methodref          #55.#117      // GENEActivReader.zonedWithDSTCorrection:(Ljava/time/LocalDateTime;)Ljava/time/ZonedDateTime;
+   #39 = Methodref          #118.#119     // java/time/ZonedDateTime.toInstant:()Ljava/time/Instant;
+   #40 = Methodref          #120.#121     // java/time/Instant.toEpochMilli:()J
+   #41 = Methodref          #122.#123     // EpochWriter.newValues:(JDDDD[I)Z
+   #42 = Methodref          #55.#124      // GENEActivReader.secs2Nanos:(D)J
+   #43 = Methodref          #86.#125      // java/time/LocalDateTime.plusNanos:(J)Ljava/time/LocalDateTime;
+   #44 = Methodref          #126.#127     // java/lang/Boolean.booleanValue:()Z
+   #45 = Methodref          #18.#128      // java/lang/StringBuilder.append:(I)Ljava/lang/StringBuilder;
+   #46 = String             #129          // %\t
+   #47 = Methodref          #106.#130     // java/io/PrintStream.print:(Ljava/lang/String;)V
+   #48 = Methodref          #3.#131       // java/io/BufferedReader.close:()V
+   #49 = Methodref          #28.#132      // java/lang/Exception.printStackTrace:(Ljava/io/PrintStream;)V
+   #50 = String             #133          // error reading/writing file
+   #51 = Methodref          #98.#134      // java/lang/System.exit:(I)V
+   #52 = Methodref          #135.#136     // java/lang/Integer.parseInt:(Ljava/lang/String;)I
+   #53 = String             #137          //
+   #54 = Methodref          #3.#138       // java/io/BufferedReader.readLine:()Ljava/lang/String;
+   #55 = Class              #139          // GENEActivReader
+   #56 = Class              #140          // DeviceReader
    #57 = Utf8               <init>
    #58 = Utf8               ()V
    #59 = Utf8               Code
    #60 = Utf8               LineNumberTable
    #61 = Utf8               readGeneaEpochs
    #62 = Utf8               (Ljava/lang/String;Ljava/lang/String;ILEpochWriter;Ljava/lang/Boolean;)V
    #63 = Utf8               StackMapTable
-   #64 = Class              #134          // java/lang/String
-   #65 = Class              #135          // EpochWriter
-   #66 = Class              #136          // java/lang/Boolean
-   #67 = Class              #137          // "[I"
-   #68 = Class              #138          // "[D"
-   #69 = Class              #139          // java/time/LocalDateTime
-   #70 = Class              #140          // java/time/format/DateTimeFormatter
-   #71 = Utf8               parseBinFileHeader
-   #72 = Utf8               (Ljava/io/BufferedReader;II[D[I)I
-   #73 = Utf8               readLine
-   #74 = Utf8               (Ljava/io/BufferedReader;)Ljava/lang/String;
-   #75 = Utf8               SourceFile
-   #76 = Utf8               GENEActivReader.java
-   #77 = NameAndType        #57:#58       // "<init>":()V
-   #78 = NameAndType        #141:#142     // setTimeSettings:(Ljava/lang/String;I)V
-   #79 = Utf8               java/io/BufferedReader
-   #80 = Utf8               java/io/FileReader
-   #81 = NameAndType        #57:#143      // "<init>":(Ljava/lang/String;)V
-   #82 = NameAndType        #57:#144      // "<init>":(Ljava/io/Reader;)V
-   #83 = NameAndType        #71:#72       // parseBinFileHeader:(Ljava/io/BufferedReader;II[D[I)I
-   #84 = NameAndType        #145:#146     // of:(IIIIII)Ljava/time/LocalDateTime;
-   #85 = Utf8               yyyy-MM-dd HH:mm:ss:SSS
-   #86 = NameAndType        #147:#148     // ofPattern:(Ljava/lang/String;)Ljava/time/format/DateTimeFormatter;
-   #87 = NameAndType        #73:#74       // readLine:(Ljava/io/BufferedReader;)Ljava/lang/String;
-   #88 = Utf8               Time:
-   #89 = NameAndType        #149:#150     // split:(Ljava/lang/String;)[Ljava/lang/String;
-   #90 = NameAndType        #151:#152     // parse:(Ljava/lang/CharSequence;Ljava/time/format/DateTimeFormatter;)Ljava/time/LocalDateTime;
-   #91 = NameAndType        #153:#154     // plusMinutes:(J)Ljava/time/LocalDateTime;
-   #92 = NameAndType        #155:#156     // setSessionStart:(Ljava/time/LocalDateTime;)V
-   #93 = Class              #157          // java/lang/System
-   #94 = NameAndType        #158:#159     // out:Ljava/io/PrintStream;
-   #95 = Utf8               java/lang/StringBuilder
-   #96 = Utf8               Session start:
-   #97 = NameAndType        #160:#161     // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-   #98 = NameAndType        #162:#163     // sessionStart:Ljava/time/ZonedDateTime;
-   #99 = NameAndType        #160:#164     // append:(Ljava/lang/Object;)Ljava/lang/StringBuilder;
-  #100 = NameAndType        #165:#166     // toString:()Ljava/lang/String;
-  #101 = Class              #167          // java/io/PrintStream
-  #102 = NameAndType        #168:#143     // println:(Ljava/lang/String;)V
-  #103 = Utf8               :
-  #104 = Class              #169          // java/lang/Double
-  #105 = NameAndType        #170:#171     // parseDouble:(Ljava/lang/String;)D
-  #106 = Utf8               java/lang/Exception
-  #107 = NameAndType        #172:#159     // err:Ljava/io/PrintStream;
-  #108 = NameAndType        #173:#174     // length:()I
-  #109 = NameAndType        #175:#176     // getSignedIntFromHex:(Ljava/lang/String;II)I
-  #110 = Utf8               block err @
-  #111 = Utf8               :
-  #112 = NameAndType        #177:#178     // zonedWithDSTCorrection:(Ljava/time/LocalDateTime;)Ljava/time/ZonedDateTime;
-  #113 = Class              #179          // java/time/ZonedDateTime
-  #114 = NameAndType        #180:#181     // toInstant:()Ljava/time/Instant;
-  #115 = Class              #182          // java/time/Instant
-  #116 = NameAndType        #183:#184     // toEpochMilli:()J
-  #117 = NameAndType        #185:#186     // newValues:(JDDDD[I)Z
-  #118 = NameAndType        #187:#188     // secs2Nanos:(D)J
-  #119 = NameAndType        #189:#154     // plusNanos:(J)Ljava/time/LocalDateTime;
-  #120 = NameAndType        #190:#191     // booleanValue:()Z
-  #121 = NameAndType        #160:#192     // append:(I)Ljava/lang/StringBuilder;
-  #122 = Utf8               %\t
-  #123 = NameAndType        #193:#143     // print:(Ljava/lang/String;)V
-  #124 = NameAndType        #194:#58      // close:()V
-  #125 = NameAndType        #195:#196     // printStackTrace:(Ljava/io/PrintStream;)V
-  #126 = Utf8               error reading/writing file
-  #127 = NameAndType        #197:#198     // exit:(I)V
-  #128 = Class              #199          // java/lang/Integer
-  #129 = NameAndType        #200:#201     // parseInt:(Ljava/lang/String;)I
-  #130 = Utf8
-  #131 = NameAndType        #73:#166      // readLine:()Ljava/lang/String;
-  #132 = Utf8               GENEActivReader
-  #133 = Utf8               DeviceReader
-  #134 = Utf8               java/lang/String
-  #135 = Utf8               EpochWriter
-  #136 = Utf8               java/lang/Boolean
-  #137 = Utf8               [I
-  #138 = Utf8               [D
-  #139 = Utf8               java/time/LocalDateTime
-  #140 = Utf8               java/time/format/DateTimeFormatter
-  #141 = Utf8               setTimeSettings
-  #142 = Utf8               (Ljava/lang/String;I)V
-  #143 = Utf8               (Ljava/lang/String;)V
-  #144 = Utf8               (Ljava/io/Reader;)V
-  #145 = Utf8               of
-  #146 = Utf8               (IIIIII)Ljava/time/LocalDateTime;
-  #147 = Utf8               ofPattern
-  #148 = Utf8               (Ljava/lang/String;)Ljava/time/format/DateTimeFormatter;
-  #149 = Utf8               split
-  #150 = Utf8               (Ljava/lang/String;)[Ljava/lang/String;
-  #151 = Utf8               parse
-  #152 = Utf8               (Ljava/lang/CharSequence;Ljava/time/format/DateTimeFormatter;)Ljava/time/LocalDateTime;
-  #153 = Utf8               plusMinutes
-  #154 = Utf8               (J)Ljava/time/LocalDateTime;
-  #155 = Utf8               setSessionStart
-  #156 = Utf8               (Ljava/time/LocalDateTime;)V
-  #157 = Utf8               java/lang/System
-  #158 = Utf8               out
-  #159 = Utf8               Ljava/io/PrintStream;
-  #160 = Utf8               append
-  #161 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #162 = Utf8               sessionStart
-  #163 = Utf8               Ljava/time/ZonedDateTime;
-  #164 = Utf8               (Ljava/lang/Object;)Ljava/lang/StringBuilder;
-  #165 = Utf8               toString
-  #166 = Utf8               ()Ljava/lang/String;
-  #167 = Utf8               java/io/PrintStream
-  #168 = Utf8               println
-  #169 = Utf8               java/lang/Double
-  #170 = Utf8               parseDouble
-  #171 = Utf8               (Ljava/lang/String;)D
-  #172 = Utf8               err
-  #173 = Utf8               length
-  #174 = Utf8               ()I
-  #175 = Utf8               getSignedIntFromHex
-  #176 = Utf8               (Ljava/lang/String;II)I
-  #177 = Utf8               zonedWithDSTCorrection
-  #178 = Utf8               (Ljava/time/LocalDateTime;)Ljava/time/ZonedDateTime;
-  #179 = Utf8               java/time/ZonedDateTime
-  #180 = Utf8               toInstant
-  #181 = Utf8               ()Ljava/time/Instant;
-  #182 = Utf8               java/time/Instant
-  #183 = Utf8               toEpochMilli
-  #184 = Utf8               ()J
-  #185 = Utf8               newValues
-  #186 = Utf8               (JDDDD[I)Z
-  #187 = Utf8               secs2Nanos
-  #188 = Utf8               (D)J
-  #189 = Utf8               plusNanos
-  #190 = Utf8               booleanValue
-  #191 = Utf8               ()Z
-  #192 = Utf8               (I)Ljava/lang/StringBuilder;
-  #193 = Utf8               print
-  #194 = Utf8               close
-  #195 = Utf8               printStackTrace
-  #196 = Utf8               (Ljava/io/PrintStream;)V
-  #197 = Utf8               exit
-  #198 = Utf8               (I)V
-  #199 = Utf8               java/lang/Integer
-  #200 = Utf8               parseInt
-  #201 = Utf8               (Ljava/lang/String;)I
+   #64 = Class              #141          // java/lang/String
+   #65 = Class              #142          // EpochWriter
+   #66 = Class              #143          // java/lang/Boolean
+   #67 = Class              #144          // "[I"
+   #68 = Class              #81           // java/io/BufferedReader
+   #69 = Class              #145          // "[D"
+   #70 = Class              #146          // java/time/LocalDateTime
+   #71 = Class              #147          // java/time/format/DateTimeFormatter
+   #72 = Class              #111          // java/lang/Exception
+   #73 = Utf8               parseBinFileHeader
+   #74 = Utf8               (Ljava/io/BufferedReader;II[D[I)I
+   #75 = Utf8               readLine
+   #76 = Utf8               (Ljava/io/BufferedReader;)Ljava/lang/String;
+   #77 = Utf8               SourceFile
+   #78 = Utf8               GENEActivReader.java
+   #79 = NameAndType        #57:#58       // "<init>":()V
+   #80 = NameAndType        #148:#149     // setTimeSettings:(Ljava/lang/String;I)V
+   #81 = Utf8               java/io/BufferedReader
+   #82 = Utf8               java/io/FileReader
+   #83 = NameAndType        #57:#150      // "<init>":(Ljava/lang/String;)V
+   #84 = NameAndType        #57:#151      // "<init>":(Ljava/io/Reader;)V
+   #85 = NameAndType        #73:#74       // parseBinFileHeader:(Ljava/io/BufferedReader;II[D[I)I
+   #86 = Class              #146          // java/time/LocalDateTime
+   #87 = NameAndType        #152:#153     // of:(IIIIII)Ljava/time/LocalDateTime;
+   #88 = Utf8               yyyy-MM-dd HH:mm:ss:SSS
+   #89 = Class              #147          // java/time/format/DateTimeFormatter
+   #90 = NameAndType        #154:#155     // ofPattern:(Ljava/lang/String;)Ljava/time/format/DateTimeFormatter;
+   #91 = NameAndType        #75:#76       // readLine:(Ljava/io/BufferedReader;)Ljava/lang/String;
+   #92 = Utf8               Time:
+   #93 = Class              #141          // java/lang/String
+   #94 = NameAndType        #156:#157     // split:(Ljava/lang/String;)[Ljava/lang/String;
+   #95 = NameAndType        #158:#159     // parse:(Ljava/lang/CharSequence;Ljava/time/format/DateTimeFormatter;)Ljava/time/LocalDateTime;
+   #96 = NameAndType        #160:#161     // plusMinutes:(J)Ljava/time/LocalDateTime;
+   #97 = NameAndType        #162:#163     // setSessionStart:(Ljava/time/LocalDateTime;)V
+   #98 = Class              #164          // java/lang/System
+   #99 = NameAndType        #165:#166     // out:Ljava/io/PrintStream;
+  #100 = Utf8               java/lang/StringBuilder
+  #101 = Utf8               Session start:
+  #102 = NameAndType        #167:#168     // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #103 = NameAndType        #169:#170     // sessionStart:Ljava/time/ZonedDateTime;
+  #104 = NameAndType        #167:#171     // append:(Ljava/lang/Object;)Ljava/lang/StringBuilder;
+  #105 = NameAndType        #172:#173     // toString:()Ljava/lang/String;
+  #106 = Class              #174          // java/io/PrintStream
+  #107 = NameAndType        #175:#150     // println:(Ljava/lang/String;)V
+  #108 = Utf8               :
+  #109 = Class              #176          // java/lang/Double
+  #110 = NameAndType        #177:#178     // parseDouble:(Ljava/lang/String;)D
+  #111 = Utf8               java/lang/Exception
+  #112 = NameAndType        #179:#166     // err:Ljava/io/PrintStream;
+  #113 = NameAndType        #180:#181     // length:()I
+  #114 = NameAndType        #182:#183     // getSignedIntFromHex:(Ljava/lang/String;II)I
+  #115 = Utf8               block err @
+  #116 = Utf8               :
+  #117 = NameAndType        #184:#185     // zonedWithDSTCorrection:(Ljava/time/LocalDateTime;)Ljava/time/ZonedDateTime;
+  #118 = Class              #186          // java/time/ZonedDateTime
+  #119 = NameAndType        #187:#188     // toInstant:()Ljava/time/Instant;
+  #120 = Class              #189          // java/time/Instant
+  #121 = NameAndType        #190:#191     // toEpochMilli:()J
+  #122 = Class              #142          // EpochWriter
+  #123 = NameAndType        #192:#193     // newValues:(JDDDD[I)Z
+  #124 = NameAndType        #194:#195     // secs2Nanos:(D)J
+  #125 = NameAndType        #196:#161     // plusNanos:(J)Ljava/time/LocalDateTime;
+  #126 = Class              #143          // java/lang/Boolean
+  #127 = NameAndType        #197:#198     // booleanValue:()Z
+  #128 = NameAndType        #167:#199     // append:(I)Ljava/lang/StringBuilder;
+  #129 = Utf8               %\t
+  #130 = NameAndType        #200:#150     // print:(Ljava/lang/String;)V
+  #131 = NameAndType        #201:#58      // close:()V
+  #132 = NameAndType        #202:#203     // printStackTrace:(Ljava/io/PrintStream;)V
+  #133 = Utf8               error reading/writing file
+  #134 = NameAndType        #204:#205     // exit:(I)V
+  #135 = Class              #206          // java/lang/Integer
+  #136 = NameAndType        #207:#208     // parseInt:(Ljava/lang/String;)I
+  #137 = Utf8
+  #138 = NameAndType        #75:#173      // readLine:()Ljava/lang/String;
+  #139 = Utf8               GENEActivReader
+  #140 = Utf8               DeviceReader
+  #141 = Utf8               java/lang/String
+  #142 = Utf8               EpochWriter
+  #143 = Utf8               java/lang/Boolean
+  #144 = Utf8               [I
+  #145 = Utf8               [D
+  #146 = Utf8               java/time/LocalDateTime
+  #147 = Utf8               java/time/format/DateTimeFormatter
+  #148 = Utf8               setTimeSettings
+  #149 = Utf8               (Ljava/lang/String;I)V
+  #150 = Utf8               (Ljava/lang/String;)V
+  #151 = Utf8               (Ljava/io/Reader;)V
+  #152 = Utf8               of
+  #153 = Utf8               (IIIIII)Ljava/time/LocalDateTime;
+  #154 = Utf8               ofPattern
+  #155 = Utf8               (Ljava/lang/String;)Ljava/time/format/DateTimeFormatter;
+  #156 = Utf8               split
+  #157 = Utf8               (Ljava/lang/String;)[Ljava/lang/String;
+  #158 = Utf8               parse
+  #159 = Utf8               (Ljava/lang/CharSequence;Ljava/time/format/DateTimeFormatter;)Ljava/time/LocalDateTime;
+  #160 = Utf8               plusMinutes
+  #161 = Utf8               (J)Ljava/time/LocalDateTime;
+  #162 = Utf8               setSessionStart
+  #163 = Utf8               (Ljava/time/LocalDateTime;)V
+  #164 = Utf8               java/lang/System
+  #165 = Utf8               out
+  #166 = Utf8               Ljava/io/PrintStream;
+  #167 = Utf8               append
+  #168 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #169 = Utf8               sessionStart
+  #170 = Utf8               Ljava/time/ZonedDateTime;
+  #171 = Utf8               (Ljava/lang/Object;)Ljava/lang/StringBuilder;
+  #172 = Utf8               toString
+  #173 = Utf8               ()Ljava/lang/String;
+  #174 = Utf8               java/io/PrintStream
+  #175 = Utf8               println
+  #176 = Utf8               java/lang/Double
+  #177 = Utf8               parseDouble
+  #178 = Utf8               (Ljava/lang/String;)D
+  #179 = Utf8               err
+  #180 = Utf8               length
+  #181 = Utf8               ()I
+  #182 = Utf8               getSignedIntFromHex
+  #183 = Utf8               (Ljava/lang/String;II)I
+  #184 = Utf8               zonedWithDSTCorrection
+  #185 = Utf8               (Ljava/time/LocalDateTime;)Ljava/time/ZonedDateTime;
+  #186 = Utf8               java/time/ZonedDateTime
+  #187 = Utf8               toInstant
+  #188 = Utf8               ()Ljava/time/Instant;
+  #189 = Utf8               java/time/Instant
+  #190 = Utf8               toEpochMilli
+  #191 = Utf8               ()J
+  #192 = Utf8               newValues
+  #193 = Utf8               (JDDDD[I)Z
+  #194 = Utf8               secs2Nanos
+  #195 = Utf8               (D)J
+  #196 = Utf8               plusNanos
+  #197 = Utf8               booleanValue
+  #198 = Utf8               ()Z
+  #199 = Utf8               (I)Ljava/lang/StringBuilder;
+  #200 = Utf8               print
+  #201 = Utf8               close
+  #202 = Utf8               printStackTrace
+  #203 = Utf8               (Ljava/io/PrintStream;)V
+  #204 = Utf8               exit
+  #205 = Utf8               (I)V
+  #206 = Utf8               java/lang/Integer
+  #207 = Utf8               parseInt
+  #208 = Utf8               (Ljava/lang/String;)I
 {
   public GENEActivReader();
     descriptor: ()V
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
```

### Comparing `accelerometer-6.2.3/accelerometer/java/GENEActivReader.java` & `accelerometer-7.0.0.dev0/src/accelerometer/java/GENEActivReader.java`

 * *Files identical despite different names*

### Comparing `accelerometer-6.2.3/accelerometer/java/JTransforms-3.1-with-dependencies.jar` & `accelerometer-7.0.0.dev0/src/accelerometer/java/JTransforms-3.1-with-dependencies.jar`

 * *Files identical despite different names*

### Comparing `accelerometer-6.2.3/accelerometer/java/LowpassFilter.class` & `accelerometer-7.0.0.dev0/src/accelerometer/java/LowpassFilter.class`

 * *Files 9% similar despite different names*

#### javap -verbose -constants -s -l -private {}

```diff
@@ -1,132 +1,134 @@
-  SHA-256 checksum b7909f205d6e202f9f18a70e1f6eb48ff47adb7d1e7562e13d90313ec3cc4e1c
+  SHA-256 checksum 3dd6b5d226fb17c1c1f2a18e5314cd5628ec4f7bf6241a648071928029592656
   Compiled from "LowpassFilter.java"
 public class LowpassFilter extends Filter
   minor version: 0
   major version: 52
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #41                         // LowpassFilter
   super_class: #1                         // Filter
   interfaces: 0, fields: 0, methods: 2, attributes: 1
 Constant pool:
-    #1 = Class              #54           // Filter
-    #2 = Methodref          #1.#55        // Filter."<init>":()V
+    #1 = Class              #55           // Filter
+    #2 = Methodref          #1.#56        // Filter."<init>":()V
     #3 = Double             2.0d
-    #5 = Fieldref           #56.#57       // java/lang/System.out:Ljava/io/PrintStream;
-    #6 = String             #58           // \nThe specified lowpass filter cutoff (%s) is >= Nyquist frequency of the sampling rate (%s), therefore the cutoff will be capped at %s\n\n
-    #7 = Class              #59           // java/lang/Object
-    #8 = Methodref          #60.#61       // java/lang/Double.valueOf:(D)Ljava/lang/Double;
-    #9 = Methodref          #62.#63       // java/io/PrintStream.format:(Ljava/lang/String;[Ljava/lang/Object;)Ljava/io/PrintStream;
+    #5 = Fieldref           #57.#58       // java/lang/System.out:Ljava/io/PrintStream;
+    #6 = String             #59           // \nThe specified lowpass filter cutoff (%s) is >= Nyquist frequency of the sampling rate (%s), therefore the cutoff will be capped at %s\n\n
+    #7 = Class              #60           // java/lang/Object
+    #8 = Methodref          #61.#62       // java/lang/Double.valueOf:(D)Ljava/lang/Double;
+    #9 = Methodref          #63.#64       // java/io/PrintStream.format:(Ljava/lang/String;[Ljava/lang/Object;)Ljava/io/PrintStream;
    #10 = Double             0.999d
-   #12 = Methodref          #29.#64       // java/lang/Math.min:(DD)D
-   #13 = Fieldref           #41.#65       // LowpassFilter.BUTTERWORTH4_NUM_COEFFICIENTS:I
-   #14 = Fieldref           #41.#66       // LowpassFilter.B:[D
-   #15 = Fieldref           #41.#67       // LowpassFilter.A:[D
-   #16 = Methodref          #41.#68       // LowpassFilter.CoefficientsButterworth4LP:(D[D[D)V
-   #17 = Methodref          #47.#69       // java/lang/Boolean.booleanValue:()Z
-   #18 = Class              #70           // java/lang/StringBuilder
-   #19 = Methodref          #18.#55       // java/lang/StringBuilder."<init>":()V
-   #20 = String             #71           // B =
-   #21 = Methodref          #18.#72       // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-   #22 = Methodref          #73.#74       // java/util/Arrays.toString:([D)Ljava/lang/String;
-   #23 = Methodref          #18.#75       // java/lang/StringBuilder.toString:()Ljava/lang/String;
-   #24 = Methodref          #62.#76       // java/io/PrintStream.println:(Ljava/lang/String;)V
-   #25 = String             #77           // A =
-   #26 = Fieldref           #41.#78       // LowpassFilter.z:[D
-   #27 = Methodref          #41.#79       // LowpassFilter.reset:()V
-   #28 = Methodref          #47.#80       // java/lang/Boolean.valueOf:(Z)Ljava/lang/Boolean;
-   #29 = Class              #81           // java/lang/Math
+   #12 = Methodref          #29.#65       // java/lang/Math.min:(DD)D
+   #13 = Fieldref           #41.#66       // LowpassFilter.BUTTERWORTH4_NUM_COEFFICIENTS:I
+   #14 = Fieldref           #41.#67       // LowpassFilter.B:[D
+   #15 = Fieldref           #41.#68       // LowpassFilter.A:[D
+   #16 = Methodref          #41.#69       // LowpassFilter.CoefficientsButterworth4LP:(D[D[D)V
+   #17 = Methodref          #70.#71       // java/lang/Boolean.booleanValue:()Z
+   #18 = Class              #72           // java/lang/StringBuilder
+   #19 = Methodref          #18.#56       // java/lang/StringBuilder."<init>":()V
+   #20 = String             #73           // B =
+   #21 = Methodref          #18.#74       // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+   #22 = Methodref          #75.#76       // java/util/Arrays.toString:([D)Ljava/lang/String;
+   #23 = Methodref          #18.#77       // java/lang/StringBuilder.toString:()Ljava/lang/String;
+   #24 = Methodref          #63.#78       // java/io/PrintStream.println:(Ljava/lang/String;)V
+   #25 = String             #79           // A =
+   #26 = Fieldref           #41.#80       // LowpassFilter.z:[D
+   #27 = Methodref          #41.#81       // LowpassFilter.reset:()V
+   #28 = Methodref          #70.#82       // java/lang/Boolean.valueOf:(Z)Ljava/lang/Boolean;
+   #29 = Class              #83           // java/lang/Math
    #30 = Double             3.141592653589793d
-   #32 = Methodref          #29.#82       // java/lang/Math.sin:(D)D
+   #32 = Methodref          #29.#84       // java/lang/Math.sin:(D)D
    #33 = Double             0.39269908169872414d
-   #35 = Methodref          #29.#83       // java/lang/Math.cos:(D)D
+   #35 = Methodref          #29.#85       // java/lang/Math.cos:(D)D
    #36 = Double             4.0d
-   #38 = Methodref          #29.#84       // java/lang/Math.pow:(DD)D
+   #38 = Methodref          #29.#86       // java/lang/Math.pow:(DD)D
    #39 = Double             8.0d
-   #41 = Class              #85           // LowpassFilter
+   #41 = Class              #87           // LowpassFilter
    #42 = Utf8               <init>
    #43 = Utf8               (DDLjava/lang/Boolean;)V
    #44 = Utf8               Code
    #45 = Utf8               LineNumberTable
    #46 = Utf8               StackMapTable
-   #47 = Class              #86           // java/lang/Boolean
-   #48 = Utf8               CoefficientsButterworth4LP
-   #49 = Utf8               (D[D[D)V
-   #50 = Class              #87           // "[D"
-   #51 = Class              #88           // "[I"
-   #52 = Utf8               SourceFile
-   #53 = Utf8               LowpassFilter.java
-   #54 = Utf8               Filter
-   #55 = NameAndType        #42:#89       // "<init>":()V
-   #56 = Class              #90           // java/lang/System
-   #57 = NameAndType        #91:#92       // out:Ljava/io/PrintStream;
-   #58 = Utf8               \nThe specified lowpass filter cutoff (%s) is >= Nyquist frequency of the sampling rate (%s), therefore the cutoff will be capped at %s\n\n
-   #59 = Utf8               java/lang/Object
-   #60 = Class              #93           // java/lang/Double
-   #61 = NameAndType        #94:#95       // valueOf:(D)Ljava/lang/Double;
-   #62 = Class              #96           // java/io/PrintStream
-   #63 = NameAndType        #97:#98       // format:(Ljava/lang/String;[Ljava/lang/Object;)Ljava/io/PrintStream;
-   #64 = NameAndType        #99:#100      // min:(DD)D
-   #65 = NameAndType        #101:#102     // BUTTERWORTH4_NUM_COEFFICIENTS:I
-   #66 = NameAndType        #103:#87      // B:[D
-   #67 = NameAndType        #104:#87      // A:[D
-   #68 = NameAndType        #48:#49       // CoefficientsButterworth4LP:(D[D[D)V
-   #69 = NameAndType        #105:#106     // booleanValue:()Z
-   #70 = Utf8               java/lang/StringBuilder
-   #71 = Utf8               B =
-   #72 = NameAndType        #107:#108     // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-   #73 = Class              #109          // java/util/Arrays
-   #74 = NameAndType        #110:#111     // toString:([D)Ljava/lang/String;
-   #75 = NameAndType        #110:#112     // toString:()Ljava/lang/String;
-   #76 = NameAndType        #113:#114     // println:(Ljava/lang/String;)V
-   #77 = Utf8               A =
-   #78 = NameAndType        #115:#87      // z:[D
-   #79 = NameAndType        #116:#89      // reset:()V
-   #80 = NameAndType        #94:#117      // valueOf:(Z)Ljava/lang/Boolean;
-   #81 = Utf8               java/lang/Math
-   #82 = NameAndType        #118:#119     // sin:(D)D
-   #83 = NameAndType        #120:#119     // cos:(D)D
-   #84 = NameAndType        #121:#100     // pow:(DD)D
-   #85 = Utf8               LowpassFilter
-   #86 = Utf8               java/lang/Boolean
-   #87 = Utf8               [D
-   #88 = Utf8               [I
-   #89 = Utf8               ()V
-   #90 = Utf8               java/lang/System
-   #91 = Utf8               out
-   #92 = Utf8               Ljava/io/PrintStream;
-   #93 = Utf8               java/lang/Double
-   #94 = Utf8               valueOf
-   #95 = Utf8               (D)Ljava/lang/Double;
-   #96 = Utf8               java/io/PrintStream
-   #97 = Utf8               format
-   #98 = Utf8               (Ljava/lang/String;[Ljava/lang/Object;)Ljava/io/PrintStream;
-   #99 = Utf8               min
-  #100 = Utf8               (DD)D
-  #101 = Utf8               BUTTERWORTH4_NUM_COEFFICIENTS
-  #102 = Utf8               I
-  #103 = Utf8               B
-  #104 = Utf8               A
-  #105 = Utf8               booleanValue
-  #106 = Utf8               ()Z
-  #107 = Utf8               append
-  #108 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #109 = Utf8               java/util/Arrays
-  #110 = Utf8               toString
-  #111 = Utf8               ([D)Ljava/lang/String;
-  #112 = Utf8               ()Ljava/lang/String;
-  #113 = Utf8               println
-  #114 = Utf8               (Ljava/lang/String;)V
-  #115 = Utf8               z
-  #116 = Utf8               reset
-  #117 = Utf8               (Z)Ljava/lang/Boolean;
-  #118 = Utf8               sin
-  #119 = Utf8               (D)D
-  #120 = Utf8               cos
-  #121 = Utf8               pow
+   #47 = Class              #87           // LowpassFilter
+   #48 = Class              #88           // java/lang/Boolean
+   #49 = Utf8               CoefficientsButterworth4LP
+   #50 = Utf8               (D[D[D)V
+   #51 = Class              #89           // "[D"
+   #52 = Class              #90           // "[I"
+   #53 = Utf8               SourceFile
+   #54 = Utf8               LowpassFilter.java
+   #55 = Utf8               Filter
+   #56 = NameAndType        #42:#91       // "<init>":()V
+   #57 = Class              #92           // java/lang/System
+   #58 = NameAndType        #93:#94       // out:Ljava/io/PrintStream;
+   #59 = Utf8               \nThe specified lowpass filter cutoff (%s) is >= Nyquist frequency of the sampling rate (%s), therefore the cutoff will be capped at %s\n\n
+   #60 = Utf8               java/lang/Object
+   #61 = Class              #95           // java/lang/Double
+   #62 = NameAndType        #96:#97       // valueOf:(D)Ljava/lang/Double;
+   #63 = Class              #98           // java/io/PrintStream
+   #64 = NameAndType        #99:#100      // format:(Ljava/lang/String;[Ljava/lang/Object;)Ljava/io/PrintStream;
+   #65 = NameAndType        #101:#102     // min:(DD)D
+   #66 = NameAndType        #103:#104     // BUTTERWORTH4_NUM_COEFFICIENTS:I
+   #67 = NameAndType        #105:#89      // B:[D
+   #68 = NameAndType        #106:#89      // A:[D
+   #69 = NameAndType        #49:#50       // CoefficientsButterworth4LP:(D[D[D)V
+   #70 = Class              #88           // java/lang/Boolean
+   #71 = NameAndType        #107:#108     // booleanValue:()Z
+   #72 = Utf8               java/lang/StringBuilder
+   #73 = Utf8               B =
+   #74 = NameAndType        #109:#110     // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+   #75 = Class              #111          // java/util/Arrays
+   #76 = NameAndType        #112:#113     // toString:([D)Ljava/lang/String;
+   #77 = NameAndType        #112:#114     // toString:()Ljava/lang/String;
+   #78 = NameAndType        #115:#116     // println:(Ljava/lang/String;)V
+   #79 = Utf8               A =
+   #80 = NameAndType        #117:#89      // z:[D
+   #81 = NameAndType        #118:#91      // reset:()V
+   #82 = NameAndType        #96:#119      // valueOf:(Z)Ljava/lang/Boolean;
+   #83 = Utf8               java/lang/Math
+   #84 = NameAndType        #120:#121     // sin:(D)D
+   #85 = NameAndType        #122:#121     // cos:(D)D
+   #86 = NameAndType        #123:#102     // pow:(DD)D
+   #87 = Utf8               LowpassFilter
+   #88 = Utf8               java/lang/Boolean
+   #89 = Utf8               [D
+   #90 = Utf8               [I
+   #91 = Utf8               ()V
+   #92 = Utf8               java/lang/System
+   #93 = Utf8               out
+   #94 = Utf8               Ljava/io/PrintStream;
+   #95 = Utf8               java/lang/Double
+   #96 = Utf8               valueOf
+   #97 = Utf8               (D)Ljava/lang/Double;
+   #98 = Utf8               java/io/PrintStream
+   #99 = Utf8               format
+  #100 = Utf8               (Ljava/lang/String;[Ljava/lang/Object;)Ljava/io/PrintStream;
+  #101 = Utf8               min
+  #102 = Utf8               (DD)D
+  #103 = Utf8               BUTTERWORTH4_NUM_COEFFICIENTS
+  #104 = Utf8               I
+  #105 = Utf8               B
+  #106 = Utf8               A
+  #107 = Utf8               booleanValue
+  #108 = Utf8               ()Z
+  #109 = Utf8               append
+  #110 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #111 = Utf8               java/util/Arrays
+  #112 = Utf8               toString
+  #113 = Utf8               ([D)Ljava/lang/String;
+  #114 = Utf8               ()Ljava/lang/String;
+  #115 = Utf8               println
+  #116 = Utf8               (Ljava/lang/String;)V
+  #117 = Utf8               z
+  #118 = Utf8               reset
+  #119 = Utf8               (Z)Ljava/lang/Boolean;
+  #120 = Utf8               sin
+  #121 = Utf8               (D)D
+  #122 = Utf8               cos
+  #123 = Utf8               pow
 {
   public LowpassFilter(double, double, java.lang.Boolean);
     descriptor: (DDLjava/lang/Boolean;)V
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=9, locals=8, args_size=4
          0: aload_0
```

### Comparing `accelerometer-6.2.3/accelerometer/java/LowpassFilter.java` & `accelerometer-7.0.0.dev0/src/accelerometer/java/LowpassFilter.java`

 * *Files identical despite different names*

### Comparing `accelerometer-6.2.3/accelerometer/java/NpyWriter.class` & `accelerometer-7.0.0.dev0/src/accelerometer/java/NpyWriter.class`

 * *Files 12% similar despite different names*

#### javap -verbose -constants -s -l -private {}

```diff
@@ -1,141 +1,141 @@
-  SHA-256 checksum bc19a983e24bc0ab362a3bbac49a86f10e55f9465a6431f65f126643193980e0
+  SHA-256 checksum b052aba7391b7a3e5e3f961802a92c9edee53d218c0125d10000e6bb1a71aa35
   Compiled from "NpyWriter.java"
 public class NpyWriter
   minor version: 0
   major version: 52
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #1                          // NpyWriter
   super_class: #124                       // java/lang/Object
   interfaces: 0, fields: 17, methods: 9, attributes: 1
 Constant pool:
-    #1 = Class              #184          // NpyWriter
-    #2 = Methodref          #124.#185     // java/lang/Object."<init>":()V
-    #3 = Fieldref           #1.#186       // NpyWriter.linesWritten:I
-    #4 = Fieldref           #1.#187       // NpyWriter.bufferLength:I
-    #5 = Class              #188          // java/lang/Long
-    #6 = Class              #189          // java/lang/Float
-    #7 = Fieldref           #1.#190       // NpyWriter.bytesPerLine:I
-    #8 = Methodref          #191.#192     // java/nio/ByteOrder.nativeOrder:()Ljava/nio/ByteOrder;
-    #9 = Fieldref           #1.#193       // NpyWriter.nativeByteOrder:Ljava/nio/ByteOrder;
-   #10 = Fieldref           #191.#194     // java/nio/ByteOrder.BIG_ENDIAN:Ljava/nio/ByteOrder;
-   #11 = Fieldref           #1.#195       // NpyWriter.numpyByteOrder:C
-   #12 = Methodref          #196.#197     // java/nio/ByteBuffer.allocate:(I)Ljava/nio/ByteBuffer;
-   #13 = Methodref          #196.#198     // java/nio/ByteBuffer.order:(Ljava/nio/ByteOrder;)Ljava/nio/ByteBuffer;
-   #14 = Fieldref           #1.#199       // NpyWriter.lineBuffer:Ljava/nio/ByteBuffer;
-   #15 = Class              #200          // java/util/ArrayList
-   #16 = Methodref          #15.#185      // java/util/ArrayList."<init>":()V
-   #17 = Fieldref           #1.#201       // NpyWriter.itemTypes:Ljava/util/ArrayList;
-   #18 = Fieldref           #1.#202       // NpyWriter.itemNames:Ljava/util/ArrayList;
-   #19 = Fieldref           #1.#203       // NpyWriter.outputFile:Ljava/lang/String;
-   #20 = Class              #204          // java/io/File
-   #21 = Methodref          #20.#205      // java/io/File."<init>":(Ljava/lang/String;)V
-   #22 = Fieldref           #1.#206       // NpyWriter.file:Ljava/io/File;
-   #23 = Class              #207          // java/io/RandomAccessFile
-   #24 = String             #208          // rw
-   #25 = Methodref          #23.#209      // java/io/RandomAccessFile."<init>":(Ljava/io/File;Ljava/lang/String;)V
-   #26 = Fieldref           #1.#210       // NpyWriter.raf:Ljava/io/RandomAccessFile;
-   #27 = Methodref          #23.#211      // java/io/RandomAccessFile.setLength:(J)V
-   #28 = Fieldref           #1.#212       // NpyWriter.NPY_HEADER:[B
-   #29 = Class              #213          // java/lang/StringBuilder
-   #30 = Methodref          #29.#185      // java/lang/StringBuilder."<init>":()V
-   #31 = Class              #214          // java/lang/String
-   #32 = Methodref          #31.#215      // java/lang/String."<init>":([C)V
-   #33 = String             #216          // \u0000
-   #34 = String             #217          //
-   #35 = Methodref          #31.#218      // java/lang/String.replace:(Ljava/lang/CharSequence;Ljava/lang/CharSequence;)Ljava/lang/String;
-   #36 = Methodref          #29.#219      // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-   #37 = String             #220          // \n
-   #38 = Methodref          #29.#221      // java/lang/StringBuilder.toString:()Ljava/lang/String;
-   #39 = Methodref          #23.#222      // java/io/RandomAccessFile.writeBytes:(Ljava/lang/String;)V
-   #40 = Methodref          #15.#223      // java/util/ArrayList.add:(Ljava/lang/Object;)Z
-   #41 = String             #224          // time
-   #42 = String             #225          // x
-   #43 = String             #226          // y
-   #44 = String             #227          // z
-   #45 = Class              #228          // java/io/IOException
-   #46 = Class              #229          // java/lang/RuntimeException
-   #47 = String             #230          // The .npy file
-   #48 = String             #231          //  could not be created
-   #49 = Methodref          #46.#205      // java/lang/RuntimeException."<init>":(Ljava/lang/String;)V
-   #50 = Methodref          #196.#232     // java/nio/ByteBuffer.putLong:(J)Ljava/nio/ByteBuffer;
-   #51 = Methodref          #6.#233       // java/lang/Float.floatValue:()F
-   #52 = Methodref          #196.#234     // java/nio/ByteBuffer.putFloat:(F)Ljava/nio/ByteBuffer;
-   #53 = Methodref          #196.#235     // java/nio/ByteBuffer.hasRemaining:()Z
-   #54 = Methodref          #196.#236     // java/nio/ByteBuffer.array:()[B
-   #55 = Methodref          #23.#237      // java/io/RandomAccessFile.write:([B)V
-   #56 = Methodref          #196.#238     // java/nio/ByteBuffer.clear:()Ljava/nio/Buffer;
+    #1 = Class              #188          // NpyWriter
+    #2 = Methodref          #124.#189     // java/lang/Object."<init>":()V
+    #3 = Fieldref           #1.#190       // NpyWriter.linesWritten:I
+    #4 = Fieldref           #1.#191       // NpyWriter.bufferLength:I
+    #5 = Class              #192          // java/lang/Long
+    #6 = Class              #193          // java/lang/Float
+    #7 = Fieldref           #1.#194       // NpyWriter.bytesPerLine:I
+    #8 = Methodref          #195.#196     // java/nio/ByteOrder.nativeOrder:()Ljava/nio/ByteOrder;
+    #9 = Fieldref           #1.#197       // NpyWriter.nativeByteOrder:Ljava/nio/ByteOrder;
+   #10 = Fieldref           #195.#198     // java/nio/ByteOrder.BIG_ENDIAN:Ljava/nio/ByteOrder;
+   #11 = Fieldref           #1.#199       // NpyWriter.numpyByteOrder:C
+   #12 = Methodref          #200.#201     // java/nio/ByteBuffer.allocate:(I)Ljava/nio/ByteBuffer;
+   #13 = Methodref          #200.#202     // java/nio/ByteBuffer.order:(Ljava/nio/ByteOrder;)Ljava/nio/ByteBuffer;
+   #14 = Fieldref           #1.#203       // NpyWriter.lineBuffer:Ljava/nio/ByteBuffer;
+   #15 = Class              #204          // java/util/ArrayList
+   #16 = Methodref          #15.#189      // java/util/ArrayList."<init>":()V
+   #17 = Fieldref           #1.#205       // NpyWriter.itemTypes:Ljava/util/ArrayList;
+   #18 = Fieldref           #1.#206       // NpyWriter.itemNames:Ljava/util/ArrayList;
+   #19 = Fieldref           #1.#207       // NpyWriter.outputFile:Ljava/lang/String;
+   #20 = Class              #208          // java/io/File
+   #21 = Methodref          #20.#209      // java/io/File."<init>":(Ljava/lang/String;)V
+   #22 = Fieldref           #1.#210       // NpyWriter.file:Ljava/io/File;
+   #23 = Class              #211          // java/io/RandomAccessFile
+   #24 = String             #212          // rw
+   #25 = Methodref          #23.#213      // java/io/RandomAccessFile."<init>":(Ljava/io/File;Ljava/lang/String;)V
+   #26 = Fieldref           #1.#214       // NpyWriter.raf:Ljava/io/RandomAccessFile;
+   #27 = Methodref          #23.#215      // java/io/RandomAccessFile.setLength:(J)V
+   #28 = Fieldref           #1.#216       // NpyWriter.NPY_HEADER:[B
+   #29 = Class              #217          // java/lang/StringBuilder
+   #30 = Methodref          #29.#189      // java/lang/StringBuilder."<init>":()V
+   #31 = Class              #218          // java/lang/String
+   #32 = Methodref          #31.#219      // java/lang/String."<init>":([C)V
+   #33 = String             #220          // \u0000
+   #34 = String             #221          //
+   #35 = Methodref          #31.#222      // java/lang/String.replace:(Ljava/lang/CharSequence;Ljava/lang/CharSequence;)Ljava/lang/String;
+   #36 = Methodref          #29.#223      // java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+   #37 = String             #224          // \n
+   #38 = Methodref          #29.#225      // java/lang/StringBuilder.toString:()Ljava/lang/String;
+   #39 = Methodref          #23.#226      // java/io/RandomAccessFile.writeBytes:(Ljava/lang/String;)V
+   #40 = Methodref          #15.#227      // java/util/ArrayList.add:(Ljava/lang/Object;)Z
+   #41 = String             #228          // time
+   #42 = String             #229          // x
+   #43 = String             #230          // y
+   #44 = String             #231          // z
+   #45 = Class              #232          // java/io/IOException
+   #46 = Class              #233          // java/lang/RuntimeException
+   #47 = String             #234          // The .npy file
+   #48 = String             #235          //  could not be created
+   #49 = Methodref          #46.#209      // java/lang/RuntimeException."<init>":(Ljava/lang/String;)V
+   #50 = Methodref          #200.#236     // java/nio/ByteBuffer.putLong:(J)Ljava/nio/ByteBuffer;
+   #51 = Methodref          #6.#237       // java/lang/Float.floatValue:()F
+   #52 = Methodref          #200.#238     // java/nio/ByteBuffer.putFloat:(F)Ljava/nio/ByteBuffer;
+   #53 = Methodref          #200.#239     // java/nio/ByteBuffer.hasRemaining:()Z
+   #54 = Methodref          #200.#240     // java/nio/ByteBuffer.array:()[B
+   #55 = Methodref          #23.#241      // java/io/RandomAccessFile.write:([B)V
+   #56 = Methodref          #200.#242     // java/nio/ByteBuffer.clear:()Ljava/nio/Buffer;
    #57 = Integer            10000000
-   #58 = Methodref          #1.#239       // NpyWriter.writeHeader:()V
-   #59 = Fieldref           #240.#241     // java/lang/System.out:Ljava/io/PrintStream;
-   #60 = Methodref          #29.#242      // java/lang/StringBuilder.append:(I)Ljava/lang/StringBuilder;
-   #61 = Methodref          #243.#244     // java/io/PrintStream.print:(Ljava/lang/String;)V
-   #62 = Methodref          #23.#245      // java/io/RandomAccessFile.seek:(J)V
-   #63 = Methodref          #23.#246      // java/io/RandomAccessFile.write:(I)V
-   #64 = String             #247          // { \'descr\': [
-   #65 = Methodref          #15.#248      // java/util/ArrayList.size:()I
-   #66 = String             #249          // (\'
-   #67 = Methodref          #15.#250      // java/util/ArrayList.get:(I)Ljava/lang/Object;
-   #68 = String             #251          // \',\'
-   #69 = Class              #252          // java/lang/Class
-   #70 = Methodref          #1.#253       // NpyWriter.toDataTypeStr:(Ljava/lang/Class;)Ljava/lang/String;
-   #71 = String             #254          // \')
-   #72 = String             #255          // ,
-   #73 = String             #256          // ], \'fortran_order\': False, \'shape\': (
-   #74 = String             #257          // ,), }
-   #75 = Methodref          #31.#258      // java/lang/String.length:()I
-   #76 = String             #259          // header is too big to be written.
-   #77 = Methodref          #29.#260      // java/lang/StringBuilder.append:(C)Ljava/lang/StringBuilder;
-   #78 = Methodref          #1.#261       // NpyWriter.writeLEShort:(Ljava/io/RandomAccessFile;S)V
-   #79 = Methodref          #23.#262      // java/io/RandomAccessFile.length:()J
-   #80 = Methodref          #45.#263      // java/io/IOException.printStackTrace:()V
-   #81 = String             #264          // The .npy file could not write a header created
+   #58 = Methodref          #1.#243       // NpyWriter.writeHeader:()V
+   #59 = Fieldref           #244.#245     // java/lang/System.out:Ljava/io/PrintStream;
+   #60 = Methodref          #29.#246      // java/lang/StringBuilder.append:(I)Ljava/lang/StringBuilder;
+   #61 = Methodref          #247.#248     // java/io/PrintStream.print:(Ljava/lang/String;)V
+   #62 = Methodref          #23.#249      // java/io/RandomAccessFile.seek:(J)V
+   #63 = Methodref          #23.#250      // java/io/RandomAccessFile.write:(I)V
+   #64 = String             #251          // { \'descr\': [
+   #65 = Methodref          #15.#252      // java/util/ArrayList.size:()I
+   #66 = String             #253          // (\'
+   #67 = Methodref          #15.#254      // java/util/ArrayList.get:(I)Ljava/lang/Object;
+   #68 = String             #255          // \',\'
+   #69 = Class              #256          // java/lang/Class
+   #70 = Methodref          #1.#257       // NpyWriter.toDataTypeStr:(Ljava/lang/Class;)Ljava/lang/String;
+   #71 = String             #258          // \')
+   #72 = String             #259          // ,
+   #73 = String             #260          // ], \'fortran_order\': False, \'shape\': (
+   #74 = String             #261          // ,), }
+   #75 = Methodref          #31.#262      // java/lang/String.length:()I
+   #76 = String             #263          // header is too big to be written.
+   #77 = Methodref          #29.#264      // java/lang/StringBuilder.append:(C)Ljava/lang/StringBuilder;
+   #78 = Methodref          #1.#265       // NpyWriter.writeLEShort:(Ljava/io/RandomAccessFile;S)V
+   #79 = Methodref          #23.#266      // java/io/RandomAccessFile.length:()J
+   #80 = Methodref          #45.#267      // java/io/IOException.printStackTrace:()V
+   #81 = String             #268          // The .npy file could not write a header created
    #82 = Integer            65280
-   #83 = Methodref          #23.#265      // java/io/RandomAccessFile.writeShort:(I)V
-   #84 = String             #266          // writing:
-   #85 = Methodref          #243.#267     // java/io/PrintStream.println:(Ljava/lang/String;)V
-   #86 = Methodref          #23.#268      // java/io/RandomAccessFile.writeByte:(I)V
-   #87 = Class              #269          // java/lang/Integer
-   #88 = Fieldref           #87.#270      // java/lang/Integer.TYPE:Ljava/lang/Class;
-   #89 = String             #271          // i4
-   #90 = Class              #272          // java/lang/Short
-   #91 = Fieldref           #90.#270      // java/lang/Short.TYPE:Ljava/lang/Class;
-   #92 = String             #273          // i2
-   #93 = Fieldref           #5.#270       // java/lang/Long.TYPE:Ljava/lang/Class;
-   #94 = String             #274          // i8
-   #95 = Fieldref           #6.#270       // java/lang/Float.TYPE:Ljava/lang/Class;
-   #96 = String             #275          // f4
-   #97 = Class              #276          // java/lang/Double
-   #98 = Fieldref           #97.#270      // java/lang/Double.TYPE:Ljava/lang/Class;
-   #99 = String             #277          // f8
-  #100 = Class              #278          // java/lang/IllegalArgumentException
-  #101 = String             #279          // Don\'t know the corresponding Python datatype for
-  #102 = Methodref          #69.#280      // java/lang/Class.getSimpleName:()Ljava/lang/String;
-  #103 = Methodref          #100.#205     // java/lang/IllegalArgumentException."<init>":(Ljava/lang/String;)V
-  #104 = Class              #281          // java/util/zip/GZIPOutputStream
-  #105 = Class              #282          // java/io/FileOutputStream
-  #106 = String             #283          // .gz
-  #107 = Methodref          #105.#284     // java/io/FileOutputStream."<init>":(Ljava/io/File;)V
-  #108 = Methodref          #104.#285     // java/util/zip/GZIPOutputStream."<init>":(Ljava/io/OutputStream;)V
-  #109 = Methodref          #23.#286      // java/io/RandomAccessFile.read:([B)I
-  #110 = Methodref          #104.#287     // java/util/zip/GZIPOutputStream.write:([BII)V
-  #111 = Methodref          #104.#288     // java/util/zip/GZIPOutputStream.close:()V
-  #112 = Fieldref           #1.#289       // NpyWriter.COMPRESS:Ljava/lang/Boolean;
-  #113 = Methodref          #290.#291     // java/lang/Boolean.booleanValue:()Z
-  #114 = String             #292          // \ncompressing .npy file...
-  #115 = Methodref          #1.#293       // NpyWriter.compress:()V
-  #116 = Methodref          #23.#288      // java/io/RandomAccessFile.close:()V
-  #117 = String             #294          // deleting uncompressed .npy file...
-  #118 = Methodref          #20.#295      // java/io/File.delete:()Z
-  #119 = String             #296          // npyWriter was shut down correctly
-  #120 = Methodref          #290.#297     // java/lang/Boolean.valueOf:(Z)Ljava/lang/Boolean;
-  #121 = String             #298          // XNUMPY
-  #122 = Fieldref           #299.#300     // java/nio/charset/StandardCharsets.US_ASCII:Ljava/nio/charset/Charset;
-  #123 = Methodref          #31.#301      // java/lang/String.getBytes:(Ljava/nio/charset/Charset;)[B
-  #124 = Class              #302          // java/lang/Object
+   #83 = Methodref          #23.#269      // java/io/RandomAccessFile.writeShort:(I)V
+   #84 = String             #270          // writing:
+   #85 = Methodref          #247.#271     // java/io/PrintStream.println:(Ljava/lang/String;)V
+   #86 = Methodref          #23.#272      // java/io/RandomAccessFile.writeByte:(I)V
+   #87 = Class              #273          // java/lang/Integer
+   #88 = Fieldref           #87.#274      // java/lang/Integer.TYPE:Ljava/lang/Class;
+   #89 = String             #275          // i4
+   #90 = Class              #276          // java/lang/Short
+   #91 = Fieldref           #90.#274      // java/lang/Short.TYPE:Ljava/lang/Class;
+   #92 = String             #277          // i2
+   #93 = Fieldref           #5.#274       // java/lang/Long.TYPE:Ljava/lang/Class;
+   #94 = String             #278          // i8
+   #95 = Fieldref           #6.#274       // java/lang/Float.TYPE:Ljava/lang/Class;
+   #96 = String             #279          // f4
+   #97 = Class              #280          // java/lang/Double
+   #98 = Fieldref           #97.#274      // java/lang/Double.TYPE:Ljava/lang/Class;
+   #99 = String             #281          // f8
+  #100 = Class              #282          // java/lang/IllegalArgumentException
+  #101 = String             #283          // Don\'t know the corresponding Python datatype for
+  #102 = Methodref          #69.#284      // java/lang/Class.getSimpleName:()Ljava/lang/String;
+  #103 = Methodref          #100.#209     // java/lang/IllegalArgumentException."<init>":(Ljava/lang/String;)V
+  #104 = Class              #285          // java/util/zip/GZIPOutputStream
+  #105 = Class              #286          // java/io/FileOutputStream
+  #106 = String             #287          // .gz
+  #107 = Methodref          #105.#288     // java/io/FileOutputStream."<init>":(Ljava/io/File;)V
+  #108 = Methodref          #104.#289     // java/util/zip/GZIPOutputStream."<init>":(Ljava/io/OutputStream;)V
+  #109 = Methodref          #23.#290      // java/io/RandomAccessFile.read:([B)I
+  #110 = Methodref          #104.#291     // java/util/zip/GZIPOutputStream.write:([BII)V
+  #111 = Methodref          #104.#292     // java/util/zip/GZIPOutputStream.close:()V
+  #112 = Fieldref           #1.#293       // NpyWriter.COMPRESS:Ljava/lang/Boolean;
+  #113 = Methodref          #294.#295     // java/lang/Boolean.booleanValue:()Z
+  #114 = String             #296          // \ncompressing .npy file...
+  #115 = Methodref          #1.#297       // NpyWriter.compress:()V
+  #116 = Methodref          #23.#292      // java/io/RandomAccessFile.close:()V
+  #117 = String             #298          // deleting uncompressed .npy file...
+  #118 = Methodref          #20.#299      // java/io/File.delete:()Z
+  #119 = String             #300          // npyWriter was shut down correctly
+  #120 = Methodref          #294.#301     // java/lang/Boolean.valueOf:(Z)Ljava/lang/Boolean;
+  #121 = String             #302          // XNUMPY
+  #122 = Fieldref           #303.#304     // java/nio/charset/StandardCharsets.US_ASCII:Ljava/nio/charset/Charset;
+  #123 = Methodref          #31.#305      // java/lang/String.getBytes:(Ljava/nio/charset/Charset;)[B
+  #124 = Class              #306          // java/lang/Object
   #125 = Utf8               COMPRESS
   #126 = Utf8               Ljava/lang/Boolean;
   #127 = Utf8               outputFile
   #128 = Utf8               Ljava/lang/String;
   #129 = Utf8               file
   #130 = Utf8               Ljava/io/File;
   #131 = Utf8               raf
@@ -169,224 +169,228 @@
   #159 = Utf8               itemNames
   #160 = Utf8               Ljava/util/ArrayList<Ljava/lang/String;>;
   #161 = Utf8               <init>
   #162 = Utf8               (Ljava/lang/String;)V
   #163 = Utf8               Code
   #164 = Utf8               LineNumberTable
   #165 = Utf8               StackMapTable
-  #166 = Utf8               writeData
-  #167 = Utf8               (JLjava/lang/Float;Ljava/lang/Float;Ljava/lang/Float;)V
-  #168 = Utf8               Exceptions
-  #169 = Utf8               writeHeader
-  #170 = Utf8               ()V
-  #171 = Utf8               writeLEShort
-  #172 = Utf8               (Ljava/io/RandomAccessFile;S)V
-  #173 = Utf8               writeLEInt
-  #174 = Utf8               (Ljava/io/RandomAccessFile;I)V
-  #175 = Utf8               toDataTypeStr
-  #176 = Utf8               (Ljava/lang/Class;)Ljava/lang/String;
-  #177 = Utf8               (Ljava/lang/Class<*>;)Ljava/lang/String;
-  #178 = Utf8               compress
-  #179 = Class              #136          // "[B"
-  #180 = Utf8               close
-  #181 = Utf8               <clinit>
-  #182 = Utf8               SourceFile
-  #183 = Utf8               NpyWriter.java
-  #184 = Utf8               NpyWriter
-  #185 = NameAndType        #161:#170     // "<init>":()V
-  #186 = NameAndType        #133:#134     // linesWritten:I
-  #187 = NameAndType        #147:#134     // bufferLength:I
-  #188 = Utf8               java/lang/Long
-  #189 = Utf8               java/lang/Float
-  #190 = NameAndType        #148:#134     // bytesPerLine:I
-  #191 = Class              #303          // java/nio/ByteOrder
-  #192 = NameAndType        #304:#305     // nativeOrder:()Ljava/nio/ByteOrder;
-  #193 = NameAndType        #149:#150     // nativeByteOrder:Ljava/nio/ByteOrder;
-  #194 = NameAndType        #306:#150     // BIG_ENDIAN:Ljava/nio/ByteOrder;
-  #195 = NameAndType        #151:#152     // numpyByteOrder:C
-  #196 = Class              #307          // java/nio/ByteBuffer
-  #197 = NameAndType        #308:#309     // allocate:(I)Ljava/nio/ByteBuffer;
-  #198 = NameAndType        #310:#311     // order:(Ljava/nio/ByteOrder;)Ljava/nio/ByteBuffer;
-  #199 = NameAndType        #153:#154     // lineBuffer:Ljava/nio/ByteBuffer;
-  #200 = Utf8               java/util/ArrayList
-  #201 = NameAndType        #155:#156     // itemTypes:Ljava/util/ArrayList;
-  #202 = NameAndType        #159:#156     // itemNames:Ljava/util/ArrayList;
-  #203 = NameAndType        #127:#128     // outputFile:Ljava/lang/String;
-  #204 = Utf8               java/io/File
-  #205 = NameAndType        #161:#162     // "<init>":(Ljava/lang/String;)V
-  #206 = NameAndType        #129:#130     // file:Ljava/io/File;
-  #207 = Utf8               java/io/RandomAccessFile
-  #208 = Utf8               rw
-  #209 = NameAndType        #161:#312     // "<init>":(Ljava/io/File;Ljava/lang/String;)V
-  #210 = NameAndType        #131:#132     // raf:Ljava/io/RandomAccessFile;
-  #211 = NameAndType        #313:#314     // setLength:(J)V
-  #212 = NameAndType        #135:#136     // NPY_HEADER:[B
-  #213 = Utf8               java/lang/StringBuilder
-  #214 = Utf8               java/lang/String
-  #215 = NameAndType        #161:#315     // "<init>":([C)V
-  #216 = Utf8               \u0000
-  #217 = Utf8
-  #218 = NameAndType        #316:#317     // replace:(Ljava/lang/CharSequence;Ljava/lang/CharSequence;)Ljava/lang/String;
-  #219 = NameAndType        #318:#319     // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #220 = Utf8               \n
-  #221 = NameAndType        #320:#321     // toString:()Ljava/lang/String;
-  #222 = NameAndType        #322:#162     // writeBytes:(Ljava/lang/String;)V
-  #223 = NameAndType        #323:#324     // add:(Ljava/lang/Object;)Z
-  #224 = Utf8               time
-  #225 = Utf8               x
-  #226 = Utf8               y
-  #227 = Utf8               z
-  #228 = Utf8               java/io/IOException
-  #229 = Utf8               java/lang/RuntimeException
-  #230 = Utf8               The .npy file
-  #231 = Utf8                could not be created
-  #232 = NameAndType        #325:#326     // putLong:(J)Ljava/nio/ByteBuffer;
-  #233 = NameAndType        #327:#328     // floatValue:()F
-  #234 = NameAndType        #329:#330     // putFloat:(F)Ljava/nio/ByteBuffer;
-  #235 = NameAndType        #331:#332     // hasRemaining:()Z
-  #236 = NameAndType        #333:#334     // array:()[B
-  #237 = NameAndType        #335:#336     // write:([B)V
-  #238 = NameAndType        #337:#338     // clear:()Ljava/nio/Buffer;
-  #239 = NameAndType        #169:#170     // writeHeader:()V
-  #240 = Class              #339          // java/lang/System
-  #241 = NameAndType        #340:#341     // out:Ljava/io/PrintStream;
-  #242 = NameAndType        #318:#342     // append:(I)Ljava/lang/StringBuilder;
-  #243 = Class              #343          // java/io/PrintStream
-  #244 = NameAndType        #344:#162     // print:(Ljava/lang/String;)V
-  #245 = NameAndType        #345:#314     // seek:(J)V
-  #246 = NameAndType        #335:#346     // write:(I)V
-  #247 = Utf8               { \'descr\': [
-  #248 = NameAndType        #347:#348     // size:()I
-  #249 = Utf8               (\'
-  #250 = NameAndType        #349:#350     // get:(I)Ljava/lang/Object;
-  #251 = Utf8               \',\'
-  #252 = Utf8               java/lang/Class
-  #253 = NameAndType        #175:#176     // toDataTypeStr:(Ljava/lang/Class;)Ljava/lang/String;
-  #254 = Utf8               \')
-  #255 = Utf8               ,
-  #256 = Utf8               ], \'fortran_order\': False, \'shape\': (
-  #257 = Utf8               ,), }
-  #258 = NameAndType        #351:#348     // length:()I
-  #259 = Utf8               header is too big to be written.
-  #260 = NameAndType        #318:#352     // append:(C)Ljava/lang/StringBuilder;
-  #261 = NameAndType        #171:#172     // writeLEShort:(Ljava/io/RandomAccessFile;S)V
-  #262 = NameAndType        #351:#353     // length:()J
-  #263 = NameAndType        #354:#170     // printStackTrace:()V
-  #264 = Utf8               The .npy file could not write a header created
-  #265 = NameAndType        #355:#346     // writeShort:(I)V
-  #266 = Utf8               writing:
-  #267 = NameAndType        #356:#162     // println:(Ljava/lang/String;)V
-  #268 = NameAndType        #357:#346     // writeByte:(I)V
-  #269 = Utf8               java/lang/Integer
-  #270 = NameAndType        #358:#359     // TYPE:Ljava/lang/Class;
-  #271 = Utf8               i4
-  #272 = Utf8               java/lang/Short
-  #273 = Utf8               i2
-  #274 = Utf8               i8
-  #275 = Utf8               f4
-  #276 = Utf8               java/lang/Double
-  #277 = Utf8               f8
-  #278 = Utf8               java/lang/IllegalArgumentException
-  #279 = Utf8               Don\'t know the corresponding Python datatype for
-  #280 = NameAndType        #360:#321     // getSimpleName:()Ljava/lang/String;
-  #281 = Utf8               java/util/zip/GZIPOutputStream
-  #282 = Utf8               java/io/FileOutputStream
-  #283 = Utf8               .gz
-  #284 = NameAndType        #161:#361     // "<init>":(Ljava/io/File;)V
-  #285 = NameAndType        #161:#362     // "<init>":(Ljava/io/OutputStream;)V
-  #286 = NameAndType        #363:#364     // read:([B)I
-  #287 = NameAndType        #335:#365     // write:([BII)V
-  #288 = NameAndType        #180:#170     // close:()V
-  #289 = NameAndType        #125:#126     // COMPRESS:Ljava/lang/Boolean;
-  #290 = Class              #366          // java/lang/Boolean
-  #291 = NameAndType        #367:#332     // booleanValue:()Z
-  #292 = Utf8               \ncompressing .npy file...
-  #293 = NameAndType        #178:#170     // compress:()V
-  #294 = Utf8               deleting uncompressed .npy file...
-  #295 = NameAndType        #368:#332     // delete:()Z
-  #296 = Utf8               npyWriter was shut down correctly
-  #297 = NameAndType        #369:#370     // valueOf:(Z)Ljava/lang/Boolean;
-  #298 = Utf8               XNUMPY
-  #299 = Class              #371          // java/nio/charset/StandardCharsets
-  #300 = NameAndType        #372:#373     // US_ASCII:Ljava/nio/charset/Charset;
-  #301 = NameAndType        #374:#375     // getBytes:(Ljava/nio/charset/Charset;)[B
-  #302 = Utf8               java/lang/Object
-  #303 = Utf8               java/nio/ByteOrder
-  #304 = Utf8               nativeOrder
-  #305 = Utf8               ()Ljava/nio/ByteOrder;
-  #306 = Utf8               BIG_ENDIAN
-  #307 = Utf8               java/nio/ByteBuffer
-  #308 = Utf8               allocate
-  #309 = Utf8               (I)Ljava/nio/ByteBuffer;
-  #310 = Utf8               order
-  #311 = Utf8               (Ljava/nio/ByteOrder;)Ljava/nio/ByteBuffer;
-  #312 = Utf8               (Ljava/io/File;Ljava/lang/String;)V
-  #313 = Utf8               setLength
-  #314 = Utf8               (J)V
-  #315 = Utf8               ([C)V
-  #316 = Utf8               replace
-  #317 = Utf8               (Ljava/lang/CharSequence;Ljava/lang/CharSequence;)Ljava/lang/String;
-  #318 = Utf8               append
-  #319 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
-  #320 = Utf8               toString
-  #321 = Utf8               ()Ljava/lang/String;
-  #322 = Utf8               writeBytes
-  #323 = Utf8               add
-  #324 = Utf8               (Ljava/lang/Object;)Z
-  #325 = Utf8               putLong
-  #326 = Utf8               (J)Ljava/nio/ByteBuffer;
-  #327 = Utf8               floatValue
-  #328 = Utf8               ()F
-  #329 = Utf8               putFloat
-  #330 = Utf8               (F)Ljava/nio/ByteBuffer;
-  #331 = Utf8               hasRemaining
-  #332 = Utf8               ()Z
-  #333 = Utf8               array
-  #334 = Utf8               ()[B
-  #335 = Utf8               write
-  #336 = Utf8               ([B)V
-  #337 = Utf8               clear
-  #338 = Utf8               ()Ljava/nio/Buffer;
-  #339 = Utf8               java/lang/System
-  #340 = Utf8               out
-  #341 = Utf8               Ljava/io/PrintStream;
-  #342 = Utf8               (I)Ljava/lang/StringBuilder;
-  #343 = Utf8               java/io/PrintStream
-  #344 = Utf8               print
-  #345 = Utf8               seek
-  #346 = Utf8               (I)V
-  #347 = Utf8               size
-  #348 = Utf8               ()I
-  #349 = Utf8               get
-  #350 = Utf8               (I)Ljava/lang/Object;
-  #351 = Utf8               length
-  #352 = Utf8               (C)Ljava/lang/StringBuilder;
-  #353 = Utf8               ()J
-  #354 = Utf8               printStackTrace
-  #355 = Utf8               writeShort
-  #356 = Utf8               println
-  #357 = Utf8               writeByte
-  #358 = Utf8               TYPE
-  #359 = Utf8               Ljava/lang/Class;
-  #360 = Utf8               getSimpleName
-  #361 = Utf8               (Ljava/io/File;)V
-  #362 = Utf8               (Ljava/io/OutputStream;)V
-  #363 = Utf8               read
-  #364 = Utf8               ([B)I
-  #365 = Utf8               ([BII)V
-  #366 = Utf8               java/lang/Boolean
-  #367 = Utf8               booleanValue
-  #368 = Utf8               delete
-  #369 = Utf8               valueOf
-  #370 = Utf8               (Z)Ljava/lang/Boolean;
-  #371 = Utf8               java/nio/charset/StandardCharsets
-  #372 = Utf8               US_ASCII
-  #373 = Utf8               Ljava/nio/charset/Charset;
-  #374 = Utf8               getBytes
-  #375 = Utf8               (Ljava/nio/charset/Charset;)[B
+  #166 = Class              #188          // NpyWriter
+  #167 = Class              #218          // java/lang/String
+  #168 = Class              #232          // java/io/IOException
+  #169 = Utf8               writeData
+  #170 = Utf8               (JLjava/lang/Float;Ljava/lang/Float;Ljava/lang/Float;)V
+  #171 = Utf8               Exceptions
+  #172 = Utf8               writeHeader
+  #173 = Utf8               ()V
+  #174 = Utf8               writeLEShort
+  #175 = Utf8               (Ljava/io/RandomAccessFile;S)V
+  #176 = Utf8               writeLEInt
+  #177 = Utf8               (Ljava/io/RandomAccessFile;I)V
+  #178 = Utf8               toDataTypeStr
+  #179 = Utf8               (Ljava/lang/Class;)Ljava/lang/String;
+  #180 = Utf8               (Ljava/lang/Class<*>;)Ljava/lang/String;
+  #181 = Utf8               compress
+  #182 = Class              #285          // java/util/zip/GZIPOutputStream
+  #183 = Class              #136          // "[B"
+  #184 = Utf8               close
+  #185 = Utf8               <clinit>
+  #186 = Utf8               SourceFile
+  #187 = Utf8               NpyWriter.java
+  #188 = Utf8               NpyWriter
+  #189 = NameAndType        #161:#173     // "<init>":()V
+  #190 = NameAndType        #133:#134     // linesWritten:I
+  #191 = NameAndType        #147:#134     // bufferLength:I
+  #192 = Utf8               java/lang/Long
+  #193 = Utf8               java/lang/Float
+  #194 = NameAndType        #148:#134     // bytesPerLine:I
+  #195 = Class              #307          // java/nio/ByteOrder
+  #196 = NameAndType        #308:#309     // nativeOrder:()Ljava/nio/ByteOrder;
+  #197 = NameAndType        #149:#150     // nativeByteOrder:Ljava/nio/ByteOrder;
+  #198 = NameAndType        #310:#150     // BIG_ENDIAN:Ljava/nio/ByteOrder;
+  #199 = NameAndType        #151:#152     // numpyByteOrder:C
+  #200 = Class              #311          // java/nio/ByteBuffer
+  #201 = NameAndType        #312:#313     // allocate:(I)Ljava/nio/ByteBuffer;
+  #202 = NameAndType        #314:#315     // order:(Ljava/nio/ByteOrder;)Ljava/nio/ByteBuffer;
+  #203 = NameAndType        #153:#154     // lineBuffer:Ljava/nio/ByteBuffer;
+  #204 = Utf8               java/util/ArrayList
+  #205 = NameAndType        #155:#156     // itemTypes:Ljava/util/ArrayList;
+  #206 = NameAndType        #159:#156     // itemNames:Ljava/util/ArrayList;
+  #207 = NameAndType        #127:#128     // outputFile:Ljava/lang/String;
+  #208 = Utf8               java/io/File
+  #209 = NameAndType        #161:#162     // "<init>":(Ljava/lang/String;)V
+  #210 = NameAndType        #129:#130     // file:Ljava/io/File;
+  #211 = Utf8               java/io/RandomAccessFile
+  #212 = Utf8               rw
+  #213 = NameAndType        #161:#316     // "<init>":(Ljava/io/File;Ljava/lang/String;)V
+  #214 = NameAndType        #131:#132     // raf:Ljava/io/RandomAccessFile;
+  #215 = NameAndType        #317:#318     // setLength:(J)V
+  #216 = NameAndType        #135:#136     // NPY_HEADER:[B
+  #217 = Utf8               java/lang/StringBuilder
+  #218 = Utf8               java/lang/String
+  #219 = NameAndType        #161:#319     // "<init>":([C)V
+  #220 = Utf8               \u0000
+  #221 = Utf8
+  #222 = NameAndType        #320:#321     // replace:(Ljava/lang/CharSequence;Ljava/lang/CharSequence;)Ljava/lang/String;
+  #223 = NameAndType        #322:#323     // append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #224 = Utf8               \n
+  #225 = NameAndType        #324:#325     // toString:()Ljava/lang/String;
+  #226 = NameAndType        #326:#162     // writeBytes:(Ljava/lang/String;)V
+  #227 = NameAndType        #327:#328     // add:(Ljava/lang/Object;)Z
+  #228 = Utf8               time
+  #229 = Utf8               x
+  #230 = Utf8               y
+  #231 = Utf8               z
+  #232 = Utf8               java/io/IOException
+  #233 = Utf8               java/lang/RuntimeException
+  #234 = Utf8               The .npy file
+  #235 = Utf8                could not be created
+  #236 = NameAndType        #329:#330     // putLong:(J)Ljava/nio/ByteBuffer;
+  #237 = NameAndType        #331:#332     // floatValue:()F
+  #238 = NameAndType        #333:#334     // putFloat:(F)Ljava/nio/ByteBuffer;
+  #239 = NameAndType        #335:#336     // hasRemaining:()Z
+  #240 = NameAndType        #337:#338     // array:()[B
+  #241 = NameAndType        #339:#340     // write:([B)V
+  #242 = NameAndType        #341:#342     // clear:()Ljava/nio/Buffer;
+  #243 = NameAndType        #172:#173     // writeHeader:()V
+  #244 = Class              #343          // java/lang/System
+  #245 = NameAndType        #344:#345     // out:Ljava/io/PrintStream;
+  #246 = NameAndType        #322:#346     // append:(I)Ljava/lang/StringBuilder;
+  #247 = Class              #347          // java/io/PrintStream
+  #248 = NameAndType        #348:#162     // print:(Ljava/lang/String;)V
+  #249 = NameAndType        #349:#318     // seek:(J)V
+  #250 = NameAndType        #339:#350     // write:(I)V
+  #251 = Utf8               { \'descr\': [
+  #252 = NameAndType        #351:#352     // size:()I
+  #253 = Utf8               (\'
+  #254 = NameAndType        #353:#354     // get:(I)Ljava/lang/Object;
+  #255 = Utf8               \',\'
+  #256 = Utf8               java/lang/Class
+  #257 = NameAndType        #178:#179     // toDataTypeStr:(Ljava/lang/Class;)Ljava/lang/String;
+  #258 = Utf8               \')
+  #259 = Utf8               ,
+  #260 = Utf8               ], \'fortran_order\': False, \'shape\': (
+  #261 = Utf8               ,), }
+  #262 = NameAndType        #355:#352     // length:()I
+  #263 = Utf8               header is too big to be written.
+  #264 = NameAndType        #322:#356     // append:(C)Ljava/lang/StringBuilder;
+  #265 = NameAndType        #174:#175     // writeLEShort:(Ljava/io/RandomAccessFile;S)V
+  #266 = NameAndType        #355:#357     // length:()J
+  #267 = NameAndType        #358:#173     // printStackTrace:()V
+  #268 = Utf8               The .npy file could not write a header created
+  #269 = NameAndType        #359:#350     // writeShort:(I)V
+  #270 = Utf8               writing:
+  #271 = NameAndType        #360:#162     // println:(Ljava/lang/String;)V
+  #272 = NameAndType        #361:#350     // writeByte:(I)V
+  #273 = Utf8               java/lang/Integer
+  #274 = NameAndType        #362:#363     // TYPE:Ljava/lang/Class;
+  #275 = Utf8               i4
+  #276 = Utf8               java/lang/Short
+  #277 = Utf8               i2
+  #278 = Utf8               i8
+  #279 = Utf8               f4
+  #280 = Utf8               java/lang/Double
+  #281 = Utf8               f8
+  #282 = Utf8               java/lang/IllegalArgumentException
+  #283 = Utf8               Don\'t know the corresponding Python datatype for
+  #284 = NameAndType        #364:#325     // getSimpleName:()Ljava/lang/String;
+  #285 = Utf8               java/util/zip/GZIPOutputStream
+  #286 = Utf8               java/io/FileOutputStream
+  #287 = Utf8               .gz
+  #288 = NameAndType        #161:#365     // "<init>":(Ljava/io/File;)V
+  #289 = NameAndType        #161:#366     // "<init>":(Ljava/io/OutputStream;)V
+  #290 = NameAndType        #367:#368     // read:([B)I
+  #291 = NameAndType        #339:#369     // write:([BII)V
+  #292 = NameAndType        #184:#173     // close:()V
+  #293 = NameAndType        #125:#126     // COMPRESS:Ljava/lang/Boolean;
+  #294 = Class              #370          // java/lang/Boolean
+  #295 = NameAndType        #371:#336     // booleanValue:()Z
+  #296 = Utf8               \ncompressing .npy file...
+  #297 = NameAndType        #181:#173     // compress:()V
+  #298 = Utf8               deleting uncompressed .npy file...
+  #299 = NameAndType        #372:#336     // delete:()Z
+  #300 = Utf8               npyWriter was shut down correctly
+  #301 = NameAndType        #373:#374     // valueOf:(Z)Ljava/lang/Boolean;
+  #302 = Utf8               XNUMPY
+  #303 = Class              #375          // java/nio/charset/StandardCharsets
+  #304 = NameAndType        #376:#377     // US_ASCII:Ljava/nio/charset/Charset;
+  #305 = NameAndType        #378:#379     // getBytes:(Ljava/nio/charset/Charset;)[B
+  #306 = Utf8               java/lang/Object
+  #307 = Utf8               java/nio/ByteOrder
+  #308 = Utf8               nativeOrder
+  #309 = Utf8               ()Ljava/nio/ByteOrder;
+  #310 = Utf8               BIG_ENDIAN
+  #311 = Utf8               java/nio/ByteBuffer
+  #312 = Utf8               allocate
+  #313 = Utf8               (I)Ljava/nio/ByteBuffer;
+  #314 = Utf8               order
+  #315 = Utf8               (Ljava/nio/ByteOrder;)Ljava/nio/ByteBuffer;
+  #316 = Utf8               (Ljava/io/File;Ljava/lang/String;)V
+  #317 = Utf8               setLength
+  #318 = Utf8               (J)V
+  #319 = Utf8               ([C)V
+  #320 = Utf8               replace
+  #321 = Utf8               (Ljava/lang/CharSequence;Ljava/lang/CharSequence;)Ljava/lang/String;
+  #322 = Utf8               append
+  #323 = Utf8               (Ljava/lang/String;)Ljava/lang/StringBuilder;
+  #324 = Utf8               toString
+  #325 = Utf8               ()Ljava/lang/String;
+  #326 = Utf8               writeBytes
+  #327 = Utf8               add
+  #328 = Utf8               (Ljava/lang/Object;)Z
+  #329 = Utf8               putLong
+  #330 = Utf8               (J)Ljava/nio/ByteBuffer;
+  #331 = Utf8               floatValue
+  #332 = Utf8               ()F
+  #333 = Utf8               putFloat
+  #334 = Utf8               (F)Ljava/nio/ByteBuffer;
+  #335 = Utf8               hasRemaining
+  #336 = Utf8               ()Z
+  #337 = Utf8               array
+  #338 = Utf8               ()[B
+  #339 = Utf8               write
+  #340 = Utf8               ([B)V
+  #341 = Utf8               clear
+  #342 = Utf8               ()Ljava/nio/Buffer;
+  #343 = Utf8               java/lang/System
+  #344 = Utf8               out
+  #345 = Utf8               Ljava/io/PrintStream;
+  #346 = Utf8               (I)Ljava/lang/StringBuilder;
+  #347 = Utf8               java/io/PrintStream
+  #348 = Utf8               print
+  #349 = Utf8               seek
+  #350 = Utf8               (I)V
+  #351 = Utf8               size
+  #352 = Utf8               ()I
+  #353 = Utf8               get
+  #354 = Utf8               (I)Ljava/lang/Object;
+  #355 = Utf8               length
+  #356 = Utf8               (C)Ljava/lang/StringBuilder;
+  #357 = Utf8               ()J
+  #358 = Utf8               printStackTrace
+  #359 = Utf8               writeShort
+  #360 = Utf8               println
+  #361 = Utf8               writeByte
+  #362 = Utf8               TYPE
+  #363 = Utf8               Ljava/lang/Class;
+  #364 = Utf8               getSimpleName
+  #365 = Utf8               (Ljava/io/File;)V
+  #366 = Utf8               (Ljava/io/OutputStream;)V
+  #367 = Utf8               read
+  #368 = Utf8               ([B)I
+  #369 = Utf8               ([BII)V
+  #370 = Utf8               java/lang/Boolean
+  #371 = Utf8               booleanValue
+  #372 = Utf8               delete
+  #373 = Utf8               valueOf
+  #374 = Utf8               (Z)Ljava/lang/Boolean;
+  #375 = Utf8               java/nio/charset/StandardCharsets
+  #376 = Utf8               US_ASCII
+  #377 = Utf8               Ljava/nio/charset/Charset;
+  #378 = Utf8               getBytes
+  #379 = Utf8               (Ljava/nio/charset/Charset;)[B
 {
   private static final java.lang.Boolean COMPRESS;
     descriptor: Ljava/lang/Boolean;
     flags: (0x001a) ACC_PRIVATE, ACC_STATIC, ACC_FINAL
 
   private java.lang.String outputFile;
     descriptor: Ljava/lang/String;
@@ -1129,15 +1133,15 @@
         frame_type = 22 /* same */
         frame_type = 12 /* same */
         frame_type = 22 /* same */
         frame_type = 12 /* same */
         frame_type = 22 /* same */
         frame_type = 12 /* same */
         frame_type = 22 /* same */
-    Signature: #177                         // (Ljava/lang/Class<*>;)Ljava/lang/String;
+    Signature: #180                         // (Ljava/lang/Class<*>;)Ljava/lang/String;
 
   private void compress();
     descriptor: ()V
     flags: (0x0002) ACC_PRIVATE
     Code:
       stack=8, locals=4, args_size=1
          0: new           #104                // class java/util/zip/GZIPOutputStream
```

### Comparing `accelerometer-6.2.3/accelerometer/java/NpyWriter.java` & `accelerometer-7.0.0.dev0/src/accelerometer/java/NpyWriter.java`

 * *Files identical despite different names*

### Comparing `accelerometer-6.2.3/accelerometer/java/Resample.class` & `accelerometer-7.0.0.dev0/src/accelerometer/java/Resample.class`

 * *Files 6% similar despite different names*

#### javap -verbose -constants -s -l -private {}

```diff
@@ -1,90 +1,91 @@
-  SHA-256 checksum 6f983720d49ca1b94726e17a63e862eb197a1f418e11759326b0fdee6c5ec038
+  SHA-256 checksum a4fa0cd4aec1234932461af77173bbcffc4890d2152c68d70f0ea62d4409cb15
   Compiled from "Resample.java"
 public class Resample
   minor version: 0
   major version: 52
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #16                         // Resample
   super_class: #17                        // java/lang/Object
   interfaces: 0, fields: 0, methods: 4, attributes: 1
 Constant pool:
    #1 = Methodref          #17.#37        // java/lang/Object."<init>":()V
-   #2 = InterfaceMethodref #25.#38        // java/util/List.size:()I
-   #3 = Class              #39            // java/lang/IllegalArgumentException
-   #4 = String             #40            // time and x must be the same length
-   #5 = Methodref          #3.#41         // java/lang/IllegalArgumentException."<init>":(Ljava/lang/String;)V
-   #6 = String             #42            // time must contain more than one value
-   #7 = InterfaceMethodref #25.#43        // java/util/List.get:(I)Ljava/lang/Object;
-   #8 = Class              #44            // java/lang/Long
-   #9 = Methodref          #8.#45         // java/lang/Long.longValue:()J
-  #10 = Methodref          #8.#46         // java/lang/Long.valueOf:(J)Ljava/lang/Long;
-  #11 = InterfaceMethodref #25.#47        // java/util/List.set:(ILjava/lang/Object;)Ljava/lang/Object;
-  #12 = Class              #48            // java/lang/Double
-  #13 = Methodref          #12.#49        // java/lang/Double.doubleValue:()D
-  #14 = Methodref          #50.#51        // java/util/Collections.binarySearch:(Ljava/util/List;Ljava/lang/Object;)I
-  #15 = Methodref          #16.#52        // Resample.nearestIndex:(Ljava/util/List;J)I
-  #16 = Class              #53            // Resample
-  #17 = Class              #54            // java/lang/Object
+   #2 = InterfaceMethodref #38.#39        // java/util/List.size:()I
+   #3 = Class              #40            // java/lang/IllegalArgumentException
+   #4 = String             #41            // time and x must be the same length
+   #5 = Methodref          #3.#42         // java/lang/IllegalArgumentException."<init>":(Ljava/lang/String;)V
+   #6 = String             #43            // time must contain more than one value
+   #7 = InterfaceMethodref #38.#44        // java/util/List.get:(I)Ljava/lang/Object;
+   #8 = Class              #45            // java/lang/Long
+   #9 = Methodref          #8.#46         // java/lang/Long.longValue:()J
+  #10 = Methodref          #8.#47         // java/lang/Long.valueOf:(J)Ljava/lang/Long;
+  #11 = InterfaceMethodref #38.#48        // java/util/List.set:(ILjava/lang/Object;)Ljava/lang/Object;
+  #12 = Class              #49            // java/lang/Double
+  #13 = Methodref          #12.#50        // java/lang/Double.doubleValue:()D
+  #14 = Methodref          #51.#52        // java/util/Collections.binarySearch:(Ljava/util/List;Ljava/lang/Object;)I
+  #15 = Methodref          #16.#53        // Resample.nearestIndex:(Ljava/util/List;J)I
+  #16 = Class              #54            // Resample
+  #17 = Class              #55            // java/lang/Object
   #18 = Utf8               <init>
   #19 = Utf8               ()V
   #20 = Utf8               Code
   #21 = Utf8               LineNumberTable
   #22 = Utf8               interpLinear
   #23 = Utf8               (Ljava/util/List;Ljava/util/List;Ljava/util/List;Ljava/util/List;[J[D[D[D)V
   #24 = Utf8               StackMapTable
-  #25 = Class              #55            // java/util/List
-  #26 = Class              #56            // "[J"
-  #27 = Class              #57            // "[D"
+  #25 = Class              #56            // java/util/List
+  #26 = Class              #57            // "[J"
+  #27 = Class              #58            // "[D"
   #28 = Utf8               Exceptions
   #29 = Utf8               Signature
   #30 = Utf8               (Ljava/util/List<Ljava/lang/Long;>;Ljava/util/List<Ljava/lang/Double;>;Ljava/util/List<Ljava/lang/Double;>;Ljava/util/List<Ljava/lang/Double;>;[J[D[D[D)V
   #31 = Utf8               interpNearest
   #32 = Utf8               nearestIndex
   #33 = Utf8               (Ljava/util/List;J)I
   #34 = Utf8               (Ljava/util/List<Ljava/lang/Long;>;J)I
   #35 = Utf8               SourceFile
   #36 = Utf8               Resample.java
   #37 = NameAndType        #18:#19        // "<init>":()V
-  #38 = NameAndType        #58:#59        // size:()I
-  #39 = Utf8               java/lang/IllegalArgumentException
-  #40 = Utf8               time and x must be the same length
-  #41 = NameAndType        #18:#60        // "<init>":(Ljava/lang/String;)V
-  #42 = Utf8               time must contain more than one value
-  #43 = NameAndType        #61:#62        // get:(I)Ljava/lang/Object;
-  #44 = Utf8               java/lang/Long
-  #45 = NameAndType        #63:#64        // longValue:()J
-  #46 = NameAndType        #65:#66        // valueOf:(J)Ljava/lang/Long;
-  #47 = NameAndType        #67:#68        // set:(ILjava/lang/Object;)Ljava/lang/Object;
-  #48 = Utf8               java/lang/Double
-  #49 = NameAndType        #69:#70        // doubleValue:()D
-  #50 = Class              #71            // java/util/Collections
-  #51 = NameAndType        #72:#73        // binarySearch:(Ljava/util/List;Ljava/lang/Object;)I
-  #52 = NameAndType        #32:#33        // nearestIndex:(Ljava/util/List;J)I
-  #53 = Utf8               Resample
-  #54 = Utf8               java/lang/Object
-  #55 = Utf8               java/util/List
-  #56 = Utf8               [J
-  #57 = Utf8               [D
-  #58 = Utf8               size
-  #59 = Utf8               ()I
-  #60 = Utf8               (Ljava/lang/String;)V
-  #61 = Utf8               get
-  #62 = Utf8               (I)Ljava/lang/Object;
-  #63 = Utf8               longValue
-  #64 = Utf8               ()J
-  #65 = Utf8               valueOf
-  #66 = Utf8               (J)Ljava/lang/Long;
-  #67 = Utf8               set
-  #68 = Utf8               (ILjava/lang/Object;)Ljava/lang/Object;
-  #69 = Utf8               doubleValue
-  #70 = Utf8               ()D
-  #71 = Utf8               java/util/Collections
-  #72 = Utf8               binarySearch
-  #73 = Utf8               (Ljava/util/List;Ljava/lang/Object;)I
+  #38 = Class              #56            // java/util/List
+  #39 = NameAndType        #59:#60        // size:()I
+  #40 = Utf8               java/lang/IllegalArgumentException
+  #41 = Utf8               time and x must be the same length
+  #42 = NameAndType        #18:#61        // "<init>":(Ljava/lang/String;)V
+  #43 = Utf8               time must contain more than one value
+  #44 = NameAndType        #62:#63        // get:(I)Ljava/lang/Object;
+  #45 = Utf8               java/lang/Long
+  #46 = NameAndType        #64:#65        // longValue:()J
+  #47 = NameAndType        #66:#67        // valueOf:(J)Ljava/lang/Long;
+  #48 = NameAndType        #68:#69        // set:(ILjava/lang/Object;)Ljava/lang/Object;
+  #49 = Utf8               java/lang/Double
+  #50 = NameAndType        #70:#71        // doubleValue:()D
+  #51 = Class              #72            // java/util/Collections
+  #52 = NameAndType        #73:#74        // binarySearch:(Ljava/util/List;Ljava/lang/Object;)I
+  #53 = NameAndType        #32:#33        // nearestIndex:(Ljava/util/List;J)I
+  #54 = Utf8               Resample
+  #55 = Utf8               java/lang/Object
+  #56 = Utf8               java/util/List
+  #57 = Utf8               [J
+  #58 = Utf8               [D
+  #59 = Utf8               size
+  #60 = Utf8               ()I
+  #61 = Utf8               (Ljava/lang/String;)V
+  #62 = Utf8               get
+  #63 = Utf8               (I)Ljava/lang/Object;
+  #64 = Utf8               longValue
+  #65 = Utf8               ()J
+  #66 = Utf8               valueOf
+  #67 = Utf8               (J)Ljava/lang/Long;
+  #68 = Utf8               set
+  #69 = Utf8               (ILjava/lang/Object;)Ljava/lang/Object;
+  #70 = Utf8               doubleValue
+  #71 = Utf8               ()D
+  #72 = Utf8               java/util/Collections
+  #73 = Utf8               binarySearch
+  #74 = Utf8               (Ljava/util/List;Ljava/lang/Object;)I
 {
   public Resample();
     descriptor: ()V
     flags: (0x0001) ACC_PUBLIC
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
@@ -728,16 +729,14 @@
       LineNumberTable:
         line 113: 0
         line 114: 20
         line 116: 54
         line 117: 63
         line 119: 69
         line 120: 75
-        line 121: 113
-        line 120: 122
       StackMapTable: number_of_entries = 5
         frame_type = 20 /* same */
         frame_type = 33 /* same */
         frame_type = 252 /* append */
           offset_delta = 14
           locals = [ int ]
         frame_type = 252 /* append */
```

### Comparing `accelerometer-6.2.3/accelerometer/java/Resample.java` & `accelerometer-7.0.0.dev0/src/accelerometer/java/Resample.java`

 * *Files identical despite different names*

### Comparing `accelerometer-6.2.3/accelerometer/models.py` & `accelerometer-7.0.0.dev0/src/accelerometer/models.py`

 * *Files identical despite different names*

### Comparing `accelerometer-6.2.3/accelerometer/summarisation.py` & `accelerometer-7.0.0.dev0/src/accelerometer/summarisation.py`

 * *Files identical despite different names*

### Comparing `accelerometer-6.2.3/accelerometer/utils.py` & `accelerometer-7.0.0.dev0/src/accelerometer/utils.py`

 * *Files identical despite different names*

### Comparing `accelerometer-6.2.3/accelerometer.egg-info/PKG-INFO` & `accelerometer-7.0.0.dev0/src/accelerometer.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 Metadata-Version: 2.1
 Name: accelerometer
-Version: 6.2.3
+Version: 7.0.0.dev0
 Summary: A package to extract meaningful health information from large accelerometer datasets e.g. how much time individuals spend in sleep, sedentary behaviour, walking and moderate intensity physical activity
 Home-page: https://github.com/activityMonitoring/biobankAccelerometerAnalysis
+Download-URL: https://github.com/activityMonitoring/biobankAccelerometerAnalysis
 Author: Aiden Doherty, Shing Chan, Rosemary Walmsley, Hang Yuan
-Author-email: aiden.doherty@ndph.ox.ac.uk, shing.chan@ndph.ox.ac.uk, rosemary.walmsley@gtc.ox.ac.uk, hang.yuan@keble.ox.ac.uk
+Maintainer: Shing Chan
+Maintainer-email: shing.chan@ndph.ox.ac.uk
+License: See LICENSE.md
+Keywords: wearables,accelerometer,health data science,human activity recognition
 Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Unix
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE.md
 
 ![Accelerometer data processing overview](docs/source/accelerometerLogo.png)
```

### Comparing `accelerometer-6.2.3/setup.py` & `accelerometer-7.0.0.dev0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,58 @@
+import sys
+import os.path
+# https://github.com/python-versioneer/python-versioneer/issues/193
+sys.path.insert(0, os.path.dirname(__file__))
+
 import setuptools
 import codecs
-import os.path
+
+import versioneer
+
 
 def read(rel_path):
     here = os.path.abspath(os.path.dirname(__file__))
     with codecs.open(os.path.join(here, rel_path), 'r') as fp:
         return fp.read()
 
-def get_string(string, rel_path="accelerometer/__init__.py"):
+def get_string(string, rel_path="src/accelerometer/__init__.py"):
     for line in read(rel_path).splitlines():
         if line.startswith(string):
             delim = '"' if '"' in line else "'"
             return line.split(delim)[1]
     else:
         raise RuntimeError(f"Unable to find {string}.")
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="accelerometer",
     python_requires=">=3.7",
-    version=get_string("__version__"),
-    author=get_string("__author__"),
-    author_email=get_string("__email__"),
+    version=versioneer.get_version(),
+    cmdclass=versioneer.get_cmdclass(),
     description="A package to extract meaningful health information from large accelerometer datasets e.g. how much time individuals spend in sleep, sedentary behaviour, walking and moderate intensity physical activity",
+    keywords="wearables, accelerometer, health data science, human activity recognition",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/activityMonitoring/biobankAccelerometerAnalysis",
-    packages=setuptools.find_packages(),
+    download_url="https://github.com/activityMonitoring/biobankAccelerometerAnalysis",
+    author=get_string("__author__"),
+    maintainer=get_string("__maintainer__"),
+    maintainer_email=get_string("__maintainer_email__"),
+    license=get_string("__license__"),
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "Topic :: Scientific/Engineering",
+        "Topic :: Scientific/Engineering :: Bio-Informatics",
+        "Topic :: Scientific/Engineering :: Information Analysis",
+        "Topic :: Scientific/Engineering :: Medical Science Apps.",
+    ],
+    packages=setuptools.find_packages(where="src", exclude=("test", "tests")),
+    package_dir={"": "src"},
     include_package_data=True,
     install_requires=[
         'numpy',
         'scipy',
         'matplotlib',
         'pandas>=1.2.5',
         'tqdm>=4.59.0',
@@ -54,19 +74,14 @@
             "sphinx>=4.2",
             "sphinx_rtd_theme>=1.0",
             "readthedocs-sphinx-search>=0.1",
             "sphinxcontrib-programoutput>=0.17",
             "docutils<0.18",
         ],
     },
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "Operating System :: MacOS :: MacOS X",
-        "Operating System :: Unix",
-    ],
     entry_points={
         "console_scripts": [
             "accProcess=accelerometer.accProcess:main",
             "accPlot=accelerometer.accPlot:main",
             "accWriteCmds=accelerometer.accWriteCmds:main",
             "accCollateSummary=accelerometer.accCollateSummary:main"
         ]
```


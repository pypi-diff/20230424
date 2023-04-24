# Comparing `tmp/MCSimPython-0.0.14.tar.gz` & `tmp/MCSimPython-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MCSimPython-0.0.14.tar", last modified: Tue Mar  7 10:14:52 2023, max compression
+gzip compressed data, was "MCSimPython-0.1.1.tar", last modified: Mon Apr 24 08:55:48 2023, max compression
```

## Comparing `MCSimPython-0.0.14.tar` & `MCSimPython-0.1.1.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-03-07 10:14:52.284914 MCSimPython-0.0.14/
--rw-rw-rw-   0        0        0    35823 2023-01-30 10:28:59.000000 MCSimPython-0.0.14/LICENSE
--rw-rw-rw-   0        0        0      200 2023-01-24 10:20:15.000000 MCSimPython-0.0.14/MANIFEST.in
--rw-rw-rw-   0        0        0     3489 2023-03-07 10:14:52.277936 MCSimPython-0.0.14/PKG-INFO
--rw-rw-rw-   0        0        0     3032 2023-03-07 09:27:32.000000 MCSimPython-0.0.14/README.md
--rw-rw-rw-   0        0        0      799 2023-03-07 10:13:57.000000 MCSimPython-0.0.14/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-07 10:14:52.285912 MCSimPython-0.0.14/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-07 10:14:51.746817 MCSimPython-0.0.14/src/
-drwxrwxrwx   0        0        0        0 2023-03-07 10:14:51.753798 MCSimPython-0.0.14/src/MCSimPython/
--rw-rw-rw-   0        0        0        0 2023-01-24 10:20:15.000000 MCSimPython-0.0.14/src/MCSimPython/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-07 10:14:51.835097 MCSimPython-0.0.14/src/MCSimPython/control/
--rw-rw-rw-   0        0        0      456 2023-03-02 08:12:49.000000 MCSimPython-0.0.14/src/MCSimPython/control/__init__.py
--rw-rw-rw-   0        0        0     3160 2023-02-15 13:51:40.000000 MCSimPython-0.0.14/src/MCSimPython/control/backstepping.py
--rw-rw-rw-   0        0        0     2832 2023-02-15 13:51:40.000000 MCSimPython-0.0.14/src/MCSimPython/control/basic.py
-drwxrwxrwx   0        0        0        0 2023-03-07 10:14:51.869274 MCSimPython-0.0.14/src/MCSimPython/guidance/
--rw-rw-rw-   0        0        0     1057 2023-02-15 13:51:40.000000 MCSimPython-0.0.14/src/MCSimPython/guidance/__init__.py
--rw-rw-rw-   0        0        0     2544 2023-02-15 13:51:40.000000 MCSimPython-0.0.14/src/MCSimPython/guidance/filter.py
--rw-rw-rw-   0        0        0     5713 2023-02-15 13:51:40.000000 MCSimPython-0.0.14/src/MCSimPython/guidance/path_param.py
-drwxrwxrwx   0        0        0        0 2023-03-07 10:14:51.884652 MCSimPython-0.0.14/src/MCSimPython/observer/
--rw-rw-rw-   0        0        0      780 2023-02-15 13:51:40.000000 MCSimPython-0.0.14/src/MCSimPython/observer/__init__.py
--rw-rw-rw-   0        0        0    10813 2023-02-13 14:05:47.000000 MCSimPython-0.0.14/src/MCSimPython/observer/ekf.py
--rw-rw-rw-   0        0        0     2199 2023-02-15 13:51:40.000000 MCSimPython-0.0.14/src/MCSimPython/observer/nonlinobs.py
-drwxrwxrwx   0        0        0        0 2023-03-07 10:14:51.913926 MCSimPython-0.0.14/src/MCSimPython/simulator/
--rw-rw-rw-   0        0        0      753 2023-03-07 09:26:54.000000 MCSimPython-0.0.14/src/MCSimPython/simulator/__init__.py
--rw-rw-rw-   0        0        0    14045 2023-03-07 09:26:54.000000 MCSimPython-0.0.14/src/MCSimPython/simulator/csad.py
--rw-rw-rw-   0        0        0     6951 2023-03-07 09:26:54.000000 MCSimPython-0.0.14/src/MCSimPython/simulator/gunnerus.py
--rw-rw-rw-   0        0        0     4313 2023-02-23 09:31:32.000000 MCSimPython-0.0.14/src/MCSimPython/simulator/thruster_dynamics.py
--rw-rw-rw-   0        0        0     4825 2023-02-15 13:51:40.000000 MCSimPython-0.0.14/src/MCSimPython/simulator/vessel.py
-drwxrwxrwx   0        0        0        0 2023-03-07 10:14:51.932112 MCSimPython-0.0.14/src/MCSimPython/thrust_allocation/
--rw-rw-rw-   0        0        0        0 2023-02-23 09:31:32.000000 MCSimPython-0.0.14/src/MCSimPython/thrust_allocation/__init__.py
--rw-rw-rw-   0        0        0     4285 2023-02-23 09:31:32.000000 MCSimPython-0.0.14/src/MCSimPython/thrust_allocation/allocation.py
--rw-rw-rw-   0        0        0      572 2023-02-23 09:31:32.000000 MCSimPython-0.0.14/src/MCSimPython/thrust_allocation/constraints.py
--rw-rw-rw-   0        0        0      930 2023-02-23 09:31:32.000000 MCSimPython-0.0.14/src/MCSimPython/thrust_allocation/thruster.py
--rw-rw-rw-   0        0        0     8245 2023-02-27 15:04:54.000000 MCSimPython-0.0.14/src/MCSimPython/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-07 10:14:51.936102 MCSimPython-0.0.14/src/MCSimPython/vessel_data/
-drwxrwxrwx   0        0        0        0 2023-03-07 10:14:52.025303 MCSimPython-0.0.14/src/MCSimPython/vessel_data/CSAD/
--rw-rw-rw-   0        0        0        0 2023-01-24 10:20:15.000000 MCSimPython-0.0.14/src/MCSimPython/vessel_data/CSAD/__init__.py
--rw-rw-rw-   0        0        0      504 2023-01-24 10:20:15.000000 MCSimPython-0.0.14/src/MCSimPython/vessel_data/CSAD/freqs.npy
--rw-rw-rw-   0        0        0      416 2023-01-24 10:20:15.000000 MCSimPython-0.0.14/src/MCSimPython/vessel_data/CSAD/headings.npy
--rw-rw-rw-   0        0        0      475 2023-02-23 09:31:32.000000 MCSimPython-0.0.14/src/MCSimPython/vessel_data/CSAD/thruster_data.py
--rw-rw-rw-   0        0        0     4022 2023-01-24 10:20:15.000000 MCSimPython-0.0.14/src/MCSimPython/vessel_data/CSAD/vesselABC_json.json
--rw-rw-rw-   0        0        0  1961336 2023-01-24 10:20:15.000000 MCSimPython-0.0.14/src/MCSimPython/vessel_data/CSAD/vessel_json.json
--rw-rw-rw-   0        0        0        0 2023-01-24 10:20:15.000000 MCSimPython-0.0.14/src/MCSimPython/vessel_data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-07 10:14:52.200353 MCSimPython-0.0.14/src/MCSimPython/vessel_data/gunnerus/
--rw-rw-rw-   0        0        0        0 2023-01-24 10:20:15.000000 MCSimPython-0.0.14/src/MCSimPython/vessel_data/gunnerus/__init__.py
--rw-rw-rw-   0        0        0  2939897 2023-01-24 10:20:15.000000 MCSimPython-0.0.14/src/MCSimPython/vessel_data/gunnerus/gunnerus_veres.json
--rw-rw-rw-   0        0        0      861 2023-01-24 10:20:15.000000 MCSimPython-0.0.14/src/MCSimPython/vessel_data/gunnerus/parV_RVG3DOF.pkl
--rw-rw-rw-   0        0        0     2870 2023-01-24 10:20:15.000000 MCSimPython-0.0.14/src/MCSimPython/vessel_data/gunnerus/parV_RVG6DOF.pkl
--rw-rw-rw-   0        0        0  4723068 2023-02-13 14:05:47.000000 MCSimPython-0.0.14/src/MCSimPython/vessel_data/gunnerus/vessel.json
--rw-rw-rw-   0        0        0  4733857 2023-02-20 14:57:25.000000 MCSimPython-0.0.14/src/MCSimPython/vessel_data/gunnerus/vessel_2.json
-drwxrwxrwx   0        0        0        0 2023-03-07 10:14:52.257687 MCSimPython-0.0.14/src/MCSimPython/waves/
--rw-rw-rw-   0        0        0      425 2023-02-15 13:51:40.000000 MCSimPython-0.0.14/src/MCSimPython/waves/__init__.py
--rw-rw-rw-   0        0        0    17355 2023-03-06 13:23:02.000000 MCSimPython-0.0.14/src/MCSimPython/waves/wave_loads.py
--rw-rw-rw-   0        0        0    12414 2023-02-15 13:51:40.000000 MCSimPython-0.0.14/src/MCSimPython/waves/wave_spectra.py
--rw-rw-rw-   0        0        0     2504 2023-01-24 10:20:15.000000 MCSimPython-0.0.14/src/MCSimPython/waves/wave_spreading.py
-drwxrwxrwx   0        0        0        0 2023-03-07 10:14:51.803186 MCSimPython-0.0.14/src/MCSimPython.egg-info/
--rw-rw-rw-   0        0        0     3489 2023-03-07 10:14:51.000000 MCSimPython-0.0.14/src/MCSimPython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1852 2023-03-07 10:14:51.000000 MCSimPython-0.0.14/src/MCSimPython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-07 10:14:51.000000 MCSimPython-0.0.14/src/MCSimPython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-03-07 10:14:51.000000 MCSimPython-0.0.14/src/MCSimPython.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-03-07 10:14:51.000000 MCSimPython-0.0.14/src/MCSimPython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-01-24 10:20:15.000000 MCSimPython-0.0.14/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-07 10:14:52.271651 MCSimPython-0.0.14/tests/
--rw-rw-rw-   0        0        0     4377 2023-02-27 15:04:54.000000 MCSimPython-0.0.14/tests/test_utils.py
--rw-rw-rw-   0        0        0     2654 2023-02-05 15:08:16.000000 MCSimPython-0.0.14/tests/test_wave_spectra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:55:48.014908 MCSimPython-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-04-24 08:55:32.000000 MCSimPython-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-24 08:55:32.000000 MCSimPython-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-24 08:55:48.014908 MCSimPython-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-24 08:55:32.000000 MCSimPython-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 08:55:48.014908 MCSimPython-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:55:47.990908 MCSimPython-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:55:47.990908 MCSimPython-0.1.1/src/MCSimPython/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-24 08:55:40.000000 MCSimPython-0.1.1/src/MCSimPython/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:55:47.994907 MCSimPython-0.1.1/src/MCSimPython/control/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/control/adaptiveFS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/control/backstepping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/control/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:55:47.994907 MCSimPython-0.1.1/src/MCSimPython/guidance/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/guidance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/guidance/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/guidance/path_param.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:55:47.994907 MCSimPython-0.1.1/src/MCSimPython/observer/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/observer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/observer/ekf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/observer/ltv_kf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/observer/nonlinobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:55:47.994907 MCSimPython-0.1.1/src/MCSimPython/simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15957 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/simulator/csad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/simulator/gunnerus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/simulator/thruster_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/simulator/vessel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:55:47.994907 MCSimPython-0.1.1/src/MCSimPython/thrust_allocation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/thrust_allocation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/thrust_allocation/allocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/thrust_allocation/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/thrust_allocation/thruster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:55:47.994907 MCSimPython-0.1.1/src/MCSimPython/vessel_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:55:47.994907 MCSimPython-0.1.1/src/MCSimPython/vessel_data/CSAD/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/vessel_data/CSAD/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/vessel_data/CSAD/freqs.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/vessel_data/CSAD/headings.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/vessel_data/CSAD/thruster_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/vessel_data/CSAD/vesselABC_json.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1961336 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/vessel_data/CSAD/vessel_json.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/vessel_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:55:48.006908 MCSimPython-0.1.1/src/MCSimPython/vessel_data/gunnerus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/vessel_data/gunnerus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2939897 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/vessel_data/gunnerus/gunnerus_veres.json
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/vessel_data/gunnerus/parV_RVG3DOF.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/vessel_data/gunnerus/parV_RVG6DOF.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)  4723068 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/vessel_data/gunnerus/vessel.json
+-rw-r--r--   0 runner    (1001) docker     (123)  4733857 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/vessel_data/gunnerus/vessel_2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:55:48.014908 MCSimPython-0.1.1/src/MCSimPython/waves/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/waves/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19467 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/waves/wave_loads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/waves/wave_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/src/MCSimPython/waves/wave_spreading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:55:47.990908 MCSimPython-0.1.1/src/MCSimPython.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-24 08:55:47.000000 MCSimPython-0.1.1/src/MCSimPython.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-04-24 08:55:47.000000 MCSimPython-0.1.1/src/MCSimPython.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 08:55:47.000000 MCSimPython-0.1.1/src/MCSimPython.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-24 08:55:47.000000 MCSimPython-0.1.1/src/MCSimPython.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 08:55:47.000000 MCSimPython-0.1.1/src/MCSimPython.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:55:48.014908 MCSimPython-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-04-24 08:55:33.000000 MCSimPython-0.1.1/tests/test_wave_spectra.py
```

### Comparing `MCSimPython-0.0.14/LICENSE` & `MCSimPython-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.0.14/README.md` & `MCSimPython-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,64 +1,59 @@
-# MCSimPython
-
-[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)    
-
-Vessel simulator used in master project and master thesis of M. Kongshaug, H. Mo and J. Hygen. The project is developed at Norwegian University of Science and Technology, Institue of Marine Technology. 
-
-The python package is not complete and there is no guarantee for the validity of the vessel models.
-
-The complete documentation can be found at: https://wave-model.readthedocs.io/en/latest/index.html
-
-## How to use MCSimPython
-
-### PyPi
-The `MCSimPython` package can be installed from PyPi using `pip`:
-
-`pip install MCSimPython`
-
-### From GitHub:
-Install from GitHub in the following way when developing the package.
-- Clone the GitHub repository to your local computer.
-- Create a virtual environment `py -m venv name-of-venv`
-- Activate virtual environment `name-of-venv\scripts\activate`
-- Update pip and setuptools: `py -m pip install --upgrade pip setuptools`
-- Install the python package locally as an editable: `pip install -e .`
-- Verify that the python package `MCSimPython` has been installed properly by running a demo script, or simply
-```
-(venv) C:\path\to\dir> python
->>> import MCSimPython
->>>
-```
-
-## Structure
-All code implementation is found in the `src` directory. The python package is structured as follows:
-
-- `src/MCSimPython/simulator/` Simulation Models. *Python Path*:= `MCSimPython.simulator`
-    - `csad.py`: Simulation models for C/S Arctic Drillship
-    - `gunnerus.py`: Simulation models for R/V Gunnerus
-- `src/MCSimPython/waves/` Wave kinematics, wave spectra, and wave loads. *Python Path* := `MCSimPython.waves`
-- `src/MCSimPython/guidance/` Reference Models. *Python path*:= `MCSimPython.guidance` *(in development)*
-    - `filter.py`: A third order reference filter.
-    - `path_param`: Waypoint path parameterization.
-- `src/MCSimPython/observers/` Observers : `MCSimPython.observer` *(in development)*
-    - `nonlinobs.py`: Nonlinear observers *(only 3DOF nonlinobs w/ wavefiltering atm)*
-- `src/MCSimPython/control` Controllers : `MCSimPython.control` *(in development)*
-    - `basic.py`: Simple PD and PID controllers
-    - `backstepping.py`: A simple backstepping controller (no bias compensation).
-
-
-## Demos
-
-Demonstration of how the individual components of the python package can be used is given in `demos`. Some demos of combination of the different components are also given here. 
-
-## Visualization
-
-### RVG 6DOF model in beam sea
-![6DOF RVG 2D Visualization](https://github.com/janerikhy/Wave-Model/blob/main/demos/animations/wave_motion1d.gif)
-
-### RVG 6DOF model in multidirectional sea
-![6DOF RVG 3D Visualization](https://github.com/janerikhy/Wave-Model/blob/main/demos/animations/vessel_motion3d__rvg2.gif)
-
-
-### CSAD 6DOF model in multidirectional sea
-![6DOF CSAD 2D Visualisation](https://github.com/janerikhy/Wave-Model/blob/main/demos/animations/vessel_motion3d_22.gif)
-
+Metadata-Version: 2.1
+Name: MCSimPython
+Version: 0.1.1
+Summary: Python vessel simulation environment
+Author-email: Jan-Erik Hygen <janereh@stud.ntnu.no>
+Keywords: mcsim,MCSimPython,DP,dynamic positioning,Marine Cybernetics
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# MCSimPython
+
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![Python: v3.8](https://shields.io/badge/python-v3.8-green.svg)](https://www.python.org/downloads/release/python-380/) [![Python: v3.9](https://shields.io/badge/python-v3.9-green.svg)](https://www.python.org/downloads/release/python-390)
+
+Vessel simulator used in master project and master thesis of M. Kongshaug, H. Mo and J. Hygen. The project is developed at Norwegian University of Science and Technology, Institue of Marine Technology. 
+
+The python package is not complete and there is no guarantee for the validity of the vessel models.
+
+The complete documentation can be found at: https://wave-model.readthedocs.io/en/latest/index.html
+
+## How to use MCSimPython
+
+### PyPi
+The `MCSimPython` package can be installed from PyPi using `pip`:
+
+`pip install MCSimPython`
+
+### From GitHub:
+Install from GitHub in the following:
+- Clone the GitHub repository to your local computer.
+- Create a virtual environment `py -m venv name-of-venv`
+- Activate virtual environment `name-of-venv\scripts\activate`
+- Update pip and setuptools: `py -m pip install --upgrade pip setuptools`
+- Install the python package locally: `pip install .` (alternatively you can install as an editable `pip install -e .`)
+- Verify that the python package `MCSimPython` has been installed properly by running a demo script, or simply in the command promt:
+```
+(venv) C:\path\to\dir> python
+>>> import MCSimPython
+>>>
+```
+
+## Demos
+
+Demonstration of how the individual components of the python package can be used is given in `demos`. Some demos of combination of the different components are also given here. 
+
+## Visualization
+
+### RVG 6DOF model in beam sea
+![6DOF RVG 2D Visualization](https://github.com/janerikhy/Wave-Model/blob/main/demos/animations/wave_motion1d.gif)
+
+### RVG 6DOF model in multidirectional sea
+![6DOF RVG 3D Visualization](https://github.com/janerikhy/Wave-Model/blob/main/demos/animations/vessel_motion3d__rvg2.gif)
+
+
+### CSAD 6DOF model in multidirectional sea
+![6DOF CSAD 2D Visualisation](https://github.com/janerikhy/Wave-Model/blob/main/demos/animations/vessel_motion3d_22.gif)
+
```

### Comparing `MCSimPython-0.0.14/src/MCSimPython/control/backstepping.py` & `MCSimPython-0.1.1/src/MCSimPython/control/backstepping.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-# backstepping.py
-
-# ----------------------------------------------------------------------------
-# This code is part of the MCSimPython toolbox and repository.
-# Created By: Jan-Erik Hygen
-# Created Date: 2023-02-01
-# Revised: 
-# Tested:
-# 
-# Copyright (C) 2023: NTNU, Trondheim
-# Licensed under GPL-3.0-or-later
-# ---------------------------------------------------------------------------
-
-import numpy as np
-from MCSimPython.utils import Rz, pipi
-
-def Smat(r):
-    return np.array([
-        [0., -r, 0.],
-        [r, 0., 0.],
-        [0., 0., 0.]
-    ])
-
-
-
-class BacksteppingController:
-    """Backsteppipng controller for maneuvering.
-    
-    The controller should be used together with 
-    a path parameterization guidance/reference model.
-
-    See Also
-    --------
-    MCSimPython.guidance.path_parm.WayPointPathParam :
-        Way-points path parameterization.
-    """
-
-    def __init__(self, M, D, K1, K2):
-        self.M = M
-        self.D = D
-        self.K1 = K1
-        self.K2 = K2
-
-    def lyapunov_grad_s(self, z1, eta, eta_d_s):
-        """Lyapunov function gradient."""
-        return -z1@Rz(eta[2]).T@eta_d_s
-
-    def error_pos(self, eta, eta_d):
-        """Deviation from desired pose in body-frame."""
-        return Rz(eta[2]).T@(eta - eta_d)
-
-    def error_vel(self, nu, alpha):
-        """Deviation from virtual control law."""
-        return nu - alpha
-
-    def virtual_control_law(self, z1, eta, eta_d_s, u_s):
-        """Virtual control law (alpha)."""
-        return -self.K1@z1 + Rz(eta[2]).T@eta_d_s*u_s
-
-    def virtual_control_dot(self, z1, z2, alpha, eta, eta_d, eta_d_s, eta_d_s2, u_s, u_s_dot, nu, s_dot, ddt_u_s):
-        """Time derivative of virtual control law (alpha_dot)."""
-        line1 = self.K1@Smat(nu[2])@z1 - self.K1@nu - \
-            Smat(nu[2])@Rz(eta[2]).T@eta_d_s*u_s
-        line2 = Rz(eta[2]).T@eta_d_s*ddt_u_s
-        line3 = (self.K1@Rz(eta[2]).T@eta_d_s + Rz(eta[2]).T @
-                 eta_d_s2*u_s + Rz(eta[2]).T@eta_d_s*u_s_dot)*s_dot
-        return line1 + line2 + line3
-
-    def control_law(self, z1, z2, alpha, alpha_dot, nu):
-        """Complete control law."""
-        return self.D@alpha + self.M@alpha_dot - z1 - self.K2@z2
-
-    def unit_gradient_update_law(self, u_s, mu, eta_d_s, lyapunov_gradient):
-        """Unit-tangent gradient update law for path parameter (s)."""
-        return u_s - mu/np.linalg.norm(eta_d_s)*lyapunov_gradient
-
-    def u(self, eta, nu, eta_d, eta_d_s, eta_d_s2, mu, u_s, u_s_dot, ddt_u_s):
-        """Control command."""
-        z1 = self.error_pos(eta, eta_d)
-        z1[2] = np.mod(z1[2] + np.pi, 2*np.pi) - np.pi
-        a = self.virtual_control_law(z1, eta, eta_d_s, u_s)
-        z2 = self.error_vel(nu, a)
-        v_d_s = self.lyapunov_grad_s(z1, eta, eta_d_s)
-        s_dot = self.unit_gradient_update_law(u_s, mu, eta_d_s, v_d_s)
-        #s_dot = u_s
-        self._s_dot = s_dot
-        a_dot = self.virtual_control_dot(
-            z1, z2, a, eta, eta_d, eta_d_s, eta_d_s2, u_s, u_s_dot, nu, s_dot, ddt_u_s)
-
+# backstepping.py
+
+# ----------------------------------------------------------------------------
+# This code is part of the MCSimPython toolbox and repository.
+# Created By: Jan-Erik Hygen
+# Created Date: 2023-02-01
+# Revised: 
+# Tested:
+# 
+# Copyright (C) 2023: NTNU, Trondheim
+# Licensed under GPL-3.0-or-later
+# ---------------------------------------------------------------------------
+
+import numpy as np
+from MCSimPython.utils import Rz, pipi
+
+def Smat(r):
+    return np.array([
+        [0., -r, 0.],
+        [r, 0., 0.],
+        [0., 0., 0.]
+    ])
+
+
+
+class BacksteppingController:
+    """Backsteppipng controller for maneuvering.
+    
+    The controller should be used together with 
+    a path parameterization guidance/reference model.
+
+    See Also
+    --------
+    MCSimPython.guidance.path_parm.WayPointPathParam :
+        Way-points path parameterization.
+    """
+
+    def __init__(self, M, D, K1, K2):
+        self.M = M
+        self.D = D
+        self.K1 = K1
+        self.K2 = K2
+
+    def lyapunov_grad_s(self, z1, eta, eta_d_s):
+        """Lyapunov function gradient."""
+        return -z1@Rz(eta[2]).T@eta_d_s
+
+    def error_pos(self, eta, eta_d):
+        """Deviation from desired pose in body-frame."""
+        return Rz(eta[2]).T@(eta - eta_d)
+
+    def error_vel(self, nu, alpha):
+        """Deviation from virtual control law."""
+        return nu - alpha
+
+    def virtual_control_law(self, z1, eta, eta_d_s, u_s):
+        """Virtual control law (alpha)."""
+        return -self.K1@z1 + Rz(eta[2]).T@eta_d_s*u_s
+
+    def virtual_control_dot(self, z1, z2, alpha, eta, eta_d, eta_d_s, eta_d_s2, u_s, u_s_dot, nu, s_dot, ddt_u_s):
+        """Time derivative of virtual control law (alpha_dot)."""
+        line1 = self.K1@Smat(nu[2])@z1 - self.K1@nu - \
+            Smat(nu[2])@Rz(eta[2]).T@eta_d_s*u_s
+        line2 = Rz(eta[2]).T@eta_d_s*ddt_u_s
+        line3 = (self.K1@Rz(eta[2]).T@eta_d_s + Rz(eta[2]).T @
+                 eta_d_s2*u_s + Rz(eta[2]).T@eta_d_s*u_s_dot)*s_dot
+        return line1 + line2 + line3
+
+    def control_law(self, z1, z2, alpha, alpha_dot, nu):
+        """Complete control law."""
+        return self.D@alpha + self.M@alpha_dot - z1 - self.K2@z2
+
+    def unit_gradient_update_law(self, u_s, mu, eta_d_s, lyapunov_gradient):
+        """Unit-tangent gradient update law for path parameter (s)."""
+        return u_s - mu/np.linalg.norm(eta_d_s)*lyapunov_gradient
+
+    def u(self, eta, nu, eta_d, eta_d_s, eta_d_s2, mu, u_s, u_s_dot, ddt_u_s):
+        """Control command."""
+        z1 = self.error_pos(eta, eta_d)
+        z1[2] = np.mod(z1[2] + np.pi, 2*np.pi) - np.pi
+        a = self.virtual_control_law(z1, eta, eta_d_s, u_s)
+        z2 = self.error_vel(nu, a)
+        v_d_s = self.lyapunov_grad_s(z1, eta, eta_d_s)
+        s_dot = self.unit_gradient_update_law(u_s, mu, eta_d_s, v_d_s)
+        #s_dot = u_s
+        self._s_dot = s_dot
+        a_dot = self.virtual_control_dot(
+            z1, z2, a, eta, eta_d, eta_d_s, eta_d_s2, u_s, u_s_dot, nu, s_dot, ddt_u_s)
+
         return self.control_law(z1, z2, a, a_dot, nu)
```

### Comparing `MCSimPython-0.0.14/src/MCSimPython/control/basic.py` & `MCSimPython-0.1.1/src/MCSimPython/guidance/filter.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,91 +1,84 @@
-# basic.py
-
-# ----------------------------------------------------------------------------
-# This code is part of the MCSimPython toolbox and repository.
-# Created By: Jan-Erik Hygen
-# Created Date: 2023-01-30
-# Revised: 
-# Tested:
-# 
-# Copyright (C) 2023: NTNU, Trondheim
-# Licensed under GPL-3.0-or-later
-# ---------------------------------------------------------------------------
-
-import numpy as np
-from MCSimPython.utils import Rz
-
-
-class PD:
-    """Proportional-Derivative controller."""
-    def __init__(self, kp: list, kd: list):
-        self.Kp = np.diag(kp)
-        self.Kd = np.diag(kd)
-        self.tau_cmd = np.zeros(3)
-
-    def get_tau(self, eta, eta_d, nu, nu_d):
-        """Calculate control loads.
-        
-        Parameters
-        ----------
-        eta : array_like
-            Vessel pose in surge, sway and yaw.
-        eta_d : array_like
-            Desired vessel pose in surge, sway and yaw (NED-frame).
-        nu : array_like
-            Vessel velocity in surge, sway, and yaw (body-frame).
-        nu_d : array_like
-            Desired vessel velocity in surge, sway and yaw (body-frame).
-        
-        Returns
-        -------
-        tau : array_like
-            Controller load in surge, sway, and yaw (body-frame).
-        """
-        psi = eta[-1]
-        z1 = Rz(psi).T@(eta-eta_d)
-        z2 = nu - nu_d
-        return -self.Kp@z1 - self.Kd@z2
-    
-    def set_kd(self, kd: list):
-        """Set the derivative gain coefficients."""
-        self.Kd = np.diag(kd)
-    
-    def set_kp(self, kp: list):
-        """Set the proportional gain coefficients."""
-        self.Kp = np.diag(kp)
-
-class PID:
-    """Proportional-Derivative control with integral action."""
-    
-    def __init__(self, kp: list, kd: list, ki: list, dt: float = 0.01):
-        self.Kp = np.diag(kp)
-        self.Kd = np.diag(kd)
-        self.Ki = np.diag(ki)
-        self.zi = np.zeros(3)
-        self.dt = dt
-
-    def get_tau(self, eta, eta_d, nu, nu_d):
-        """Calculate control loads.
-        
-        Parameters
-        ----------
-        eta : array_like
-            Vessel pose in surge, sway and yaw.
-        eta_d : array_like
-            Desired vessel pose in surge, sway and yaw (NED-frame).
-        nu : array_like
-            Vessel velocity in surge, sway, and yaw (body-frame).
-        nu_d : array_like
-            Desired vessel velocity in surge, sway and yaw (body-frame).
-        
-        Returns
-        -------
-        tau : array_like
-            Controller load in surge, sway, and yaw (body-frame).
-        """
-        psi = eta[-1]
-        z1 = Rz(psi).T@(eta - eta_d)
-        z2 = nu - nu_d
-
-        self.zi += self.dt*(eta - eta_d)
-        return -self.Kp@z1 - self.Kd@z2 - Rz(psi).T@self.Ki@self.zi
+# filter.py
+
+# ----------------------------------------------------------------------------
+# This code is part of the MCSimPython toolbox and repository.
+# Created By: Jan-Erik Hygen
+# Created Date: 2023-01-30
+# Revised: 
+# Tested:
+# Copyright (C) 2023: NTNU, Trondheim
+# Licensed under GPL-3.0-or-later
+# ---------------------------------------------------------------------------
+
+import numpy as np
+from MCSimPython.utils import Rz
+
+class ThrdOrderRefFilter():
+    """Third-order reference filter for guidance. 
+    
+    Attributes
+    ----------
+    eta_d : array_like
+        3D-array of desired vessel pose in NED-frame
+    eta_d_dot : array_like
+        3D-array of desired vessel velocity in NED-frame
+    eta_d_ddot : array_like
+        3D-array of desired vessel acceleration in NED-frame
+    """
+
+    def __init__(self, dt, omega=[0.3, 0.3, 0.3]):
+        self._dt = dt
+        self.eta_d = np.zeros(3)
+        self.eta_d_dot = np.zeros(3)
+        self.eta_d_ddot = np.zeros(3)
+        self._eta_r = np.zeros(3)
+        self._x = np.zeros(9)
+        self._delta = np.eye(3)
+        self._w = np.diag(omega)
+        O3x3 = np.zeros((3, 3))
+        self.Ad = np.block([
+            [O3x3, np.eye(3), O3x3],
+            [O3x3, O3x3, np.eye(3)],
+            [-self._w**3, -(2*self._delta + np.eye(3))@self._w**2, - (2*self._delta + np.eye(3))@self._w]
+        ])
+        self.Bd = np.block([
+            [O3x3],
+            [O3x3],
+            [self._w**3]
+        ])
+
+
+    def get_eta_d(self):
+        """Get desired pose in NED-frame."""
+        return self.eta_d
+    
+    def get_eta_d_dot(self):
+        """Get desired velocity in NED-frame."""
+        return self.eta_d_dot
+    
+    def get_eta_d_ddot(self):
+        """Get desired acceleration in NED-frame."""
+        return self.eta_d_ddot
+
+    def get_nu_d(self):
+        """Get desired velocity in body-frame."""
+        psi = self.eta_d[-1]
+        return Rz(psi).T@self.eta_d_dot
+
+    def set_eta_r(self, eta_r):
+        """Set the reference pose.
+        
+        Parameters
+        ----------
+        eta_r : array_like
+            Reference vessel pose in surge, sway and yaw.
+        """
+        self._eta_r = eta_r
+
+    def update(self):
+        """Update the desired position."""
+        x_dot = self.Ad@self._x + self.Bd@self._eta_r
+        self._x = self._x + self._dt*x_dot
+        self.eta_d = self._x[:3]
+        self.eta_d_dot = self._x[3:6]
+        self.eta_d_ddot = self._x[6:]
```

### Comparing `MCSimPython-0.0.14/src/MCSimPython/guidance/path_param.py` & `MCSimPython-0.1.1/src/MCSimPython/guidance/path_param.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,175 +1,175 @@
-# path_param.py
-
-# ----------------------------------------------------------------------------
-# This code is part of the MCSimPython toolbox and repository.
-# Created By: Jan-Erik Hygen
-# Created Date: 2023-01-30
-# Revised: 
-# Tested:
-#
-# Copyright (C) 2023: NTNU, Trondheim
-# Licensed under GPL-3.0-or-later
-# ---------------------------------------------------------------------------
-
-import numpy as np
-from MCSimPython.utils import Rz, pipi2cont
-
-
-class WayPointsRefModel:
-    """Way-point path parametrization model. 
-    
-    Attributes
-    ----------
-    pd : array_like
-        Array of desired vessel positions (2D).
-    pd_s : array_like
-        Array of the parital derivative of pd w.r.t path parameter s.
-    pd_s2 : array_like
-        Array of the two times partial derivative of pd w.r.t s
-    pd_s3 : array_like
-        The three time partial derivative of pd w.r.t s.
-    
-    """
-
-    r = 3
-    A = np.array([
-        [1, 0, 0, 0, 0, 0, 0, 0],
-        [0, 1, 0, 0, 0, 0, 0, 0],
-        [0, 0, 1, 0, 0, 0, 0, 0],
-        [0, 0, 0, 1, 0, 0, 0, 0],
-        [1, 1, 1, 1, 1, 1, 1, 1],
-        [0, 1, 2, 3, 4, 5, 6, 7],
-        [0, 0, 2, 6, 12, 20, 30, 42],
-        [0, 0, 0, 6, 24, 60, 120, 210]
-    ])
-    Ainv = np.linalg.pinv(A)
-    THETA = np.arange(0, 1, 0.01)
-
-    def __init__(self, way_points, slope, ds):
-        self.n = len(way_points)    # Number of way-points
-        self.I = self.n-1           # Number of line-segments
-        self.k = 2*self.r + 1       # Number of coefficients we must solve for
-        self.slope = slope
-        self.wps = way_points
-
-        pd = np.zeros((self.I, int(1/ds), 2))
-        pd_s = np.zeros_like(pd)
-        pd_s2 = np.zeros_like(pd)
-        pd_s3 = np.zeros_like(pd)
-
-        # Set initial values
-        pd[:, 0] = way_points[0:-1]
-        pd[:, -1] = way_points[1:]
-
-        pd_s[0, 0] = way_points[1] - way_points[0]
-        pd_s[-1, -1] = way_points[self.I] - way_points[self.I-1]
-
-        pd_s[1:self.I, 0] = slope * \
-            (way_points[2:] - way_points[0:self.I-1])
-        pd_s[0:self.I-1, -1] = slope * \
-            (way_points[2:] - way_points[0:self.I-1])
-
-        pd_s2[0:self.I, 0] = 0
-        pd_s3[0:self.I, 0] = 0
-        pd_s2[0:self.I, 1] = 0
-        pd_s3[0:self.I, 1] = 0
-
-        # Calculate the coefficients
-        self.bn = np.zeros((self.I, self.k+1, 2))
-        for j in range(self.I):
-            self.bn[j, :] = np.array([
-                pd[j, 0],
-                pd_s[j, 0],
-                pd_s2[j, 0],
-                pd_s3[j, 0],
-                pd[j, -1],
-                pd_s[j, -1],
-                pd_s2[j, -1],
-                pd_s3[j, -1]
-            ])
-        self.xn = np.zeros_like(self.bn)
-        for j in range(self.I):
-            self.xn[j, :] = WayPointsRefModel.Ainv@self.bn[j]
-
-    def T(self, theta):
-        return np.array([1, theta, theta**2, theta**3, theta **
-                         4, theta**5, theta**6, theta**7])
-
-    def T2(self, theta):
-        return np.array([0, 1, 2*theta, 3*theta**2, 4*theta **
-                         3, 5*theta**4, 6*theta**5, 7*theta**6])
-
-    def T3(self, theta):
-        return np.array([0, 0, 2, 6*theta, 12*theta**2, 20*theta**3, 30*theta**4, 42*theta**5])
-
-    def T4(self, theta):
-        return np.array([0, 0, 0, 6, 24*theta, 60*theta**2, 120*theta**3, 210*theta**4])
-
-    def pd(self, theta):
-        s = theta - np.floor(theta)
-        i = int(np.floor(theta))
-        if i >= self.I:
-            i = 0
-            s = 0
-        point = self.T(s)@self.xn[i]
-        return np.array([point[0], point[1]]).T
-
-    def pd_s(self, theta):
-        s = theta - np.floor(theta)
-        i = int(np.floor(theta))
-        if i >= self.I:
-            i = 0
-            s = 0
-        point = self.T2(s)@self.xn[i]
-        return np.array([point[0], point[1]]).T
-
-    def pd_s2(self, theta):
-        s = theta - np.floor(theta)
-        i = int(np.floor(theta))
-        if i >= self.I:
-            i = 0
-            s = 0
-        point = self.T3(s)@self.xn[i]
-        return np.array([point[0], point[1]]).T
-
-    def pd_s3(self, theta):
-        s = theta - np.floor(theta)
-        i = int(np.floor(theta))
-        if i >= self.I:
-            i = 0
-            s = 0
-        point = self.T4(s)@self.xn[i]
-        return np.array([point[0], point[1]]).T
-
-    def eta_d(self, theta, psi_prev):
-        pd = self.pd(theta)
-        pd_s = self.pd_s(theta)
-        psi_d = np.arctan2(pd_s[1], pd_s[0])
-        return np.array([pd[0], pd[1], pipi2cont(psi_d, psi_prev)])
-
-    def eta_d_s(self, theta):
-        pd_s = self.pd_s(theta)
-        pd_s2 = self.pd_s2(theta)
-        psi_d_s = (pd_s2[1]*pd_s[0] - pd_s[1]*pd_s2[0]) / \
-            (pd_s[0]**2 + pd_s[1]**2)
-        return np.array([pd_s[0], pd_s[1], psi_d_s])
-
-    def eta_d_s2(self, theta):
-        pd_s = self.pd_s(theta)
-        pd_s2 = self.pd_s2(theta)
-        pd_s3 = self.pd_s3(theta)
-        psi_d_s2 = ((pd_s3[1]*pd_s[0] - pd_s[1]*pd_s3[0])*(pd_s[0]**2 + pd_s[1]**2) -
-                    2*(pd_s2[1]*pd_s[0] - pd_s[1]*pd_s2[0])*(pd_s[0]*pd_s2[0] + pd_s[1]*pd_s2[1])) / (pd_s[0]**2 + pd_s[1]**2)**2
-        return np.array([pd_s2[0], pd_s2[1], psi_d_s2])
-
-    def full_path(self, theta):
-        path = np.zeros((len(theta), 3))
-        for i in range(len(theta)):
-            path[i] = self.eta_d(theta[i], path[i-1, -1])
-        return path
-
-    def path_speed(self, theta):
-        speed = np.zeros((len(theta), 2))
-        for i in range(len(theta)):
-            speed[i] = self.pd_s(theta[i])
+# path_param.py
+
+# ----------------------------------------------------------------------------
+# This code is part of the MCSimPython toolbox and repository.
+# Created By: Jan-Erik Hygen
+# Created Date: 2023-01-30
+# Revised: 
+# Tested:
+#
+# Copyright (C) 2023: NTNU, Trondheim
+# Licensed under GPL-3.0-or-later
+# ---------------------------------------------------------------------------
+
+import numpy as np
+from MCSimPython.utils import Rz, pipi2cont
+
+
+class WayPointsRefModel:
+    """Way-point path parametrization model. 
+    
+    Attributes
+    ----------
+    pd : array_like
+        Array of desired vessel positions (2D).
+    pd_s : array_like
+        Array of the parital derivative of pd w.r.t path parameter s.
+    pd_s2 : array_like
+        Array of the two times partial derivative of pd w.r.t s
+    pd_s3 : array_like
+        The three time partial derivative of pd w.r.t s.
+    
+    """
+
+    r = 3
+    A = np.array([
+        [1, 0, 0, 0, 0, 0, 0, 0],
+        [0, 1, 0, 0, 0, 0, 0, 0],
+        [0, 0, 1, 0, 0, 0, 0, 0],
+        [0, 0, 0, 1, 0, 0, 0, 0],
+        [1, 1, 1, 1, 1, 1, 1, 1],
+        [0, 1, 2, 3, 4, 5, 6, 7],
+        [0, 0, 2, 6, 12, 20, 30, 42],
+        [0, 0, 0, 6, 24, 60, 120, 210]
+    ])
+    Ainv = np.linalg.pinv(A)
+    THETA = np.arange(0, 1, 0.01)
+
+    def __init__(self, way_points, slope, ds):
+        self.n = len(way_points)    # Number of way-points
+        self.I = self.n-1           # Number of line-segments
+        self.k = 2*self.r + 1       # Number of coefficients we must solve for
+        self.slope = slope
+        self.wps = way_points
+
+        pd = np.zeros((self.I, int(1/ds), 2))
+        pd_s = np.zeros_like(pd)
+        pd_s2 = np.zeros_like(pd)
+        pd_s3 = np.zeros_like(pd)
+
+        # Set initial values
+        pd[:, 0] = way_points[0:-1]
+        pd[:, -1] = way_points[1:]
+
+        pd_s[0, 0] = way_points[1] - way_points[0]
+        pd_s[-1, -1] = way_points[self.I] - way_points[self.I-1]
+
+        pd_s[1:self.I, 0] = slope * \
+            (way_points[2:] - way_points[0:self.I-1])
+        pd_s[0:self.I-1, -1] = slope * \
+            (way_points[2:] - way_points[0:self.I-1])
+
+        pd_s2[0:self.I, 0] = 0
+        pd_s3[0:self.I, 0] = 0
+        pd_s2[0:self.I, 1] = 0
+        pd_s3[0:self.I, 1] = 0
+
+        # Calculate the coefficients
+        self.bn = np.zeros((self.I, self.k+1, 2))
+        for j in range(self.I):
+            self.bn[j, :] = np.array([
+                pd[j, 0],
+                pd_s[j, 0],
+                pd_s2[j, 0],
+                pd_s3[j, 0],
+                pd[j, -1],
+                pd_s[j, -1],
+                pd_s2[j, -1],
+                pd_s3[j, -1]
+            ])
+        self.xn = np.zeros_like(self.bn)
+        for j in range(self.I):
+            self.xn[j, :] = WayPointsRefModel.Ainv@self.bn[j]
+
+    def T(self, theta):
+        return np.array([1, theta, theta**2, theta**3, theta **
+                         4, theta**5, theta**6, theta**7])
+
+    def T2(self, theta):
+        return np.array([0, 1, 2*theta, 3*theta**2, 4*theta **
+                         3, 5*theta**4, 6*theta**5, 7*theta**6])
+
+    def T3(self, theta):
+        return np.array([0, 0, 2, 6*theta, 12*theta**2, 20*theta**3, 30*theta**4, 42*theta**5])
+
+    def T4(self, theta):
+        return np.array([0, 0, 0, 6, 24*theta, 60*theta**2, 120*theta**3, 210*theta**4])
+
+    def pd(self, theta):
+        s = theta - np.floor(theta)
+        i = int(np.floor(theta))
+        if i >= self.I:
+            i = 0
+            s = 0
+        point = self.T(s)@self.xn[i]
+        return np.array([point[0], point[1]]).T
+
+    def pd_s(self, theta):
+        s = theta - np.floor(theta)
+        i = int(np.floor(theta))
+        if i >= self.I:
+            i = 0
+            s = 0
+        point = self.T2(s)@self.xn[i]
+        return np.array([point[0], point[1]]).T
+
+    def pd_s2(self, theta):
+        s = theta - np.floor(theta)
+        i = int(np.floor(theta))
+        if i >= self.I:
+            i = 0
+            s = 0
+        point = self.T3(s)@self.xn[i]
+        return np.array([point[0], point[1]]).T
+
+    def pd_s3(self, theta):
+        s = theta - np.floor(theta)
+        i = int(np.floor(theta))
+        if i >= self.I:
+            i = 0
+            s = 0
+        point = self.T4(s)@self.xn[i]
+        return np.array([point[0], point[1]]).T
+
+    def eta_d(self, theta, psi_prev):
+        pd = self.pd(theta)
+        pd_s = self.pd_s(theta)
+        psi_d = np.arctan2(pd_s[1], pd_s[0])
+        return np.array([pd[0], pd[1], pipi2cont(psi_d, psi_prev)])
+
+    def eta_d_s(self, theta):
+        pd_s = self.pd_s(theta)
+        pd_s2 = self.pd_s2(theta)
+        psi_d_s = (pd_s2[1]*pd_s[0] - pd_s[1]*pd_s2[0]) / \
+            (pd_s[0]**2 + pd_s[1]**2)
+        return np.array([pd_s[0], pd_s[1], psi_d_s])
+
+    def eta_d_s2(self, theta):
+        pd_s = self.pd_s(theta)
+        pd_s2 = self.pd_s2(theta)
+        pd_s3 = self.pd_s3(theta)
+        psi_d_s2 = ((pd_s3[1]*pd_s[0] - pd_s[1]*pd_s3[0])*(pd_s[0]**2 + pd_s[1]**2) -
+                    2*(pd_s2[1]*pd_s[0] - pd_s[1]*pd_s2[0])*(pd_s[0]*pd_s2[0] + pd_s[1]*pd_s2[1])) / (pd_s[0]**2 + pd_s[1]**2)**2
+        return np.array([pd_s2[0], pd_s2[1], psi_d_s2])
+
+    def full_path(self, theta):
+        path = np.zeros((len(theta), 3))
+        for i in range(len(theta)):
+            path[i] = self.eta_d(theta[i], path[i-1, -1])
+        return path
+
+    def path_speed(self, theta):
+        speed = np.zeros((len(theta), 2))
+        for i in range(len(theta)):
+            speed[i] = self.pd_s(theta[i])
         return speed
```

### Comparing `MCSimPython-0.0.14/src/MCSimPython/observer/__init__.py` & `MCSimPython-0.1.1/src/MCSimPython/observer/__init__.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-"""
-Observer (:mod:`MCSimPython.observer`)
-=======================================
-
-The package consist of different observers
-for state estimation.
-
-Contents
---------
-
- - ekf.py: Extended Kalman Filter
- - nonlinobs.py: Nonlinear observers
-
-Description
------------
-
-The different observers are implemented as 
-classes, and are structured in different modules as
-listed in `contents`.
-
-Examples
---------
-
->>> from MCSimPython.observer import NonlinObs3dof
-
-Alternative import
-
->>> from MCSimPython.observer.nonlinobs import NonlinObs3dof
-
-Third option
-
->>> import MCSimPython.observer as obs
->>> estimator = obs.NonlinObs3dof(*args, **kwargs)
-"""
-
-from MCSimPython.observer.nonlinobs import NonlinObs3dof
+"""
+Observer (:mod:`MCSimPython.observer`)
+=======================================
+
+The package consist of different observers
+for state estimation.
+
+Contents
+--------
+
+ - ekf.py: Extended Kalman Filter
+ - nonlinobs.py: Nonlinear observers
+
+Description
+-----------
+
+The different observers are implemented as 
+classes, and are structured in different modules as
+listed in `contents`.
+
+Examples
+--------
+
+>>> from MCSimPython.observer import NonlinObs3dof
+
+Alternative import
+
+>>> from MCSimPython.observer.nonlinobs import NonlinObs3dof
+
+Third option
+
+>>> import MCSimPython.observer as obs
+>>> estimator = obs.NonlinObs3dof(*args, **kwargs)
+"""
+
+from MCSimPython.observer.nonlinobs import NonlinObs3dof
 from MCSimPython.observer.ekf import EKF
```

### Comparing `MCSimPython-0.0.14/src/MCSimPython/observer/ekf.py` & `MCSimPython-0.1.1/src/MCSimPython/observer/ekf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,676 +1,672 @@
-00000000: 0d0a 2320 656b 662e 7079 0d0a 2320 2d2d  ..# ekf.py..# --
+00000000: 0a23 2065 6b66 2e70 790a 2320 2d2d 2d2d  .# ekf.py.# ----
 00000010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00000020: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00000030: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00000040: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000050: 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2320 5468  ----------..# Th
-00000060: 6973 2063 6f64 6520 6973 2070 6172 7420  is code is part 
-00000070: 6f66 2074 6865 204d 4353 696d 5079 7468  of the MCSimPyth
-00000080: 6f6e 2074 6f6f 6c62 6f78 2061 6e64 2072  on toolbox and r
-00000090: 6570 6f73 6974 6f72 792e 0d0a 2320 4372  epository...# Cr
-000000a0: 6561 7465 6420 4279 3a20 4d6f 2c20 4b6f  eated By: Mo, Ko
-000000b0: 6e67 7368 6175 672c 2048 7967 656e 0d0a  ngshaug, Hygen..
-000000c0: 2320 4372 6561 7465 6420 4461 7465 3a20  # Created Date: 
-000000d0: 3230 3233 2d30 322d 3133 0d0a 2320 5265  2023-02-13..# Re
-000000e0: 7669 7365 643a 204e 2f41 0d0a 2320 5465  vised: N/A..# Te
-000000f0: 7374 6564 3a20 2032 3032 332d 3032 2d31  sted:  2023-02-1
-00000100: 3320 4675 6c6c 2074 6573 7420 6f66 206f  3 Full test of o
-00000110: 6273 6572 7665 7220 7065 7266 6f72 6d61  bserver performa
-00000120: 6e63 652e 2054 756e 696e 6720 6361 6e20  nce. Tuning can 
-00000130: 6265 2069 6d70 726f 7665 642e 0d0a 2320  be improved...# 
-00000140: 0d0a 2320 436f 7079 7269 6768 7420 2843  ..# Copyright (C
-00000150: 2920 3230 3233 3a20 4e54 4e55 2c20 5472  ) 2023: NTNU, Tr
-00000160: 6f6e 6468 6569 6d0d 0a23 204c 6963 656e  ondheim..# Licen
-00000170: 7365 6420 756e 6465 7220 4750 4c2d 332e  sed under GPL-3.
-00000180: 302d 6f72 2d6c 6174 6572 0d0a 2320 2d2d  0-or-later..# --
-00000190: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000001a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000001b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000001c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000001d0: 2d2d 2d2d 2d2d 2d2d 2d0d 0a0d 0a23 2049  ---------....# I
-000001e0: 6d70 6f72 7473 0d0a 696d 706f 7274 206e  mports..import n
-000001f0: 756d 7079 2061 7320 6e70 0d0a 6672 6f6d  umpy as np..from
-00000200: 204d 4353 696d 5079 7468 6f6e 2e75 7469   MCSimPython.uti
-00000210: 6c73 2069 6d70 6f72 7420 527a 2c20 7069  ls import Rz, pi
-00000220: 7069 2c20 7369 7832 7468 7265 6544 4f46  pi, six2threeDOF
-00000230: 0d0a 0d0a 0d0a 636c 6173 7320 454b 4628  ......class EKF(
-00000240: 293a 0d0a 2020 2020 2727 270d 0a20 2020  ):..    '''..   
-00000250: 2049 6d70 6c65 6d65 6e74 6174 696f 6e20   Implementation 
-00000260: 6f66 2045 7874 656e 6465 6420 4b61 6c6d  of Extended Kalm
-00000270: 616e 2046 696c 7465 7220 2845 4b46 2920  an Filter (EKF) 
-00000280: 666f 7220 4353 4144 2e0d 0a0d 0a20 2020  for CSAD.....   
-00000290: 2078 5f68 6174 203d 205b 0d0a 2020 2020   x_hat = [..    
-000002a0: 2020 2020 7a65 7461 2020 2020 2836 444f      zeta    (6DO
-000002b0: 4629 0d0a 2020 2020 2020 2020 6574 6120  F)..        eta 
-000002c0: 2020 2020 2833 444f 4629 0d0a 2020 2020      (3DOF)..    
-000002d0: 2020 2020 6269 6173 2020 2020 2833 444f      bias    (3DO
-000002e0: 4629 0d0a 2020 2020 2020 2020 6e75 2020  F)..        nu  
-000002f0: 2020 2020 2833 444f 4629 0d0a 2020 2020      (3DOF)..    
-00000300: 5d0d 0a20 2020 2027 2727 0d0a 2020 2020  ]..    '''..    
-00000310: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-00000320: 662c 2064 742c 204d 2c20 442c 2078 303d  f, dt, M, D, x0=
-00000330: 6e70 2e7a 6572 6f73 2831 3529 2c20 5030  np.zeros(15), P0
-00000340: 203d 206e 702e 7a65 726f 7328 2831 352c   = np.zeros((15,
-00000350: 3135 2929 293a 0d0a 2020 2020 2020 2020  15))):..        
-00000360: 2727 270d 0a20 2020 2020 2020 2049 6e69  '''..        Ini
-00000370: 7469 616c 697a 6174 696f 6e3a 0d0a 0d0a  tialization:....
-00000380: 2020 2020 2020 2020 5061 7261 6d73 3a0d          Params:.
-00000390: 0a20 2020 2020 2020 2020 2020 202d 2064  .            - d
-000003a0: 743a 2054 696d 6520 7374 6570 0d0a 2020  t: Time step..  
-000003b0: 2020 2020 2020 2020 2020 2d20 4d3a 2049            - M: I
-000003c0: 6e65 7274 6961 206d 6174 7269 7820 6f66  nertia matrix of
-000003d0: 2073 7973 7465 6d20 2869 6e63 6c75 6469   system (includi
-000003e0: 6e67 2061 6464 6564 206d 6173 7329 2036  ng added mass) 6
-000003f0: 444f 460d 0a20 2020 2020 2020 2020 2020  DOF..           
-00000400: 202d 2044 3a20 4675 6c6c 2064 616d 7069   - D: Full dampi
-00000410: 6e67 206d 6174 7269 7820 6f66 2073 7973  ng matrix of sys
-00000420: 7465 6d20 3644 4f46 0d0a 2020 2020 2020  tem 6DOF..      
-00000430: 2020 2727 270d 0a20 2020 2020 2020 2073    '''..        s
-00000440: 656c 662e 5f64 7420 3d20 6474 0d0a 0d0a  elf._dt = dt....
-00000450: 2020 2020 2020 2020 2320 5475 6e69 6e67          # Tuning
-00000460: 202d 2044 6f6e 6520 6d61 6e75 616c 6c79   - Done manually
-00000470: 2028 6173 206f 6620 6e6f 7729 0d0a 2020   (as of now)..  
-00000480: 2020 2020 2020 7365 6c66 2e5f 5164 203d        self._Qd =
-00000490: 206e 702e 6172 7261 7928 5b0d 0a20 2020   np.array([..   
-000004a0: 2020 2020 2020 2020 205b 3165 2d33 2c30           [1e-3,0
-000004b0: 2c30 2c30 2c30 2c30 5d2c 0d0a 2020 2020  ,0,0,0,0],..    
-000004c0: 2020 2020 2020 2020 5b30 2c31 652d 332c          [0,1e-3,
-000004d0: 302c 302c 302c 305d 2c0d 0a20 2020 2020  0,0,0,0],..     
-000004e0: 2020 2020 2020 205b 302c 302c 2e32 2a6e         [0,0,.2*n
-000004f0: 702e 7069 2f31 3830 2c30 2c30 2c30 5d2c  p.pi/180,0,0,0],
-00000500: 0d0a 2020 2020 2020 2020 2020 2020 5b30  ..            [0
-00000510: 2c30 2c30 2c31 6532 2c30 2c30 5d2c 0d0a  ,0,0,1e2,0,0],..
-00000520: 2020 2020 2020 2020 2020 2020 5b30 2c30              [0,0
-00000530: 2c30 2c30 2c35 6532 2c30 5d2c 0d0a 2020  ,0,0,5e2,0],..  
-00000540: 2020 2020 2020 2020 2020 5b30 2c30 2c30            [0,0,0
-00000550: 2c30 2c30 2c31 6531 5d0d 0a20 2020 2020  ,0,0,1e1]..     
-00000560: 2020 205d 290d 0a20 2020 2020 2020 2023     ])..        #
-00000570: 204d 696e 6b65 2033 2066 c3b8 7273 7465   Minke 3 f..rste
-00000580: 2067 6972 3a20 6d69 6e64 7265 2073 74c3   gir: mindre st.
-00000590: b879 2070 c3a5 2076 656c 202b 2064 c3a5  .y p.. vel + d..
-000005a0: 726c 6967 6572 6520 706f 730d 0a20 2020  rligere pos..   
-000005b0: 2020 2020 2023 20c3 986b 6520 3320 7369       # ..ke 3 si
-000005c0: 7374 6520 6769 7220 6265 6472 6520 706f  ste gir bedre po
-000005d0: 7320 6573 7469 6d61 7465 722c 202b 206d  s estimater, + m
-000005e0: 6572 2073 74c3 b879 2070 c3a5 2076 656c  er st..y p.. vel
-000005f0: 0d0a 2020 2020 2020 2020 2320 53c3 a56e  ..        # S..n
-00000600: 6e20 6973 682e 2e2e 0d0a 2020 2020 2020  n ish.....      
-00000610: 2020 7365 6c66 2e5f 5264 203d 206e 702e    self._Rd = np.
-00000620: 6172 7261 7928 5b0d 0a20 2020 2020 2020  array([..       
-00000630: 2020 2020 205b 3130 302c 302c 305d 2c0d       [100,0,0],.
-00000640: 0a20 2020 2020 2020 2020 2020 205b 302c  .            [0,
-00000650: 3130 2c30 5d2c 0d0a 2020 2020 2020 2020  10,0],..        
-00000660: 2020 2020 5b30 2c30 2c35 3030 2a6e 702e      [0,0,500*np.
-00000670: 7069 2f31 3830 5d0d 0a20 2020 2020 2020  pi/180]..       
-00000680: 205d 290d 0a20 2020 2020 2020 2023 7365   ])..        #se
-00000690: 6c66 2e5f 5164 203d 206e 702e 6579 6528  lf._Qd = np.eye(
-000006a0: 3629 2a2e 3031 0d0a 2020 2020 2020 2020  6)*.01..        
-000006b0: 2373 656c 662e 5f52 6420 3d20 6e70 2e65  #self._Rd = np.e
-000006c0: 7965 2833 290d 0a0d 0a20 2020 2020 2020  ye(3)....       
-000006d0: 2023 2043 6f6e 7374 616e 7420 6d61 7472   # Constant matr
-000006e0: 6963 6573 0d0a 2020 2020 2020 2020 2369  ices..        #i
-000006f0: 203d 206e 702e 6978 5f28 5b30 2c31 2c35   = np.ix_([0,1,5
-00000700: 5d2c 5b30 2c31 2c35 5d29 2020 2020 2020  ],[0,1,5])      
-00000710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000730: 2020 2023 2045 7874 7261 6374 2073 7572     # Extract sur
-00000740: 6765 2d73 7761 792d 7961 7720 444f 4673  ge-sway-yaw DOFs
-00000750: 0d0a 2020 2020 2020 2020 234d 203d 204d  ..        #M = M
-00000760: 5b69 5d0d 0a20 2020 2020 2020 204d 203d  [i]..        M =
-00000770: 2073 6978 3274 6872 6565 444f 4628 4d29   six2threeDOF(M)
-00000780: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-00000790: 4d69 6e76 203d 206e 702e 6c69 6e61 6c67  Minv = np.linalg
-000007a0: 2e69 6e76 284d 2920 2020 2020 2020 2020  .inv(M)         
-000007b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007c0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-000007d0: 3344 4f46 2069 6e76 6572 7465 6420 6d61  3DOF inverted ma
-000007e0: 7373 206d 6174 7269 780d 0a20 2020 2020  ss matrix..     
-000007f0: 2020 2073 656c 662e 5f44 203d 2073 6978     self._D = six
-00000800: 3274 6872 6565 444f 4628 4429 2020 2020  2threeDOF(D)    
-00000810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000830: 2020 2020 2020 2023 2033 444f 4620 6461         # 3DOF da
-00000840: 6d70 696e 6720 6d61 7472 6978 0d0a 2020  mping matrix..  
-00000850: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00000860: 7365 6c66 2e5f 482c 2073 656c 662e 5f42  self._H, self._B
-00000870: 2c20 7365 6c66 2e5f 452c 2073 656c 662e  , self._E, self.
-00000880: 5f41 772c 2073 656c 662e 5f67 616d 6d61  _Aw, self._gamma
-00000890: 203d 2030 2c30 2c30 2c30 2c30 0d0a 2020   = 0,0,0,0,0..  
-000008a0: 2020 2020 2020 7365 6c66 2e69 6e69 7469        self.initi
-000008b0: 616c 697a 655f 636f 6e73 7461 6e74 5f6d  alize_constant_m
-000008c0: 6174 7269 6365 7328 290d 0a20 2020 2020  atrices()..     
-000008d0: 2020 200d 0a20 2020 2020 2020 200d 0a20     ..        .. 
-000008e0: 2020 2020 2020 2023 2049 6e69 7469 616c         # Initial
-000008f0: 2076 616c 7565 730d 0a20 2020 2020 2020   values..       
-00000900: 2073 656c 662e 5f78 6861 7420 3d20 6e70   self._xhat = np
-00000910: 2e7a 6572 6f73 2831 3529 0d0a 2020 2020  .zeros(15)..    
-00000920: 2020 2020 7365 6c66 2e5f 7862 6172 203d      self._xbar =
-00000930: 2078 300d 0a0d 0a20 2020 2020 2020 2073   x0....        s
-00000940: 656c 662e 5f50 6261 7220 3d20 5030 0d0a  elf._Pbar = P0..
-00000950: 2020 2020 2020 2020 7365 6c66 2e5f 5068          self._Ph
-00000960: 6174 203d 206e 702e 7a65 726f 7328 2831  at = np.zeros((1
-00000970: 352c 3135 2929 0d0a 2020 2020 0d0a 2020  5,15))..    ..  
-00000980: 2020 0d0a 2020 2020 2020 0d0a 2020 2020    ..      ..    
-00000990: 6465 6620 7570 6461 7465 2873 656c 662c  def update(self,
-000009a0: 2074 6175 2c20 7929 3a0d 0a20 2020 2020   tau, y):..     
-000009b0: 2020 2027 2727 0d0a 2020 2020 2020 2020     '''..        
-000009c0: 5570 6461 7465 3a0d 0a20 2020 2020 2020  Update:..       
-000009d0: 2055 7064 6174 6520 6675 6e63 7469 6f6e   Update function
-000009e0: 2074 6f20 6265 2063 616c 6c65 6420 6174   to be called at
-000009f0: 2065 7665 7279 2074 696d 6573 7465 7020   every timestep 
-00000a00: 6475 7269 6e67 2061 2073 696d 756c 6174  during a simulat
-00000a10: 696f 6e2e 2043 616c 6c73 2074 6865 2070  ion. Calls the p
-00000a20: 7265 6469 6374 6f72 2061 6e64 2063 6f72  redictor and cor
-00000a30: 7265 6374 6f72 2e0d 0a0d 0a20 2020 2020  rector.....     
-00000a40: 2020 2050 6172 616d 6574 6572 733a 0d0a     Parameters:..
-00000a50: 2020 2020 2020 2020 2020 2020 2d20 7461              - ta
-00000a60: 753a 2043 6f6e 7472 6f6c 2050 6172 616d  u: Control Param
-00000a70: 6574 6572 7320 2833 444f 4629 0d0a 2020  eters (3DOF)..  
-00000a80: 2020 2020 2020 2020 2020 2d20 793a 204d            - y: M
-00000a90: 6561 7375 7265 6420 706f 7369 7469 6f6e  easured position
-00000aa0: 2028 3344 4f46 290d 0a0d 0a20 2020 2020   (3DOF)....     
-00000ab0: 2020 2054 6f20 6265 2069 6d70 6c65 6d65     To be impleme
-00000ac0: 6e74 6564 202f 2049 6d70 726f 7665 6d65  nted / Improveme
-00000ad0: 6e74 733a 0d0a 2020 2020 2020 2020 2020  nts:..          
-00000ae0: 2020 2d20 4572 726f 7220 6368 6563 6b73    - Error checks
-00000af0: 3f0d 0a20 2020 2020 2020 2020 2020 202d  ?..            -
-00000b00: 2041 7379 6e63 6872 6f6e 6f75 7320 6d65   Asynchronous me
-00000b10: 6173 7572 656d 656e 7473 3f0d 0a20 2020  asurements?..   
-00000b20: 2020 2020 2020 2020 202d 2053 6574 2079           - Set y
-00000b30: 2074 6f20 6e61 6e20 6966 206e 6f20 6d65   to nan if no me
-00000b40: 6173 7572 656d 656e 740d 0a20 2020 2020  asurement..     
-00000b50: 2020 2027 2727 0d0a 2020 2020 2020 2020     '''..        
-00000b60: 2320 5072 6564 6963 7420 2020 2020 2020  # Predict       
-00000b70: 200d 0a20 2020 2020 2020 2073 656c 662e   ..        self.
-00000b80: 7072 6564 6963 746f 7228 7461 7529 0d0a  predictor(tau)..
-00000b90: 2020 2020 2020 2020 2320 436f 7272 6563          # Correc
-00000ba0: 740d 0a20 2020 2020 2020 2073 656c 662e  t..        self.
-00000bb0: 636f 7272 6563 746f 7228 7929 0d0a 0d0a  corrector(y)....
-00000bc0: 2020 2020 0d0a 2020 2020 6465 6620 7072      ..    def pr
-00000bd0: 6564 6963 746f 7228 7365 6c66 2c20 7461  edictor(self, ta
-00000be0: 7529 3a0d 0a20 2020 2020 2020 2027 2727  u):..        '''
-00000bf0: 0d0a 2020 2020 2020 2020 5072 6564 6963  ..        Predic
-00000c00: 746f 723a 0d0a 2020 2020 2020 2020 5573  tor:..        Us
-00000c10: 6564 2074 6f20 6573 7469 6d61 7465 2074  ed to estimate t
-00000c20: 6865 2073 7461 7465 206f 6620 7468 6520  he state of the 
-00000c30: 7379 7374 656d 2061 7420 7468 6520 6e65  system at the ne
-00000c40: 7874 2074 696d 6520 7374 6570 2062 6173  xt time step bas
-00000c50: 6564 206f 6e20 7468 6520 6375 7272 656e  ed on the curren
-00000c60: 7420 7374 6174 6520 6573 7469 6d61 7465  t state estimate
-00000c70: 2061 6e64 2074 6865 2073 7973 7465 6d20   and the system 
-00000c80: 6479 6e61 6d69 6373 206d 6f64 656c 2e0d  dynamics model..
-00000c90: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-00000ca0: 2020 2050 6172 616d 6574 6572 733a 0d0a     Parameters:..
-00000cb0: 2020 2020 2020 2020 2020 2020 2d20 7461              - ta
-00000cc0: 7520 3d20 5b58 2c20 592c 204e 5d27 2c20  u = [X, Y, N]', 
-00000cd0: 2043 6f6e 7472 6f6c 2069 6e70 7574 2028   Control input (
-00000ce0: 3344 4f46 290d 0a0d 0a20 2020 2020 2020  3DOF)....       
-00000cf0: 2054 6f20 6265 2069 6d70 6c65 6d65 6e74   To be implement
-00000d00: 6564 202f 2049 6d70 726f 7665 6d65 6e74  ed / Improvement
-00000d10: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00000d20: 2d20 0d0a 2020 2020 2020 2020 2727 270d  - ..        '''.
-00000d30: 0a20 2020 2020 2020 2070 6869 203d 2073  .        phi = s
-00000d40: 656c 662e 7374 6174 655f 6675 6e63 7469  elf.state_functi
-00000d50: 6f6e 5f6a 6163 6f62 6961 6e28 290d 0a20  on_jacobian().. 
-00000d60: 2020 2020 2020 2066 203d 2073 656c 662e         f = self.
-00000d70: 7374 6174 655f 6675 6e63 7469 6f6e 2873  state_function(s
-00000d80: 656c 662e 5f78 6861 742c 2074 6175 2c20  elf._xhat, tau, 
-00000d90: 6e70 2e7a 6572 6f73 2836 2929 0d0a 0d0a  np.zeros(6))....
-00000da0: 2020 2020 2020 2020 7365 6c66 2e5f 5062          self._Pb
-00000db0: 6172 203d 2070 6869 4073 656c 662e 5f50  ar = phi@self._P
-00000dc0: 6861 7440 2870 6869 2e54 2920 2b20 7365  hat@(phi.T) + se
-00000dd0: 6c66 2e5f 6761 6d6d 6140 7365 6c66 2e5f  lf._gamma@self._
-00000de0: 5164 4028 7365 6c66 2e5f 6761 6d6d 612e  Qd@(self._gamma.
-00000df0: 5429 0d0a 2020 2020 2020 2020 7365 6c66  T)..        self
-00000e00: 2e5f 7862 6172 203d 2073 656c 662e 5f78  ._xbar = self._x
-00000e10: 6861 7420 2b20 7365 6c66 2e5f 6474 202a  hat + self._dt *
-00000e20: 2066 0d0a 0d0a 0d0a 2020 2020 6465 6620   f......    def 
-00000e30: 636f 7272 6563 746f 7228 7365 6c66 2c20  corrector(self, 
-00000e40: 7929 3a0d 0a20 2020 2020 2020 2027 2727  y):..        '''
-00000e50: 0d0a 2020 2020 2020 2020 436f 7272 6563  ..        Correc
-00000e60: 746f 723a 0d0a 2020 2020 2020 2020 5573  tor:..        Us
-00000e70: 6564 2074 6f20 7265 6669 6e65 2074 6865  ed to refine the
-00000e80: 2070 7265 6469 6374 6564 2073 7461 7465   predicted state
-00000e90: 2065 7374 696d 6174 6520 6672 6f6d 2074   estimate from t
-00000ea0: 6865 2070 7265 6469 6374 6f72 2c20 6261  he predictor, ba
-00000eb0: 7365 6420 6f6e 2074 6865 206f 6274 6169  sed on the obtai
-00000ec0: 6e65 6420 6d65 6173 7572 656d 656e 7473  ned measurements
-00000ed0: 2e20 5468 6520 6675 6e63 7469 6f6e 2063  . The function c
-00000ee0: 6865 636b 7320 666f 7220 7369 676e 616c  hecks for signal
-00000ef0: 206c 6f73 7320 286e 6f20 6d65 6173 7572   loss (no measur
-00000f00: 656d 656e 7429 2e0d 0a0d 0a20 2020 2020  ement).....     
-00000f10: 2020 2050 6172 616d 6574 6572 733a 0d0a     Parameters:..
-00000f20: 2020 2020 2020 2020 2020 2020 2d20 7920              - y 
-00000f30: 3d20 5b65 7461 3120 2065 7461 3220 2065  = [eta1  eta2  e
-00000f40: 7461 365d 272c 204d 6561 7375 7265 6d65  ta6]', Measureme
-00000f50: 6e74 7320 2833 444f 4629 200d 0a0d 0a20  nts (3DOF) .... 
-00000f60: 2020 2020 2020 2054 6f20 6265 2069 6d70         To be imp
-00000f70: 6c65 6d65 6e74 6564 202f 2049 6d70 726f  lemented / Impro
-00000f80: 7665 6d65 6e74 733a 0d0a 2020 2020 2020  vements:..      
-00000f90: 2020 2020 2020 2d20 4368 6563 6b20 6966        - Check if
-00000fa0: 206d 6561 7375 7265 6d65 6e74 2069 7320   measurement is 
-00000fb0: 6769 7665 6e2e 2043 616e 2061 6c73 6f20  given. Can also 
-00000fc0: 6265 206d 6164 6520 7769 7468 206d 6f64  be made with mod
-00000fd0: 756c 7573 206f 7065 7261 746f 7220 6966  ulus operator if
-00000fe0: 206d 6561 7375 7265 6d65 6e74 2066 7265   measurement fre
-00000ff0: 7120 6973 2064 6966 6665 7265 6e74 2066  q is different f
-00001000: 726f 6d20 6474 2e0d 0a20 2020 2020 2020  rom dt...       
-00001010: 2020 2020 202d 200d 0a20 2020 2020 2020       - ..       
-00001020: 2027 2727 0d0a 0d0a 2020 2020 2020 2020   '''....        
-00001030: 6966 206e 702e 616e 7928 6e70 2e69 736e  if np.any(np.isn
-00001040: 616e 2879 2929 203d 3d20 5472 7565 3a20  an(y)) == True: 
-00001050: 2020 2023 2049 6620 6e6f 206e 6577 206d     # If no new m
-00001060: 6561 7375 7265 6d65 6e74 733a 2053 6574  easurements: Set
-00001070: 2063 6f72 7265 6374 6f72 2065 7175 616c   corrector equal
-00001080: 2074 6f20 7072 6564 6963 746f 720d 0a20   to predictor.. 
-00001090: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000010a0: 5f50 6861 7420 3d20 7365 6c66 2e5f 5062  _Phat = self._Pb
-000010b0: 6172 0d0a 2020 2020 2020 2020 2020 2020  ar..            
-000010c0: 7365 6c66 2e5f 7868 6174 203d 2073 656c  self._xhat = sel
-000010d0: 662e 5f78 6261 720d 0a20 2020 2020 2020  f._xbar..       
-000010e0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-000010f0: 2020 2020 4b20 3d20 7365 6c66 2e45 4b46      K = self.EKF
-00001100: 5f67 6169 6e0d 0a0d 0a20 2020 2020 2020  _gain....       
-00001110: 2020 2020 2070 6172 656e 7468 6573 6973       parenthesis
-00001120: 203d 206e 702e 6579 6528 3135 2920 2d20   = np.eye(15) - 
-00001130: 4b40 7365 6c66 2e5f 480d 0a0d 0a20 2020  K@self._H....   
-00001140: 2020 2020 2020 2020 2070 7265 6469 6374           predict
-00001150: 696f 6e5f 6572 726f 7220 3d20 7920 2d20  ion_error = y - 
-00001160: 2873 656c 662e 5f48 4073 656c 662e 5f78  (self._H@self._x
-00001170: 6261 7229 0d0a 2020 2020 2020 2020 2020  bar)..          
-00001180: 2020 7072 6564 6963 7469 6f6e 5f65 7272    prediction_err
-00001190: 6f72 5b32 5d20 3d20 7069 7069 2870 7265  or[2] = pipi(pre
-000011a0: 6469 6374 696f 6e5f 6572 726f 725b 325d  diction_error[2]
-000011b0: 2920 2020 2320 536d 616c 6c65 7374 2073  )   # Smallest s
-000011c0: 6967 6e65 6420 616e 676c 6520 6d6f 6469  igned angle modi
-000011d0: 6669 6361 7469 6f6e 0d0a 0d0a 2020 2020  fication....    
-000011e0: 2020 2020 2020 2020 7365 6c66 2e5f 5068          self._Ph
-000011f0: 6174 203d 2070 6172 656e 7468 6573 6973  at = parenthesis
-00001200: 4073 656c 662e 5f50 6261 7240 2870 6172  @self._Pbar@(par
-00001210: 656e 7468 6573 6973 2e54 2920 2b20 4b40  enthesis.T) + K@
-00001220: 7365 6c66 2e5f 5264 4028 4b2e 5429 0d0a  self._Rd@(K.T)..
-00001230: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00001240: 2e5f 7868 6174 203d 2073 656c 662e 5f78  ._xhat = self._x
-00001250: 6261 7220 2b20 4b40 7072 6564 6963 7469  bar + K@predicti
-00001260: 6f6e 5f65 7272 6f72 0d0a 2020 2020 2020  on_error..      
-00001270: 2020 0d0a 0d0a 2020 2020 4070 726f 7065    ....    @prope
-00001280: 7274 790d 0a20 2020 2064 6566 2045 4b46  rty..    def EKF
-00001290: 5f67 6169 6e28 7365 6c66 293a 0d0a 2020  _gain(self):..  
-000012a0: 2020 2020 2020 2727 270d 0a20 2020 2020        '''..     
-000012b0: 2020 204b 616c 6d61 6e20 6761 696e 3a0d     Kalman gain:.
-000012c0: 0a20 2020 2020 2020 2055 7365 6420 746f  .        Used to
-000012d0: 2062 616c 616e 6365 2074 6865 2063 6f6e   balance the con
-000012e0: 7472 6962 7574 696f 6e73 206f 6620 7468  tributions of th
-000012f0: 6520 7072 6564 6963 7465 6420 7374 6174  e predicted stat
-00001300: 6520 6573 7469 6d61 7465 2061 6e64 2074  e estimate and t
-00001310: 6865 206d 6561 7375 7265 6d65 6e74 2064  he measurement d
-00001320: 6174 6120 696e 2074 6865 2075 7064 6174  ata in the updat
-00001330: 6564 2065 7374 696d 6174 652e 0d0a 0d0a  ed estimate.....
-00001340: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-00001350: 7273 3a0d 0a20 2020 2020 2020 2020 2020  rs:..           
-00001360: 202d 204e 2f41 0d0a 2020 2020 2020 2020   - N/A..        
-00001370: 4f75 7470 7574 3a0d 0a20 2020 2020 2020  Output:..       
-00001380: 2020 2020 202d 204b 3a20 4b61 6c6d 616e       - K: Kalman
-00001390: 2067 6169 6e20 2844 696d 203d 2031 3578   gain (Dim = 15x
-000013a0: 3329 0d0a 0d0a 2020 2020 2020 2020 546f  3)....        To
-000013b0: 2062 6520 696d 706c 656d 656e 7465 6420   be implemented 
-000013c0: 2f20 496d 7072 6f76 656d 656e 7473 3a0d  / Improvements:.
-000013d0: 0a20 2020 2020 2020 2020 2020 202d 200d  .            - .
-000013e0: 0a20 2020 2020 2020 2027 2727 0d0a 2020  .        '''..  
-000013f0: 2020 2020 2020 7061 7265 6e74 6865 7369        parenthesi
-00001400: 7320 3d20 7365 6c66 2e5f 4840 7365 6c66  s = self._H@self
-00001410: 2e5f 5062 6172 4028 7365 6c66 2e5f 482e  ._Pbar@(self._H.
-00001420: 5429 202b 2073 656c 662e 5f52 640d 0a20  T) + self._Rd.. 
-00001430: 2020 2020 2020 204b 203d 2073 656c 662e         K = self.
-00001440: 5f50 6261 7240 2873 656c 662e 5f48 2e54  _Pbar@(self._H.T
-00001450: 2940 6e70 2e6c 696e 616c 672e 696e 7628  )@np.linalg.inv(
-00001460: 7061 7265 6e74 6865 7369 7329 0d0a 2020  parenthesis)..  
-00001470: 2020 2020 2020 7265 7475 726e 204b 0d0a        return K..
-00001480: 0d0a 0d0a 2020 2020 6465 6620 7374 6174  ....    def stat
-00001490: 655f 6675 6e63 7469 6f6e 2873 656c 662c  e_function(self,
-000014a0: 2078 2c20 7461 752c 206e 6f69 7365 293a   x, tau, noise):
-000014b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014c0: 2020 2020 2320 6628 782c 752c 7729 0d0a      # f(x,u,w)..
-000014d0: 2020 2020 2020 2020 2727 270d 0a20 2020          '''..   
-000014e0: 2020 2020 2078 5f64 6f74 203d 2041 2878       x_dot = A(x
-000014f0: 2920 2b20 422a 7461 7520 2b20 452a 7720  ) + B*tau + E*w 
-00001500: 2020 2020 203d 2066 2878 2c75 2c77 290d       = f(x,u,w).
-00001510: 0a0d 0a20 2020 2020 2020 2077 6865 7265  ...        where
-00001520: 2041 2878 2920 3d20 5b0d 0a20 2020 2020   A(x) = [..     
-00001530: 2020 2020 2020 2041 7720 2a20 7869 0d0a         Aw * xi..
-00001540: 2020 2020 2020 2020 2020 2020 5228 7073              R(ps
-00001550: 6929 202a 206e 750d 0a20 2020 2020 2020  i) * nu..       
-00001560: 2020 2020 2030 5f28 3378 3129 0d0a 2020       0_(3x1)..  
-00001570: 2020 2020 2020 2020 2020 2d4d 5f69 6e76            -M_inv
-00001580: 2a44 202a 206e 7520 2b20 4d5f 696e 762a  *D * nu + M_inv*
-00001590: 5228 7073 6929 2e54 202a 2062 0d0a 2020  R(psi).T * b..  
-000015a0: 2020 2020 2020 5d0d 0a0d 0a20 2020 2020        ]....     
-000015b0: 2020 2050 6172 616d 6574 6572 733a 0d0a     Parameters:..
-000015c0: 2020 2020 2020 2020 2020 2020 2d20 783a              - x:
-000015d0: 2073 7461 7465 2076 6563 746f 7220 2844   state vector (D
-000015e0: 696d 203d 2031 3529 0d0a 2020 2020 2020  im = 15)..      
-000015f0: 2020 2020 2020 2d20 7461 753a 2043 6f6e        - tau: Con
-00001600: 7472 6f6c 2076 6563 746f 7220 5b58 2020  trol vector [X  
-00001610: 5920 204e 5d0d 0a20 2020 2020 2020 2020  Y  N]..         
-00001620: 2020 202d 206e 6f69 7365 3a20 4d6f 6465     - noise: Mode
-00001630: 6c6c 6564 2077 6869 7465 206e 6f69 7365  lled white noise
-00001640: 2c20 7365 7420 746f 207a 6572 6f20 696e  , set to zero in
-00001650: 2061 2064 6574 6572 6d69 6e69 7374 6963   a deterministic
-00001660: 2045 4b46 2e20 2844 696d 3d36 290d 0a20   EKF. (Dim=6).. 
-00001670: 2020 2020 2020 204f 7574 7075 743a 0d0a         Output:..
-00001680: 2020 2020 2020 2020 2020 2020 2d20 663a              - f:
-00001690: 2078 5f64 6f74 2028 4469 6d20 3d20 3135   x_dot (Dim = 15
-000016a0: 290d 0a0d 0a20 2020 2020 2020 2054 6f20  )....        To 
-000016b0: 6265 2069 6d70 6c65 6d65 6e74 6564 202f  be implemented /
-000016c0: 2049 6d70 726f 7665 6d65 6e74 733a 0d0a   Improvements:..
-000016d0: 2020 2020 2020 2020 2020 2020 2d20 0d0a              - ..
-000016e0: 2020 2020 2020 2020 2727 270d 0a20 2020          '''..   
-000016f0: 2020 2020 2078 6920 3d20 785b 303a 365d       xi = x[0:6]
-00001700: 0d0a 2020 2020 2020 2020 6574 6120 3d20  ..        eta = 
-00001710: 785b 363a 395d 0d0a 2020 2020 2020 2020  x[6:9]..        
-00001720: 7073 6920 3d20 6574 615b 325d 0d0a 2020  psi = eta[2]..  
-00001730: 2020 2020 2020 6220 3d20 785b 393a 3132        b = x[9:12
-00001740: 5d0d 0a20 2020 2020 2020 206e 7520 3d20  ]..        nu = 
-00001750: 785b 3132 3a31 355d 0d0a 0d0a 2020 2020  x[12:15]....    
-00001760: 2020 2020 4178 203d 206e 702e 6172 7261      Ax = np.arra
-00001770: 7928 0d0a 2020 2020 2020 2020 2020 2020  y(..            
-00001780: 5b0d 0a20 2020 2020 2020 2020 2020 2028  [..            (
-00001790: 7365 6c66 2e5f 4177 4078 6929 2c0d 0a20  self._Aw@xi),.. 
-000017a0: 2020 2020 2020 2020 2020 2028 527a 2870             (Rz(p
-000017b0: 7369 2940 6e75 292c 0d0a 2020 2020 2020  si)@nu),..      
-000017c0: 2020 2020 2020 6e70 2e7a 6572 6f73 2833        np.zeros(3
-000017d0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-000017e0: 282d 7365 6c66 2e5f 4d69 6e76 4073 656c  (-self._Minv@sel
-000017f0: 662e 5f44 406e 7520 2b20 7365 6c66 2e5f  f._D@nu + self._
-00001800: 4d69 6e76 4028 527a 2870 7369 292e 5429  Minv@(Rz(psi).T)
-00001810: 4062 2920 2020 2020 2320 706c 7573 206f  @b)     # plus o
-00001820: 7220 6d69 6e75 7320 696e 2032 6e64 2074  r minus in 2nd t
-00001830: 6572 6d3f 0d0a 2020 2020 2020 2020 2020  erm?..          
-00001840: 2020 5d2c 2064 7479 7065 3d6f 626a 6563    ], dtype=objec
-00001850: 740d 0a20 2020 2020 2020 2029 0d0a 0d0a  t..        )....
-00001860: 2020 2020 2020 2020 4178 203d 206e 702e          Ax = np.
-00001870: 636f 6e63 6174 656e 6174 6528 4178 2920  concatenate(Ax) 
-00001880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018a0: 2020 2020 2320 436f 6e76 6572 7420 746f      # Convert to
-000018b0: 2031 3578 310d 0a0d 0a20 2020 2020 2020   15x1....       
-000018c0: 2066 203d 2041 7820 2b20 7365 6c66 2e5f   f = Ax + self._
-000018d0: 4240 7461 7520 2b20 7365 6c66 2e5f 4540  B@tau + self._E@
-000018e0: 6e6f 6973 650d 0a20 2020 2020 2020 2072  noise..        r
-000018f0: 6574 7572 6e20 660d 0a0d 0a0d 0a20 2020  eturn f......   
-00001900: 2064 6566 2073 7461 7465 5f66 756e 6374   def state_funct
-00001910: 696f 6e5f 6a61 636f 6269 616e 2873 656c  ion_jacobian(sel
-00001920: 6629 3a20 2020 2020 2020 2320 6466 2f64  f):       # df/d
-00001930: 780d 0a20 2020 2020 2020 2027 2727 0d0a  x..        '''..
-00001940: 2020 2020 2020 2020 7068 6920 3d20 6579          phi = ey
-00001950: 6528 3135 2920 2b20 6474 202a 2064 656c  e(15) + dt * del
-00001960: 2866 292f 6465 6c28 7829 0d0a 0d0a 2020  (f)/del(x)....  
-00001970: 2020 2020 2020 7768 6572 650d 0a0d 0a20        where.... 
-00001980: 2020 2020 2020 2064 656c 2866 292f 6465         del(f)/de
-00001990: 6c28 7829 203d 205b 0d0a 2020 2020 2020  l(x) = [..      
-000019a0: 2020 2020 2020 726f 7720 2831 293a 2020        row (1):  
-000019b0: 2020 2020 2020 415f 7720 2020 2020 2020        A_w       
-000019c0: 2020 305f 2836 7833 2920 2020 2020 305f    0_(6x3)     0_
-000019d0: 2836 7833 2920 2020 2020 2020 2020 305f  (6x3)         0_
-000019e0: 2836 7833 2920 2020 2020 2020 2020 2020  (6x3)           
-000019f0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00001a00: 2020 2020 726f 7720 2832 293a 2020 2020      row (2):    
-00001a10: 2020 2020 305f 2833 7836 2920 2020 2020      0_(3x6)     
-00001a20: 6465 6c5f 6632 2020 2020 2020 305f 2833  del_f2      0_(3
-00001a30: 7833 2920 2020 2020 2020 2020 5228 7073  x3)         R(ps
-00001a40: 6929 2020 2020 2020 2020 2020 2020 2020  i)              
-00001a50: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00001a60: 2020 726f 7720 2833 293a 2020 2020 2020    row (3):      
-00001a70: 2020 305f 2833 7836 2920 2020 2020 305f    0_(3x6)     0_
-00001a80: 2833 7833 2920 2020 2020 305f 2833 7833  (3x3)     0_(3x3
-00001a90: 2920 2020 2020 2020 2020 305f 2833 7833  )         0_(3x3
-00001aa0: 2920 2020 2020 2020 2020 2020 2020 2020  )               
-00001ab0: 200d 0a20 2020 2020 2020 2020 2020 2072   ..            r
-00001ac0: 6f77 2028 3429 3a20 2020 2020 2020 2030  ow (4):        0
-00001ad0: 5f28 3378 3629 2020 2020 2064 656c 5f66  _(3x6)     del_f
-00001ae0: 3420 2020 2020 204d 5f69 6e76 2a52 2870  4      M_inv*R(p
-00001af0: 7369 292e 5420 202d 4d5f 696e 762a 4420  si).T  -M_inv*D 
-00001b00: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00001b10: 0a20 2020 2020 2020 205d 2020 200d 0a0d  .        ]   ...
-00001b20: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-00001b30: 6572 733a 0d0a 2020 2020 2020 2020 2020  ers:..          
-00001b40: 2020 2d20 4e2f 410d 0a20 2020 2020 2020    - N/A..       
-00001b50: 204f 7574 7075 743a 0d0a 2020 2020 2020   Output:..      
-00001b60: 2020 2020 2020 2d20 7068 693a 2044 6973        - phi: Dis
-00001b70: 6372 6574 697a 6564 206a 6163 6f62 6961  cretized jacobia
-00001b80: 6e20 6f66 2073 7973 7465 6d20 6479 6e61  n of system dyna
-00001b90: 6d69 6373 2028 4469 6d20 3d20 3135 7831  mics (Dim = 15x1
-00001ba0: 3529 0d0a 0d0a 2020 2020 2020 2020 546f  5)....        To
-00001bb0: 2062 6520 696d 706c 656d 656e 7465 6420   be implemented 
-00001bc0: 2f20 496d 7072 6f76 656d 656e 7473 3a0d  / Improvements:.
-00001bd0: 0a20 2020 2020 2020 2020 2020 202d 200d  .            - .
-00001be0: 0a20 2020 2020 2020 2027 2727 0d0a 2020  .        '''..  
-00001bf0: 2020 2020 2020 2320 4578 7472 6163 7420        # Extract 
-00001c00: 7374 6174 6573 0d0a 2020 2020 2020 2020  states..        
-00001c10: 7073 6920 3d20 7365 6c66 2e5f 7868 6174  psi = self._xhat
-00001c20: 5b38 5d0d 0a20 2020 2020 2020 2062 3120  [8]..        b1 
-00001c30: 3d20 7365 6c66 2e5f 7868 6174 5b39 5d0d  = self._xhat[9].
-00001c40: 0a20 2020 2020 2020 2062 3220 3d20 7365  .        b2 = se
-00001c50: 6c66 2e5f 7868 6174 5b31 305d 0d0a 2020  lf._xhat[10]..  
-00001c60: 2020 2020 2020 7520 3d20 7365 6c66 2e5f        u = self._
-00001c70: 7868 6174 5b31 325d 0d0a 2020 2020 2020  xhat[12]..      
-00001c80: 2020 7620 3d20 7365 6c66 2e5f 7868 6174    v = self._xhat
-00001c90: 5b31 335d 0d0a 0d0a 2020 2020 2020 2020  [13]....        
-00001ca0: 6465 6c5f 6632 203d 206e 702e 6172 7261  del_f2 = np.arra
-00001cb0: 7928 5b0d 0a20 2020 2020 2020 2020 2020  y([..           
-00001cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001cd0: 205b 302c 302c 2d75 2a6e 702e 7369 6e28   [0,0,-u*np.sin(
-00001ce0: 7073 6929 2d76 2a6e 702e 636f 7328 7073  psi)-v*np.cos(ps
-00001cf0: 6929 5d2c 0d0a 2020 2020 2020 2020 2020  i)],..          
+00000050: 2d2d 2d2d 2d2d 2d2d 0a23 2054 6869 7320  --------.# This 
+00000060: 636f 6465 2069 7320 7061 7274 206f 6620  code is part of 
+00000070: 7468 6520 4d43 5369 6d50 7974 686f 6e20  the MCSimPython 
+00000080: 746f 6f6c 626f 7820 616e 6420 7265 706f  toolbox and repo
+00000090: 7369 746f 7279 2e0a 2320 4372 6561 7465  sitory..# Create
+000000a0: 6420 4279 3a20 4861 7261 6c64 204d 6f0a  d By: Harald Mo.
+000000b0: 2320 4372 6561 7465 6420 4461 7465 3a20  # Created Date: 
+000000c0: 3230 3233 2d30 322d 3133 0a0a 2320 5265  2023-02-13..# Re
+000000d0: 7669 7365 643a 204e 2f41 0a0a 2320 5465  vised: N/A..# Te
+000000e0: 7374 6564 3a20 2053 6565 2064 656d 6f73  sted:  See demos
+000000f0: 5c6f 6273 6572 7665 725c 656b 6433 646f  \observer\ekd3do
+00000100: 662e 7079 0a23 200a 2320 436f 7079 7269  f.py.# .# Copyri
+00000110: 6768 7420 2843 2920 3230 3233 3a20 4e54  ght (C) 2023: NT
+00000120: 4e55 2c20 5472 6f6e 6468 6569 6d0a 2320  NU, Trondheim.# 
+00000130: 4c69 6365 6e73 6564 2075 6e64 6572 2047  Licensed under G
+00000140: 504c 2d33 2e30 2d6f 722d 6c61 7465 720a  PL-3.0-or-later.
+00000150: 2320 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  # --------------
+00000160: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000170: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000180: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000190: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a23  -------------..#
+000001a0: 2049 6d70 6f72 7473 0a69 6d70 6f72 7420   Imports.import 
+000001b0: 6e75 6d70 7920 6173 206e 700a 6672 6f6d  numpy as np.from
+000001c0: 204d 4353 696d 5079 7468 6f6e 2e75 7469   MCSimPython.uti
+000001d0: 6c73 2069 6d70 6f72 7420 527a 2c20 7069  ls import Rz, pi
+000001e0: 7069 2c20 7369 7832 7468 7265 6544 4f46  pi, six2threeDOF
+000001f0: 0a0a 0a63 6c61 7373 2045 4b46 2829 3a0a  ...class EKF():.
+00000200: 2020 2020 2727 270a 2020 2020 496d 706c      '''.    Impl
+00000210: 656d 656e 7461 7469 6f6e 206f 6620 4578  ementation of Ex
+00000220: 7465 6e64 6564 204b 616c 6d61 6e20 4669  tended Kalman Fi
+00000230: 6c74 6572 2028 454b 4629 2066 6f72 2043  lter (EKF) for C
+00000240: 5341 442e 0a0a 2020 2020 785f 6861 7420  SAD...    x_hat 
+00000250: 3d20 5b0a 2020 2020 2020 2020 7a65 7461  = [.        zeta
+00000260: 2020 2020 2836 444f 4629 0a20 2020 2020      (6DOF).     
+00000270: 2020 2065 7461 2020 2020 2028 3344 4f46     eta     (3DOF
+00000280: 290a 2020 2020 2020 2020 6269 6173 2020  ).        bias  
+00000290: 2020 2833 444f 4629 0a20 2020 2020 2020    (3DOF).       
+000002a0: 206e 7520 2020 2020 2028 3344 4f46 290a   nu      (3DOF).
+000002b0: 2020 2020 5d0a 0a20 2020 2052 6566 6572      ]..    Refer
+000002c0: 656e 6365 3a0a 2020 2020 2020 2020 2d20  ence:.        - 
+000002d0: 466f 7373 656e 2028 3230 3231 292c 204d  Fossen (2021), M
+000002e0: 6172 696e 6520 6372 6166 7420 6879 6472  arine craft hydr
+000002f0: 6f64 796e 616d 6963 7320 616e 6420 6d6f  odynamics and mo
+00000300: 7469 6f6e 2063 6f6e 7472 6f6c 2c20 6368  tion control, ch
+00000310: 2031 332e 0a20 2020 2027 2727 0a20 2020   13..    '''.   
+00000320: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+00000330: 6c66 2c20 6474 2c20 4d2c 2044 2c20 5470  lf, dt, M, D, Tp
+00000340: 2c20 7830 3d6e 702e 7a65 726f 7328 3135  , x0=np.zeros(15
+00000350: 292c 2050 3020 3d20 6e70 2e7a 6572 6f73  ), P0 = np.zeros
+00000360: 2828 3135 2c31 3529 2929 3a0a 2020 2020  ((15,15))):.    
+00000370: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+00000380: 496e 6974 6961 6c69 7a61 7469 6f6e 3a0a  Initialization:.
+00000390: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+000003a0: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+000003b0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+000003c0: 2020 2020 2d20 6474 2028 666c 6f61 7429      - dt (float)
+000003d0: 3a20 5469 6d65 2073 7465 700a 2020 2020  : Time step.    
+000003e0: 2020 2020 2020 2020 2d20 4d20 286e 756d          - M (num
+000003f0: 7079 2061 7272 6179 2028 362c 2036 2929  py array (6, 6))
+00000400: 3a20 496e 6572 7469 6120 6d61 7472 6978  : Inertia matrix
+00000410: 206f 6620 7379 7374 656d 2028 696e 636c   of system (incl
+00000420: 7564 696e 6720 6164 6465 6420 6d61 7373  uding added mass
+00000430: 2920 3644 4f46 0a20 2020 2020 2020 2020  ) 6DOF.         
+00000440: 2020 202d 2044 2028 6e75 6d70 7920 6172     - D (numpy ar
+00000450: 7261 7920 2836 2c20 3629 293a 2046 756c  ray (6, 6)): Ful
+00000460: 6c20 6461 6d70 696e 6720 6d61 7472 6978  l damping matrix
+00000470: 206f 6620 7379 7374 656d 2036 444f 460a   of system 6DOF.
+00000480: 2020 2020 2020 2020 2020 2020 2d20 5470              - Tp
+00000490: 2028 696e 7429 3a20 5065 616b 2070 6572   (int): Peak per
+000004a0: 696f 6420 6f66 2077 6176 6520 7370 6563  iod of wave spec
+000004b0: 7472 650a 2020 2020 2020 2020 2727 270a  tre.        '''.
+000004c0: 2020 2020 2020 2020 7365 6c66 2e5f 6474          self._dt
+000004d0: 203d 2064 740a 0a20 2020 2020 2020 2023   = dt..        #
+000004e0: 2054 756e 696e 6720 2d20 446f 6e65 206d   Tuning - Done m
+000004f0: 616e 7561 6c6c 7920 2861 7320 6f66 206e  anually (as of n
+00000500: 6f77 290a 2020 2020 2020 2020 7365 6c66  ow).        self
+00000510: 2e5f 5164 203d 206e 702e 6172 7261 7928  ._Qd = np.array(
+00000520: 5b0a 2020 2020 2020 2020 2020 2020 5b31  [.            [1
+00000530: 652d 332c 302c 302c 302c 302c 305d 2c0a  e-3,0,0,0,0,0],.
+00000540: 2020 2020 2020 2020 2020 2020 5b30 2c31              [0,1
+00000550: 652d 332c 302c 302c 302c 305d 2c0a 2020  e-3,0,0,0,0],.  
+00000560: 2020 2020 2020 2020 2020 5b30 2c30 2c2e            [0,0,.
+00000570: 322a 6e70 2e70 692f 3138 302c 302c 302c  2*np.pi/180,0,0,
+00000580: 305d 2c0a 2020 2020 2020 2020 2020 2020  0],.            
+00000590: 5b30 2c30 2c30 2c31 6532 2c30 2c30 5d2c  [0,0,0,1e2,0,0],
+000005a0: 0a20 2020 2020 2020 2020 2020 205b 302c  .            [0,
+000005b0: 302c 302c 302c 3165 322c 305d 2c0a 2020  0,0,0,1e2,0],.  
+000005c0: 2020 2020 2020 2020 2020 5b30 2c30 2c30            [0,0,0
+000005d0: 2c30 2c30 2c31 6531 5d0a 2020 2020 2020  ,0,0,1e1].      
+000005e0: 2020 5d29 0a20 2020 200a 2020 2020 2020    ]).    .      
+000005f0: 2020 7365 6c66 2e5f 5264 203d 206e 702e    self._Rd = np.
+00000600: 6172 7261 7928 5b0a 2020 2020 2020 2020  array([.        
+00000610: 2020 2020 5b31 3030 2c30 2c30 5d2c 0a20      [100,0,0],. 
+00000620: 2020 2020 2020 2020 2020 205b 302c 3130             [0,10
+00000630: 302c 305d 2c0a 2020 2020 2020 2020 2020  0,0],.          
+00000640: 2020 5b30 2c30 2c35 3030 2a6e 702e 7069    [0,0,500*np.pi
+00000650: 2f31 3830 5d0a 2020 2020 2020 2020 5d29  /180].        ])
+00000660: 0a20 2020 2020 2020 2023 7365 6c66 2e5f  .        #self._
+00000670: 5164 203d 206e 702e 6469 6167 285b 342e  Qd = np.diag([4.
+00000680: 3537 3636 3634 3533 652d 3034 2c20 362e  57666453e-04, 6.
+00000690: 3534 3432 3438 3338 652d 3034 2c20 302e  54424838e-04, 0.
+000006a0: 3030 3030 3030 3030 652b 3030 2c20 302e  00000000e+00, 0.
+000006b0: 3030 3030 3030 3030 652b 3030 2c20 302e  00000000e+00, 0.
+000006c0: 3030 3030 3030 3030 652b 3030 2c20 372e  00000000e+00, 7.
+000006d0: 3335 3334 3931 3336 652d 3031 5d29 0a20  35349136e-01]). 
+000006e0: 2020 2020 2020 2023 7365 6c66 2e5f 5264         #self._Rd
+000006f0: 203d 206e 702e 6579 6528 3329 0a0a 2020   = np.eye(3)..  
+00000700: 2020 2020 2020 2320 436f 6e73 7461 6e74        # Constant
+00000710: 206d 6174 7269 6365 730a 2020 2020 2020   matrices.      
+00000720: 2020 4d20 3d20 7369 7832 7468 7265 6544    M = six2threeD
+00000730: 4f46 284d 290a 2020 2020 2020 2020 7365  OF(M).        se
+00000740: 6c66 2e5f 4d69 6e76 203d 206e 702e 6c69  lf._Minv = np.li
+00000750: 6e61 6c67 2e69 6e76 284d 2920 2020 2020  nalg.inv(M)     
+00000760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000780: 2020 2320 3344 4f46 2069 6e76 6572 7465    # 3DOF inverte
+00000790: 6420 6d61 7373 206d 6174 7269 780a 2020  d mass matrix.  
+000007a0: 2020 2020 2020 7365 6c66 2e5f 4420 3d20        self._D = 
+000007b0: 7369 7832 7468 7265 6544 4f46 2844 2920  six2threeDOF(D) 
+000007c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007e0: 2020 2020 2020 2020 2020 2320 3344 4f46            # 3DOF
+000007f0: 2064 616d 7069 6e67 206d 6174 7269 780a   damping matrix.
+00000800: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00000810: 2073 656c 662e 5f48 2c20 7365 6c66 2e5f   self._H, self._
+00000820: 422c 2073 656c 662e 5f45 2c20 7365 6c66  B, self._E, self
+00000830: 2e5f 4177 2c20 7365 6c66 2e5f 6761 6d6d  ._Aw, self._gamm
+00000840: 6120 3d20 302c 302c 302c 302c 300a 2020  a = 0,0,0,0,0.  
+00000850: 2020 2020 2020 7365 6c66 2e69 6e69 7469        self.initi
+00000860: 616c 697a 655f 636f 6e73 7461 6e74 5f6d  alize_constant_m
+00000870: 6174 7269 6365 7328 5470 290a 2020 2020  atrices(Tp).    
+00000880: 2020 2020 0a20 2020 2020 2020 200a 2020      .        .  
+00000890: 2020 2020 2020 2320 496e 6974 6961 6c20        # Initial 
+000008a0: 7661 6c75 6573 0a20 2020 2020 2020 2073  values.        s
+000008b0: 656c 662e 5f78 6861 7420 3d20 6e70 2e7a  elf._xhat = np.z
+000008c0: 6572 6f73 2831 3529 0a20 2020 2020 2020  eros(15).       
+000008d0: 2073 656c 662e 5f78 6261 7220 3d20 7830   self._xbar = x0
+000008e0: 0a0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+000008f0: 5062 6172 203d 2050 300a 2020 2020 2020  Pbar = P0.      
+00000900: 2020 7365 6c66 2e5f 5068 6174 203d 206e    self._Phat = n
+00000910: 702e 7a65 726f 7328 2831 352c 3135 2929  p.zeros((15,15))
+00000920: 0a20 2020 200a 2020 2020 0a20 2020 2020  .    .    .     
+00000930: 200a 2020 2020 6465 6620 7570 6461 7465   .    def update
+00000940: 2873 656c 662c 2074 6175 2c20 7929 3a0a  (self, tau, y):.
+00000950: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
+00000960: 2020 2020 5570 6461 7465 3a0a 2020 2020      Update:.    
+00000970: 2020 2020 5570 6461 7465 2066 756e 6374      Update funct
+00000980: 696f 6e20 746f 2062 6520 6361 6c6c 6564  ion to be called
+00000990: 2061 7420 6576 6572 7920 7469 6d65 7374   at every timest
+000009a0: 6570 2064 7572 696e 6720 6120 7369 6d75  ep during a simu
+000009b0: 6c61 7469 6f6e 2e20 4361 6c6c 7320 7468  lation. Calls th
+000009c0: 6520 7072 6564 6963 746f 7220 616e 6420  e predictor and 
+000009d0: 636f 7272 6563 746f 722e 0a0a 2020 2020  corrector...    
+000009e0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+000009f0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+00000a00: 2d0a 2020 2020 2020 2020 2020 2020 2d20  -.            - 
+00000a10: 7461 753a 2043 6f6e 7472 6f6c 2050 6172  tau: Control Par
+00000a20: 616d 6574 6572 7320 2833 444f 4629 0a20  ameters (3DOF). 
+00000a30: 2020 2020 2020 2020 2020 202d 2079 3a20             - y: 
+00000a40: 4d65 6173 7572 6564 2070 6f73 6974 696f  Measured positio
+00000a50: 6e20 2833 444f 4629 0a0a 2020 2020 2020  n (3DOF)..      
+00000a60: 2020 546f 2062 6520 696d 706c 656d 656e    To be implemen
+00000a70: 7465 6420 2f20 496d 7072 6f76 656d 656e  ted / Improvemen
+00000a80: 7473 0a20 2020 2020 2020 202d 2d2d 2d2d  ts.        -----
+00000a90: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2020  ------.         
+00000aa0: 2020 202d 2045 7272 6f72 2063 6865 636b     - Error check
+00000ab0: 733f 0a20 2020 2020 2020 2020 2020 202d  s?.            -
+00000ac0: 2041 7379 6e63 6872 6f6e 6f75 7320 6d65   Asynchronous me
+00000ad0: 6173 7572 656d 656e 7473 3f0a 2020 2020  asurements?.    
+00000ae0: 2020 2020 2020 2020 2d20 5365 7420 7920          - Set y 
+00000af0: 746f 206e 616e 2069 6620 6e6f 206d 6561  to nan if no mea
+00000b00: 7375 7265 6d65 6e74 0a20 2020 2020 2020  surement.       
+00000b10: 2027 2727 0a20 2020 2020 2020 2023 2043   '''.        # C
+00000b20: 6f72 7265 6374 0a20 2020 2020 2020 2073  orrect.        s
+00000b30: 656c 662e 636f 7272 6563 746f 7228 7929  elf.corrector(y)
+00000b40: 0a20 2020 2020 2020 2023 2050 7265 6469  .        # Predi
+00000b50: 6374 2020 2020 2020 2020 0a20 2020 2020  ct        .     
+00000b60: 2020 2073 656c 662e 7072 6564 6963 746f     self.predicto
+00000b70: 7228 7461 7529 0a20 2020 2020 2020 200a  r(tau).        .
+00000b80: 0a20 2020 200a 2020 2020 6465 6620 7072  .    .    def pr
+00000b90: 6564 6963 746f 7228 7365 6c66 2c20 7461  edictor(self, ta
+00000ba0: 7529 3a0a 2020 2020 2020 2020 2727 270a  u):.        '''.
+00000bb0: 2020 2020 2020 2020 5072 6564 6963 746f          Predicto
+00000bc0: 723a 0a20 2020 2020 2020 2055 7365 6420  r:.        Used 
+00000bd0: 746f 2065 7374 696d 6174 6520 7468 6520  to estimate the 
+00000be0: 7374 6174 6520 6f66 2074 6865 2073 7973  state of the sys
+00000bf0: 7465 6d20 6174 2074 6865 206e 6578 7420  tem at the next 
+00000c00: 7469 6d65 2073 7465 7020 6261 7365 6420  time step based 
+00000c10: 6f6e 2074 6865 2063 7572 7265 6e74 2073  on the current s
+00000c20: 7461 7465 2065 7374 696d 6174 6520 616e  tate estimate an
+00000c30: 6420 7468 6520 7379 7374 656d 2064 796e  d the system dyn
+00000c40: 616d 6963 7320 6d6f 6465 6c2e 0a20 2020  amics model..   
+00000c50: 2020 2020 200a 2020 2020 2020 2020 5061       .        Pa
+00000c60: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+00000c70: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+00000c80: 2020 2020 2020 2020 2d20 7461 7520 3d20          - tau = 
+00000c90: 5b58 2c20 592c 204e 5d27 2c20 2043 6f6e  [X, Y, N]',  Con
+00000ca0: 7472 6f6c 2069 6e70 7574 2028 3344 4f46  trol input (3DOF
+00000cb0: 290a 2020 2020 2020 2020 2020 2020 200a  ).             .
+00000cc0: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
+00000cd0: 2020 2020 7068 6920 3d20 7365 6c66 2e73      phi = self.s
+00000ce0: 7461 7465 5f66 756e 6374 696f 6e5f 6a61  tate_function_ja
+00000cf0: 636f 6269 616e 2829 0a20 2020 2020 2020  cobian().       
+00000d00: 2066 203d 2073 656c 662e 7374 6174 655f   f = self.state_
+00000d10: 6675 6e63 7469 6f6e 2873 656c 662e 5f78  function(self._x
+00000d20: 6861 742c 2074 6175 2c20 6e70 2e7a 6572  hat, tau, np.zer
+00000d30: 6f73 2836 2929 0a0a 2020 2020 2020 2020  os(6))..        
+00000d40: 7365 6c66 2e5f 5062 6172 203d 2070 6869  self._Pbar = phi
+00000d50: 4073 656c 662e 5f50 6861 7440 2870 6869  @self._Phat@(phi
+00000d60: 2e54 2920 2b20 7365 6c66 2e5f 6761 6d6d  .T) + self._gamm
+00000d70: 6140 7365 6c66 2e5f 5164 4028 7365 6c66  a@self._Qd@(self
+00000d80: 2e5f 6761 6d6d 612e 5429 0a20 2020 2020  ._gamma.T).     
+00000d90: 2020 2073 656c 662e 5f78 6261 7220 3d20     self._xbar = 
+00000da0: 7365 6c66 2e5f 7868 6174 202b 2073 656c  self._xhat + sel
+00000db0: 662e 5f64 7420 2a20 660a 0a0a 2020 2020  f._dt * f...    
+00000dc0: 6465 6620 636f 7272 6563 746f 7228 7365  def corrector(se
+00000dd0: 6c66 2c20 7929 3a0a 2020 2020 2020 2020  lf, y):.        
+00000de0: 2727 270a 2020 2020 2020 2020 436f 7272  '''.        Corr
+00000df0: 6563 746f 723a 0a20 2020 2020 2020 2055  ector:.        U
+00000e00: 7365 6420 746f 2072 6566 696e 6520 7468  sed to refine th
+00000e10: 6520 7072 6564 6963 7465 6420 7374 6174  e predicted stat
+00000e20: 6520 6573 7469 6d61 7465 2066 726f 6d20  e estimate from 
+00000e30: 7468 6520 7072 6564 6963 746f 722c 2062  the predictor, b
+00000e40: 6173 6564 206f 6e20 7468 6520 6f62 7461  ased on the obta
+00000e50: 696e 6564 206d 6561 7375 7265 6d65 6e74  ined measurement
+00000e60: 732e 2054 6865 2066 756e 6374 696f 6e20  s. The function 
+00000e70: 6368 6563 6b73 2066 6f72 2073 6967 6e61  checks for signa
+00000e80: 6c20 6c6f 7373 2028 6e6f 206d 6561 7375  l loss (no measu
+00000e90: 7265 6d65 6e74 292e 0a0a 2020 2020 2020  rement)...      
+00000ea0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+00000eb0: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d       -----------
+00000ec0: 0a20 2020 2020 2020 2020 2020 202d 2079  .            - y
+00000ed0: 203d 205b 6574 6131 2020 6574 6132 2020   = [eta1  eta2  
+00000ee0: 6574 6136 5d27 2c20 4d65 6173 7572 656d  eta6]', Measurem
+00000ef0: 656e 7473 2028 3344 4f46 2920 0a0a 2020  ents (3DOF) ..  
+00000f00: 2020 2020 2020 546f 2062 6520 696d 706c        To be impl
+00000f10: 656d 656e 7465 6420 2f20 496d 7072 6f76  emented / Improv
+00000f20: 656d 656e 7473 0a20 2020 2020 2020 202d  ements.        -
+00000f30: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+00000f40: 2020 2020 2020 2d20 4368 6563 6b20 6966        - Check if
+00000f50: 206d 6561 7375 7265 6d65 6e74 2069 7320   measurement is 
+00000f60: 6769 7665 6e2e 2043 616e 2061 6c73 6f20  given. Can also 
+00000f70: 6265 206d 6164 6520 7769 7468 206d 6f64  be made with mod
+00000f80: 756c 7573 206f 7065 7261 746f 7220 6966  ulus operator if
+00000f90: 206d 6561 7375 7265 6d65 6e74 2066 7265   measurement fre
+00000fa0: 7120 6973 2064 6966 6665 7265 6e74 2066  q is different f
+00000fb0: 726f 6d20 6474 2e0a 2020 2020 2020 2020  rom dt..        
+00000fc0: 2020 2020 2d20 0a20 2020 2020 2020 2027      - .        '
+00000fd0: 2727 0a0a 2020 2020 2020 2020 6966 206e  ''..        if n
+00000fe0: 702e 616e 7928 6e70 2e69 736e 616e 2879  p.any(np.isnan(y
+00000ff0: 2929 203d 3d20 5472 7565 3a20 2020 2023  )) == True:    #
+00001000: 2049 6620 6e6f 206e 6577 206d 6561 7375   If no new measu
+00001010: 7265 6d65 6e74 733a 2053 6574 2063 6f72  rements: Set cor
+00001020: 7265 6374 6f72 2065 7175 616c 2074 6f20  rector equal to 
+00001030: 7072 6564 6963 746f 7220 2844 6561 6420  predictor (Dead 
+00001040: 7265 636b 6f6e 696e 6729 0a20 2020 2020  reckoning).     
+00001050: 2020 2020 2020 2073 656c 662e 5f50 6861         self._Pha
+00001060: 7420 3d20 7365 6c66 2e5f 5062 6172 0a20  t = self._Pbar. 
+00001070: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00001080: 5f78 6861 7420 3d20 7365 6c66 2e5f 7862  _xhat = self._xb
+00001090: 6172 0a20 2020 2020 2020 2065 6c73 653a  ar.        else:
+000010a0: 0a20 2020 2020 2020 2020 2020 204b 203d  .            K =
+000010b0: 2073 656c 662e 454b 465f 6761 696e 0a0a   self.EKF_gain..
+000010c0: 2020 2020 2020 2020 2020 2020 7061 7265              pare
+000010d0: 6e74 6865 7369 7320 3d20 6e70 2e65 7965  nthesis = np.eye
+000010e0: 2831 3529 202d 204b 4073 656c 662e 5f48  (15) - K@self._H
+000010f0: 0a0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+00001100: 6564 6963 7469 6f6e 5f65 7272 6f72 203d  ediction_error =
+00001110: 2079 202d 2028 7365 6c66 2e5f 4840 7365   y - (self._H@se
+00001120: 6c66 2e5f 7862 6172 290a 2020 2020 2020  lf._xbar).      
+00001130: 2020 2020 2020 7072 6564 6963 7469 6f6e        prediction
+00001140: 5f65 7272 6f72 5b32 5d20 3d20 7069 7069  _error[2] = pipi
+00001150: 2870 7265 6469 6374 696f 6e5f 6572 726f  (prediction_erro
+00001160: 725b 325d 2920 2020 2320 536d 616c 6c65  r[2])   # Smalle
+00001170: 7374 2073 6967 6e65 6420 616e 676c 6520  st signed angle 
+00001180: 6d6f 6469 6669 6361 7469 6f6e 0a0a 2020  modification..  
+00001190: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+000011a0: 5068 6174 203d 2070 6172 656e 7468 6573  Phat = parenthes
+000011b0: 6973 4073 656c 662e 5f50 6261 7240 2870  is@self._Pbar@(p
+000011c0: 6172 656e 7468 6573 6973 2e54 2920 2b20  arenthesis.T) + 
+000011d0: 4b40 7365 6c66 2e5f 5264 4028 4b2e 5429  K@self._Rd@(K.T)
+000011e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000011f0: 662e 5f78 6861 7420 3d20 7365 6c66 2e5f  f._xhat = self._
+00001200: 7862 6172 202b 204b 4070 7265 6469 6374  xbar + K@predict
+00001210: 696f 6e5f 6572 726f 720a 2020 2020 2020  ion_error.      
+00001220: 2020 0a0a 2020 2020 4070 726f 7065 7274    ..    @propert
+00001230: 790a 2020 2020 6465 6620 454b 465f 6761  y.    def EKF_ga
+00001240: 696e 2873 656c 6629 3a0a 2020 2020 2020  in(self):.      
+00001250: 2020 2727 270a 2020 2020 2020 2020 4b61    '''.        Ka
+00001260: 6c6d 616e 2067 6169 6e3a 0a20 2020 2020  lman gain:.     
+00001270: 2020 2055 7365 6420 746f 2062 616c 616e     Used to balan
+00001280: 6365 2074 6865 2063 6f6e 7472 6962 7574  ce the contribut
+00001290: 696f 6e73 206f 6620 7468 6520 7072 6564  ions of the pred
+000012a0: 6963 7465 6420 7374 6174 6520 6573 7469  icted state esti
+000012b0: 6d61 7465 2061 6e64 2074 6865 206d 6561  mate and the mea
+000012c0: 7375 7265 6d65 6e74 2064 6174 6120 696e  surement data in
+000012d0: 2074 6865 2075 7064 6174 6564 2065 7374   the updated est
+000012e0: 696d 6174 652e 0a0a 2020 2020 2020 2020  imate...        
+000012f0: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+00001300: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20     -----------. 
+00001310: 2020 2020 2020 2020 2020 202d 204e 2f41             - N/A
+00001320: 0a0a 2020 2020 2020 2020 4f75 7470 7574  ..        Output
+00001330: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00001340: 2d2d 2d2d 0a20 2020 2020 2020 2020 2020  ----.           
+00001350: 202d 204b 3a20 4b61 6c6d 616e 2067 6169   - K: Kalman gai
+00001360: 6e20 2844 696d 203d 2031 3578 3329 0a20  n (Dim = 15x3). 
+00001370: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+00001380: 2020 2070 6172 656e 7468 6573 6973 203d     parenthesis =
+00001390: 2073 656c 662e 5f48 4073 656c 662e 5f50   self._H@self._P
+000013a0: 6261 7240 2873 656c 662e 5f48 2e54 2920  bar@(self._H.T) 
+000013b0: 2b20 7365 6c66 2e5f 5264 0a20 2020 2020  + self._Rd.     
+000013c0: 2020 204b 203d 2073 656c 662e 5f50 6261     K = self._Pba
+000013d0: 7240 2873 656c 662e 5f48 2e54 2940 6e70  r@(self._H.T)@np
+000013e0: 2e6c 696e 616c 672e 696e 7628 7061 7265  .linalg.inv(pare
+000013f0: 6e74 6865 7369 7329 0a20 2020 2020 2020  nthesis).       
+00001400: 2072 6574 7572 6e20 4b0a 0a0a 2020 2020   return K...    
+00001410: 6465 6620 7374 6174 655f 6675 6e63 7469  def state_functi
+00001420: 6f6e 2873 656c 662c 2078 2c20 7461 752c  on(self, x, tau,
+00001430: 206e 6f69 7365 203d 206e 702e 7a65 726f   noise = np.zero
+00001440: 7328 3629 293a 2020 2020 2020 2020 2020  s(6)):          
+00001450: 2020 2020 2020 2020 2020 2320 6628 782c            # f(x,
+00001460: 752c 7729 0a20 2020 2020 2020 2027 2727  u,w).        '''
+00001470: 0a20 2020 2020 2020 2078 5f64 6f74 203d  .        x_dot =
+00001480: 2041 2878 2920 2b20 422a 7461 7520 2b20   A(x) + B*tau + 
+00001490: 452a 7720 2020 2020 203d 2066 2878 2c75  E*w      = f(x,u
+000014a0: 2c77 290a 0a20 2020 2020 2020 2077 6865  ,w)..        whe
+000014b0: 7265 2041 2878 2920 3d20 5b0a 2020 2020  re A(x) = [.    
+000014c0: 2020 2020 2020 2020 4177 202a 2078 690a          Aw * xi.
+000014d0: 2020 2020 2020 2020 2020 2020 5228 7073              R(ps
+000014e0: 6929 202a 206e 750a 2020 2020 2020 2020  i) * nu.        
+000014f0: 2020 2020 305f 2833 7831 290a 2020 2020      0_(3x1).    
+00001500: 2020 2020 2020 2020 2d4d 5f69 6e76 2a44          -M_inv*D
+00001510: 202a 206e 7520 2b20 4d5f 696e 762a 5228   * nu + M_inv*R(
+00001520: 7073 6929 2e54 202a 2062 0a20 2020 2020  psi).T * b.     
+00001530: 2020 205d 0a0a 2020 2020 2020 2020 5061     ]..        Pa
+00001540: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+00001550: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+00001560: 2020 2020 2020 2020 2d20 783a 2073 7461          - x: sta
+00001570: 7465 2076 6563 746f 7220 2844 696d 203d  te vector (Dim =
+00001580: 2031 3529 0a20 2020 2020 2020 2020 2020   15).           
+00001590: 202d 2074 6175 3a20 436f 6e74 726f 6c20   - tau: Control 
+000015a0: 7665 6374 6f72 205b 5820 2059 2020 4e5d  vector [X  Y  N]
+000015b0: 0a20 2020 2020 2020 2020 2020 202d 206e  .            - n
+000015c0: 6f69 7365 3a20 4d6f 6465 6c6c 6564 2077  oise: Modelled w
+000015d0: 6869 7465 206e 6f69 7365 2c20 7365 7420  hite noise, set 
+000015e0: 746f 207a 6572 6f20 696e 2061 2064 6574  to zero in a det
+000015f0: 6572 6d69 6e69 7374 6963 2045 4b46 2e20  erministic EKF. 
+00001600: 2844 696d 3d36 290a 0a20 2020 2020 2020  (Dim=6)..       
+00001610: 204f 7574 7075 740a 2020 2020 2020 2020   Output.        
+00001620: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+00001630: 2020 2020 2020 202d 2066 3a20 785f 646f         - f: x_do
+00001640: 7420 2844 696d 203d 2031 3529 0a20 2020  t (Dim = 15).   
+00001650: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+00001660: 2078 6920 3d20 785b 303a 365d 0a20 2020   xi = x[0:6].   
+00001670: 2020 2020 2065 7461 203d 2078 5b36 3a39       eta = x[6:9
+00001680: 5d0a 2020 2020 2020 2020 7073 6920 3d20  ].        psi = 
+00001690: 6574 615b 325d 0a20 2020 2020 2020 2062  eta[2].        b
+000016a0: 203d 2078 5b39 3a31 325d 0a20 2020 2020   = x[9:12].     
+000016b0: 2020 206e 7520 3d20 785b 3132 3a31 355d     nu = x[12:15]
+000016c0: 0a0a 2020 2020 2020 2020 4178 203d 206e  ..        Ax = n
+000016d0: 702e 6172 7261 7928 0a20 2020 2020 2020  p.array(.       
+000016e0: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
+000016f0: 2020 2028 7365 6c66 2e5f 4177 4078 6929     (self._Aw@xi)
+00001700: 2c0a 2020 2020 2020 2020 2020 2020 2852  ,.            (R
+00001710: 7a28 7073 6929 406e 7529 2c0a 2020 2020  z(psi)@nu),.    
+00001720: 2020 2020 2020 2020 6e70 2e7a 6572 6f73          np.zeros
+00001730: 2833 292c 0a20 2020 2020 2020 2020 2020  (3),.           
+00001740: 2028 2d73 656c 662e 5f4d 696e 7640 7365   (-self._Minv@se
+00001750: 6c66 2e5f 4440 6e75 202b 2073 656c 662e  lf._D@nu + self.
+00001760: 5f4d 696e 7640 2852 7a28 7073 6929 2e54  _Minv@(Rz(psi).T
+00001770: 2940 6229 2020 2020 2023 2070 6c75 7320  )@b)     # plus 
+00001780: 6f72 206d 696e 7573 2069 6e20 326e 6420  or minus in 2nd 
+00001790: 7465 726d 3f0a 2020 2020 2020 2020 2020  term?.          
+000017a0: 2020 5d2c 2064 7479 7065 3d6f 626a 6563    ], dtype=objec
+000017b0: 740a 2020 2020 2020 2020 290a 0a20 2020  t.        )..   
+000017c0: 2020 2020 2041 7820 3d20 6e70 2e63 6f6e       Ax = np.con
+000017d0: 6361 7465 6e61 7465 2841 7829 2020 2020  catenate(Ax)    
+000017e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001800: 2023 2043 6f6e 7665 7274 2074 6f20 3135   # Convert to 15
+00001810: 7831 0a0a 2020 2020 2020 2020 6620 3d20  x1..        f = 
+00001820: 4178 202b 2073 656c 662e 5f42 4074 6175  Ax + self._B@tau
+00001830: 202b 2073 656c 662e 5f45 406e 6f69 7365   + self._E@noise
+00001840: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00001850: 660a 0a0a 2020 2020 6465 6620 7374 6174  f...    def stat
+00001860: 655f 6675 6e63 7469 6f6e 5f6a 6163 6f62  e_function_jacob
+00001870: 6961 6e28 7365 6c66 293a 2020 2020 2020  ian(self):      
+00001880: 2023 2064 662f 6478 0a20 2020 2020 2020   # df/dx.       
+00001890: 2027 2727 0a20 2020 2020 2020 2070 6869   '''.        phi
+000018a0: 203d 2065 7965 2831 3529 202b 2064 7420   = eye(15) + dt 
+000018b0: 2a20 6465 6c28 6629 2f64 656c 2878 290a  * del(f)/del(x).
+000018c0: 0a20 2020 2020 2020 2077 6865 7265 0a0a  .        where..
+000018d0: 2020 2020 2020 2020 6465 6c28 6629 2f64          del(f)/d
+000018e0: 656c 2878 2920 3d20 5b0a 2020 2020 2020  el(x) = [.      
+000018f0: 2020 2020 2020 726f 7720 2831 293a 2020        row (1):  
+00001900: 2020 2020 2020 415f 7720 2020 2020 2020        A_w       
+00001910: 2020 305f 2836 7833 2920 2020 2020 305f    0_(6x3)     0_
+00001920: 2836 7833 2920 2020 2020 2020 2020 305f  (6x3)         0_
+00001930: 2836 7833 2920 2020 2020 2020 2020 2020  (6x3)           
+00001940: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
+00001950: 2020 2072 6f77 2028 3229 3a20 2020 2020     row (2):     
+00001960: 2020 2030 5f28 3378 3629 2020 2020 2064     0_(3x6)     d
+00001970: 656c 5f66 3220 2020 2020 2030 5f28 3378  el_f2      0_(3x
+00001980: 3329 2020 2020 2020 2020 2052 2870 7369  3)         R(psi
+00001990: 2920 2020 2020 2020 2020 2020 2020 2020  )               
+000019a0: 2020 200a 2020 2020 2020 2020 2020 2020     .            
+000019b0: 726f 7720 2833 293a 2020 2020 2020 2020  row (3):        
+000019c0: 305f 2833 7836 2920 2020 2020 305f 2833  0_(3x6)     0_(3
+000019d0: 7833 2920 2020 2020 305f 2833 7833 2920  x3)     0_(3x3) 
+000019e0: 2020 2020 2020 2020 305f 2833 7833 2920          0_(3x3) 
+000019f0: 2020 2020 2020 2020 2020 2020 2020 200a                 .
+00001a00: 2020 2020 2020 2020 2020 2020 726f 7720              row 
+00001a10: 2834 293a 2020 2020 2020 2020 305f 2833  (4):        0_(3
+00001a20: 7836 2920 2020 2020 6465 6c5f 6634 2020  x6)     del_f4  
+00001a30: 2020 2020 4d5f 696e 762a 5228 7073 6929      M_inv*R(psi)
+00001a40: 2e54 2020 2d4d 5f69 6e76 2a44 2020 2020  .T  -M_inv*D    
+00001a50: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
+00001a60: 2020 2020 205d 2020 200a 0a20 2020 2020       ]   ..     
+00001a70: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+00001a80: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+00001a90: 0a20 2020 2020 2020 2020 2020 202d 204e  .            - N
+00001aa0: 2f41 0a0a 2020 2020 2020 2020 4f75 7470  /A..        Outp
+00001ab0: 7574 0a20 2020 2020 2020 202d 2d2d 2d2d  ut.        -----
+00001ac0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2020  ------.         
+00001ad0: 2020 202d 2070 6869 3a20 4469 7363 7265     - phi: Discre
+00001ae0: 7469 7a65 6420 6a61 636f 6269 616e 206f  tized jacobian o
+00001af0: 6620 7379 7374 656d 2064 796e 616d 6963  f system dynamic
+00001b00: 7320 2844 696d 203d 2031 3578 3135 290a  s (Dim = 15x15).
+00001b10: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
+00001b20: 2020 2020 2023 2045 7874 7261 6374 2073       # Extract s
+00001b30: 7461 7465 730a 2020 2020 2020 2020 7073  tates.        ps
+00001b40: 6920 3d20 7365 6c66 2e5f 7868 6174 5b38  i = self._xhat[8
+00001b50: 5d0a 2020 2020 2020 2020 6231 203d 2073  ].        b1 = s
+00001b60: 656c 662e 5f78 6861 745b 395d 0a20 2020  elf._xhat[9].   
+00001b70: 2020 2020 2062 3220 3d20 7365 6c66 2e5f       b2 = self._
+00001b80: 7868 6174 5b31 305d 0a20 2020 2020 2020  xhat[10].       
+00001b90: 2075 203d 2073 656c 662e 5f78 6861 745b   u = self._xhat[
+00001ba0: 3132 5d0a 2020 2020 2020 2020 7620 3d20  12].        v = 
+00001bb0: 7365 6c66 2e5f 7868 6174 5b31 335d 0a0a  self._xhat[13]..
+00001bc0: 2020 2020 2020 2020 6465 6c5f 6632 203d          del_f2 =
+00001bd0: 206e 702e 6172 7261 7928 5b0a 2020 2020   np.array([.    
+00001be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001bf0: 2020 2020 2020 2020 5b30 2c30 2c2d 752a          [0,0,-u*
+00001c00: 6e70 2e73 696e 2870 7369 292d 762a 6e70  np.sin(psi)-v*np
+00001c10: 2e63 6f73 2870 7369 295d 2c0a 2020 2020  .cos(psi)],.    
+00001c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c30: 2020 2020 2020 2020 5b30 2c30 2c75 2a6e          [0,0,u*n
+00001c40: 702e 636f 7328 7073 6929 2d76 2a6e 702e  p.cos(psi)-v*np.
+00001c50: 7369 6e28 7073 6929 5d2c 0a20 2020 2020  sin(psi)],.     
+00001c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c70: 2020 2020 2020 205b 302c 302c 305d 0a20         [0,0,0]. 
+00001c80: 2020 2020 2020 205d 290a 2020 2020 2020         ]).      
+00001c90: 2020 6465 6c5f 6634 203d 206e 702e 6172    del_f4 = np.ar
+00001ca0: 7261 7928 5b0a 2020 2020 2020 2020 2020  ray([.          
+00001cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001cc0: 2020 5b30 2c30 2c73 656c 662e 5f4d 696e    [0,0,self._Min
+00001cd0: 765b 302c 305d 2a28 6232 2a6e 702e 636f  v[0,0]*(b2*np.co
+00001ce0: 7328 7073 6929 202d 2062 312a 6e70 2e73  s(psi) - b1*np.s
+00001cf0: 696e 2870 7369 2929 5d2c 0a20 2020 2020  in(psi))],.     
 00001d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d10: 2020 5b30 2c30 2c75 2a6e 702e 636f 7328    [0,0,u*np.cos(
-00001d20: 7073 6929 2d76 2a6e 702e 7369 6e28 7073  psi)-v*np.sin(ps
-00001d30: 6929 5d2c 0d0a 2020 2020 2020 2020 2020  i)],..          
-00001d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d50: 2020 5b30 2c30 2c30 5d0d 0a20 2020 2020    [0,0,0]..     
-00001d60: 2020 205d 290d 0a20 2020 2020 2020 2064     ])..        d
-00001d70: 656c 5f66 3420 3d20 6e70 2e61 7272 6179  el_f4 = np.array
-00001d80: 285b 0d0a 2020 2020 2020 2020 2020 2020  ([..            
-00001d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001da0: 5b30 2c30 2c73 656c 662e 5f4d 696e 765b  [0,0,self._Minv[
-00001db0: 302c 305d 2a28 6232 2a6e 702e 636f 7328  0,0]*(b2*np.cos(
-00001dc0: 7073 6929 202d 2062 312a 6e70 2e73 696e  psi) - b1*np.sin
-00001dd0: 2870 7369 2929 5d2c 0d0a 2020 2020 2020  (psi))],..      
-00001de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001df0: 2020 2020 2020 5b30 2c30 2c2d 7365 6c66        [0,0,-self
-00001e00: 2e5f 4d69 6e76 5b31 2c31 5d2a 2862 312a  ._Minv[1,1]*(b1*
-00001e10: 6e70 2e63 6f73 2870 7369 2920 2b20 6232  np.cos(psi) + b2
-00001e20: 2a6e 702e 7369 6e28 7073 6929 295d 2c0d  *np.sin(psi))],.
-00001e30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001e40: 2020 2020 2020 2020 2020 2020 205b 302c               [0,
-00001e50: 302c 2d73 656c 662e 5f4d 696e 765b 322c  0,-self._Minv[2,
-00001e60: 315d 2a28 6231 2a6e 702e 636f 7328 7073  1]*(b1*np.cos(ps
-00001e70: 6929 202b 2062 322a 6e70 2e73 696e 2870  i) + b2*np.sin(p
-00001e80: 7369 2929 5d0d 0a20 2020 2020 2020 205d  si))]..        ]
-00001e90: 290d 0a0d 0a20 2020 2020 2020 2072 6f77  )....        row
-00001ea0: 3120 3d20 6e70 2e63 6f6e 6361 7465 6e61  1 = np.concatena
-00001eb0: 7465 2828 7365 6c66 2e5f 4177 2c20 6e70  te((self._Aw, np
-00001ec0: 2e7a 6572 6f73 2828 362c 3929 2929 2c20  .zeros((6,9))), 
-00001ed0: 6178 6973 3d31 290d 0a20 2020 2020 2020  axis=1)..       
-00001ee0: 2072 6f77 3220 3d20 6e70 2e63 6f6e 6361   row2 = np.conca
-00001ef0: 7465 6e61 7465 2828 6e70 2e7a 6572 6f73  tenate((np.zeros
-00001f00: 2828 332c 3629 292c 2064 656c 5f66 322c  ((3,6)), del_f2,
-00001f10: 206e 702e 7a65 726f 7328 2833 2c33 2929   np.zeros((3,3))
-00001f20: 2c20 527a 2870 7369 2929 2c20 6178 6973  , Rz(psi)), axis
-00001f30: 3d31 290d 0a20 2020 2020 2020 2072 6f77  =1)..        row
-00001f40: 3320 3d20 6e70 2e7a 6572 6f73 2828 332c  3 = np.zeros((3,
-00001f50: 3135 2929 0d0a 2020 2020 2020 2020 726f  15))..        ro
-00001f60: 7734 203d 206e 702e 636f 6e63 6174 656e  w4 = np.concaten
-00001f70: 6174 6528 286e 702e 7a65 726f 7328 2833  ate((np.zeros((3
-00001f80: 2c36 2929 2c20 6465 6c5f 6634 2c20 7365  ,6)), del_f4, se
-00001f90: 6c66 2e5f 4d69 6e76 4028 527a 2870 7369  lf._Minv@(Rz(psi
-00001fa0: 292e 5429 2c20 2d73 656c 662e 5f4d 696e  ).T), -self._Min
-00001fb0: 7640 7365 6c66 2e5f 4429 2c20 6178 6973  v@self._D), axis
-00001fc0: 3d31 290d 0a0d 0a20 2020 2020 2020 2070  =1)....        p
-00001fd0: 6869 203d 206e 702e 6579 6528 3135 2920  hi = np.eye(15) 
-00001fe0: 2b20 7365 6c66 2e5f 6474 202a 206e 702e  + self._dt * np.
-00001ff0: 636f 6e63 6174 656e 6174 6528 2872 6f77  concatenate((row
-00002000: 312c 726f 7732 2c72 6f77 332c 726f 7734  1,row2,row3,row4
-00002010: 292c 2061 7869 7320 3d20 3029 0d0a 0d0a  ), axis = 0)....
-00002020: 2020 2020 2020 2020 7265 7475 726e 2070          return p
-00002030: 6869 0d0a 0d0a 0d0a 0d0a 2020 2020 6465  hi........    de
-00002040: 6620 696e 6974 6961 6c69 7a65 5f63 6f6e  f initialize_con
-00002050: 7374 616e 745f 6d61 7472 6963 6573 2873  stant_matrices(s
-00002060: 656c 6629 3a0d 0a20 2020 2020 2020 2027  elf):..        '
-00002070: 2727 0d0a 2020 2020 2020 2020 496e 6974  ''..        Init
-00002080: 6961 6c69 7a65 2066 6f6c 6c6f 7769 6e67  ialize following
-00002090: 206d 6174 7269 6365 733a 0d0a 0d0a 2020   matrices:....  
-000020a0: 2020 2020 2020 415f 7720 3d20 5b0d 0a20        A_w = [.. 
-000020b0: 2020 2020 2020 2020 2020 2030 5f28 3378             0_(3x
-000020c0: 3329 2020 2020 2049 5f33 0d0a 2020 2020  3)     I_3..    
-000020d0: 2020 2020 2020 2020 2d6f 6d65 6761 5e32          -omega^2
-000020e0: 2020 2020 2d32 2a7a 6574 612a 6f6d 6567      -2*zeta*omeg
-000020f0: 610d 0a20 2020 2020 2020 205d 0d0a 0d0a  a..        ]....
-00002100: 2020 2020 2020 2020 4520 3d20 5b0d 0a20          E = [.. 
-00002110: 2020 2020 2020 2020 2020 2030 5f28 3378             0_(3x
-00002120: 3329 2020 2020 2030 5f28 3378 3329 0d0a  3)     0_(3x3)..
-00002130: 2020 2020 2020 2020 2020 2020 455f 7720              E_w 
-00002140: 2020 2020 2020 2020 305f 2833 7833 290d          0_(3x3).
-00002150: 0a20 2020 2020 2020 2020 2020 2030 5f28  .            0_(
-00002160: 3378 3329 2020 2020 2045 5f62 0d0a 2020  3x3)     E_b..  
-00002170: 2020 2020 2020 2020 2020 305f 2833 7833            0_(3x3
-00002180: 2920 2020 2020 305f 2833 7833 290d 0a20  )     0_(3x3).. 
-00002190: 2020 2020 2020 205d 0d0a 0d0a 2020 2020         ]....    
-000021a0: 2020 2020 6761 6d6d 6120 3d20 6474 202a      gamma = dt *
-000021b0: 2045 0d0a 0d0a 2020 2020 2020 2020 4820   E....        H 
-000021c0: 3d20 5b0d 0a20 2020 2020 2020 2020 2020  = [..           
-000021d0: 2030 5f28 3378 3329 2020 2020 2049 5f33   0_(3x3)     I_3
-000021e0: 2020 2020 2049 5f33 2020 2020 2030 5f28       I_3     0_(
-000021f0: 3378 3629 0d0a 2020 2020 2020 2020 5d0d  3x6)..        ].
-00002200: 0a0d 0a20 2020 2020 2020 2042 203d 205b  ...        B = [
-00002210: 0d0a 2020 2020 2020 2020 2020 2020 305f  ..            0_
-00002220: 2831 3278 3329 0d0a 2020 2020 2020 2020  (12x3)..        
-00002230: 2020 2020 4d5f 696e 760d 0a20 2020 2020      M_inv..     
-00002240: 2020 205d 0d0a 0d0a 2020 2020 2020 2020     ]....        
-00002250: 5061 7261 6d65 7465 7273 3a0d 0a20 2020  Parameters:..   
-00002260: 2020 2020 2020 2020 202d 204e 2f41 0d0a           - N/A..
-00002270: 0d0a 2020 2020 2020 2020 546f 2062 6520  ..        To be 
-00002280: 696d 706c 656d 656e 7465 6420 2f20 496d  implemented / Im
-00002290: 7072 6f76 656d 656e 7473 3a0d 0a20 2020  provements:..   
-000022a0: 2020 2020 2020 2020 202d 2054 756e 696e           - Tunin
-000022b0: 6720 6d75 7374 2062 6520 646f 6e65 0d0a  g must be done..
-000022c0: 2020 2020 2020 2020 2020 2020 2d20 4361              - Ca
-000022d0: 6e20 6164 6420 7761 7665 2073 7065 6374  n add wave spect
-000022e0: 7275 6d20 7072 6f70 6572 7469 6573 2061  rum properties a
-000022f0: 7320 696e 7075 7420 696e 2074 756e 696e  s input in tunin
-00002300: 673f 2054 702c 2044 616d 7069 6e67 2c20  g? Tp, Damping, 
-00002310: 4b77 5f69 0d0a 2020 2020 2020 2020 2020  Kw_i..          
-00002320: 2020 2d20 5573 6520 6e70 2e62 6c6f 636b    - Use np.block
-00002330: 2829 2069 6e20 5f41 770d 0a20 2020 2020  () in _Aw..     
-00002340: 2020 2027 2727 0d0a 0d0a 2020 2020 2020     '''....      
-00002350: 2020 2320 415f 770d 0a20 2020 2020 2020    # A_w..       
-00002360: 2054 7020 3d20 3165 3720 2020 2020 2020   Tp = 1e7       
-00002370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002390: 2020 2020 2020 2020 2023 2057 6176 6520           # Wave 
-000023a0: 7065 7269 6f64 0d0a 2020 2020 2020 2020  period..        
-000023b0: 6f6d 6567 6120 3d20 322a 6e70 2e70 692f  omega = 2*np.pi/
-000023c0: 5470 2020 2020 2020 2020 2020 2020 2020  Tp              
-000023d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023e0: 2020 2020 2020 2020 2320 5368 6f75 6c64          # Should
-000023f0: 2061 7070 726f 7820 6265 2070 6561 6b20   approx be peak 
-00002400: 6672 6571 2069 6e20 7761 7665 2073 7065  freq in wave spe
-00002410: 6374 7275 6d0d 0a20 2020 2020 2020 207a  ctrum..        z
-00002420: 6574 6120 3d20 2e30 3520 2020 2020 2020  eta = .05       
-00002430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002450: 2020 2020 2020 2023 2044 616d 7069 6e67         # Damping
-00002460: 2063 6f65 6666 0d0a 2020 2020 2020 2020   coeff..        
-00002470: 2320 4465 6669 6e65 2041 5f77 203d 205b  # Define A_w = [
-00002480: 0d0a 2020 2020 2020 2020 2320 4177 3120  ..        # Aw1 
-00002490: 2020 4177 320d 0a20 2020 2020 2020 2023    Aw2..        #
-000024a0: 2041 7733 2020 2041 7734 0d0a 2020 2020   Aw3   Aw4..    
-000024b0: 2020 2020 2320 5d0d 0a20 2020 2020 2020      # ]..       
-000024c0: 2041 7731 203d 206e 702e 7a65 726f 7328   Aw1 = np.zeros(
-000024d0: 2833 2c33 2929 0d0a 2020 2020 2020 2020  (3,3))..        
-000024e0: 4177 3220 3d20 6e70 2e65 7965 2833 290d  Aw2 = np.eye(3).
-000024f0: 0a20 2020 2020 2020 2041 7733 203d 202d  .        Aw3 = -
-00002500: 6f6d 6567 612a 2a32 2a6e 702e 6579 6528  omega**2*np.eye(
-00002510: 3329 0d0a 2020 2020 2020 2020 4177 3420  3)..        Aw4 
-00002520: 3d20 2d32 2a7a 6574 612a 6f6d 6567 612a  = -2*zeta*omega*
-00002530: 6e70 2e65 7965 2833 290d 0a20 2020 2020  np.eye(3)..     
-00002540: 2020 2073 656c 662e 5f41 7720 3d20 6e70     self._Aw = np
-00002550: 2e63 6f6e 6361 7465 6e61 7465 2828 6e70  .concatenate((np
-00002560: 2e63 6f6e 6361 7465 6e61 7465 2828 4177  .concatenate((Aw
-00002570: 312c 2041 7732 292c 2061 7869 733d 3129  1, Aw2), axis=1)
-00002580: 2c6e 702e 636f 6e63 6174 656e 6174 6528  ,np.concatenate(
-00002590: 2841 7733 2c20 4177 3429 2c20 6178 6973  (Aw3, Aw4), axis
-000025a0: 3d31 2929 2c20 6178 6973 3d30 2920 2023  =1)), axis=0)  #
-000025b0: 2053 686f 756c 6420 7072 6f62 6162 6c79   Should probably
-000025c0: 2062 6520 6d61 6465 206d 6f72 6520 7265   be made more re
-000025d0: 6164 6162 6c65 2e20 5573 6520 6e70 2e62  adable. Use np.b
-000025e0: 6c6f 636b 0d0a 2020 2020 2020 2020 0d0a  lock..        ..
-000025f0: 2020 2020 2020 2020 2320 450d 0a20 2020          # E..   
-00002600: 2020 2020 2073 656c 662e 5f45 203d 206e       self._E = n
-00002610: 702e 7a65 726f 7328 2831 352c 3629 290d  p.zeros((15,6)).
-00002620: 0a20 2020 2020 2020 2045 7720 3d20 6e70  .        Ew = np
-00002630: 2e64 6961 6728 5b31 2c31 2c31 5d29 2a2e  .diag([1,1,1])*.
-00002640: 3031 2020 2020 2020 2020 2020 2020 2020  01              
-00002650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002660: 2023 204d 756c 7469 706c 6965 6420 7769   # Multiplied wi
-00002670: 7468 202e 3031 2062 6563 6175 7365 206e  th .01 because n
-00002680: 6f20 7761 7665 730d 0a20 2020 2020 2020  o waves..       
-00002690: 2045 6220 3d20 6e70 2e65 7965 2833 290d   Eb = np.eye(3).
-000026a0: 0a20 2020 2020 2020 2073 656c 662e 5f45  .        self._E
-000026b0: 5b33 3a36 2c30 3a33 5d20 3d20 4577 200d  [3:6,0:3] = Ew .
-000026c0: 0a20 2020 2020 2020 2073 656c 662e 5f45  .        self._E
-000026d0: 5b39 3a31 322c 333a 365d 203d 2045 620d  [9:12,3:6] = Eb.
-000026e0: 0a0d 0a20 2020 2020 2020 2023 2047 616d  ...        # Gam
-000026f0: 6d61 0d0a 2020 2020 2020 2020 7365 6c66  ma..        self
-00002700: 2e5f 6761 6d6d 6120 3d20 7365 6c66 2e5f  ._gamma = self._
-00002710: 6474 202a 2073 656c 662e 5f45 0d0a 0d0a  dt * self._E....
-00002720: 2020 2020 2020 2020 2320 480d 0a20 2020          # H..   
-00002730: 2020 2020 2073 656c 662e 5f48 203d 206e       self._H = n
-00002740: 702e 7a65 726f 7328 2833 2c31 3529 290d  p.zeros((3,15)).
-00002750: 0a20 2020 2020 2020 2073 656c 662e 5f48  .        self._H
-00002760: 5b30 3a33 2c33 3a36 5d20 3d20 6e70 2e65  [0:3,3:6] = np.e
-00002770: 7965 2833 290d 0a20 2020 2020 2020 2073  ye(3)..        s
-00002780: 656c 662e 5f48 5b30 3a33 2c36 3a39 5d20  elf._H[0:3,6:9] 
-00002790: 3d20 6e70 2e65 7965 2833 290d 0a0d 0a20  = np.eye(3).... 
-000027a0: 2020 2020 2020 2023 2042 0d0a 2020 2020         # B..    
-000027b0: 2020 2020 7365 6c66 2e5f 4220 3d20 6e70      self._B = np
-000027c0: 2e7a 6572 6f73 2828 3135 2c33 2929 0d0a  .zeros((15,3))..
-000027d0: 2020 2020 2020 2020 7365 6c66 2e5f 425b          self._B[
-000027e0: 3132 3a31 352c 2030 3a33 5d20 3d20 7365  12:15, 0:3] = se
-000027f0: 6c66 2e5f 4d69 6e76 0d0a 2020 2020 0d0a  lf._Minv..    ..
-00002800: 0d0a 2020 2020 6465 6620 7365 745f 7475  ..    def set_tu
-00002810: 6e69 6e67 5f6d 6174 7269 6365 7328 7365  ning_matrices(se
-00002820: 6c66 2c20 512c 2052 293a 0d0a 2020 2020  lf, Q, R):..    
-00002830: 2020 2020 7365 6c66 2e5f 5164 203d 2051      self._Qd = Q
-00002840: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-00002850: 5264 203d 2052 0d0a 2020 2020 0d0a 0d0a  Rd = R..    ....
-00002860: 2020 2020 4070 726f 7065 7274 790d 0a20      @property.. 
-00002870: 2020 2064 6566 2078 5f68 6174 2873 656c     def x_hat(sel
-00002880: 6629 3a0d 0a20 2020 2020 2020 2072 6574  f):..        ret
-00002890: 7572 6e20 7365 6c66 2e5f 7868 6174 0d0a  urn self._xhat..
-000028a0: 2020 2020 4070 726f 7065 7274 790d 0a20      @property.. 
-000028b0: 2020 2064 6566 2050 5f68 6174 2873 656c     def P_hat(sel
-000028c0: 6629 3a0d 0a20 2020 2020 2020 2072 6574  f):..        ret
-000028d0: 7572 6e20 7365 6c66 2e5f 5068 6174 0d0a  urn self._Phat..
-000028e0: 2020 2020 4070 726f 7065 7274 790d 0a20      @property.. 
-000028f0: 2020 2064 6566 2065 7461 5f68 6174 2873     def eta_hat(s
-00002900: 656c 6629 3a0d 0a20 2020 2020 2020 2072  elf):..        r
-00002910: 6574 7572 6e20 7365 6c66 2e5f 7868 6174  eturn self._xhat
-00002920: 5b36 3a39 5d0d 0a20 2020 2040 7072 6f70  [6:9]..    @prop
-00002930: 6572 7479 0d0a 2020 2020 6465 6620 6e75  erty..    def nu
-00002940: 5f68 6174 2873 656c 6629 3a0d 0a20 2020  _hat(self):..   
-00002950: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00002960: 2e5f 7868 6174 5b31 323a 3135 5d20 0d0a  ._xhat[12:15] ..
-00002970: 2020 2020 2020 2020 0d0a 0d0a 2727 270d          ....'''.
-00002980: 0a22 5475 6e69 6e67 2066 6163 746f 7273  ."Tuning factors
-00002990: 223a 0d0a 2020 2020 2d20 5120 616e 6420  ":..    - Q and 
-000029a0: 520d 0a20 2020 202d 2054 7020 696e 2041  R..    - Tp in A
-000029b0: 5f77 0d0a 2020 2020 2d20 7a65 7461 2069  _w..    - zeta i
-000029c0: 6e20 415f 770d 0a20 2020 202d 2064 6961  n A_w..    - dia
-000029d0: 6728 4b77 2c4b 772c 4b77 2920 696e 2045  g(Kw,Kw,Kw) in E
-000029e0: 0d0a 2020 2020 2d20 4562 2069 6e20 4520  ..    - Eb in E 
-000029f0: 286e 6ac3 a629 0d0a 2020 2020 2d20 4164  (nj..)..    - Ad
-00002a00: 6a75 7374 6d65 6e74 206f 6620 6e6f 6973  justment of nois
-00002a10: 650d 0a20 2020 202d 2054 696d 6520 7374  e..    - Time st
-00002a20: 6570 0d0a 2020 2020 2d20 496e 6974 6961  ep..    - Initia
-00002a30: 6c20 7661 6c75 6573 0d0a 2727 27         l values..'''
+00001d10: 2020 2020 2020 205b 302c 302c 2d73 656c         [0,0,-sel
+00001d20: 662e 5f4d 696e 765b 312c 315d 2a28 6231  f._Minv[1,1]*(b1
+00001d30: 2a6e 702e 636f 7328 7073 6929 202b 2062  *np.cos(psi) + b
+00001d40: 322a 6e70 2e73 696e 2870 7369 2929 5d2c  2*np.sin(psi))],
+00001d50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001d60: 2020 2020 2020 2020 2020 2020 205b 302c               [0,
+00001d70: 302c 2d73 656c 662e 5f4d 696e 765b 322c  0,-self._Minv[2,
+00001d80: 315d 2a28 6231 2a6e 702e 636f 7328 7073  1]*(b1*np.cos(ps
+00001d90: 6929 202b 2062 322a 6e70 2e73 696e 2870  i) + b2*np.sin(p
+00001da0: 7369 2929 5d0a 2020 2020 2020 2020 5d29  si))].        ])
+00001db0: 0a0a 2020 2020 2020 2020 726f 7731 203d  ..        row1 =
+00001dc0: 206e 702e 636f 6e63 6174 656e 6174 6528   np.concatenate(
+00001dd0: 2873 656c 662e 5f41 772c 206e 702e 7a65  (self._Aw, np.ze
+00001de0: 726f 7328 2836 2c39 2929 292c 2061 7869  ros((6,9))), axi
+00001df0: 733d 3129 0a20 2020 2020 2020 2072 6f77  s=1).        row
+00001e00: 3220 3d20 6e70 2e63 6f6e 6361 7465 6e61  2 = np.concatena
+00001e10: 7465 2828 6e70 2e7a 6572 6f73 2828 332c  te((np.zeros((3,
+00001e20: 3629 292c 2064 656c 5f66 322c 206e 702e  6)), del_f2, np.
+00001e30: 7a65 726f 7328 2833 2c33 2929 2c20 527a  zeros((3,3)), Rz
+00001e40: 2870 7369 2929 2c20 6178 6973 3d31 290a  (psi)), axis=1).
+00001e50: 2020 2020 2020 2020 726f 7733 203d 206e          row3 = n
+00001e60: 702e 7a65 726f 7328 2833 2c31 3529 290a  p.zeros((3,15)).
+00001e70: 2020 2020 2020 2020 726f 7734 203d 206e          row4 = n
+00001e80: 702e 636f 6e63 6174 656e 6174 6528 286e  p.concatenate((n
+00001e90: 702e 7a65 726f 7328 2833 2c36 2929 2c20  p.zeros((3,6)), 
+00001ea0: 6465 6c5f 6634 2c20 7365 6c66 2e5f 4d69  del_f4, self._Mi
+00001eb0: 6e76 4028 527a 2870 7369 292e 5429 2c20  nv@(Rz(psi).T), 
+00001ec0: 2d73 656c 662e 5f4d 696e 7640 7365 6c66  -self._Minv@self
+00001ed0: 2e5f 4429 2c20 6178 6973 3d31 290a 0a20  ._D), axis=1).. 
+00001ee0: 2020 2020 2020 2070 6869 203d 206e 702e         phi = np.
+00001ef0: 6579 6528 3135 2920 2b20 7365 6c66 2e5f  eye(15) + self._
+00001f00: 6474 202a 206e 702e 636f 6e63 6174 656e  dt * np.concaten
+00001f10: 6174 6528 2872 6f77 312c 726f 7732 2c72  ate((row1,row2,r
+00001f20: 6f77 332c 726f 7734 292c 2061 7869 7320  ow3,row4), axis 
+00001f30: 3d20 3029 0a0a 2020 2020 2020 2020 7265  = 0)..        re
+00001f40: 7475 726e 2070 6869 0a0a 0a0a 2020 2020  turn phi....    
+00001f50: 6465 6620 696e 6974 6961 6c69 7a65 5f63  def initialize_c
+00001f60: 6f6e 7374 616e 745f 6d61 7472 6963 6573  onstant_matrices
+00001f70: 2873 656c 662c 2054 7029 3a0a 2020 2020  (self, Tp):.    
+00001f80: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+00001f90: 496e 6974 6961 6c69 7a65 2066 6f6c 6c6f  Initialize follo
+00001fa0: 7769 6e67 206d 6174 7269 6365 733a 0a0a  wing matrices:..
+00001fb0: 2020 2020 2020 2020 415f 7720 3d20 5b0a          A_w = [.
+00001fc0: 2020 2020 2020 2020 2020 2020 305f 2833              0_(3
+00001fd0: 7833 2920 2020 2020 495f 330a 2020 2020  x3)     I_3.    
+00001fe0: 2020 2020 2020 2020 2d6f 6d65 6761 5e32          -omega^2
+00001ff0: 2020 2020 2d32 2a7a 6574 612a 6f6d 6567      -2*zeta*omeg
+00002000: 610a 2020 2020 2020 2020 5d0a 0a20 2020  a.        ]..   
+00002010: 2020 2020 2045 203d 205b 0a20 2020 2020       E = [.     
+00002020: 2020 2020 2020 2030 5f28 3378 3329 2020         0_(3x3)  
+00002030: 2020 2030 5f28 3378 3329 0a20 2020 2020     0_(3x3).     
+00002040: 2020 2020 2020 2045 5f77 2020 2020 2020         E_w      
+00002050: 2020 2030 5f28 3378 3329 0a20 2020 2020     0_(3x3).     
+00002060: 2020 2020 2020 2030 5f28 3378 3329 2020         0_(3x3)  
+00002070: 2020 2030 5f28 3378 3329 0a20 2020 2020     0_(3x3).     
+00002080: 2020 2020 2020 2030 5f28 3378 3329 2020         0_(3x3)  
+00002090: 2020 2045 5f62 0a20 2020 2020 2020 2020     E_b.         
+000020a0: 2020 2030 5f28 3378 3329 2020 2020 2030     0_(3x3)     0
+000020b0: 5f28 3378 3329 0a20 2020 2020 2020 205d  _(3x3).        ]
+000020c0: 0a0a 2020 2020 2020 2020 6761 6d6d 6120  ..        gamma 
+000020d0: 3d20 6474 202a 2045 0a0a 2020 2020 2020  = dt * E..      
+000020e0: 2020 4820 3d20 5b0a 2020 2020 2020 2020    H = [.        
+000020f0: 2020 2020 305f 2833 7833 2920 2020 2020      0_(3x3)     
+00002100: 495f 3320 2020 2020 495f 3320 2020 2020  I_3     I_3     
+00002110: 305f 2833 7836 290a 2020 2020 2020 2020  0_(3x6).        
+00002120: 5d0a 0a20 2020 2020 2020 2042 203d 205b  ]..        B = [
+00002130: 0a20 2020 2020 2020 2020 2020 2030 5f28  .            0_(
+00002140: 3132 7833 290a 2020 2020 2020 2020 2020  12x3).          
+00002150: 2020 4d5f 696e 760a 2020 2020 2020 2020    M_inv.        
+00002160: 5d0a 0a20 2020 2020 2020 2050 6172 616d  ]..        Param
+00002170: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+00002180: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+00002190: 2020 2020 202d 2054 703a 2053 6561 2073       - Tp: Sea s
+000021a0: 7461 7465 2070 6561 6b20 7065 7269 6f64  tate peak period
+000021b0: 0a0a 2020 2020 2020 2020 546f 2062 6520  ..        To be 
+000021c0: 696d 706c 656d 656e 7465 6420 2f20 496d  implemented / Im
+000021d0: 7072 6f76 656d 656e 7473 0a20 2020 2020  provements.     
+000021e0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+000021f0: 2020 2020 2020 2020 2020 2d20 5475 6e69            - Tuni
+00002200: 6e67 206d 7573 7420 6265 2064 6f6e 650a  ng must be done.
+00002210: 2020 2020 2020 2020 2020 2020 2d20 4361              - Ca
+00002220: 6e20 6164 6420 7761 7665 2073 7065 6374  n add wave spect
+00002230: 7275 6d20 7072 6f70 6572 7469 6573 2061  rum properties a
+00002240: 7320 696e 7075 7420 696e 2074 756e 696e  s input in tunin
+00002250: 673f 2054 702c 2044 616d 7069 6e67 2c20  g? Tp, Damping, 
+00002260: 4b77 5f69 0a20 2020 2020 2020 2020 2020  Kw_i.           
+00002270: 202d 2055 7365 206e 702e 626c 6f63 6b28   - Use np.block(
+00002280: 2920 696e 205f 4177 0a20 2020 2020 2020  ) in _Aw.       
+00002290: 2027 2727 0a0a 2020 2020 2020 2020 2320   '''..        # 
+000022a0: 415f 770a 2020 2020 2020 2020 6f6d 6567  A_w.        omeg
+000022b0: 6120 3d20 322a 6e70 2e70 692f 5470 2020  a = 2*np.pi/Tp  
+000022c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022e0: 2020 2020 2320 5368 6f75 6c64 2061 7070      # Should app
+000022f0: 726f 7820 6265 2070 6561 6b20 6672 6571  rox be peak freq
+00002300: 2069 6e20 7761 7665 2073 7065 6374 7275   in wave spectru
+00002310: 6d0a 2020 2020 2020 2020 7a65 7461 203d  m.        zeta =
+00002320: 202e 3035 2020 2020 2020 2020 2020 2020   .05            
+00002330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002350: 2020 2320 4461 6d70 696e 6720 636f 6566    # Damping coef
+00002360: 660a 2020 2020 2020 2020 2727 2744 6566  f.        '''Def
+00002370: 696e 6520 415f 7720 3d20 5b0a 2020 2020  ine A_w = [.    
+00002380: 2020 2020 2020 2020 2020 2020 4177 3131              Aw11
+00002390: 2020 2041 7731 320a 2020 2020 2020 2020     Aw12.        
+000023a0: 2020 2020 2020 2020 4177 3231 2020 2041          Aw21   A
+000023b0: 7732 3220 205d 2727 270a 2020 2020 2020  w22  ]'''.      
+000023c0: 2020 4177 3131 203d 206e 702e 7a65 726f    Aw11 = np.zero
+000023d0: 7328 2833 2c33 2929 0a20 2020 2020 2020  s((3,3)).       
+000023e0: 2041 7731 3220 3d20 6e70 2e65 7965 2833   Aw12 = np.eye(3
+000023f0: 290a 2020 2020 2020 2020 4177 3231 203d  ).        Aw21 =
+00002400: 202d 6f6d 6567 612a 2a32 2a6e 702e 6579   -omega**2*np.ey
+00002410: 6528 3329 0a20 2020 2020 2020 2041 7732  e(3).        Aw2
+00002420: 3220 3d20 2d32 2a7a 6574 612a 6f6d 6567  2 = -2*zeta*omeg
+00002430: 612a 6e70 2e65 7965 2833 290a 2020 2020  a*np.eye(3).    
+00002440: 2020 2020 7365 6c66 2e5f 4177 203d 206e      self._Aw = n
+00002450: 702e 626c 6f63 6b28 5b5b 4177 3131 2c20  p.block([[Aw11, 
+00002460: 4177 3132 5d2c 205b 4177 3231 2c20 4177  Aw12], [Aw21, Aw
+00002470: 3232 5d5d 290a 0a20 2020 2020 2020 2023  22]])..        #
+00002480: 2045 0a20 2020 2020 2020 2073 656c 662e   E.        self.
+00002490: 5f45 203d 206e 702e 7a65 726f 7328 2831  _E = np.zeros((1
+000024a0: 352c 3629 290a 2020 2020 2020 2020 4577  5,6)).        Ew
+000024b0: 203d 206e 702e 6469 6167 285b 312c 312c   = np.diag([1,1,
+000024c0: 315d 2920 2020 2020 2020 2020 2020 2020  1])             
+000024d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024e0: 2020 2320 4d75 6c74 6970 6c69 6564 2077    # Multiplied w
+000024f0: 6974 6820 2e30 3120 6265 6361 7573 6520  ith .01 because 
+00002500: 6e6f 2077 6176 6573 0a20 2020 2020 2020  no waves.       
+00002510: 2045 6220 3d20 6e70 2e65 7965 2833 290a   Eb = np.eye(3).
+00002520: 2020 2020 2020 2020 7365 6c66 2e5f 455b          self._E[
+00002530: 333a 362c 303a 335d 203d 2045 7720 0a20  3:6,0:3] = Ew . 
+00002540: 2020 2020 2020 2073 656c 662e 5f45 5b39         self._E[9
+00002550: 3a31 322c 333a 365d 203d 2045 620a 0a20  :12,3:6] = Eb.. 
+00002560: 2020 2020 2020 2023 2047 616d 6d61 0a20         # Gamma. 
+00002570: 2020 2020 2020 2073 656c 662e 5f67 616d         self._gam
+00002580: 6d61 203d 2073 656c 662e 5f64 7420 2a20  ma = self._dt * 
+00002590: 7365 6c66 2e5f 450a 0a20 2020 2020 2020  self._E..       
+000025a0: 2023 2048 0a20 2020 2020 2020 2073 656c   # H.        sel
+000025b0: 662e 5f48 203d 206e 702e 7a65 726f 7328  f._H = np.zeros(
+000025c0: 2833 2c31 3529 290a 2020 2020 2020 2020  (3,15)).        
+000025d0: 7365 6c66 2e5f 485b 303a 332c 333a 365d  self._H[0:3,3:6]
+000025e0: 203d 206e 702e 6579 6528 3329 0a20 2020   = np.eye(3).   
+000025f0: 2020 2020 2073 656c 662e 5f48 5b30 3a33       self._H[0:3
+00002600: 2c36 3a39 5d20 3d20 6e70 2e65 7965 2833  ,6:9] = np.eye(3
+00002610: 290a 0a20 2020 2020 2020 2023 2042 0a20  )..        # B. 
+00002620: 2020 2020 2020 2073 656c 662e 5f42 203d         self._B =
+00002630: 206e 702e 7a65 726f 7328 2831 352c 3329   np.zeros((15,3)
+00002640: 290a 2020 2020 2020 2020 7365 6c66 2e5f  ).        self._
+00002650: 425b 3132 3a31 352c 2030 3a33 5d20 3d20  B[12:15, 0:3] = 
+00002660: 7365 6c66 2e5f 4d69 6e76 0a20 2020 200a  self._Minv.    .
+00002670: 0a20 2020 2064 6566 2073 6574 5f74 756e  .    def set_tun
+00002680: 696e 675f 6d61 7472 6963 6573 2873 656c  ing_matrices(sel
+00002690: 662c 2051 2c20 5229 3a0a 2020 2020 2020  f, Q, R):.      
+000026a0: 2020 2727 270a 2020 2020 2020 2020 7365    '''.        se
+000026b0: 745f 7475 6e69 6e67 5f6d 6174 7269 6365  t_tuning_matrice
+000026c0: 730a 2020 2020 2020 2020 4375 7374 6f6d  s.        Custom
+000026d0: 697a 6520 7475 6e69 6e67 206d 6174 7269  ize tuning matri
+000026e0: 6365 7320 696e 2074 6865 2045 4b46 0a0a  ces in the EKF..
+000026f0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+00002700: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
+00002710: 2d2d 2d2d 2d0a 2020 2020 2020 2020 5120  -----.        Q 
+00002720: 3a20 6172 7261 795f 6c69 6b65 0a20 2020  : array_like.   
+00002730: 2020 2020 2020 2020 2028 362c 3629 2d64           (6,6)-d
+00002740: 696d 2061 7272 6179 2073 7461 7469 6e67  im array stating
+00002750: 2063 6f76 6172 6961 6e63 6520 696e 206d   covariance in m
+00002760: 6f64 656c 2075 6e63 6572 7461 696e 7479  odel uncertainty
+00002770: 0a20 2020 2020 2020 2052 203a 2061 7272  .        R : arr
+00002780: 6179 5f6c 696b 650a 2020 2020 2020 2020  ay_like.        
+00002790: 2020 2020 2836 2c36 292d 6469 6d20 6172      (6,6)-dim ar
+000027a0: 7261 7920 7374 6174 696e 6720 636f 7661  ray stating cova
+000027b0: 7269 616e 6365 2069 6e20 6d65 6173 7572  riance in measur
+000027c0: 656d 656e 7420 756e 6365 7274 6169 6e74  ement uncertaint
+000027d0: 790a 0a20 2020 2020 2020 2052 6574 7572  y..        Retur
+000027e0: 6e0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  n.        ------
+000027f0: 0a20 2020 2020 2020 204e 2f41 0a20 2020  .        N/A.   
+00002800: 2020 2020 200a 2020 2020 2020 2020 2727       .        ''
+00002810: 270a 2020 2020 2020 2020 7365 6c66 2e5f  '.        self._
+00002820: 5164 203d 2051 0a20 2020 2020 2020 2073  Qd = Q.        s
+00002830: 656c 662e 5f52 6420 3d20 520a 2020 2020  elf._Rd = R.    
+00002840: 0a0a 2020 2020 0a20 2020 2064 6566 2067  ..    .    def g
+00002850: 6574 5f78 5f68 6174 2873 656c 6629 3a0a  et_x_hat(self):.
+00002860: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00002870: 656c 662e 5f78 6861 740a 2020 2020 0a20  elf._xhat.    . 
+00002880: 2020 2064 6566 2067 6574 5f50 5f68 6174     def get_P_hat
+00002890: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000028a0: 7265 7475 726e 2073 656c 662e 5f50 6861  return self._Pha
+000028b0: 740a 2020 2020 0a20 2020 2064 6566 2067  t.    .    def g
+000028c0: 6574 5f65 7461 5f68 6174 2873 656c 6629  et_eta_hat(self)
+000028d0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+000028e0: 2073 656c 662e 5f78 6861 745b 363a 395d   self._xhat[6:9]
+000028f0: 0a20 2020 200a 2020 2020 6465 6620 6765  .    .    def ge
+00002900: 745f 6e75 5f68 6174 2873 656c 6629 3a0a  t_nu_hat(self):.
+00002910: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00002920: 656c 662e 5f78 6861 745b 3132 3a31 355d  elf._xhat[12:15]
+00002930: 200a 2020 2020 2020 2020 0a0a 2727 270a   .        ..'''.
+00002940: 2254 756e 696e 6720 6661 6374 6f72 7322  "Tuning factors"
+00002950: 3a0a 2020 2020 2d20 5120 616e 6420 520a  :.    - Q and R.
+00002960: 2020 2020 2d20 5470 2069 6e20 415f 770a      - Tp in A_w.
+00002970: 2020 2020 2d20 7a65 7461 2069 6e20 415f      - zeta in A_
+00002980: 770a 2020 2020 2d20 6469 6167 284b 772c  w.    - diag(Kw,
+00002990: 4b77 2c4b 7729 2069 6e20 450a 2020 2020  Kw,Kw) in E.    
+000029a0: 2d20 4562 2069 6e20 4520 286e 6ac3 a629  - Eb in E (nj..)
+000029b0: 0a20 2020 202d 2041 646a 7573 746d 656e  .    - Adjustmen
+000029c0: 7420 6f66 206e 6f69 7365 0a20 2020 202d  t of noise.    -
+000029d0: 2054 696d 6520 7374 6570 0a20 2020 202d   Time step.    -
+000029e0: 2049 6e69 7469 616c 2076 616c 7565 730a   Initial values.
+000029f0: 2727 27                                  '''
```

### Comparing `MCSimPython-0.0.14/src/MCSimPython/observer/nonlinobs.py` & `MCSimPython-0.1.1/src/MCSimPython/observer/nonlinobs.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-# nonlinobs.py
-
-# ----------------------------------------------------------------------------
-# This code is part of the MCSimPython toolbox and repository.
-# Created By: Jan-Erik Hygen
-# Created Date: 2023-01-23
-# Revised: 
-# Tested:
-# Copyright (C) 2023: NTNU, Trondheim
-# Licensed under GPL-3.0-or-later
-# ---------------------------------------------------------------------------
-
-import numpy as np
-from MCSimPython.utils import Rz, pipi
-
-
-class NonlinObs3dof:
-
-    def __init__(self, dt, wc, wo, lambd, T, M, D, lambda_w=0.03):
-        self._dt = dt
-        lambda_w = lambda_w
-        self.zeta = 1.0
-        self.K1 = np.block([
-            [-2*(self.zeta-lambd)*(wc/wo) * np.eye(3)],
-            [2*wo*(self.zeta-lambd)*np.eye(3)]
-        ])
-        self.K2 = np.diag([wc, wc, wc])
-        self.K4 = np.diag([1.0, 1.0, 0.1])
-        self.K3 = .1*self.K4
-        self.Aw = np.block([
-            [np.zeros((3,3)), np.eye(3)],
-            [-wo**2*np.eye(3), -2*lambd*wo*np.eye(3)],
-        ])
-        self.Tinv = np.linalg.inv(T*np.eye(3))
-        self._x_hat = np.zeros((15))
-        self._y_hat = np.zeros(3)
-        self.M = M
-        self.D = D
-        self.Minv = np.linalg.inv(M)
-
-    @property
-    def xi(self):
-        return self._x_hat[:6]
-
-    @property
-    def eta(self):
-        return self._x_hat[6:9]
-    
-    @property
-    def bias(self):
-        return self._x_hat[9:12]
-
-    @property
-    def nu(self):
-        return self._x_hat[12:]
-    
-    def dynamics(self, tau, y):
-        y_tilde = y - self._y_hat
-        # Ensure that the smallest angle is used
-        y_tilde[2] = pipi(np.copy(y_tilde[2]))
-        xi_hat_dot = self.Aw@self.xi + self.K1@y_tilde
-        eta_hat_dot = Rz(y[2])@self.nu + self.K2@y_tilde
-        b_hat_dot = -self.Tinv@self.bias + self.K3@y_tilde
-        nu_hat_dot = self.Minv@(-self.D@self.nu + tau + Rz(y[2]).T@self.bias + Rz(y[2]).T@self.K4@y_tilde)
-        return np.concatenate((xi_hat_dot, eta_hat_dot, b_hat_dot, nu_hat_dot))
-
-    def update(self, y, tau):
-        self._x_hat = self._x_hat + self._dt * self.dynamics(tau, y)
+# nonlinobs.py
+
+# ----------------------------------------------------------------------------
+# This code is part of the MCSimPython toolbox and repository.
+# Created By: Jan-Erik Hygen
+# Created Date: 2023-01-23
+# Revised: 
+# Tested:
+# Copyright (C) 2023: NTNU, Trondheim
+# Licensed under GPL-3.0-or-later
+# ---------------------------------------------------------------------------
+
+import numpy as np
+from MCSimPython.utils import Rz, pipi
+
+
+class NonlinObs3dof:
+
+    def __init__(self, dt, wc, wo, lambd, T, M, D, lambda_w=0.03):
+        self._dt = dt
+        lambda_w = lambda_w
+        self.zeta = 1.0
+        self.K1 = np.block([
+            [-2*(self.zeta-lambd)*(wc/wo) * np.eye(3)],
+            [2*wo*(self.zeta-lambd)*np.eye(3)]
+        ])
+        self.K2 = np.diag([wc, wc, wc])
+        self.K4 = np.diag([1.0, 1.0, 0.1])
+        self.K3 = .1*self.K4
+        self.Aw = np.block([
+            [np.zeros((3,3)), np.eye(3)],
+            [-wo**2*np.eye(3), -2*lambd*wo*np.eye(3)],
+        ])
+        self.Tinv = np.linalg.inv(T*np.eye(3))
+        self._x_hat = np.zeros((15))
+        self._y_hat = np.zeros(3)
+        self.M = M
+        self.D = D
+        self.Minv = np.linalg.inv(M)
+
+    @property
+    def xi(self):
+        return self._x_hat[:6]
+
+    @property
+    def eta(self):
+        return self._x_hat[6:9]
+    
+    @property
+    def bias(self):
+        return self._x_hat[9:12]
+
+    @property
+    def nu(self):
+        return self._x_hat[12:]
+    
+    def dynamics(self, tau, y):
+        y_tilde = y - self._y_hat
+        # Ensure that the smallest angle is used
+        y_tilde[2] = pipi(np.copy(y_tilde[2]))
+        xi_hat_dot = self.Aw@self.xi + self.K1@y_tilde
+        eta_hat_dot = Rz(y[2])@self.nu + self.K2@y_tilde
+        b_hat_dot = -self.Tinv@self.bias + self.K3@y_tilde
+        nu_hat_dot = self.Minv@(-self.D@self.nu + tau + Rz(y[2]).T@self.bias + Rz(y[2]).T@self.K4@y_tilde)
+        return np.concatenate((xi_hat_dot, eta_hat_dot, b_hat_dot, nu_hat_dot))
+
+    def update(self, y, tau):
+        self._x_hat = self._x_hat + self._dt * self.dynamics(tau, y)
         self._y_hat = self.xi[3:] + self.eta
```

### Comparing `MCSimPython-0.0.14/src/MCSimPython/simulator/__init__.py` & `MCSimPython-0.1.1/src/MCSimPython/simulator/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""
-Vessel Simulation Models (:mod:`MCSimPython.simulator`)
-=======================================================
-
-The MCSimPython simulator package contains a set of 
-different simulation models.
-
-Contents
----------
-The following modules are found in the `MCSimPython.simulator`.
-
-- vessel.py        --- Base class for vessel simulation models.
-
-- csad.py          --- Simulation models for C/S Arctic Drillship.
-
-- gunnerus.py      --- Simulation models for R/V Gunnerus.
-"""
-
-# Import all the models s.t we can access them from e.g. 
-# from MCSimPython.simulator import CSAD_DP_6DOF
-from MCSimPython.simulator.csad import CSAD_DP_6DOF, CSADMan3DOF
+"""
+Vessel Simulation Models (:mod:`MCSimPython.simulator`)
+=======================================================
+
+The MCSimPython simulator package contains a set of 
+different simulation models.
+
+Contents
+---------
+The following modules are found in the `MCSimPython.simulator`.
+
+- vessel.py        --- Base class for vessel simulation models.
+
+- csad.py          --- Simulation models for C/S Arctic Drillship.
+
+- gunnerus.py      --- Simulation models for R/V Gunnerus.
+"""
+
+# Import all the models s.t we can access them from e.g. 
+# from MCSimPython.simulator import CSAD_DP_6DOF
+from MCSimPython.simulator.csad import CSAD_DP_6DOF, CSADMan3DOF, CSAD_DP_Seakeeping
 from MCSimPython.simulator.gunnerus import GunnerusManeuvering3DoF, RVG_DP_6DOF
```

### Comparing `MCSimPython-0.0.14/src/MCSimPython/simulator/thruster_dynamics.py` & `MCSimPython-0.1.1/src/MCSimPython/simulator/thruster_dynamics.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,180 +1,180 @@
-import numpy as np
-import MCSimPython.vessel_data.CSAD.thruster_data as data 
-
-
-class ThrusterDynamics:
-
-    def __init__(self, u, alpha, dt):
-        self._u = u
-        self._alpha = alpha
-        self._dt = dt
-
-        self._K = np.diag(data.K)
-        self._lx = data.lx
-        self._ly = data.ly
-        self._n_thrusters = len(data.lx)
-
-    def saturate(self, signal, min, max):
-
-        """
-        Saturates a given signal with both an upper and lower bound.
-
-        Parameters
-        -----------
-        signal : array_like or scalar
-            To be saturated.
-
-        Returns
-        --------
-        array_like or scalar
-            Saturated signal
-        """
-
-        return np.clip(signal, min, max)
-
-    def limit_rate(self, signal_curr, signal_prev, max):
-
-        """
-        Limits the rate of change of the signal with respect to a max rate.
-        Signal is a vector with the same dimension as number of thrusters.
-
-        POSSIBLE EXTENTIONS:
-            - at the time being, each thruster will need to have the same rate limit,
-              better to exclude the loop?
-
-        Parameters
-        -----------
-        signal_curr : array_like
-            Current signal.
-        signal_prev : array_like
-            Signal prom frevious time step.
-        max : scalar
-            Max rate of change for signal
-
-        Returns
-        --------
-        array_like
-            Rate limited signal
-        """
-
-        for i in range(self._n_thrusters):
-            if (np.abs(signal_curr[i]-signal_prev[i])/self._dt > max):
-                signal_curr[i] = signal_prev[i] + abs(max * self._dt)
-
-        return signal_curr
-
-    def propeller_revolution(self, u):
-
-        """
-        Calculates the propeller revolution number from the control signal.
-        To be used if n needs to be saturated/rate limited.
-
-        CHECK:
-            - is this the correct way to multiply
-        
-        Parameters
-        -----------
-        u : array_like
-            Control signal.
-
-        Returns
-        --------
-        n : array_like
-            propeller revolution number.
-        """
-
-        n = np.sign(u) * np.sqrt(np.abs(u))
-
-        return n
-    
-    def control_input(self, n):
-
-        """
-        Calculates the the control input from the propeller revolution number.
-        Use this if you have been saturating n.
-
-        CHECK:
-            - is this the correct way to multiply
-
-        Parameters
-        -----------
-        n : array_like
-            propeller revolution number.
-
-        Returns
-        --------
-        u : array_like
-            Control signal.
-        """
-
-        u = n * np.abs(n)
-
-        return u 
-
-    def actuator_loads(self, u):
-
-        """
-        Computes load on each actuator from the control inputs.
-
-        Parameters
-        -----------
-        u : array_like
-            Control signal.
-
-        Returns
-        --------
-         : array_like
-            Actuator loads.
-
-        """
-        
-        return self._K @ u
-    
-    def thruster_configuration(self, alpha):
-
-        """
-        Sets up the thrust configuration matrix.
-        
-        Parameters
-        -----------
-        alpha : array_like
-            Azimuth angles.
-
-        Returns
-        --------
-         : array_like
-            Thrust configuration matrix.
-        """
-
-        return np.array([
-            np.cos(alpha),
-            np.sin(alpha),
-            self._lx * np.sin(alpha) - self._ly * np.cos(alpha)
-        ])
-
-    def get_tau(self, u, alpha):
-
-        """
-        Computes resulting thrust and moments in surge, sway and yaw from the actuators.
-        
-        Parameters
-        -----------
-        actual_actuator_loads : array_like
-            The value of the actuator loads after rate limitation and saturation.
-        alpha_actual : array_like
-            The angle of the azimuth thrusters after rate limitations and zone restriction.
-
-        Returns
-        --------
-         : array_like
-            Thrust and moments in surge, sway and yaw.
-        """
-
-        return self.thruster_configuration(alpha) @ self.actuator_loads(u)
-
-
-
-        
-
-
-
+import numpy as np
+import MCSimPython.vessel_data.CSAD.thruster_data as data 
+
+
+class ThrusterDynamics:
+
+    def __init__(self):
+        #self._u = u
+        #self._alpha = alpha
+        #self._dt = dt
+
+        self._K = np.diag(data.K)
+        self._lx = data.lx
+        self._ly = data.ly
+        self._n_thrusters = len(data.lx)
+
+    def saturate(self, signal, min, max):
+
+        """
+        Saturates a given signal with both an upper and lower bound.
+
+        Parameters
+        -----------
+        signal : array_like or scalar
+            To be saturated.
+
+        Returns
+        --------
+        array_like or scalar
+            Saturated signal
+        """
+
+        return np.clip(signal, min, max)
+
+    def limit_rate(self, signal_curr, signal_prev, max):
+
+        """
+        Limits the rate of change of the signal with respect to a max rate.
+        Signal is a vector with the same dimension as number of thrusters.
+
+        POSSIBLE EXTENTIONS:
+            - at the time being, each thruster will need to have the same rate limit,
+              better to exclude the loop?
+
+        Parameters
+        -----------
+        signal_curr : array_like
+            Current signal.
+        signal_prev : array_like
+            Signal prom frevious time step.
+        max : scalar
+            Max rate of change for signal
+
+        Returns
+        --------
+        array_like
+            Rate limited signal
+        """
+
+        for i in range(self._n_thrusters):
+            if (np.abs(signal_curr[i]-signal_prev[i])/self._dt > max):
+                signal_curr[i] = signal_prev[i] + abs(max * self._dt)
+
+        return signal_curr
+
+    def propeller_revolution(self, u):
+
+        """
+        Calculates the propeller revolution number from the control signal.
+        To be used if n needs to be saturated/rate limited.
+
+        CHECK:
+            - is this the correct way to multiply
+        
+        Parameters
+        -----------
+        u : array_like
+            Control signal.
+
+        Returns
+        --------
+        n : array_like
+            propeller revolution number.
+        """
+
+        n = np.sign(u) * np.sqrt(np.abs(u))
+
+        return n
+    
+    def control_input(self, n):
+
+        """
+        Calculates the the control input from the propeller revolution number.
+        Use this if you have been saturating n.
+
+        CHECK:
+            - is this the correct way to multiply
+
+        Parameters
+        -----------
+        n : array_like
+            propeller revolution number.
+
+        Returns
+        --------
+        u : array_like
+            Control signal.
+        """
+
+        u = n * np.abs(n)
+
+        return u 
+
+    def actuator_loads(self, u):
+
+        """
+        Computes load on each actuator from the control inputs.
+
+        Parameters
+        -----------
+        u : array_like
+            Control signal.
+
+        Returns
+        --------
+         : array_like
+            Actuator loads.
+
+        """
+        
+        return self._K @ u
+    
+    def thruster_configuration(self, alpha):
+
+        """
+        Sets up the thrust configuration matrix.
+        
+        Parameters
+        -----------
+        alpha : array_like
+            Azimuth angles.
+
+        Returns
+        --------
+         : array_like
+            Thrust configuration matrix.
+        """
+
+        return np.array([
+            np.cos(alpha),
+            np.sin(alpha),
+            self._lx * np.sin(alpha) - self._ly * np.cos(alpha)
+        ])
+
+    def get_tau(self, u, alpha):
+
+        """
+        Computes resulting thrust and moments in surge, sway and yaw from the actuators.
+        
+        Parameters
+        -----------
+        actual_actuator_loads : array_like
+            The value of the actuator loads after rate limitation and saturation.
+        alpha_actual : array_like
+            The angle of the azimuth thrusters after rate limitations and zone restriction.
+
+        Returns
+        --------
+         : array_like
+            Thrust and moments in surge, sway and yaw.
+        """
+
+        return self.thruster_configuration(alpha) @ self.actuator_loads(u)
+
+
+
+        
+
+
+
```

### Comparing `MCSimPython-0.0.14/src/MCSimPython/thrust_allocation/allocation.py` & `MCSimPython-0.1.1/src/MCSimPython/thrust_allocation/allocation.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,166 +1,166 @@
-from abc import ABC, abstractmethod
-from MCSimPython.thrust_allocation.thruster import Thruster
-from itertools import repeat
-import numpy as np
-
-DOFS = 3
-
-class AllocationError(Exception):
-    """
-    AllocationError class
-    """
-
-class AllocatorCSAD(ABC):
-    """
-    Abstract base class for allocation problem
-    formulations. Spesific for CSAD.
-    """
-
-    def __init__(self):
-        self._thrusters = []
-
-    @property
-    def n_thrusters(self):
-        """
-        Number of thrusters assigned to this
-        allocation problem.
-        """
-        return len(self._thrusters)
-
-    def add_thruster(self, thruster):
-        """
-        Add a thruster to the allocation problem.
-        """
-        if isinstance(thruster, Thruster):
-            self._thrusters.append(thruster)
-        else:
-            raise TypeError("Thruster is not of proper type!")
-    
-
-    @abstractmethod
-    def allocation_problem(self):
-        """
-        Assemble allocation problem into matrix form
-        """
-
-
-    @abstractmethod
-    def allocate(self, tau_d):
-        """
-        Allocate global thrust vector to available thrusters. 
-        """
-    
-
-class pseudo_inverse_allocator(AllocatorCSAD):
-
-    @property
-    def n_problem(self):
-        """
-        Number of unknown variables to be allocated
-        in the original problem.
-        """
-        return 2 * self.n_thrusters
-
-    def allocation_problem(self):
-
-        """
-        Assemble extended allocation problem into matrix form.
-        """
-
-        T_e = np.zeros((DOFS, self.n_problem))
-        T_e[0, ::2] = 1
-        T_e[1, 1::2] = 1
-        T_e[2, ::2] = [-thruster.pos_y for thruster in self._thrusters]
-        T_e[2, 1::2] = [thruster.pos_x for thruster in self._thrusters]
-        
-        K_lst = [thruster._K for thruster in self._thrusters]
-
-        K_vec = [x for item in K_lst for x in repeat(item, 2)]
-
-        K_e = np.diag(K_vec)
-
-        return T_e, K_e
-    
-
-    def allocate(self, tau_d):
-
-        """
-        Allocate global thrust vector to available thrusters. 
-        """
-
-        if self.n_thrusters == 0:
-            raise AllocationError(
-                """At least one thruster must be added
-                    to the
-                    allocator-object before attempting an allocation!"""
-            )
-        
-        T_e, K_e = self.allocation_problem()
-
-        T_e_pseudo = np.transpose(T_e) @ (np.linalg.inv(T_e @ np.transpose(T_e)))
-
-        u_e = np.linalg.inv(K_e) @ T_e_pseudo @ tau_d
-
-        u = np.zeros(self.n_thrusters)
-        alpha = np.zeros(self.n_thrusters)
-
-        for i in range(self.n_thrusters):
-            u[i] = np.sqrt(u_e[i*2]**2 + u_e[i*2+1]**2)
-            alpha[i] = np.arctan2(u_e[i*2+1], u_e[i*2])
-        
-        return u, alpha
-
-
-class fixed_angle_allocator(AllocatorCSAD):
-
-    theta = np.deg2rad(30)
-
-    alpha = np.array([np.pi,
-             np.pi/2 + theta,
-             3 * np.pi/2 - theta,
-             - np.pi,
-             - np.pi/2 + theta,
-             np.pi/2 - theta])
-
-    def allocation_problem(self):
-        """
-        Assemble extended allocation problem into matrix form
-        """
-
-        K_lst = [thruster._K for thruster in self._thrusters]
-
-        lx = [thruster.pos_x for thruster in self._thrusters]
-        ly = [thruster.pos_y for thruster in self._thrusters]
-
-        K = np.diag(K_lst)
-        
-        T = np.array([
-            np.cos(self.alpha),
-            np.sin(self.alpha),
-            lx * np.sin(self.alpha) - ly * np.cos(self.alpha)])
-
-        return T, K
-
-    def allocate(self, tau_d):
-        """
-        Allocate global thrust vector to available thrusters. 
-        """
-
-        if self.n_thrusters == 0:
-            raise AllocationError(
-                """At least one thruster must be added
-                    to the
-                    allocator-object before attempting an allocation!"""
-            )
-        
-        T, K = self.allocation_problem()
-
-        B = T @ K
-
-        B_inv = np.transpose(B) @ (np.linalg.inv(B @ np.transpose(B)))
-
-        u = B_inv @ tau_d
-
-        alpha = self.alpha
-        
-        return u, alpha
+from abc import ABC, abstractmethod
+from MCSimPython.thrust_allocation.thruster import Thruster
+from itertools import repeat
+import numpy as np
+
+DOFS = 3
+
+class AllocationError(Exception):
+    """
+    AllocationError class
+    """
+
+class AllocatorCSAD(ABC):
+    """
+    Abstract base class for allocation problem
+    formulations. Spesific for CSAD.
+    """
+
+    def __init__(self):
+        self._thrusters = []
+
+    @property
+    def n_thrusters(self):
+        """
+        Number of thrusters assigned to this
+        allocation problem.
+        """
+        return len(self._thrusters)
+
+    def add_thruster(self, thruster):
+        """
+        Add a thruster to the allocation problem.
+        """
+        if isinstance(thruster, Thruster):
+            self._thrusters.append(thruster)
+        else:
+            raise TypeError("Thruster is not of proper type!")
+    
+
+    @abstractmethod
+    def allocation_problem(self):
+        """
+        Assemble allocation problem into matrix form
+        """
+
+
+    @abstractmethod
+    def allocate(self, tau_d):
+        """
+        Allocate global thrust vector to available thrusters. 
+        """
+    
+
+class pseudo_inverse_allocator(AllocatorCSAD):
+
+    @property
+    def n_problem(self):
+        """
+        Number of unknown variables to be allocated
+        in the original problem.
+        """
+        return 2 * self.n_thrusters
+
+    def allocation_problem(self):
+
+        """
+        Assemble extended allocation problem into matrix form.
+        """
+
+        T_e = np.zeros((DOFS, self.n_problem))
+        T_e[0, ::2] = 1
+        T_e[1, 1::2] = 1
+        T_e[2, ::2] = [-thruster.pos_y for thruster in self._thrusters]
+        T_e[2, 1::2] = [thruster.pos_x for thruster in self._thrusters]
+        
+        K_lst = [thruster._K for thruster in self._thrusters]
+
+        K_vec = [x for item in K_lst for x in repeat(item, 2)]
+
+        K_e = np.diag(K_vec)
+
+        return T_e, K_e
+    
+
+    def allocate(self, tau_d):
+
+        """
+        Allocate global thrust vector to available thrusters. 
+        """
+
+        if self.n_thrusters == 0:
+            raise AllocationError(
+                """At least one thruster must be added
+                    to the
+                    allocator-object before attempting an allocation!"""
+            )
+        
+        T_e, K_e = self.allocation_problem()
+
+        T_e_pseudo = np.transpose(T_e) @ (np.linalg.inv(T_e @ np.transpose(T_e)))
+
+        u_e = np.linalg.inv(K_e) @ T_e_pseudo @ tau_d
+
+        u = np.zeros(self.n_thrusters)
+        alpha = np.zeros(self.n_thrusters)
+
+        for i in range(self.n_thrusters):
+            u[i] = np.sqrt(u_e[i*2]**2 + u_e[i*2+1]**2)
+            alpha[i] = np.arctan2(u_e[i*2+1], u_e[i*2])
+        
+        return u, alpha
+
+
+class fixed_angle_allocator(AllocatorCSAD):
+
+    theta = np.deg2rad(30)
+
+    alpha = np.array([np.pi,
+             np.pi/2 + theta,
+             3 * np.pi/2 - theta,
+             - np.pi,
+             - np.pi/2 + theta,
+             np.pi/2 - theta])
+
+    def allocation_problem(self):
+        """
+        Assemble extended allocation problem into matrix form
+        """
+
+        K_lst = [thruster._K for thruster in self._thrusters]
+
+        lx = [thruster.pos_x for thruster in self._thrusters]
+        ly = [thruster.pos_y for thruster in self._thrusters]
+
+        K = np.diag(K_lst)
+        
+        T = np.array([
+            np.cos(self.alpha),
+            np.sin(self.alpha),
+            lx * np.sin(self.alpha) - ly * np.cos(self.alpha)])
+
+        return T, K
+
+    def allocate(self, tau_d):
+        """
+        Allocate global thrust vector to available thrusters. 
+        """
+
+        if self.n_thrusters == 0:
+            raise AllocationError(
+                """At least one thruster must be added
+                    to the
+                    allocator-object before attempting an allocation!"""
+            )
+        
+        T, K = self.allocation_problem()
+
+        B = T @ K
+
+        B_inv = np.transpose(B) @ (np.linalg.inv(B @ np.transpose(B)))
+
+        u = B_inv @ tau_d
+
+        alpha = self.alpha
+        
+        return u, alpha
```

### Comparing `MCSimPython-0.0.14/src/MCSimPython/utils.py` & `MCSimPython-0.1.1/src/MCSimPython/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,360 +1,390 @@
-# Utility functions
-
-# ----------------------------------------------------------------------------
-# This code is part of the MCSimPython toolbox and repository.
-# Created By: Jan-Erik Hygen
-# Created Date: 2022-10-12
-# Revised: 2023-02-09 Harald Mo    Add from/to 6 and 3DOF functions
-# 
-# Tested:  See tests/test_utils.py
-# 
-# Copyright (C) 202x: NTNU, Trondheim
-# Licensed under GPL-3.0-or-later
-# ---------------------------------------------------------------------------
-
-import numpy as np
-from time import time
-
-
-dof3_matrix_mask = np.ix_([0, 1, 5], [0, 1 ,5])
-dof3_array = np.ix_([0, 1, 5])
-
-def complex_to_polar(complex_values):
-    """Complex value to polar coordinates.
-    
-    Parameters
-    ----------
-    complex_values : flot, array_like
-        Complex value to be transformed.
-
-    Returns
-    -------
-    amp : float
-        Amplitude/radius
-    theta : float
-        Angle in rad.
-    """
-    complex_values = np.asarray_chkfinite(complex_values)
-    amp = np.abs(complex_values)
-    theta = np.angle(complex_values)
-    return amp, theta
-
-
-def polar_to_complex(amp, theta):
-    """Polar coordinate to complex value.
-    
-    The complex value is calculated from the polar
-    coordinates as 
-
-    .. math::
-       z = A (\\cos(\\theta) + j\\sin(\\theta))
-    
-    Parameters
-    ----------
-    amp : float
-        Amplitude/radius of polar value.
-    theta : float
-        Angle in radians.
-
-    Returns
-    -------
-    complex_value : complex
-        Complex value.
-    
-    Examples
-    --------
-
-    >>> from MCSimPython.utils import polar_to_complex
-    >>> amp, theta = 1.0, 0.0
-    >>> polar_to_complex(amp, theta)
-    (1 + 0j)
-    
-    >>> amp, theta = 1.0, np.pi
-    >>> polar_to_complex(amp, theta)
-    (-1 + 0j)
-
-    """
-    amp = np.asarray_chkfinite(amp)
-    theta = np.asarray_chkfinite(theta)
-    return amp*(np.cos(theta) + 1j * np.sin(theta))
-
-
-def pipi(theta):
-    """Return angle in range [-pi, pi).
-    
-    Parameters
-    ----------
-    theta : float, array_like
-        Angle in radians to be mapped to [-pi, pi).
-
-    Returns
-    -------
-    angle : float, array_like
-        Smallest signed angle in range [-pi, pi).
-
-    Examples
-    --------
-
-    >>> from MCSimPython.utils import pipi
-    >>> import numpy as np
-    >>> angle = 2*np.pi
-    >>> pipi(angle)
-    0.0
-
-    >>> angle = np.deg2rad(270)
-    >>> pipi(angle)
-    -1.570796
-
-    """
-    return np.mod(theta + np.pi, 2*np.pi) - np.pi
-
-
-def to_positive_angle(theta):
-    """Map angle from [-pi, pi) to [0, 2*pi).
-    
-    Parameters
-    ----------
-    theta : array_like
-        Angle in radians in [-pi, pi).
-    
-    Returns
-    -------
-    out : array_like
-        Angle in [0, 2*pi).
-
-    Note
-    ----
-    The function does not calculate the smallest
-    signed positive angle if the input is outside
-    [-pi, pi).
-
-    See Also
-    --------
-    MCSimPython.utils.pipi : 
-        Map angle to [-pi, pi).
-
-    Examples
-    --------
-
-    >>> from MCSimPython.utils import to_positive_angle
-    >>> import numpy as np
-    >>> angle = -np.pi
-    >>> to_positive_angle(angle)
-    array(3.14159265)
-    
-    Example of wrong use
-    
-    >>> angle = 2.5*np.pi # 7.85398163
-    >>> to_positive_angle(angle)
-    array(7.85398163)
-
-    Correct use for angle > 2pi
-
-    >>> from MCSimPython.utils import pipi
-    >>> angle = 2.5*np.pi
-    >>> to_positive_angle(pipi(angle))
-    array(1.57079633)
-
-    """
-    return np.where(theta < 0, theta + 2*np.pi, theta)
-
-
-def pipi2cont(psi, psi_prev):
-    """Lifting algorithm."""
-    arr = np.array([psi_prev, psi])
-    return np.unwrap(arr)[-1]
-
-
-def Rx(phi):
-    """3DOF Rotation matrix about x-axis."""
-    return np.array([
-        [1, 0, 0],
-        [0, np.cos(phi), -np.sin(phi)],
-        [0, np.sin(phi), np.cos(phi)]
-    ])
-
-
-def Ry(theta):
-    """3DOF Rotation matrix about y-axis."""
-    return np.array([
-        [np.cos(theta), 0, np.sin(theta)],
-        [0, 1, 0],
-        [-np.sin(theta), 0, np.cos(theta)]
-    ])
-
-
-def Rz(psi):
-    """3DOF Rotation matrix about z-axis."""
-    return np.array([
-        [np.cos(psi), -np.sin(psi), 0],
-        [np.sin(psi), np.cos(psi), 0],
-        [0, 0, 1]
-    ])
-
-
-def Rzyx(eta):
-    """Full roation matrix."""
-    phi = eta[3]
-    theta = eta[4]
-    psi = eta[5]
-    return Rz(psi)@Ry(theta)@Rx(phi)
-
-
-def Tzyx(eta):
-    phi = eta[3]
-    theta = eta[4]
-    psi = eta[5]
-    return np.array([
-        [1, np.sin(phi)*np.tan(theta), np.cos(phi)*np.tan(theta)],
-        [0, np.cos(phi), -np.sin(phi)],
-        [0, np.sin(phi)/np.cos(theta), np.cos(phi)/np.cos(theta)]
-    ])
-
-
-def J(eta):
-    """6 DOF rotation matrix."""
-    phi = eta[3]
-    theta = eta[4]
-    psi = eta[5]
-
-    return np.block([
-        [Rzyx(eta), np.zeros((3, 3))],
-        [np.zeros((3, 3)), Tzyx(eta)]
-    ])
-
-
-def Smat(x):
-    """
-    Skew-symmetric cross-product operator matrix.
-
-    Parameters
-    ----------
-    x: 3x1-array
-
-    Return
-    ------
-    S: 3x3-array
-    """
-    return np.array([
-        [0, -x[2], x[1]],
-        [x[2], 0, -x[0]],
-        [-x[1], x[0], 0]
-    ])
-
-
-def three2sixDOF(v):
-    """3 to 6 DOF conversion.
-    
-    Converts a vector a matrix from 3DOF
-    to 6DOF.
-
-    Parameters
-    ----------
-    v : array_like
-        Vector or matrix to be converted.
-
-    Returns
-    -------
-    out : array_like
-        Vector (6,1) or matrix (6, 6) array.
-    """
-    if v.ndim == 2:   # Matrix
-        v = np.concatenate(v, axis=None)
-        v = np.concatenate((v[0:2], np.zeros(3), v[2:5], np.zeros(3), v[5], np.zeros(18), v[6:8], np.zeros(3), v[8]), axis=None).reshape((6,6))
-    elif v.ndim == 1: # Vector
-        v = np.array([v[0], v[1], 0, 0, 0, v[2]])
-    return v
-
-def six2threeDOF(v):
-    """6 to 3 DOF conversion.
-    
-    Convert a 6DOF vecor or matrix to 3DOF.
-
-    Parameters
-    ----------
-    v : array_like
-        6 DOF vector or matrix to be converted to 3DOF.
-    
-    Returns
-    -------
-    out : array_like
-        Vector (3,1) or matrix (3,3) array.
-    """
-    if v.ndim == 2:   # Matrix
-        i = np.ix_([0,1,5],[0,1,5])
-        v = v[i]  
-    elif v.ndim == 1: # Vector
-        i = np.ix_([0,1,5])  
-        v = v[i]
-    return v
-
-
-
-def timeit(func):
-    """
-    Decorator for measuring execution time of function.
-
-    Print the execution time of a function. (Mainly for
-    debugging and analyzis purposes).
-
-    Parameters
-    ----------
-    func : function
-        Function to be timed.
-
-    
-    Examples
-    --------
-    >>> from MCSimPython.utils import timeit
-    >>> @timeit
-    ... def loop(n):
-    ...     for i in range(n):
-    ...         print(i)
-    ...
-    >>> loop(5)
-    0
-    1
-    2
-    3
-    4
-    Execution time of loop: 0.004         
-
-    """
-    def wrapper(*args, **kwargs):
-        t1 = time()
-        results = func(*args, **kwargs)
-        t2 = time()
-        print(f"Execution time of {func.__name__}: {(t2 - t1):.4f}")
-        return results
-    return wrapper
-
-
-def rigid_body_transform(r, eta, in_ned=True):
-    """Calculate the relative motion of a point r different from the COG.
-
-    The calculation assumes small angles (s.t. cos(theta)=0 and sin(theta)=theta)
-    and is computed as:
-
-    ``s = (\eta_1, \eta_2, \eta_3)^T + (\eta_4, \eta_5, \eta_6) x (r_x, r_y, r_z)``
-    
-    Parameters
-    ----------
-    r : array_like
-        Lever arm from COG to point of interest
-    eta : array_like
-        6DOF vessel pose (surge, sway, heave, roll, pitch, yaw)
-    in_ned : bool (default = False)
-        Reference frame definition of eta. If True, the vessel
-        pose eta is assumed to be defined in the NED-frame. If False
-        eta is assumed to be defined in body-frame.
-
-    Returns
-    -------
-    s : array_like
-        Translation vector which is the same as (delta_x, delta_y, delta_z).
-    """
-
-    if in_ned:
-        eta = np.copy(np.linalg.inv(J(eta))@eta)
-        print(eta)
-    return eta[:3] + np.cross(eta[3:], r)
+# Utility functions
+
+# ----------------------------------------------------------------------------
+# This code is part of the MCSimPython toolbox and repository.
+# Created By: Jan-Erik Hygen
+# Created Date: 2022-10-12
+# Revised: 2023-02-09 Harald Mo    Add from/to 6 and 3DOF functions
+# 
+# Tested:  See tests/test_utils.py
+# 
+# Copyright (C) 202x: NTNU, Trondheim
+# Licensed under GPL-3.0-or-later
+# ---------------------------------------------------------------------------
+
+import numpy as np
+from time import time
+from scipy.signal import welch
+
+
+dof3_matrix_mask = np.ix_([0, 1, 5], [0, 1 ,5])
+dof3_array = np.ix_([0, 1, 5])
+
+def complex_to_polar(complex_values):
+    """Complex value to polar coordinates.
+    
+    Parameters
+    ----------
+    complex_values : flot, array_like
+        Complex value to be transformed.
+
+    Returns
+    -------
+    amp : float
+        Amplitude/radius
+    theta : float
+        Angle in rad.
+    """
+    complex_values = np.asarray_chkfinite(complex_values)
+    amp = np.abs(complex_values)
+    theta = np.angle(complex_values)
+    return amp, theta
+
+
+def polar_to_complex(amp, theta):
+    """Polar coordinate to complex value.
+    
+    The complex value is calculated from the polar
+    coordinates as 
+
+    .. math::
+       z = A (\\cos(\\theta) + j\\sin(\\theta))
+    
+    Parameters
+    ----------
+    amp : float
+        Amplitude/radius of polar value.
+    theta : float
+        Angle in radians.
+
+    Returns
+    -------
+    complex_value : complex
+        Complex value.
+    
+    Examples
+    --------
+
+    >>> from MCSimPython.utils import polar_to_complex
+    >>> amp, theta = 1.0, 0.0
+    >>> polar_to_complex(amp, theta)
+    (1 + 0j)
+    
+    >>> amp, theta = 1.0, np.pi
+    >>> polar_to_complex(amp, theta)
+    (-1 + 0j)
+
+    """
+    amp = np.asarray_chkfinite(amp)
+    theta = np.asarray_chkfinite(theta)
+    return amp*(np.cos(theta) + 1j * np.sin(theta))
+
+
+def pipi(theta):
+    """Return angle in range [-pi, pi).
+    
+    Parameters
+    ----------
+    theta : float, array_like
+        Angle in radians to be mapped to [-pi, pi).
+
+    Returns
+    -------
+    angle : float, array_like
+        Smallest signed angle in range [-pi, pi).
+
+    Examples
+    --------
+
+    >>> from MCSimPython.utils import pipi
+    >>> import numpy as np
+    >>> angle = 2*np.pi
+    >>> pipi(angle)
+    0.0
+
+    >>> angle = np.deg2rad(270)
+    >>> pipi(angle)
+    -1.570796
+
+    """
+    return np.mod(theta + np.pi, 2*np.pi) - np.pi
+
+
+def to_positive_angle(theta):
+    """Map angle from [-pi, pi) to [0, 2*pi).
+    
+    Parameters
+    ----------
+    theta : array_like
+        Angle in radians in [-pi, pi).
+    
+    Returns
+    -------
+    out : array_like
+        Angle in [0, 2*pi).
+
+    Note
+    ----
+    The function does not calculate the smallest
+    signed positive angle if the input is outside
+    [-pi, pi).
+
+    See Also
+    --------
+    MCSimPython.utils.pipi : 
+        Map angle to [-pi, pi).
+
+    Examples
+    --------
+
+    >>> from MCSimPython.utils import to_positive_angle
+    >>> import numpy as np
+    >>> angle = -np.pi
+    >>> to_positive_angle(angle)
+    array(3.14159265)
+    
+    Example of wrong use
+    
+    >>> angle = 2.5*np.pi # 7.85398163
+    >>> to_positive_angle(angle)
+    array(7.85398163)
+
+    Correct use for angle > 2pi
+
+    >>> from MCSimPython.utils import pipi
+    >>> angle = 2.5*np.pi
+    >>> to_positive_angle(pipi(angle))
+    array(1.57079633)
+
+    """
+    return np.where(theta < 0, theta + 2*np.pi, theta)
+
+
+def pipi2cont(psi, psi_prev):
+    """Lifting algorithm."""
+    arr = np.array([psi_prev, psi])
+    return np.unwrap(arr)[-1]
+
+
+def Rx(phi):
+    """3DOF Rotation matrix about x-axis."""
+    return np.array([
+        [1, 0, 0],
+        [0, np.cos(phi), -np.sin(phi)],
+        [0, np.sin(phi), np.cos(phi)]
+    ])
+
+
+def Ry(theta):
+    """3DOF Rotation matrix about y-axis."""
+    return np.array([
+        [np.cos(theta), 0, np.sin(theta)],
+        [0, 1, 0],
+        [-np.sin(theta), 0, np.cos(theta)]
+    ])
+
+
+def Rz(psi):
+    """3DOF Rotation matrix about z-axis."""
+    return np.array([
+        [np.cos(psi), -np.sin(psi), 0],
+        [np.sin(psi), np.cos(psi), 0],
+        [0, 0, 1]
+    ])
+
+
+def Rzyx(eta):
+    """Full roation matrix."""
+    phi = eta[3]
+    theta = eta[4]
+    psi = eta[5]
+    return Rz(psi)@Ry(theta)@Rx(phi)
+
+
+def Tzyx(eta):
+    phi = eta[3]
+    theta = eta[4]
+    psi = eta[5]
+    return np.array([
+        [1, np.sin(phi)*np.tan(theta), np.cos(phi)*np.tan(theta)],
+        [0, np.cos(phi), -np.sin(phi)],
+        [0, np.sin(phi)/np.cos(theta), np.cos(phi)/np.cos(theta)]
+    ])
+
+
+def J(eta):
+    """6 DOF rotation matrix."""
+    phi = eta[3]
+    theta = eta[4]
+    psi = eta[5]
+
+    return np.block([
+        [Rzyx(eta), np.zeros((3, 3))],
+        [np.zeros((3, 3)), Tzyx(eta)]
+    ])
+
+
+def Smat(x):
+    """
+    Skew-symmetric cross-product operator matrix.
+
+    Parameters
+    ----------
+    x: 3x1-array
+
+    Return
+    ------
+    S: 3x3-array
+    """
+    return np.array([
+        [0, -x[2], x[1]],
+        [x[2], 0, -x[0]],
+        [-x[1], x[0], 0]
+    ])
+
+
+def three2sixDOF(v):
+    """3 to 6 DOF conversion.
+    
+    Converts a vector a matrix from 3DOF
+    to 6DOF.
+
+    Parameters
+    ----------
+    v : array_like
+        Vector or matrix to be converted.
+
+    Returns
+    -------
+    out : array_like
+        Vector (6,1) or matrix (6, 6) array.
+    """
+    if v.ndim == 2:   # Matrix
+        v = np.concatenate(v, axis=None)
+        v = np.concatenate((v[0:2], np.zeros(3), v[2:5], np.zeros(3), v[5], np.zeros(18), v[6:8], np.zeros(3), v[8]), axis=None).reshape((6,6))
+    elif v.ndim == 1: # Vector
+        v = np.array([v[0], v[1], 0, 0, 0, v[2]])
+    return v
+
+def six2threeDOF(v):
+    """6 to 3 DOF conversion.
+    
+    Convert a 6DOF vecor or matrix to 3DOF.
+
+    Parameters
+    ----------
+    v : array_like
+        6 DOF vector or matrix to be converted to 3DOF.
+    
+    Returns
+    -------
+    out : array_like
+        Vector (3,1) or matrix (3,3) array.
+    """
+    if v.ndim == 2:   # Matrix
+        i = np.ix_([0,1,5],[0,1,5])
+        v = v[i]  
+    elif v.ndim == 1: # Vector
+        i = np.ix_([0,1,5])  
+        v = v[i]
+    return v
+
+
+
+def timeit(func):
+    """
+    Decorator for measuring execution time of function.
+
+    Print the execution time of a function. (Mainly for
+    debugging and analyzis purposes).
+
+    Parameters
+    ----------
+    func : function
+        Function to be timed.
+
+    
+    Examples
+    --------
+    >>> from MCSimPython.utils import timeit
+    >>> @timeit
+    ... def loop(n):
+    ...     for i in range(n):
+    ...         print(i)
+    ...
+    >>> loop(5)
+    0
+    1
+    2
+    3
+    4
+    Execution time of loop: 0.004         
+
+    """
+    def wrapper(*args, **kwargs):
+        t1 = time()
+        results = func(*args, **kwargs)
+        t2 = time()
+        print(f"Execution time of {func.__name__}: {(t2 - t1):.4f}")
+        return results
+    return wrapper
+
+
+def rigid_body_transform(r, eta, in_ned=True):
+    """Calculate the relative motion of a point r different from the COG.
+
+    The calculation assumes small angles (s.t. cos(theta)=0 and sin(theta)=theta)
+    and is computed as:
+
+    ``s = (\eta_1, \eta_2, \eta_3)^T + (\eta_4, \eta_5, \eta_6) x (r_x, r_y, r_z)``
+    
+    Parameters
+    ----------
+    r : array_like
+        Lever arm from COG to point of interest
+    eta : array_like
+        6DOF vessel pose (surge, sway, heave, roll, pitch, yaw)
+    in_ned : bool (default = False)
+        Reference frame definition of eta. If True, the vessel
+        pose eta is assumed to be defined in the NED-frame. If False
+        eta is assumed to be defined in body-frame.
+
+    Returns
+    -------
+    s : array_like
+        Translation vector which is the same as (delta_x, delta_y, delta_z).
+    """
+
+    if in_ned:
+        eta = np.copy(np.linalg.inv(J(eta))@eta)
+        print(eta)
+    return eta[:3] + np.cross(eta[3:], r)
+
+
+def power_spectral_density(timeseries, fs, freq_hz=False, nperseg=2**11):
+    """Compute the Power Spectral Density (PSD) of a timeseries.
+    
+    The PSD is calculated using scipy.signals.welch
+
+    Parameters
+    ----------
+    timerseries : array_like
+        Timeseries array.
+    fs : int
+        Sampling frequency
+    freq_hz : bool (optional)
+        Calculate the PSD in [hz]. Defaults to False.
+    nperseg : float (optional)
+        Number of points per segments used in the scipy.signal.welch function.
+    
+    Returns
+    -------
+    f : array_like
+        Frequencies in PSD. Returned as [rad/s] if freq_hz=False.
+    PSD : array_like
+        PSD of timeseries. Returned as [unit/(rad/s)] if freq_hz=False
+    """
+    f, S_f = welch(timeseries, fs=fs, nperseg=nperseg)
+    if not freq_hz:
+        return f*2*np.pi, S_f/(2*np.pi)
+    return f, S_f
```

### Comparing `MCSimPython-0.0.14/src/MCSimPython/vessel_data/CSAD/vesselABC_json.json` & `MCSimPython-0.1.1/src/MCSimPython/vessel_data/CSAD/vesselABC_json.json`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.0.14/src/MCSimPython/vessel_data/CSAD/vessel_json.json` & `MCSimPython-0.1.1/src/MCSimPython/vessel_data/CSAD/vessel_json.json`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.0.14/src/MCSimPython/vessel_data/gunnerus/gunnerus_veres.json` & `MCSimPython-0.1.1/src/MCSimPython/vessel_data/gunnerus/gunnerus_veres.json`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.0.14/src/MCSimPython/vessel_data/gunnerus/parV_RVG3DOF.pkl` & `MCSimPython-0.1.1/src/MCSimPython/vessel_data/gunnerus/parV_RVG3DOF.pkl`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.0.14/src/MCSimPython/vessel_data/gunnerus/parV_RVG6DOF.pkl` & `MCSimPython-0.1.1/src/MCSimPython/vessel_data/gunnerus/parV_RVG6DOF.pkl`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.0.14/src/MCSimPython/vessel_data/gunnerus/vessel.json` & `MCSimPython-0.1.1/src/MCSimPython/vessel_data/gunnerus/vessel.json`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.0.14/src/MCSimPython/vessel_data/gunnerus/vessel_2.json` & `MCSimPython-0.1.1/src/MCSimPython/vessel_data/gunnerus/vessel_2.json`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.0.14/src/MCSimPython/waves/wave_spectra.py` & `MCSimPython-0.1.1/src/MCSimPython/waves/wave_spectra.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,402 +1,402 @@
-# Wave spectra
-
-# ----------------------------------------------------------------------------
-# This code is part of the MCSimPython toolbox and repository.
-# Created By: Jan-Erik Hygen
-# Created Date: 2022-10-11
-# Revised: 2022-10-19 Jan-Erik Hygen    Add 2d spectrum functionality.
-#          2022-10-27 Jan-Erik Hygen    Add spreading function.
-# 
-# Copyright (C) 2023: NTNU, Trondheim
-# Licensed under GPL-3.0-or-later
-# ---------------------------------------------------------------------------
-
-import numpy as np
-from abc import ABC, abstractclassmethod
-
-
-class BaseSpectrum(ABC):
-    """
-    Base class for 1-D Wave Spectra.
-
-    Parameters
-    ----------
-    freq : 1-D array
-        Frequencies of wave spectrum
-    freq_hz : bool
-        Boolean to define spectrum in either rad/s (false) or Hz (true)
-    """
-
-    def __init__(self, freq, freq_hz=False):
-        self._freq = freq
-        self._freq_hz = freq_hz
-
-        if self._freq_hz:
-            self._freq *= 2*np.pi
-        
-
-    def __call__(self, *args, freq_hz=None, **kwargs):
-        freq = self._freq.copy()
-        spectrum = self._spectrum(freq, *args, **kwargs)
-
-        return freq, spectrum
-
-    def moment(self, n, *args, **kwargs):
-        """Calculate n-th spectral moment."""
-        freq, spec = self.__call__(*args, **kwargs)
-        return np.trapz(freq**n * spec, freq)
-
-
-    def realization(self, time, *args, **kwargs):
-        """Generate a wave realization from wave spectrum at a fixed position.
-
-        Parameters
-        ----------
-        time : 1D-array
-            Array of time points used in realization
-        *args : tuple
-            Additional arguments should be passed as keyword arguments
-        **kwargs : dict
-            Wave spectrum parameters like hs and tp, include gamma for JONSWAP wave spectrum.
-        
-        Return
-        ------
-        timeseries : 1D-array
-            Array of wave elevation at different time instances for a fixed point (x=0).
-        """
-        
-        freq, spectrum = self.__call__(*args, **kwargs)
-        dw = freq[1]-freq[0]
-        amp = np.sqrt(2*spectrum*dw)
-        eps = np.random.uniform(0, 2*np.pi, size=len(amp))
-        return np.sum(amp * np.cos(freq*time[:, None] + eps), axis=1)
-
-
-    @abstractclassmethod
-    def _spectrum(self, omega, *args, **kwargs):
-        raise NotImplementedError
-
-
-class BasePMSpectrum(BaseSpectrum):
-
-    def __call__(self, A, B, freq_hz=None):
-        return super().__call__(A, B, freq_hz=freq_hz)
-    
-    def _spectrum(self, omega, A, B):
-        return A/omega**5 * np.exp(-B/omega**4)
-
-
-class ModifiedPiersonMoskowitz(BasePMSpectrum):
-
-    def __call__(self, hs, tp, freq_hz=None):
-        """Generate a Modified Pierson-Moskowitz wave spectrum.
-
-        Parameters
-        ----------
-        hs : float
-            Significant wave height
-        tp : float
-            Peak period of wave spectrum
-        freq_hz : bool
-            Wave spectrum and frequencies in Hz or rad/s.
-
-        Return
-        ------
-        freq : 1D-array
-            Array of frequencies in wave spectrum
-        spectrum : 1D-array
-            1D Modified Pierson-Moskowitz wave spectrum
-        """
-
-        A = self._A(hs, tp)
-        B = self._B(tp)
-
-        return super().__call__(A, B, freq_hz=freq_hz)
-
-    def _A(self, hs, tp):
-        wp = 2*np.pi / tp
-        return (5.0/16.0) * hs**2 * wp**4
-
-    def _B(self, tp):
-        wp = 2*np.pi / tp
-        return (5.0/4.0) * wp**4
-
-
-class JONSWAP(ModifiedPiersonMoskowitz):
-
-    def __call__(self, hs, tp, gamma=1, freq_hz=None):
-        """Generate a JONSWAP wave spectrum.
-
-        Parameters
-        ----------
-        hs : float
-            Significant wave heihgt
-        tp : float
-            Peak period of wave spectrum
-        gamma : float
-            Steapness factor
-        freq_hz : bool, default=False
-            Frequency in Hz or rad/s
-
-        Return
-        ------
-        freq : 1D-array
-            Frequencies of wave spectrum
-        spectrum : 1D-array
-            1D JONSWAP wave spectrum
-        """
-
-        freq, pm_spectrum = super().__call__(hs, tp, freq_hz=freq_hz)
-
-        alpha = self._alpha(gamma)
-        b = self._b(tp)
-        
-        return freq, alpha * pm_spectrum * gamma**b
-
-    def _alpha(self, gamma):
-        return 1 - 0.287 * np.log(gamma)
-
-    def _b(self, tp):
-        wp = 2*np.pi / tp
-        sigma = self._sigma(wp)
-        return np.exp(-0.5 * ((self._freq - wp) / (sigma*wp))**2)
-
-    def _sigma(self, wp):
-        # Set conditional parameter sigma used in JONSWAP spectrum.
-        arg = self._freq <= wp
-        sigma = np.empty_like(self._freq)
-        sigma[arg] = 0.07
-        sigma[~arg] = 0.09
-        return sigma
-
-
-
-class DirectionalSpectrum():
-    
-    """
-    Directional Wave Spectrum class. 
-
-    Attributes
-    ----------
-    _freq : 1D-array
-        Array of frequencies for wave spectrum
-    _angles : 1D-array
-        Array of angles for spreading function of wave spectrum    
-    _theta_p : float
-        Peak angle for spreading function
-    _spectrum : 1D-array
-        Array of one-dimensional wave spectrum values for frequencies _freq.
-    _s : int (default = 1)
-        Peakness parameter of spreading functing. Must be large than or equal to 1.
-    _spreading : 1D-array
-        Spreading function for angles _angles.
-    _dw : float
-        Frequency steps
-    _dtheta : float
-        Angle step
-    _g : float
-        Gravitational acceleration constant
-    _eps : 2D-array
-        Array of random phases for wave component j, k. Where j <= len(freq) and k <= len(angles).
-     
-    Methods
-    -------
-
-    """
-
-    def __init__(self, freqs, angles, theta_p, spectrum, s=1, seed=12345):
-        self._freq = freqs
-        self._angles = angles
-        self._spectrum = spectrum
-        self._theta_p = theta_p
-        self._spreading = self._spread_func(s=s)
-        self._dw = (freqs[-1] - freqs[0])/len(freqs)
-        self._dtheta = (angles[-1] - angles[0])/len(angles)
-        self._g = 9.81
-        self._seed = seed
-        np.random.seed(seed)
-        self._eps = np.random.uniform(0, 2*np.pi, size=(len(freqs), len(angles)))
-
-    
-    def _spread_func(self, s=1):
-        """
-        Cosine spreading function.
-
-        Parameters
-        ----------
-        theta : 1D-array
-            Angles in spreading function.
-        theta_p : float
-            Peak angle for spreading function. (Dominant wave direction).
-        s : int (default = 1)
-            Steapness value to determine amount of spreading. Must be equal or large than 1.
-
-        Return
-        ------
-        spreading : 1D-array
-            Spreading function for the given angles, peak angles and steapness value.
-        """
-        d_theta = self._angles - self._theta_p
-        state = np.abs(d_theta) < np.pi/2
-        spreading = 2**(2*s - 1) * np.math.factorial(s)*np.math.factorial(s-1)/(np.pi*np.math.factorial(2*s-1)) * np.cos(d_theta)**(2*s)
-        spreading[~state] = 0
-        return spreading
-
-    def spectrum2d(self):
-        """
-        Calculate the two-dimensional directional wave spectrum.
-
-        Return
-        ------
-        F : 2D-array
-            Frequencies in meshgrid
-        T : 2D-array
-            Theta angle in meshgrid
-        spec2d : 2D-array
-            Directional wave spectrum for frequencies and angles.
-        """
-
-        F, T = np.meshgrid(self._freq, self._angles)
-        spec2d = self._spectrum*self._spreading[:, None]
-        self._spectrum2d = spec2d
-        return F, T, spec2d
-
-    def wave_realization(self, time, x, y):
-        """
-        Generate a 2D Multidirectional wavefield
-
-        Parameters
-        ----------
-        time : 1D-array
-            Array of time instances
-        x : 1D-array
-            Array of x-positions
-        y : 1D-array
-            Array of y-positions
-        
-        Return
-        ------
-        X : 2D-array
-            x values in meshgrid
-        Y : 2D-array
-            y values in meshgrid
-        wave_elevation : 2D-array
-            Wave elevation at position (x, y) at time t.
-        """
-
-        X, Y = np.meshgrid(x, y) # Create meshgrid
-        wave_elevation = 0
-
-        for j in range(len(self._freq)):
-            k_j = self._freq[j]**2 / self._g
-            for k in range(len(self._angles)):
-                theta = self._angles[k]
-                # eps_jk = np.random.uniform(0, 2*np.pi)
-                amplitude = np.sqrt(2*self._spectrum2d[k, j] * self._dw * self._dtheta)
-                wave_elevation += amplitude*np.sin(self._freq[j]*time - k_j*X*np.cos(theta) - k_j*Y*np.sin(theta) + self._eps[j, k])
-                
-        return X, Y, wave_elevation
-
-
-
-
-if __name__ == "__main__":
-    # Simple How-To for wave module
-    import doctest
-    doctest.testmod()
-    import matplotlib.pyplot as plt
-    from matplotlib import cm
-    plt.rcParams.update({
-        'figure.figsize': (12, 4),
-        'font.size': 14,
-        'lines.linewidth': 1.4
-    })
-
-    hs = 2.0
-    tp = 9.5
-    wp = 2*np.pi / tp
-    gamma = 5
-
-    wmin = wp - wp/2
-    wmax = 2*wp
-    N = 20
-    w = np.linspace(wmin, wmax, N)
-
-    pm_spectrum = ModifiedPiersonMoskowitz(w)       # Instantiate MPM spectrum object
-    jonswap_spectrum = JONSWAP(w)                   # Instantiate Jonwswap spectrum object
-
-    # Calculate the zero-moment for both spectra.
-    m0_jonswap = jonswap_spectrum.moment(n=0, hs=hs, tp=tp, gamma=gamma)
-    m0_pm = pm_spectrum.moment(n=0, hs=hs, tp=tp)
-
-    print(f"JONSWAP: Hs = {4*np.sqrt(m0_jonswap):.2f} [m]")
-    print(f"PM: Hs = {4*np.sqrt(m0_pm):.2f} [m]")
-    
-    # plt.plot(*pm_spectrum(hs, tp), label="PM")
-    # plt.plot(*jonswap_spectrum(hs, tp, gamma), label="JONSWAP")
-    # plt.grid()
-    # plt.legend()
-    # plt.show()
-
-    freq, spectrum = jonswap_spectrum(hs, tp, gamma)
-
-    time = np.arange(0, 500, 0.1)
-
-    jonswap_realizatin = jonswap_spectrum.realization(time, hs=hs, tp=tp, gamma=gamma)
-    pm_realizatino = pm_spectrum.realization(time, hs=hs, tp=tp)
-
-    # plt.plot(time, pm_spectrum.realization(time, hs=hs, tp=tp))
-    # plt.plot(time, jonswap_spectrum.realization(time, hs=hs, tp=tp, gamma=gamma))
-    # plt.xlim(time[0], time[-1])
-    # plt.ylim(-6*np.sqrt(m0_jonswap), 6*np.sqrt(m0_jonswap))
-    # plt.show()
-
-    theta0 = np.pi/36
-    s=2
-    psi = np.linspace(-np.pi, np.pi, 15)
-    dir_spectra = DirectionalSpectrum(w, psi, theta_p=theta0, spectrum=spectrum, s=s)
-    F, T, spectrum2d = dir_spectra.spectrum2d()
-
-    fig = plt.figure(figsize=(16, 8))
-    ax = plt.axes(projection='3d')
-    ax.view_init(35, 40)
-    ax.plot_surface(F, T, spectrum2d, cmap=cm.coolwarm)
-    ax.set_xlabel(r"$\omega \; [\frac{rad}{s}]$")
-    ax.set_ylabel(r"$\psi \; [deg]$")
-    plt.show()
-
-    Nxy = 400
-    x = np.linspace(-150, 150, Nxy)
-    y = np.linspace(-150, 150, Nxy)
-    X, Y, realization_2d = dir_spectra.wave_realization(0, x, y)
-
-    def update3d(t, plot, x, y):
-        # Callback function for animation.
-        plot[0].remove()
-        _, _, wave = dir_spectra.wave_realization(t, x, y)
-        plot[0] = ax.plot_surface(X, Y, wave, cmap=cm.coolwarm)
-
-    fig = plt.figure(figsize=(16, 8))
-    ax = fig.add_subplot(111, projection="3d")
-    ax.view_init(30, 40)
-    # ax.plot_surface(X, Y, realization_2d, cmap=cm.coolwarm)
-    ax.set_zlim([-2*hs, 2*hs])
-    ax.set_xlabel("$x \, [m]$")
-    ax.set_ylabel("$y \, [m]$")
-    ax.set_zlabel("$\zeta \, [m]$")
-    
-    fps = 32
-
-    plot = [ax.plot_surface(X, Y, realization_2d, cmap=cm.coolwarm)]
-
-    from matplotlib.animation import FuncAnimation
-    
-    from datetime import datetime
-
-    duration = 20
-    t_start = datetime.now()
-    w_anim = FuncAnimation(fig, update3d, frames=np.linspace(0, duration, (duration*fps)), fargs=(plot, x, y,))
-    w_anim.save(f'wave_realization_disc{Nxy}_hs{hs:.2f}_tp{tp:.2f}_dir{np.rad2deg(theta0):.0f}_s{s:.0f}_{duration}_gamma{gamma:.1f}_sec.mp4', fps=fps, dpi=50)
-    t_end = datetime.now()
-
+# Wave spectra
+
+# ----------------------------------------------------------------------------
+# This code is part of the MCSimPython toolbox and repository.
+# Created By: Jan-Erik Hygen
+# Created Date: 2022-10-11
+# Revised: 2022-10-19 Jan-Erik Hygen    Add 2d spectrum functionality.
+#          2022-10-27 Jan-Erik Hygen    Add spreading function.
+# 
+# Copyright (C) 2023: NTNU, Trondheim
+# Licensed under GPL-3.0-or-later
+# ---------------------------------------------------------------------------
+
+import numpy as np
+from abc import ABC, abstractclassmethod
+
+
+class BaseSpectrum(ABC):
+    """
+    Base class for 1-D Wave Spectra.
+
+    Parameters
+    ----------
+    freq : 1-D array
+        Frequencies of wave spectrum
+    freq_hz : bool
+        Boolean to define spectrum in either rad/s (false) or Hz (true)
+    """
+
+    def __init__(self, freq, freq_hz=False):
+        self._freq = freq
+        self._freq_hz = freq_hz
+
+        if self._freq_hz:
+            self._freq *= 2*np.pi
+        
+
+    def __call__(self, *args, freq_hz=None, **kwargs):
+        freq = self._freq.copy()
+        spectrum = self._spectrum(freq, *args, **kwargs)
+
+        return freq, spectrum
+
+    def moment(self, n, *args, **kwargs):
+        """Calculate n-th spectral moment."""
+        freq, spec = self.__call__(*args, **kwargs)
+        return np.trapz(freq**n * spec, freq)
+
+
+    def realization(self, time, *args, **kwargs):
+        """Generate a wave realization from wave spectrum at a fixed position.
+
+        Parameters
+        ----------
+        time : 1D-array
+            Array of time points used in realization
+        *args : tuple
+            Additional arguments should be passed as keyword arguments
+        **kwargs : dict
+            Wave spectrum parameters like hs and tp, include gamma for JONSWAP wave spectrum.
+        
+        Return
+        ------
+        timeseries : 1D-array
+            Array of wave elevation at different time instances for a fixed point (x=0).
+        """
+        
+        freq, spectrum = self.__call__(*args, **kwargs)
+        dw = freq[1]-freq[0]
+        amp = np.sqrt(2*spectrum*dw)
+        eps = np.random.uniform(0, 2*np.pi, size=len(amp))
+        return np.sum(amp * np.cos(freq*time[:, None] + eps), axis=1)
+
+
+    @abstractclassmethod
+    def _spectrum(self, omega, *args, **kwargs):
+        raise NotImplementedError
+
+
+class BasePMSpectrum(BaseSpectrum):
+
+    def __call__(self, A, B, freq_hz=None):
+        return super().__call__(A, B, freq_hz=freq_hz)
+    
+    def _spectrum(self, omega, A, B):
+        return A/omega**5 * np.exp(-B/omega**4)
+
+
+class ModifiedPiersonMoskowitz(BasePMSpectrum):
+
+    def __call__(self, hs, tp, freq_hz=None):
+        """Generate a Modified Pierson-Moskowitz wave spectrum.
+
+        Parameters
+        ----------
+        hs : float
+            Significant wave height
+        tp : float
+            Peak period of wave spectrum
+        freq_hz : bool
+            Wave spectrum and frequencies in Hz or rad/s.
+
+        Return
+        ------
+        freq : 1D-array
+            Array of frequencies in wave spectrum
+        spectrum : 1D-array
+            1D Modified Pierson-Moskowitz wave spectrum
+        """
+
+        A = self._A(hs, tp)
+        B = self._B(tp)
+
+        return super().__call__(A, B, freq_hz=freq_hz)
+
+    def _A(self, hs, tp):
+        wp = 2*np.pi / tp
+        return (5.0/16.0) * hs**2 * wp**4
+
+    def _B(self, tp):
+        wp = 2*np.pi / tp
+        return (5.0/4.0) * wp**4
+
+
+class JONSWAP(ModifiedPiersonMoskowitz):
+
+    def __call__(self, hs, tp, gamma=1, freq_hz=None):
+        """Generate a JONSWAP wave spectrum.
+
+        Parameters
+        ----------
+        hs : float
+            Significant wave heihgt
+        tp : float
+            Peak period of wave spectrum
+        gamma : float
+            Steapness factor
+        freq_hz : bool, default=False
+            Frequency in Hz or rad/s
+
+        Return
+        ------
+        freq : 1D-array
+            Frequencies of wave spectrum
+        spectrum : 1D-array
+            1D JONSWAP wave spectrum
+        """
+
+        freq, pm_spectrum = super().__call__(hs, tp, freq_hz=freq_hz)
+
+        alpha = self._alpha(gamma)
+        b = self._b(tp)
+        
+        return freq, alpha * pm_spectrum * gamma**b
+
+    def _alpha(self, gamma):
+        return 1 - 0.287 * np.log(gamma)
+
+    def _b(self, tp):
+        wp = 2*np.pi / tp
+        sigma = self._sigma(wp)
+        return np.exp(-0.5 * ((self._freq - wp) / (sigma*wp))**2)
+
+    def _sigma(self, wp):
+        # Set conditional parameter sigma used in JONSWAP spectrum.
+        arg = self._freq <= wp
+        sigma = np.empty_like(self._freq)
+        sigma[arg] = 0.07
+        sigma[~arg] = 0.09
+        return sigma
+
+
+
+class DirectionalSpectrum():
+    
+    """
+    Directional Wave Spectrum class. 
+
+    Attributes
+    ----------
+    _freq : 1D-array
+        Array of frequencies for wave spectrum
+    _angles : 1D-array
+        Array of angles for spreading function of wave spectrum    
+    _theta_p : float
+        Peak angle for spreading function
+    _spectrum : 1D-array
+        Array of one-dimensional wave spectrum values for frequencies _freq.
+    _s : int (default = 1)
+        Peakness parameter of spreading functing. Must be large than or equal to 1.
+    _spreading : 1D-array
+        Spreading function for angles _angles.
+    _dw : float
+        Frequency steps
+    _dtheta : float
+        Angle step
+    _g : float
+        Gravitational acceleration constant
+    _eps : 2D-array
+        Array of random phases for wave component j, k. Where j <= len(freq) and k <= len(angles).
+     
+    Methods
+    -------
+
+    """
+
+    def __init__(self, freqs, angles, theta_p, spectrum, s=1, seed=12345):
+        self._freq = freqs
+        self._angles = angles
+        self._spectrum = spectrum
+        self._theta_p = theta_p
+        self._spreading = self._spread_func(s=s)
+        self._dw = (freqs[-1] - freqs[0])/len(freqs)
+        self._dtheta = (angles[-1] - angles[0])/len(angles)
+        self._g = 9.81
+        self._seed = seed
+        np.random.seed(seed)
+        self._eps = np.random.uniform(0, 2*np.pi, size=(len(freqs), len(angles)))
+
+    
+    def _spread_func(self, s=1):
+        """
+        Cosine spreading function.
+
+        Parameters
+        ----------
+        theta : 1D-array
+            Angles in spreading function.
+        theta_p : float
+            Peak angle for spreading function. (Dominant wave direction).
+        s : int (default = 1)
+            Steapness value to determine amount of spreading. Must be equal or large than 1.
+
+        Return
+        ------
+        spreading : 1D-array
+            Spreading function for the given angles, peak angles and steapness value.
+        """
+        d_theta = self._angles - self._theta_p
+        state = np.abs(d_theta) < np.pi/2
+        spreading = 2**(2*s - 1) * np.math.factorial(s)*np.math.factorial(s-1)/(np.pi*np.math.factorial(2*s-1)) * np.cos(d_theta)**(2*s)
+        spreading[~state] = 0
+        return spreading
+
+    def spectrum2d(self):
+        """
+        Calculate the two-dimensional directional wave spectrum.
+
+        Return
+        ------
+        F : 2D-array
+            Frequencies in meshgrid
+        T : 2D-array
+            Theta angle in meshgrid
+        spec2d : 2D-array
+            Directional wave spectrum for frequencies and angles.
+        """
+
+        F, T = np.meshgrid(self._freq, self._angles)
+        spec2d = self._spectrum*self._spreading[:, None]
+        self._spectrum2d = spec2d
+        return F, T, spec2d
+
+    def wave_realization(self, time, x, y):
+        """
+        Generate a 2D Multidirectional wavefield
+
+        Parameters
+        ----------
+        time : 1D-array
+            Array of time instances
+        x : 1D-array
+            Array of x-positions
+        y : 1D-array
+            Array of y-positions
+        
+        Return
+        ------
+        X : 2D-array
+            x values in meshgrid
+        Y : 2D-array
+            y values in meshgrid
+        wave_elevation : 2D-array
+            Wave elevation at position (x, y) at time t.
+        """
+
+        X, Y = np.meshgrid(x, y) # Create meshgrid
+        wave_elevation = 0
+
+        for j in range(len(self._freq)):
+            k_j = self._freq[j]**2 / self._g
+            for k in range(len(self._angles)):
+                theta = self._angles[k]
+                # eps_jk = np.random.uniform(0, 2*np.pi)
+                amplitude = np.sqrt(2*self._spectrum2d[k, j] * self._dw * self._dtheta)
+                wave_elevation += amplitude*np.sin(self._freq[j]*time - k_j*X*np.cos(theta) - k_j*Y*np.sin(theta) + self._eps[j, k])
+                
+        return X, Y, wave_elevation
+
+
+
+
+if __name__ == "__main__":
+    # Simple How-To for wave module
+    import doctest
+    doctest.testmod()
+    import matplotlib.pyplot as plt
+    from matplotlib import cm
+    plt.rcParams.update({
+        'figure.figsize': (12, 4),
+        'font.size': 14,
+        'lines.linewidth': 1.4
+    })
+
+    hs = 2.0
+    tp = 9.5
+    wp = 2*np.pi / tp
+    gamma = 5
+
+    wmin = wp - wp/2
+    wmax = 2*wp
+    N = 20
+    w = np.linspace(wmin, wmax, N)
+
+    pm_spectrum = ModifiedPiersonMoskowitz(w)       # Instantiate MPM spectrum object
+    jonswap_spectrum = JONSWAP(w)                   # Instantiate Jonwswap spectrum object
+
+    # Calculate the zero-moment for both spectra.
+    m0_jonswap = jonswap_spectrum.moment(n=0, hs=hs, tp=tp, gamma=gamma)
+    m0_pm = pm_spectrum.moment(n=0, hs=hs, tp=tp)
+
+    print(f"JONSWAP: Hs = {4*np.sqrt(m0_jonswap):.2f} [m]")
+    print(f"PM: Hs = {4*np.sqrt(m0_pm):.2f} [m]")
+    
+    # plt.plot(*pm_spectrum(hs, tp), label="PM")
+    # plt.plot(*jonswap_spectrum(hs, tp, gamma), label="JONSWAP")
+    # plt.grid()
+    # plt.legend()
+    # plt.show()
+
+    freq, spectrum = jonswap_spectrum(hs, tp, gamma)
+
+    time = np.arange(0, 500, 0.1)
+
+    jonswap_realizatin = jonswap_spectrum.realization(time, hs=hs, tp=tp, gamma=gamma)
+    pm_realizatino = pm_spectrum.realization(time, hs=hs, tp=tp)
+
+    # plt.plot(time, pm_spectrum.realization(time, hs=hs, tp=tp))
+    # plt.plot(time, jonswap_spectrum.realization(time, hs=hs, tp=tp, gamma=gamma))
+    # plt.xlim(time[0], time[-1])
+    # plt.ylim(-6*np.sqrt(m0_jonswap), 6*np.sqrt(m0_jonswap))
+    # plt.show()
+
+    theta0 = np.pi/36
+    s=2
+    psi = np.linspace(-np.pi, np.pi, 15)
+    dir_spectra = DirectionalSpectrum(w, psi, theta_p=theta0, spectrum=spectrum, s=s)
+    F, T, spectrum2d = dir_spectra.spectrum2d()
+
+    fig = plt.figure(figsize=(16, 8))
+    ax = plt.axes(projection='3d')
+    ax.view_init(35, 40)
+    ax.plot_surface(F, T, spectrum2d, cmap=cm.coolwarm)
+    ax.set_xlabel(r"$\omega \; [\frac{rad}{s}]$")
+    ax.set_ylabel(r"$\psi \; [deg]$")
+    plt.show()
+
+    Nxy = 400
+    x = np.linspace(-150, 150, Nxy)
+    y = np.linspace(-150, 150, Nxy)
+    X, Y, realization_2d = dir_spectra.wave_realization(0, x, y)
+
+    def update3d(t, plot, x, y):
+        # Callback function for animation.
+        plot[0].remove()
+        _, _, wave = dir_spectra.wave_realization(t, x, y)
+        plot[0] = ax.plot_surface(X, Y, wave, cmap=cm.coolwarm)
+
+    fig = plt.figure(figsize=(16, 8))
+    ax = fig.add_subplot(111, projection="3d")
+    ax.view_init(30, 40)
+    # ax.plot_surface(X, Y, realization_2d, cmap=cm.coolwarm)
+    ax.set_zlim([-2*hs, 2*hs])
+    ax.set_xlabel("$x \, [m]$")
+    ax.set_ylabel("$y \, [m]$")
+    ax.set_zlabel("$\zeta \, [m]$")
+    
+    fps = 32
+
+    plot = [ax.plot_surface(X, Y, realization_2d, cmap=cm.coolwarm)]
+
+    from matplotlib.animation import FuncAnimation
+    
+    from datetime import datetime
+
+    duration = 20
+    t_start = datetime.now()
+    w_anim = FuncAnimation(fig, update3d, frames=np.linspace(0, duration, (duration*fps)), fargs=(plot, x, y,))
+    w_anim.save(f'wave_realization_disc{Nxy}_hs{hs:.2f}_tp{tp:.2f}_dir{np.rad2deg(theta0):.0f}_s{s:.0f}_{duration}_gamma{gamma:.1f}_sec.mp4', fps=fps, dpi=50)
+    t_end = datetime.now()
+
     print(f"Execution time : {(t_end - t_start).total_seconds()} [s].")
```

### Comparing `MCSimPython-0.0.14/src/MCSimPython/waves/wave_spreading.py` & `MCSimPython-0.1.1/src/MCSimPython/waves/wave_spreading.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-# Spreading functions for unidirectional and multidirectional wave fields
-import numpy as np
-from abc import ABC, abstractclassmethod
-
-class BaseSpreading(ABC):
-
-    """
-    Base class for spreading functions for wave fields.
-
-    Parameters
-    ----------
-    angles : 1D-array
-        Angles for spreading function in radians or degrees
-    degrees : bool (default = False)
-        Unit of angles radians if false degrees if true
-
-    """
-
-    def __init__(self, angles, degrees=False):
-        self._angles = angles
-        self._deg = degrees
-
-    def __call__(self, *args, degrees=None, **kwargs):
-        return self._spreading(*args, **kwargs)
-
-    @abstractclassmethod
-    def _spreading(self, *args, **kwargs):
-        raise NotImplementedError
-
-    
-class Unidirectional(BaseSpreading):
-
-    def _spreading(self, *args, **kwargs):
-        pass
-
-
-class MultiDirectional(BaseSpreading):
-
-    def __call__(self):
-        return super().__call__()
-
-    def _spreading(self):
-        in_pipi2 = np.abs(self._angles) < np.pi/2
-        f_beta = (2/np.pi) * np.cos(self._angles)**2
-        f_beta[~in_pipi2] = 0
-        return self._angles, f_beta
-
-    
-
-class MultiDirectionalAlt(BaseSpreading):
-
-    def __call__(self, theta0, s=1, degrees=None):
-        if s < 1:
-            raise ValueError(f"s={s}, s must be larger than or equal to 1.")
-        return super().__call__(theta0, s, degrees=degrees)
-
-    def _spreading(self, theta0, s):
-        d_theta = self._angles - theta0
-        in_pipi_half = np.abs(d_theta) < np.pi/2
-        f_theta = 2**(2*s - 1) * np.math.factorial(s)*np.math.factorial(s-1)/(np.pi*np.math.factorial(2*s-1)) * np.cos(d_theta)**(2*s)
-        f_theta[~in_pipi_half] = 0
-        return self._angles, f_theta
-
-
-if __name__ == "__main__":
-    import matplotlib.pyplot as plt
-
-    plt.rcParams.update({
-        'figure.figsize': (12, 4),
-        'font.size': 14,
-        'axes.grid': True,
-        'lines.linewidth': 1.4
-    })
-
-    N = 100
-    theta_min, theta_max = -np.pi, np.pi
-    theta = np.linspace(theta_min, theta_max, N)
-
-    spreading_spectra = MultiDirectional(theta)
-    spreading_nonzero = MultiDirectionalAlt(theta)
-    angles, spreading = spreading_spectra()
-    _, spreading2 = spreading_nonzero(np.pi/4, s=0)
-
-    plt.plot(angles, spreading, label="$f(\theta)$")
-    plt.plot(angles, spreading2, label="$f_2(\theta)$")
-    plt.xlim(angles[0], angles[-1])
-
+# Spreading functions for unidirectional and multidirectional wave fields
+import numpy as np
+from abc import ABC, abstractclassmethod
+
+class BaseSpreading(ABC):
+
+    """
+    Base class for spreading functions for wave fields.
+
+    Parameters
+    ----------
+    angles : 1D-array
+        Angles for spreading function in radians or degrees
+    degrees : bool (default = False)
+        Unit of angles radians if false degrees if true
+
+    """
+
+    def __init__(self, angles, degrees=False):
+        self._angles = angles
+        self._deg = degrees
+
+    def __call__(self, *args, degrees=None, **kwargs):
+        return self._spreading(*args, **kwargs)
+
+    @abstractclassmethod
+    def _spreading(self, *args, **kwargs):
+        raise NotImplementedError
+
+    
+class Unidirectional(BaseSpreading):
+
+    def _spreading(self, *args, **kwargs):
+        pass
+
+
+class MultiDirectional(BaseSpreading):
+
+    def __call__(self):
+        return super().__call__()
+
+    def _spreading(self):
+        in_pipi2 = np.abs(self._angles) < np.pi/2
+        f_beta = (2/np.pi) * np.cos(self._angles)**2
+        f_beta[~in_pipi2] = 0
+        return self._angles, f_beta
+
+    
+
+class MultiDirectionalAlt(BaseSpreading):
+
+    def __call__(self, theta0, s=1, degrees=None):
+        if s < 1:
+            raise ValueError(f"s={s}, s must be larger than or equal to 1.")
+        return super().__call__(theta0, s, degrees=degrees)
+
+    def _spreading(self, theta0, s):
+        d_theta = self._angles - theta0
+        in_pipi_half = np.abs(d_theta) < np.pi/2
+        f_theta = 2**(2*s - 1) * np.math.factorial(s)*np.math.factorial(s-1)/(np.pi*np.math.factorial(2*s-1)) * np.cos(d_theta)**(2*s)
+        f_theta[~in_pipi_half] = 0
+        return self._angles, f_theta
+
+
+if __name__ == "__main__":
+    import matplotlib.pyplot as plt
+
+    plt.rcParams.update({
+        'figure.figsize': (12, 4),
+        'font.size': 14,
+        'axes.grid': True,
+        'lines.linewidth': 1.4
+    })
+
+    N = 100
+    theta_min, theta_max = -np.pi, np.pi
+    theta = np.linspace(theta_min, theta_max, N)
+
+    spreading_spectra = MultiDirectional(theta)
+    spreading_nonzero = MultiDirectionalAlt(theta)
+    angles, spreading = spreading_spectra()
+    _, spreading2 = spreading_nonzero(np.pi/4, s=0)
+
+    plt.plot(angles, spreading, label="$f(\theta)$")
+    plt.plot(angles, spreading2, label="$f_2(\theta)$")
+    plt.xlim(angles[0], angles[-1])
+
     plt.show()
```

### Comparing `MCSimPython-0.0.14/src/MCSimPython.egg-info/SOURCES.txt` & `MCSimPython-0.1.1/src/MCSimPython.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-src/__init__.py
 src/MCSimPython/__init__.py
 src/MCSimPython/utils.py
 src/MCSimPython.egg-info/PKG-INFO
 src/MCSimPython.egg-info/SOURCES.txt
 src/MCSimPython.egg-info/dependency_links.txt
 src/MCSimPython.egg-info/requires.txt
 src/MCSimPython.egg-info/top_level.txt
 src/MCSimPython/control/__init__.py
+src/MCSimPython/control/adaptiveFS.py
 src/MCSimPython/control/backstepping.py
 src/MCSimPython/control/basic.py
 src/MCSimPython/guidance/__init__.py
 src/MCSimPython/guidance/filter.py
 src/MCSimPython/guidance/path_param.py
 src/MCSimPython/observer/__init__.py
 src/MCSimPython/observer/ekf.py
+src/MCSimPython/observer/ltv_kf.py
 src/MCSimPython/observer/nonlinobs.py
 src/MCSimPython/simulator/__init__.py
 src/MCSimPython/simulator/csad.py
 src/MCSimPython/simulator/gunnerus.py
 src/MCSimPython/simulator/thruster_dynamics.py
 src/MCSimPython/simulator/vessel.py
 src/MCSimPython/thrust_allocation/__init__.py
```

### Comparing `MCSimPython-0.0.14/tests/test_utils.py` & `MCSimPython-0.1.1/tests/test_utils.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,119 +1,119 @@
-import numpy as np
-import pytest
-
-import sys
-import os
-
-cwd = os.getcwd()
-sys.path.insert(0, cwd)
-
-from MCSimPython.utils import Rz, Ry, Rx, Rzyx, J, to_positive_angle, rigid_body_transform
-
-
-class TestKinematicUtils:
-
-    def test_Rz(self):
-        # Transformation from body frame to NED frame for rotation about z-axis
-        psi = np.deg2rad(90)
-        nu = np.array([1, 0, 0])
-
-        # Expected true value
-        eta_dot = np.array([0, 1, 0])
-
-        assert np.all(np.isclose(eta_dot, Rz(psi)@nu, rtol=1e-6))
-
-
-    def test_Rzyx(self):
-        psi, theta, phi = np.pi / 2, 0, 0
-        nu = np.array([1., 0., 0.])
-        eta = np.array([0, 0, 0, phi, theta, psi])
-
-        # Expected true value
-        eta_dot = np.array([0., 1., 0.])
-
-        assert np.all(np.isclose(eta_dot, Rzyx(eta)@nu, rtol=1e-6))
-
-
-    def test_J_dim(self):
-        psi, theta, phi = 0, 0, 0
-        eta = np.array([0, 0, 0, phi, theta, psi])
-
-        rotmat_6dof = J(eta)
-
-        assert np.all(np.equal((6, 6), rotmat_6dof.shape))
-
-    def test_J(self):
-        nu = np.array([1., 0., 0., 0., 0., 0.])
-        phi, theta, psi = 0., 0., np.pi/2
-        eta = np.array([0, 0, 0, phi, theta, psi])
-
-        eta_dot = np.array([0., 1., 0., 0., 0., 0.])
-        
-        assert np.all(np.isclose(eta_dot, J(eta)@nu, rtol=1e-6))
-
-    def test_positive_angle_map(self):
-        angle = -np.pi / 2  # corresponding to 270 degrees (3pi/2)
-        pos_angle = to_positive_angle(angle)
-        true_angle = 3*np.pi / 2
-        assert np.equal(pos_angle, true_angle)
-
-    def test_array_positive_angle_map(self):
-        angles = np.array([-np.pi, -np.pi/2])
-        pos_angles = to_positive_angle(angles)
-        true_angles = np.array([np.pi, 3*np.pi/2])
-        assert np.all(np.isclose(pos_angles, true_angles, rtol=1e-6))
-
-    def test_rigid_body_transform_translation(self):
-        r = np.array([1., 0., -1.]) # Defined in the body-frame
-        eta_1 = np.concatenate((np.array([1., 0., 0.]), np.zeros(3)))
-        eta_2 = np.concatenate((np.array([0., 1., 0]), np.zeros(3)))
-        eta_3 = np.concatenate((np.array([0., 0., 1.0]), np.zeros(3)))
-
-        s_true_1 = np.array([1., 0., 0.])
-        s_true_2 = np.array([0., 1., 0.])
-        s_true_3 = np.array([0., 0., 1.])
-
-        assert np.all(np.isclose(rigid_body_transform(r, eta_1, in_ned=False), s_true_1, rtol=1e-5))
-        assert np.all(np.isclose(rigid_body_transform(r, eta_2, in_ned=False), s_true_2, rtol=1e-5))
-        assert np.all(np.isclose(rigid_body_transform(r, eta_3, in_ned=False), s_true_3, rtol=1e-5))
-
-    def test_rigid_body_transform_rotations(self):
-        r = np.array([1., 0., -1]) # Define the lever arm in body-frame
-        eta13 = np.zeros(3) # No translational motions
-        eta36_1 = np.array([np.pi/180*2, 0.0, 0.])  # 2 degree roll
-        eta36_2 = np.array([0., 3*np.pi/180, 0.0])  # 3 degree pitch
-        eta36_3 = np.array([0., 0., 5*np.pi/180])   # 5 degree yaw
-
-        eta_1 = np.concatenate([eta13, eta36_1])
-        eta_2 = np.concatenate([eta13, eta36_2])
-        eta_3 = np.concatenate([eta13, eta36_3])
-
-        s_1 = np.array([0.0, 2*np.pi/180, 0.0]) # Only a change in the y-axis
-        s_2 = np.array([-1*3*np.pi/180, 0.0, -3*np.pi/180])
-        s_3 = np.array([0., 5*np.pi/180, 0.0])
-
-        assert np.allclose(rigid_body_transform(r, eta_1, in_ned=False), s_1, rtol=1e-5)
-        assert np.allclose(rigid_body_transform(r, eta_2, in_ned=False), s_2, rtol=1e-5)
-        assert np.allclose(rigid_body_transform(r, eta_3, in_ned=False), s_3, rtol=1e-5)
-
-    def test_rigid_transform_ref_frames(self):
-        r = np.array([1., 0., 0.])  # Lever arm defined in body-frame
-
-        # Vessel pose in NED-frame
-        eta = np.array([
-            1.0,
-            0.0,
-            0.0,
-            0.0,
-            0.0,
-            np.pi/4
-        ])
-
-        s_body = np.array([1., np.pi/4, 0.0])    # Lever arm change in body-frame
-        s_ned = np.array([np.cos(np.pi/4), -np.sin(np.pi/4) + np.pi/4, 0.]) # Lever arm change in ned-frame
-
-        print(rigid_body_transform(r, eta, in_ned=True))
-        
-        assert np.allclose(rigid_body_transform(r, eta, in_ned=False), s_body)
-        assert np.allclose(rigid_body_transform(r, eta, in_ned=True), s_ned)
-
+import numpy as np
+import pytest
+
+import sys
+import os
+
+cwd = os.getcwd()
+sys.path.insert(0, cwd)
+
+from MCSimPython.utils import Rz, Ry, Rx, Rzyx, J, to_positive_angle, rigid_body_transform
+
+
+class TestKinematicUtils:
+
+    def test_Rz(self):
+        # Transformation from body frame to NED frame for rotation about z-axis
+        psi = np.deg2rad(90)
+        nu = np.array([1, 0, 0])
+
+        # Expected true value
+        eta_dot = np.array([0, 1, 0])
+
+        assert np.all(np.isclose(eta_dot, Rz(psi)@nu, rtol=1e-6))
+
+
+    def test_Rzyx(self):
+        psi, theta, phi = np.pi / 2, 0, 0
+        nu = np.array([1., 0., 0.])
+        eta = np.array([0, 0, 0, phi, theta, psi])
+
+        # Expected true value
+        eta_dot = np.array([0., 1., 0.])
+
+        assert np.all(np.isclose(eta_dot, Rzyx(eta)@nu, rtol=1e-6))
+
+
+    def test_J_dim(self):
+        psi, theta, phi = 0, 0, 0
+        eta = np.array([0, 0, 0, phi, theta, psi])
+
+        rotmat_6dof = J(eta)
+
+        assert np.all(np.equal((6, 6), rotmat_6dof.shape))
+
+    def test_J(self):
+        nu = np.array([1., 0., 0., 0., 0., 0.])
+        phi, theta, psi = 0., 0., np.pi/2
+        eta = np.array([0, 0, 0, phi, theta, psi])
+
+        eta_dot = np.array([0., 1., 0., 0., 0., 0.])
+        
+        assert np.all(np.isclose(eta_dot, J(eta)@nu, rtol=1e-6))
+
+    def test_positive_angle_map(self):
+        angle = -np.pi / 2  # corresponding to 270 degrees (3pi/2)
+        pos_angle = to_positive_angle(angle)
+        true_angle = 3*np.pi / 2
+        assert np.equal(pos_angle, true_angle)
+
+    def test_array_positive_angle_map(self):
+        angles = np.array([-np.pi, -np.pi/2])
+        pos_angles = to_positive_angle(angles)
+        true_angles = np.array([np.pi, 3*np.pi/2])
+        assert np.all(np.isclose(pos_angles, true_angles, rtol=1e-6))
+
+    def test_rigid_body_transform_translation(self):
+        r = np.array([1., 0., -1.]) # Defined in the body-frame
+        eta_1 = np.concatenate((np.array([1., 0., 0.]), np.zeros(3)))
+        eta_2 = np.concatenate((np.array([0., 1., 0]), np.zeros(3)))
+        eta_3 = np.concatenate((np.array([0., 0., 1.0]), np.zeros(3)))
+
+        s_true_1 = np.array([1., 0., 0.])
+        s_true_2 = np.array([0., 1., 0.])
+        s_true_3 = np.array([0., 0., 1.])
+
+        assert np.all(np.isclose(rigid_body_transform(r, eta_1, in_ned=False), s_true_1, rtol=1e-5))
+        assert np.all(np.isclose(rigid_body_transform(r, eta_2, in_ned=False), s_true_2, rtol=1e-5))
+        assert np.all(np.isclose(rigid_body_transform(r, eta_3, in_ned=False), s_true_3, rtol=1e-5))
+
+    def test_rigid_body_transform_rotations(self):
+        r = np.array([1., 0., -1]) # Define the lever arm in body-frame
+        eta13 = np.zeros(3) # No translational motions
+        eta36_1 = np.array([np.pi/180*2, 0.0, 0.])  # 2 degree roll
+        eta36_2 = np.array([0., 3*np.pi/180, 0.0])  # 3 degree pitch
+        eta36_3 = np.array([0., 0., 5*np.pi/180])   # 5 degree yaw
+
+        eta_1 = np.concatenate([eta13, eta36_1])
+        eta_2 = np.concatenate([eta13, eta36_2])
+        eta_3 = np.concatenate([eta13, eta36_3])
+
+        s_1 = np.array([0.0, 2*np.pi/180, 0.0]) # Only a change in the y-axis
+        s_2 = np.array([-1*3*np.pi/180, 0.0, -3*np.pi/180])
+        s_3 = np.array([0., 5*np.pi/180, 0.0])
+
+        assert np.allclose(rigid_body_transform(r, eta_1, in_ned=False), s_1, rtol=1e-5)
+        assert np.allclose(rigid_body_transform(r, eta_2, in_ned=False), s_2, rtol=1e-5)
+        assert np.allclose(rigid_body_transform(r, eta_3, in_ned=False), s_3, rtol=1e-5)
+
+    def test_rigid_transform_ref_frames(self):
+        r = np.array([1., 0., 0.])  # Lever arm defined in body-frame
+
+        # Vessel pose in NED-frame
+        eta = np.array([
+            1.0,
+            0.0,
+            0.0,
+            0.0,
+            0.0,
+            np.pi/4
+        ])
+
+        s_body = np.array([1., np.pi/4, 0.0])    # Lever arm change in body-frame
+        s_ned = np.array([np.cos(np.pi/4), -np.sin(np.pi/4) + np.pi/4, 0.]) # Lever arm change in ned-frame
+
+        print(rigid_body_transform(r, eta, in_ned=True))
+        
+        assert np.allclose(rigid_body_transform(r, eta, in_ned=False), s_body)
+        assert np.allclose(rigid_body_transform(r, eta, in_ned=True), s_ned)
+
```


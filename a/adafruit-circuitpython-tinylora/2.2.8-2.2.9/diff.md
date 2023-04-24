# Comparing `tmp/adafruit-circuitpython-tinylora-2.2.8.tar.gz` & `tmp/adafruit-circuitpython-tinylora-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-tinylora-2.2.8.tar", last modified: Thu Jun  9 18:36:51 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-tinylora-2.2.9.tar", last modified: Tue Aug  9 19:40:56 2022, max compression
```

## Comparing `adafruit-circuitpython-tinylora-2.2.8.tar` & `adafruit-circuitpython-tinylora-2.2.9.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:36:51.464852 adafruit-circuitpython-tinylora-2.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:36:51.456852 adafruit-circuitpython-tinylora-2.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:36:51.460852 adafruit-circuitpython-tinylora-2.2.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:36:51.460852 adafruit-circuitpython-tinylora-2.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:36:51.460852 adafruit-circuitpython-tinylora-2.2.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)    31752 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/LICENSES/GPL-3.0-or-later.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3824 2022-06-09 18:36:51.464852 adafruit-circuitpython-tinylora-2.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3088 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:36:51.460852 adafruit-circuitpython-tinylora-2.2.8/adafruit_circuitpython_tinylora.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3824 2022-06-09 18:36:51.000000 adafruit-circuitpython-tinylora-2.2.8/adafruit_circuitpython_tinylora.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1256 2022-06-09 18:36:51.000000 adafruit-circuitpython-tinylora-2.2.8/adafruit_circuitpython_tinylora.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-09 18:36:51.000000 adafruit-circuitpython-tinylora-2.2.8/adafruit_circuitpython_tinylora.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-06-09 18:36:51.000000 adafruit-circuitpython-tinylora-2.2.8/adafruit_circuitpython_tinylora.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-06-09 18:36:51.000000 adafruit-circuitpython-tinylora-2.2.8/adafruit_circuitpython_tinylora.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:36:51.460852 adafruit-circuitpython-tinylora-2.2.8/adafruit_tinylora/
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/adafruit_tinylora/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    13129 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/adafruit_tinylora/adafruit_tinylora.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    13205 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/adafruit_tinylora/adafruit_tinylora_encryption.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      577 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/adafruit_tinylora/ttn_as.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      579 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/adafruit_tinylora/ttn_au.py
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/adafruit_tinylora/ttn_cn.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      579 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/adafruit_tinylora/ttn_eu.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      580 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/adafruit_tinylora/ttn_usa.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:36:51.464852 adafruit-circuitpython-tinylora-2.2.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:36:51.464852 adafruit-circuitpython-tinylora-2.2.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      714 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5541 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      975 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:36:51.464852 adafruit-circuitpython-tinylora-2.2.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1706 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/examples/tinylora_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2435 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/examples/tinylora_simpletest_si7021.py
--rw-r--r--   0 runner    (1001) docker     (121)     1770 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/examples/tinylora_simpletest_single_channel.py
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-09 18:36:51.464852 adafruit-circuitpython-tinylora-2.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1853 2022-06-09 18:36:39.000000 adafruit-circuitpython-tinylora-2.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:40:56.949673 adafruit-circuitpython-tinylora-2.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:40:56.945673 adafruit-circuitpython-tinylora-2.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:40:56.949673 adafruit-circuitpython-tinylora-2.2.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-09 19:40:41.000000 adafruit-circuitpython-tinylora-2.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:40:56.949673 adafruit-circuitpython-tinylora-2.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-09 19:40:41.000000 adafruit-circuitpython-tinylora-2.2.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-09 19:40:41.000000 adafruit-circuitpython-tinylora-2.2.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-09 19:40:41.000000 adafruit-circuitpython-tinylora-2.2.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-09 19:40:41.000000 adafruit-circuitpython-tinylora-2.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-09 19:40:41.000000 adafruit-circuitpython-tinylora-2.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-09 19:40:41.000000 adafruit-circuitpython-tinylora-2.2.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-09 19:40:41.000000 adafruit-circuitpython-tinylora-2.2.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-09 19:40:41.000000 adafruit-circuitpython-tinylora-2.2.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-08-09 19:40:41.000000 adafruit-circuitpython-tinylora-2.2.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:40:56.949673 adafruit-circuitpython-tinylora-2.2.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-09 19:40:41.000000 adafruit-circuitpython-tinylora-2.2.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    31752 2022-08-09 19:40:41.000000 adafruit-circuitpython-tinylora-2.2.9/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-09 19:40:41.000000 adafruit-circuitpython-tinylora-2.2.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-09 19:40:41.000000 adafruit-circuitpython-tinylora-2.2.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3996 2022-08-09 19:40:56.949673 adafruit-circuitpython-tinylora-2.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3231 2022-08-09 19:40:41.000000 adafruit-circuitpython-tinylora-2.2.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:40:41.000000 adafruit-circuitpython-tinylora-2.2.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:40:56.949673 adafruit-circuitpython-tinylora-2.2.9/adafruit_circuitpython_tinylora.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3996 2022-08-09 19:40:56.000000 adafruit-circuitpython-tinylora-2.2.9/adafruit_circuitpython_tinylora.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1288 2022-08-09 19:40:56.000000 adafruit-circuitpython-tinylora-2.2.9/adafruit_circuitpython_tinylora.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-09 19:40:56.000000 adafruit-circuitpython-tinylora-2.2.9/adafruit_circuitpython_tinylora.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-09 19:40:56.000000 adafruit-circuitpython-tinylora-2.2.9/adafruit_circuitpython_tinylora.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-08-09 19:40:56.000000 adafruit-circuitpython-tinylora-2.2.9/adafruit_circuitpython_tinylora.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:40:56.949673 adafruit-circuitpython-tinylora-2.2.9/adafruit_tinylora/
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2022-08-09 19:40:49.000000 adafruit-circuitpython-tinylora-2.2.9/adafruit_tinylora/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    13122 2022-08-09 19:40:49.000000 adafruit-circuitpython-tinylora-2.2.9/adafruit_tinylora/adafruit_tinylora.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    13205 2022-08-09 19:40:49.000000 adafruit-circuitpython-tinylora-2.2.9/adafruit_tinylora/adafruit_tinylora_encryption.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      577 2022-08-09 19:40:49.000000 adafruit-circuitpython-tinylora-2.2.9/adafruit_tinylora/ttn_as.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      579 2022-08-09 19:40:49.000000 adafruit-circuitpython-tinylora-2.2.9/adafruit_tinylora/ttn_au.py
+-rw-r--r--   0 runner    (1001) docker     (121)      615 2022-08-09 19:40:49.000000 adafruit-circuitpython-tinylora-2.2.9/adafruit_tinylora/ttn_cn.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      579 2022-08-09 19:40:49.000000 adafruit-circuitpython-tinylora-2.2.9/adafruit_tinylora/ttn_eu.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      580 2022-08-09 19:40:49.000000 adafruit-circuitpython-tinylora-2.2.9/adafruit_tinylora/ttn_usa.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:40:56.949673 adafruit-circuitpython-tinylora-2.2.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:40:56.949673 adafruit-circuitpython-tinylora-2.2.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-09 19:40:41.000000 adafruit-circuitpython-tinylora-2.2.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-09 19:40:41.000000 adafruit-circuitpython-tinylora-2.2.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      714 2022-08-09 19:40:41.000000 adafruit-circuitpython-tinylora-2.2.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:40:41.000000 adafruit-circuitpython-tinylora-2.2.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5541 2022-08-09 19:40:41.000000 adafruit-circuitpython-tinylora-2.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      658 2022-08-09 19:40:41.000000 adafruit-circuitpython-tinylora-2.2.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:40:41.000000 adafruit-circuitpython-tinylora-2.2.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      975 2022-08-09 19:40:41.000000 adafruit-circuitpython-tinylora-2.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:40:41.000000 adafruit-circuitpython-tinylora-2.2.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-09 19:40:41.000000 adafruit-circuitpython-tinylora-2.2.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:40:56.949673 adafruit-circuitpython-tinylora-2.2.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1706 2022-08-09 19:40:49.000000 adafruit-circuitpython-tinylora-2.2.9/examples/tinylora_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2435 2022-08-09 19:40:49.000000 adafruit-circuitpython-tinylora-2.2.9/examples/tinylora_simpletest_si7021.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1770 2022-08-09 19:40:49.000000 adafruit-circuitpython-tinylora-2.2.9/examples/tinylora_simpletest_single_channel.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:40:41.000000 adafruit-circuitpython-tinylora-2.2.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-09 19:40:49.000000 adafruit-circuitpython-tinylora-2.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      158 2022-08-09 19:40:41.000000 adafruit-circuitpython-tinylora-2.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-09 19:40:56.949673 adafruit-circuitpython-tinylora-2.2.9/setup.cfg
```

### Comparing `adafruit-circuitpython-tinylora-2.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-tinylora-2.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tinylora-2.2.8/.github/workflows/build.yml` & `adafruit-circuitpython-tinylora-2.2.9/.github/workflows/build.yml`

 * *Files 16% similar despite different names*

```diff
@@ -43,33 +43,35 @@
       run: |
         source actions-ci/install.sh
     - name: Pip install Sphinx, pre-commit
       run: |
         pip install --force-reinstall Sphinx sphinx-rtd-theme pre-commit
     - name: Library version
       run: git describe --dirty --always --tags
+    - name: Setup problem matchers
+      uses: adafruit/circuitpython-action-library-ci-problem-matchers@v1
     - name: Pre-commit hooks
       run: |
         pre-commit run --all-files
     - name: Build assets
       run: circuitpython-build-bundles --filename_prefix ${{ steps.repo-name.outputs.repo-name }} --library_location .
     - name: Archive bundles
       uses: actions/upload-artifact@v2
       with:
         name: bundles
         path: ${{ github.workspace }}/bundles/
     - name: Build docs
       working-directory: docs
       run: sphinx-build -E -W -b html . _build/html
-    - name: Check For setup.py
+    - name: Check For pyproject.toml
       id: need-pypi
       run: |
-        echo ::set-output name=setup-py::$( find . -wholename './setup.py' )
+        echo ::set-output name=pyproject-toml::$( find . -wholename './pyproject.toml' )
     - name: Build Python package
-      if: contains(steps.need-pypi.outputs.setup-py, 'setup.py')
+      if: contains(steps.need-pypi.outputs.pyproject-toml, 'pyproject.toml')
       run: |
-        pip install --upgrade setuptools wheel twine readme_renderer testresources
-        python setup.py sdist
-        python setup.py bdist_wheel --universal
+        pip install --upgrade build twine
+        for file in $(find -not -path "./.*" -not -path "./docs*" \( -name "*.py" -o -name "*.toml" \) ); do
+            sed -i -e "s/0.0.0-auto.0/1.2.3/" $file;
+        done;
+        python -m build
         twine check dist/*
-    - name: Setup problem matchers
-      uses: adafruit/circuitpython-action-library-ci-problem-matchers@v1
```

### Comparing `adafruit-circuitpython-tinylora-2.2.8/.gitignore` & `adafruit-circuitpython-tinylora-2.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tinylora-2.2.8/.pre-commit-config.yaml` & `adafruit-circuitpython-tinylora-2.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tinylora-2.2.8/.pylintrc` & `adafruit-circuitpython-tinylora-2.2.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tinylora-2.2.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-tinylora-2.2.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tinylora-2.2.8/LICENSE` & `adafruit-circuitpython-tinylora-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tinylora-2.2.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-tinylora-2.2.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tinylora-2.2.8/LICENSES/GPL-3.0-or-later.txt` & `adafruit-circuitpython-tinylora-2.2.9/LICENSES/GPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tinylora-2.2.8/LICENSES/MIT.txt` & `adafruit-circuitpython-tinylora-2.2.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tinylora-2.2.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-tinylora-2.2.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tinylora-2.2.8/PKG-INFO` & `adafruit-circuitpython-tinylora-2.2.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-tinylora
-Version: 2.2.8
+Version: 2.2.9
 Summary: CircuitPython library for LoRaWAN and The Things Network.
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_TinyLoRa
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
-Keywords: adafruit lorawan thethingsnetwork hardware micropython circuitpython
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_TinyLoRa
+Keywords: adafruit,lorawan,thethingsnetwork,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
+Provides-Extra: optional
 License-File: LICENSE
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/circuitpython-tinylora/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/tinylora/en/latest/
@@ -28,14 +27,18 @@
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_TinyLoRa/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_TinyLoRa/actions/
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 **WARNING: This library is not compatible with The Things Network v3 stack. Since TTN has fully migrated to v3, this library is not longer able to communicate with TTN.**
 
 
 LoRaWAN/The Things Network V2, for CircuitPython.
 
 Dependencies
 =============
@@ -64,16 +67,16 @@
     sudo pip3 install adafruit-circuitpython-tinylora
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-tinylora
 
 Usage Example
 =============
 
 Usage is described in the `learn guide for this library <https://learn.adafruit.com/using-lorawan-and-the-things-network-with-circuitpython>`_.
 
@@ -95,9 +98,7 @@
 =======
 
 This library was written by ClemensRiederer. We've converted it to work with Adafruit CircuitPython and made
 changes so it works with the Raspberry Pi and Adafruit Feather M0/M4. We've added examples for using this library
 to transmit data and sensor data to The Things Network.
 
 This open source code is licensed under the LGPL license (see LICENSE for details).
-
-
```

### Comparing `adafruit-circuitpython-tinylora-2.2.8/README.rst` & `adafruit-circuitpython-tinylora-2.2.9/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,18 @@
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_TinyLoRa/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_TinyLoRa/actions/
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 **WARNING: This library is not compatible with The Things Network v3 stack. Since TTN has fully migrated to v3, this library is not longer able to communicate with TTN.**
 
 
 LoRaWAN/The Things Network V2, for CircuitPython.
 
 Dependencies
 =============
@@ -45,16 +49,16 @@
     sudo pip3 install adafruit-circuitpython-tinylora
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-tinylora
 
 Usage Example
 =============
 
 Usage is described in the `learn guide for this library <https://learn.adafruit.com/using-lorawan-and-the-things-network-with-circuitpython>`_.
```

### Comparing `adafruit-circuitpython-tinylora-2.2.8/adafruit_circuitpython_tinylora.egg-info/PKG-INFO` & `adafruit-circuitpython-tinylora-2.2.9/adafruit_circuitpython_tinylora.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-tinylora
-Version: 2.2.8
+Version: 2.2.9
 Summary: CircuitPython library for LoRaWAN and The Things Network.
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_TinyLoRa
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
-Keywords: adafruit lorawan thethingsnetwork hardware micropython circuitpython
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_TinyLoRa
+Keywords: adafruit,lorawan,thethingsnetwork,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
+Provides-Extra: optional
 License-File: LICENSE
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/circuitpython-tinylora/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/tinylora/en/latest/
@@ -28,14 +27,18 @@
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_TinyLoRa/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_TinyLoRa/actions/
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 **WARNING: This library is not compatible with The Things Network v3 stack. Since TTN has fully migrated to v3, this library is not longer able to communicate with TTN.**
 
 
 LoRaWAN/The Things Network V2, for CircuitPython.
 
 Dependencies
 =============
@@ -64,16 +67,16 @@
     sudo pip3 install adafruit-circuitpython-tinylora
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-tinylora
 
 Usage Example
 =============
 
 Usage is described in the `learn guide for this library <https://learn.adafruit.com/using-lorawan-and-the-things-network-with-circuitpython>`_.
 
@@ -95,9 +98,7 @@
 =======
 
 This library was written by ClemensRiederer. We've converted it to work with Adafruit CircuitPython and made
 changes so it works with the Raspberry Pi and Adafruit Feather M0/M4. We've added examples for using this library
 to transmit data and sensor data to The Things Network.
 
 This open source code is licensed under the LGPL license (see LICENSE for details).
-
-
```

### Comparing `adafruit-circuitpython-tinylora-2.2.8/adafruit_circuitpython_tinylora.egg-info/SOURCES.txt` & `adafruit-circuitpython-tinylora-2.2.9/adafruit_circuitpython_tinylora.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 .pre-commit-config.yaml
 .pylintrc
 .readthedocs.yaml
 CODE_OF_CONDUCT.md
 LICENSE
 README.rst
 README.rst.license
+optional_requirements.txt
+pyproject.toml
 requirements.txt
-setup.py
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
 .github/workflows/release.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/GPL-3.0-or-later.txt
 LICENSES/MIT.txt
```

### Comparing `adafruit-circuitpython-tinylora-2.2.8/adafruit_tinylora/adafruit_tinylora.py` & `adafruit-circuitpython-tinylora-2.2.9/adafruit_tinylora/adafruit_tinylora.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 import time
 from random import randint
 from micropython import const
 import adafruit_bus_device.spi_device
 from adafruit_tinylora.adafruit_tinylora_encryption import AES
 
-__version__ = "0.0.0-auto.0"
+__version__ = "2.2.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_TinyLoRa.git"
 
 # RFM Module Settings
 _MODE_SLEEP = const(0x00)
 _MODE_LORA = const(0x80)
 _MODE_STDBY = const(0x01)
 _MODE_TX = const(0x83)
```

### Comparing `adafruit-circuitpython-tinylora-2.2.8/adafruit_tinylora/adafruit_tinylora_encryption.py` & `adafruit-circuitpython-tinylora-2.2.9/adafruit_tinylora/adafruit_tinylora_encryption.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tinylora-2.2.8/adafruit_tinylora/ttn_as.py` & `adafruit-circuitpython-tinylora-2.2.9/adafruit_tinylora/ttn_as.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tinylora-2.2.8/adafruit_tinylora/ttn_au.py` & `adafruit-circuitpython-tinylora-2.2.9/adafruit_tinylora/ttn_au.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tinylora-2.2.8/adafruit_tinylora/ttn_cn.py` & `adafruit-circuitpython-tinylora-2.2.9/adafruit_tinylora/ttn_cn.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tinylora-2.2.8/adafruit_tinylora/ttn_eu.py` & `adafruit-circuitpython-tinylora-2.2.9/adafruit_tinylora/ttn_eu.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tinylora-2.2.8/adafruit_tinylora/ttn_usa.py` & `adafruit-circuitpython-tinylora-2.2.9/adafruit_tinylora/ttn_usa.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tinylora-2.2.8/docs/_static/favicon.ico` & `adafruit-circuitpython-tinylora-2.2.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tinylora-2.2.8/docs/api.rst` & `adafruit-circuitpython-tinylora-2.2.9/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tinylora-2.2.8/docs/conf.py` & `adafruit-circuitpython-tinylora-2.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tinylora-2.2.8/docs/examples.rst` & `adafruit-circuitpython-tinylora-2.2.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tinylora-2.2.8/docs/index.rst` & `adafruit-circuitpython-tinylora-2.2.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tinylora-2.2.8/examples/tinylora_simpletest.py` & `adafruit-circuitpython-tinylora-2.2.9/examples/tinylora_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tinylora-2.2.8/examples/tinylora_simpletest_si7021.py` & `adafruit-circuitpython-tinylora-2.2.9/examples/tinylora_simpletest_si7021.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tinylora-2.2.8/examples/tinylora_simpletest_single_channel.py` & `adafruit-circuitpython-tinylora-2.2.9/examples/tinylora_simpletest_single_channel.py`

 * *Files identical despite different names*


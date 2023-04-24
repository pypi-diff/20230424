# Comparing `tmp/adafruit-circuitpython-mcp2515-1.1.0.tar.gz` & `tmp/adafruit-circuitpython-mcp2515-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-mcp2515-1.1.0.tar", last modified: Fri Jan 27 00:35:57 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-mcp2515-1.1.1.tar", last modified: Mon Apr 24 19:17:30 2023, max compression
```

## Comparing `adafruit-circuitpython-mcp2515-1.1.0.tar` & `adafruit-circuitpython-mcp2515-1.1.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 00:35:57.828384 adafruit-circuitpython-mcp2515-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 00:35:57.824384 adafruit-circuitpython-mcp2515-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 00:35:57.824384 adafruit-circuitpython-mcp2515-1.1.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-01-27 00:35:42.000000 adafruit-circuitpython-mcp2515-1.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 00:35:57.824384 adafruit-circuitpython-mcp2515-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-01-27 00:35:42.000000 adafruit-circuitpython-mcp2515-1.1.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-01-27 00:35:42.000000 adafruit-circuitpython-mcp2515-1.1.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-01-27 00:35:42.000000 adafruit-circuitpython-mcp2515-1.1.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-01-27 00:35:42.000000 adafruit-circuitpython-mcp2515-1.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-01-27 00:35:42.000000 adafruit-circuitpython-mcp2515-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-01-27 00:35:42.000000 adafruit-circuitpython-mcp2515-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-01-27 00:35:42.000000 adafruit-circuitpython-mcp2515-1.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-01-27 00:35:42.000000 adafruit-circuitpython-mcp2515-1.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-01-27 00:35:42.000000 adafruit-circuitpython-mcp2515-1.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-01-27 00:35:42.000000 adafruit-circuitpython-mcp2515-1.1.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 00:35:57.824384 adafruit-circuitpython-mcp2515-1.1.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-01-27 00:35:42.000000 adafruit-circuitpython-mcp2515-1.1.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-01-27 00:35:42.000000 adafruit-circuitpython-mcp2515-1.1.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-01-27 00:35:42.000000 adafruit-circuitpython-mcp2515-1.1.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-01-27 00:35:57.828384 adafruit-circuitpython-mcp2515-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-01-27 00:35:42.000000 adafruit-circuitpython-mcp2515-1.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-27 00:35:42.000000 adafruit-circuitpython-mcp2515-1.1.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 00:35:57.824384 adafruit-circuitpython-mcp2515-1.1.0/adafruit_circuitpython_mcp2515.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-01-27 00:35:57.000000 adafruit-circuitpython-mcp2515-1.1.0/adafruit_circuitpython_mcp2515.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-01-27 00:35:57.000000 adafruit-circuitpython-mcp2515-1.1.0/adafruit_circuitpython_mcp2515.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 00:35:57.000000 adafruit-circuitpython-mcp2515-1.1.0/adafruit_circuitpython_mcp2515.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-27 00:35:57.000000 adafruit-circuitpython-mcp2515-1.1.0/adafruit_circuitpython_mcp2515.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-27 00:35:57.000000 adafruit-circuitpython-mcp2515-1.1.0/adafruit_circuitpython_mcp2515.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 00:35:57.824384 adafruit-circuitpython-mcp2515-1.1.0/adafruit_mcp2515/
--rw-r--r--   0 runner    (1001) docker     (123)    31453 2023-01-27 00:35:50.000000 adafruit-circuitpython-mcp2515-1.1.0/adafruit_mcp2515/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 00:35:57.824384 adafruit-circuitpython-mcp2515-1.1.0/adafruit_mcp2515/canio/
--rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-01-27 00:35:50.000000 adafruit-circuitpython-mcp2515-1.1.0/adafruit_mcp2515/canio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-01-27 00:35:50.000000 adafruit-circuitpython-mcp2515-1.1.0/adafruit_mcp2515/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 00:35:57.828384 adafruit-circuitpython-mcp2515-1.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 00:35:57.828384 adafruit-circuitpython-mcp2515-1.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-01-27 00:35:42.000000 adafruit-circuitpython-mcp2515-1.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-01-27 00:35:42.000000 adafruit-circuitpython-mcp2515-1.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-01-27 00:35:42.000000 adafruit-circuitpython-mcp2515-1.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-27 00:35:42.000000 adafruit-circuitpython-mcp2515-1.1.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-01-27 00:35:42.000000 adafruit-circuitpython-mcp2515-1.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-01-27 00:35:42.000000 adafruit-circuitpython-mcp2515-1.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-27 00:35:42.000000 adafruit-circuitpython-mcp2515-1.1.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-01-27 00:35:42.000000 adafruit-circuitpython-mcp2515-1.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-27 00:35:42.000000 adafruit-circuitpython-mcp2515-1.1.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-01-27 00:35:42.000000 adafruit-circuitpython-mcp2515-1.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 00:35:57.828384 adafruit-circuitpython-mcp2515-1.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    14883 2023-01-27 00:35:50.000000 adafruit-circuitpython-mcp2515-1.1.0/examples/mcp2515_canio_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-01-27 00:35:50.000000 adafruit-circuitpython-mcp2515-1.1.0/examples/mcp2515_loopback_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-01-27 00:35:50.000000 adafruit-circuitpython-mcp2515-1.1.0/examples/mcp2515_receive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-01-27 00:35:50.000000 adafruit-circuitpython-mcp2515-1.1.0/examples/mcp2515_send_and_receive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-01-27 00:35:50.000000 adafruit-circuitpython-mcp2515-1.1.0/examples/mcp2515_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-27 00:35:42.000000 adafruit-circuitpython-mcp2515-1.1.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-01-27 00:35:50.000000 adafruit-circuitpython-mcp2515-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-01-27 00:35:42.000000 adafruit-circuitpython-mcp2515-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-27 00:35:57.828384 adafruit-circuitpython-mcp2515-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:17:30.137586 adafruit-circuitpython-mcp2515-1.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:17:30.129586 adafruit-circuitpython-mcp2515-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:17:30.133586 adafruit-circuitpython-mcp2515-1.1.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:17:30.133586 adafruit-circuitpython-mcp2515-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:17:30.133586 adafruit-circuitpython-mcp2515-1.1.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-04-24 19:17:30.137586 adafruit-circuitpython-mcp2515-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:17:30.133586 adafruit-circuitpython-mcp2515-1.1.1/adafruit_circuitpython_mcp2515.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-04-24 19:17:30.000000 adafruit-circuitpython-mcp2515-1.1.1/adafruit_circuitpython_mcp2515.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-24 19:17:30.000000 adafruit-circuitpython-mcp2515-1.1.1/adafruit_circuitpython_mcp2515.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 19:17:30.000000 adafruit-circuitpython-mcp2515-1.1.1/adafruit_circuitpython_mcp2515.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-24 19:17:30.000000 adafruit-circuitpython-mcp2515-1.1.1/adafruit_circuitpython_mcp2515.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-24 19:17:30.000000 adafruit-circuitpython-mcp2515-1.1.1/adafruit_circuitpython_mcp2515.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:17:30.137586 adafruit-circuitpython-mcp2515-1.1.1/adafruit_mcp2515/
+-rw-r--r--   0 runner    (1001) docker     (123)    31200 2023-04-24 19:17:20.000000 adafruit-circuitpython-mcp2515-1.1.1/adafruit_mcp2515/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:17:30.137586 adafruit-circuitpython-mcp2515-1.1.1/adafruit_mcp2515/canio/
+-rw-r--r--   0 runner    (1001) docker     (123)     7486 2023-04-24 19:17:20.000000 adafruit-circuitpython-mcp2515-1.1.1/adafruit_mcp2515/canio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-24 19:17:20.000000 adafruit-circuitpython-mcp2515-1.1.1/adafruit_mcp2515/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:17:30.137586 adafruit-circuitpython-mcp2515-1.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:17:30.137586 adafruit-circuitpython-mcp2515-1.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:17:30.137586 adafruit-circuitpython-mcp2515-1.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    14883 2023-04-24 19:17:20.000000 adafruit-circuitpython-mcp2515-1.1.1/examples/mcp2515_canio_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-24 19:17:20.000000 adafruit-circuitpython-mcp2515-1.1.1/examples/mcp2515_loopback_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-24 19:17:20.000000 adafruit-circuitpython-mcp2515-1.1.1/examples/mcp2515_receive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-24 19:17:20.000000 adafruit-circuitpython-mcp2515-1.1.1/examples/mcp2515_send_and_receive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-24 19:17:20.000000 adafruit-circuitpython-mcp2515-1.1.1/examples/mcp2515_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-24 19:17:20.000000 adafruit-circuitpython-mcp2515-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-24 19:17:07.000000 adafruit-circuitpython-mcp2515-1.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 19:17:30.137586 adafruit-circuitpython-mcp2515-1.1.1/setup.cfg
```

### Comparing `adafruit-circuitpython-mcp2515-1.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-mcp2515-1.1.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.0/.gitignore` & `adafruit-circuitpython-mcp2515-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.0/.pre-commit-config.yaml` & `adafruit-circuitpython-mcp2515-1.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.0/.pylintrc` & `adafruit-circuitpython-mcp2515-1.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.0/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-mcp2515-1.1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.0/LICENSE` & `adafruit-circuitpython-mcp2515-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.0/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-mcp2515-1.1.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.0/LICENSES/MIT.txt` & `adafruit-circuitpython-mcp2515-1.1.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.0/LICENSES/Unlicense.txt` & `adafruit-circuitpython-mcp2515-1.1.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.0/PKG-INFO` & `adafruit-circuitpython-mcp2515-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-mcp2515
-Version: 1.1.0
+Version: 1.1.1
 Summary: A CircuitPython library for working with the MCP2515 CAN bus controller
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MCP2515
 Keywords: adafruit,blinka,circuitpython,micropython,mcp2515,CAN,CANBUS,OBD
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-mcp2515-1.1.0/README.rst` & `adafruit-circuitpython-mcp2515-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.0/adafruit_circuitpython_mcp2515.egg-info/PKG-INFO` & `adafruit-circuitpython-mcp2515-1.1.1/adafruit_circuitpython_mcp2515.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-mcp2515
-Version: 1.1.0
+Version: 1.1.1
 Summary: A CircuitPython library for working with the MCP2515 CAN bus controller
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MCP2515
 Keywords: adafruit,blinka,circuitpython,micropython,mcp2515,CAN,CANBUS,OBD
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-mcp2515-1.1.0/adafruit_circuitpython_mcp2515.egg-info/SOURCES.txt` & `adafruit-circuitpython-mcp2515-1.1.1/adafruit_circuitpython_mcp2515.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.0/adafruit_mcp2515/__init__.py` & `adafruit-circuitpython-mcp2515-1.1.1/adafruit_mcp2515/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from .timer import Timer
 
 try:
     from typing_extensions import Literal
 except ImportError:
     pass
 
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MCP2515.git"
 
 # modes
 _MODE_NORMAL = const(0x00)
 _MODE_SLEEP = const(0x20)
 _MODE_LOOPBACK = const(0x40)
 _MODE_LISTENONLY = const(0x60)
@@ -154,22 +154,16 @@
 # REC: RECEIVE ERROR COUNTER REGISTER (ADDRESS: 1Dh)
 _EFLG = const(0x2D)
 
 ############ Misc Consts #########
 _SEND_TIMEOUT_MS = const(5)  # 500ms
 _MAX_CAN_MSG_LEN = 8  # ?!
 # perhaps this will be stateful later?
-TransmitBuffer = namedtuple(
-    "TransmitBuffer",
-    ["CTRL_REG", "STD_ID_REG", "INT_FLAG_MASK", "LOAD_CMD", "SEND_CMD"],
-)
-
-# perhaps this will be stateful later? #TODO : dedup with above
-ReceiveBuffer = namedtuple(
-    "TransmitBuffer",
+_TransmitBuffer = namedtuple(
+    "_TransmitBuffer",
     ["CTRL_REG", "STD_ID_REG", "INT_FLAG_MASK", "LOAD_CMD", "SEND_CMD"],
 )
 
 #    ---   Baud Rates Table   ---
 # Values for the 8MHz and 10MHz Crystal Oscillator are based on this calculator:
 # https://www.kvaser.com/support/calculators/bit-timing-calculator/
 # - MCP2510 can be used to calculate the timing values since the registers are allmost the same
@@ -262,49 +256,47 @@
         out_str += " Message sent"
     out_str += " Priority: " + ["LAST", "LOW", "MEDIUM", "HIGH"][status_byte & 0x3]
 
     return out_str
 
 
 class MCP2515:  # pylint:disable=too-many-instance-attributes
-    """A common shared-bus protocol."""
-
-    def __init__(
-        self,
-        spi_bus,
-        cs_pin,
-        *,
-        baudrate: int = 250000,
-        crystal_freq: Literal[8000000, 10000000, 16000000] = 16000000,
-        loopback: bool = False,
-        silent: bool = False,
-        auto_restart: bool = False,
-        debug: bool = False,
-    ):
-        """A common shared-bus protocol.
+    """A common shared-bus protocol.
 
         :param ~busio.SPI spi: The SPI bus used to communicate with the MCP2515
         :param ~digitalio.DigitalInOut cs_pin:  SPI bus enable pin
-        :param int baudrate: The bit rate of the bus in Hz, using a 16Mhz crystal. All devices on\
+        :param int baudrate: The bit rate of the bus in Hz. All devices on\
             the bus must agree on this value. Defaults to 250000.
         :param Literal crystal_freq: MCP2515 crystal frequency. Valid values are:\
             16000000, 10000000 and 8000000. Defaults to 16000000 (16MHz).\
         :param bool loopback: Receive only packets sent from this device, and send only to this\
         device. Requires that `silent` is also set to `True`, but only prevents transmission to\
         other devices. Otherwise the send/receive behavior is normal.
         :param bool silent: When `True` the controller does not transmit and all messages are\
         received, ignoring errors and filters. This mode can be used to “sniff” a CAN bus without\
         interfering. Defaults to `False`.
         :param bool auto_restart: **Not supported by hardware. An `AttributeError` will be raised\
         if `auto_restart` is set to `True`** If `True`, will restart communications after entering\
         bus-off state. Defaults to `False`.
-
         :param bool debug: If `True`, will enable printing debug information. Defaults to `False`.
         """
 
+    def __init__(
+        self,
+        spi_bus,
+        cs_pin,
+        *,
+        baudrate: int = 250000,
+        crystal_freq: Literal[8000000, 10000000, 16000000] = 16000000,
+        loopback: bool = False,
+        silent: bool = False,
+        auto_restart: bool = False,
+        debug: bool = False,
+    ):
+
         if loopback and not silent:
             raise AttributeError("Loopback mode requires silent to be set")
         if auto_restart:
             raise AttributeError("`auto-restart` is not supported by hardware")
 
         self._auto_restart = auto_restart
         self._debug = debug
@@ -328,29 +320,29 @@
 
         self._init_buffers()
         self.initialize()
 
     def _init_buffers(self):
 
         self._tx_buffers = [
-            TransmitBuffer(
+            _TransmitBuffer(
                 CTRL_REG=_TXB0CTRL,
                 STD_ID_REG=_TXB0SIDH,
                 INT_FLAG_MASK=_TX0IF,
                 LOAD_CMD=_LOAD_TX0,
                 SEND_CMD=_SEND_TX0,
             ),
-            TransmitBuffer(
+            _TransmitBuffer(
                 CTRL_REG=_TXB1CTRL,
                 STD_ID_REG=_TXB1SIDH,
                 INT_FLAG_MASK=_TX1IF,
                 LOAD_CMD=_LOAD_TX1,
                 SEND_CMD=_SEND_TX1,
             ),
-            TransmitBuffer(
+            _TransmitBuffer(
                 CTRL_REG=_TXB2CTRL,
                 STD_ID_REG=_TXB2SIDH,
                 INT_FLAG_MASK=_TX2IF,
                 LOAD_CMD=_LOAD_TX2,
                 SEND_CMD=_SEND_TX2,
             ),
         ]
```

### Comparing `adafruit-circuitpython-mcp2515-1.1.0/adafruit_mcp2515/canio/__init__.py` & `adafruit-circuitpython-mcp2515-1.1.1/adafruit_mcp2515/canio/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,37 +4,38 @@
 """Python implementation of the CircuitPython core `canio` API"""
 # pylint:disable=too-few-public-methods, invalid-name, redefined-builtin
 import time
 from ..timer import Timer
 
 
 class Message:
-    """A class representing a CANbus data frame"""
+    """A class representing a CANbus data frame
+
+    :param int id: The numeric ID of the message
+    :param bytes data: The content of the message, from 0 to 8 bytes of data
+    :param bool extended: True if the message has an extended identifier,
+        False if it has a standard identifier
+    """
 
     # pylint:disable=too-many-arguments,invalid-name,redefined-builtin
     def __init__(self, id, data, extended=False):
-        """Create a `Message` to send
-
-        Args:
-            id (int): The numeric ID of the message
-            data (bytes): The content of the message
-            extended (bool): True if the
-        Raises:
-            AttributeError: If `data` of type `bytes` is not provided for a non-RTR message
-            AttributeError: If `data` is larger than 8 bytes
-        """
-
         self._data = None
         self.id = id
         self.data = data
         self.extended = extended
 
+    id: int
+    """The numeric ID of the message"""
+
+    extended: bool
+    """Indicates whether the the message has an extended identifier"""
+
     @property
     def data(self):
-        """The content of the message, or dummy content in the case of an rtr"""
+        """The content of the message"""
         return self._data
 
     @data.setter
     def data(self, new_data):
         if (new_data is None) or (not (type(new_data) in [bytes, bytearray])):
 
             raise AttributeError(
@@ -46,48 +47,61 @@
             )
         # self.rtr = False
         # self._data = new_data
         self._data = bytearray(new_data)
 
 
 class RemoteTransmissionRequest:
-    """A class representing a CANbus remote frame"""
-
-    def __init__(self, id: int, length: int, *, extended: bool = False):
-        """Construct a RemoteTransmissionRequest to send on a CAN bus
+    """A class representing a CANbus remote frame
 
-        Args:
-            id (int): The numeric ID of the requested message
-            length (int): The length of the requested message
-            extended (bool, optional): True if the message has an extended identifier, False if it\
-                has a standard identifier. Defaults to False.
+    :param int id: The numeric ID of the message
+    :param length int: The length of the requested message
+    :param bool extended: True if the message has an extended identifier,
+        False if it has a standard identifier
+    """
 
-        """
+    def __init__(self, id: int, length: int, *, extended: bool = False):
         self.id = id
         self.length = length
         self.extended = extended
 
+    id: int
+    """The numeric ID of the message"""
+
+    extended: bool
+    """Indicates whether the the message has an extended identifier"""
+
+    length: int
+    """The length of the requested message, from 0 to 8"""
+
+
+# Replace the above implementation with core canio implementation if it is available
+try:
+    from canio import Message, RemoteTransmissionRequest
+except ImportError:
+    pass
+
 
 class Listener:
     """Listens for a CAN message
 
-        canio.Listener is not constructed directly, but instead by calling the `listen` method of a\
-        canio.CAN object.
+    canio.Listener is not constructed directly, but instead by calling the
+    ``listen`` method of a canio.CAN object.
     """
 
     def __init__(self, can_bus_obj, timeout=1.0):
         self._timer = Timer()
         self._can_bus_obj = can_bus_obj
         self._timeout = None
         self.timeout = timeout
 
     @property
     def timeout(self):
-        """The maximum amount of time in seconds that `read` or `readinto` will wait before giving\
-            up"""
+        """The maximum amount of time in seconds that ``read`` or ``readinto``
+        will wait before giving up"""
         return self._timeout
 
     @timeout.setter
     def timeout(self, timeout):
         self._timeout = float(timeout)
 
     def receive(self):
```

### Comparing `adafruit-circuitpython-mcp2515-1.1.0/adafruit_mcp2515/timer.py` & `adafruit-circuitpython-mcp2515-1.1.1/adafruit_mcp2515/timer.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.0/docs/_static/favicon.ico` & `adafruit-circuitpython-mcp2515-1.1.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.0/docs/conf.py` & `adafruit-circuitpython-mcp2515-1.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.0/docs/index.rst` & `adafruit-circuitpython-mcp2515-1.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.0/examples/mcp2515_canio_test.py` & `adafruit-circuitpython-mcp2515-1.1.1/examples/mcp2515_canio_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.0/examples/mcp2515_loopback_test.py` & `adafruit-circuitpython-mcp2515-1.1.1/examples/mcp2515_loopback_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.0/examples/mcp2515_receive.py` & `adafruit-circuitpython-mcp2515-1.1.1/examples/mcp2515_receive.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.0/examples/mcp2515_send_and_receive.py` & `adafruit-circuitpython-mcp2515-1.1.1/examples/mcp2515_send_and_receive.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.0/examples/mcp2515_simpletest.py` & `adafruit-circuitpython-mcp2515-1.1.1/examples/mcp2515_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp2515-1.1.0/pyproject.toml` & `adafruit-circuitpython-mcp2515-1.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-mcp2515"
 description = "A CircuitPython library for working with the MCP2515 CAN bus controller"
-version = "1.1.0"
+version = "1.1.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_MCP2515"}
 keywords = [
     "adafruit",
```


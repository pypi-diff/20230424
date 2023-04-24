# Comparing `tmp/adafruit-circuitpython-httpserver-3.0.0.tar.gz` & `tmp/adafruit-circuitpython-httpserver-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-httpserver-3.0.0.tar", last modified: Mon Apr 24 14:34:07 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-httpserver-3.0.1.tar", last modified: Mon Apr 24 14:38:51 2023, max compression
```

## Comparing `adafruit-circuitpython-httpserver-3.0.0.tar` & `adafruit-circuitpython-httpserver-3.0.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:34:07.648537 adafruit-circuitpython-httpserver-3.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:34:07.636538 adafruit-circuitpython-httpserver-3.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:34:07.640538 adafruit-circuitpython-httpserver-3.0.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-24 14:33:41.000000 adafruit-circuitpython-httpserver-3.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:34:07.640538 adafruit-circuitpython-httpserver-3.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-24 14:33:41.000000 adafruit-circuitpython-httpserver-3.0.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-24 14:33:41.000000 adafruit-circuitpython-httpserver-3.0.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-24 14:33:41.000000 adafruit-circuitpython-httpserver-3.0.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-24 14:33:41.000000 adafruit-circuitpython-httpserver-3.0.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-24 14:33:41.000000 adafruit-circuitpython-httpserver-3.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-24 14:33:41.000000 adafruit-circuitpython-httpserver-3.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-24 14:33:41.000000 adafruit-circuitpython-httpserver-3.0.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-24 14:33:41.000000 adafruit-circuitpython-httpserver-3.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-04-24 14:33:41.000000 adafruit-circuitpython-httpserver-3.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-24 14:33:41.000000 adafruit-circuitpython-httpserver-3.0.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:34:07.640538 adafruit-circuitpython-httpserver-3.0.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-24 14:33:41.000000 adafruit-circuitpython-httpserver-3.0.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-24 14:33:41.000000 adafruit-circuitpython-httpserver-3.0.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-24 14:33:41.000000 adafruit-circuitpython-httpserver-3.0.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-04-24 14:34:07.648537 adafruit-circuitpython-httpserver-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-04-24 14:33:41.000000 adafruit-circuitpython-httpserver-3.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-24 14:33:41.000000 adafruit-circuitpython-httpserver-3.0.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:34:07.644538 adafruit-circuitpython-httpserver-3.0.0/adafruit_circuitpython_httpserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-04-24 14:34:07.000000 adafruit-circuitpython-httpserver-3.0.0/adafruit_circuitpython_httpserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-24 14:34:07.000000 adafruit-circuitpython-httpserver-3.0.0/adafruit_circuitpython_httpserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 14:34:07.000000 adafruit-circuitpython-httpserver-3.0.0/adafruit_circuitpython_httpserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-24 14:34:07.000000 adafruit-circuitpython-httpserver-3.0.0/adafruit_circuitpython_httpserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-24 14:34:07.000000 adafruit-circuitpython-httpserver-3.0.0/adafruit_circuitpython_httpserver.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:34:07.644538 adafruit-circuitpython-httpserver-3.0.0/adafruit_httpserver/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-24 14:33:58.000000 adafruit-circuitpython-httpserver-3.0.0/adafruit_httpserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-24 14:33:58.000000 adafruit-circuitpython-httpserver-3.0.0/adafruit_httpserver/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-24 14:33:58.000000 adafruit-circuitpython-httpserver-3.0.0/adafruit_httpserver/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-24 14:33:58.000000 adafruit-circuitpython-httpserver-3.0.0/adafruit_httpserver/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-24 14:33:58.000000 adafruit-circuitpython-httpserver-3.0.0/adafruit_httpserver/mime_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-04-24 14:33:58.000000 adafruit-circuitpython-httpserver-3.0.0/adafruit_httpserver/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     9549 2023-04-24 14:33:58.000000 adafruit-circuitpython-httpserver-3.0.0/adafruit_httpserver/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-04-24 14:33:58.000000 adafruit-circuitpython-httpserver-3.0.0/adafruit_httpserver/route.py
--rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-04-24 14:33:58.000000 adafruit-circuitpython-httpserver-3.0.0/adafruit_httpserver/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-24 14:33:58.000000 adafruit-circuitpython-httpserver-3.0.0/adafruit_httpserver/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:34:07.648537 adafruit-circuitpython-httpserver-3.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:34:07.648537 adafruit-circuitpython-httpserver-3.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-24 14:33:41.000000 adafruit-circuitpython-httpserver-3.0.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-24 14:33:41.000000 adafruit-circuitpython-httpserver-3.0.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-24 14:33:41.000000 adafruit-circuitpython-httpserver-3.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-24 14:33:41.000000 adafruit-circuitpython-httpserver-3.0.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-04-24 14:33:41.000000 adafruit-circuitpython-httpserver-3.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-04-24 14:33:41.000000 adafruit-circuitpython-httpserver-3.0.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-24 14:33:41.000000 adafruit-circuitpython-httpserver-3.0.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-24 14:33:41.000000 adafruit-circuitpython-httpserver-3.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-24 14:33:41.000000 adafruit-circuitpython-httpserver-3.0.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-24 14:33:41.000000 adafruit-circuitpython-httpserver-3.0.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:34:07.648537 adafruit-circuitpython-httpserver-3.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-24 14:33:58.000000 adafruit-circuitpython-httpserver-3.0.0/examples/httpserver_chunked.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-24 14:33:58.000000 adafruit-circuitpython-httpserver-3.0.0/examples/httpserver_cpu_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-24 14:33:58.000000 adafruit-circuitpython-httpserver-3.0.0/examples/httpserver_mdns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-24 14:33:58.000000 adafruit-circuitpython-httpserver-3.0.0/examples/httpserver_neopixel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-24 14:33:58.000000 adafruit-circuitpython-httpserver-3.0.0/examples/httpserver_simple_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-24 14:33:58.000000 adafruit-circuitpython-httpserver-3.0.0/examples/httpserver_simple_serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-24 14:33:58.000000 adafruit-circuitpython-httpserver-3.0.0/examples/httpserver_url_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-24 14:33:41.000000 adafruit-circuitpython-httpserver-3.0.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-24 14:33:58.000000 adafruit-circuitpython-httpserver-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-24 14:33:41.000000 adafruit-circuitpython-httpserver-3.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 14:34:07.648537 adafruit-circuitpython-httpserver-3.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:38:51.094157 adafruit-circuitpython-httpserver-3.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:38:51.078158 adafruit-circuitpython-httpserver-3.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:38:51.082157 adafruit-circuitpython-httpserver-3.0.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-24 14:38:30.000000 adafruit-circuitpython-httpserver-3.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:38:51.086157 adafruit-circuitpython-httpserver-3.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-24 14:38:30.000000 adafruit-circuitpython-httpserver-3.0.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-24 14:38:30.000000 adafruit-circuitpython-httpserver-3.0.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-24 14:38:30.000000 adafruit-circuitpython-httpserver-3.0.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-24 14:38:30.000000 adafruit-circuitpython-httpserver-3.0.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-24 14:38:30.000000 adafruit-circuitpython-httpserver-3.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-24 14:38:30.000000 adafruit-circuitpython-httpserver-3.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-24 14:38:30.000000 adafruit-circuitpython-httpserver-3.0.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-24 14:38:30.000000 adafruit-circuitpython-httpserver-3.0.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-04-24 14:38:30.000000 adafruit-circuitpython-httpserver-3.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-24 14:38:30.000000 adafruit-circuitpython-httpserver-3.0.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:38:51.086157 adafruit-circuitpython-httpserver-3.0.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-24 14:38:30.000000 adafruit-circuitpython-httpserver-3.0.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-24 14:38:30.000000 adafruit-circuitpython-httpserver-3.0.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-24 14:38:30.000000 adafruit-circuitpython-httpserver-3.0.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-04-24 14:38:51.094157 adafruit-circuitpython-httpserver-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-04-24 14:38:30.000000 adafruit-circuitpython-httpserver-3.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-24 14:38:30.000000 adafruit-circuitpython-httpserver-3.0.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:38:51.086157 adafruit-circuitpython-httpserver-3.0.1/adafruit_circuitpython_httpserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-04-24 14:38:51.000000 adafruit-circuitpython-httpserver-3.0.1/adafruit_circuitpython_httpserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-24 14:38:51.000000 adafruit-circuitpython-httpserver-3.0.1/adafruit_circuitpython_httpserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 14:38:51.000000 adafruit-circuitpython-httpserver-3.0.1/adafruit_circuitpython_httpserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-24 14:38:51.000000 adafruit-circuitpython-httpserver-3.0.1/adafruit_circuitpython_httpserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-24 14:38:51.000000 adafruit-circuitpython-httpserver-3.0.1/adafruit_circuitpython_httpserver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:38:51.090157 adafruit-circuitpython-httpserver-3.0.1/adafruit_httpserver/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-24 14:38:43.000000 adafruit-circuitpython-httpserver-3.0.1/adafruit_httpserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-24 14:38:43.000000 adafruit-circuitpython-httpserver-3.0.1/adafruit_httpserver/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-24 14:38:43.000000 adafruit-circuitpython-httpserver-3.0.1/adafruit_httpserver/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-24 14:38:43.000000 adafruit-circuitpython-httpserver-3.0.1/adafruit_httpserver/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-24 14:38:43.000000 adafruit-circuitpython-httpserver-3.0.1/adafruit_httpserver/mime_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-04-24 14:38:43.000000 adafruit-circuitpython-httpserver-3.0.1/adafruit_httpserver/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9571 2023-04-24 14:38:43.000000 adafruit-circuitpython-httpserver-3.0.1/adafruit_httpserver/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-04-24 14:38:43.000000 adafruit-circuitpython-httpserver-3.0.1/adafruit_httpserver/route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-04-24 14:38:43.000000 adafruit-circuitpython-httpserver-3.0.1/adafruit_httpserver/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-24 14:38:43.000000 adafruit-circuitpython-httpserver-3.0.1/adafruit_httpserver/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:38:51.094157 adafruit-circuitpython-httpserver-3.0.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:38:51.094157 adafruit-circuitpython-httpserver-3.0.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-24 14:38:30.000000 adafruit-circuitpython-httpserver-3.0.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-24 14:38:30.000000 adafruit-circuitpython-httpserver-3.0.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-24 14:38:30.000000 adafruit-circuitpython-httpserver-3.0.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-24 14:38:30.000000 adafruit-circuitpython-httpserver-3.0.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-04-24 14:38:30.000000 adafruit-circuitpython-httpserver-3.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-04-24 14:38:30.000000 adafruit-circuitpython-httpserver-3.0.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-24 14:38:30.000000 adafruit-circuitpython-httpserver-3.0.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-24 14:38:30.000000 adafruit-circuitpython-httpserver-3.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-24 14:38:30.000000 adafruit-circuitpython-httpserver-3.0.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-24 14:38:30.000000 adafruit-circuitpython-httpserver-3.0.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:38:51.094157 adafruit-circuitpython-httpserver-3.0.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-24 14:38:43.000000 adafruit-circuitpython-httpserver-3.0.1/examples/httpserver_chunked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-24 14:38:43.000000 adafruit-circuitpython-httpserver-3.0.1/examples/httpserver_cpu_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-24 14:38:43.000000 adafruit-circuitpython-httpserver-3.0.1/examples/httpserver_mdns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-24 14:38:43.000000 adafruit-circuitpython-httpserver-3.0.1/examples/httpserver_neopixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-24 14:38:43.000000 adafruit-circuitpython-httpserver-3.0.1/examples/httpserver_simple_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-24 14:38:43.000000 adafruit-circuitpython-httpserver-3.0.1/examples/httpserver_simple_serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-24 14:38:43.000000 adafruit-circuitpython-httpserver-3.0.1/examples/httpserver_url_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-24 14:38:30.000000 adafruit-circuitpython-httpserver-3.0.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-24 14:38:43.000000 adafruit-circuitpython-httpserver-3.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-24 14:38:30.000000 adafruit-circuitpython-httpserver-3.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 14:38:51.094157 adafruit-circuitpython-httpserver-3.0.1/setup.cfg
```

### Comparing `adafruit-circuitpython-httpserver-3.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-httpserver-3.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.0/.gitignore` & `adafruit-circuitpython-httpserver-3.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.0/.pre-commit-config.yaml` & `adafruit-circuitpython-httpserver-3.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.0/.pylintrc` & `adafruit-circuitpython-httpserver-3.0.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.0/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-httpserver-3.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.0/LICENSE` & `adafruit-circuitpython-httpserver-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.0/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-httpserver-3.0.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.0/LICENSES/MIT.txt` & `adafruit-circuitpython-httpserver-3.0.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.0/LICENSES/Unlicense.txt` & `adafruit-circuitpython-httpserver-3.0.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.0/PKG-INFO` & `adafruit-circuitpython-httpserver-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-httpserver
-Version: 3.0.0
+Version: 3.0.1
 Summary: Simple HTTP Server for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_HTTPServer.git
 Keywords: adafruit,blinka,circuitpython,micropython,httpserver,web,server,webserver,http
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-httpserver-3.0.0/README.rst` & `adafruit-circuitpython-httpserver-3.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.0/adafruit_circuitpython_httpserver.egg-info/PKG-INFO` & `adafruit-circuitpython-httpserver-3.0.1/adafruit_circuitpython_httpserver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-httpserver
-Version: 3.0.0
+Version: 3.0.1
 Summary: Simple HTTP Server for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_HTTPServer.git
 Keywords: adafruit,blinka,circuitpython,micropython,httpserver,web,server,webserver,http
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-httpserver-3.0.0/adafruit_circuitpython_httpserver.egg-info/SOURCES.txt` & `adafruit-circuitpython-httpserver-3.0.1/adafruit_circuitpython_httpserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.0/adafruit_httpserver/__init__.py` & `adafruit-circuitpython-httpserver-3.0.1/adafruit_httpserver/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 """
 
-__version__ = "3.0.0"
+__version__ = "3.0.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_HTTPServer.git"
```

### Comparing `adafruit-circuitpython-httpserver-3.0.0/adafruit_httpserver/exceptions.py` & `adafruit-circuitpython-httpserver-3.0.1/adafruit_httpserver/exceptions.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.0/adafruit_httpserver/headers.py` & `adafruit-circuitpython-httpserver-3.0.1/adafruit_httpserver/headers.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.0/adafruit_httpserver/methods.py` & `adafruit-circuitpython-httpserver-3.0.1/adafruit_httpserver/methods.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.0/adafruit_httpserver/mime_type.py` & `adafruit-circuitpython-httpserver-3.0.1/adafruit_httpserver/mime_type.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.0/adafruit_httpserver/request.py` & `adafruit-circuitpython-httpserver-3.0.1/adafruit_httpserver/request.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.0/adafruit_httpserver/response.py` & `adafruit-circuitpython-httpserver-3.0.1/adafruit_httpserver/response.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,7 +295,8 @@
             try:
                 bytes_sent += conn.send(view[bytes_sent:])
             except OSError as exc:
                 if exc.errno == EAGAIN:
                     continue
                 if exc.errno == ECONNRESET:
                     return
+                raise
```

### Comparing `adafruit-circuitpython-httpserver-3.0.0/adafruit_httpserver/route.py` & `adafruit-circuitpython-httpserver-3.0.1/adafruit_httpserver/route.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.0/adafruit_httpserver/server.py` & `adafruit-circuitpython-httpserver-3.0.1/adafruit_httpserver/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,14 +102,15 @@
         while b"\r\n\r\n" not in received_bytes:
             try:
                 length = sock.recv_into(self._buffer, len(self._buffer))
                 received_bytes += self._buffer[:length]
             except OSError as ex:
                 if ex.errno == ETIMEDOUT:
                     break
+                raise
             except Exception as ex:
                 raise ex
         return received_bytes
 
     def _receive_body_bytes(
         self,
         sock: Union["SocketPool.Socket", "socket.socket"],
@@ -120,14 +121,15 @@
         while len(received_body_bytes) < content_length:
             try:
                 length = sock.recv_into(self._buffer, len(self._buffer))
                 received_body_bytes += self._buffer[:length]
             except OSError as ex:
                 if ex.errno == ETIMEDOUT:
                     break
+                raise
             except Exception as ex:
                 raise ex
         return received_body_bytes[:content_length]
 
     def poll(self):
         """
         Call this method inside your main event loop to get the server to
```

### Comparing `adafruit-circuitpython-httpserver-3.0.0/adafruit_httpserver/status.py` & `adafruit-circuitpython-httpserver-3.0.1/adafruit_httpserver/status.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.0/docs/_static/favicon.ico` & `adafruit-circuitpython-httpserver-3.0.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.0/docs/api.rst` & `adafruit-circuitpython-httpserver-3.0.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.0/docs/conf.py` & `adafruit-circuitpython-httpserver-3.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.0/docs/examples.rst` & `adafruit-circuitpython-httpserver-3.0.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.0/docs/index.rst` & `adafruit-circuitpython-httpserver-3.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.0/examples/httpserver_chunked.py` & `adafruit-circuitpython-httpserver-3.0.1/examples/httpserver_chunked.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.0/examples/httpserver_cpu_information.py` & `adafruit-circuitpython-httpserver-3.0.1/examples/httpserver_cpu_information.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.0/examples/httpserver_mdns.py` & `adafruit-circuitpython-httpserver-3.0.1/examples/httpserver_mdns.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.0/examples/httpserver_neopixel.py` & `adafruit-circuitpython-httpserver-3.0.1/examples/httpserver_neopixel.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.0/examples/httpserver_simple_poll.py` & `adafruit-circuitpython-httpserver-3.0.1/examples/httpserver_simple_poll.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.0/examples/httpserver_simple_serve.py` & `adafruit-circuitpython-httpserver-3.0.1/examples/httpserver_simple_serve.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.0/examples/httpserver_url_parameters.py` & `adafruit-circuitpython-httpserver-3.0.1/examples/httpserver_url_parameters.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-3.0.0/pyproject.toml` & `adafruit-circuitpython-httpserver-3.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-httpserver"
 description = "Simple HTTP Server for CircuitPython"
-version = "3.0.0"
+version = "3.0.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_HTTPServer.git"}
 keywords = [
     "adafruit",
```


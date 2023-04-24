# Comparing `tmp/adafruit-circuitpython-pixel-framebuf-1.1.8.tar.gz` & `tmp/adafruit-circuitpython-pixel-framebuf-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-pixel-framebuf-1.1.8.tar", last modified: Mon Aug 22 19:01:08 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-pixel-framebuf-1.1.9.tar", last modified: Fri Aug 26 02:44:54 2022, max compression
```

## Comparing `adafruit-circuitpython-pixel-framebuf-1.1.8.tar` & `adafruit-circuitpython-pixel-framebuf-1.1.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:01:08.362098 adafruit-circuitpython-pixel-framebuf-1.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:01:08.358098 adafruit-circuitpython-pixel-framebuf-1.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:01:08.358098 adafruit-circuitpython-pixel-framebuf-1.1.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-22 19:00:42.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:01:08.358098 adafruit-circuitpython-pixel-framebuf-1.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-22 19:00:42.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-22 19:00:42.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-22 19:00:42.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-22 19:00:42.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-22 19:00:42.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16265 2022-08-22 19:00:42.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-22 19:00:42.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-08-22 19:00:42.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-08-22 19:00:42.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:01:08.362098 adafruit-circuitpython-pixel-framebuf-1.1.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-22 19:00:42.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-22 19:00:42.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-22 19:00:42.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4203 2022-08-22 19:01:08.362098 adafruit-circuitpython-pixel-framebuf-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3384 2022-08-22 19:00:42.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 19:00:42.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:01:08.362098 adafruit-circuitpython-pixel-framebuf-1.1.8/adafruit_circuitpython_pixel_framebuf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4203 2022-08-22 19:01:08.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/adafruit_circuitpython_pixel_framebuf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-08-22 19:01:08.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/adafruit_circuitpython_pixel_framebuf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 19:01:08.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/adafruit_circuitpython_pixel_framebuf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-08-22 19:01:08.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/adafruit_circuitpython_pixel_framebuf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-22 19:01:08.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/adafruit_circuitpython_pixel_framebuf.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)     4300 2022-08-22 19:00:58.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/adafruit_pixel_framebuf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:01:08.362098 adafruit-circuitpython-pixel-framebuf-1.1.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:01:08.362098 adafruit-circuitpython-pixel-framebuf-1.1.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-22 19:00:42.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-22 19:00:42.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-08-22 19:00:42.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 19:00:42.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5630 2022-08-22 19:00:42.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      686 2022-08-22 19:00:42.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 19:00:42.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1660 2022-08-22 19:00:42.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 19:00:42.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-22 19:00:42.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 19:01:08.362098 adafruit-circuitpython-pixel-framebuf-1.1.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     3178 2022-08-22 19:00:42.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/examples/blinka_16x16.png
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-08-22 19:00:42.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/examples/blinka_16x16.png.license
--rwxr-xr-x   0 runner    (1001) docker     (121)     1158 2022-08-22 19:00:58.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/examples/pixel_framebuf_16x16_animation.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      870 2022-08-22 19:00:58.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/examples/pixel_framebuf_32x8_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      737 2022-08-22 19:00:58.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/examples/pixel_framebuf_dotstar_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1165 2022-08-22 19:00:58.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/examples/pixel_framebuf_pillow_image.py
--rw-r--r--   0 runner    (1001) docker     (121)      707 2022-08-22 19:00:58.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/examples/pixel_framebuf_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 19:00:42.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1329 2022-08-22 19:00:58.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-08-22 19:00:42.000000 adafruit-circuitpython-pixel-framebuf-1.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-22 19:01:08.362098 adafruit-circuitpython-pixel-framebuf-1.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:44:54.218798 adafruit-circuitpython-pixel-framebuf-1.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:44:54.214798 adafruit-circuitpython-pixel-framebuf-1.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:44:54.218798 adafruit-circuitpython-pixel-framebuf-1.1.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-26 02:44:40.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:44:54.218798 adafruit-circuitpython-pixel-framebuf-1.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-26 02:44:40.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-26 02:44:40.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-26 02:44:40.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-26 02:44:40.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-26 02:44:40.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16265 2022-08-26 02:44:40.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-26 02:44:40.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-08-26 02:44:40.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-08-26 02:44:40.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:44:54.218798 adafruit-circuitpython-pixel-framebuf-1.1.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-26 02:44:40.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-26 02:44:40.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-26 02:44:40.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4203 2022-08-26 02:44:54.218798 adafruit-circuitpython-pixel-framebuf-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3384 2022-08-26 02:44:40.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:44:40.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:44:54.218798 adafruit-circuitpython-pixel-framebuf-1.1.9/adafruit_circuitpython_pixel_framebuf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4203 2022-08-26 02:44:54.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/adafruit_circuitpython_pixel_framebuf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-08-26 02:44:54.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/adafruit_circuitpython_pixel_framebuf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 02:44:54.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/adafruit_circuitpython_pixel_framebuf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-08-26 02:44:54.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/adafruit_circuitpython_pixel_framebuf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-26 02:44:54.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/adafruit_circuitpython_pixel_framebuf.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4300 2022-08-26 02:44:46.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/adafruit_pixel_framebuf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:44:54.218798 adafruit-circuitpython-pixel-framebuf-1.1.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:44:54.218798 adafruit-circuitpython-pixel-framebuf-1.1.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-26 02:44:40.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-26 02:44:40.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2022-08-26 02:44:40.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:44:40.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5850 2022-08-26 02:44:40.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      686 2022-08-26 02:44:40.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:44:40.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1660 2022-08-26 02:44:40.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:44:40.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-26 02:44:40.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:44:54.218798 adafruit-circuitpython-pixel-framebuf-1.1.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     3178 2022-08-26 02:44:40.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/examples/blinka_16x16.png
+-rw-r--r--   0 runner    (1001) docker     (121)      120 2022-08-26 02:44:40.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/examples/blinka_16x16.png.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1158 2022-08-26 02:44:46.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/examples/pixel_framebuf_16x16_animation.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      870 2022-08-26 02:44:46.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/examples/pixel_framebuf_32x8_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      737 2022-08-26 02:44:46.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/examples/pixel_framebuf_dotstar_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1165 2022-08-26 02:44:46.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/examples/pixel_framebuf_pillow_image.py
+-rw-r--r--   0 runner    (1001) docker     (121)      707 2022-08-26 02:44:46.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/examples/pixel_framebuf_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:44:40.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1329 2022-08-26 02:44:46.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      201 2022-08-26 02:44:40.000000 adafruit-circuitpython-pixel-framebuf-1.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 02:44:54.218798 adafruit-circuitpython-pixel-framebuf-1.1.9/setup.cfg
```

### Comparing `adafruit-circuitpython-pixel-framebuf-1.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-pixel-framebuf-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pixel-framebuf-1.1.8/.github/workflows/build.yml` & `adafruit-circuitpython-pixel-framebuf-1.1.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pixel-framebuf-1.1.8/.github/workflows/release.yml` & `adafruit-circuitpython-pixel-framebuf-1.1.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pixel-framebuf-1.1.8/.gitignore` & `adafruit-circuitpython-pixel-framebuf-1.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pixel-framebuf-1.1.8/.pre-commit-config.yaml` & `adafruit-circuitpython-pixel-framebuf-1.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pixel-framebuf-1.1.8/.pylintrc` & `adafruit-circuitpython-pixel-framebuf-1.1.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pixel-framebuf-1.1.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-pixel-framebuf-1.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pixel-framebuf-1.1.8/LICENSE` & `adafruit-circuitpython-pixel-framebuf-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pixel-framebuf-1.1.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-pixel-framebuf-1.1.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pixel-framebuf-1.1.8/LICENSES/MIT.txt` & `adafruit-circuitpython-pixel-framebuf-1.1.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pixel-framebuf-1.1.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-pixel-framebuf-1.1.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pixel-framebuf-1.1.8/PKG-INFO` & `adafruit-circuitpython-pixel-framebuf-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-pixel-framebuf
-Version: 1.1.8
+Version: 1.1.9
 Summary: Neopixel and Dotstar Framebuffer Helper
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Pixel_Framebuf
 Keywords: adafruit,blinka,circuitpython,micropython,pixel_framebuf,neopixel,framebuf,framebuffer,dotstar,matrix,animation,led,ws2812,ap102
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-pixel-framebuf-1.1.8/README.rst` & `adafruit-circuitpython-pixel-framebuf-1.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pixel-framebuf-1.1.8/adafruit_circuitpython_pixel_framebuf.egg-info/PKG-INFO` & `adafruit-circuitpython-pixel-framebuf-1.1.9/adafruit_circuitpython_pixel_framebuf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-pixel-framebuf
-Version: 1.1.8
+Version: 1.1.9
 Summary: Neopixel and Dotstar Framebuffer Helper
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Pixel_Framebuf
 Keywords: adafruit,blinka,circuitpython,micropython,pixel_framebuf,neopixel,framebuf,framebuffer,dotstar,matrix,animation,led,ws2812,ap102
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-pixel-framebuf-1.1.8/adafruit_circuitpython_pixel_framebuf.egg-info/SOURCES.txt` & `adafruit-circuitpython-pixel-framebuf-1.1.9/adafruit_circuitpython_pixel_framebuf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pixel-framebuf-1.1.8/adafruit_pixel_framebuf.py` & `adafruit-circuitpython-pixel-framebuf-1.1.9/adafruit_pixel_framebuf.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 # imports
 
 from micropython import const
 import adafruit_framebuf
 from adafruit_led_animation.grid import PixelGrid
 
-__version__ = "1.1.8"
+__version__ = "1.1.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Pixel_Framebuf.git"
 
 HORIZONTAL = const(1)
 VERTICAL = const(2)
 
 # pylint: disable=too-many-function-args
 class PixelFramebuffer(adafruit_framebuf.FrameBuffer):
```

### Comparing `adafruit-circuitpython-pixel-framebuf-1.1.8/docs/_static/favicon.ico` & `adafruit-circuitpython-pixel-framebuf-1.1.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pixel-framebuf-1.1.8/docs/conf.py` & `adafruit-circuitpython-pixel-framebuf-1.1.9/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # SPDX-FileCopyrightText: 2017 Scott Shawcroft, written for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import sys
+import datetime
 
 sys.path.insert(0, os.path.abspath(".."))
 
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
@@ -42,15 +43,22 @@
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "Adafruit Pixel_Framebuf Library"
-copyright = "2020 Melissa LeBlanc-Williams"
+creation_year = "2020"
+current_year = str(datetime.datetime.now().year)
+year_duration = (
+    current_year
+    if current_year == creation_year
+    else creation_year + " - " + current_year
+)
+copyright = year_duration + " Melissa LeBlanc-Williams"
 author = "Melissa LeBlanc-Williams"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
```

### Comparing `adafruit-circuitpython-pixel-framebuf-1.1.8/docs/examples.rst` & `adafruit-circuitpython-pixel-framebuf-1.1.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pixel-framebuf-1.1.8/docs/index.rst` & `adafruit-circuitpython-pixel-framebuf-1.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pixel-framebuf-1.1.8/examples/blinka_16x16.png` & `adafruit-circuitpython-pixel-framebuf-1.1.9/examples/blinka_16x16.png`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pixel-framebuf-1.1.8/examples/pixel_framebuf_16x16_animation.py` & `adafruit-circuitpython-pixel-framebuf-1.1.9/examples/pixel_framebuf_16x16_animation.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pixel-framebuf-1.1.8/examples/pixel_framebuf_32x8_test.py` & `adafruit-circuitpython-pixel-framebuf-1.1.9/examples/pixel_framebuf_32x8_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pixel-framebuf-1.1.8/examples/pixel_framebuf_dotstar_simpletest.py` & `adafruit-circuitpython-pixel-framebuf-1.1.9/examples/pixel_framebuf_dotstar_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pixel-framebuf-1.1.8/examples/pixel_framebuf_pillow_image.py` & `adafruit-circuitpython-pixel-framebuf-1.1.9/examples/pixel_framebuf_pillow_image.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pixel-framebuf-1.1.8/examples/pixel_framebuf_simpletest.py` & `adafruit-circuitpython-pixel-framebuf-1.1.9/examples/pixel_framebuf_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pixel-framebuf-1.1.8/pyproject.toml` & `adafruit-circuitpython-pixel-framebuf-1.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-pixel-framebuf"
 description = "Neopixel and Dotstar Framebuffer Helper"
-version = "1.1.8"
+version = "1.1.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Pixel_Framebuf"}
 keywords = [
     "adafruit",
```


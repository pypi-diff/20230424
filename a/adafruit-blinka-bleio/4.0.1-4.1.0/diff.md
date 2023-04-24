# Comparing `tmp/adafruit-blinka-bleio-4.0.1.tar.gz` & `tmp/adafruit-blinka-bleio-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-blinka-bleio-4.0.1.tar", last modified: Fri Apr 14 13:18:08 2023, max compression
+gzip compressed data, was "adafruit-blinka-bleio-4.1.0.tar", last modified: Mon Apr 24 16:01:13 2023, max compression
```

## Comparing `adafruit-blinka-bleio-4.0.1.tar` & `adafruit-blinka-bleio-4.1.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:18:08.976387 adafruit-blinka-bleio-4.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:18:08.968387 adafruit-blinka-bleio-4.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:18:08.968387 adafruit-blinka-bleio-4.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20709 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:18:08.972386 adafruit-blinka-bleio-4.0.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-04-14 13:18:08.976387 adafruit-blinka-bleio-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:18:08.972386 adafruit-blinka-bleio-4.0.1/_bleio/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-14 13:18:00.000000 adafruit-blinka-bleio-4.0.1/_bleio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-04-14 13:18:00.000000 adafruit-blinka-bleio-4.0.1/_bleio/address.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-14 13:18:00.000000 adafruit-blinka-bleio-4.0.1/_bleio/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-04-14 13:18:00.000000 adafruit-blinka-bleio-4.0.1/_bleio/characteristic_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    34364 2023-04-14 13:18:00.000000 adafruit-blinka-bleio-4.0.1/_bleio/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-04-14 13:18:00.000000 adafruit-blinka-bleio-4.0.1/_bleio/descriptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-14 13:18:00.000000 adafruit-blinka-bleio-4.0.1/_bleio/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-04-14 13:18:00.000000 adafruit-blinka-bleio-4.0.1/_bleio/packet_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-04-14 13:18:00.000000 adafruit-blinka-bleio-4.0.1/_bleio/scan_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-04-14 13:18:00.000000 adafruit-blinka-bleio-4.0.1/_bleio/uuid_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:18:08.972386 adafruit-blinka-bleio-4.0.1/adafruit_blinka_bleio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-04-14 13:18:08.000000 adafruit-blinka-bleio-4.0.1/adafruit_blinka_bleio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-14 13:18:08.000000 adafruit-blinka-bleio-4.0.1/adafruit_blinka_bleio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 13:18:08.000000 adafruit-blinka-bleio-4.0.1/adafruit_blinka_bleio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-14 13:18:08.000000 adafruit-blinka-bleio-4.0.1/adafruit_blinka_bleio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 13:18:08.000000 adafruit-blinka-bleio-4.0.1/adafruit_blinka_bleio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:18:08.972386 adafruit-blinka-bleio-4.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:18:08.972386 adafruit-blinka-bleio-4.0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/docs/index.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:18:08.972386 adafruit-blinka-bleio-4.0.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-14 13:18:00.000000 adafruit-blinka-bleio-4.0.1/examples/blinka_bleio_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 13:18:00.000000 adafruit-blinka-bleio-4.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-14 13:17:51.000000 adafruit-blinka-bleio-4.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 13:18:08.976387 adafruit-blinka-bleio-4.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:01:13.941667 adafruit-blinka-bleio-4.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:01:13.937667 adafruit-blinka-bleio-4.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:01:13.937667 adafruit-blinka-bleio-4.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-24 16:00:57.000000 adafruit-blinka-bleio-4.1.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-04-24 16:00:57.000000 adafruit-blinka-bleio-4.1.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-24 16:00:57.000000 adafruit-blinka-bleio-4.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-24 16:00:57.000000 adafruit-blinka-bleio-4.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20709 2023-04-24 16:00:57.000000 adafruit-blinka-bleio-4.1.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-24 16:00:57.000000 adafruit-blinka-bleio-4.1.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-04-24 16:00:57.000000 adafruit-blinka-bleio-4.1.0/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:01:13.937667 adafruit-blinka-bleio-4.1.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-24 16:00:57.000000 adafruit-blinka-bleio-4.1.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-24 16:00:57.000000 adafruit-blinka-bleio-4.1.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-24 16:00:57.000000 adafruit-blinka-bleio-4.1.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-04-24 16:01:13.941667 adafruit-blinka-bleio-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-04-24 16:00:57.000000 adafruit-blinka-bleio-4.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-24 16:00:57.000000 adafruit-blinka-bleio-4.1.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:01:13.937667 adafruit-blinka-bleio-4.1.0/_bleio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-24 16:01:06.000000 adafruit-blinka-bleio-4.1.0/_bleio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-04-24 16:01:06.000000 adafruit-blinka-bleio-4.1.0/_bleio/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-24 16:01:06.000000 adafruit-blinka-bleio-4.1.0/_bleio/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-04-24 16:01:06.000000 adafruit-blinka-bleio-4.1.0/_bleio/characteristic_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34364 2023-04-24 16:01:06.000000 adafruit-blinka-bleio-4.1.0/_bleio/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-04-24 16:01:06.000000 adafruit-blinka-bleio-4.1.0/_bleio/descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-24 16:01:06.000000 adafruit-blinka-bleio-4.1.0/_bleio/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-04-24 16:01:06.000000 adafruit-blinka-bleio-4.1.0/_bleio/packet_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-04-24 16:01:06.000000 adafruit-blinka-bleio-4.1.0/_bleio/scan_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-04-24 16:01:06.000000 adafruit-blinka-bleio-4.1.0/_bleio/uuid_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:01:13.941667 adafruit-blinka-bleio-4.1.0/adafruit_blinka_bleio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-04-24 16:01:13.000000 adafruit-blinka-bleio-4.1.0/adafruit_blinka_bleio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-24 16:01:13.000000 adafruit-blinka-bleio-4.1.0/adafruit_blinka_bleio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 16:01:13.000000 adafruit-blinka-bleio-4.1.0/adafruit_blinka_bleio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-24 16:01:13.000000 adafruit-blinka-bleio-4.1.0/adafruit_blinka_bleio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 16:01:13.000000 adafruit-blinka-bleio-4.1.0/adafruit_blinka_bleio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:01:13.941667 adafruit-blinka-bleio-4.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:01:13.941667 adafruit-blinka-bleio-4.1.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-24 16:00:57.000000 adafruit-blinka-bleio-4.1.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-24 16:00:57.000000 adafruit-blinka-bleio-4.1.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-24 16:00:57.000000 adafruit-blinka-bleio-4.1.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-24 16:00:57.000000 adafruit-blinka-bleio-4.1.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-04-24 16:00:57.000000 adafruit-blinka-bleio-4.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-24 16:00:57.000000 adafruit-blinka-bleio-4.1.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-24 16:00:57.000000 adafruit-blinka-bleio-4.1.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-24 16:00:57.000000 adafruit-blinka-bleio-4.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-24 16:00:57.000000 adafruit-blinka-bleio-4.1.0/docs/index.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:01:13.941667 adafruit-blinka-bleio-4.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-24 16:01:06.000000 adafruit-blinka-bleio-4.1.0/examples/blinka_bleio_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-24 16:00:57.000000 adafruit-blinka-bleio-4.1.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-24 16:01:06.000000 adafruit-blinka-bleio-4.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-24 16:00:57.000000 adafruit-blinka-bleio-4.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 16:01:13.941667 adafruit-blinka-bleio-4.1.0/setup.cfg
```

### Comparing `adafruit-blinka-bleio-4.0.1/.github/workflows/build.yml` & `adafruit-blinka-bleio-4.1.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-bleio-4.0.1/.github/workflows/release.yml` & `adafruit-blinka-bleio-4.1.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-bleio-4.0.1/.pre-commit-config.yaml` & `adafruit-blinka-bleio-4.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-bleio-4.0.1/.pylintrc` & `adafruit-blinka-bleio-4.1.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-bleio-4.0.1/CODE_OF_CONDUCT.md` & `adafruit-blinka-bleio-4.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-bleio-4.0.1/LICENSES/CC-BY-4.0.txt` & `adafruit-blinka-bleio-4.1.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-bleio-4.0.1/LICENSES/MIT.txt` & `adafruit-blinka-bleio-4.1.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-bleio-4.0.1/LICENSES/Unlicense.txt` & `adafruit-blinka-bleio-4.1.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-bleio-4.0.1/PKG-INFO` & `adafruit-blinka-bleio-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-blinka-bleio
-Version: 4.0.1
+Version: 4.1.0
 Summary: `_bleio` for Blinka based on `bleak`
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_Blinka_bleio.git
 Keywords: adafruit,blinka,circuitpython,micropython,blinka_bleio,bleio,bleak
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-blinka-bleio-4.0.1/README.rst` & `adafruit-blinka-bleio-4.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-bleio-4.0.1/_bleio/__init__.py` & `adafruit-blinka-bleio-4.1.0/_bleio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     RoleError,
     SecurityError,
 )
 from _bleio.packet_buffer import PacketBuffer
 from _bleio.scan_entry import ScanEntry
 from _bleio.uuid_ import UUID
 
-__version__ = "4.0.1"
+__version__ = "4.1.0"
 __repo__ = "https://github.com/adafruit/Adafruit_Blinka_bleio.git"
 
 
 def set_adapter(new_adapter: Optional[Adapter]) -> None:
     """Set the adapter to use for BLE, such as when using an HCI adapter.
     Raises `NotImplementedError` when the adapter is a singleton and cannot be set.
     """
```

### Comparing `adafruit-blinka-bleio-4.0.1/_bleio/address.py` & `adafruit-blinka-bleio-4.1.0/_bleio/address.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import annotations
 from typing import Any, Optional, Union
 
 import re
 
 Buf = Union[bytes, bytearray, memoryview]
 
-__version__ = "4.0.1"
+__version__ = "4.1.0"
 __repo__ = "https://github.com/adafruit/Adafruit_Blinka_bleio.git"
 
 
 class Address:
     PUBLIC = 0x0
     RANDOM_STATIC = 0x1
     RANDOM_PRIVATE_RESOLVABLE = 0x2
```

### Comparing `adafruit-blinka-bleio-4.0.1/_bleio/attribute.py` & `adafruit-blinka-bleio-4.1.0/_bleio/attribute.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ================================================================================
 
 `_bleio` for Blinka based on ``bleak``
 
 * Author(s): Dan Halbert
 """
 
-__version__ = "4.0.1"
+__version__ = "4.1.0"
 __repo__ = "https://github.com/adafruit/Adafruit_Blinka_bleio.git"
 
 from enum import Enum
 
 
 class Attribute(Enum):
     NO_ACCESS = 0x00
```

### Comparing `adafruit-blinka-bleio-4.0.1/_bleio/characteristic_buffer.py` & `adafruit-blinka-bleio-4.1.0/_bleio/characteristic_buffer.py`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-bleio-4.0.1/_bleio/common.py` & `adafruit-blinka-bleio-4.1.0/_bleio/common.py`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-bleio-4.0.1/_bleio/descriptor.py` & `adafruit-blinka-bleio-4.1.0/_bleio/descriptor.py`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-bleio-4.0.1/_bleio/exceptions.py` & `adafruit-blinka-bleio-4.1.0/_bleio/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 =======================================================================
 
 _bleio implementation for Adafruit_Blinka_bleio
 
 * Author(s): Dan Halbert for Adafruit Industries
 """
 
-__version__ = "4.0.1"
+__version__ = "4.1.0"
 __repo__ = "https://github.com/adafruit/Adafruit_Blinka_bleio.git"
 
 
 class BluetoothError(Exception):
     """Catch-all exception for Bluetooth related errors."""
```

### Comparing `adafruit-blinka-bleio-4.0.1/_bleio/packet_buffer.py` & `adafruit-blinka-bleio-4.1.0/_bleio/packet_buffer.py`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-bleio-4.0.1/_bleio/scan_entry.py` & `adafruit-blinka-bleio-4.1.0/_bleio/scan_entry.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,44 +145,63 @@
             return fields
 
         return tuple(
             bytes((data_type,)) + data for data_type, data in self._data_dict.items()
         )
 
     @staticmethod
+    def _manufacturer_data_from_bleak(manufacturer_data: Dict[int, bytes]) -> bytes:
+        # The manufacturer data value is a dictionary.
+        # Re-concatenate it into bytes
+        all_mfr_data = bytearray()
+        for mfr_id, mfr_data in manufacturer_data.items():
+            all_mfr_data.extend(mfr_id.to_bytes(2, byteorder="little"))
+            all_mfr_data.extend(mfr_data)
+        return bytes(all_mfr_data)
+
+    @staticmethod
+    def _uuids_from_bleak(uuids: List[str]) -> bytes:
+        uuids16 = bytearray()
+        uuids32 = bytearray()
+        uuids128 = bytearray()
+        for uuid in uuids:
+            bleio_uuid = UUID(uuid)
+            # If this is a Standard UUID in 128-bit form, convert it to a 16- or 32-bit UUID.
+            if bleio_uuid.is_standard_uuid:
+                if bleio_uuid.size == 16:
+                    uuids16.extend(bleio_uuid.uuid128[12:14])
+                elif bleio_uuid.size == 32:
+                    uuids32.extend(bleio_uuid.uuid128[12:16])
+                else:
+                    raise RuntimeError("Unexpected UUID size")
+            else:
+                uuids128.extend(bleio_uuid.uuid128)
+
+        fields = {}
+        if uuids16:
+            # Complete list of 16-bit UUIDs.
+            fields[0x03] = uuids16
+        if uuids32:
+            # Complete list of 32-bit UUIDs.
+            fields[0x05] = uuids32
+        if uuids128:
+            # Complete list of 128-bit UUIDs
+            fields[0x07] = uuids128
+        return fields
+
+    @staticmethod
     def _data_dict_from_bleak(
         device: BLEDevice, advertisement_data: AdvertisementData
     ) -> DataDict:
         data_dict = {}
         if manufacturer_data := advertisement_data.manufacturer_data:
-            # The manufacturer data value is a dictionary.
-            # Re-concatenate it into bytes
-            all_mfr_data = bytearray()
-            for mfr_id, mfr_data in manufacturer_data.items():
-                all_mfr_data.extend(mfr_id.to_bytes(2, byteorder="little"))
-                all_mfr_data.extend(mfr_data)
-            data_dict[0xFF] = all_mfr_data
+            data_dict[0xFF] = ScanEntry._manufacturer_data_from_bleak(manufacturer_data)
 
         if uuids := advertisement_data.service_uuids:
-            uuids16 = bytearray()
-            uuids128 = bytearray()
-            for uuid in uuids:
-                bleio_uuid = UUID(uuid)
-                # If this is a Standard UUID in 128-bit form, convert it to a 16-bit UUID.
-                if bleio_uuid.is_standard_uuid:
-                    uuids16.extend(bleio_uuid.uuid128[12:14])
-                else:
-                    uuids128.extend(bleio_uuid.uuid128)
-
-            if uuids16:
-                # Complete list of 16-bit UUIDs.
-                data_dict[0x03] = uuids16
-            if uuids128:
-                # Complete list of 128-bit UUIDs
-                data_dict[0x07] = uuids128
+            data_dict.update(ScanEntry._uuids_from_bleak(uuids))
 
         name = advertisement_data.local_name or device.name
         if name and not ScanEntry._RE_IGNORABLE_NAME.fullmatch(name):
             # Complete name
             data_dict[0x09] = name.encode("utf-8")
 
         return data_dict
```

### Comparing `adafruit-blinka-bleio-4.0.1/_bleio/uuid_.py` & `adafruit-blinka-bleio-4.1.0/_bleio/uuid_.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,91 +14,111 @@
 from __future__ import annotations
 from typing import Any, Union
 
 import re
 
 Buf = Union[bytes, bytearray, memoryview]
 
-__version__ = "4.0.1"
+__version__ = "4.1.0"
 __repo__ = "https://github.com/adafruit/Adafruit_Blinka_bleio.git"
 
 _UUID_RE = re.compile(
     r"[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}", flags=re.IGNORECASE
 )
 
-_STANDARD_UUID_RE = re.compile(
+_STANDARD_UUID_RE_16 = re.compile(
     r"0000....-0000-1000-8000-00805f9b34fb", flags=re.IGNORECASE
 )
 
-_STANDARD_HEX_UUID_RE = re.compile(r"[0-9a-f]{1,4}", flags=re.IGNORECASE)
+_STANDARD_UUID_RE_32 = re.compile(
+    r"........-0000-1000-8000-00805f9b34fb", flags=re.IGNORECASE
+)
+
+_STANDARD_HEX_UUID_RE = re.compile(r"[0-9a-f]{1,8}", flags=re.IGNORECASE)
 
 _BASE_STANDARD_UUID = (
     b"\xFB\x34\x9B\x5F\x80\x00\x00\x80\x00\x10\x00\x00\x00\x00\x00\x00"
 )
 
 
 class UUID:
+    @staticmethod
+    def standard_uuid128_from_uuid32(uuid32: int) -> bytes:
+        """Return a 128-bit standard UUID from a 32-bit standard UUID."""
+        if not 0 <= uuid32 < 2**32:
+            raise ValueError("UUID integer value must be unsigned 32-bit")
+        return _BASE_STANDARD_UUID[:-4] + uuid32.to_bytes(4, "little")
+
+    @staticmethod
+    def _init_from_str(uuid: str) -> tuple[bytes, int]:
+        if _UUID_RE.fullmatch(uuid):
+            # Pick the smallest standard size.
+            if _STANDARD_UUID_RE_16.fullmatch(uuid):
+                size = 16
+                uuid16 = int(uuid[4:8], 16)
+                uuid128 = UUID.standard_uuid128_from_uuid32(uuid16)
+                return uuid128, size
+
+            if _STANDARD_UUID_RE_32.fullmatch(uuid):
+                size = 32
+                uuid32 = int(uuid[0:8], 16)
+                uuid128 = UUID.standard_uuid128_from_uuid32(uuid32)
+                return uuid128, size
+
+            size = 128
+            uuid = uuid.replace("-", "")
+            uuid128 = bytes(int(uuid[i : i + 2], 16) for i in range(30, -1, -2))
+            return uuid128, size
+
+        if _STANDARD_HEX_UUID_RE.fullmatch(uuid) and len(uuid) in (4, 8):
+            # Fall through and reprocess as an int.
+            uuid_int = int(uuid, 16)
+            size = len(uuid) * 4  # 4 bits per hex digit
+            uuid128 = UUID.standard_uuid128_from_uuid32(uuid_int)
+            return uuid128, size
+
+        raise ValueError(
+            "UUID string not 'xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx',"
+            "'xxxx', or 'xxxxxxxx', but is " + uuid
+        )
+
+    @staticmethod
+    def _init_from_int(uuid: int) -> tuple[bytes, int]:
+        if not 0 <= uuid <= 2**32:
+            raise ValueError("UUID integer value must be unsigned 16- or 32-bit")
+        if uuid <= 2**16:
+            size = 16
+        if uuid <= 2**32:
+            size = 32
+        uuid128 = UUID.standard_uuid128_from_uuid32(uuid)
+        return uuid128, size
+
+    @staticmethod
+    def _init_from_buf(uuid: Buf) -> tuple[bytes, int]:
+        try:
+            uuid = memoryview(uuid)
+        except TypeError:
+            raise ValueError("UUID value is not str, int or byte buffer") from TypeError
+        if len(uuid) != 16:
+            raise ValueError("Byte buffer must be 16 bytes")
+        size = 128
+        uuid128 = bytes(uuid)
+        return uuid128, size
+
     def __init__(self, uuid: Union[int, Buf, str]):
         self.__bleak_uuid = None
 
         if isinstance(uuid, str):
-            if _UUID_RE.fullmatch(uuid):
-                self._size = 16 if _STANDARD_UUID_RE.fullmatch(uuid) else 128
-                uuid = uuid.replace("-", "")
-                self._uuid128 = bytes(
-                    int(uuid[i : i + 2], 16) for i in range(30, -1, -2)
-                )
-                return
-
-            if _STANDARD_HEX_UUID_RE.fullmatch(uuid):
-                # Fall through and reprocess as an int.
-                uuid = int(uuid, 16)
-            else:
-                raise ValueError(
-                    "UUID string not 'xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx' or 'xxxx', but is "
-                    + uuid
-                )
-
-        if isinstance(uuid, int):
-            if not 0 <= uuid <= 0xFFFF:
-                raise ValueError("UUID integer value must be 0-0xffff")
-            self._size = 16
-            self._uuid16 = uuid
-            # Put into "0000xxxx-0000-1000-8000-00805F9B34FB"
-            self._uuid128 = bytes(
-                (
-                    0xFB,
-                    0x34,
-                    0x9B,
-                    0x5F,
-                    0x80,
-                    0x00,  # 00805F9B34FB
-                    0x00,
-                    0x80,  # 8000
-                    0x00,
-                    0x10,  # 1000
-                    0x00,
-                    0x00,  # 0000
-                    uuid & 0xFF,
-                    (uuid >> 8) & 0xFF,  # xxxx
-                    0x00,
-                    0x00,
-                )
-            )  # 0000
+            self._uuid128, self._size = self._init_from_str(uuid)
+
+        elif isinstance(uuid, int):
+            self._uuid128, self._size = self._init_from_int(uuid)
+
         else:
-            try:
-                uuid = memoryview(uuid)
-            except TypeError:
-                raise ValueError(
-                    "UUID value is not str, int or byte buffer"
-                ) from TypeError
-            if len(uuid) != 16:
-                raise ValueError("Byte buffer must be 16 bytes")
-            self._size = 128
-            self._uuid128 = bytes(uuid)
+            self._uuid128, self._size = self._init_from_buf(uuid)
 
     @classmethod
     def _from_bleak(cls, bleak_uuid: Any) -> "UUID":
         """Convert a bleak UUID to a _bleio.UUID."""
         uuid = UUID(bleak_uuid)
         uuid.__bleak_uuid = bleak_uuid  # pylint: disable=unused-private-member
         return uuid
@@ -108,17 +128,23 @@
         """Bleak UUID"""
         if not self.__bleak_uuid:
             self.__bleak_uuid = str(self)
         return self.__bleak_uuid
 
     @property
     def uuid16(self) -> int:
-        if self.size == 128:
-            raise ValueError("This is a 128-bit UUID")
-        return (self._uuid128[13] << 8) | self._uuid128[12]
+        if self.size > 16:
+            raise ValueError(f"This is a {self.size}-bit UUID")
+        return int.from_bytes(self._uuid128[12:14], "little")
+
+    @property
+    def uuid32(self) -> int:
+        if self.size > 32:
+            raise ValueError(f"This is a {self.size}-bit UUID")
+        return int.from_bytes(self._uuid128[12:], "little")
 
     @property
     def uuid128(self) -> bytes:
         return self._uuid128
 
     @property
     def size(self) -> int:
@@ -126,46 +152,58 @@
 
     def pack_into(self, buffer, offset=0) -> None:
         byte_size = self.size // 8
         if len(buffer) - offset < byte_size:
             raise IndexError("Buffer offset too small")
         if self.size == 16:
             buffer[offset:byte_size] = self.uuid128[12:14]
+        elif self.size == 32:
+            buffer[offset:byte_size] = self.uuid128[12:]
         else:
             buffer[offset:byte_size] = self.uuid128
 
     @property
     def is_standard_uuid(self) -> bool:
-        """True if this is a standard 16-bit UUID (0000xxxx-0000-1000-8000-00805F9B34FB)
+        """True if this is a standard 16 or 32-bit UUID (xxxxxxxx-0000-1000-8000-00805F9B34FB)
         even if it's 128-bit."""
-        return self.size == 16 or (
-            self._uuid128[0:12] == _BASE_STANDARD_UUID[0:12]
-            and self._uuid128[14:] == _BASE_STANDARD_UUID[14:]
+        return (
+            self.size == 16
+            or self.size == 32
+            or (
+                self._uuid128[0:12] == _BASE_STANDARD_UUID[0:12]
+                and self._uuid128[14:] == _BASE_STANDARD_UUID[14:]
+            )
         )
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, UUID):
             if self.size == 16 and other.size == 16:
                 return self.uuid16 == other.uuid16
+            if self.size == 32 and other.size == 32:
+                return self.uuid32 == other.uuid32
             if self.size == 128 and other.size == 128:
                 return self.uuid128 == other.uuid128
 
         return False
 
     def __hash__(self):
         if self.size == 16:
             return hash(self.uuid16)
+        if self.size == 32:
+            return hash(self.uuid32)
         return hash(self.uuid128)
 
     def __str__(self) -> str:
         return (
             "{:02x}{:02x}{:02x}{:02x}-"  # pylint: disable=consider-using-f-string
             "{:02x}{:02x}-"
             "{:02x}{:02x}-"
             "{:02x}{:02x}-"
             "{:02x}{:02x}{:02x}{:02x}{:02x}{:02x}"
         ).format(*reversed(self.uuid128))
 
     def __repr__(self) -> str:
         if self.size == 16:
             return f"UUID({self.uuid16:#04x})"
+        if self.size == 32:
+            return f"UUID({self.uuid32:#08x})"
         return f"UUID({self!s})"
```

### Comparing `adafruit-blinka-bleio-4.0.1/adafruit_blinka_bleio.egg-info/PKG-INFO` & `adafruit-blinka-bleio-4.1.0/adafruit_blinka_bleio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-blinka-bleio
-Version: 4.0.1
+Version: 4.1.0
 Summary: `_bleio` for Blinka based on `bleak`
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_Blinka_bleio.git
 Keywords: adafruit,blinka,circuitpython,micropython,blinka_bleio,bleio,bleak
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-blinka-bleio-4.0.1/adafruit_blinka_bleio.egg-info/SOURCES.txt` & `adafruit-blinka-bleio-4.1.0/adafruit_blinka_bleio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-bleio-4.0.1/docs/_static/favicon.ico` & `adafruit-blinka-bleio-4.1.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-bleio-4.0.1/docs/api.rst` & `adafruit-blinka-bleio-4.1.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-bleio-4.0.1/docs/conf.py` & `adafruit-blinka-bleio-4.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-bleio-4.0.1/docs/index.rst` & `adafruit-blinka-bleio-4.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-blinka-bleio-4.0.1/pyproject.toml` & `adafruit-blinka-bleio-4.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "setuptools-scm",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "adafruit-blinka-bleio"
 description = "`_bleio` for Blinka based on `bleak`"
-version = "4.0.1"
+version = "4.1.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_Blinka_bleio.git"}
 keywords = [
     "adafruit",
```


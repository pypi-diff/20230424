# Comparing `tmp/qrplatba-1.1.0.tar.gz` & `tmp/qrplatba-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qrplatba-1.1.0.tar", max compression
+gzip compressed data, was "qrplatba-1.1.1.tar", max compression
```

## Comparing `qrplatba-1.1.0.tar` & `qrplatba-1.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1073 2023-04-05 13:15:39.538565 qrplatba-1.1.0/LICENSE
--rw-r--r--   0        0        0     2328 2023-04-05 13:15:39.538565 qrplatba-1.1.0/README.md
--rw-r--r--   0        0        0     1163 2023-04-05 13:15:39.538565 qrplatba-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       70 2023-04-05 13:15:39.538565 qrplatba-1.1.0/qrplatba/__init__.py
--rw-r--r--   0        0        0     5776 2023-04-05 13:15:39.538565 qrplatba-1.1.0/qrplatba/spayd.py
--rw-r--r--   0        0        0     4946 2023-04-05 13:15:39.538565 qrplatba-1.1.0/qrplatba/svg.py
--rw-r--r--   0        0        0     3516 1970-01-01 00:00:00.000000 qrplatba-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-24 11:25:37.367820 qrplatba-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2328 2023-04-24 11:25:37.367820 qrplatba-1.1.1/README.md
+-rw-r--r--   0        0        0     1163 2023-04-24 11:25:37.367820 qrplatba-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-04-24 11:25:37.367820 qrplatba-1.1.1/qrplatba/__init__.py
+-rw-r--r--   0        0        0     5776 2023-04-24 11:25:37.367820 qrplatba-1.1.1/qrplatba/spayd.py
+-rw-r--r--   0        0        0     4946 2023-04-24 11:25:37.367820 qrplatba-1.1.1/qrplatba/svg.py
+-rw-r--r--   0        0        0     3516 1970-01-01 00:00:00.000000 qrplatba-1.1.1/PKG-INFO
```

### Comparing `qrplatba-1.1.0/LICENSE` & `qrplatba-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qrplatba-1.1.0/README.md` & `qrplatba-1.1.1/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -48,25 +48,25 @@
 
 ## License
 
 This software is licensed under [MIT license](https://opensource.org/license/mit/) since version `1.0.0`.
 
 ## Changelog
 
+### `1.1.0` (5 April 2023)
+
+- Dropped support for Python 3.7
+- Added pre-commit, black and ruff for code formatting
+
 ### `1.0.0` (4 April 2023)
 
 **Warning:** While the API is mostly backwards compatible, the look and size of the generated QR codes has changed.
 
 - Updated requirements to support the latest `qrcode` version
 - Added support for custom output sizes using `box_size` and `border` parameters
 - Changed legacy setuptools to [poetry](https://python-poetry.org/)
 - Dropped support for Python `2.x` and `<3.7`
 - Changed license to MIT
 - Added unit tests
 
-### `1.1.0` (5 April 2023)
-
-- Dropped support for Python 3.7
-- Added pre-commit, black and ruff for code formatting
-
```

### Comparing `qrplatba-1.1.0/pyproject.toml` & `qrplatba-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qrplatba"
-version = "1.1.0"
+version = "1.1.1"
 description = "QR platba SVG QR code and SPAYD string generator."
 authors = ["Viktor Stískala <viktor@stiskala.cz>"]
 repository = "https://github.com/ViktorStiskala/python-qrplatba"
 classifiers=[
     'Intended Audience :: Developers',
     'Operating System :: OS Independent',
     'Programming Language :: Python',
```

### Comparing `qrplatba-1.1.0/qrplatba/spayd.py` & `qrplatba-1.1.1/qrplatba/spayd.py`

 * *Files identical despite different names*

### Comparing `qrplatba-1.1.0/qrplatba/svg.py` & `qrplatba-1.1.1/qrplatba/svg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from decimal import Decimal
 from typing import NamedTuple
 
 from qrcode.image import svg
-import xml.etree.ElementTree as ET
+from qrcode.compat.etree import ET
 
 
 class ScaledSizes(NamedTuple):
     inside_border: Decimal
     outside_border: Decimal
     width: Decimal
     line_size: Decimal
```

### Comparing `qrplatba-1.1.0/PKG-INFO` & `qrplatba-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qrplatba
-Version: 1.1.0
+Version: 1.1.1
 Summary: QR platba SVG QR code and SPAYD string generator.
 Home-page: https://github.com/ViktorStiskala/python-qrplatba
 License: MIT
 Author: Viktor Stískala
 Author-email: viktor@stiskala.cz
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
@@ -76,26 +76,26 @@
 
 ## License
 
 This software is licensed under [MIT license](https://opensource.org/license/mit/) since version `1.0.0`.
 
 ## Changelog
 
+### `1.1.0` (5 April 2023)
+
+- Dropped support for Python 3.7
+- Added pre-commit, black and ruff for code formatting
+
 ### `1.0.0` (4 April 2023)
 
 **Warning:** While the API is mostly backwards compatible, the look and size of the generated QR codes has changed.
 
 - Updated requirements to support the latest `qrcode` version
 - Added support for custom output sizes using `box_size` and `border` parameters
 - Changed legacy setuptools to [poetry](https://python-poetry.org/)
 - Dropped support for Python `2.x` and `<3.7`
 - Changed license to MIT
 - Added unit tests
 
-### `1.1.0` (5 April 2023)
-
-- Dropped support for Python 3.7
-- Added pre-commit, black and ruff for code formatting
-
```


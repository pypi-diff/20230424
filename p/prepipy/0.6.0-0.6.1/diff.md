# Comparing `tmp/prepipy-0.6.0.tar.gz` & `tmp/prepipy-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prepipy-0.6.0.tar", max compression
+gzip compressed data, was "prepipy-0.6.1.tar", max compression
```

## Comparing `prepipy-0.6.0.tar` & `prepipy-0.6.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    35823 2022-09-29 09:47:18.805206 prepipy-0.6.0/LICENSE
--rw-r--r--   0        0        0     1104 2023-04-23 19:43:40.671610 prepipy-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2049 2023-03-19 20:16:59.384002 prepipy-0.6.0/README.md
--rw-r--r--   0        0        0        0 2023-04-23 11:55:03.000536 prepipy-0.6.0/src/prepipy/__init__.py
--rw-r--r--   0        0        0     7615 2023-03-31 21:09:47.634370 prepipy-0.6.0/src/prepipy/auxiliaries.py
--rw-r--r--   0        0        0     1291 2023-03-22 14:05:29.668486 prepipy-0.6.0/src/prepipy/config/config_comments.yml
--rw-r--r--   0        0        0      859 2023-03-31 20:54:09.462366 prepipy-0.6.0/src/prepipy/config/logging_config.yml
--rw-r--r--   0        0        0      549 2023-03-30 22:08:20.988049 prepipy-0.6.0/src/prepipy/config/masking_example.yml
--rw-r--r--   0        0        0     1565 2023-03-31 09:38:15.114796 prepipy-0.6.0/src/prepipy/config_file_examples/bands.yml
--rw-r--r--   0        0        0     1736 2023-03-31 09:38:15.114796 prepipy-0.6.0/src/prepipy/config_file_examples/config_single.yml
--rw-r--r--   0        0        0      184 2023-03-31 09:38:15.114796 prepipy-0.6.0/src/prepipy/config_file_examples/mask.yml
--rw-r--r--   0        0        0     3535 2023-03-31 09:38:20.474789 prepipy-0.6.0/src/prepipy/configuration.py
--rw-r--r--   0        0        0    47849 2023-04-23 18:54:41.005509 prepipy-0.6.0/src/prepipy/framework.py
--rw-r--r--   0        0        0     7094 2023-04-23 18:55:59.195121 prepipy-0.6.0/src/prepipy/framework_sources.py
--rw-r--r--   0        0        0     2501 2023-03-31 20:58:21.229729 prepipy-0.6.0/src/prepipy/masking.py
--rw-r--r--   0        0        0       68 2023-03-31 21:09:47.636364 prepipy-0.6.0/src/prepipy/resources/grey_values.yml
--rw-r--r--   0        0        0     1044 2023-03-12 22:50:46.683730 prepipy-0.6.0/src/prepipy/resources/html_templates.yml
--rw-r--r--   0        0        0      468 2023-03-12 22:50:46.685849 prepipy-0.6.0/src/prepipy/resources/stiff_params.yml
--rw-r--r--   0        0        0    19384 2023-04-23 19:02:59.685403 prepipy-0.6.0/src/prepipy/rgbcombo.py
--rw-r--r--   0        0        0     3416 1970-01-01 00:00:00.000000 prepipy-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    35823 2022-09-29 09:47:18.805206 prepipy-0.6.1/LICENSE
+-rw-r--r--   0        0        0     1104 2023-04-23 23:15:18.096830 prepipy-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     2049 2023-03-19 20:16:59.384002 prepipy-0.6.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-23 11:55:03.000536 prepipy-0.6.1/src/prepipy/__init__.py
+-rw-r--r--   0        0        0     7617 2023-04-23 23:11:52.299277 prepipy-0.6.1/src/prepipy/auxiliaries.py
+-rw-r--r--   0        0        0     1291 2023-03-22 14:05:29.668486 prepipy-0.6.1/src/prepipy/config/config_comments.yml
+-rw-r--r--   0        0        0      859 2023-03-31 20:54:09.462366 prepipy-0.6.1/src/prepipy/config/logging_config.yml
+-rw-r--r--   0        0        0      549 2023-03-30 22:08:20.988049 prepipy-0.6.1/src/prepipy/config/masking_example.yml
+-rw-r--r--   0        0        0     1565 2023-03-31 09:38:15.114796 prepipy-0.6.1/src/prepipy/config_file_examples/bands.yml
+-rw-r--r--   0        0        0     1736 2023-03-31 09:38:15.114796 prepipy-0.6.1/src/prepipy/config_file_examples/config_single.yml
+-rw-r--r--   0        0        0      184 2023-03-31 09:38:15.114796 prepipy-0.6.1/src/prepipy/config_file_examples/mask.yml
+-rw-r--r--   0        0        0     3535 2023-03-31 09:38:20.474789 prepipy-0.6.1/src/prepipy/configuration.py
+-rw-r--r--   0        0        0    47850 2023-04-23 23:11:35.981625 prepipy-0.6.1/src/prepipy/framework.py
+-rw-r--r--   0        0        0     7094 2023-04-23 18:55:59.195121 prepipy-0.6.1/src/prepipy/framework_sources.py
+-rw-r--r--   0        0        0     2502 2023-04-23 23:11:23.068772 prepipy-0.6.1/src/prepipy/masking.py
+-rw-r--r--   0        0        0       68 2023-03-31 21:09:47.636364 prepipy-0.6.1/src/prepipy/resources/grey_values.yml
+-rw-r--r--   0        0        0     1044 2023-03-12 22:50:46.683730 prepipy-0.6.1/src/prepipy/resources/html_templates.yml
+-rw-r--r--   0        0        0      468 2023-03-12 22:50:46.685849 prepipy-0.6.1/src/prepipy/resources/stiff_params.yml
+-rw-r--r--   0        0        0    19395 2023-04-23 23:11:12.370453 prepipy-0.6.1/src/prepipy/rgbcombo.py
+-rw-r--r--   0        0        0     3416 1970-01-01 00:00:00.000000 prepipy-0.6.1/PKG-INFO
```

### Comparing `prepipy-0.6.0/LICENSE` & `prepipy-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.0/pyproject.toml` & `prepipy-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prepipy"
-version = "0.6.0"
+version = "0.6.1"
 description = "Provides the ability to stretch and combine astronomical images from multiple bands into (RGB) colour images."
 authors = ["Fabian Haberhauer <fabian.haberhauer@univie.ac.at>"]
 maintainers = ["teutoburg <ghost@instruct.at>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/teutoburg/prepipy"
 classifiers = [
```

### Comparing `prepipy-0.6.0/README.md` & `prepipy-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.0/src/prepipy/auxiliaries.py` & `prepipy-0.6.1/src/prepipy/auxiliaries.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 from pathlib import Path
 from dataclasses import replace, asdict, is_dataclass, fields
 from string import Template
 from typing import Iterable, Optional, ClassVar, Dict, Protocol, TypeVar, Any
 
 from ruamel.yaml import YAML
 
-from framework import RGBPicture, Frame, Band
-from configuration import Configurator
+from .framework import RGBPicture, Frame, Band
+from .configuration import Configurator
 
 yaml = YAML()
 
 absolute_path = Path(__file__).resolve(strict=True).parent
 DEFAULT_CONFIG_NAME = "config_single.yml"
 DEFAULT_BANDS_NAME = "bands.yml"
```

### Comparing `prepipy-0.6.0/src/prepipy/config/config_comments.yml` & `prepipy-0.6.1/src/prepipy/config/config_comments.yml`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.0/src/prepipy/config/logging_config.yml` & `prepipy-0.6.1/src/prepipy/config/logging_config.yml`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.0/src/prepipy/config/masking_example.yml` & `prepipy-0.6.1/src/prepipy/config/masking_example.yml`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.0/src/prepipy/config_file_examples/bands.yml` & `prepipy-0.6.1/src/prepipy/config_file_examples/bands.yml`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.0/src/prepipy/config_file_examples/config_single.yml` & `prepipy-0.6.1/src/prepipy/config_file_examples/config_single.yml`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.0/src/prepipy/configuration.py` & `prepipy-0.6.1/src/prepipy/configuration.py`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.0/src/prepipy/framework.py` & `prepipy-0.6.1/src/prepipy/framework.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 from astropy.visualization.wcsaxes import WCSAxes
 
 from ruamel.yaml import YAML
 from PIL import Image
 from PIL import __version__ as pillow_version
 from tqdm import tqdm
 
-from configuration import ProcessConfigurator, FiguresConfigurator
+from .configuration import ProcessConfigurator, FiguresConfigurator
 
 __author__ = "Fabian Haberhauer"
 __copyright__ = "Copyright 2023"
 __credits__ = [("Bertin, E.", "2012ASPC..461..263B")]
 __license__ = "GPL"
 __maintainer__ = "Fabian Haberhauer"
 __email__ = "fabian.haberhauer@univie.ac.at"
```

### Comparing `prepipy-0.6.0/src/prepipy/framework_sources.py` & `prepipy-0.6.1/src/prepipy/framework_sources.py`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.0/src/prepipy/masking.py` & `prepipy-0.6.1/src/prepipy/masking.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import numpy.typing as npt
 from ruamel.yaml import YAML
 
 from astropy.coordinates import Angle, SkyCoord
 from regions import PixCoord, SkyRegion, CircleSkyRegion, \
                     RectangleSkyRegion, PolygonSkyRegion
 
-from framework import Frame
+from .framework import Frame
 
 __author__ = "Fabian Haberhauer"
 __copyright__ = "Copyright 2023"
 
 yaml = YAML()
```

### Comparing `prepipy-0.6.0/src/prepipy/resources/html_templates.yml` & `prepipy-0.6.1/src/prepipy/resources/html_templates.yml`

 * *Files identical despite different names*

### Comparing `prepipy-0.6.0/src/prepipy/rgbcombo.py` & `prepipy-0.6.1/src/prepipy/rgbcombo.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 
 from ruamel.yaml import YAML
 import numpy as np
 from tqdm import tqdm
 from tqdm.contrib.logging import logging_redirect_tqdm
 from colorama import Fore, Back, Style
 
-from framework import JPEGPicture, Band
-from framework import logger as framework_logger
-from masking import get_mask
-import auxiliaries
-from configuration import Configurator, GeneralConfigurator, ProcessConfigurator
+from .framework import JPEGPicture, Band
+from .framework import logger as framework_logger
+from .masking import get_mask
+from . import auxiliaries
+from .configuration import Configurator, GeneralConfigurator, ProcessConfigurator
 
 __author__ = "Fabian Haberhauer"
 __copyright__ = "Copyright 2023"
 
 _P = ParamSpec("_P")
 _T = TypeVar("_T")
```

### Comparing `prepipy-0.6.0/PKG-INFO` & `prepipy-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prepipy
-Version: 0.6.0
+Version: 0.6.1
 Summary: Provides the ability to stretch and combine astronomical images from multiple bands into (RGB) colour images.
 Home-page: https://github.com/teutoburg/prepipy
 License: GPL-3.0-or-later
 Author: Fabian Haberhauer
 Author-email: fabian.haberhauer@univie.ac.at
 Maintainer: teutoburg
 Maintainer-email: ghost@instruct.at
```


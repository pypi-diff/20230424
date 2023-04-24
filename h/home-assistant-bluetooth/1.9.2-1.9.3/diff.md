# Comparing `tmp/home_assistant_bluetooth-1.9.2.tar.gz` & `tmp/home_assistant_bluetooth-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "home_assistant_bluetooth-1.9.2.tar", max compression
+gzip compressed data, was "home_assistant_bluetooth-1.9.3.tar", max compression
```

## Comparing `home_assistant_bluetooth-1.9.2.tar` & `home_assistant_bluetooth-1.9.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11345 2023-01-04 16:58:01.467043 home_assistant_bluetooth-1.9.2/LICENSE
--rw-r--r--   0        0        0     4300 2023-01-04 16:58:01.467043 home_assistant_bluetooth-1.9.2/README.md
--rw-r--r--   0        0        0      922 2023-01-04 16:58:01.467043 home_assistant_bluetooth-1.9.2/build_ext.py
--rw-r--r--   0        0        0     2179 2023-01-04 16:58:02.403049 home_assistant_bluetooth-1.9.2/pyproject.toml
--rw-r--r--   0        0        0      262 2023-01-04 16:58:02.375049 home_assistant_bluetooth-1.9.2/src/home_assistant_bluetooth/__init__.py
--rw-r--r--   0        0        0      703 2023-01-04 16:58:01.467043 home_assistant_bluetooth-1.9.2/src/home_assistant_bluetooth/models.pxd
--rw-r--r--   0        0        0     6182 2023-01-04 16:58:01.467043 home_assistant_bluetooth-1.9.2/src/home_assistant_bluetooth/models.py
--rw-r--r--   0        0        0        0 2023-01-04 16:58:01.467043 home_assistant_bluetooth-1.9.2/src/home_assistant_bluetooth/py.typed
--rw-r--r--   0        0        0     5122 1970-01-01 00:00:00.000000 home_assistant_bluetooth-1.9.2/setup.py
--rw-r--r--   0        0        0     5451 1970-01-01 00:00:00.000000 home_assistant_bluetooth-1.9.2/PKG-INFO
+-rw-r--r--   0        0        0    11345 2023-02-14 03:49:47.903326 home_assistant_bluetooth-1.9.3/LICENSE
+-rw-r--r--   0        0        0     4300 2023-02-14 03:49:47.903326 home_assistant_bluetooth-1.9.3/README.md
+-rw-r--r--   0        0        0      922 2023-02-14 03:49:47.903326 home_assistant_bluetooth-1.9.3/build_ext.py
+-rw-r--r--   0        0        0     2228 2023-02-14 03:49:48.859332 home_assistant_bluetooth-1.9.3/pyproject.toml
+-rw-r--r--   0        0        0      262 2023-02-14 03:49:48.815332 home_assistant_bluetooth-1.9.3/src/home_assistant_bluetooth/__init__.py
+-rw-r--r--   0        0        0      703 2023-02-14 03:49:47.903326 home_assistant_bluetooth-1.9.3/src/home_assistant_bluetooth/models.pxd
+-rw-r--r--   0        0        0     6182 2023-02-14 03:49:47.903326 home_assistant_bluetooth-1.9.3/src/home_assistant_bluetooth/models.py
+-rw-r--r--   0        0        0        0 2023-02-14 03:49:47.903326 home_assistant_bluetooth-1.9.3/src/home_assistant_bluetooth/py.typed
+-rw-r--r--   0        0        0     5122 1970-01-01 00:00:00.000000 home_assistant_bluetooth-1.9.3/setup.py
+-rw-r--r--   0        0        0     5451 1970-01-01 00:00:00.000000 home_assistant_bluetooth-1.9.3/PKG-INFO
```

### Comparing `home_assistant_bluetooth-1.9.2/LICENSE` & `home_assistant_bluetooth-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `home_assistant_bluetooth-1.9.2/README.md` & `home_assistant_bluetooth-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `home_assistant_bluetooth-1.9.2/build_ext.py` & `home_assistant_bluetooth-1.9.3/build_ext.py`

 * *Files identical despite different names*

### Comparing `home_assistant_bluetooth-1.9.2/pyproject.toml` & `home_assistant_bluetooth-1.9.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 [tool.poetry]
 name = "home-assistant-bluetooth"
-version = "1.9.2"
+version = "1.9.3"
 description = "Home Assistant Bluetooth Models and Helpers"
 authors = ["J. Nick Koston <nick@home-assistant.io>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/home-assistant-libs/home-assistant-bluetooth"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries",
 ]
-build = "build_ext.py"
 packages = [
     { include = "home_assistant_bluetooth", from = "src" },
 ]
 
+[tool.poetry.build]
+generate-setup-file = true
+script = "build_ext.py"
+
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/home-assistant-libs/home-assistant-bluetooth/issues"
 "Changelog" = "https://github.com/home-assistant-libs/home-assistant-bluetooth/blob/main/CHANGELOG.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `home_assistant_bluetooth-1.9.2/src/home_assistant_bluetooth/models.pxd` & `home_assistant_bluetooth-1.9.3/src/home_assistant_bluetooth/models.pxd`

 * *Files identical despite different names*

### Comparing `home_assistant_bluetooth-1.9.2/src/home_assistant_bluetooth/models.py` & `home_assistant_bluetooth-1.9.3/src/home_assistant_bluetooth/models.py`

 * *Files identical despite different names*

### Comparing `home_assistant_bluetooth-1.9.2/setup.py` & `home_assistant_bluetooth-1.9.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ['home_assistant_bluetooth']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'home-assistant-bluetooth',
-    'version': '1.9.2',
+    'version': '1.9.3',
     'description': 'Home Assistant Bluetooth Models and Helpers',
     'long_description': '# Home Assistant Bluetooth\n\n<p align="center">\n  <a href="https://github.com/home-assistant-libs/home-assistant-bluetooth/actions?query=workflow%3ACI">\n    <img src="https://img.shields.io/github/workflow/status/home-assistant-libs/home-assistant-bluetooth/CI/main?label=CI&logo=github&style=flat-square" alt="CI Status" >\n  </a>\n  <a href="https://codecov.io/gh/home-assistant-libs/home-assistant-bluetooth">\n    <img src="https://img.shields.io/codecov/c/github/home-assistant-libs/home-assistant-bluetooth.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">\n  </a>\n</p>\n<p align="center">\n  <a href="https://python-poetry.org/">\n    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">\n  </a>\n  <a href="https://github.com/ambv/black">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">\n  </a>\n  <a href="https://github.com/pre-commit/pre-commit">\n    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">\n  </a>\n</p>\n<p align="center">\n  <a href="https://pypi.org/project/home-assistant-bluetooth/">\n    <img src="https://img.shields.io/pypi/v/home-assistant-bluetooth.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">\n  </a>\n  <img src="https://img.shields.io/pypi/pyversions/home-assistant-bluetooth.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">\n  <img src="https://img.shields.io/pypi/l/home-assistant-bluetooth.svg?style=flat-square" alt="License">\n</p>\n\nHome Assistant Bluetooth Models and Helpers\n\n## Usage\n\nThis library is for accessing Home Assistant Bluetooth models. Libraries use these models to receive and parse Bluetooth advertisement data.\n\n```python\n@dataclasses.dataclass\nclass BluetoothServiceInfo(BaseServiceInfo):\n    """Prepared info from bluetooth entries."""\n\n    name: str\n    address: str\n    rssi: int\n    manufacturer_data: dict[int, bytes]\n    service_data: dict[str, bytes]\n    service_uuids: list[str]\n    source: str\n```\n\nThe data used to populate BluetoothServiceInfo comes from [bleak](https://github.com/hbldh/bleak)\'s `BLEDevice` and `AdvertisementData`, except for the `source` field, which comes from Home Assistant and represents the source of the data.\n\nIn the future, Home Assistant may support remote Bluetooth transceivers, which may use the source field to determine which device is closest.\n\n## Installation\n\nInstall this via pip (or your favourite package manager):\n\n`pip install home-assistant-bluetooth`\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- prettier-ignore-start -->\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- markdownlint-disable -->\n<!-- markdownlint-enable -->\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n<!-- prettier-ignore-end -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package was created with\n[Cookiecutter](https://github.com/audreyr/cookiecutter) and the\n[browniebroke/cookiecutter-pypackage](https://github.com/browniebroke/cookiecutter-pypackage)\nproject template.\n',
     'author': 'J. Nick Koston',
     'author_email': 'nick@home-assistant.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/home-assistant-libs/home-assistant-bluetooth',
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['home_assistant_bluetooth'] package_data = \ {'': ['*']}
-setup_kwargs = { 'name': 'home-assistant-bluetooth', 'version': '1.9.2',
+setup_kwargs = { 'name': 'home-assistant-bluetooth', 'version': '1.9.3',
 'description': 'Home Assistant Bluetooth Models and Helpers',
 'long_description': '# Home Assistant Bluetooth\n\n
             \n \n_[CI_Status]\n\n \n_[Test_coverage_percentage]\n\n
 \n
              \n \n_[Poetry]\n\n \n_[black]\n\n \n_[pre-commit]\n\n
 \n
       \n \n_[PyPI_Version]\n\n [Supported Python versions]\n [License]\n
```

### Comparing `home_assistant_bluetooth-1.9.2/PKG-INFO` & `home_assistant_bluetooth-1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: home-assistant-bluetooth
-Version: 1.9.2
+Version: 1.9.3
 Summary: Home Assistant Bluetooth Models and Helpers
 Home-page: https://github.com/home-assistant-libs/home-assistant-bluetooth
 License: Apache Software License 2.0
 Author: J. Nick Koston
 Author-email: nick@home-assistant.io
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```


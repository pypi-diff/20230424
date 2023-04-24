# Comparing `tmp/epiweeks-2.1.4.tar.gz` & `tmp/epiweeks-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epiweeks-2.1.4.tar", last modified: Sat Feb 12 07:39:11 2022, max compression
+gzip compressed data, was "epiweeks-2.2.0.tar", last modified: Mon Apr 24 19:56:29 2023, max compression
```

## Comparing `epiweeks-2.1.4.tar` & `epiweeks-2.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-12 07:39:11.569821 epiweeks-2.1.4/
--rw-r--r--   0 runner    (1001) docker     (121)     2468 2022-02-12 07:39:01.000000 epiweeks-2.1.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1107 2022-02-12 07:39:01.000000 epiweeks-2.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-02-12 07:39:01.000000 epiweeks-2.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3847 2022-02-12 07:39:11.569821 epiweeks-2.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2580 2022-02-12 07:39:01.000000 epiweeks-2.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-02-12 07:39:01.000000 epiweeks-2.1.4/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     1406 2022-02-12 07:39:01.000000 epiweeks-2.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-02-12 07:39:11.569821 epiweeks-2.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      327 2022-02-12 07:39:01.000000 epiweeks-2.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-12 07:39:11.565821 epiweeks-2.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-12 07:39:11.569821 epiweeks-2.1.4/src/epiweeks/
--rw-r--r--   0 runner    (1001) docker     (121)    12172 2022-02-12 07:39:01.000000 epiweeks-2.1.4/src/epiweeks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-12 07:39:11.569821 epiweeks-2.1.4/src/epiweeks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3847 2022-02-12 07:39:11.000000 epiweeks-2.1.4/src/epiweeks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      443 2022-02-12 07:39:11.000000 epiweeks-2.1.4/src/epiweeks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-12 07:39:11.000000 epiweeks-2.1.4/src/epiweeks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-12 07:39:11.000000 epiweeks-2.1.4/src/epiweeks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-02-12 07:39:11.000000 epiweeks-2.1.4/src/epiweeks.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-12 07:39:11.565821 epiweeks-2.1.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-12 07:39:11.569821 epiweeks-2.1.4/tests/integration/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-12 07:39:11.569821 epiweeks-2.1.4/tests/integration/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)    24105 2022-02-12 07:39:01.000000 epiweeks-2.1.4/tests/integration/fixtures/cdc_weeks.json
--rw-r--r--   0 runner    (1001) docker     (121)    24107 2022-02-12 07:39:01.000000 epiweeks-2.1.4/tests/integration/fixtures/iso_weeks.json
--rw-r--r--   0 runner    (1001) docker     (121)     1497 2022-02-12 07:39:01.000000 epiweeks-2.1.4/tests/integration/test_reference_weeks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-12 07:39:11.569821 epiweeks-2.1.4/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (121)    10710 2022-02-12 07:39:01.000000 epiweeks-2.1.4/tests/unit/test_epiweeks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:56:29.676380 epiweeks-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-24 19:56:19.000000 epiweeks-2.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-24 19:56:19.000000 epiweeks-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-24 19:56:19.000000 epiweeks-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-24 19:56:29.676380 epiweeks-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-24 19:56:19.000000 epiweeks-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-24 19:56:19.000000 epiweeks-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-24 19:56:29.676380 epiweeks-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-24 19:56:19.000000 epiweeks-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:56:29.672379 epiweeks-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:56:29.672379 epiweeks-2.2.0/src/epiweeks/
+-rw-r--r--   0 runner    (1001) docker     (123)    12172 2023-04-24 19:56:19.000000 epiweeks-2.2.0/src/epiweeks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-24 19:56:19.000000 epiweeks-2.2.0/src/epiweeks/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:56:29.672379 epiweeks-2.2.0/src/epiweeks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-24 19:56:29.000000 epiweeks-2.2.0/src/epiweeks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-24 19:56:29.000000 epiweeks-2.2.0/src/epiweeks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 19:56:29.000000 epiweeks-2.2.0/src/epiweeks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 19:56:29.000000 epiweeks-2.2.0/src/epiweeks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-24 19:56:29.000000 epiweeks-2.2.0/src/epiweeks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:56:29.672379 epiweeks-2.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:56:29.672379 epiweeks-2.2.0/tests/integration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:56:29.676380 epiweeks-2.2.0/tests/integration/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)    24105 2023-04-24 19:56:19.000000 epiweeks-2.2.0/tests/integration/fixtures/cdc_weeks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24107 2023-04-24 19:56:19.000000 epiweeks-2.2.0/tests/integration/fixtures/iso_weeks.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-24 19:56:19.000000 epiweeks-2.2.0/tests/integration/test_reference_weeks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 19:56:29.676380 epiweeks-2.2.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)    10710 2023-04-24 19:56:19.000000 epiweeks-2.2.0/tests/unit/test_epiweeks.py
```

### Comparing `epiweeks-2.1.4/CHANGELOG.md` & `epiweeks-2.2.0/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 # Changelog
 
-The format is based on [semantic versioning] and [pre-release versioning]
-schemes recommended by the Python Packaging Authority (PPA).
+The versioning scheme is compliant with the [PEP 440] specification.
 
-[semantic versioning]:
-  https://packaging.python.org/guides/distributing-packages-using-setuptools/#semantic-versioning-preferred
-[pre-release versioning]:
-  https://packaging.python.org/guides/distributing-packages-using-setuptools/#pre-release-versioning
+[PEP 440]: https://peps.python.org/pep-0440/#public-version-identifiers
+
+## 2.2.0 (2023-04-24)
+
+- Dropped support for Python 3.6 and added support for Python 3.11.
+- Fixed location of type-checking marker file.
+- Added more classifiers to package configuration.
+- Updated documentation and removed badges from the package description.
+- Updated development configurations and GitHub actions.
+- Changed GitHub username back to @dralshehri and updated related links.
 
 ## 2.1.4 (2022-02-12)
 
-- Changed GitHub username to @mhalshehri and updated related links.
 - Changed package docstrings to Google style and updated documentation.
 - Updated development workflows and configurations.
 - Other minor fixes and enhancements.
+- Changed GitHub username to @mhalshehri and updated related links.
 
 ## 2.1.3 (2021-09-24)
 
 - Added `__version__` attribute to the package.
 - Changed `Week` rich comparison to return `NotImplemented` when the second
   operand is not a `Week` object.
 - Changed the project structure by converting the`epiweeks` module into a
```

### Comparing `epiweeks-2.1.4/LICENSE` & `epiweeks-2.2.0/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2018 Mohammed H Alshehri (@mhalshehri) and contributors
+Copyright (c) 2018 Mohammed Alshehri (https://www.dralshehri.com)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `epiweeks-2.1.4/README.md` & `epiweeks-2.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -3,46 +3,50 @@
 <!-- start description -->
 
 A Python package to calculate epidemiological weeks using the US CDC (MMWR) and
 ISO week numbering systems.
 
 <!-- end description -->
 
-[![Build Status](https://img.shields.io/github/workflow/status/mhalshehri/epiweeks/Release)][build]
+<!-- start badges -->
+
+[![Release Status](https://img.shields.io/github/actions/workflow/status/dralshehri/epiweeks/release.yml?label=release)][release]
 [![Coverage Status](https://img.shields.io/badge/coverage-100%25-success)][coverage]
-[![Code Quality](https://img.shields.io/codefactor/grade/github/mhalshehri/epiweeks/main?&label=codefactor)][quality]
+[![Code Quality](https://img.shields.io/codefactor/grade/github/dralshehri/epiweeks/main?&label=codefactor)][quality]
 [![Docs Status](https://img.shields.io/readthedocs/epiweeks/stable)][docs]
 [![PyPI Downloads](https://img.shields.io/pypi/dm/epiweeks?color=blue)][downloads]
 [![PyPI Version](https://img.shields.io/pypi/v/epiweeks)][pypi-version]
 [![Conda Version](https://img.shields.io/conda/vn/bioconda/epiweeks)][conda-version]
-[![Package License](https://img.shields.io/github/license/mhalshehri/epiweeks)][license]
+[![Package License](https://img.shields.io/github/license/dralshehri/epiweeks)][license]
 
-[build]: https://github.com/mhalshehri/epiweeks/actions/workflows/release.yml
-[coverage]: https://github.com/mhalshehri/epiweeks/actions/workflows/release.yml
+[release]: https://github.com/dralshehri/epiweeks/actions/workflows/release.yml
+[coverage]: https://github.com/dralshehri/epiweeks/actions/workflows/release.yml
 [quality]:
-  https://www.codefactor.io/repository/github/mhalshehri/epiweeks/overview/main
+  https://www.codefactor.io/repository/github/dralshehri/epiweeks/overview/main
 [docs]: https://epiweeks.readthedocs.io
 [downloads]: https://pypistats.org/packages/epiweeks
 [pypi-version]: https://pypi.python.org/pypi/epiweeks
 [conda-version]: https://anaconda.org/bioconda/epiweeks
-[license]: https://github.com/mhalshehri/epiweeks/blob/main/LICENSE
+[license]: https://github.com/dralshehri/epiweeks/blob/main/LICENSE
+
+<!-- end badges -->
 
 <!-- start summary -->
 
 ## Features
 
 - Support for both the US CDC (MMWR) and ISO week numbering systems.
 - Accurate and tested calculations.
 - Intuitive, clean, and easy-to-use interface.
 - Calculation of the start and end dates of weeks.
 - Iteration of year's weeks or week's dates.
 - Rich comparison between weeks.
 - Logical operations for weeks (addition, subtraction and containment).
 - Validation of input data.
-- Works on Python 3.6+ with zero dependencies.
+- Works on Python 3.7+ with zero dependencies.
 - Thoroughly tested with 100% test coverage.
 
 ## Installation
 
 To install using `pip`, run:
 
 ```shell
```

### Comparing `epiweeks-2.1.4/pyproject.toml` & `epiweeks-2.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,50 @@
 [build-system]
-requires = ["setuptools>=51", "wheel"]
+requires = ["setuptools>=51"]
 build-backend = "setuptools.build_meta"
 
 [tool.pytest.ini_options]
-minversion = "6.0"
+minversion = "7.0"
 addopts = "-ra -q"
 testpaths = ["tests/unit"]
 
 [tool.coverage.run]
 branch = true
 source = ["epiweeks"]
 
 [tool.coverage.paths]
 source = ["src"]
 
 [tool.black]
 line-length = 80
-target-version = ["py36", "py37", "py38", "py39", "py310"]
+target-version = ["py37", "py38", "py39", "py310", "py311"]
 
 [tool.isort]
 profile = "black"
 
-[tool.pylint.messages_control]
-disable = ["bad-whitespace", "bad-continuation"]  # recommended by Black
-
 [tool.pylint.reports]
 score = false
 
 [tool.pylint.format]
 max-line-length = 80
 expected-line-ending-format = "LF"
 
 [tool.pylint.master]
-py-version = "3.6"
+py-version = "3.7"
 
 [tool.mypy]
-python_version = "3.6"
+python_version = "3.7"
 strict = true
 
 [tool.taskipy.tasks]
 test = "task test_cov tests"
+test_min = "pytest"
+test_all = "pytest tests"
 test_cov = "pytest --cov --cov-report=term-missing --cov-fail-under=100"
 test_cov_html = "pytest --cov --cov-report=term --cov-report=html"
-test_all = "pytest tests"
 lint = "task lint_isort && task lint_black && task lint_pylint && task lint_mypy"
 lint_isort = "isort --check-only src tests"
 lint_black = "black --check --quiet src tests"
 lint_pylint = "pylint src"
 lint_mypy = "mypy src"
 format = "isort src tests && black src tests"
 upgrade = "task upgrade_dev && task upgrade_docs"
```

### Comparing `epiweeks-2.1.4/setup.cfg` & `epiweeks-2.2.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 [metadata]
 name = epiweeks
 version = attr: epiweeks.__version__
-author = Mohammed H Alshehri
+author = Mohammed Alshehri
 author_email = 
 description = Epidemiological weeks calculation based on the US CDC (MMWR) and ISO week numbering systems
-long_description = file: README.md
-long_description_content_type = text/markdown
 keywords = epidemiology, weeks, cdc, mmwr, iso, calendar, surveillance, public-health
 license = MIT
 license_files = LICENSE
-url = https://github.com/mhalshehri/epiweeks
+url = https://github.com/dralshehri/epiweeks
 project_urls = 
 	Documentation = https://epiweeks.readthedocs.io
-	Source Code = https://github.com/mhalshehri/epiweeks
+	Source Code = https://github.com/dralshehri/epiweeks
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Intended Audience :: Healthcare Industry
 	License :: OSI Approved :: MIT License
+	Natural Language :: English
+	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering
 	Topic :: Utilities
 	Typing :: Typed
 
 [options]
 packages = find:
 package_dir = 
 	= src
 include_package_data = True
-python_requires = >=3.6
+python_requires = >=3.7
 zip_safe = False
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build =
```

### Comparing `epiweeks-2.1.4/src/epiweeks/__init__.py` & `epiweeks-2.2.0/src/epiweeks/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Epidemiological weeks calculation based on the US CDC (MMWR) and ISO week
 numbering systems.
 
-https://github.com/mhalshehri/epiweeks
+https://github.com/dralshehri/epiweeks
 """
 
-__version__ = "2.1.4"
+__version__ = "2.2.0"
 
 from datetime import date, timedelta
 from typing import Iterator, Tuple
 
 
 class Week:
     """A Week object represents a week in epidemiological week calendar."""
```

### Comparing `epiweeks-2.1.4/tests/integration/fixtures/cdc_weeks.json` & `epiweeks-2.2.0/tests/integration/fixtures/cdc_weeks.json`

 * *Files identical despite different names*

### Comparing `epiweeks-2.1.4/tests/integration/fixtures/iso_weeks.json` & `epiweeks-2.2.0/tests/integration/fixtures/iso_weeks.json`

 * *Files identical despite different names*

### Comparing `epiweeks-2.1.4/tests/integration/test_reference_weeks.py` & `epiweeks-2.2.0/tests/integration/test_reference_weeks.py`

 * *Files identical despite different names*

### Comparing `epiweeks-2.1.4/tests/unit/test_epiweeks.py` & `epiweeks-2.2.0/tests/unit/test_epiweeks.py`

 * *Files identical despite different names*


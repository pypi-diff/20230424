# Comparing `tmp/hijri-converter-2.2.4.tar.gz` & `tmp/hijri-converter-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hijri-converter-2.2.4.tar", last modified: Mon May 23 18:46:36 2022, max compression
+gzip compressed data, was "hijri-converter-2.3.0.tar", last modified: Mon Apr 24 18:45:27 2023, max compression
```

## Comparing `hijri-converter-2.2.4.tar` & `hijri-converter-2.3.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 18:46:36.768762 hijri-converter-2.2.4/
--rw-r--r--   0 runner    (1001) docker     (121)     6227 2022-05-23 18:46:25.000000 hijri-converter-2.2.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1107 2022-05-23 18:46:25.000000 hijri-converter-2.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-05-23 18:46:25.000000 hijri-converter-2.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4936 2022-05-23 18:46:36.768762 hijri-converter-2.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3352 2022-05-23 18:46:25.000000 hijri-converter-2.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1413 2022-05-23 18:46:25.000000 hijri-converter-2.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1594 2022-05-23 18:46:36.768762 hijri-converter-2.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      334 2022-05-23 18:46:25.000000 hijri-converter-2.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 18:46:36.764762 hijri-converter-2.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 18:46:36.764762 hijri-converter-2.2.4/src/hijri_converter/
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-05-23 18:46:25.000000 hijri-converter-2.2.4/src/hijri_converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10938 2022-05-23 18:46:25.000000 hijri-converter-2.2.4/src/hijri_converter/convert.py
--rw-r--r--   0 runner    (1001) docker     (121)      805 2022-05-23 18:46:25.000000 hijri-converter-2.2.4/src/hijri_converter/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     5108 2022-05-23 18:46:25.000000 hijri-converter-2.2.4/src/hijri_converter/locales.py
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-05-23 18:46:25.000000 hijri-converter-2.2.4/src/hijri_converter/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    14615 2022-05-23 18:46:25.000000 hijri-converter-2.2.4/src/hijri_converter/ummalqura.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 18:46:36.764762 hijri-converter-2.2.4/src/hijri_converter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4936 2022-05-23 18:46:36.000000 hijri-converter-2.2.4/src/hijri_converter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      773 2022-05-23 18:46:36.000000 hijri-converter-2.2.4/src/hijri_converter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-23 18:46:36.000000 hijri-converter-2.2.4/src/hijri_converter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-23 18:46:35.000000 hijri-converter-2.2.4/src/hijri_converter.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-05-23 18:46:36.000000 hijri-converter-2.2.4/src/hijri_converter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 18:46:36.764762 hijri-converter-2.2.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 18:46:36.764762 hijri-converter-2.2.4/tests/integration/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 18:46:36.764762 hijri-converter-2.2.4/tests/integration/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)    20308 2022-05-23 18:46:25.000000 hijri-converter-2.2.4/tests/integration/fixtures/kfupm_comparison_calendar.json
--rw-r--r--   0 runner    (1001) docker     (121)    25374 2022-05-23 18:46:25.000000 hijri-converter-2.2.4/tests/integration/fixtures/ummalqura_calendar_website.json
--rw-r--r--   0 runner    (1001) docker     (121)    13869 2022-05-23 18:46:25.000000 hijri-converter-2.2.4/tests/integration/fixtures/ummalqura_newspaper_issues.json
--rwxr-xr-x   0 runner    (1001) docker     (121)     1280 2022-05-23 18:46:25.000000 hijri-converter-2.2.4/tests/integration/test_month_starts.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 18:46:36.768762 hijri-converter-2.2.4/tests/unit/
--rwxr-xr-x   0 runner    (1001) docker     (121)     6753 2022-05-23 18:46:25.000000 hijri-converter-2.2.4/tests/unit/test_convert.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      380 2022-05-23 18:46:25.000000 hijri-converter-2.2.4/tests/unit/test_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1787 2022-05-23 18:46:25.000000 hijri-converter-2.2.4/tests/unit/test_locales.py
+drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 18:45:27.870163 hijri-converter-2.3.0/
+-rw-r--r--   0 mohd       (501) staff       (20)     6243 2023-04-24 18:21:26.000000 hijri-converter-2.3.0/CHANGELOG.md
+-rw-r--r--   0 mohd       (501) staff       (20)     1103 2023-04-24 04:43:29.000000 hijri-converter-2.3.0/LICENSE
+-rw-r--r--   0 mohd       (501) staff       (20)       56 2023-04-24 04:34:05.000000 hijri-converter-2.3.0/MANIFEST.in
+-rw-r--r--   0 mohd       (501) staff       (20)     3884 2023-04-24 18:45:27.870228 hijri-converter-2.3.0/PKG-INFO
+-rw-r--r--   0 mohd       (501) staff       (20)     3822 2023-04-24 18:21:27.000000 hijri-converter-2.3.0/README.md
+-rw-r--r--   0 mohd       (501) staff       (20)     1320 2023-04-24 04:43:29.000000 hijri-converter-2.3.0/pyproject.toml
+-rw-r--r--   0 mohd       (501) staff       (20)     1512 2023-04-24 18:45:27.870490 hijri-converter-2.3.0/setup.cfg
+-rw-r--r--   0 mohd       (501) staff       (20)      858 2023-04-24 04:43:29.000000 hijri-converter-2.3.0/setup.py
+drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 18:45:27.864941 hijri-converter-2.3.0/src/
+drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 18:45:27.867640 hijri-converter-2.3.0/src/hijri_converter/
+-rw-r--r--   0 mohd       (501) staff       (20)      207 2023-04-24 18:21:27.000000 hijri-converter-2.3.0/src/hijri_converter/__init__.py
+-rw-r--r--   0 mohd       (501) staff       (20)    10938 2023-04-20 18:10:31.000000 hijri-converter-2.3.0/src/hijri_converter/convert.py
+-rw-r--r--   0 mohd       (501) staff       (20)      805 2023-04-20 18:10:34.000000 hijri-converter-2.3.0/src/hijri_converter/helpers.py
+-rw-r--r--   0 mohd       (501) staff       (20)     5108 2023-04-20 18:10:37.000000 hijri-converter-2.3.0/src/hijri_converter/locales.py
+-rw-r--r--   0 mohd       (501) staff       (20)       26 2022-05-23 16:57:16.000000 hijri-converter-2.3.0/src/hijri_converter/py.typed
+-rw-r--r--   0 mohd       (501) staff       (20)    14615 2023-04-20 18:10:42.000000 hijri-converter-2.3.0/src/hijri_converter/ummalqura.py
+drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 18:45:27.868423 hijri-converter-2.3.0/src/hijri_converter.egg-info/
+-rw-r--r--   0 mohd       (501) staff       (20)     3884 2023-04-24 18:45:27.000000 hijri-converter-2.3.0/src/hijri_converter.egg-info/PKG-INFO
+-rw-r--r--   0 mohd       (501) staff       (20)      773 2023-04-24 18:45:27.000000 hijri-converter-2.3.0/src/hijri_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 mohd       (501) staff       (20)        1 2023-04-24 18:45:27.000000 hijri-converter-2.3.0/src/hijri_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 mohd       (501) staff       (20)        1 2023-04-24 04:35:10.000000 hijri-converter-2.3.0/src/hijri_converter.egg-info/not-zip-safe
+-rw-r--r--   0 mohd       (501) staff       (20)       16 2023-04-24 18:45:27.000000 hijri-converter-2.3.0/src/hijri_converter.egg-info/top_level.txt
+drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 18:45:27.865188 hijri-converter-2.3.0/tests/
+drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 18:45:27.868530 hijri-converter-2.3.0/tests/integration/
+drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 18:45:27.869558 hijri-converter-2.3.0/tests/integration/fixtures/
+-rw-r--r--   0 mohd       (501) staff       (20)    20308 2022-02-09 22:30:41.000000 hijri-converter-2.3.0/tests/integration/fixtures/kfupm_comparison_calendar.json
+-rw-r--r--   0 mohd       (501) staff       (20)    25374 2022-02-09 22:30:41.000000 hijri-converter-2.3.0/tests/integration/fixtures/ummalqura_calendar_website.json
+-rw-r--r--   0 mohd       (501) staff       (20)    13869 2022-02-09 22:30:41.000000 hijri-converter-2.3.0/tests/integration/fixtures/ummalqura_newspaper_issues.json
+-rwxr-xr-x   0 mohd       (501) staff       (20)     1280 2022-02-09 22:30:41.000000 hijri-converter-2.3.0/tests/integration/test_month_starts.py
+drwxr-xr-x   0 mohd       (501) staff       (20)        0 2023-04-24 18:45:27.870039 hijri-converter-2.3.0/tests/unit/
+-rwxr-xr-x   0 mohd       (501) staff       (20)     6753 2022-02-09 22:52:24.000000 hijri-converter-2.3.0/tests/unit/test_convert.py
+-rwxr-xr-x   0 mohd       (501) staff       (20)      380 2022-02-09 22:30:41.000000 hijri-converter-2.3.0/tests/unit/test_helpers.py
+-rwxr-xr-x   0 mohd       (501) staff       (20)     1787 2022-02-09 22:30:41.000000 hijri-converter-2.3.0/tests/unit/test_locales.py
```

### Comparing `hijri-converter-2.2.4/CHANGELOG.md` & `hijri-converter-2.3.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,60 @@
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
+## 2.3.0 (2023-04-24)
+
+- Deprecated the package in favor of the new `hijridate` package.
+- Dropped support for Python 3.6 and added support for Python 3.11.
+- Updated documentation and removed badges from the package description.
+- Changed GitHub username back to @dralshehri and updated related links.
 
 ## 2.2.4 (2022-05-23)
 
 - Added more classifiers to package configuration.
-- Fixed location of type checking marker file. ([#10] bt [@dimbleby])
+- Fixed location of type-checking marker file. (By [@dimbleby] in [#10])
 - Updated development and build requirements.
 
-[#10]: https://github.com/mhalshehri/hijri-converter/pull/10
+[#10]: https://github.com/dralshehri/hijri-converter/pull/10
 [@dimbleby]: https://github.com/dimbleby
 
 ## 2.2.3 (2022-02-12)
 
-- Changed GitHub username to [@mhalshehri] and updated related links.
 - Changed package docstrings to Google style and updated documentation.
 - Updated development workflows and configurations.
 - Other minor fixes and enhancements.
-
-[@mhalshehri]: https://github.com/mhalshehri
+- Changed GitHub username to @mhalshehri and updated related links.
 
 ## 2.2.2 (2021-09-25)
 
 - Added some missing variable annotations to `ummalqura` module.
 - Fixed an issue when generating documentation.
 - Fixed some typos in docstrings and improved documentation.
 - Other minor fixes and enhancements.
 
 ## 2.2.1 (2021-09-04)
 
-- Fixed calculation of month 12 of year 1354 AH.
+- Fixed calculation of month 12 of the year 1354 AH.
 - Fixed an issue when generating documentation without the package being
   installed. ([#7])
 - Refactored internal helper functions.
 - Updated and improved tests and documentation.
 - Fixed some typos.
 
-[#7]: https://github.com/mhalshehri/hijri-converter/issues/7
+[#7]: https://github.com/dralshehri/hijri-converter/issues/7
 
 ## 2.2.0 (2021-08-16)
 
 - Added `today()` classmethod to Hijri class to get the Hijri Object of today's
   date.
 - Added `separator` and `padding` parameters to `dmyformat()` method to have
-  more control on formatting.
+  more control over formatting.
 - Refactored locales for better management and testing. (Inspired by [Arrow]
   localization)
 - Updated main classes to be conveniently imported into the package level e.g.
   `from hijri_converter import Hijri, Gregorian`.
 - Removed deprecated method `slashformat()` from Hijri and Gregorian classes.
 - Updated tests and documentation.
 - Other minor fixes and internal enhancements.
@@ -62,33 +63,33 @@
 
 ## 2.1.3 (2021-06-22)
 
 - Minor fixes and enhancements for docstrings and documentation.
 
 ## 2.1.2 (2021-05-30)
 
-- Added Bangla translation. ([#4] by [@nokibsarkar])
+- Added Bangla translation. (By [@nokibsarkar] in [#4])
 - Changed `Hijri` rich comparison to return `NotImplemented` when the second
   operand is not `Hijri` class.
 - Changed `ummalqura` constants to be in capital letters adhering to PEP8.
 - Updated packaging configuration files and local development workflow.
 - Other minor fixes and documentation enhancements.
 
-[#4]: https://github.com/mhalshehri/hijri-converter/pull/4
+[#4]: https://github.com/dralshehri/hijri-converter/pull/4
 [@nokibsarkar]: https://github.com/nokibsarkar
 
 ## 2.1.1 (2020-05-21)
 
 - Added `dmyformat()` to return dates in `DD/MM/YYYY` format.
 - Deprecated `slashformat()` method to be replaced by `dmyformat()` method.
 - Fixed PyPI package not including some required files. ([#3])
 - Fixed some typos.
 - Updated tests.
 
-[#3]: https://github.com/mhalshehri/hijri-converter/issues/3
+[#3]: https://github.com/dralshehri/hijri-converter/issues/3
 
 ## 2.1.0 (2019-06-16)
 
 This version has more accurate conversion and better internal code. Details are
 as follows:
 
 - Dropped support for the years before 1343 AH because the Umm al-Qura calendar
```

### Comparing `hijri-converter-2.2.4/LICENSE` & `hijri-converter-2.3.0/LICENSE`

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

### Comparing `hijri-converter-2.2.4/README.md` & `hijri-converter-2.3.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,51 +1,73 @@
 # hijri-converter
 
 <!-- start description -->
 
 A Python package to convert accurately between Hijri and Gregorian dates using
 the Umm al-Qura calendar.
 
+> ⚠️ **Deprecation Notice**
+>
+> This package has been **deprecated** and will not receive future updates.
+> Please use the [hijridate](https://pypi.org/project/hijridate/) package
+> instead.
+>
+> For migration to `hijridate`, install the package:
+>
+> ```
+> pip install hijridate~=2.3.0
+> ```
+>
+> Then change the import statement as:
+>
+> ```py
+> from hijridate import Hijri, Gregorian
+> ```
+
 <!-- end description -->
 
-[![Build Status](https://img.shields.io/github/workflow/status/mhalshehri/hijri-converter/Release)][build]
+<!-- start badges -->
+
+[![Release Status](https://img.shields.io/github/actions/workflow/status/dralshehri/hijri-converter/release.yml?label=release)][release]
 [![Coverage Status](https://img.shields.io/badge/coverage-100%25-success)][coverage]
-[![Code Quality](https://img.shields.io/codefactor/grade/github/mhalshehri/hijri-converter/main?&label=codefactor)][quality]
+[![Code Quality](https://img.shields.io/codefactor/grade/github/dralshehri/hijri-converter/main?&label=codefactor)][quality]
 [![Docs Status](https://img.shields.io/readthedocs/hijri-converter/stable)][docs]
 [![PyPI Downloads](https://img.shields.io/pypi/dm/hijri-converter?color=blue)][downloads]
 [![PyPI Version](https://img.shields.io/pypi/v/hijri-converter)][pypi-version]
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/hijri-converter)][conda-version]
-[![Package License](https://img.shields.io/github/license/mhalshehri/hijri-converter)][license]
+[![Package License](https://img.shields.io/github/license/dralshehri/hijri-converter)][license]
 
-[build]:
-  https://github.com/mhalshehri/hijri-converter/actions/workflows/release.yml
+[release]:
+  https://github.com/dralshehri/hijri-converter/actions/workflows/release.yml
 [coverage]:
-  https://github.com/mhalshehri/hijri-converter/actions/workflows/release.yml
+  https://github.com/dralshehri/hijri-converter/actions/workflows/release.yml
 [quality]:
-  https://www.codefactor.io/repository/github/mhalshehri/hijri-converter/overview/main
+  https://www.codefactor.io/repository/github/dralshehri/hijri-converter/overview/main
 [docs]: https://hijri-converter.readthedocs.io
 [downloads]: https://pypistats.org/packages/hijri-converter
 [pypi-version]: https://pypi.python.org/pypi/hijri-converter
 [conda-version]: https://anaconda.org/conda-forge/hijri-converter
-[license]: https://github.com/mhalshehri/hijri-converter/blob/main/LICENSE
+[license]: https://github.com/dralshehri/hijri-converter/blob/main/LICENSE
+
+<!-- end badges -->
 
 <!-- start summary -->
 
 ## Features
 
 - Accurate and verified date conversion.
 - Optimized code performance compared to similar packages.
 - Intuitive, clean, and easy-to-use interface.
 - Most of the methods and formats are similar to those of standard library.
 - Multilingual representation of weekday names, months, and calendar era
   notations.
 - Easily extendable to support other natural languages.
 - Rich comparison between dates.
 - Validation of input dates.
-- Works on Python 3.6+ with zero dependencies.
+- Works on Python 3.7+ with zero dependencies.
 - Thoroughly tested with 100% test coverage.
 
 ## Limitations
 
 - The date range supported by converter is limited to the period from the
   beginning of 1343 AH (1 August 1924 CE) to the end of 1500 AH (16 November
   2077 CE).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hijri-converter-2.2.4/pyproject.toml` & `hijri-converter-2.3.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,52 +1,50 @@
 [build-system]
-requires = ["setuptools>=43", "wheel"]
+requires = ["setuptools>=51"]
 build-backend = "setuptools.build_meta"
 
 [tool.pytest.ini_options]
-minversion = "6.0"
+minversion = "7.0"
 addopts = "-ra -q"
 testpaths = ["tests/unit"]
 
 [tool.coverage.run]
 branch = true
 source = ["hijri_converter"]
 
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

### Comparing `hijri-converter-2.2.4/setup.cfg` & `hijri-converter-2.3.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,50 @@
 [metadata]
 name = hijri-converter
 version = attr: hijri_converter.__version__
-author = Mohammed H Alshehri
+author = Mohammed Alshehri
 author_email = 
 description = Accurate Hijri-Gregorian dates converter based on the Umm al-Qura calendar
-long_description = file: README.md
-long_description_content_type = text/markdown
 keywords = hijri, gregorian, date, converter, ummalqura, saudi, calendar
 license = MIT
 license_files = LICENSE
-url = https://github.com/mhalshehri/hijri-converter
+url = https://github.com/dralshehri/hijri-converter
 project_urls = 
 	Documentation = https://hijri-converter.readthedocs.io
-	Source Code = https://github.com/mhalshehri/hijri-converter
+	Source Code = https://github.com/dralshehri/hijri-converter
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Intended Audience :: Healthcare Industry
 	Intended Audience :: Legal Industry
 	License :: OSI Approved :: MIT License
 	Natural Language :: Arabic
 	Natural Language :: Bengali
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering
 	Topic :: Software Development :: Internationalization
 	Topic :: Software Development :: Localization
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

### Comparing `hijri-converter-2.2.4/src/hijri_converter/convert.py` & `hijri-converter-2.3.0/src/hijri_converter/convert.py`

 * *Files identical despite different names*

### Comparing `hijri-converter-2.2.4/src/hijri_converter/helpers.py` & `hijri-converter-2.3.0/src/hijri_converter/helpers.py`

 * *Files identical despite different names*

### Comparing `hijri-converter-2.2.4/src/hijri_converter/locales.py` & `hijri-converter-2.3.0/src/hijri_converter/locales.py`

 * *Files identical despite different names*

### Comparing `hijri-converter-2.2.4/src/hijri_converter/ummalqura.py` & `hijri-converter-2.3.0/src/hijri_converter/ummalqura.py`

 * *Files identical despite different names*

### Comparing `hijri-converter-2.2.4/src/hijri_converter.egg-info/SOURCES.txt` & `hijri-converter-2.3.0/src/hijri_converter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hijri-converter-2.2.4/tests/integration/fixtures/kfupm_comparison_calendar.json` & `hijri-converter-2.3.0/tests/integration/fixtures/kfupm_comparison_calendar.json`

 * *Files identical despite different names*

### Comparing `hijri-converter-2.2.4/tests/integration/fixtures/ummalqura_calendar_website.json` & `hijri-converter-2.3.0/tests/integration/fixtures/ummalqura_calendar_website.json`

 * *Files identical despite different names*

### Comparing `hijri-converter-2.2.4/tests/integration/fixtures/ummalqura_newspaper_issues.json` & `hijri-converter-2.3.0/tests/integration/fixtures/ummalqura_newspaper_issues.json`

 * *Files identical despite different names*

### Comparing `hijri-converter-2.2.4/tests/integration/test_month_starts.py` & `hijri-converter-2.3.0/tests/integration/test_month_starts.py`

 * *Files identical despite different names*

### Comparing `hijri-converter-2.2.4/tests/unit/test_convert.py` & `hijri-converter-2.3.0/tests/unit/test_convert.py`

 * *Files identical despite different names*

### Comparing `hijri-converter-2.2.4/tests/unit/test_locales.py` & `hijri-converter-2.3.0/tests/unit/test_locales.py`

 * *Files identical despite different names*


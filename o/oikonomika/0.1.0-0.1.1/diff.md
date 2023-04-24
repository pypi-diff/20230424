# Comparing `tmp/oikonomika-0.1.0.tar.gz` & `tmp/oikonomika-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oikonomika-0.1.0.tar", max compression
+gzip compressed data, was "oikonomika-0.1.1.tar", max compression
```

## Comparing `oikonomika-0.1.0.tar` & `oikonomika-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1071 2023-04-21 21:26:04.050675 oikonomika-0.1.0/LICENSE
--rw-r--r--   0        0        0     3775 2023-04-21 21:26:04.050675 oikonomika-0.1.0/README.md
--rw-r--r--   0        0        0     2993 2023-04-21 21:26:30.519207 oikonomika-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      178 2023-04-21 21:26:04.050675 oikonomika-0.1.0/src/oikonomika/__cli__.py
--rw-r--r--   0        0        0      879 2023-04-21 21:26:04.050675 oikonomika-0.1.0/src/oikonomika/__init__.py
--rw-r--r--   0        0        0       22 2023-04-21 21:26:30.463206 oikonomika-0.1.0/src/oikonomika/_version.py
--rw-r--r--   0        0        0        0 2023-04-21 21:26:04.050675 oikonomika-0.1.0/src/oikonomika/conf/__init__.py
--rw-r--r--   0        0        0      170 2023-04-21 21:26:04.050675 oikonomika-0.1.0/src/oikonomika/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-04-21 21:26:04.050675 oikonomika-0.1.0/src/oikonomika/conf/batch/__init__.yaml
--rw-r--r--   0        0        0      506 2023-04-21 21:26:04.050675 oikonomika-0.1.0/src/oikonomika/conf/config.yaml
--rw-r--r--   0        0        0      789 2023-04-21 21:26:04.050675 oikonomika-0.1.0/src/oikonomika/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      502 2023-04-21 21:26:04.050675 oikonomika-0.1.0/src/oikonomika/conf/hconf.yaml
--rw-r--r--   0        0        0     1126 2023-04-21 21:26:04.050675 oikonomika-0.1.0/src/oikonomika/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-04-21 21:26:04.050675 oikonomika-0.1.0/src/oikonomika/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      295 2023-04-21 21:26:04.050675 oikonomika-0.1.0/src/oikonomika/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-04-21 21:26:04.050675 oikonomika-0.1.0/src/oikonomika/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-04-21 21:26:04.050675 oikonomika-0.1.0/src/oikonomika/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-04-21 21:26:04.050675 oikonomika-0.1.0/src/oikonomika/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-04-21 21:26:04.050675 oikonomika-0.1.0/src/oikonomika/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-04-21 21:26:04.054675 oikonomika-0.1.0/src/oikonomika/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-04-21 21:26:04.054675 oikonomika-0.1.0/src/oikonomika/conf/project/__init__.yaml
--rw-r--r--   0        0        0       83 2023-04-21 21:26:04.054675 oikonomika-0.1.0/src/oikonomika/conf/task/__init__.yaml
--rw-r--r--   0        0        0      204 2023-04-21 21:26:04.054675 oikonomika-0.1.0/src/oikonomika/project.toml
--rw-r--r--   0        0        0        0 2023-04-21 21:26:04.054675 oikonomika-0.1.0/src/oikonomika/py.typed
--rw-r--r--   0        0        0     4397 1970-01-01 00:00:00.000000 oikonomika-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-24 19:25:40.326856 oikonomika-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3735 2023-04-24 19:25:40.326856 oikonomika-0.1.1/README.md
+-rw-r--r--   0        0        0     2867 2023-04-24 19:26:05.383178 oikonomika-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      178 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/__cli__.py
+-rw-r--r--   0        0        0      819 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-24 19:26:05.331177 oikonomika-0.1.1/src/oikonomika/_version.py
+-rw-r--r--   0        0        0        0 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/conf/__init__.py
+-rw-r--r--   0        0        0      203 2023-04-24 19:26:05.331177 oikonomika-0.1.1/src/oikonomika/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0      506 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/conf/config.yaml
+-rw-r--r--   0        0        0      789 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      502 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/conf/hconf.yaml
+-rw-r--r--   0        0        0     1126 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      295 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      701 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      164 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/conf/path/__default__.yaml
+-rw-r--r--   0        0        0      616 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      360 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       83 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      204 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/project.toml
+-rw-r--r--   0        0        0        0 2023-04-24 19:25:40.326856 oikonomika-0.1.1/src/oikonomika/py.typed
+-rw-r--r--   0        0        0     4385 1970-01-01 00:00:00.000000 oikonomika-0.1.1/PKG-INFO
```

### Comparing `oikonomika-0.1.0/LICENSE` & `oikonomika-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oikonomika-0.1.0/README.md` & `oikonomika-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,14 @@
 [pypi-url]: https://pypi.org/project/oikonomika
 [docs-url]: https://oikonomika.entelecheia.ai
 [changelog]: https://github.com/entelecheia/oikonomika/blob/main/CHANGELOG.md
 [contributing guidelines]: https://github.com/entelecheia/oikonomika/blob/main/CONTRIBUTING.md
 
 <!-- Links: -->
 
-A Python Library for Economic Analysis
-
 - Documentation: [https://oikonomika.entelecheia.ai][docs-url]
 - GitHub: [https://github.com/entelecheia/oikonomika][repo-url]
 - PyPI: [https://pypi.org/project/oikonomika][pypi-url]
 
 Oikonomika is a powerful and versatile Python library designed for economic analysis, facilitating data-driven decision-making in the fields of economics, finance, and policy-making. The name Oikonomika is derived from the Greek word Οικονομικά, signifying the library's commitment to providing robust tools for studying and understanding economic phenomena.
 
 ## Features
```

### Comparing `oikonomika-0.1.0/pyproject.toml` & `oikonomika-0.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 [tool.poetry]
 name = "oikonomika"
-version = "0.1.0"
+version = "0.1.1"
 description = "A Python Library for Economic Analysis"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://oikonomika.entelecheia.ai"
+repository = "https://github.com/entelecheia/oikonomika"
 readme = "README.md"
 packages = [{ include = "oikonomika", from = "src" }]
 
 [tool.poetry.scripts]
 oikonomika = 'oikonomika.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-hyfi = "^0.2.11"
-toml = "^0.10.2"
+hyfi = "^0.2.13"
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
-setuptools-scm = "^7.1.0"
 isort = "^5.12.0"
 black = "^23.1.0"
 flake8 = "^6.0.0"
 mypy = "^1.0.0"
 flake8-pyproject = "^1.2.2"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
@@ -74,31 +73,27 @@
 exclude_lines = ['if __name__ == "__main__":']
 
 [tool.commitizen]
 name = "cz_conventional_commits"
 version = "1.0.1"
 tag_format = "v$version"
 
-[tool.setuptools_scm]
-write_to_template = '__version__ = "{version}"'
-tag_regex = '^(?P<prefix>v)?(?P<version>[^\+]+)(?P<suffix>.*)?$'
-
 [tool.semantic_release]
 branch = "main"
 version_toml = "pyproject.toml:tool.poetry.version"
 version_variable = "src/oikonomika/_version.py:__version__"
+version_pattern = 'src/oikonomika/conf/about/__init__.yaml:version: "{version}"'
 version_source = "tag"
 commit_version_number = true # required for version_source = "tag"
 commit_subject = "chore(release): :rocket: {version} [skip ci]"
 prerelease_tag = "rc"
 major_on_zero = true
 tag_commit = true
-pre_commit_command = "make scm-version"
 changelog_file = "CHANGELOG.md"
 upload_to_repository = true
 upload_to_release = true
 build_command = "poetry build --no-cache"
 hvcs = "github" # hosting version control system, gitlab is also supported
 
 [build-system]
-requires = ["poetry-core>=1.0.0", "setuptools>=45", "setuptools_scm[toml]>=6.2"]
-build-backend = 'setuptools.build_meta'
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `oikonomika-0.1.0/src/oikonomika/conf/dotenv/__init__.yaml` & `oikonomika-0.1.1/src/oikonomika/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `oikonomika-0.1.0/src/oikonomika/conf/hydra/help/help.yaml` & `oikonomika-0.1.1/src/oikonomika/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `oikonomika-0.1.0/src/oikonomika/conf/mode/__init__.yaml` & `oikonomika-0.1.1/src/oikonomika/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `oikonomika-0.1.0/src/oikonomika/conf/path/__default__.yaml` & `oikonomika-0.1.1/src/oikonomika/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `oikonomika-0.1.0/src/oikonomika/conf/path/__init__.yaml` & `oikonomika-0.1.1/src/oikonomika/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `oikonomika-0.1.0/PKG-INFO` & `oikonomika-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: oikonomika
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python Library for Economic Analysis
 Home-page: https://oikonomika.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: hyfi (>=0.2.11,<0.3.0)
-Requires-Dist: toml (>=0.10.2,<0.11.0)
+Requires-Dist: hyfi (>=0.2.13,<0.3.0)
+Project-URL: Repository, https://github.com/entelecheia/oikonomika
 Description-Content-Type: text/markdown
 
 # Oikonomika: A Python Library for Economic Analysis
 
 [![pypi-image]][pypi-url]
 [![license-image]][license-url]
 [![version-image]][release-url]
@@ -37,16 +37,14 @@
 [pypi-url]: https://pypi.org/project/oikonomika
 [docs-url]: https://oikonomika.entelecheia.ai
 [changelog]: https://github.com/entelecheia/oikonomika/blob/main/CHANGELOG.md
 [contributing guidelines]: https://github.com/entelecheia/oikonomika/blob/main/CONTRIBUTING.md
 
 <!-- Links: -->
 
-A Python Library for Economic Analysis
-
 - Documentation: [https://oikonomika.entelecheia.ai][docs-url]
 - GitHub: [https://github.com/entelecheia/oikonomika][repo-url]
 - PyPI: [https://pypi.org/project/oikonomika][pypi-url]
 
 Oikonomika is a powerful and versatile Python library designed for economic analysis, facilitating data-driven decision-making in the fields of economics, finance, and policy-making. The name Oikonomika is derived from the Greek word Οικονομικά, signifying the library's commitment to providing robust tools for studying and understanding economic phenomena.
 
 ## Features
```


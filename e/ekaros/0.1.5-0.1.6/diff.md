# Comparing `tmp/ekaros-0.1.5.tar.gz` & `tmp/ekaros-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ekaros-0.1.5.tar", max compression
+gzip compressed data, was "ekaros-0.1.6.tar", max compression
```

## Comparing `ekaros-0.1.5.tar` & `ekaros-0.1.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1071 2023-04-24 18:50:13.655914 ekaros-0.1.5/LICENSE
--rw-r--r--   0        0        0     3345 2023-04-24 18:50:13.655914 ekaros-0.1.5/README.md
--rw-r--r--   0        0        0     2964 2023-04-24 18:50:41.660159 ekaros-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      174 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/__cli__.py
--rw-r--r--   0        0        0      815 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/__init__.py
--rw-r--r--   0        0        0       22 2023-04-24 18:50:41.604159 ekaros-0.1.5/src/ekaros/_version.py
--rw-r--r--   0        0        0        0 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/conf/__init__.py
--rw-r--r--   0        0        0      195 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/conf/batch/__init__.yaml
--rw-r--r--   0        0        0      506 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/conf/config.yaml
--rw-r--r--   0        0        0      789 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      502 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/conf/hconf.yaml
--rw-r--r--   0        0        0     1126 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      295 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/conf/project/__init__.yaml
--rw-r--r--   0        0        0       83 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/conf/task/__init__.yaml
--rw-r--r--   0        0        0      196 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/project.toml
--rw-r--r--   0        0        0        0 2023-04-24 18:50:13.655914 ekaros-0.1.5/src/ekaros/py.typed
--rw-r--r--   0        0        0     3958 1970-01-01 00:00:00.000000 ekaros-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-24 19:26:56.357921 ekaros-0.1.6/LICENSE
+-rw-r--r--   0        0        0     3345 2023-04-24 19:26:56.357921 ekaros-0.1.6/README.md
+-rw-r--r--   0        0        0     2835 2023-04-24 19:27:23.441757 ekaros-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      174 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/__cli__.py
+-rw-r--r--   0        0        0      815 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-24 19:27:23.393757 ekaros-0.1.6/src/ekaros/_version.py
+-rw-r--r--   0        0        0        0 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/conf/__init__.py
+-rw-r--r--   0        0        0      195 2023-04-24 19:27:23.393757 ekaros-0.1.6/src/ekaros/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0      506 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/conf/config.yaml
+-rw-r--r--   0        0        0      789 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      502 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/conf/hconf.yaml
+-rw-r--r--   0        0        0     1126 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      295 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      701 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      164 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/conf/path/__default__.yaml
+-rw-r--r--   0        0        0      616 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      360 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       83 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      196 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/project.toml
+-rw-r--r--   0        0        0        0 2023-04-24 19:26:56.361921 ekaros-0.1.6/src/ekaros/py.typed
+-rw-r--r--   0        0        0     3983 1970-01-01 00:00:00.000000 ekaros-0.1.6/PKG-INFO
```

### Comparing `ekaros-0.1.5/LICENSE` & `ekaros-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ekaros-0.1.5/README.md` & `ekaros-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `ekaros-0.1.5/pyproject.toml` & `ekaros-0.1.6/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 [tool.poetry]
 name = "ekaros"
-version = "0.1.5"
+version = "0.1.6"
 description = "A Python Library for Generative AI Art"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://ekaros.entelecheia.ai"
+repository = "https://github.com/entelecheia/ekaros"
 readme = "README.md"
 packages = [{ include = "ekaros", from = "src" }]
 
 [tool.poetry.scripts]
 ekaros = 'ekaros.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-hyfi = "^0.2.6"
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
-write_to = "src/ekaros/_version.py"
-write_to_template = '__version__ = "{version}"'
-tag_regex = '^(?P<prefix>v)?(?P<version>[^\+]+)(?P<suffix>.*)?$'
-
 [tool.semantic_release]
 branch = "main"
 version_toml = "pyproject.toml:tool.poetry.version"
 version_variable = "src/ekaros/_version.py:__version__"
+version_pattern = 'src/ekaros/conf/about/__init__.yaml:version: "{version}"'
 version_source = "tag"
 commit_version_number = true # required for version_source = "tag"
 commit_subject = "chore(release): :rocket: {version} [skip ci]"
 prerelease_tag = "rc"
 major_on_zero = true
 tag_commit = true
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

### Comparing `ekaros-0.1.5/src/ekaros/__init__.py` & `ekaros-0.1.6/src/ekaros/__init__.py`

 * *Files identical despite different names*

### Comparing `ekaros-0.1.5/src/ekaros/conf/dotenv/__init__.yaml` & `ekaros-0.1.6/src/ekaros/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `ekaros-0.1.5/src/ekaros/conf/hydra/help/help.yaml` & `ekaros-0.1.6/src/ekaros/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `ekaros-0.1.5/src/ekaros/conf/mode/__init__.yaml` & `ekaros-0.1.6/src/ekaros/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `ekaros-0.1.5/src/ekaros/conf/path/__default__.yaml` & `ekaros-0.1.6/src/ekaros/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `ekaros-0.1.5/src/ekaros/conf/path/__init__.yaml` & `ekaros-0.1.6/src/ekaros/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `ekaros-0.1.5/PKG-INFO` & `ekaros-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: ekaros
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python Library for Generative AI Art
 Home-page: https://ekaros.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: hyfi (>=0.2.6,<0.3.0)
-Requires-Dist: toml (>=0.10.2,<0.11.0)
+Requires-Dist: hyfi (>=0.2.13,<0.3.0)
+Project-URL: Repository, https://github.com/entelecheia/ekaros
 Description-Content-Type: text/markdown
 
 # Ekaros: A Python Library for Generative AI Art
 
 [![pypi-image]][pypi-url]
 [![license-image]][license-url]
 [![version-image]][release-url]
```


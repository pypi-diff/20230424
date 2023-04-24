# Comparing `tmp/partifact-0.1.5.tar.gz` & `tmp/partifact-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "partifact-0.1.5.tar", max compression
+gzip compressed data, was "partifact-0.1.6.tar", max compression
```

## Comparing `partifact-0.1.5.tar` & `partifact-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1080 2021-11-10 09:35:16.513389 partifact-0.1.5/LICENSE
--rw-r--r--   0        0        0     2191 2021-11-10 11:11:03.364475 partifact-0.1.5/README.md
--rw-r--r--   0        0        0        0 2021-11-10 09:35:16.513765 partifact-0.1.5/partifact/__init__.py
--rw-r--r--   0        0        0     1450 2021-11-10 09:35:16.513940 partifact-0.1.5/partifact/auth_token.py
--rw-r--r--   0        0        0     3396 2021-11-10 11:20:42.220768 partifact-0.1.5/partifact/config.py
--rw-r--r--   0        0        0     1065 2021-11-10 09:35:16.514487 partifact-0.1.5/partifact/main.py
--rw-r--r--   0        0        0     2067 2021-11-10 09:35:16.514669 partifact-0.1.5/partifact/shell_commands.py
--rw-r--r--   0        0        0     1251 2021-11-10 11:22:44.244969 partifact-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3074 2021-11-10 11:22:47.311480 partifact-0.1.5/setup.py
--rw-r--r--   0        0        0     2917 2021-11-10 11:22:47.311677 partifact-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1080 2021-11-10 09:35:16.513389 partifact-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2192 2023-04-24 18:59:12.451630 partifact-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2021-11-10 09:35:16.513765 partifact-0.1.6/partifact/__init__.py
+-rw-r--r--   0        0        0     1450 2021-11-10 09:35:16.513940 partifact-0.1.6/partifact/auth_token.py
+-rw-r--r--   0        0        0     3698 2023-04-24 18:55:45.224275 partifact-0.1.6/partifact/config.py
+-rw-r--r--   0        0        0     1065 2021-11-10 09:35:16.514487 partifact-0.1.6/partifact/main.py
+-rw-r--r--   0        0        0     2067 2021-11-10 09:35:16.514669 partifact-0.1.6/partifact/shell_commands.py
+-rw-r--r--   0        0        0     1234 2023-04-24 18:58:35.107010 partifact-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2930 1970-01-01 00:00:00.000000 partifact-0.1.6/PKG-INFO
```

### Comparing `partifact-0.1.5/LICENSE` & `partifact-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `partifact-0.1.5/README.md` & `partifact-0.1.6/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -49,8 +49,8 @@
 partifact login myrepo --profile myprofile
 partifact login myrepo --role myrole
 ```
 
 # Known issues
 
 1. The `CodeArtifact` token seems to exceed the maximum length allowed in Windows Credential Manager, resulting
-in a misleading `(1783, 'CredWrite', 'The stub received bad data.')` error. The library has been tested on macOS.
+in a misleading `(1783, 'CredWrite', 'The stub received bad data.')` error. The library has been tested on macOS.
```

### Comparing `partifact-0.1.5/partifact/auth_token.py` & `partifact-0.1.6/partifact/auth_token.py`

 * *Files identical despite different names*

### Comparing `partifact-0.1.5/partifact/config.py` & `partifact-0.1.6/partifact/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
+import re
 from dataclasses import dataclass
 from typing import Optional
 
-from parse import parse
 from tomlkit import parse as parse_toml
 from tomlkit.exceptions import TOMLKitError
 
 CONFIG_PATH = "./pyproject.toml"
-URL_TEMPLATE = "https://{code_artifact_domain}-{aws_account}.d.codeartifact.{aws_region}.amazonaws.com/pypi/{code_artifact_repository}"
+URL_PATTERN = r"https://(?P<code_artifact_domain>.*)-(?P<aws_account>\d+).d.codeartifact.(?P<aws_region>[a-z0-9-]+).amazonaws.com/pypi/(?P<code_artifact_repository>.*)"
 
 
 @dataclass(frozen=True)
 class Configuration:
     """Data for a repository entry in the config file.
 
     Attributes:
@@ -70,23 +70,29 @@
         parsed_url = parse_url(url)
 
         return Configuration(aws_profile=profile, aws_role_name=role_name, **parsed_url)  # type: ignore
 
 
 def parse_url(url: str) -> dict:
     """Parses the URL into a mapping of parameter names to values."""
-    result = parse(URL_TEMPLATE, url)
-    if not result:
+    regex_result = re.match(URL_PATTERN, url)
+    if not regex_result:
         raise InvalidConfiguration(
-            f"failed to parse source URL, make sure it's in the format of {URL_TEMPLATE}"
+            f"failed to parse source URL, make sure it's in the format of {URL_PATTERN}"
         )
 
-    parsed_url = result.named
+    parsed_url = {}
+    regex_result = regex_result.groupdict()
+    parsed_url["code_artifact_domain"] = regex_result.get("code_artifact_domain")
+    parsed_url["aws_account"] = regex_result.get("aws_account")
+    parsed_url["aws_region"] = regex_result.get("aws_region")
     parsed_url["code_artifact_repository"] = (
-        parsed_url["code_artifact_repository"].replace("simple", "").rstrip("/")
+        regex_result.get("code_artifact_repository", "")
+        .replace("simple", "")
+        .rstrip("/")
     )
 
     return parsed_url
 
 
 class MissingConfiguration(Exception):
     """Raised if the configuration file is missing or does not contain the repository."""
```

### Comparing `partifact-0.1.5/partifact/main.py` & `partifact-0.1.6/partifact/main.py`

 * *Files identical despite different names*

### Comparing `partifact-0.1.5/partifact/shell_commands.py` & `partifact-0.1.6/partifact/shell_commands.py`

 * *Files identical despite different names*

### Comparing `partifact-0.1.5/pyproject.toml` & `partifact-0.1.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 [tool.poetry]
 name = "partifact"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["David Steiner <david_j_steiner@yahoo.co.nz>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Validus-Risk-Management/partifact"
 
 [tool.poetry.scripts]
 partifact = "partifact.main:app"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 boto3 = "^1.15"
 tomlkit = ">=0.7.0,<1.0.0"
 typer = "^0.3.2"
-parse = "^1.19.0"
 
 [tool.poetry.dev-dependencies]
-black = "^21.7b0"
+black = "^23.3.0"
 flake8 = "^3.9.0"
 flake8-absolute-import = "^1.0"
 flake8-blind-except = "^0.2.0"
 flake8-breakpoint = "^1.1.0"
 flake8-bugbear = "^21.4.3"
 flake8-builtins = "^1.5.3"
 flake8-cognitive-complexity = "^0.1.0"
@@ -30,15 +29,15 @@
 flake8-docstrings = "^1.6"
 flake8-eradicate = "^1.1.0"
 flake8-implicit-str-concat = "^0.2.0"
 flake8-mutable = "^1.2.0"
 flake8-print = "^4.0.0"
 flake8-pytest-style = "^1.5.0"
 flake8-simplify = "^0.14.1"
-isort = "^5.9.3"
+isort = "^5.12.0"
 mypy = "^0.910"
 pep8-naming = "^0.12.1"
 pre-commit = "^2.14.0"
 pyfakefs = "^4.5.0"
 pytest = "^6.2.4"
 pytest-mock = "^3.6.1"
```

### Comparing `partifact-0.1.5/PKG-INFO` & `partifact-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: partifact
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Home-page: https://github.com/Validus-Risk-Management/partifact
 License: MIT
 Author: David Steiner
 Author-email: david_j_steiner@yahoo.co.nz
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.15,<2.0)
-Requires-Dist: parse (>=1.19.0,<2.0.0)
 Requires-Dist: tomlkit (>=0.7.0,<1.0.0)
 Requires-Dist: typer (>=0.3.2,<0.4.0)
 Description-Content-Type: text/markdown
 
 # partifact
 
 partifact is a tool to help with configuring and authenticating CodeArtifact as a repository for [Poetry](https://github.com/python-poetry/poetry) and [pip](https://pip.pypa.io/en/stable/).
@@ -71,7 +71,8 @@
 partifact login myrepo --role myrole
 ```
 
 # Known issues
 
 1. The `CodeArtifact` token seems to exceed the maximum length allowed in Windows Credential Manager, resulting
 in a misleading `(1783, 'CredWrite', 'The stub received bad data.')` error. The library has been tested on macOS.
+
```


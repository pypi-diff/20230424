# Comparing `tmp/environ_config-23.1.0.tar.gz` & `tmp/environ_config-23.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, last modified: Mon Apr 24 19:52:48 2023, max compression
```

## Comparing `environ_config-23.1.0.tar` & `environ_config-23.2.0.tar`

### file list

```diff
@@ -1,40 +1,42 @@
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 environ_config-23.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 environ_config-23.1.0/.readthedocs.yaml
--rw-r--r--   0        0        0     4236 2020-02-02 00:00:00.000000 environ_config-23.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     4313 2020-02-02 00:00:00.000000 environ_config-23.1.0/README.md
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 environ_config-23.1.0/noxfile.py
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 environ_config-23.1.0/typing_examples.py
--rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 environ_config-23.1.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     7573 2020-02-02 00:00:00.000000 environ_config-23.1.0/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 environ_config-23.1.0/.github/FUNDING.yml
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 environ_config-23.1.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 environ_config-23.1.0/.github/SECURITY.md
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 environ_config-23.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 environ_config-23.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 environ_config-23.1.0/.github/workflows/pypi-package.yml
--rw-r--r--   0        0        0     7441 2020-02-02 00:00:00.000000 environ_config-23.1.0/docs/Makefile
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 environ_config-23.1.0/docs/api.md
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 environ_config-23.1.0/docs/changelog.md
--rw-r--r--   0        0        0     8950 2020-02-02 00:00:00.000000 environ_config-23.1.0/docs/conf.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 environ_config-23.1.0/docs/index.md
--rw-r--r--   0        0        0     7260 2020-02-02 00:00:00.000000 environ_config-23.1.0/docs/make.bat
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 environ_config-23.1.0/docs/testing.md
--rw-r--r--   0        0        0    10331 2020-02-02 00:00:00.000000 environ_config-23.1.0/docs/tutorial.md
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 environ_config-23.1.0/src/environ/__init__.py
--rw-r--r--   0        0        0    14774 2020-02-02 00:00:00.000000 environ_config-23.1.0/src/environ/_environ_config.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 environ_config-23.1.0/src/environ/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 environ_config-23.1.0/src/environ/py.typed
--rw-r--r--   0        0        0     9005 2020-02-02 00:00:00.000000 environ_config-23.1.0/src/environ/secrets/__init__.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 environ_config-23.1.0/src/environ/secrets/_utils.py
--rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 environ_config-23.1.0/src/environ/secrets/awssm.py
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 environ_config-23.1.0/tests/test_class_generate_help.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 environ_config-23.1.0/tests/test_class_to_config.py
--rw-r--r--   0        0        0    14722 2020-02-02 00:00:00.000000 environ_config-23.1.0/tests/test_environ_config.py
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 environ_config-23.1.0/tests/test_packaging.py
--rw-r--r--   0        0        0     8473 2020-02-02 00:00:00.000000 environ_config-23.1.0/tests/test_secrets.py
--rw-r--r--   0        0        0     5571 2020-02-02 00:00:00.000000 environ_config-23.1.0/tests/test_secrets_awssm.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 environ_config-23.1.0/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 environ_config-23.1.0/LICENSE
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 environ_config-23.1.0/NOTICE
--rw-r--r--   0        0        0     3381 2020-02-02 00:00:00.000000 environ_config-23.1.0/pyproject.toml
--rw-r--r--   0        0        0     7030 2020-02-02 00:00:00.000000 environ_config-23.1.0/PKG-INFO
+-rw-r--r--   0        0        0      125 2023-04-24 19:52:48.000000 environ_config-23.2.0/.git_archival.txt
+-rw-r--r--   0        0        0       32 2023-04-24 19:52:48.000000 environ_config-23.2.0/.gitattributes
+-rw-r--r--   0        0        0      476 2023-04-24 19:52:48.000000 environ_config-23.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      199 2023-04-24 19:52:48.000000 environ_config-23.2.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     4497 2023-04-24 19:52:48.000000 environ_config-23.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     4313 2023-04-24 19:52:48.000000 environ_config-23.2.0/README.md
+-rw-r--r--   0        0        0     2645 2023-04-24 19:52:48.000000 environ_config-23.2.0/noxfile.py
+-rw-r--r--   0        0        0     1619 2023-04-24 19:52:48.000000 environ_config-23.2.0/typing_examples.py
+-rw-r--r--   0        0        0     3164 2023-04-24 19:52:48.000000 environ_config-23.2.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     7573 2023-04-24 19:52:48.000000 environ_config-23.2.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0       48 2023-04-24 19:52:48.000000 environ_config-23.2.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1471 2023-04-24 19:52:48.000000 environ_config-23.2.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      378 2023-04-24 19:52:48.000000 environ_config-23.2.0/.github/SECURITY.md
+-rw-r--r--   0        0        0      119 2023-04-24 19:52:48.000000 environ_config-23.2.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     5887 2023-04-24 19:52:48.000000 environ_config-23.2.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1682 2023-04-24 19:52:48.000000 environ_config-23.2.0/.github/workflows/pypi-package.yml
+-rw-r--r--   0        0        0     7441 2023-04-24 19:52:48.000000 environ_config-23.2.0/docs/Makefile
+-rw-r--r--   0        0        0      934 2023-04-24 19:52:48.000000 environ_config-23.2.0/docs/api.md
+-rw-r--r--   0        0        0       33 2023-04-24 19:52:48.000000 environ_config-23.2.0/docs/changelog.md
+-rw-r--r--   0        0        0     8983 2023-04-24 19:52:48.000000 environ_config-23.2.0/docs/conf.py
+-rw-r--r--   0        0        0      492 2023-04-24 19:52:48.000000 environ_config-23.2.0/docs/index.md
+-rw-r--r--   0        0        0     7260 2023-04-24 19:52:48.000000 environ_config-23.2.0/docs/make.bat
+-rw-r--r--   0        0        0     2912 2023-04-24 19:52:48.000000 environ_config-23.2.0/docs/testing.md
+-rw-r--r--   0        0        0    10331 2023-04-24 19:52:48.000000 environ_config-23.2.0/docs/tutorial.md
+-rw-r--r--   0        0        0     1931 2023-04-24 19:52:48.000000 environ_config-23.2.0/src/environ/__init__.py
+-rw-r--r--   0        0        0    15076 2023-04-24 19:52:48.000000 environ_config-23.2.0/src/environ/_environ_config.py
+-rw-r--r--   0        0        0      990 2023-04-24 19:52:48.000000 environ_config-23.2.0/src/environ/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-24 19:52:48.000000 environ_config-23.2.0/src/environ/py.typed
+-rw-r--r--   0        0        0     8972 2023-04-24 19:52:48.000000 environ_config-23.2.0/src/environ/secrets/__init__.py
+-rw-r--r--   0        0        0      467 2023-04-24 19:52:48.000000 environ_config-23.2.0/src/environ/secrets/_utils.py
+-rw-r--r--   0        0        0     3434 2023-04-24 19:52:48.000000 environ_config-23.2.0/src/environ/secrets/awssm.py
+-rw-r--r--   0        0        0     2130 2023-04-24 19:52:48.000000 environ_config-23.2.0/tests/test_class_generate_help.py
+-rw-r--r--   0        0        0     2166 2023-04-24 19:52:48.000000 environ_config-23.2.0/tests/test_class_to_config.py
+-rw-r--r--   0        0        0    14698 2023-04-24 19:52:48.000000 environ_config-23.2.0/tests/test_environ_config.py
+-rw-r--r--   0        0        0     1992 2023-04-24 19:52:48.000000 environ_config-23.2.0/tests/test_packaging.py
+-rw-r--r--   0        0        0     8478 2023-04-24 19:52:48.000000 environ_config-23.2.0/tests/test_secrets.py
+-rw-r--r--   0        0        0     5564 2023-04-24 19:52:48.000000 environ_config-23.2.0/tests/test_secrets_awssm.py
+-rw-r--r--   0        0        0      124 2023-04-24 19:52:48.000000 environ_config-23.2.0/.gitignore
+-rw-r--r--   0        0        0    11358 2023-04-24 19:52:48.000000 environ_config-23.2.0/LICENSE
+-rw-r--r--   0        0        0       82 2023-04-24 19:52:48.000000 environ_config-23.2.0/NOTICE
+-rw-r--r--   0        0        0     4485 2023-04-24 19:52:48.000000 environ_config-23.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6588 2023-04-24 19:52:48.000000 environ_config-23.2.0/PKG-INFO
```

### Comparing `environ_config-23.1.0/CHANGELOG.md` & `environ_config-23.2.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,23 @@
 ---
 
 You shouldn't ever be afraid to upgrade *environ-config* if you're using its public APIs and pay attention to `DeprecationWarning`s.
 Whenever there is a need to break compatibility, it is announced here in the changelog and raises a `DeprecationWarning` for a year (if possible) before it's finally really broken.
 
 <!-- changelog follows -->
 
+
+## [23.2.0](https://github.com/hynek/environ-config/compare/23.1.0...23.2.0) - 2023-04-24
+
+### Fixed
+
+- Type hints for `environ.config()` now allow for arguments (e.g. `@environ.config(prefix="")`).
+  [#56](https://github.com/hynek/environ-config/issues/56)
+
+
 ## [23.1.0](https://github.com/hynek/environ-config/compare/22.1.0...23.1.0) - 2023-01-27
 
 ### Backwards-incompatible Changes
 
 *none*
 
 ### Deprecations
```

### Comparing `environ_config-23.1.0/README.md` & `environ_config-23.2.0/README.md`

 * *Files identical despite different names*

### Comparing `environ_config-23.1.0/noxfile.py` & `environ_config-23.2.0/noxfile.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,44 @@
 from __future__ import annotations
 
 import os
+import re
+
+from pathlib import Path
 
 import nox
 
 
 nox.options.reuse_existing_virtualenvs = True
 nox.options.error_on_external_run = True
 
 
+# Avoid dependencies on YAML / TOML libs using a questionable hacks.
+match_docs_python = re.compile(r"\s+python\: \"(\d\.\d\d)\"").fullmatch
+for line in Path(".readthedocs.yaml").read_text().splitlines():
+    m = match_docs_python(line)
+    if m:
+        DOCS_PYTHON = m.group(1)
+        break
+
+match_oldest_python = re.compile(
+    r"requires-python = \">=(\d\.\d+)\""
+).fullmatch
+match_oldest_attrs = re.compile(r".*\"attrs>=(\d+\.\d+\.\d+)\",.*").match
+for line in Path("pyproject.toml").read_text().splitlines():
+    m = match_oldest_python(line)
+    if m:
+        OLDEST_PYTHON = m.group(1)
+
+    m = match_oldest_attrs(line)
+    if m:
+        OLDEST_ATTRS = m.group(1)
+        break  # dependencies always come after requires-python
+
+
 @nox.session
 def pre_commit(session: nox.Session) -> None:
     session.install("pre-commit")
 
     session.run("pre-commit", "run", "--all-files")
 
 
@@ -33,39 +59,37 @@
 @nox.session(python=["3.8", "3.9", "3.10", "3.12"], tags=["tests"])
 def tests(session: nox.Session) -> None:
     session.install(".[tests]")
 
     session.run("pytest", *session.posargs)
 
 
-@nox.session(python="3.7", tags=["tests"])
-def tests_oldestAttrs(session: nox.Session) -> None:
-    # Keeps attrs pin in sync with pyproject.toml/dependencies.
-    session.install(".[tests]", "attrs==17.4.0")
+@nox.session(python=OLDEST_PYTHON, tags=["tests"])
+def tests_oldest_attrs(session: nox.Session) -> None:
+    session.install(".[tests]", f"attrs=={OLDEST_ATTRS}")
 
     _cov(session)
 
 
 @nox.session
 def coverage_report(session: nox.Session) -> None:
     session.install("coverage[toml]")
 
     session.run("coverage", "combine")
-    session.run("coverage", "report")
+    session.run("coverage", "report", "--fail-under=100")
 
 
 @nox.session
 def mypy(session: nox.Session) -> None:
     session.install(".", "mypy")
 
     session.run("mypy", "typing_examples.py")
 
 
-# Keep python in sync with ci.yml/docs and .readthedocs.yaml.
-@nox.session(python="3.10")
+@nox.session(python=DOCS_PYTHON)
 def docs(session: nox.Session) -> None:
     session.install(".[docs]")
 
     for cmd in ["html", "doctest"]:
         session.run(
             # fmt: off
             "python", "-m", "sphinx",
```

### Comparing `environ_config-23.1.0/.github/CODE_OF_CONDUCT.md` & `environ_config-23.2.0/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `environ_config-23.1.0/.github/CONTRIBUTING.md` & `environ_config-23.2.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `environ_config-23.1.0/.github/PULL_REQUEST_TEMPLATE.md` & `environ_config-23.2.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `environ_config-23.1.0/.github/workflows/pypi-package.yml` & `environ_config-23.2.0/.github/workflows/pypi-package.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,85 +1,69 @@
 ---
-name: Deploy to (Test-) PyPI
+name: Build & maybe upload PyPI package
 
 on:
   push:
+    branches: [main]
     tags: ["*"]
+  pull_request:
     branches: [main]
   release:
     types:
       - published
+  workflow_dispatch:
 
 permissions:
   contents: read
+  # Needed for trusted publishing.
+  id-token: write
 
 jobs:
+  # Always build & lint package.
   build-package:
+    name: Build & verify package
     runs-on: ubuntu-latest
-    steps:
-      - uses: step-security/harden-runner@v2
-        with:
-          disable-sudo: true
-          egress-policy: block
-          allowed-endpoints: >
-            files.pythonhosted.org
-            github.com:443
-            pypi.org:443
-            test.pypi.org:443
 
+    steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - uses: hynek/build-and-inspect-python-package@v1
 
+  # Upload to Test PyPI on every commit on main.
   release-test-pypi:
-    # Upload to Test PyPI on every commit & pushed tag.
+    name: Publish in-dev package to test.pypi.org
     environment: release-test-pypi
+    if: github.event_name == 'push' && github.ref == 'refs/heads/main'
     runs-on: ubuntu-latest
     needs: build-package
 
     steps:
-      - uses: step-security/harden-runner@v2
-        with:
-          disable-sudo: true
-          egress-policy: block
-          allowed-endpoints: >
-            test.pypi.org:443
-
       - name: Download packages built by build-and-inspect-python-package
         uses: actions/download-artifact@v3
         with:
           name: Packages
           path: dist
 
-      - name: Publish package to Test PyPI
+      - name: Upload package to Test PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
-          password: ${{ secrets.TEST_PYPI_API_TOKEN }}
-          repository_url: https://test.pypi.org/legacy/
+          repository-url: https://test.pypi.org/legacy/
 
+  # Upload to real PyPI on GitHub Releases.
   release-pypi:
-    # Upload to real PyPI on GitHub Releases.
+    name: Publish released package to pypi.org
     environment: release-pypi
     if: github.event.action == 'published'
     runs-on: ubuntu-latest
     needs: build-package
 
     steps:
-      - uses: step-security/harden-runner@v2
-        with:
-          disable-sudo: true
-          egress-policy: audit
-          allowed-endpoints: >
-            upload.pypi.org:443
-
       - name: Download packages built by build-and-inspect-python-package
         uses: actions/download-artifact@v3
         with:
           name: Packages
           path: dist
 
-      - name: Publish package to PyPI
+      - name: Upload package to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
-        with:
-          password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `environ_config-23.1.0/docs/Makefile` & `environ_config-23.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `environ_config-23.1.0/docs/api.md` & `environ_config-23.2.0/docs/api.md`

 * *Files identical despite different names*

### Comparing `environ_config-23.1.0/docs/conf.py` & `environ_config-23.2.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,12 +280,12 @@
 # How to display URL addresses: 'footnote', 'no', or 'inline'.
 # texinfo_show_urls = 'footnote'
 
 # If true, do not generate a @detailmenu in the "Top" node's menu.
 # texinfo_no_detailmenu = False
 
 
-# Refer to the Python standard library.
+# Refer to the Python standard library.and attrts
 intersphinx_mapping = {
-    "https://docs.python.org/3/": None,
-    "https://www.attrs.org/en/stable": None,
+    "python": ("https://docs.python.org/3/", None),
+    "attrs": ("https://www.attrs.org/en/stable", None),
 }
```

### Comparing `environ_config-23.1.0/docs/make.bat` & `environ_config-23.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `environ_config-23.1.0/docs/testing.md` & `environ_config-23.2.0/docs/testing.md`

 * *Files identical despite different names*

### Comparing `environ_config-23.1.0/docs/tutorial.md` & `environ_config-23.2.0/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `environ_config-23.1.0/src/environ/__init__.py` & `environ_config-23.2.0/src/environ/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,11 +62,12 @@
         stacklevel=2,
     )
 
     meta = metadata("environ-config")
 
     if name == "__uri__":
         return meta["Project-URL"].split(" ", 1)[-1]
-    elif name == "__email__":
+
+    if name == "__email__":
         return meta["Author-email"].split("<", 1)[1].rstrip(">")
 
     return meta[dunder_to_metadata[name]]
```

### Comparing `environ_config-23.1.0/src/environ/_environ_config.py` & `environ_config-23.2.0/src/environ/_environ_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 import logging
 import os
 
-from typing import Any, Callable, TypeVar
+from typing import Any, Callable, TypeVar, overload
 
 import attr
 
 from .exceptions import MissingEnvValueError
 
 
 CNF_KEY = "environ_config"
@@ -56,21 +56,38 @@
 
 RAISE = Raise()
 
 
 T = TypeVar("T")
 
 
+@overload
+def config(
+    *,
+    prefix: str | Sentinel = PREFIX_NOT_SET,
+    from_environ: str = "from_environ",
+    generate_help: str = "generate_help",
+    frozen: bool = False,
+) -> Callable[[type[T]], type[T]]:
+    ...
+
+
+@overload
+def config(maybe_cls: type[T]) -> type[T]:
+    ...
+
+
 def config(
     maybe_cls: type[T] | None = None,
+    *,
     prefix: str | Sentinel = PREFIX_NOT_SET,
     from_environ: str = "from_environ",
     generate_help: str = "generate_help",
     frozen: bool = False,
-) -> T:
+) -> type[T] | Callable[[type[T]], type[T]]:
     """
     Make a class a configuration class.
 
     :param prefix: The prefix that is used for the env variables.  If you have
         an `var` attribute on the class and you leave the default argument
         value of *PREFIX_NOT_SET*, the *DEFAULT_PREFIX* value of ``APP`` will
         be used and *environ-config* will look for an environment variable
@@ -160,16 +177,15 @@
 
 def _env_to_bool(val: str | bool) -> bool:
     """
     Convert *val* to a bool if it's not a bool in the first place.
     """
     if isinstance(val, bool):
         return val
-    val = val.strip().lower()
-    if val in ("1", "true", "yes"):
+    if val.strip().lower() in ("1", "true", "yes"):
         return True
 
     return False
 
 
 def bool_var(
     default: Any = RAISE, name: str | None = None, help: str | None = None
@@ -231,23 +247,20 @@
 
 
 def _default_getter(environ, metadata, prefix, name):
     """
     This default lookup implementation simply gets values from *environ*.
     """
     ce = metadata[CNF_KEY]
-    if ce.name is not None:
-        var = ce.name
-    else:
-        var = "_".join(prefix + (name,)).upper()
+    var = ce.name if ce.name is not None else "_".join((*prefix, name)).upper()
     log.debug("looking for env var '%s'.", var)
     try:
         return environ[var]
     except KeyError:
-        raise MissingEnvValueError(var)
+        raise MissingEnvValueError(var) from None
 
 
 def _to_config_recurse(config_cls, environ, prefixes, default=RAISE):
     """
     Traverse *config_cls* to construct an instance with values from *environ*.
 
     This function walks through a potential tree of config definition classes
@@ -270,15 +283,15 @@
         except KeyError:
             continue
         name = attr_obj.name
 
         if ce.sub_cls is not None:
             prefix = ce.sub_cls._prefix or name
             got[name] = _to_config_recurse(
-                ce.sub_cls, environ, prefixes + (prefix,), default=ce.default
+                ce.sub_cls, environ, (*prefixes, prefix), default=ce.default
             )
         else:
             getter = ce.callback or _default_getter
             try:
                 got[name] = getter(environ, attr_obj.metadata, prefixes, name)
             except MissingEnvValueError as exc:
                 if isinstance(ce.default, Raise):
@@ -290,19 +303,20 @@
                         else ce.default
                     )
 
     if missing_vars:
         # If we were told to raise OR if we got *any* values for our attrs, we
         # will raise a `MissingEnvValueError` with all the missing variables
         if isinstance(default, Raise) or got:
-            raise MissingEnvValueError(*missing_vars)
-        # otherwise we will simply use the default passed into this call
-        else:
-            # Should be no need to handle `Factory`s here
-            return default
+            raise MissingEnvValueError(*missing_vars) from None
+
+        # Otherwise we will simply use the default passed into this call.
+        # Should be no need to handle `Factory`s here.
+        return default
+
     # Merge the defaulted and actually collected values into the config type
     defaulted.update(got)
     return config_cls(**defaulted)
 
 
 def to_config(config_cls: type[T], environ: dict[str, str] = os.environ) -> T:
     """
```

### Comparing `environ_config-23.1.0/src/environ/exceptions.py` & `environ_config-23.2.0/src/environ/exceptions.py`

 * *Files identical despite different names*

### Comparing `environ_config-23.1.0/src/environ/secrets/__init__.py` & `environ_config-23.2.0/src/environ/secrets/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,18 +136,17 @@
                 environ.get(self._env_name, self._env_default)
             )
 
         ce = metadata[CNF_KEY]
         ic = metadata[CNF_INI_SECRET_KEY]
         section = ic.section
 
-        if ce.name is not None:
-            var = ce.name
-        else:
-            var = "_".join(prefix[1:] + (name,))
+        var = (
+            ce.name if ce.name is not None else "_".join(prefix[1:] + (name,))
+        )
         try:
             log.debug("looking for '%s' in section '%s'.", var, section)
             val = self._cfg.get(section, var)
 
             return _SecretStr(val)
         except NoOptionError:
             return _get_default_secret(var, ce.default)
@@ -288,16 +287,16 @@
         # The frame numbers varies across attrs versions. Use this convoluted
         # form to make the call lazy.
         if (
             sys._getframe(1).f_code.co_name == "__repr__"
             or sys._getframe(2).f_code.co_name == "__repr__"
         ):
             return "<SECRET>"
-        else:
-            return str.__repr__(self)
+
+        return str.__repr__(self)
 
 
 CNF_INI_SECRET_KEY = CNF_KEY + "_ini_secret"
 
 
 @attr.s
 class _INIConfig:
```

### Comparing `environ_config-23.1.0/src/environ/secrets/awssm.py` & `environ_config-23.2.0/src/environ/secrets/awssm.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             self._client = _build_secretsmanager_client()
 
         return self._client
 
     def secret(
         self,
         default: Any = RAISE,
-        converter: Callable = convert_secret("SecretString"),
+        converter: Callable = convert_secret("SecretString"),  # noqa: B008
         name: str | None = None,
         help: str | None = None,
     ):
         """
         Declare a secrets manager secret on an `environ.config`-decorated class
 
         All parameters work just like in `environ.var`.
@@ -98,15 +98,15 @@
         if ce.name:
             secret_name_envvar = ce.name
             log.debug(
                 "override env variable with explicit name %s",
                 secret_name_envvar,
             )
         else:
-            parts = prefix + (name,)
+            parts = (*prefix, name)
             secret_name_envvar = "_".join(parts).upper()
             log.debug(
                 "secret name environment variable %s", secret_name_envvar
             )
 
         try:
             secret_name = environ[secret_name_envvar]
```

### Comparing `environ_config-23.1.0/tests/test_class_generate_help.py` & `environ_config-23.2.0/tests/test_class_generate_help.py`

 * *Files identical despite different names*

### Comparing `environ_config-23.1.0/tests/test_class_to_config.py` & `environ_config-23.2.0/tests/test_class_to_config.py`

 * *Files identical despite different names*

### Comparing `environ_config-23.1.0/tests/test_environ_config.py` & `environ_config-23.2.0/tests/test_environ_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -369,15 +369,15 @@
             child = environ.group(Child)
 
         cfg = environ.to_config(
             WithRequiredChild, {"PARENT_CHILD_GRANDCHILD": "FOO"}
         )
         assert cfg.child.grandchild == "FOO"
         with pytest.raises(environ.MissingEnvValueError) as e:
-            environ.to_config(WithRequiredChild, dict())
+            environ.to_config(WithRequiredChild, {})
         assert ("PARENT_CHILD_GRANDCHILD",) == e.value.args
 
     def test_required_group_optional_child_missing(self):
         """
         Required groups are fully structured if the only child is optional.
         """
 
@@ -385,15 +385,15 @@
         class WithRequiredChild:
             @environ.config(prefix="CHILD")
             class Child:
                 grandchild = environ.var("FOO")
 
             child = environ.group(Child)
 
-        cfg = environ.to_config(WithRequiredChild, dict())
+        cfg = environ.to_config(WithRequiredChild, {})
         assert cfg.child.grandchild == "FOO"
 
     def test_optional_group_required_child_missing(self):
         """
         Optional groups are set to `None` if a required child is missing.
         """
 
@@ -401,15 +401,15 @@
         class WithOptionalChild:
             @environ.config(prefix="CHILD")
             class Child:
                 grandchild = environ.var()
 
             child = environ.group(Child, optional=True)
 
-        cfg = environ.to_config(WithOptionalChild, dict())
+        cfg = environ.to_config(WithOptionalChild, {})
         assert cfg.child is None
 
     def test_optional_group_optional_child_missing(self):
         """
         Optional groups with an optional child is fully structured.
         """
 
@@ -417,15 +417,15 @@
         class WithOptionalChild:
             @environ.config(prefix="CHILD")
             class Child:
                 grandchild = environ.var("FOO")
 
             child = environ.group(Child, optional=True)
 
-        cfg = environ.to_config(WithOptionalChild, dict())
+        cfg = environ.to_config(WithOptionalChild, {})
         assert cfg.child.grandchild == "FOO"
 
     def test_optional_group_mixed_children_all_missing(self):
         """
         Optional groups are set to `None` if all mixed children are missing.
         """
 
@@ -434,15 +434,15 @@
             @environ.config(prefix="CHILD")
             class Child:
                 grandchild_a = environ.var()
                 grandchild_b = environ.var("FOO")
 
             child = environ.group(Child, optional=True)
 
-        cfg = environ.to_config(WithOptionalChild, dict())
+        cfg = environ.to_config(WithOptionalChild, {})
         assert cfg.child is None
 
     def test_optional_group_mixed_children_optional_present(self):
         """
         Optional groups are required if any optional child is present.
         """
 
@@ -476,14 +476,14 @@
 
                 grandchild = environ.group(GrandChild, optional=True)
 
             child = environ.group(Child)
 
         # By providing nothing, we expect the grandchild to default to `None`
         # which will fulfill the requirement that it have a value in the child
-        cfg = environ.to_config(WithOptionalGrandChild, dict())
+        cfg = environ.to_config(WithOptionalGrandChild, {})
         assert cfg.child.grandchild is None
         # We also ensure that a properly set value is stored as expected
         cfg = environ.to_config(
             WithOptionalGrandChild, {"PARENT_CHILD_GRANDCHILD_FOO": "BAR"}
         )
         assert cfg.child.grandchild.foo == "BAR"
```

### Comparing `environ_config-23.1.0/tests/test_packaging.py` & `environ_config-23.2.0/tests/test_packaging.py`

 * *Files identical despite different names*

### Comparing `environ_config-23.1.0/tests/test_secrets.py` & `environ_config-23.2.0/tests/test_secrets.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,24 +241,24 @@
 
         cfg = environ.to_config(Cfg, fake_environ)
 
         assert _SecretStr("foo") == cfg.pw
 
 
 @pytest.fixture
-def secrets_dir(tmpdir):
+def secrets_dir(tmp_path):
     def make_secrets_file(name, content):
-        secret_file = tmpdir.join(name)
-        secret_file.write(content)
+        secret_file = tmp_path / name
+        secret_file.write_text(content)
 
     make_secrets_file("empty", "")
     make_secrets_file("apples", "apples\n")
     make_secrets_file("oranges", "oranges")
 
-    return str(tmpdir)
+    return str(tmp_path)
 
 
 class TestDirectorySecrets:
     def test_secret_content(self, secrets_dir):
         """
         Reading secrets with different content.
         """
@@ -295,15 +295,15 @@
         assert _SecretStr("apples\n") == cfg.has_newline
         assert _SecretStr("oranges") == cfg.no_newline
 
     def test_secret_from_env(self, secrets_dir):
         """
         A directory can be specified in an environment variable.
         """
-        dir = DirectorySecrets.from_path_in_env("SECRETS_DIR", "/tmp")
+        dir = DirectorySecrets.from_path_in_env("SECRETS_DIR", None)
 
         @environ.config
         class Cfg:
             apples = dir.secret()
 
         cfg = environ.to_config(Cfg, {"SECRETS_DIR": secrets_dir})
         assert _SecretStr("apples\n") == cfg.apples
```

### Comparing `environ_config-23.1.0/tests/test_secrets_awssm.py` & `environ_config-23.2.0/tests/test_secrets_awssm.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from environ.secrets import SecretsManagerSecrets, _SecretStr
 
 
 @pytest.fixture(name="shut_boto_up", autouse=True, scope="session")
 def _shut_boto_up():
     import logging
 
-    for name in logging.Logger.manager.loggerDict.keys():
+    for name in logging.Logger.manager.loggerDict:
         if ("boto" in name) or ("urllib3" in name):
             logging.getLogger(name).setLevel(logging.WARNING)
 
 
 @pytest.fixture(name="force_region", autouse=True, scope="session")
 def _force_region():
     with patch.dict(os.environ, {"AWS_DEFAULT_REGION": "us-east-1"}):
```

### Comparing `environ_config-23.1.0/LICENSE` & `environ_config-23.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `environ_config-23.1.0/PKG-INFO` & `environ_config-23.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: environ-config
-Version: 23.1.0
+Version: 23.2.0
 Summary: Boilerplate-free configuration with env variables.
 Project-URL: Documentation, https://environ-config.readthedocs.io/
 Project-URL: Changelog, https://environ-config.rtfd.io/en/stable/changelog.html
 Project-URL: Bug Tracker, https://github.com/hynek/environ-config/issues
 Project-URL: Source Code, https://github.com/hynek/environ-config
 Project-URL: Funding, https://github.com/sponsors/hynek
 Project-URL: Tidelift, https://tidelift.com/subscription/pkg/pypi-environ-config?utm_source=pypi-environ-config&utm_medium=pypi
@@ -12,25 +12,21 @@
 License-Expression: Apache-2.0
 License-File: LICENSE
 License-File: NOTICE
 Keywords: app,cfg,config,env
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Requires-Dist: attrs>=17.4.0
 Requires-Dist: importlib-metadata; python_version < '3.8'
 Provides-Extra: aws
 Requires-Dist: boto3; extra == 'aws'
 Provides-Extra: dev
@@ -138,27 +134,17 @@
 Available as part of the Tidelift Subscription.
 
 The maintainers of *structlog* and thousands of other packages are working with Tidelift to deliver commercial support and maintenance for the open source packages you use to build your applications. Save time, reduce risk, and improve code health, while paying the maintainers of the exact packages you use. [Learn more.](https://tidelift.com/subscription/pkg/pypi-environ-config?utm_source=pypi-environ-config&utm_medium=pypi)
 
 
 ## Release Information
 
-### Backwards-incompatible Changes
+### Fixed
 
-*none*
-
-### Deprecations
-
-*none*
-
-### Changes
-
-- `environ.secrets.DirectorySecrets.from_path()` now works when loading from `os.environ`.
-  [#45](https://github.com/hynek/environ-config/issues/45)
-- Public APIs now carry type hints (except in-class methods like ``AppConfig.from_environ()``).
-  [#49](https://github.com/hynek/environ-config/issues/49)
+- Type hints for `environ.config()` now allow for arguments (e.g. `@environ.config(prefix="")`).
+  [#56](https://github.com/hynek/environ-config/issues/56)
 
 
  ---
 
  [**Full Changelog**](https://www.structlog.org/en/stable/changelog.html)
```


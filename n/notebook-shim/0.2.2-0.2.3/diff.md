# Comparing `tmp/notebook_shim-0.2.2.tar.gz` & `tmp/notebook_shim-0.2.3.tar.gz`

## Comparing `notebook_shim-0.2.2.tar` & `notebook_shim-0.2.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     4170 2020-02-02 00:00:00.000000 notebook_shim-0.2.2/CHANGELOG.md
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 notebook_shim-0.2.2/MANIFEST.in
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 notebook_shim-0.2.2/RELEASE.md
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 notebook_shim-0.2.2/conftest.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 notebook_shim-0.2.2/.github/workflows/check-release.yml
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 notebook_shim-0.2.2/.github/workflows/enforce-label.yml
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 notebook_shim-0.2.2/.github/workflows/prep-release.yaml
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 notebook_shim-0.2.2/.github/workflows/publish-release.yaml
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 notebook_shim-0.2.2/.github/workflows/test.yml
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 notebook_shim-0.2.2/jupyter_server_config.d/notebook_shim.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 notebook_shim-0.2.2/notebook_shim/__init__.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 notebook_shim-0.2.2/notebook_shim/_version.py
--rw-r--r--   0        0        0     5189 2020-02-02 00:00:00.000000 notebook_shim-0.2.2/notebook_shim/nbserver.py
--rw-r--r--   0        0        0    11718 2020-02-02 00:00:00.000000 notebook_shim-0.2.2/notebook_shim/shim.py
--rw-r--r--   0        0        0     5600 2020-02-02 00:00:00.000000 notebook_shim-0.2.2/notebook_shim/traits.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 notebook_shim-0.2.2/notebook_shim/tests/__init__.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 notebook_shim-0.2.2/notebook_shim/tests/mockextension.py
--rw-r--r--   0        0        0     3850 2020-02-02 00:00:00.000000 notebook_shim-0.2.2/notebook_shim/tests/test_extension.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 notebook_shim-0.2.2/notebook_shim/tests/confs/jupyter_my_ext_config.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 notebook_shim-0.2.2/notebook_shim/tests/confs/jupyter_notebook_config.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notebook_shim-0.2.2/notebook_shim/tests/confs/jupyter_server_config.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 notebook_shim-0.2.2/.gitignore
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 notebook_shim-0.2.2/LICENSE
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 notebook_shim-0.2.2/README.md
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 notebook_shim-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 notebook_shim-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 notebook_shim-0.2.3/CHANGELOG.md
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 notebook_shim-0.2.3/MANIFEST.in
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 notebook_shim-0.2.3/RELEASE.md
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 notebook_shim-0.2.3/conftest.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 notebook_shim-0.2.3/.github/workflows/check-release.yml
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 notebook_shim-0.2.3/.github/workflows/enforce-label.yml
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 notebook_shim-0.2.3/.github/workflows/prep-release.yaml
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 notebook_shim-0.2.3/.github/workflows/publish-release.yaml
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 notebook_shim-0.2.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 notebook_shim-0.2.3/jupyter_server_config.d/notebook_shim.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 notebook_shim-0.2.3/notebook_shim/__init__.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 notebook_shim-0.2.3/notebook_shim/_version.py
+-rw-r--r--   0        0        0     5189 2020-02-02 00:00:00.000000 notebook_shim-0.2.3/notebook_shim/nbserver.py
+-rw-r--r--   0        0        0    11733 2020-02-02 00:00:00.000000 notebook_shim-0.2.3/notebook_shim/shim.py
+-rw-r--r--   0        0        0     5600 2020-02-02 00:00:00.000000 notebook_shim-0.2.3/notebook_shim/traits.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 notebook_shim-0.2.3/notebook_shim/tests/__init__.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 notebook_shim-0.2.3/notebook_shim/tests/mockextension.py
+-rw-r--r--   0        0        0     3850 2020-02-02 00:00:00.000000 notebook_shim-0.2.3/notebook_shim/tests/test_extension.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 notebook_shim-0.2.3/notebook_shim/tests/confs/jupyter_my_ext_config.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 notebook_shim-0.2.3/notebook_shim/tests/confs/jupyter_notebook_config.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 notebook_shim-0.2.3/notebook_shim/tests/confs/jupyter_server_config.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 notebook_shim-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 notebook_shim-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 notebook_shim-0.2.3/README.md
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 notebook_shim-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 notebook_shim-0.2.3/PKG-INFO
```

### Comparing `notebook_shim-0.2.2/CHANGELOG.md` & `notebook_shim-0.2.3/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,27 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.2.3
+
+([Full Changelog](https://github.com/jupyter/notebook_shim/compare/v0.2.2...bb84e6475a757b6299cb07ec3ce027a8c57d052e))
+
+### Maintenance and upkeep improvements
+
+- Add show_banner to ignored_traits [#29](https://github.com/jupyter/notebook_shim/pull/29) ([@echarles](https://github.com/echarles))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter/notebook_shim/graphs/contributors?from=2022-11-03&to=2023-04-24&type=c))
+
+[@echarles](https://github.com/search?q=repo%3Ajupyter%2Fnotebook_shim+involves%3Aecharles+updated%3A2022-11-03..2023-04-24&type=Issues) | [@Zsailer](https://github.com/search?q=repo%3Ajupyter%2Fnotebook_shim+involves%3AZsailer+updated%3A2022-11-03..2023-04-24&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 0.2.2
 
 ([Full Changelog](https://github.com/jupyter/notebook_shim/compare/v0.2.0...e1f1219888d9bfa69fc0e1f130f6f1bcf3825fcb))
 
 ### Bugs fixed
 
 - Fixes #7 [#24](https://github.com/jupyter/notebook_shim/pull/24) ([@dleen](https://github.com/dleen))
@@ -17,16 +33,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter/notebook_shim/graphs/contributors?from=2022-10-17&to=2022-11-03&type=c))
 
 [@dleen](https://github.com/search?q=repo%3Ajupyter%2Fnotebook_shim+involves%3Adleen+updated%3A2022-10-17..2022-11-03&type=Issues) | [@Zsailer](https://github.com/search?q=repo%3Ajupyter%2Fnotebook_shim+involves%3AZsailer+updated%3A2022-10-17..2022-11-03&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.2.1
 
 ([Full Changelog](https://github.com/jupyter/notebook_shim/compare/v0.2.0...b72af7411fa41115c3025a95f261e10bf0221fb0))
 
 ### Bugs fixed
 
 - Add config file [#23](https://github.com/jupyter/notebook_shim/pull/23) ([@dleen](https://github.com/dleen))
```

### Comparing `notebook_shim-0.2.2/.github/workflows/check-release.yml` & `notebook_shim-0.2.3/.github/workflows/check-release.yml`

 * *Files identical despite different names*

### Comparing `notebook_shim-0.2.2/.github/workflows/prep-release.yaml` & `notebook_shim-0.2.3/.github/workflows/prep-release.yaml`

 * *Files identical despite different names*

### Comparing `notebook_shim-0.2.2/.github/workflows/publish-release.yaml` & `notebook_shim-0.2.3/.github/workflows/publish-release.yaml`

 * *Files identical despite different names*

### Comparing `notebook_shim-0.2.2/.github/workflows/test.yml` & `notebook_shim-0.2.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `notebook_shim-0.2.2/notebook_shim/nbserver.py` & `notebook_shim-0.2.3/notebook_shim/nbserver.py`

 * *Files identical despite different names*

### Comparing `notebook_shim-0.2.2/notebook_shim/shim.py` & `notebook_shim-0.2.3/notebook_shim/shim.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         extapp_name=extapp_name
     )
 )
 
 
 # A tuple of traits that shouldn't be shimmed or throw any
 # warnings of any kind.
-IGNORED_TRAITS = ("open_browser", "log_level", "log_format", "default_url")
+IGNORED_TRAITS = ("open_browser", "log_level", "log_format", "default_url", "show_banner")
 
 
 class NotebookConfigShimMixin:
     """A Mixin class for shimming configuration from
     NotebookApp to ServerApp. This class handles warnings, errors,
     etc.
```

### Comparing `notebook_shim-0.2.2/notebook_shim/traits.py` & `notebook_shim-0.2.3/notebook_shim/traits.py`

 * *Files identical despite different names*

### Comparing `notebook_shim-0.2.2/notebook_shim/tests/mockextension.py` & `notebook_shim-0.2.3/notebook_shim/tests/mockextension.py`

 * *Files identical despite different names*

### Comparing `notebook_shim-0.2.2/notebook_shim/tests/test_extension.py` & `notebook_shim-0.2.3/notebook_shim/tests/test_extension.py`

 * *Files identical despite different names*

### Comparing `notebook_shim-0.2.2/.gitignore` & `notebook_shim-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `notebook_shim-0.2.2/LICENSE` & `notebook_shim-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `notebook_shim-0.2.2/README.md` & `notebook_shim-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `notebook_shim-0.2.2/pyproject.toml` & `notebook_shim-0.2.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -35,23 +35,25 @@
 "jupyter_server_config.d/notebook_shim.json" = "etc/jupyter/jupyter_server_config.d/notebook_shim.json"
 
 [project.optional-dependencies]
 test = [
     "pytest",
     "pytest-tornasync",
     "pytest-console-scripts",
+    "pytest_jupyter"
 ]
 
 
 
+
 [tool.hatch.version]
 path = "notebook_shim/_version.py"
 
 [tool.tbump.version]
-current = "0.2.2"
+current = "0.2.3"
 regex = '''
   (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)
   ((?P<channel>a|b|rc|.dev)(?P<release>\d+))?
 '''
 
 [tool.tbump.git]
 message_template = "Bump to {new_version}"
```

### Comparing `notebook_shim-0.2.2/PKG-INFO` & `notebook_shim-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notebook_shim
-Version: 0.2.2
+Version: 0.2.3
 Summary: A shim layer for notebook traits and config
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022 Project Jupyter Contributors
         All rights reserved.
         
@@ -47,14 +47,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Requires-Dist: jupyter-server<3,>=1.8
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-console-scripts; extra == 'test'
+Requires-Dist: pytest-jupyter; extra == 'test'
 Requires-Dist: pytest-tornasync; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Notebook Shim
 
 This project provides a way for JupyterLab and other frontends to switch to [Jupyter Server](https://github.com/jupyter/jupyter_server/) for their Python Web application backend.
```


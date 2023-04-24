# Comparing `tmp/microscopy_portfolio-0.0.4.tar.gz` & `tmp/microscopy_portfolio-0.0.5.tar.gz`

## Comparing `microscopy_portfolio-0.0.4.tar` & `microscopy_portfolio-0.0.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.4/.copier-answers.yml
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.4/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.4/.github/TEST_FAIL_TEMPLATE.md
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.4/.github/dependabot.yml
--rw-r--r--   0        0        0     4382 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.4/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.4/.github/workflows/datasets_ci.yml
--rw-r--r--   0        0        0     8848 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.4/datasets/datasets.json
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.4/examples/example.ipynb
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.4/scripts/download_and_examine.py
--rwxr-xr-x   0        0        0      328 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.4/scripts/export_portfolio_to_json.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.4/src/microscopy_portfolio/__init__.py
--rw-r--r--   0        0        0     8506 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.4/src/microscopy_portfolio/denoiseg_datasets.py
--rw-r--r--   0        0        0     7742 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.4/src/microscopy_portfolio/denoising_datasets.py
--rw-r--r--   0        0        0    11273 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.4/src/microscopy_portfolio/portfolio.py
--rw-r--r--   0        0        0     7260 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.4/src/microscopy_portfolio/portfolio_entry.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.4/src/microscopy_portfolio/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.4/tests/conftest.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.4/tests/test_denoiseg_datasets.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.4/tests/test_denoising_datasets.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.4/tests/test_portfolio.py
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.4/tests/test_portfolio_entry.py
--rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.4/tests/utils.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.4/.gitignore
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.4/LICENSE
--rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.4/README.md
--rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4798 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.5/.copier-answers.yml
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.5/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.5/.github/TEST_FAIL_TEMPLATE.md
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.5/.github/dependabot.yml
+-rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.5/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.5/.github/workflows/datasets_ci.yml
+-rw-r--r--   0        0        0     8848 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.5/datasets/datasets.json
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.5/examples/example.ipynb
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.5/scripts/download_and_examine.py
+-rwxr-xr-x   0        0        0      328 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.5/scripts/export_portfolio_to_json.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.5/src/microscopy_portfolio/__init__.py
+-rw-r--r--   0        0        0     8506 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.5/src/microscopy_portfolio/denoiseg_datasets.py
+-rw-r--r--   0        0        0     7742 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.5/src/microscopy_portfolio/denoising_datasets.py
+-rw-r--r--   0        0        0    11273 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.5/src/microscopy_portfolio/portfolio.py
+-rw-r--r--   0        0        0     7260 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.5/src/microscopy_portfolio/portfolio_entry.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.5/src/microscopy_portfolio/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.5/tests/conftest.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.5/tests/test_denoiseg_datasets.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.5/tests/test_denoising_datasets.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.5/tests/test_portfolio.py
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.5/tests/test_portfolio_entry.py
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.5/tests/utils.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.5/README.md
+-rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4798 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.5/PKG-INFO
```

### Comparing `microscopy_portfolio-0.0.4/.copier-answers.yml` & `microscopy_portfolio-0.0.5/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.4/.pre-commit-config.yaml` & `microscopy_portfolio-0.0.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.4/.github/workflows/ci.yml` & `microscopy_portfolio-0.0.5/.github/workflows/ci.yml`

 * *Files 0% similar despite different names*

```diff
@@ -122,14 +122,15 @@
     needs: test
     if: success() && startsWith(github.ref, 'refs/tags/') && github.event_name != 'schedule'
     runs-on: ubuntu-latest
     environment: release
     permissions:
       # IMPORTANT: this permission is mandatory for trusted publishing
       id-token: write
+      contents: write
 
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - name: Set up Python
```

### Comparing `microscopy_portfolio-0.0.4/.github/workflows/datasets_ci.yml` & `microscopy_portfolio-0.0.5/.github/workflows/datasets_ci.yml`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.4/datasets/datasets.json` & `microscopy_portfolio-0.0.5/datasets/datasets.json`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.4/examples/example.ipynb` & `microscopy_portfolio-0.0.5/examples/example.ipynb`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.4/scripts/download_and_examine.py` & `microscopy_portfolio-0.0.5/scripts/download_and_examine.py`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.4/src/microscopy_portfolio/__init__.py` & `microscopy_portfolio-0.0.5/src/microscopy_portfolio/__init__.py`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.4/src/microscopy_portfolio/denoiseg_datasets.py` & `microscopy_portfolio-0.0.5/src/microscopy_portfolio/denoiseg_datasets.py`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.4/src/microscopy_portfolio/denoising_datasets.py` & `microscopy_portfolio-0.0.5/src/microscopy_portfolio/denoising_datasets.py`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.4/src/microscopy_portfolio/portfolio.py` & `microscopy_portfolio-0.0.5/src/microscopy_portfolio/portfolio.py`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.4/src/microscopy_portfolio/portfolio_entry.py` & `microscopy_portfolio-0.0.5/src/microscopy_portfolio/portfolio_entry.py`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.4/tests/conftest.py` & `microscopy_portfolio-0.0.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.4/tests/test_denoiseg_datasets.py` & `microscopy_portfolio-0.0.5/tests/test_denoiseg_datasets.py`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.4/tests/test_denoising_datasets.py` & `microscopy_portfolio-0.0.5/tests/test_denoising_datasets.py`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.4/tests/test_portfolio.py` & `microscopy_portfolio-0.0.5/tests/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.4/tests/test_portfolio_entry.py` & `microscopy_portfolio-0.0.5/tests/test_portfolio_entry.py`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.4/tests/utils.py` & `microscopy_portfolio-0.0.5/tests/utils.py`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.4/.gitignore` & `microscopy_portfolio-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.4/LICENSE` & `microscopy_portfolio-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.4/README.md` & `microscopy_portfolio-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.4/pyproject.toml` & `microscopy_portfolio-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.4/PKG-INFO` & `microscopy_portfolio-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microscopy-portfolio
-Version: 0.0.4
+Version: 0.0.5
 Summary: A helper package to download example datasets used in various publications and deep-learning algorithms, including data featured in N2V, P(P)N2V, DivNoising, HDN, EmbedSeg, etc.
 Project-URL: homepage, https://github.com/juglab-torch/microscopy-portfolio
 Project-URL: repository, https://github.com/juglab-torch/microscopy-portfolio
 Author-email: Joran Deschamps <joran.deschamps@fht.org>
 License: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
```


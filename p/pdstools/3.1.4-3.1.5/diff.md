# Comparing `tmp/pdstools-3.1.4.tar.gz` & `tmp/pdstools-3.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdstools-3.1.4.tar", last modified: Mon Apr 17 15:59:51 2023, max compression
+gzip compressed data, was "pdstools-3.1.5.tar", last modified: Mon Apr 24 13:14:29 2023, max compression
```

## Comparing `pdstools-3.1.4.tar` & `pdstools-3.1.5.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:59:51.591575 pdstools-3.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-17 15:59:42.000000 pdstools-3.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-17 15:59:51.591575 pdstools-3.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-17 15:59:42.000000 pdstools-3.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:59:51.579575 pdstools-3.1.4/pdstools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-17 15:59:51.000000 pdstools-3.1.4/pdstools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-17 15:59:51.000000 pdstools-3.1.4/pdstools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:59:51.000000 pdstools-3.1.4/pdstools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-17 15:59:51.000000 pdstools-3.1.4/pdstools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-17 15:59:51.000000 pdstools-3.1.4/pdstools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-17 15:59:51.000000 pdstools-3.1.4/pdstools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-17 15:59:42.000000 pdstools-3.1.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:59:51.575575 pdstools-3.1.4/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:59:51.579575 pdstools-3.1.4/python/pdstools/
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-17 15:59:42.000000 pdstools-3.1.4/python/pdstools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:59:51.583575 pdstools-3.1.4/python/pdstools/adm/
--rw-r--r--   0 runner    (1001) docker     (123)    56177 2023-04-17 15:59:42.000000 pdstools-3.1.4/python/pdstools/adm/ADMDatamart.py
--rw-r--r--   0 runner    (1001) docker     (123)    40060 2023-04-17 15:59:42.000000 pdstools-3.1.4/python/pdstools/adm/ADMTrees.py
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-04-17 15:59:42.000000 pdstools-3.1.4/python/pdstools/adm/Tables.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 15:59:42.000000 pdstools-3.1.4/python/pdstools/adm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:59:51.583575 pdstools-3.1.4/python/pdstools/app/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-17 15:59:42.000000 pdstools-3.1.4/python/pdstools/app/Home.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 15:59:42.000000 pdstools-3.1.4/python/pdstools/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-17 15:59:42.000000 pdstools-3.1.4/python/pdstools/app/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:59:51.583575 pdstools-3.1.4/python/pdstools/app/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-04-17 15:59:42.000000 pdstools-3.1.4/python/pdstools/app/pages/Health Check.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:59:51.583575 pdstools-3.1.4/python/pdstools/ih/
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-04-17 15:59:42.000000 pdstools-3.1.4/python/pdstools/ih/IHAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 15:59:42.000000 pdstools-3.1.4/python/pdstools/ih/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-04-17 15:59:42.000000 pdstools-3.1.4/python/pdstools/ih/legacy_IH.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:59:51.583575 pdstools-3.1.4/python/pdstools/pega_io/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-17 15:59:42.000000 pdstools-3.1.4/python/pdstools/pega_io/API.py
--rw-r--r--   0 runner    (1001) docker     (123)    14118 2023-04-17 15:59:42.000000 pdstools-3.1.4/python/pdstools/pega_io/File.py
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-04-17 15:59:42.000000 pdstools-3.1.4/python/pdstools/pega_io/S3.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-17 15:59:42.000000 pdstools-3.1.4/python/pdstools/pega_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:59:51.587575 pdstools-3.1.4/python/pdstools/plots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 15:59:42.000000 pdstools-3.1.4/python/pdstools/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51016 2023-04-17 15:59:42.000000 pdstools-3.1.4/python/pdstools/plots/plot_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29608 2023-04-17 15:59:42.000000 pdstools-3.1.4/python/pdstools/plots/plots_plotly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:59:51.587575 pdstools-3.1.4/python/pdstools/reports/
--rw-r--r--   0 runner    (1001) docker     (123)    39159 2023-04-17 15:59:42.000000 pdstools-3.1.4/python/pdstools/reports/HealthCheck.qmd
--rw-r--r--   0 runner    (1001) docker     (123)    14084 2023-04-17 15:59:42.000000 pdstools-3.1.4/python/pdstools/reports/HealthCheckModel.qmd
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 15:59:42.000000 pdstools-3.1.4/python/pdstools/reports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:59:51.591575 pdstools-3.1.4/python/pdstools/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 15:59:42.000000 pdstools-3.1.4/python/pdstools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21567 2023-04-17 15:59:42.000000 pdstools-3.1.4/python/pdstools/utils/cdh_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-17 15:59:42.000000 pdstools-3.1.4/python/pdstools/utils/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-17 15:59:42.000000 pdstools-3.1.4/python/pdstools/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    15921 2023-04-17 15:59:42.000000 pdstools-3.1.4/python/pdstools/utils/hds_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-17 15:59:42.000000 pdstools-3.1.4/python/pdstools/utils/pega_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-17 15:59:42.000000 pdstools-3.1.4/python/pdstools/utils/polars_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-17 15:59:42.000000 pdstools-3.1.4/python/pdstools/utils/show_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-04-17 15:59:42.000000 pdstools-3.1.4/python/pdstools/utils/streamlit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-17 15:59:42.000000 pdstools-3.1.4/python/pdstools/utils/table_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-17 15:59:42.000000 pdstools-3.1.4/python/pdstools/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:59:51.591575 pdstools-3.1.4/python/pdstools/valuefinder/
--rw-r--r--   0 runner    (1001) docker     (123)    24381 2023-04-17 15:59:42.000000 pdstools-3.1.4/python/pdstools/valuefinder/ValueFinder.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 15:59:42.000000 pdstools-3.1.4/python/pdstools/valuefinder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 15:59:51.591575 pdstools-3.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:14:29.426708 pdstools-3.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-24 13:14:18.000000 pdstools-3.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-24 13:14:29.426708 pdstools-3.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-24 13:14:18.000000 pdstools-3.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:14:29.418708 pdstools-3.1.5/pdstools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-24 13:14:29.000000 pdstools-3.1.5/pdstools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-24 13:14:29.000000 pdstools-3.1.5/pdstools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:14:29.000000 pdstools-3.1.5/pdstools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-24 13:14:29.000000 pdstools-3.1.5/pdstools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-24 13:14:29.000000 pdstools-3.1.5/pdstools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-24 13:14:29.000000 pdstools-3.1.5/pdstools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-24 13:14:18.000000 pdstools-3.1.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:14:29.418708 pdstools-3.1.5/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:14:29.422708 pdstools-3.1.5/python/pdstools/
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-24 13:14:18.000000 pdstools-3.1.5/python/pdstools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:14:29.422708 pdstools-3.1.5/python/pdstools/adm/
+-rw-r--r--   0 runner    (1001) docker     (123)    56177 2023-04-24 13:14:18.000000 pdstools-3.1.5/python/pdstools/adm/ADMDatamart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40060 2023-04-24 13:14:18.000000 pdstools-3.1.5/python/pdstools/adm/ADMTrees.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-04-24 13:14:18.000000 pdstools-3.1.5/python/pdstools/adm/Tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:14:18.000000 pdstools-3.1.5/python/pdstools/adm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:14:29.422708 pdstools-3.1.5/python/pdstools/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-24 13:14:18.000000 pdstools-3.1.5/python/pdstools/app/Home.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:14:18.000000 pdstools-3.1.5/python/pdstools/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-24 13:14:18.000000 pdstools-3.1.5/python/pdstools/app/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:14:29.422708 pdstools-3.1.5/python/pdstools/app/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-04-24 13:14:18.000000 pdstools-3.1.5/python/pdstools/app/pages/Health Check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:14:29.422708 pdstools-3.1.5/python/pdstools/ih/
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-04-24 13:14:18.000000 pdstools-3.1.5/python/pdstools/ih/IHAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:14:18.000000 pdstools-3.1.5/python/pdstools/ih/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-04-24 13:14:18.000000 pdstools-3.1.5/python/pdstools/ih/legacy_IH.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:14:29.422708 pdstools-3.1.5/python/pdstools/pega_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-24 13:14:18.000000 pdstools-3.1.5/python/pdstools/pega_io/API.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14118 2023-04-24 13:14:18.000000 pdstools-3.1.5/python/pdstools/pega_io/File.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-04-24 13:14:18.000000 pdstools-3.1.5/python/pdstools/pega_io/S3.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-24 13:14:18.000000 pdstools-3.1.5/python/pdstools/pega_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:14:29.422708 pdstools-3.1.5/python/pdstools/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:14:18.000000 pdstools-3.1.5/python/pdstools/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51016 2023-04-24 13:14:18.000000 pdstools-3.1.5/python/pdstools/plots/plot_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29608 2023-04-24 13:14:18.000000 pdstools-3.1.5/python/pdstools/plots/plots_plotly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:14:29.422708 pdstools-3.1.5/python/pdstools/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)    39159 2023-04-24 13:14:18.000000 pdstools-3.1.5/python/pdstools/reports/HealthCheck.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)    14084 2023-04-24 13:14:18.000000 pdstools-3.1.5/python/pdstools/reports/HealthCheckModel.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:14:18.000000 pdstools-3.1.5/python/pdstools/reports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:14:29.426708 pdstools-3.1.5/python/pdstools/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:14:18.000000 pdstools-3.1.5/python/pdstools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21567 2023-04-24 13:14:18.000000 pdstools-3.1.5/python/pdstools/utils/cdh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-24 13:14:18.000000 pdstools-3.1.5/python/pdstools/utils/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-24 13:14:18.000000 pdstools-3.1.5/python/pdstools/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16467 2023-04-24 13:14:18.000000 pdstools-3.1.5/python/pdstools/utils/hds_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-24 13:14:18.000000 pdstools-3.1.5/python/pdstools/utils/pega_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-24 13:14:18.000000 pdstools-3.1.5/python/pdstools/utils/polars_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-24 13:14:18.000000 pdstools-3.1.5/python/pdstools/utils/show_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-04-24 13:14:18.000000 pdstools-3.1.5/python/pdstools/utils/streamlit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-24 13:14:18.000000 pdstools-3.1.5/python/pdstools/utils/table_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-24 13:14:18.000000 pdstools-3.1.5/python/pdstools/utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:14:29.426708 pdstools-3.1.5/python/pdstools/valuefinder/
+-rw-r--r--   0 runner    (1001) docker     (123)    24381 2023-04-24 13:14:18.000000 pdstools-3.1.5/python/pdstools/valuefinder/ValueFinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:14:18.000000 pdstools-3.1.5/python/pdstools/valuefinder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 13:14:29.426708 pdstools-3.1.5/setup.cfg
```

### Comparing `pdstools-3.1.4/LICENSE` & `pdstools-3.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.4/PKG-INFO` & `pdstools-3.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdstools
-Version: 3.1.4
+Version: 3.1.5
 Summary: Open source tooling that helps Data Scientists to analyze Pega models and conduct impactful analyses.
 Author-email: Stijn Kas <stijn.kas@pega.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/pegasystems/pega-datascientist-tools
 Project-URL: Bug Tracker, https://github.com/pegasystems/pega-datascientist-tools/issues
 Project-URL: Wiki, https://github.com/pegasystems/pega-datascientist-tools/wiki
 Project-URL: Docs, https://pegasystems.github.io/pega-datascientist-tools/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pdstools Version: 3.1.4 Summary: Open source
+Metadata-Version: 2.1 Name: pdstools Version: 3.1.5 Summary: Open source
 tooling that helps Data Scientists to analyze Pega models and conduct impactful
 analyses. Author-email: Stijn Kas
 kas@pega.com> License: Apache-2.0 Project-URL: Homepage, https://github.com/
 pegasystems/pega-datascientist-tools Project-URL: Bug Tracker, https://
 github.com/pegasystems/pega-datascientist-tools/issues Project-URL: Wiki,
 https://github.com/pegasystems/pega-datascientist-tools/wiki Project-URL: Docs,
 https://pegasystems.github.io/pega-datascientist-tools/ Keywords:
```

### Comparing `pdstools-3.1.4/README.md` & `pdstools-3.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.4/pdstools.egg-info/PKG-INFO` & `pdstools-3.1.5/pdstools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdstools
-Version: 3.1.4
+Version: 3.1.5
 Summary: Open source tooling that helps Data Scientists to analyze Pega models and conduct impactful analyses.
 Author-email: Stijn Kas <stijn.kas@pega.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/pegasystems/pega-datascientist-tools
 Project-URL: Bug Tracker, https://github.com/pegasystems/pega-datascientist-tools/issues
 Project-URL: Wiki, https://github.com/pegasystems/pega-datascientist-tools/wiki
 Project-URL: Docs, https://pegasystems.github.io/pega-datascientist-tools/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pdstools Version: 3.1.4 Summary: Open source
+Metadata-Version: 2.1 Name: pdstools Version: 3.1.5 Summary: Open source
 tooling that helps Data Scientists to analyze Pega models and conduct impactful
 analyses. Author-email: Stijn Kas
 kas@pega.com> License: Apache-2.0 Project-URL: Homepage, https://github.com/
 pegasystems/pega-datascientist-tools Project-URL: Bug Tracker, https://
 github.com/pegasystems/pega-datascientist-tools/issues Project-URL: Wiki,
 https://github.com/pegasystems/pega-datascientist-tools/wiki Project-URL: Docs,
 https://pegasystems.github.io/pega-datascientist-tools/ Keywords:
```

### Comparing `pdstools-3.1.4/pdstools.egg-info/SOURCES.txt` & `pdstools-3.1.5/pdstools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.4/pyproject.toml` & `pdstools-3.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.4/python/pdstools/__init__.py` & `pdstools-3.1.5/python/pdstools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Python pdstools"""
 
-__version__ = "3.1.4"
+__version__ = "3.1.5"
 
 from polars import enable_string_cache
 
 enable_string_cache(True)
 
 import sys
 from pathlib import Path
```

### Comparing `pdstools-3.1.4/python/pdstools/adm/ADMDatamart.py` & `pdstools-3.1.5/python/pdstools/adm/ADMDatamart.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.4/python/pdstools/adm/ADMTrees.py` & `pdstools-3.1.5/python/pdstools/adm/ADMTrees.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.4/python/pdstools/adm/Tables.py` & `pdstools-3.1.5/python/pdstools/adm/Tables.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.4/python/pdstools/app/cli.py` & `pdstools-3.1.5/python/pdstools/app/cli.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.4/python/pdstools/app/pages/Health Check.py` & `pdstools-3.1.5/python/pdstools/app/pages/Health Check.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.4/python/pdstools/ih/IHAnalysis.py` & `pdstools-3.1.5/python/pdstools/ih/IHAnalysis.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.4/python/pdstools/ih/legacy_IH.py` & `pdstools-3.1.5/python/pdstools/ih/legacy_IH.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.4/python/pdstools/pega_io/API.py` & `pdstools-3.1.5/python/pdstools/pega_io/API.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.4/python/pdstools/pega_io/File.py` & `pdstools-3.1.5/python/pdstools/pega_io/File.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.4/python/pdstools/pega_io/S3.py` & `pdstools-3.1.5/python/pdstools/pega_io/S3.py`

 * *Files 23% similar despite different names*

```diff
@@ -22,71 +22,139 @@
         temp_dir: str, default = './s3_download'
             The directory to download the s3 files to before reading them
         """
 
         self.bucketName = bucketName
         self.temp_dir = temp_dir
 
-    async def getS3Files(self, prefix, verbose=True):
+    async def getS3Files(self, prefix, use_meta_files=False, verbose=True):
         """OOTB file exports can be written in many very small files.
 
         This method asyncronously retrieves these files, and puts them in
         a temporary directory.
 
-        parameters
+        The logic, if `use_meta_files` is True, is:
+
+        1. Take the prefix, add a `.` in front of it
+        (`'path/to/files'` becomes (`'path/to/.files'`)
+
+        * rsplit on `/` (`['path/to', 'files']`)
+
+        * take the last element (`'files'`)
+
+        * add `.` in front of it (`'.files'`)
+
+        * concat back to a filepath  (`'path/to/.files'`)
+
+        3. fetch all files in the repo that adhere to the prefix (`'path/to/.files*'`)
+
+        4. For each file, if the file ends with `.meta`:
+
+        * rsplit on '/' (`['path/to', '.files_001.json.meta']`)
+
+        * for the last element (just the filename), strip the period and the .meta (`['path/to', 'files_001.json']`)
+
+        * concat back to a filepath (`'path/to/files_001.json'`)
+
+        5. Import all files in the list
+
+        If `use_meta_files` is False, the logic is as simple as:
+
+        1. Import all files starting with the prefix 
+        (`'path/to/files'` gives 
+        `['path/to/files_001.json', 'path/to/files_002.json', etc]`, 
+        irrespective of whether a `.meta` file exists).
+
+        Parameters
         ----------
         prefix: str
             The prefix, pointing to the s3 files. See boto3 docs for filter.
+        use_meta_files: bool, default=False
+            Whether to use the meta files to check for eligible files
+
+        Notes
+        -----
+        We don't import/copy over the .meta files at all.
+        There is an internal function, getNewFiles(), that checks if the filename
+        exists in the local file system. Since the meta files are not really useful for
+        local processing, there's no sense in copying them over. This logic also still
+        works with the use_meta_files - we first check which files are 'eligible' in S3
+        because they have a meta file, then we check if the 'real' files exist on disk.
+        If the file is already on disk, we don't copy it over.
 
         """
         import os
 
         def createPathIfNotExists(path):
             if not os.path.exists(path):
                 os.mkdir(path)
 
+        def localFile(file):
+            return f"{self.temp_dir}/{file}"
+
+        def getNewFiles(files):
+            newFiles, alreadyOnDisk = [], []
+            for file in files:
+                localFileName = localFile(file)
+                if os.path.exists(localFileName):
+                    alreadyOnDisk.append(file)
+                else:
+                    newFiles.append(file)
+            return newFiles, alreadyOnDisk
+
+        def createTask(file):
+            filename = f"{self.temp_dir}/{file}"
+            createPathIfNotExists(f"{self.temp_dir}/{file.rsplit('/')[:-1][0]}")
+            return asyncio.create_task(
+                s3.meta.client.download_file(self.bucketName, file, filename)
+            )
+
+        async def getfilesToImport(bucket, prefix, use_meta_files=False):
+            if use_meta_files:
+                to_import = []
+                prefix2 = "/.".join(prefix.rsplit("/", 1))
+                async for s3_object in bucket.objects.filter(Prefix=prefix2):
+                    f = s3_object.key
+                    if str(f).endswith(".meta"):
+                        to_import.append(
+                            "/".join(f.rsplit("/.", 1)).rsplit(".meta", 1)[0]
+                        )
+            else:
+                to_import = [
+                    s3_object.key
+                    async for s3_object in bucket.objects.filter(Prefix=prefix)
+                ]
+            return getNewFiles(to_import)
+
         createPathIfNotExists(self.temp_dir)
+
         session = aioboto3.Session()
         async with session.resource("s3") as s3:
-            tasks = []
-            files = []
-            alreadyOnDisk = []
             bucket = await s3.Bucket(self.bucketName)
-            async for s3_object in bucket.objects.filter(Prefix=prefix):
-                filename = f"{self.temp_dir}/{s3_object.key}"
-                files.append(filename)
-                if os.path.exists(filename):
-                    alreadyOnDisk.append(filename)
-                    continue
+            files, alreadyOnDisk = await getfilesToImport(
+                bucket, prefix, use_meta_files
+            )
 
-                createPathIfNotExists(
-                    f"{self.temp_dir}/{s3_object.key.rsplit('/')[:-1][0]}"
-                )
+            tasks = [createTask(f) for f in files]
 
-                tasks.append(
-                    asyncio.create_task(
-                        s3.meta.client.download_file(
-                            self.bucketName, s3_object.key, filename
-                        )
-                    )
-                )
             _ = [
                 await task_
                 for task_ in tqdm.as_completed(
                     tasks,
                     total=len(tasks),
                     desc="Downloading files...",
                     disable=not verbose,
                 )
             ]
+
         if verbose:
             print(
                 f"Completed {prefix}. Imported {len(files)} files, skipped {len(alreadyOnDisk)} files."
             )
-        return files
+        return list(map(localFile, [*files, *alreadyOnDisk]))
 
     async def getDatamartData(
         self, table, datamart_folder: str = "datamart", verbose: bool = True
     ):
         """Wrapper method to import one of the tables in the datamart.
 
         Parameters
```

### Comparing `pdstools-3.1.4/python/pdstools/plots/plot_base.py` & `pdstools-3.1.5/python/pdstools/plots/plot_base.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.4/python/pdstools/plots/plots_plotly.py` & `pdstools-3.1.5/python/pdstools/plots/plots_plotly.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.4/python/pdstools/reports/HealthCheck.qmd` & `pdstools-3.1.5/python/pdstools/reports/HealthCheck.qmd`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.4/python/pdstools/reports/HealthCheckModel.qmd` & `pdstools-3.1.5/python/pdstools/reports/HealthCheckModel.qmd`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.4/python/pdstools/utils/cdh_utils.py` & `pdstools-3.1.5/python/pdstools/utils/cdh_utils.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.4/python/pdstools/utils/datasets.py` & `pdstools-3.1.5/python/pdstools/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.4/python/pdstools/utils/hds_utils.py` & `pdstools-3.1.5/python/pdstools/utils/hds_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,18 @@
         The name of the outcome column
     positive_outcomes: list = ["Accepted", "Clicked"]
         Which positive outcomes to map to True
     negative_outcomes: list = ["Rejected", "Impression"]
         Which negative outcomes to map to False
     special_predictors: list = ["Decision_DecisionTime", "Decision_OutcomeTime"]
         A list of special predictors which are not touched
+    sample_percentage_schema_inferencing: float
+        The percentage of records to sample to infer the column type.
+        In case you're getting casting errors, it may be useful to 
+        increase this percentage to check a larger portion of data.
     """
 
     def __init__(
         self,
         config_file: Optional[str] = None,
         hds_folder: Path = ".",
         use_datamart: bool = False,
@@ -78,14 +82,15 @@
         mask_outcome_values: bool = True,
         context_key_label: str = "Context_*",
         ih_label: str = "IH_*",
         outcome_column: str = "Decision_Outcome",
         positive_outcomes: list = ["Accepted", "Clicked"],
         negative_outcomes: list = ["Rejected", "Impression"],
         special_predictors: list = ["Decision_DecisionTime", "Decision_OutcomeTime"],
+        sample_percentage_schema_inferencing:float=0.01,
     ):
         self._opts = {key: value for key, value in vars().items() if key != "self"}
 
         if config_file is not None:
             self.load_from_config_file(config_file)
         for key, value in self._opts.items():
             setattr(self, key, value)
@@ -223,16 +228,15 @@
         out = []
         for file in files:
             out.append(pl.scan_ndjson(file))
 
         df = pl.concat(out, how="diagonal")
         return df
 
-    @staticmethod
-    def read_predictor_type_from_file(df: pl.LazyFrame):
+    def read_predictor_type_from_file(self, df: pl.LazyFrame):
         """Infer the types of the preditors from the data.
 
         This is non-trivial, as it's not ideal to pull in all data to memory for this.
         For this reason, we sample 1% of data, or all data if less than 50 rows,
         and try to cast it to numeric. If that fails, we set it to categorical,
         else we set it to numeric.
 
@@ -247,15 +251,17 @@
         """
         types = {}
 
         import numpy as np
 
         def sample_it(s: pl.Series) -> pl.Series:
             out = pl.Series(
-                values=np.random.binomial(1, 0.01, s.len()),
+                values=np.random.binomial(
+                    1, self.config.sample_percentage_schema_inferencing, s.len()
+                ),
                 dtype=pl.Boolean,
             )
             if out.len() < 50:
                 out = pl.Series(values=[True] * out.len(), dtype=pl.Boolean)
             return out
 
         df_ = (
@@ -264,15 +270,17 @@
             .filter(pl.col("_sample"))
             .drop("_sample")
             .collect()
         )
 
         for col in df_.columns:
             try:
-                df_.get_column(col).cast(pl.Float64)
+                df_.get_column(col).map_dict({"": None}, default=pl.first()).cast(
+                    pl.Float64
+                )
                 types[col] = "numeric"
             except:
                 types[col] = "symbolic"
 
         return types
 
     @staticmethod
@@ -391,15 +399,15 @@
 
         return symbolic_predictors_to_mask, numeric_predictors_to_mask, column_mapping
 
     def getHasher(
         self,
         cols,
         algorithm="xxhash",
-        seed: Union[Literal[0, "random"], int] = 0,
+        seed="random",
         seed_1=None,
         seed_2=None,
         seed_3=None,
     ):
         if algorithm == "xxhash":
             if seed == "random":
                 seed, seed_1, seed_2, seed_3 = (
@@ -412,15 +420,15 @@
             return pl.col(cols).hash(
                 seed=seed, seed_1=seed_1, seed_2=seed_2, seed_3=seed_3
             )
 
         else:
             return pl.col(cols).apply(algorithm)
 
-    def process(self, **kwargs):
+    def process(self, strategy="eager", **kwargs):
         """Anonymize the dataset."""
 
         def to_hash(cols, **kwargs):
             hasher = self.getHasher(cols, **kwargs)
             return (
                 pl.when(
                     (pl.col(cols).is_not_null())
@@ -438,25 +446,27 @@
 
         def to_boolean(col, positives):
             return (
                 pl.when(pl.col(col).is_in(positives)).then(True).otherwise(False)
             ).alias(col)
 
         df = self.df.with_columns(
-            pl.col(self.numeric_predictors_to_mask).cast(pl.Float64)
+            pl.col(self.numeric_predictors_to_mask)
+            .map_dict({"": None}, default=pl.first())
+            .cast(pl.Float64)
         ).with_columns(
             [
                 to_hash(
                     self.symbolic_predictors_to_mask,
                     **kwargs,
                 ),
                 to_normalize(self.numeric_predictors_to_mask),
             ]
         )
         if self.config.mask_outcome_values:
             df = df.with_columns(
                 to_boolean(self.config.outcome_column, self.config.positive_outcomes)
             )
-        df = (
-            df.select(self.column_mapping.keys()).rename(self.column_mapping)
-        ).collect()
+        df = df.select(self.column_mapping.keys()).rename(self.column_mapping)
+        if strategy == "eager":
+            return df.collect()
         return df
```

### Comparing `pdstools-3.1.4/python/pdstools/utils/pega_template.py` & `pdstools-3.1.5/python/pdstools/utils/pega_template.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.4/python/pdstools/utils/polars_ext.py` & `pdstools-3.1.5/python/pdstools/utils/polars_ext.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.4/python/pdstools/utils/show_versions.py` & `pdstools-3.1.5/python/pdstools/utils/show_versions.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.4/python/pdstools/utils/streamlit_utils.py` & `pdstools-3.1.5/python/pdstools/utils/streamlit_utils.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.4/python/pdstools/utils/table_definitions.py` & `pdstools-3.1.5/python/pdstools/utils/table_definitions.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.4/python/pdstools/valuefinder/ValueFinder.py` & `pdstools-3.1.5/python/pdstools/valuefinder/ValueFinder.py`

 * *Files identical despite different names*


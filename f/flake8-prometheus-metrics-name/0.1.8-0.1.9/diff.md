# Comparing `tmp/flake8-prometheus-metrics-name-0.1.8.tar.gz` & `tmp/flake8-prometheus-metrics-name-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-prometheus-metrics-name-0.1.8.tar", max compression
+gzip compressed data, was "flake8-prometheus-metrics-name-0.1.9.tar", max compression
```

## Comparing `flake8-prometheus-metrics-name-0.1.8.tar` & `flake8-prometheus-metrics-name-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2022-05-04 07:33:24.715520 flake8-prometheus-metrics-name-0.1.8/LICENSE
--rw-r--r--   0        0        0     1754 2022-05-04 07:33:24.715904 flake8-prometheus-metrics-name-0.1.8/README.md
--rw-r--r--   0        0        0        0 2022-05-04 07:33:24.716286 flake8-prometheus-metrics-name-0.1.8/flake8_prometheus_metrics_name/__init__.py
--rw-r--r--   0        0        0     3270 2022-05-04 07:37:29.557183 flake8-prometheus-metrics-name-0.1.8/flake8_prometheus_metrics_name/api.py
--rw-r--r--   0        0        0     1460 2022-05-04 07:33:24.717045 flake8-prometheus-metrics-name-0.1.8/flake8_prometheus_metrics_name/cheker.py
--rw-r--r--   0        0        0      912 2022-05-04 07:43:36.517776 flake8-prometheus-metrics-name-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2697 2022-05-04 07:43:48.427857 flake8-prometheus-metrics-name-0.1.8/setup.py
--rw-r--r--   0        0        0     2627 2022-05-04 07:43:48.428068 flake8-prometheus-metrics-name-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-05-04 07:33:24.715520 flake8-prometheus-metrics-name-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1754 2022-05-04 07:33:24.715904 flake8-prometheus-metrics-name-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2022-05-04 07:33:24.716286 flake8-prometheus-metrics-name-0.1.9/flake8_prometheus_metrics_name/__init__.py
+-rw-r--r--   0        0        0     3270 2022-05-05 06:14:27.159867 flake8-prometheus-metrics-name-0.1.9/flake8_prometheus_metrics_name/api.py
+-rw-r--r--   0        0        0     1577 2022-05-05 06:13:52.215892 flake8-prometheus-metrics-name-0.1.9/flake8_prometheus_metrics_name/cheker.py
+-rw-r--r--   0        0        0      912 2022-05-05 06:14:27.150294 flake8-prometheus-metrics-name-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2697 2022-05-05 06:15:04.177788 flake8-prometheus-metrics-name-0.1.9/setup.py
+-rw-r--r--   0        0        0     2576 2022-05-05 06:15:04.178016 flake8-prometheus-metrics-name-0.1.9/PKG-INFO
```

### Comparing `flake8-prometheus-metrics-name-0.1.8/LICENSE` & `flake8-prometheus-metrics-name-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-prometheus-metrics-name-0.1.8/README.md` & `flake8-prometheus-metrics-name-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `flake8-prometheus-metrics-name-0.1.8/flake8_prometheus_metrics_name/api.py` & `flake8-prometheus-metrics-name-0.1.9/flake8_prometheus_metrics_name/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from prometheus_client.metrics import MetricWrapperBase
 
 from flake8_prometheus_metrics_name.cheker import (
     MetricNameValidatioError,
     validate_statement,
 )
 
-__version__ = '0.1.8'
+__version__ = '0.1.9'
 
 
 class Api:
     name = 'flake8-prometheus-metrics-name'
     version = __version__
 
     _error_template = (
```

### Comparing `flake8-prometheus-metrics-name-0.1.8/flake8_prometheus_metrics_name/cheker.py` & `flake8-prometheus-metrics-name-0.1.9/flake8_prometheus_metrics_name/cheker.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,17 +21,23 @@
     called = getattr(
         statement.func, 'id', getattr(statement.func, 'attr', None),
     )
     if called is None or called not in prometheus_mapping:
         return
     cls = prometheus_mapping[called]
 
-    args = [_parse_call_arguments(arg) for arg in statement.args]
+    args = [
+        _parse_call_arguments(arg)
+        for arg in statement.args
+        if not isinstance(arg, ast.Name)
+    ]
     kwargs = {
-        kw.arg: _parse_call_arguments(kw.value) for kw in statement.keywords
+        kw.arg: _parse_call_arguments(kw.value)
+        for kw in statement.keywords
+        if not isinstance(kw.value, ast.Name)
     }
     try:
         metric = cls(*args, **kwargs)
     except (ValueError, TypeError):
         return
 
     metric_name = metric._name  # pylint: disable=W0212
```

### Comparing `flake8-prometheus-metrics-name-0.1.8/pyproject.toml` & `flake8-prometheus-metrics-name-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flake8-prometheus-metrics-name"
-version = "0.1.8"
+version = "0.1.9"
 description = "Flake8 plugin for prometheus metric name validation"
 authors = ["perminovs"]
 license = "MIT"
 
 readme = 'README.md'
 repository = "https://github.com/perminovs/flake8_prometheus_metrics_name"
 keywords = ['flake8', 'linter', 'python', 'prometheus']
```

### Comparing `flake8-prometheus-metrics-name-0.1.8/setup.py` & `flake8-prometheus-metrics-name-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['flake8>=4.0.0,<5.0.0', 'prometheus_client>=0.7.1,<0.8.0']
 
 entry_points = \
 {'flake8.extension': ['PRM = flake8_prometheus_metrics_name.api:Api']}
 
 setup_kwargs = {
     'name': 'flake8-prometheus-metrics-name',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Flake8 plugin for prometheus metric name validation',
     'long_description': '# Flake8 prometheus metric name plugin\n\n\n[![pypi](https://badge.fury.io/py/flake8-prometheus-metrics-name.svg)](https://pypi.org/project/flake8-prometheus-metrics-name/)\n[![Python: 3.6+](https://img.shields.io/badge/Python-3.6+-blue.svg)](https://pypi.org/project/flake8-breakpoint)\n[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://en.wikipedia.org/wiki/MIT_License)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n\nFlake8 plugin to check metrics name prefix for official client https://github.com/prometheus/client_python.\n\n## Installation\n```bash\npip install flake8-prometheus-metrics-name\n```\n\n## Usage\nImagine we have python module `some_module.py`:\n```python\nfrom prometheus_client import Counter\n\nCounter(name=\'kek_values\', documentation=\'some doc\')\nCounter(name=\'some_name1\', documentation=\'some doc\')\nCounter(name=\'some_name2\', documentation=\'some doc\')  # noqa: PRM902\nCounter(name=\'some_name3\', documentation=\'some doc\')\nCounter(name=\'lol_values\', documentation=\'some doc\')\n```\n\nAdd valid metrics name prefixes to `setup.cfg`:\n```buildoutcfg\n[flake8]\nprometheus-metrics-name-prefixes =\n    kek_\n    lol_\n```\n\nRun flake8 `flake8 some_modue.py` cause following warnings:\n```bash\nsome_module.py:4:1: PRM902: Metric name should start with one of following prefixes: "kek_", "lol_", got "some_name1" instead\nsome_module.py:6:1: PRM902: Metric name should start with one of following prefixes: "kek_", "lol_", got "some_name3" instead\n```\n\nPlugin also may be disabled by adding following option to `setup.cfg`:\n```buildoutcfg\n[flake8]\nprometheus-metrics-disabled = 1\n```\nthen AST nodes will not be analized for metrics name on flake8 run.\n\n## License\nMIT\n',
     'author': 'perminovs',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/perminovs/flake8_prometheus_metrics_name',
```

### Comparing `flake8-prometheus-metrics-name-0.1.8/PKG-INFO` & `flake8-prometheus-metrics-name-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: flake8-prometheus-metrics-name
-Version: 0.1.8
+Version: 0.1.9
 Summary: Flake8 plugin for prometheus metric name validation
 Home-page: https://github.com/perminovs/flake8_prometheus_metrics_name
 License: MIT
 Keywords: flake8,linter,python,prometheus
 Author: perminovs
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: flake8 (>=4.0.0,<5.0.0)
 Requires-Dist: prometheus_client (>=0.7.1,<0.8.0)
 Project-URL: Repository, https://github.com/perminovs/flake8_prometheus_metrics_name
```


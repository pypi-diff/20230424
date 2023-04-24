# Comparing `tmp/chainsail-helpers-0.1.4.tar.gz` & `tmp/chainsail_helpers-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainsail-helpers-0.1.4.tar", max compression
+gzip compressed data, was "chainsail_helpers-0.1.5.tar", max compression
```

## Comparing `chainsail-helpers-0.1.4.tar` & `chainsail_helpers-0.1.5.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1420 2022-01-14 10:12:01.709061 chainsail-helpers-0.1.4/README.md
--rw-r--r--   0        0        0        0 2021-10-14 12:54:03.654877 chainsail-helpers-0.1.4/chainsail_helpers/__init__.py
--rw-r--r--   0        0        0     3370 2022-10-19 07:40:52.273307 chainsail-helpers-0.1.4/chainsail_helpers/pdf/__init__.py
--rw-r--r--   0        0        0     3306 2022-08-30 09:17:35.481680 chainsail-helpers-0.1.4/chainsail_helpers/pdf/pymc/__init__.py
--rw-r--r--   0        0        0     3096 2022-01-14 10:12:01.709061 chainsail-helpers-0.1.4/chainsail_helpers/pdf/stan/__init__.py
--rw-r--r--   0        0        0      537 2022-03-17 17:30:30.771890 chainsail-helpers-0.1.4/chainsail_helpers/scripts/README.md
--rw-r--r--   0        0        0        0 2022-01-14 10:12:01.709061 chainsail-helpers-0.1.4/chainsail_helpers/scripts/__init__.py
--rw-r--r--   0        0        0     1204 2022-03-17 17:30:30.772890 chainsail-helpers-0.1.4/chainsail_helpers/scripts/concatenate_samples.py
--rw-r--r--   0        0        0      962 2022-09-29 19:27:17.223165 chainsail-helpers-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2613 2022-10-19 13:09:37.760809 chainsail-helpers-0.1.4/setup.py
--rw-r--r--   0        0        0     2353 2022-10-19 13:09:37.761134 chainsail-helpers-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1420 2022-01-14 10:12:01.709061 chainsail_helpers-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2021-10-14 12:54:03.654877 chainsail_helpers-0.1.5/chainsail_helpers/__init__.py
+-rw-r--r--   0        0        0     3369 2022-12-16 13:02:30.021416 chainsail_helpers-0.1.5/chainsail_helpers/pdf/__init__.py
+-rw-r--r--   0        0        0     3306 2022-08-30 09:17:35.481680 chainsail_helpers-0.1.5/chainsail_helpers/pdf/pymc/__init__.py
+-rw-r--r--   0        0        0    10458 2022-12-20 12:48:07.934395 chainsail_helpers-0.1.5/chainsail_helpers/pdf/stan/#__init__.py#
+-rw-r--r--   0        0        0    10459 2023-04-24 09:11:48.417011 chainsail_helpers-0.1.5/chainsail_helpers/pdf/stan/__init__.py
+-rw-r--r--   0        0        0      537 2022-03-17 17:30:30.771890 chainsail_helpers-0.1.5/chainsail_helpers/scripts/README.md
+-rw-r--r--   0        0        0        0 2022-01-14 10:12:01.709061 chainsail_helpers-0.1.5/chainsail_helpers/scripts/__init__.py
+-rw-r--r--   0        0        0     1204 2022-12-18 16:33:10.898896 chainsail_helpers-0.1.5/chainsail_helpers/scripts/concatenate_samples.py
+-rw-r--r--   0        0        0      962 2023-04-24 09:11:48.417011 chainsail_helpers-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2617 1970-01-01 00:00:00.000000 chainsail_helpers-0.1.5/setup.py
+-rw-r--r--   0        0        0     2353 1970-01-01 00:00:00.000000 chainsail_helpers-0.1.5/PKG-INFO
```

### Comparing `chainsail-helpers-0.1.4/README.md` & `chainsail_helpers-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `chainsail-helpers-0.1.4/chainsail_helpers/pdf/__init__.py` & `chainsail_helpers-0.1.5/chainsail_helpers/pdf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             x(np.ndarray): 1D array of floats at which the log-probability
               gradient is evaluated
 
         Returns:
             np.ndarray: 1D array of floats containing the flattened
               log-probability gradient evaluated at x
         """
-        passs
+        pass
 
 
 class PosteriorPDF(PDF):
     """
     Interface for posterior probability densities consumed by Chainsail
     """
     @abstractmethod
```

### Comparing `chainsail-helpers-0.1.4/chainsail_helpers/pdf/pymc/__init__.py` & `chainsail_helpers-0.1.5/chainsail_helpers/pdf/pymc/__init__.py`

 * *Files identical despite different names*

### Comparing `chainsail-helpers-0.1.4/chainsail_helpers/scripts/README.md` & `chainsail_helpers-0.1.5/chainsail_helpers/scripts/README.md`

 * *Files identical despite different names*

### Comparing `chainsail-helpers-0.1.4/chainsail_helpers/scripts/concatenate_samples.py` & `chainsail_helpers-0.1.5/chainsail_helpers/scripts/concatenate_samples.py`

 * *Files identical despite different names*

### Comparing `chainsail-helpers-0.1.4/pyproject.toml` & `chainsail_helpers-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chainsail-helpers"
-version = "0.1.4"
+version = "0.1.5"
 description = "Probability distribution interfaces, examples, and utilities for the Chainsail sampling service"
 authors = ["Simeon Carstens <simeon.carstens@tweag.io>"]
 license = "MIT"
 readme = 'README.md'
 repository = 'https://github.com/tweag/chainsail-resources'
 homepage = 'https://github.com/tweag/chainsail-resources'
 keywords = ['probabilistic programming', 'sampling', 'MCMC']
```

### Comparing `chainsail-helpers-0.1.4/setup.py` & `chainsail_helpers-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,21 +19,21 @@
 
 entry_points = \
 {'console_scripts': ['concatenate-samples = '
                      'chainsail_helpers.scripts.concatenate_samples:main']}
 
 setup_kwargs = {
     'name': 'chainsail-helpers',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': 'Probability distribution interfaces, examples, and utilities for the Chainsail sampling service',
     'long_description': "# Chainsail PDF interfaces and utilities\n\nThis small package complements the [Chainsail](https://chainsail.io) sampling service. It\n- defines the general interface for objects representing Chainsail-consumable probability distributions,\n- provides implementations thereof for popular probabilistic programming languages,\n- and contains a few helper scripts for post-processing.\n\n## Installation\n```bash\n$ pip install chainsail-helpers\n```\nIf you'd like implement a probability density using [Stan](https://mc-stan.org) or [PyMC3](https://docs.pymc.io), install the corresponding extra dependencies like so: `poetry install --extras pymc3` and similarly for `stan`. \nWhen using Chainsail, this package will be automatically installed, so no need to add it to the list of dependencies in the job submission form.\nIf you like to develop this package, best use [Poetry](https://python-poetry.org):\n```bash\n$ poetry install\n$ poetry shell\n```\nand you will be dropped into a virtual environment with all dependencies installed.\n\n## Contributing\nContributions, for example PDF implementations for other probabilistic programming languages, are highly welcome!\nJust open a pull request and we'll be happy to work with you to make Chainsail even more useful.\n\n## License\n&copy; 2021 [Tweag](https://tweag.io). `chainsail_helpers` is open-source software and licensed under the [MIT license](https://opensource.org/licenses/MIT).\n",
     'author': 'Simeon Carstens',
     'author_email': 'simeon.carstens@tweag.io',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/tweag/chainsail-resources',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'entry_points': entry_points,
     'python_requires': '>=3.8,<3.11',
```

### Comparing `chainsail-helpers-0.1.4/PKG-INFO` & `chainsail_helpers-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: chainsail-helpers
-Version: 0.1.4
+Version: 0.1.5
 Summary: Probability distribution interfaces, examples, and utilities for the Chainsail sampling service
 Home-page: https://github.com/tweag/chainsail-resources
 License: MIT
 Keywords: probabilistic programming,sampling,MCMC
 Author: Simeon Carstens
 Author-email: simeon.carstens@tweag.io
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: pymc
 Provides-Extra: stan
 Requires-Dist: numpy (>=1.21.2,<2.0.0)
 Requires-Dist: pymc (>=4.1.4,<5.0.0); extra == "pymc"
 Requires-Dist: requests (>=2.26.0,<3.0.0); extra == "stan"
 Project-URL: Repository, https://github.com/tweag/chainsail-resources
 Description-Content-Type: text/markdown
```


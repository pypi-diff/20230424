# Comparing `tmp/pycsvy-0.2.1.tar.gz` & `tmp/pycsvy-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycsvy-0.2.1.tar", max compression
+gzip compressed data, was "pycsvy-0.2.2.tar", max compression
```

## Comparing `pycsvy-0.2.1.tar` & `pycsvy-0.2.2.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1531 2022-05-18 20:11:02.523059 pycsvy-0.2.1/LICENSE
--rw-r--r--   0        0        0     7194 2023-02-03 14:44:21.135178 pycsvy-0.2.1/README.md
--rw-r--r--   0        0        0      275 2023-02-10 06:37:54.993906 pycsvy-0.2.1/csvy/__init__.py
--rw-r--r--   0        0        0     6816 2023-02-03 14:44:21.137900 pycsvy-0.2.1/csvy/readers.py
--rw-r--r--   0        0        0     8308 2023-02-03 14:44:21.138692 pycsvy-0.2.1/csvy/writers.py
--rw-r--r--   0        0        0     1417 2023-02-10 06:37:54.992443 pycsvy-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     7924 1970-01-01 00:00:00.000000 pycsvy-0.2.1/setup.py
--rw-r--r--   0        0        0     8234 1970-01-01 00:00:00.000000 pycsvy-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1531 2022-05-18 20:11:02.523059 pycsvy-0.2.2/LICENSE
+-rw-r--r--   0        0        0     7194 2023-02-03 14:44:21.135178 pycsvy-0.2.2/README.md
+-rw-r--r--   0        0        0      275 2023-04-24 16:22:06.972014 pycsvy-0.2.2/csvy/__init__.py
+-rw-r--r--   0        0        0     6776 2023-04-24 16:18:25.657841 pycsvy-0.2.2/csvy/readers.py
+-rw-r--r--   0        0        0     8308 2023-02-03 14:44:21.138692 pycsvy-0.2.2/csvy/writers.py
+-rw-r--r--   0        0        0     1397 2023-04-24 16:22:06.971466 pycsvy-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     8234 1970-01-01 00:00:00.000000 pycsvy-0.2.2/PKG-INFO
```

### Comparing `pycsvy-0.2.1/LICENSE` & `pycsvy-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pycsvy-0.2.1/README.md` & `pycsvy-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pycsvy-0.2.1/csvy/readers.py` & `pycsvy-0.2.2/csvy/readers.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import yaml
 
 try:
     from numpy.typing import NDArray
 except ModuleNotFoundError:
-    NDArray = NotImplemented  # type: ignore
+    NDArray = None  # type: ignore
     logging.getLogger().debug(
         "Numpy is not installed. Reading into an array will not work."
     )
 
 try:
     from pandas import DataFrame
 except ModuleNotFoundError:
-    DataFrame = NotImplemented  # type: ignore
+    DataFrame = None  # type: ignore
     logging.getLogger().debug(
         "Pandas is not installed. Reading into a DataFrame will not work."
     )
 
 
 def get_comment(line: str, marker: str = "---") -> str:
     """Retrieves the comment character used in the header.
@@ -111,15 +111,15 @@
 
     Raises:
         ModuleNotFoundError: If numpy is not found.
 
     Returns:
         Tuple containing: The numpy array and the header as a dictionary.
     """
-    if NDArray is NotImplemented:
+    if NDArray is None:
         raise ModuleNotFoundError(
             "Module numpy is not present. Install it to read data into an array."
         )
     import numpy as np
 
     yaml_options = yaml_options if yaml_options is not None else {}
     header, nlines, comment = read_header(filename, marker=marker, **yaml_options)
@@ -149,15 +149,15 @@
 
     Raises:
         ModuleNotFoundError: If pandas is not found.
 
     Returns:
         Tuple containing: The pandas DataFrame and the header as a dictionary.
     """
-    if DataFrame is NotImplemented:
+    if DataFrame is None:
         raise ModuleNotFoundError(
             "Module pandas is not present. Install it to read data into DataFrame."
         )
     import pandas as pd
 
     yaml_options = yaml_options if yaml_options is not None else {}
     header, nlines, comment = read_header(filename, marker=marker, **yaml_options)
```

### Comparing `pycsvy-0.2.1/csvy/writers.py` & `pycsvy-0.2.2/csvy/writers.py`

 * *Files identical despite different names*

### Comparing `pycsvy-0.2.1/pyproject.toml` & `pycsvy-0.2.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycsvy"
-version = "0.2.1"
+version = "0.2.2"
 description = "Python reader/writer for CSV files with YAML header information."
 authors = ["Diego Alonso Álvarez <d.alonso-alvarez@imperial.ac.uk>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 repository = "https://github.com/ImperialCollegeLondon/pycsvy"
 classifiers = [
 	"Development Status :: 4 - Beta",
@@ -22,29 +22,28 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 PyYAML = "^6.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.0"
+pytest = "^7.2"
 pytest-cov = "^3.0.0"
 pytest-flake8 = "^1.1.1"
 pytest-mypy = "^0.9.1"
 pytest-mock = "^3.7.0"
 isort = "^5.10.1"
 pre-commit = "^2.18.1"
 black = "^22.3.0"
-numpy = "^1.22.3"
+numpy = "^1.24.2"
 pandas = "^1.4.1"
 flake8 = "^4.0.1"
 types-PyYAML = "^6.0.7"
-codecov = "^2.1.12"
-coverage = "^6.3.3"
 bump2version = "^1.0.1"
+coverage = "^7.1.0"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.4.1"
 mkdocstrings = {extras = ["python"], version = "^0.19.0"}
 mkdocs-material = "^8.5.7"
 mkdocs-gen-files = "^0.4.0"
 mkdocs-literate-nav = "^0.5.0"
```

### Comparing `pycsvy-0.2.1/setup.py` & `pycsvy-0.2.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,153 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pycsvy
+Version: 0.2.2
+Summary: Python reader/writer for CSV files with YAML header information.
+Home-page: https://github.com/ImperialCollegeLondon/pycsvy
+License: BSD-3-Clause
+Author: Diego Alonso Álvarez
+Author-email: d.alonso-alvarez@imperial.ac.uk
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: PyYAML (>=6.0,<7.0)
+Project-URL: Repository, https://github.com/ImperialCollegeLondon/pycsvy
+Description-Content-Type: text/markdown
+
+# CSVY for Python
+
+[![Test and build](https://github.com/ImperialCollegeLondon/csvy/actions/workflows/ci.yml/badge.svg)](https://github.com/ImperialCollegeLondon/csvy/actions/workflows/ci.yml)
+[![PyPI version shields.io](https://img.shields.io/pypi/v/pycsvy.svg)](https://pypi.python.org/pypi/pycsvy/)
+[![PyPI status](https://img.shields.io/pypi/status/pycsvy.svg)](https://pypi.python.org/pypi/pycsvy/)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/pycsvy.svg)](https://pypi.python.org/pypi/pycsvy/)
+[![PyPI license](https://img.shields.io/pypi/l/pycsvy.svg)](https://pypi.python.org/pypi/pycsvy/)
+[![codecov](https://codecov.io/gh/ImperialCollegeLondon/pycsvy/branch/develop/graph/badge.svg?token=N03KYNUD18)](https://codecov.io/gh/ImperialCollegeLondon/pycsvy)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/8d1b791b315f4814a128d94483499561)](https://www.codacy.com/gh/ImperialCollegeLondon/pycsvy/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=ImperialCollegeLondon/pycsvy&amp;utm_campaign=Badge_Grade)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/ImperialCollegeLondon/pycsvy/develop.svg)](https://results.pre-commit.ci/latest/github/ImperialCollegeLondon/pycsvy/develop)
+<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
+[![All Contributors](https://img.shields.io/badge/all_contributors-3-orange.svg?style=flat-square)](#contributors-)
+<!-- ALL-CONTRIBUTORS-BADGE:END -->
+
+CSV is a popular format for storing tabular data used in many disciplines. Metadata
+concerning the contents of the file is often included in the header, but it rarely
+follows a format that is machine readable - sometimes is not even human readable! In
+some cases, such information is provided in a separate file, which is not ideal as it is
+easy for data and metadata to get separated.
+
+CSVY is a small Python package to handle CSV files in which the metadata in the header
+is formatted in YAML. It supports reading/writing tabular data contained in numpy
+arrays, pandas DataFrames and nested lists, as well as metadata using a standard python
+dictionary. Ultimately, it aims to incorporate information about the [CSV
+dialect](https://specs.frictionlessdata.io/csv-dialect/) used and a [Table
+Schema](https://specs.frictionlessdata.io/table-schema/) specifying the contents of each
+column to aid the reading and interpretation of the data.
+
+## Instalation
+
+'pycsvy' is available in PyPI therefore its installation is as easy as:
+
+```bash
+pip install pycsvy
+```
+
+In order to support reading into `numpy` arrays or into `pandas` DataFrames, you will
+need to install those two packages, too.
+
+## Usage
+
+In the simplest case, to save some data contained in `data` and some metadata contained
+in a `metadata` dictionary into a CSVY file `important_data.csv` (the extension is not
+relevant), just do the following:
+
+```python
+import csvy
+
+csvy.write("important_data.csv", data, metadata)
+```
+
+The resulting file will have the YAML-formatted header in between `---` markers with,
+optionally, a comment character starting each header line. It could look something like
+the following:
+
+```text
+---
+name: my-dataset
+title: Example file of csvy
+description: Show a csvy sample file.
+encoding: utf-8
+schema:
+  fields:
+  - name: Date
+    type: object
+  - name: WTI
+    type: number
+---
+Date,WTI
+1986-01-02,25.56
+1986-01-03,26.00
+1986-01-06,26.53
+1986-01-07,25.85
+1986-01-08,25.87
+```
+
+For reading the information back:
+
+```python
+import csvy
+
+# To read into a numpy array
+data, metadata = csvy.read_to_array("important_data.csv")
+
+# To read into a pandas DataFrame
+data, metadata = csvy.read_to_dataframe("important_data.csv")
+```
+
+The appropriate writer/reader will be selected based on the type of `data`:
+
+- numpy array: `np.savetxt` and `np.loadtxt`
+- pandas DataFrame: `pd.DataFrame.to_csv` and `pd.read_csv`
+- nested lists:' `csv.writer` and `csv.reader`
+
+Options can be passed to the tabular data writer/reader by setting the `csv_options`
+dictionary. Likewise you can set the `yaml_options` dictionary with whatever options you
+want to pass to `yaml.safe_load` and `yaml.safe_dump` functions, reading/writing the
+YAML-formatted header, respectively.
+
+Finally, you can control the character(s) used to indicate comments by setting the
+`comment` keyword when writing a file. By default, there is no character (""). During reading, the comment character is found atomatically.
+
+## Contributors ✨
+
+Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
+
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+<table>
+  <tbody>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://www.imperial.ac.uk/admin-services/ict/self-service/research-support/rcs/research-software-engineering/"><img src="https://avatars.githubusercontent.com/u/6095790?v=4?s=100" width="100px;" alt="Diego Alonso Álvarez"/><br /><sub><b>Diego Alonso Álvarez</b></sub></a><br /><a href="#infra-dalonsoa" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#ideas-dalonsoa" title="Ideas, Planning, & Feedback">🤔</a> <a href="#maintenance-dalonsoa" title="Maintenance">🚧</a> <a href="https://github.com/ImperialCollegeLondon/pycsvy/commits?author=dalonsoa" title="Tests">⚠️</a> <a href="https://github.com/ImperialCollegeLondon/pycsvy/issues?q=author%3Adalonsoa" title="Bug reports">🐛</a> <a href="https://github.com/ImperialCollegeLondon/pycsvy/commits?author=dalonsoa" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://www.imperial.ac.uk/research-software-engineering"><img src="https://avatars.githubusercontent.com/u/23149834?v=4?s=100" width="100px;" alt="Alex Dewar"/><br /><sub><b>Alex Dewar</b></sub></a><br /><a href="#ideas-alexdewar" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/ImperialCollegeLondon/pycsvy/commits?author=alexdewar" title="Tests">⚠️</a> <a href="https://github.com/ImperialCollegeLondon/pycsvy/commits?author=alexdewar" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/AdrianDAlessandro"><img src="https://avatars.githubusercontent.com/u/40875798?v=4?s=100" width="100px;" alt="Adrian D'Alessandro"/><br /><sub><b>Adrian D'Alessandro</b></sub></a><br /><a href="https://github.com/ImperialCollegeLondon/pycsvy/issues?q=author%3AAdrianDAlessandro" title="Bug reports">🐛</a> <a href="https://github.com/ImperialCollegeLondon/pycsvy/commits?author=AdrianDAlessandro" title="Code">💻</a> <a href="https://github.com/ImperialCollegeLondon/pycsvy/commits?author=AdrianDAlessandro" title="Documentation">📖</a></td>
+    </tr>
+  </tbody>
+</table>
 
-packages = \
-['csvy']
+<!-- markdownlint-restore -->
+<!-- prettier-ignore-end -->
 
-package_data = \
-{'': ['*']}
+<!-- ALL-CONTRIBUTORS-LIST:END -->
 
-install_requires = \
-['PyYAML>=6.0,<7.0']
-
-setup_kwargs = {
-    'name': 'pycsvy',
-    'version': '0.2.1',
-    'description': 'Python reader/writer for CSV files with YAML header information.',
-    'long_description': '# CSVY for Python\n\n[![Test and build](https://github.com/ImperialCollegeLondon/csvy/actions/workflows/ci.yml/badge.svg)](https://github.com/ImperialCollegeLondon/csvy/actions/workflows/ci.yml)\n[![PyPI version shields.io](https://img.shields.io/pypi/v/pycsvy.svg)](https://pypi.python.org/pypi/pycsvy/)\n[![PyPI status](https://img.shields.io/pypi/status/pycsvy.svg)](https://pypi.python.org/pypi/pycsvy/)\n[![PyPI pyversions](https://img.shields.io/pypi/pyversions/pycsvy.svg)](https://pypi.python.org/pypi/pycsvy/)\n[![PyPI license](https://img.shields.io/pypi/l/pycsvy.svg)](https://pypi.python.org/pypi/pycsvy/)\n[![codecov](https://codecov.io/gh/ImperialCollegeLondon/pycsvy/branch/develop/graph/badge.svg?token=N03KYNUD18)](https://codecov.io/gh/ImperialCollegeLondon/pycsvy)\n[![Codacy Badge](https://app.codacy.com/project/badge/Grade/8d1b791b315f4814a128d94483499561)](https://www.codacy.com/gh/ImperialCollegeLondon/pycsvy/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=ImperialCollegeLondon/pycsvy&amp;utm_campaign=Badge_Grade)\n[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/ImperialCollegeLondon/pycsvy/develop.svg)](https://results.pre-commit.ci/latest/github/ImperialCollegeLondon/pycsvy/develop)\n<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->\n[![All Contributors](https://img.shields.io/badge/all_contributors-3-orange.svg?style=flat-square)](#contributors-)\n<!-- ALL-CONTRIBUTORS-BADGE:END -->\n\nCSV is a popular format for storing tabular data used in many disciplines. Metadata\nconcerning the contents of the file is often included in the header, but it rarely\nfollows a format that is machine readable - sometimes is not even human readable! In\nsome cases, such information is provided in a separate file, which is not ideal as it is\neasy for data and metadata to get separated.\n\nCSVY is a small Python package to handle CSV files in which the metadata in the header\nis formatted in YAML. It supports reading/writing tabular data contained in numpy\narrays, pandas DataFrames and nested lists, as well as metadata using a standard python\ndictionary. Ultimately, it aims to incorporate information about the [CSV\ndialect](https://specs.frictionlessdata.io/csv-dialect/) used and a [Table\nSchema](https://specs.frictionlessdata.io/table-schema/) specifying the contents of each\ncolumn to aid the reading and interpretation of the data.\n\n## Instalation\n\n\'pycsvy\' is available in PyPI therefore its installation is as easy as:\n\n```bash\npip install pycsvy\n```\n\nIn order to support reading into `numpy` arrays or into `pandas` DataFrames, you will\nneed to install those two packages, too.\n\n## Usage\n\nIn the simplest case, to save some data contained in `data` and some metadata contained\nin a `metadata` dictionary into a CSVY file `important_data.csv` (the extension is not\nrelevant), just do the following:\n\n```python\nimport csvy\n\ncsvy.write("important_data.csv", data, metadata)\n```\n\nThe resulting file will have the YAML-formatted header in between `---` markers with,\noptionally, a comment character starting each header line. It could look something like\nthe following:\n\n```text\n---\nname: my-dataset\ntitle: Example file of csvy\ndescription: Show a csvy sample file.\nencoding: utf-8\nschema:\n  fields:\n  - name: Date\n    type: object\n  - name: WTI\n    type: number\n---\nDate,WTI\n1986-01-02,25.56\n1986-01-03,26.00\n1986-01-06,26.53\n1986-01-07,25.85\n1986-01-08,25.87\n```\n\nFor reading the information back:\n\n```python\nimport csvy\n\n# To read into a numpy array\ndata, metadata = csvy.read_to_array("important_data.csv")\n\n# To read into a pandas DataFrame\ndata, metadata = csvy.read_to_dataframe("important_data.csv")\n```\n\nThe appropriate writer/reader will be selected based on the type of `data`:\n\n- numpy array: `np.savetxt` and `np.loadtxt`\n- pandas DataFrame: `pd.DataFrame.to_csv` and `pd.read_csv`\n- nested lists:\' `csv.writer` and `csv.reader`\n\nOptions can be passed to the tabular data writer/reader by setting the `csv_options`\ndictionary. Likewise you can set the `yaml_options` dictionary with whatever options you\nwant to pass to `yaml.safe_load` and `yaml.safe_dump` functions, reading/writing the\nYAML-formatted header, respectively.\n\nFinally, you can control the character(s) used to indicate comments by setting the\n`comment` keyword when writing a file. By default, there is no character (""). During reading, the comment character is found atomatically.\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n<table>\n  <tbody>\n    <tr>\n      <td align="center" valign="top" width="14.28%"><a href="https://www.imperial.ac.uk/admin-services/ict/self-service/research-support/rcs/research-software-engineering/"><img src="https://avatars.githubusercontent.com/u/6095790?v=4?s=100" width="100px;" alt="Diego Alonso Álvarez"/><br /><sub><b>Diego Alonso Álvarez</b></sub></a><br /><a href="#infra-dalonsoa" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#ideas-dalonsoa" title="Ideas, Planning, & Feedback">🤔</a> <a href="#maintenance-dalonsoa" title="Maintenance">🚧</a> <a href="https://github.com/ImperialCollegeLondon/pycsvy/commits?author=dalonsoa" title="Tests">⚠️</a> <a href="https://github.com/ImperialCollegeLondon/pycsvy/issues?q=author%3Adalonsoa" title="Bug reports">🐛</a> <a href="https://github.com/ImperialCollegeLondon/pycsvy/commits?author=dalonsoa" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://www.imperial.ac.uk/research-software-engineering"><img src="https://avatars.githubusercontent.com/u/23149834?v=4?s=100" width="100px;" alt="Alex Dewar"/><br /><sub><b>Alex Dewar</b></sub></a><br /><a href="#ideas-alexdewar" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/ImperialCollegeLondon/pycsvy/commits?author=alexdewar" title="Tests">⚠️</a> <a href="https://github.com/ImperialCollegeLondon/pycsvy/commits?author=alexdewar" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/AdrianDAlessandro"><img src="https://avatars.githubusercontent.com/u/40875798?v=4?s=100" width="100px;" alt="Adrian D\'Alessandro"/><br /><sub><b>Adrian D\'Alessandro</b></sub></a><br /><a href="https://github.com/ImperialCollegeLondon/pycsvy/issues?q=author%3AAdrianDAlessandro" title="Bug reports">🐛</a> <a href="https://github.com/ImperialCollegeLondon/pycsvy/commits?author=AdrianDAlessandro" title="Code">💻</a> <a href="https://github.com/ImperialCollegeLondon/pycsvy/commits?author=AdrianDAlessandro" title="Documentation">📖</a></td>\n    </tr>\n  </tbody>\n</table>\n\n<!-- markdownlint-restore -->\n<!-- prettier-ignore-end -->\n\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n',
-    'author': 'Diego Alonso Álvarez',
-    'author_email': 'd.alonso-alvarez@imperial.ac.uk',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/ImperialCollegeLondon/pycsvy',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
 
-
-setup(**setup_kwargs)
```


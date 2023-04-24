# Comparing `tmp/flake8_bas-0.1.2.tar.gz` & `tmp/flake8_bas-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_bas-0.1.2.tar", max compression
+gzip compressed data, was "flake8_bas-0.2.0.tar", max compression
```

## Comparing `flake8_bas-0.1.2.tar` & `flake8_bas-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2023-01-26 12:38:25.850546 flake8_bas-0.1.2/LICENSE
--rw-r--r--   0        0        0     6896 2023-01-26 12:38:25.850546 flake8_bas-0.1.2/README.md
--rw-r--r--   0        0        0       71 2023-01-26 12:38:25.850546 flake8_bas-0.1.2/flake8_bas/__init__.py
--rw-r--r--   0        0        0    13128 2023-01-26 12:38:25.850546 flake8_bas-0.1.2/flake8_bas/checker.py
--rw-r--r--   0        0        0     1817 2023-01-26 12:38:49.378742 flake8_bas-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     7913 1970-01-01 00:00:00.000000 flake8_bas-0.1.2/setup.py
--rw-r--r--   0        0        0     8325 1970-01-01 00:00:00.000000 flake8_bas-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-24 16:46:27.573609 flake8_bas-0.2.0/LICENSE
+-rw-r--r--   0        0        0     6892 2023-04-24 16:46:27.573609 flake8_bas-0.2.0/README.md
+-rw-r--r--   0        0        0       71 2023-04-24 16:46:27.573609 flake8_bas-0.2.0/flake8_bas/__init__.py
+-rw-r--r--   0        0        0    13128 2023-04-24 16:46:27.573609 flake8_bas-0.2.0/flake8_bas/checker.py
+-rw-r--r--   0        0        0     2020 2023-04-24 16:46:27.577610 flake8_bas-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7914 1970-01-01 00:00:00.000000 flake8_bas-0.2.0/setup.py
+-rw-r--r--   0        0        0     8276 1970-01-01 00:00:00.000000 flake8_bas-0.2.0/PKG-INFO
```

### Comparing `flake8_bas-0.1.2/LICENSE` & `flake8_bas-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8_bas-0.1.2/README.md` & `flake8_bas-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -31,30 +31,30 @@
 
 This Flake8 plugin therefore checks for a blank line before/after each statement as long as it's **not the first/last
 line of code within a module** and **not the first/last statement within a compound statement**.
 
 
 ## Requirements
 
-* Python >= 3.8
+* Python >= 3.8.1
 * Flake8 >= 3.8.0
 
 
 ## Installation
 
 ### Pip
 
 ```bash
 pip install flake8-bas
 ```
 
 ### Poetry
 
 ```bash
-poetry add --dev flake8-bas
+poetry add flake8-bas
 ```
 
 
 ## Use in production
 
 Until version 1.0.0 is reached, this plugin is considered to be **NOT ready for production**.
```

### Comparing `flake8_bas-0.1.2/flake8_bas/checker.py` & `flake8_bas-0.2.0/flake8_bas/checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import ast
 import re
 from contextlib import suppress
-from dataclasses import dataclass, astuple
-from typing import Generator, List, Optional, NamedTuple, Tuple
+from dataclasses import astuple, dataclass
+from typing import Generator, List, NamedTuple, Optional, Tuple
 
 with suppress(Exception):
     import pkg_resources
 
 
 @dataclass(init=False, frozen=True)
 class StatementErrorCodes:
```

### Comparing `flake8_bas-0.1.2/pyproject.toml` & `flake8_bas-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flake8-bas"
-version = "0.1.2"
+version = "0.2.0"
 description = "Flake8 extension that checks for blank lines around (compound) statements."
 authors = ["Tomas Mrozek <tm@nohup.run>"]
 maintainers = ["Tomas Mrozek <tm@nohup.run>"]
 repository = "https://github.com/ts-mk/flake8-bas/"
 documentation = "https://github.com/ts-mk/flake8-bas/blob/master/README.md"
 readme = "README.md"
 license = "MIT"
@@ -19,21 +19,22 @@
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8"
+python = ">=3.8.1,<4"
 flake8 = ">=3.8.0"
 setuptools = "*"
 
 [tool.poetry.group.dev.dependencies]
-black = "22.12.0"
-pre-commit = ">=2.10.0,<3.0"
+black = "23.3.0"
+isort = ">=5.12.0,<6.0.0"
+pre-commit = ">=3.1.0,<4.0.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = ">=7.0.0,<8.0.0"
 pytest-cov = ">=3.0.0,<4.0.0"
 
 [tool.poetry.group.ci.dependencies]
 click = ">=8.1.0,<9.0.0"
@@ -42,16 +43,17 @@
 BAS = "flake8_bas:StatementChecker"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
-skip-numeric-underscore-normalization = true
 force-exclude = ".*tests/fixtures/.*"
+line-length = 88
+skip-numeric-underscore-normalization = true
 
 [tool.interrogate]
 color = true
 exclude = ["tests", ".local"]
 fail-under = 100
 ignore-init-method = true
 ignore-init-module = true
@@ -59,7 +61,14 @@
 ignore-module = true
 ignore-nested-functions = true
 ignore-private = false
 ignore-property-decorators = true
 ignore-semiprivate = false
 quiet = false
 verbose = 2
+
+[tool.isort]
+extend_skip_glob = [".local/*", "tests/fixtures/*"]
+filter_files = true
+line_length = 88
+no_lines_before = ["LOCALFOLDER"]
+profile = "black"
```

### Comparing `flake8_bas-0.1.2/setup.py` & `flake8_bas-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 ['flake8>=3.8.0', 'setuptools']
 
 entry_points = \
 {'flake8.extension': ['BAS = flake8_bas:StatementChecker']}
 
 setup_kwargs = {
     'name': 'flake8-bas',
-    'version': '0.1.2',
+    'version': '0.2.0',
     'description': 'Flake8 extension that checks for blank lines around (compound) statements.',
-    'long_description': '# Flake8 - check for blank lines around statements\n\n![Python](https://img.shields.io/badge/Python-3.8+-blue?logo=python&logoColor=white)\n![PyPI](https://img.shields.io/pypi/v/flake8-bas.svg?label=PyPI&logo=PyPI&logoColor=white)\n![License](https://img.shields.io/badge/License-MIT-blue?logo=opensourceinitiative&logoColor=white)\n![codecov](https://codecov.io/gh/ts-mk/flake8-bas/branch/master/graph/badge.svg?token=PI2I083V09)\n![CI](https://github.com/ts-mk/flake8-bas/actions/workflows/tests.yml/badge.svg)\n\n[PEP 8](https://peps.python.org/pep-0008/) recommends to use blank lines only to separate logical sections:\n\n> Extra blank lines may be used (sparingly) to separate groups of related functions. Blank lines may be omitted between\n> a bunch of related one-liners (e.g. a set of dummy implementations).\n>\n> Use blank lines in functions, sparingly, to indicate logical sections.\n\nHowever, adding blank lines before and after compound statements (e.g.\xa0`if/else` block) as well as some simple\nstatements (e.g.\xa0`return`) might improve code readability which is otherwise hindered despite syntax highlighting\nthat modern code editors provide, as demonstrated in the following example:\n\n```python\nif 1 == 1:\n    print(1)\nfor n in [2, 3]:\n    print(n)\nelse:\n    print(4)\n```\n\n...where it might not be immediately apparent that this is not one `if/else` statement but an `if` statement followed by\na `for/else` statement.\n\nThis Flake8 plugin therefore checks for a blank line before/after each statement as long as it\'s **not the first/last\nline of code within a module** and **not the first/last statement within a compound statement**.\n\n\n## Requirements\n\n* Python >= 3.8\n* Flake8 >= 3.8.0\n\n\n## Installation\n\n### Pip\n\n```bash\npip install flake8-bas\n```\n\n### Poetry\n\n```bash\npoetry add --dev flake8-bas\n```\n\n\n## Use in production\n\nUntil version 1.0.0 is reached, this plugin is considered to be **NOT ready for production**.\n\n\n## Statements and their error codes\n\nThe statements are split into different categories based on whether they are\n[simple statements](https://docs.python.org/3.11/reference/simple_stmts.html) or\n[compound statements](https://docs.python.org/3.11/reference/compound_stmts.html), and whether the error occurs between\ntwo statements of the same type or not. This allows you to filter entire groups using `BAS` and the first digit,\ne.g.\xa0`BAS2`.\n\n**Error types:**\n\n* *Before Error* - missing line before a statement as long as the preceding element is not a statement of the same type.\n* *After Error* - missing line after a statement as long as the element that follows is not a statement of the same\n                  type.\n* *Sibling Error* - missing line between two or more consecutive statements of the same type.\n\n### BAS1xx/BAS2xx/BAS3xx: Simple statements\n\nSimple statements, excluding\n[expressions](https://docs.python.org/3.11/reference/simple_stmts.html#expression-statements) and\n[assignments](https://docs.python.org/3.11/reference/simple_stmts.html#assignment-statements), which are technically\nstatements as well.\n\n| Statement         | Before Error | After Error | Sibling Error |\n|:------------------|:-------------|:------------|:--------------|\n| `assert`          | BAS101       | BAS201      | BAS301        |\n| `break`           | BAS102       | BAS202      | BAS302        |\n| `continue`        | BAS103       | BAS203      | BAS303        |\n| `del`             | BAS104       | BAS204      | BAS304        |\n| `global`          | BAS105       | BAS205      | BAS305        |\n| `import`          | BAS106       | BAS206      | BAS306        |\n| `from import`     | BAS107       | BAS207      | BAS307        |\n| `nonlocal`        | BAS108       | BAS208      | BAS308        |\n| `pass`            | BAS109       | BAS209      | BAS309        |\n| `raise`           | BAS110       | BAS210      | BAS310        |\n| `return`          | BAS111       | BAS211      | BAS311        |\n| `yield`           | BAS112       | BAS212      | BAS312        |\n| `yield from`      | BAS113       | BAS213      | BAS313        |\n\n**Note:** Some of these errors shouldn\'t occur (e.g.\xa0`return` followed by another `return`) because having\nconsecutive siblings of those types does not make sense, but the plugin would raise these errors anyway.\n\n### BAS5xx/BAS6xx/BAS7xx: Compound statements\n\n| Statement    | Before Error | After Error | Sibling Error |\n|:-------------|:-------------|:------------|:--------------|\n| `class`      | BAS501       | BAS601      | BAS701        |\n| `def`        | BAS502       | BAS602      | BAS702        |\n| `async def`  | BAS503       | BAS603      | BAS703        |\n| `for`        | BAS504       | BAS604      | BAS704        |\n| `async for`  | BAS505       | BAS605      | BAS705        |\n| `if`         | BAS506       | BAS606      | BAS706        |\n| `match`      | BAS507       | BAS607      | BAS707        |\n| `try`        | BAS508       | BAS608      | BAS708        |\n| `while`      | BAS509       | BAS609      | BAS709        |\n| `with`       | BAS510       | BAS610      | BAS710        |\n| `async with` | BAS511       | BAS611      | BAS711        |\n\n\n## Overlapping errors\n\nThe extension produces overlapping errors, that is **two statements of different types** following each other would\nproduce one "before" error and one "after" error pointing to the same line of code:\n\n```python\na = 1\n\nglobal a\ndel a\n```\n\nThis would result in two errors for line 4:\n\n```text\n./file.py:4:1: BAS205 missing blank line after "global" statement\n./file.py:4:1: BAS104 missing blank line before "del" statement\n```\n\nHowever, two statements of the same type would produce only one "sibling" error.\n\n## Configuration\n\nThe plugin checks for blank lines around **every statement**. There are no custom configuration options. Instead, you\ncould simply ignore some errors. This system has benefits as well as drawbacks.\n\nThe benefit is that you could take advantage of Flake8\'s `ignore` and `per-file-ignores` (flake8\xa0>=\xa03.7.0) config\noptions and have a different behaviour for a different set of files:\n\n```ini\n[flake8]\nignore = BAS3\nper-file-ignores =\n    app/*: BAS10, BAS110, BAS20, BAS210\n    tests/*: BAS1, BAS2\n```\n\nThe drawback is that there are no sane defaults and you would inevitably need to exclude some errors, either because\nthey are undesirable, make little sense, or the same/conflicting checks might already be applied by another plugin\n(e.g.\xa0checks by [flake8-import-order](https://github.com/PyCQA/flake8-import-order)) or should be handled by other\n(formatting) tools (e.g. [black](https://github.com/psf/black)).\n\n### Recommended exclusions\n\nOnly compound statements plus `return` and `yield` would raise errors.\n\n```ini\n[flake8]\nignore = BAS10, BAS110, BAS20, BAS210, BAS30, BAS310\n```\n\n### All simple statements excluded\n\nOnly compound statements would raise errors.\n\n```ini\n[flake8]\nignore = BAS1, BAS2, BAS3\n```\n',
+    'long_description': '# Flake8 - check for blank lines around statements\n\n![Python](https://img.shields.io/badge/Python-3.8+-blue?logo=python&logoColor=white)\n![PyPI](https://img.shields.io/pypi/v/flake8-bas.svg?label=PyPI&logo=PyPI&logoColor=white)\n![License](https://img.shields.io/badge/License-MIT-blue?logo=opensourceinitiative&logoColor=white)\n![codecov](https://codecov.io/gh/ts-mk/flake8-bas/branch/master/graph/badge.svg?token=PI2I083V09)\n![CI](https://github.com/ts-mk/flake8-bas/actions/workflows/tests.yml/badge.svg)\n\n[PEP 8](https://peps.python.org/pep-0008/) recommends to use blank lines only to separate logical sections:\n\n> Extra blank lines may be used (sparingly) to separate groups of related functions. Blank lines may be omitted between\n> a bunch of related one-liners (e.g. a set of dummy implementations).\n>\n> Use blank lines in functions, sparingly, to indicate logical sections.\n\nHowever, adding blank lines before and after compound statements (e.g.\xa0`if/else` block) as well as some simple\nstatements (e.g.\xa0`return`) might improve code readability which is otherwise hindered despite syntax highlighting\nthat modern code editors provide, as demonstrated in the following example:\n\n```python\nif 1 == 1:\n    print(1)\nfor n in [2, 3]:\n    print(n)\nelse:\n    print(4)\n```\n\n...where it might not be immediately apparent that this is not one `if/else` statement but an `if` statement followed by\na `for/else` statement.\n\nThis Flake8 plugin therefore checks for a blank line before/after each statement as long as it\'s **not the first/last\nline of code within a module** and **not the first/last statement within a compound statement**.\n\n\n## Requirements\n\n* Python >= 3.8.1\n* Flake8 >= 3.8.0\n\n\n## Installation\n\n### Pip\n\n```bash\npip install flake8-bas\n```\n\n### Poetry\n\n```bash\npoetry add flake8-bas\n```\n\n\n## Use in production\n\nUntil version 1.0.0 is reached, this plugin is considered to be **NOT ready for production**.\n\n\n## Statements and their error codes\n\nThe statements are split into different categories based on whether they are\n[simple statements](https://docs.python.org/3.11/reference/simple_stmts.html) or\n[compound statements](https://docs.python.org/3.11/reference/compound_stmts.html), and whether the error occurs between\ntwo statements of the same type or not. This allows you to filter entire groups using `BAS` and the first digit,\ne.g.\xa0`BAS2`.\n\n**Error types:**\n\n* *Before Error* - missing line before a statement as long as the preceding element is not a statement of the same type.\n* *After Error* - missing line after a statement as long as the element that follows is not a statement of the same\n                  type.\n* *Sibling Error* - missing line between two or more consecutive statements of the same type.\n\n### BAS1xx/BAS2xx/BAS3xx: Simple statements\n\nSimple statements, excluding\n[expressions](https://docs.python.org/3.11/reference/simple_stmts.html#expression-statements) and\n[assignments](https://docs.python.org/3.11/reference/simple_stmts.html#assignment-statements), which are technically\nstatements as well.\n\n| Statement         | Before Error | After Error | Sibling Error |\n|:------------------|:-------------|:------------|:--------------|\n| `assert`          | BAS101       | BAS201      | BAS301        |\n| `break`           | BAS102       | BAS202      | BAS302        |\n| `continue`        | BAS103       | BAS203      | BAS303        |\n| `del`             | BAS104       | BAS204      | BAS304        |\n| `global`          | BAS105       | BAS205      | BAS305        |\n| `import`          | BAS106       | BAS206      | BAS306        |\n| `from import`     | BAS107       | BAS207      | BAS307        |\n| `nonlocal`        | BAS108       | BAS208      | BAS308        |\n| `pass`            | BAS109       | BAS209      | BAS309        |\n| `raise`           | BAS110       | BAS210      | BAS310        |\n| `return`          | BAS111       | BAS211      | BAS311        |\n| `yield`           | BAS112       | BAS212      | BAS312        |\n| `yield from`      | BAS113       | BAS213      | BAS313        |\n\n**Note:** Some of these errors shouldn\'t occur (e.g.\xa0`return` followed by another `return`) because having\nconsecutive siblings of those types does not make sense, but the plugin would raise these errors anyway.\n\n### BAS5xx/BAS6xx/BAS7xx: Compound statements\n\n| Statement    | Before Error | After Error | Sibling Error |\n|:-------------|:-------------|:------------|:--------------|\n| `class`      | BAS501       | BAS601      | BAS701        |\n| `def`        | BAS502       | BAS602      | BAS702        |\n| `async def`  | BAS503       | BAS603      | BAS703        |\n| `for`        | BAS504       | BAS604      | BAS704        |\n| `async for`  | BAS505       | BAS605      | BAS705        |\n| `if`         | BAS506       | BAS606      | BAS706        |\n| `match`      | BAS507       | BAS607      | BAS707        |\n| `try`        | BAS508       | BAS608      | BAS708        |\n| `while`      | BAS509       | BAS609      | BAS709        |\n| `with`       | BAS510       | BAS610      | BAS710        |\n| `async with` | BAS511       | BAS611      | BAS711        |\n\n\n## Overlapping errors\n\nThe extension produces overlapping errors, that is **two statements of different types** following each other would\nproduce one "before" error and one "after" error pointing to the same line of code:\n\n```python\na = 1\n\nglobal a\ndel a\n```\n\nThis would result in two errors for line 4:\n\n```text\n./file.py:4:1: BAS205 missing blank line after "global" statement\n./file.py:4:1: BAS104 missing blank line before "del" statement\n```\n\nHowever, two statements of the same type would produce only one "sibling" error.\n\n## Configuration\n\nThe plugin checks for blank lines around **every statement**. There are no custom configuration options. Instead, you\ncould simply ignore some errors. This system has benefits as well as drawbacks.\n\nThe benefit is that you could take advantage of Flake8\'s `ignore` and `per-file-ignores` (flake8\xa0>=\xa03.7.0) config\noptions and have a different behaviour for a different set of files:\n\n```ini\n[flake8]\nignore = BAS3\nper-file-ignores =\n    app/*: BAS10, BAS110, BAS20, BAS210\n    tests/*: BAS1, BAS2\n```\n\nThe drawback is that there are no sane defaults and you would inevitably need to exclude some errors, either because\nthey are undesirable, make little sense, or the same/conflicting checks might already be applied by another plugin\n(e.g.\xa0checks by [flake8-import-order](https://github.com/PyCQA/flake8-import-order)) or should be handled by other\n(formatting) tools (e.g. [black](https://github.com/psf/black)).\n\n### Recommended exclusions\n\nOnly compound statements plus `return` and `yield` would raise errors.\n\n```ini\n[flake8]\nignore = BAS10, BAS110, BAS20, BAS210, BAS30, BAS310\n```\n\n### All simple statements excluded\n\nOnly compound statements would raise errors.\n\n```ini\n[flake8]\nignore = BAS1, BAS2, BAS3\n```\n',
     'author': 'Tomas Mrozek',
     'author_email': 'tm@nohup.run',
     'maintainer': 'Tomas Mrozek',
     'maintainer_email': 'tm@nohup.run',
     'url': 'https://github.com/ts-mk/flake8-bas/',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.8',
+    'python_requires': '>=3.8.1,<4',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `flake8_bas-0.1.2/PKG-INFO` & `flake8_bas-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: flake8-bas
-Version: 0.1.2
+Version: 0.2.0
 Summary: Flake8 extension that checks for blank lines around (compound) statements.
 Home-page: https://github.com/ts-mk/flake8-bas/
 License: MIT
 Author: Tomas Mrozek
 Author-email: tm@nohup.run
 Maintainer: Tomas Mrozek
 Maintainer-email: tm@nohup.run
-Requires-Python: >=3.8
+Requires-Python: >=3.8.1,<4
 Classifier: Environment :: Console
 Classifier: Framework :: Flake8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -65,30 +64,30 @@
 
 This Flake8 plugin therefore checks for a blank line before/after each statement as long as it's **not the first/last
 line of code within a module** and **not the first/last statement within a compound statement**.
 
 
 ## Requirements
 
-* Python >= 3.8
+* Python >= 3.8.1
 * Flake8 >= 3.8.0
 
 
 ## Installation
 
 ### Pip
 
 ```bash
 pip install flake8-bas
 ```
 
 ### Poetry
 
 ```bash
-poetry add --dev flake8-bas
+poetry add flake8-bas
 ```
 
 
 ## Use in production
 
 Until version 1.0.0 is reached, this plugin is considered to be **NOT ready for production**.
```


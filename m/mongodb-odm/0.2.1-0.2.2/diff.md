# Comparing `tmp/mongodb_odm-0.2.1.tar.gz` & `tmp/mongodb_odm-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongodb_odm-0.2.1.tar", max compression
+gzip compressed data, was "mongodb_odm-0.2.2.tar", max compression
```

## Comparing `mongodb_odm-0.2.1.tar` & `mongodb_odm-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1056 2023-03-31 21:18:41.236449 mongodb_odm-0.2.1/LICENSE
--rw-r--r--   0        0        0     7214 2023-04-07 17:33:31.447106 mongodb_odm-0.2.1/README.md
--rw-r--r--   0        0        0      497 2023-03-31 21:18:41.240449 mongodb_odm-0.2.1/mongodb_odm/__init__.py
--rw-r--r--   0        0        0     1540 2023-04-07 17:33:31.451106 mongodb_odm-0.2.1/mongodb_odm/connection.py
--rw-r--r--   0        0        0     1230 2023-04-07 17:33:31.451106 mongodb_odm-0.2.1/mongodb_odm/data_conversion.py
--rw-r--r--   0        0        0       91 2023-03-31 21:18:41.240449 mongodb_odm-0.2.1/mongodb_odm/exceptions.py
--rw-r--r--   0        0        0     2824 2023-03-31 21:18:41.240449 mongodb_odm-0.2.1/mongodb_odm/fields.py
--rw-r--r--   0        0        0    14281 2023-04-07 17:33:31.451106 mongodb_odm-0.2.1/mongodb_odm/models.py
--rw-r--r--   0        0        0      577 2023-04-07 17:33:31.451106 mongodb_odm-0.2.1/mongodb_odm/types.py
--rw-r--r--   0        0        0        0 2023-03-31 21:18:41.240449 mongodb_odm-0.2.1/mongodb_odm/utils/__init__.py
--rw-r--r--   0        0        0      310 2023-04-07 17:33:31.451106 mongodb_odm-0.2.1/mongodb_odm/utils/_internal_models.py
--rw-r--r--   0        0        0     5453 2023-04-07 17:33:31.451106 mongodb_odm-0.2.1/mongodb_odm/utils/apply_indexes.py
--rw-r--r--   0        0        0     1566 2023-04-07 17:33:31.451106 mongodb_odm-0.2.1/mongodb_odm/utils/utils.py
--rw-r--r--   0        0        0     2619 2023-04-07 17:35:11.586345 mongodb_odm-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     8212 1970-01-01 00:00:00.000000 mongodb_odm-0.2.1/setup.py
--rw-r--r--   0        0        0     8869 1970-01-01 00:00:00.000000 mongodb_odm-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-03-31 21:18:41.236449 mongodb_odm-0.2.2/LICENSE
+-rw-r--r--   0        0        0     7214 2023-04-07 17:33:31.447106 mongodb_odm-0.2.2/README.md
+-rw-r--r--   0        0        0      897 2023-04-24 06:10:00.161951 mongodb_odm-0.2.2/mongodb_odm/__init__.py
+-rw-r--r--   0        0        0     1540 2023-04-07 17:33:31.451106 mongodb_odm-0.2.2/mongodb_odm/connection.py
+-rw-r--r--   0        0        0     1230 2023-04-07 17:33:31.451106 mongodb_odm-0.2.2/mongodb_odm/data_conversion.py
+-rw-r--r--   0        0        0       91 2023-03-31 21:18:41.240449 mongodb_odm-0.2.2/mongodb_odm/exceptions.py
+-rw-r--r--   0        0        0     2824 2023-03-31 21:18:41.240449 mongodb_odm-0.2.2/mongodb_odm/fields.py
+-rw-r--r--   0        0        0    14304 2023-04-24 06:10:00.165951 mongodb_odm-0.2.2/mongodb_odm/models.py
+-rw-r--r--   0        0        0        0 2023-04-24 06:10:00.165951 mongodb_odm-0.2.2/mongodb_odm/py.typed
+-rw-r--r--   0        0        0      577 2023-04-07 17:33:31.451106 mongodb_odm-0.2.2/mongodb_odm/types.py
+-rw-r--r--   0        0        0        0 2023-03-31 21:18:41.240449 mongodb_odm-0.2.2/mongodb_odm/utils/__init__.py
+-rw-r--r--   0        0        0      310 2023-04-07 17:33:31.451106 mongodb_odm-0.2.2/mongodb_odm/utils/_internal_models.py
+-rw-r--r--   0        0        0     5453 2023-04-07 17:33:31.451106 mongodb_odm-0.2.2/mongodb_odm/utils/apply_indexes.py
+-rw-r--r--   0        0        0     1566 2023-04-07 17:33:31.451106 mongodb_odm-0.2.2/mongodb_odm/utils/utils.py
+-rw-r--r--   0        0        0     2633 2023-04-24 06:10:47.633935 mongodb_odm-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     8212 1970-01-01 00:00:00.000000 mongodb_odm-0.2.2/setup.py
+-rw-r--r--   0        0        0     8869 1970-01-01 00:00:00.000000 mongodb_odm-0.2.2/PKG-INFO
```

### Comparing `mongodb_odm-0.2.1/LICENSE` & `mongodb_odm-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mongodb_odm-0.2.1/README.md` & `mongodb_odm-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `mongodb_odm-0.2.1/mongodb_odm/connection.py` & `mongodb_odm-0.2.2/mongodb_odm/connection.py`

 * *Files identical despite different names*

### Comparing `mongodb_odm-0.2.1/mongodb_odm/data_conversion.py` & `mongodb_odm-0.2.2/mongodb_odm/data_conversion.py`

 * *Files identical despite different names*

### Comparing `mongodb_odm-0.2.1/mongodb_odm/fields.py` & `mongodb_odm-0.2.2/mongodb_odm/fields.py`

 * *Files identical despite different names*

### Comparing `mongodb_odm-0.2.1/mongodb_odm/models.py` & `mongodb_odm-0.2.2/mongodb_odm/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,16 +130,16 @@
     #         exclude=cls.get_exclude_fields(), exclude_none=True
     #     )
 
     def to_mongo(self) -> DICT_TYPE:
         return self.dict(exclude=self.get_exclude_fields(), exclude_none=True)
 
     @classmethod
-    def start_session(cls) -> client_session.ClientSession:
-        return get_client().start_session()
+    def start_session(cls, **kwargs: Any) -> client_session.ClientSession:
+        return get_client().start_session(**kwargs)
 
     def __str__(self) -> str:
         return super().__repr__()
 
 
 class Document(_BaseDocument):
     _id: ODMObjectId = Field(default_factory=ObjectId)
```

### Comparing `mongodb_odm-0.2.1/mongodb_odm/types.py` & `mongodb_odm-0.2.2/mongodb_odm/types.py`

 * *Files identical despite different names*

### Comparing `mongodb_odm-0.2.1/mongodb_odm/utils/apply_indexes.py` & `mongodb_odm-0.2.2/mongodb_odm/utils/apply_indexes.py`

 * *Files identical despite different names*

### Comparing `mongodb_odm-0.2.1/mongodb_odm/utils/utils.py` & `mongodb_odm-0.2.2/mongodb_odm/utils/utils.py`

 * *Files identical despite different names*

### Comparing `mongodb_odm-0.2.1/pyproject.toml` & `mongodb_odm-0.2.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [tool.poetry]
 name = "mongodb-odm"
-version = "0.2.1"
+version = "0.2.2"
 description = "MongoDB-ODM, NOSQL databases in Python, designed for simplicity, compatibility, and robustness."
 authors = ["Nayan Biswas <nayan32biswas@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 # homepage = "https://github.com/nayan32biswas/mongodb-odm"
 documentation = "https://mongodb-odm.readthedocs.io"
 repository = "https://github.com/nayan32biswas/mongodb-odm"
+# include = ["mongodb_odm"]
+# exclude = []
 
-exclude = []
 classifiers = [
     "Development Status :: 4 - Beta",
     "Framework :: AsyncIO",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Intended Audience :: System Administrators",
@@ -89,11 +90,11 @@
 # --strict end
 
 [[tool.mypy.overrides]]
 module = ""
 warn_unused_ignores = false
 
 [tool.flake8]
-    exclude = ".env"
-    max-complexity = 10
-    max-line-length = 100
-    extend-ignore = """"""
+exclude = ".env"
+max-complexity = 10
+max-line-length = 100
+extend-ignore = """"""
```

### Comparing `mongodb_odm-0.2.1/setup.py` & `mongodb_odm-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pydantic>=1.10.7,<2.0.0', 'pymongo[srv]>=4.3.3,<5.0.0']
 
 setup_kwargs = {
     'name': 'mongodb-odm',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'MongoDB-ODM, NOSQL databases in Python, designed for simplicity, compatibility, and robustness.',
     'long_description': '# MongoDB-ODM\n\n<p align="center">\n    <em>MongoDB-ODM, NOSQL databases in Python, designed for simplicity, compatibility, and robustness.</em>\n</p>\n\n<p align="center">\n\n<a href="https://github.com/nayan32biswas/mongodb-odm/actions/workflows/test.yml" target="_blank">\n    <img src="https://github.com/nayan32biswas/mongodb-odm/actions/workflows/test.yml/badge.svg?branch=main&event=push" alt="Test">\n</a>\n<a href="https://coverage-badge.samuelcolvin.workers.dev/redirect/nayan32biswas/mongodb-odm" target="_blank">\n    <img src="https://coverage-badge.samuelcolvin.workers.dev/nayan32biswas/mongodb-odm.svg" alt="Coverage">\n<br />\n<a href="https://pypi.org/project/mongodb-odm/" target="_blank">\n    <img alt="PyPI" src="https://img.shields.io/pypi/v/mongodb-odm?color=%2334D058&label=PyPi%20Package">\n</a>\n<a href="https://pypi.org/project/mongodb-odm/" target="_blank">\n    <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/mongodb-odm?color=%2334D058">\n</a>\n\n</p>\n\n---\n\n**Documentation**: <a href="https://mongodb-odm.readthedocs.io" target="_blank">https://mongodb-odm.readthedocs.io</a>\n\n**PyPi**: <a href="https://pypi.org/project/mongodb-odm" target="_blank">https://pypi.org/project/mongodb-odm</a>\n\n**Repository**: <a href="https://github.com/nayan32biswas/mongodb-odm" target="_blank">https://github.com/nayan32biswas/mongodb-odm</a>\n\n---\n\n## Introduction\n\nThe purpose of this module is to provide easy access to the database with the python object feature with **MongoDB** and **PyMongo**. With PyMongo that was very easy to make spelling mistakes in a collection name when you are doing database operation. This module provides you with minimal ODM with a modeling feature so that you don’t have to look up the MongoDB dashboard(Mongo Compass) to know about field names or data types.\n\n**MongoDB-ODM** is based on Python type annotations, and powered by <a href="https://pymongo.readthedocs.io/en/stable/" class="external-link" target="_blank">PyMongo</a> and <a href="https://docs.pydantic.dev/" class="external-link" target="_blank">Pydantic</a>.\n\nThe key features are:\n\n- **Intuitive to write**: Great editor support. Completion everywhere. Less time debugging. Designed to be easy to use and learn. Less time reading docs.\n- **Easy to use**: It has sensible defaults and does a lot of work underneath to simplify the code you write.\n- **Compatible**: It is designed to be compatible with **FastAPI**, **Pydantic**, and **PyMongo**.\n- **Extensible**: You have all the power of **PyMongo** and **Pydantic** underneath.\n- **Short**: Minimize code duplication. A single type annotation does a lot of work. No need to duplicate models in **PyMongo** and Pydantic.\n\n---\n\n## Requirement\n\n**MongoDB-ODM** will work on <a href="https://www.python.org/downloads/" class="external-link" target="_blank">Python 3.8 and above</a>\n\nThis **MongoDB-ODM** is built on top of **PyMongo** and **Pydantic**. Those packages are required and will auto-install while **MongoDB-ODM** was installed.\n\n## Installation\n\n```console\n$ pip install mongodb-odm\n```\n\n## Example\n\n### Define model\n\n```Python\nimport os\nfrom typing import Optional\n\nfrom mongodb_odm import ASCENDING, Document, IndexModel, connect\n\n\nclass Player(Document):\n    name: str\n    country_code: str\n    rating: Optional[int] = None\n\n    class Config(Document.Config):\n        indexes = [\n            IndexModel([("rating", ASCENDING)]),\n        ]\n```\n\n### Set Connection\n\n```Python\nconnect(os.environ.get("MONGO_URL", "mongodb://localhost:27017/testdb"))\n```\n\n### Create Document\n\n```Python\npele = Player(name="Pelé", country_code="BRA").create()\nmaradona = Player(name="Diego Maradona", country_code="ARG", rating=97).create()\nzidane = Player(name="Zinedine Zidane", country_code="FRA", rating=96).create()\n```\n\n### Retrieve Document\n\n#### Find data from collection\n\n```Python\nfor player in Player.find():\n    print(player)\n```\n\n#### Find one object with filter\n\n```Python\nplayer = Player.find_one({"name": "Pelé"})\n```\n\n### Update Data\n\n```Python\nplayer = Player.find_one({"name": "Pelé"})\nif player:\n    player.rating = 98  # potential\n    player.update()\n```\n\n### Delete Data\n\n```Python\nplayer = Player.find_one({"name": "Pelé"})\nif player:\n    player.delete()\n```\n\n### Apply Indexes\n\n```Python\nimport os\nfrom typing import Optional\n\nfrom mongodb_odm import ASCENDING, Document, IndexModel, connect\n\n\nclass Player(Document):\n    name: str\n    country_code: str\n    rating: Optional[int] = None\n\n    class Config(Document.Config):\n        indexes = [\n            IndexModel([("rating", ASCENDING)]),\n        ]\n```\n\n- To create indexes in the database declare [IndexModel](https://pymongo.readthedocs.io/en/stable/tutorial.html#indexing) and assign in indexes array in Config class. **IndexModel** modules that are directly imported from **pymongo**.\n- Import the `apply_indexes` from `mongodb_odm`. Call the `apply_indexes` function from your CLI. You can use <a href="https://typer.tiangolo.com" class="external-link" target="_blank">Typer</a> to implement CLI.\n\n## Example Code\n\nThis is the example of full code of above.\n\n```python\nimport os\nfrom typing import Optional\n\nfrom mongodb_odm import ASCENDING, Document, IndexModel, connect\n\n\nclass Player(Document):\n    name: str\n    country_code: str\n    rating: Optional[int] = None\n\n    class Config(Document.Config):\n        indexes = [\n            IndexModel([("rating", ASCENDING)]),\n        ]\n\n\nconnect(os.environ.get("MONGO_URL", "mongodb://localhost:27017/testdb"))\n\npele = Player(name="Pelé", country_code="BRA").create()\nmaradona = Player(name="Diego Maradona", country_code="ARG", rating=97).create()\nzidane = Player(name="Zinedine Zidane", country_code="FRA", rating=96).create()\n\nfor player in Player.find():\n    print(player)\n\nplayer = Player.find_one({"name": "Pelé"})\nif player:\n    player.rating = 98  # potential\n    player.update()\n\nplayer = Player.find_one({"name": "Pelé"})\nif player:\n    player.delete()\n```\n\n### Supported Framework\n\n**MongoDB-ODM** is not framework dependent. We can use this package in any system. But we take special consideration being compatible with <a href="https://fastapi.tiangolo.com/" class="external-link" target="_blank">FastAPI</a> and <a href="https://flask.palletsprojects.com/en/2.2.x/" class="external-link" target="_blank">Flask</a>.\n\n### Credit\n\nThis package is built on top of <a href="https://pymongo.readthedocs.io/en/stable" class="external-link" target="_blank">PyMongo</a> and <a href="https://docs.pydantic.dev" class="external-link" target="_blank">Pydantic</a>.\n\nDocumentation generated by <a href="https://www.mkdocs.org/" class="external-link" target="_blank">MkDocs</a> and <a href="https://squidfunk.github.io/mkdocs-material/" class="external-link" target="_blank">Material for MkDocs</a>.\n\nDocumentation inspired by <a href="https://sqlmodel.tiangolo.com" class="external-link" target="_blank">SQLModel</a>.\n\nBut we use other packages for development and other purposes. Check **pyproject.toml** to know about all packages we use to build this package.\n\n## License\n\nThis project is licensed under the terms of the [MIT license](https://github.com/nayan32biswas/mongodb-odm/blob/main/LICENSE).\n',
     'author': 'Nayan Biswas',
     'author_email': 'nayan32biswas@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/nayan32biswas/mongodb-odm',
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['mongodb_odm', 'mongodb_odm.utils'] package_data = \ {'': ['*']}
 install_requires = \ ['pydantic>=1.10.7,<2.0.0', 'pymongo[srv]>=4.3.3,<5.0.0']
-setup_kwargs = { 'name': 'mongodb-odm', 'version': '0.2.1', 'description':
+setup_kwargs = { 'name': 'mongodb-odm', 'version': '0.2.2', 'description':
 'MongoDB-ODM, NOSQL databases in Python, designed for simplicity,
 compatibility, and robustness.', 'long_description': '# MongoDB-ODM\n\n
       \n MongoDB-ODM, NOSQL databases in Python, designed for simplicity,
                        compatibility, and robustness.\n
 \n\n
                        \n\n\n_[Test]\n\n\n_[Coverage]\n
                 \n\n_[PyPI]\n\n\n_[PyPI_-_Python_Version]\n\n\n
```

### Comparing `mongodb_odm-0.2.1/PKG-INFO` & `mongodb_odm-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongodb-odm
-Version: 0.2.1
+Version: 0.2.2
 Summary: MongoDB-ODM, NOSQL databases in Python, designed for simplicity, compatibility, and robustness.
 Home-page: https://github.com/nayan32biswas/mongodb-odm
 License: MIT
 Author: Nayan Biswas
 Author-email: nayan32biswas@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```


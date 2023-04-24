# Comparing `tmp/pyaemet-1.1.0rc0.tar.gz` & `tmp/pyaemet-1.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaemet-1.1.0rc0.tar", max compression
+gzip compressed data, was "pyaemet-1.1.0rc1.tar", max compression
```

## Comparing `pyaemet-1.1.0rc0.tar` & `pyaemet-1.1.0rc1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35149 2022-08-29 18:57:39.634520 pyaemet-1.1.0rc0/LICENSE
--rw-r--r--   0        0        0     4584 2023-04-24 20:17:14.017440 pyaemet-1.1.0rc0/README.md
--rw-r--r--   0        0        0     1140 2023-04-24 21:11:23.196165 pyaemet-1.1.0rc0/pyproject.toml
--rw-r--r--   0        0        0       93 2023-04-24 21:12:23.372714 pyaemet-1.1.0rc0/src/pyaemet/__init__.py
--rw-r--r--   0        0        0     6050 2023-04-24 20:17:14.025440 pyaemet-1.1.0rc0/src/pyaemet/aemet_request.py
--rw-r--r--   0        0        0    18982 2023-04-24 20:17:14.025440 pyaemet-1.1.0rc0/src/pyaemet/climatology.py
--rw-r--r--   0        0        0        0 2023-04-24 20:17:14.025440 pyaemet-1.1.0rc0/src/pyaemet/static/__init__.py
--rw-r--r--   0        0        0    33781 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc0/src/pyaemet/static/sites/data.csv
--rw-r--r--   0        0        0     3029 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc0/src/pyaemet/static/sites/metadata.json
--rw-r--r--   0        0        0        0 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc0/src/pyaemet/types_classes/__init__.py
--rw-r--r--   0        0        0      866 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc0/src/pyaemet/types_classes/observations.py
--rw-r--r--   0        0        0    10835 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc0/src/pyaemet/types_classes/sites.py
--rw-r--r--   0        0        0        0 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc0/src/pyaemet/utilities/__init__.py
--rw-r--r--   0        0        0     2127 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc0/src/pyaemet/utilities/coordinates.py
--rw-r--r--   0        0        0     1865 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc0/src/pyaemet/utilities/curation.py
--rw-r--r--   0        0        0     2511 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc0/src/pyaemet/utilities/dictionaries.py
--rw-r--r--   0        0        0     5718 1970-01-01 00:00:00.000000 pyaemet-1.1.0rc0/setup.py
--rw-r--r--   0        0        0     5833 1970-01-01 00:00:00.000000 pyaemet-1.1.0rc0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-08-29 18:57:39.634520 pyaemet-1.1.0rc1/LICENSE
+-rw-r--r--   0        0        0     4584 2023-04-24 20:17:14.017440 pyaemet-1.1.0rc1/README.md
+-rw-r--r--   0        0        0     1174 2023-04-24 21:29:29.586546 pyaemet-1.1.0rc1/pyproject.toml
+-rw-r--r--   0        0        0       91 2023-04-24 21:27:51.334140 pyaemet-1.1.0rc1/src/pyaemet/__init__.py
+-rw-r--r--   0        0        0     6050 2023-04-24 20:17:14.025440 pyaemet-1.1.0rc1/src/pyaemet/aemet_request.py
+-rw-r--r--   0        0        0    18982 2023-04-24 21:27:51.334140 pyaemet-1.1.0rc1/src/pyaemet/climatology.py
+-rw-r--r--   0        0        0        0 2023-04-24 20:17:14.025440 pyaemet-1.1.0rc1/src/pyaemet/static/__init__.py
+-rw-r--r--   0        0        0    33781 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc1/src/pyaemet/static/sites/data.csv
+-rw-r--r--   0        0        0     3029 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc1/src/pyaemet/static/sites/metadata.json
+-rw-r--r--   0        0        0        0 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc1/src/pyaemet/types_classes/__init__.py
+-rw-r--r--   0        0        0      866 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc1/src/pyaemet/types_classes/observations.py
+-rw-r--r--   0        0        0    10835 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc1/src/pyaemet/types_classes/sites.py
+-rw-r--r--   0        0        0        0 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc1/src/pyaemet/utilities/__init__.py
+-rw-r--r--   0        0        0     2127 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc1/src/pyaemet/utilities/coordinates.py
+-rw-r--r--   0        0        0     1865 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc1/src/pyaemet/utilities/curation.py
+-rw-r--r--   0        0        0     2511 2023-04-24 20:17:14.029440 pyaemet-1.1.0rc1/src/pyaemet/utilities/dictionaries.py
+-rw-r--r--   0        0        0     5669 1970-01-01 00:00:00.000000 pyaemet-1.1.0rc1/setup.py
+-rw-r--r--   0        0        0     5684 1970-01-01 00:00:00.000000 pyaemet-1.1.0rc1/PKG-INFO
```

### Comparing `pyaemet-1.1.0rc0/LICENSE` & `pyaemet-1.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaemet-1.1.0rc0/README.md` & `pyaemet-1.1.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `pyaemet-1.1.0rc0/pyproject.toml` & `pyaemet-1.1.0rc1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyaemet"
-version = "1.1.0rc"
+version = "1.1.0rc1"
 
 description = "Python module to interact with the AEMET API to download meteorological data"
 readme = "README.md"
 homepage = "https://github.com/jaimedgp/pyAEMET"
 repository = "https://github.com/jaimedgp/pyAEMET"
 license = "GPL-3.0-or-later"
 
@@ -30,22 +30,25 @@
     { path = ".env" },
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/jaimedgp/pyAEMET/issues"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
-requests = "^2.28.2"
-numpy = "^1.24.3"
-matplotlib = "^3.7.1"
-pandas = "^2.0.1"
-geocoder = "^1.38.1"
-folium = "^0.14.0"
-tqdm = "^4.65.0"
+python = ">=3.10,<4.0"
+requests = "2.24.0"
+numpy = "1.19.0"
+matplotlib = "3.2.2"
+pandas = "1.1.0"
+geocoder = "1.38.0"
+folium = "0.11.0"
+tqdm = "4.46.1"
+
+[tool.poetry.group.dev.dependencies]
+
 
 [tool.poetry.group.test.dependencies]
 pytest = "6.0.0"
 python-dotenv = "0.14.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `pyaemet-1.1.0rc0/src/pyaemet/aemet_request.py` & `pyaemet-1.1.0rc1/src/pyaemet/aemet_request.py`

 * *Files identical despite different names*

### Comparing `pyaemet-1.1.0rc0/src/pyaemet/climatology.py` & `pyaemet-1.1.0rc1/src/pyaemet/climatology.py`

 * *Files identical despite different names*

### Comparing `pyaemet-1.1.0rc0/src/pyaemet/static/sites/data.csv` & `pyaemet-1.1.0rc1/src/pyaemet/static/sites/data.csv`

 * *Files identical despite different names*

### Comparing `pyaemet-1.1.0rc0/src/pyaemet/static/sites/metadata.json` & `pyaemet-1.1.0rc1/src/pyaemet/static/sites/metadata.json`

 * *Files identical despite different names*

### Comparing `pyaemet-1.1.0rc0/src/pyaemet/types_classes/observations.py` & `pyaemet-1.1.0rc1/src/pyaemet/types_classes/observations.py`

 * *Files identical despite different names*

### Comparing `pyaemet-1.1.0rc0/src/pyaemet/types_classes/sites.py` & `pyaemet-1.1.0rc1/src/pyaemet/types_classes/sites.py`

 * *Files identical despite different names*

### Comparing `pyaemet-1.1.0rc0/src/pyaemet/utilities/coordinates.py` & `pyaemet-1.1.0rc1/src/pyaemet/utilities/coordinates.py`

 * *Files identical despite different names*

### Comparing `pyaemet-1.1.0rc0/src/pyaemet/utilities/curation.py` & `pyaemet-1.1.0rc1/src/pyaemet/utilities/curation.py`

 * *Files identical despite different names*

### Comparing `pyaemet-1.1.0rc0/src/pyaemet/utilities/dictionaries.py` & `pyaemet-1.1.0rc1/src/pyaemet/utilities/dictionaries.py`

 * *Files identical despite different names*

### Comparing `pyaemet-1.1.0rc0/setup.py` & `pyaemet-1.1.0rc1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,34 +7,34 @@
 packages = \
 ['pyaemet', 'pyaemet.static', 'pyaemet.types_classes', 'pyaemet.utilities']
 
 package_data = \
 {'': ['*'], 'pyaemet.static': ['sites/*']}
 
 install_requires = \
-['folium>=0.14.0,<0.15.0',
- 'geocoder>=1.38.1,<2.0.0',
- 'matplotlib>=3.7.1,<4.0.0',
- 'numpy>=1.24.3,<2.0.0',
- 'pandas>=2.0.1,<3.0.0',
- 'requests>=2.28.2,<3.0.0',
- 'tqdm>=4.65.0,<5.0.0']
+['folium==0.11.0',
+ 'geocoder==1.38.0',
+ 'matplotlib==3.2.2',
+ 'numpy==1.19.0',
+ 'pandas==1.1.0',
+ 'requests==2.24.0',
+ 'tqdm==4.46.1']
 
 setup_kwargs = {
     'name': 'pyaemet',
-    'version': '1.1.0rc0',
+    'version': '1.1.0rc1',
     'description': 'Python module to interact with the AEMET API to download meteorological data',
     'long_description': '# pyAEMET\n\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/pyaemet.svg)](https://pypi.org/project/pyaemet/)\n[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5655307.svg)](https://doi.org/10.5281/zenodo.5655307)\n[![License](https://img.shields.io/pypi/l/pandas.svg)](https://github.com/jaimedgp/pyAEMET/blob/main/LICENSE)\n[![Downloads](https://static.pepy.tech/personalized-badge/pyaemet?period=month&units=international_system&left_color=gray&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/pyaemet)\n\nA python library developed to download daily climatological values from the Spanish National\nMeteorological Agency (AEMET) through its OpenData API. The library contains several methods\nto facilitate downloading and filtering the climatological data.\n\n> The information that this library collects and uses is property of the Spanish State\n> Meteorological Agency, available through its AEMET OpenData REST API.\n\n\n## Installation\n``` bash\n$ pip install pyaemet\n```\nTo use the pyAEMET module, you need to get an API key from the AEMET (Spanish State Meteorological\nAgency) OpenData platform. You can apply for a key [here](https://opendata.aemet.es/centrodedescargas/altaUsuario).\n\n## Usage\n\nOnce the module is installed and you have your API key, you can start using the module by\nimporting it in your Python script. To use the module\'s functions, you need to initialize\nthe client with your API key:\n\n```python\nimport pyaemet\n\naemet = pyaemet.AemetClima(api_key)\n```\n\nThe `AemetClima` class takes an API key as a parameter in its constructor and allows you to get\ninformation about the available monitoring sites, filter sites based on different parameters\n(e.g., city, province, autonomous community), and get nearby sites to a specific location.\n\nHere is a summary of some of the methods provided by the `AemetClima` class:\n\n* **`sites_info`**: Retrieves information about all the available monitoring sites. The method\nreturns an instance of the `SitesDataFrame` class, which is a subclass of the pandas `DataFrame`.\n```python\naemet.sites_info(update=True)\n```\n\n* **`sites_in`**: Filters the available monitoring sites based on specified parameters\n(e.g., city, province, autonomous community). The method returns an instance of the `SitesDataFrame` class.\n```python\naemet.sites_in(subregion="Cantabria")\n```\n![image](https://github.com/Jaimedgp/pyAEMET/raw/main/docs/screenshots/sites_cantabria.png)\n\n* **`near_sites`**: Retrieves the ``n_near`` monitoring sites closest to a specified latitude and longitude,\nwithin a maximum distance of `max_distance` kilometers. The method returns an instance of the\n`NearSitesDataFrame` class.\n```python\naemet.near_sites(latitude=43.47,\n                 longitude=-3.798,\n                 n_near=5, max_distance=50)\n```\n![image](https://github.com/Jaimedgp/pyAEMET/raw/main/docs/screenshots/near_sites.png)\n\n* **`sites_curation`**: Retrieves the amount of available data of certain `variables` in the monitoring `sites` in a period of time defined by\n    `start_dt` and `end_dt`. The function returns a `SitesDataFrame` or `NearSitesDataFrame` (depends of the type of the `sites` parameter given)\n    with a column with the average `amount` between all `variables` and `has_enough` boolean if the amount is greater or equal to a `threshold`.\n\n* **`daily_clima`**: Retrieves daily climate data for a given ``site`` or a list of sites over a\nspecified date range defined by `start_dt` and `end_dt`. The function returns a\n`ObservationsDataFrame` object, which is a data structure that holds the retrieved climate data\nalong with any associated metadata.\n```python\nimport datetime\naemet.daily_clima(site=aemet.sites_in(city="Santander"),\n                  start_dt=datetime.date(2022, 6, 3),\n                  end_dt=datetime.date.today())\n```\n\nThe module also provides three deprecated methods `estaciones_info`, `estaciones_loc` and `clima_diaria`\nthat perform similar functionality as the `sites_info`, `sites_in` and `daily_clima` methods, respectively.\n\nYou can find the complete documentation of the module\'s functions in the GitHub repository,\nunder the docs directory.\n\n## FAQ\n## Contributing\n## References\n* ["Estimating changes in air pollutant levels due to COVID-19 lockdown measures based on a business-as-usual prediction scenario using data mining models: A case-study for urban traffic sites in Spain"](https://doi.org/10.1016/j.scitotenv.2022.153786), submitted to Environmental Software & Modelling by [J. González-Pardo](https://orcid.org/0000-0001-7268-9933) et al. (2021)\n',
     'author': 'Jaimedgp',
     'author_email': 'jaime.diez.gp@gmail.com',
     'maintainer': 'CarmenGBM',
     'maintainer_email': 'carmen.garcia.be96@gmail.com',
     'url': 'https://github.com/jaimedgp/pyAEMET',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `pyaemet-1.1.0rc0/PKG-INFO` & `pyaemet-1.1.0rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: pyaemet
-Version: 1.1.0rc0
+Version: 1.1.0rc1
 Summary: Python module to interact with the AEMET API to download meteorological data
 Home-page: https://github.com/jaimedgp/pyAEMET
 License: GPL-3.0-or-later
 Keywords: AEMET,Meteorology,API,AEMET OpenData
 Author: Jaimedgp
 Author-email: jaime.diez.gp@gmail.com
 Maintainer: CarmenGBM
 Maintainer-email: carmen.garcia.be96@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3
-Requires-Dist: folium (>=0.14.0,<0.15.0)
-Requires-Dist: geocoder (>=1.38.1,<2.0.0)
-Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
-Requires-Dist: numpy (>=1.24.3,<2.0.0)
-Requires-Dist: pandas (>=2.0.1,<3.0.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
-Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Requires-Dist: folium (==0.11.0)
+Requires-Dist: geocoder (==1.38.0)
+Requires-Dist: matplotlib (==3.2.2)
+Requires-Dist: numpy (==1.19.0)
+Requires-Dist: pandas (==1.1.0)
+Requires-Dist: requests (==2.24.0)
+Requires-Dist: tqdm (==4.46.1)
 Project-URL: Bug Tracker, https://github.com/jaimedgp/pyAEMET/issues
 Project-URL: Repository, https://github.com/jaimedgp/pyAEMET
 Description-Content-Type: text/markdown
 
 # pyAEMET
```


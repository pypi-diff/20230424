# Comparing `tmp/tum_esm_em27_metadata-2.0.0rc2.tar.gz` & `tmp/tum_esm_em27_metadata-2.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tum_esm_em27_metadata-2.0.0rc2.tar", max compression
+gzip compressed data, was "tum_esm_em27_metadata-2.0.0rc3.tar", max compression
```

## Comparing `tum_esm_em27_metadata-2.0.0rc2.tar` & `tum_esm_em27_metadata-2.0.0rc3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2826 2023-04-23 11:30:01.572048 tum_esm_em27_metadata-2.0.0rc2/README.md
--rw-r--r--   0        0        0     1107 2023-04-23 12:10:46.736552 tum_esm_em27_metadata-2.0.0rc2/pyproject.toml
--rw-r--r--   0        0        0      126 2023-04-23 10:28:10.736200 tum_esm_em27_metadata-2.0.0rc2/tum_esm_em27_metadata/__init__.py
--rw-r--r--   0        0        0     6358 2023-04-23 12:10:29.334964 tum_esm_em27_metadata-2.0.0rc2/tum_esm_em27_metadata/interfaces.py
--rw-r--r--   0        0        0     2112 2023-04-23 11:12:48.008464 tum_esm_em27_metadata-2.0.0rc2/tum_esm_em27_metadata/loader.py
--rw-r--r--   0        0        0        0 2023-04-19 09:38:48.570525 tum_esm_em27_metadata-2.0.0rc2/tum_esm_em27_metadata/py.typed
--rw-r--r--   0        0        0     3910 2023-04-23 11:09:58.388668 tum_esm_em27_metadata-2.0.0rc2/tum_esm_em27_metadata/types.py
--rw-r--r--   0        0        0     3759 1970-01-01 00:00:00.000000 tum_esm_em27_metadata-2.0.0rc2/setup.py
--rw-r--r--   0        0        0     3541 1970-01-01 00:00:00.000000 tum_esm_em27_metadata-2.0.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     2826 2023-04-23 11:30:01.572048 tum_esm_em27_metadata-2.0.0rc3/README.md
+-rw-r--r--   0        0        0     1061 2023-04-24 18:57:54.884363 tum_esm_em27_metadata-2.0.0rc3/pyproject.toml
+-rw-r--r--   0        0        0      126 2023-04-23 10:28:10.736200 tum_esm_em27_metadata-2.0.0rc3/tum_esm_em27_metadata/__init__.py
+-rw-r--r--   0        0        0     6459 2023-04-24 18:57:22.893799 tum_esm_em27_metadata-2.0.0rc3/tum_esm_em27_metadata/interfaces.py
+-rw-r--r--   0        0        0     2112 2023-04-23 11:12:48.008464 tum_esm_em27_metadata-2.0.0rc3/tum_esm_em27_metadata/loader.py
+-rw-r--r--   0        0        0        0 2023-04-19 09:38:48.570525 tum_esm_em27_metadata-2.0.0rc3/tum_esm_em27_metadata/py.typed
+-rw-r--r--   0        0        0     4033 2023-04-24 18:50:37.062912 tum_esm_em27_metadata-2.0.0rc3/tum_esm_em27_metadata/types.py
+-rw-r--r--   0        0        0     3731 1970-01-01 00:00:00.000000 tum_esm_em27_metadata-2.0.0rc3/setup.py
+-rw-r--r--   0        0        0     3500 1970-01-01 00:00:00.000000 tum_esm_em27_metadata-2.0.0rc3/PKG-INFO
```

### Comparing `tum_esm_em27_metadata-2.0.0rc2/README.md` & `tum_esm_em27_metadata-2.0.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `tum_esm_em27_metadata-2.0.0rc2/pyproject.toml` & `tum_esm_em27_metadata-2.0.0rc3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 [tool.poetry]
 name = "tum_esm_em27_metadata"
-version = "2.0.0-rc.2"
+version = "2.0.0-rc.3"
 description = "Single source of truth for ESM's EM27 measurement logistics"
 readme = "README.md"
 authors = [
     "Moritz Makowski <moritz.makowski@tum.de>",
     "Marlon Mueller <marlon.mueller@tum.de>"
 ]
 packages = [
     {include = "tum_esm_em27_metadata"},
     {include = "tum_esm_em27_metadata/py.typed"},
 ]
 repository = "https://github.com/tum-esm/em27-metadata"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-pydantic = "^1.10.4"
-tum-esm-utils = "^1.0.0"
-pendulum = "^2.1.2"
+pydantic = "^1.10.7"
+tum-esm-utils = "^1.4.0"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.2.1"
+pytest = "^7.3.1"
 black = "^22.12.0"
-python-dotenv = "^0.21.1"
 mypy = "^1.2.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
```

### Comparing `tum_esm_em27_metadata-2.0.0rc2/tum_esm_em27_metadata/interfaces.py` & `tum_esm_em27_metadata-2.0.0rc3/tum_esm_em27_metadata/interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from pydantic import BaseModel
 from tum_esm_em27_metadata import types
-import pendulum
 
 
 class EM27MetadataInterface:
     def __init__(
         self,
         locations: list[types.LocationMetadata],
         sensors: list[types.SensorMetadata],
@@ -154,14 +153,17 @@
     for c1 in campaigns:
         for s2 in c1.stations:
             assert (
                 s2.default_location_id in location_ids
             ), f"unknown location id {s2.default_location_id}"
             assert s2.sensor_id in sensor_ids, f"unknown sensor id {s2.sensor_id}"
 
+        for lid in c1.additional_location_ids:
+            assert lid in location_ids, f"unknown location id {lid}"
+
     # integrity of time series in sensors.json
     for s3 in sensors:
         for location_timeseries in [
             [_DatetimeSeriesItem(**l2.dict()) for l2 in s3.locations],
             [_DatetimeSeriesItem(**l2.dict()) for l2 in s3.different_utc_offsets],
             [_DatetimeSeriesItem(**l2.dict()) for l2 in s3.different_pressure_data_sources],
             [_DatetimeSeriesItem(**l2.dict()) for l2 in s3.different_pressure_calibration_factors],
```

### Comparing `tum_esm_em27_metadata-2.0.0rc2/tum_esm_em27_metadata/loader.py` & `tum_esm_em27_metadata-2.0.0rc3/tum_esm_em27_metadata/loader.py`

 * *Files identical despite different names*

### Comparing `tum_esm_em27_metadata-2.0.0rc2/tum_esm_em27_metadata/types.py` & `tum_esm_em27_metadata-2.0.0rc3/tum_esm_em27_metadata/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,20 @@
 
 
 class _TimeSeriesElement(BaseModel):
     from_date: str
     to_date: str
 
     # validators
-    _val_date_string = validator("from_date", "to_date", pre=True, allow_reuse=True,)(
+    _val_date_string = validator(
+        "from_date",
+        "to_date",
+        pre=True,
+        allow_reuse=True,
+    )(
         validate_str(is_date_string=True),
     )
 
 
 class SensorTypes:
     class DifferentUTCOffset(_TimeSeriesElement):
         utc_offset: float
@@ -21,15 +26,19 @@
             validate_float(minimum=-12, maximum=12),
         )
 
     class DifferentPressureDataSource(_TimeSeriesElement):
         source: str
 
         # validators
-        _val_source = validator("source", pre=True, allow_reuse=True,)(
+        _val_source = validator(
+            "source",
+            pre=True,
+            allow_reuse=True,
+        )(
             validate_str(),
         )
 
     class DifferentPressureCalibrationFactor(_TimeSeriesElement):
         factor: float
 
         # validators
@@ -114,14 +123,15 @@
         validate_int(minimum=1),
     )
 
 
 class CampaignMetadata(_TimeSeriesElement):
     campaign_id: str
     stations: list[CampaignTypes.Station]
+    additional_location_ids: list[str]
 
     # validators
     _val_campaign_id = validator("campaign_id", pre=True, allow_reuse=True)(
         validate_str(min_len=1, max_len=64, regex="^[a-z0-9_]+$"),
     )
```

### Comparing `tum_esm_em27_metadata-2.0.0rc2/setup.py` & `tum_esm_em27_metadata-2.0.0rc3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,21 +6,19 @@
 
 package_data = \
 {'': ['*']}
 
 modules = \
 ['py']
 install_requires = \
-['pendulum>=2.1.2,<3.0.0',
- 'pydantic>=1.10.4,<2.0.0',
- 'tum-esm-utils>=1.0.0,<2.0.0']
+['pydantic>=1.10.7,<2.0.0', 'tum-esm-utils>=1.4.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'tum-esm-em27-metadata',
-    'version': '2.0.0rc2',
+    'version': '2.0.0rc3',
     'description': "Single source of truth for ESM's EM27 measurement logistics",
     'long_description': '# EM27 Metadata\n\n## The purpose of this library\n\nThis repository is the single source of truth for our EM27 measurement logistics: "Where has each station been on each day of measurements?" We selected this format over putting it in a database due to various reasons:\n\n-   Easy to read, modify and extend by selective group members using GitHub permissions\n-   Changes to this are more evident here than in database logs\n-   Versioning (easy to revert mistakes)\n-   Automatic testing of the files integrities\n-   Easy import as a statically typed Python library\n\n<br/>\n\n## How it works\n\nThis repository only contains a Python library to interact with the metadata. The metadata itself is stored in local files or a GitHub repository. The library can load the metadata from both sources and provides a unified interface with static types to access it.\n\n<br/>\n\n## Library Usage\n\nInstall as a library:\n\n```bash\npoetry add tum-esm-em27-metadata\n# or\npip install tum-esm-em27-metadata\n```\n\n```python\nimport tum_esm_em27_metadata\n\nem27_metadata = tum_esm_em27_metadata.load_from_github(\n    github_repository="org-name/repo-name",\n    access_token="your-github-access-token",\n)\n\n# or load it from local files\nem27_metadata = tum_esm_em27_metadata.load_from_local_files(\n    locations_path="location-data/locations.json",\n    sensors_path="location-data/sensors.json",\n    campaigns_path="location-data/campaigns.json",\n)\n\nmetadata = em27_metadata.get(\n    sensor_id = "ma", date = "20220601"\n)\n\nprint(metadata.dict())\n```\n\nPrints out:\n\n```json\n{\n    "sensor_id": "ma",\n    "serial_number": 61,\n    "utc_offset": 0,\n    "pressure_data_source": "ma",\n    "pressure_calibration_factor": 1,\n    "output_calibration_factor": 1,\n    "date": "20220601",\n    "location": {\n        "location_id": "TUM_I",\n        "details": "TUM Dach Innenstadt",\n        "lon": 11.569,\n        "lat": 48.151,\n        "alt": 539\n    }\n}\n```\n\nThe object returned by `em27_metadata.get()` is of type `tum_esm_em27_metadata.types.SensorDataContext`. It is a Pydantic model (https://docs.pydantic.dev/) but can be converted to a dictionary using `metadata.dict()`.\n\nYou can find dummy data in the `data/` folder.\n\n<br/>\n\n## Set up an EM27 Metadata Storage Directory\n\nYou can use the repository https://github.com/tum-esm/em27-metadata-storage-template to create your own repository for storing the metadata. It contains a GitHub Actions workflow that automatically validates the metadata on every commit in any branch.\n\n<br/>\n\n## For Developers\n\nRun tests:\n\n```bash\n# used inside the GitHub CI for this repo\npytest -m "ci"\n\n# used inside the GitHub Actions workflow for storage repos\npytest -m "action"\n\n# can be used for local development (skips pulling from GitHub)\npytest -m "local"\n```\n\nPublish the Package to PyPI:\n\n```bash\npoetry build\npoetry publish\n```\n',
     'author': 'Moritz Makowski',
     'author_email': 'moritz.makowski@tum.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tum-esm/em27-metadata',
```

### Comparing `tum_esm_em27_metadata-2.0.0rc2/PKG-INFO` & `tum_esm_em27_metadata-2.0.0rc3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: tum-esm-em27-metadata
-Version: 2.0.0rc2
+Version: 2.0.0rc3
 Summary: Single source of truth for ESM's EM27 measurement logistics
 Home-page: https://github.com/tum-esm/em27-metadata
 Author: Moritz Makowski
 Author-email: moritz.makowski@tum.de
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pendulum (>=2.1.2,<3.0.0)
-Requires-Dist: pydantic (>=1.10.4,<2.0.0)
-Requires-Dist: tum-esm-utils (>=1.0.0,<2.0.0)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: tum-esm-utils (>=1.4.0,<2.0.0)
 Project-URL: Repository, https://github.com/tum-esm/em27-metadata
 Description-Content-Type: text/markdown
 
 # EM27 Metadata
 
 ## The purpose of this library
```


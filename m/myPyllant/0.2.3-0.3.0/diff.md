# Comparing `tmp/mypyllant-0.2.3.tar.gz` & `tmp/mypyllant-0.3.0.tar.gz`

## Comparing `mypyllant-0.2.3.tar` & `mypyllant-0.3.0.tar`

### file list

```diff
@@ -1,37 +1,36 @@
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 mypyllant-0.2.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0    45426 2020-02-02 00:00:00.000000 mypyllant-0.2.3/logo.png
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 mypyllant-0.2.3/requirements-dev.txt
--rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 mypyllant-0.2.3/run_pytest.sh
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 mypyllant-0.2.3/.github/workflows/build-test.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/__init__.py
--rw-r--r--   0        0        0    15957 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/api.py
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/const.py
--rwxr-xr-x   0        0        0     2687 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/export.py
--rw-r--r--   0        0        0     7738 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/py.typed
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/sample.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/__init__.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/conftest.py
--rwxr-xr-x   0        0        0      934 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/find_countries.py
--rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/generate_test_data.py
--rw-r--r--   0        0        0     7177 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/test_api.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/test_countries.py
--rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/test_generate_test_data.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/test_sample.py
--rwxr-xr-x   0        0        0      655 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/update_sample.py
--rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/utils.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/current_system.json
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/device_buckets.json
--rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/systems.json
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/current_system.json
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/device_buckets.json
--rw-r--r--   0        0        0     6354 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/systems.json
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/current_system.json
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/device_buckets.json
--rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/systems.json
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 mypyllant-0.2.3/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 mypyllant-0.2.3/LICENSE
--rw-r--r--   0        0        0     4581 2020-02-02 00:00:00.000000 mypyllant-0.2.3/README.md
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 mypyllant-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     5187 2020-02-02 00:00:00.000000 mypyllant-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 mypyllant-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    45426 2020-02-02 00:00:00.000000 mypyllant-0.3.0/logo.png
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 mypyllant-0.3.0/requirements-dev.txt
+-rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 mypyllant-0.3.0/run_pytest.sh
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 mypyllant-0.3.0/.github/workflows/build-test.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.3.0/src/myPyllant/__init__.py
+-rw-r--r--   0        0        0    17423 2020-02-02 00:00:00.000000 mypyllant-0.3.0/src/myPyllant/api.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 mypyllant-0.3.0/src/myPyllant/const.py
+-rwxr-xr-x   0        0        0     2782 2020-02-02 00:00:00.000000 mypyllant-0.3.0/src/myPyllant/export.py
+-rw-r--r--   0        0        0     8071 2020-02-02 00:00:00.000000 mypyllant-0.3.0/src/myPyllant/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.3.0/src/myPyllant/py.typed
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 mypyllant-0.3.0/src/myPyllant/sample.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 mypyllant-0.3.0/src/myPyllant/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.3.0/src/myPyllant/tests/__init__.py
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 mypyllant-0.3.0/src/myPyllant/tests/conftest.py
+-rwxr-xr-x   0        0        0      934 2020-02-02 00:00:00.000000 mypyllant-0.3.0/src/myPyllant/tests/find_countries.py
+-rw-r--r--   0        0        0     6824 2020-02-02 00:00:00.000000 mypyllant-0.3.0/src/myPyllant/tests/generate_test_data.py
+-rw-r--r--   0        0        0     7710 2020-02-02 00:00:00.000000 mypyllant-0.3.0/src/myPyllant/tests/test_api.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mypyllant-0.3.0/src/myPyllant/tests/test_countries.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 mypyllant-0.3.0/src/myPyllant/tests/test_export.py
+-rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 mypyllant-0.3.0/src/myPyllant/tests/test_generate_test_data.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 mypyllant-0.3.0/src/myPyllant/tests/test_sample.py
+-rwxr-xr-x   0        0        0      655 2020-02-02 00:00:00.000000 mypyllant-0.3.0/src/myPyllant/tests/update_sample.py
+-rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 mypyllant-0.3.0/src/myPyllant/tests/utils.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 mypyllant-0.3.0/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/claims.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 mypyllant-0.3.0/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/connection_status.json
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mypyllant-0.3.0/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/control_identifier.json
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 mypyllant-0.3.0/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/current_system.json
+-rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 mypyllant-0.3.0/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/device_buckets.json
+-rw-r--r--   0        0        0     5558 2020-02-02 00:00:00.000000 mypyllant-0.3.0/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/system.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mypyllant-0.3.0/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/time_zone.json
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 mypyllant-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 mypyllant-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 mypyllant-0.3.0/README.md
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 mypyllant-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 mypyllant-0.3.0/PKG-INFO
```

### Comparing `mypyllant-0.2.3/.pre-commit-config.yaml` & `mypyllant-0.3.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
         additional_dependencies:
           - aiohttp
           - aioresponses
           - freezegun
           - pydantic
           - pytest
           - types-requests
+          - types-python-dateutil
   - repo: local
     hooks:
       - id: update-sample
         name: update-sample
         entry: python src/myPyllant/tests/update_sample.py
         language: python
         pass_filenames: false
```

### Comparing `mypyllant-0.2.3/logo.png` & `mypyllant-0.3.0/logo.png`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.3/.github/workflows/build-test.yaml` & `mypyllant-0.3.0/.github/workflows/build-test.yaml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.3/src/myPyllant/api.py` & `mypyllant-0.3.0/src/myPyllant/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 from __future__ import annotations
 
 import datetime
 import logging
 import re
-from collections.abc import AsyncGenerator
+from collections.abc import AsyncIterator
 from html import unescape
 from urllib.parse import parse_qs, urlencode, urlparse
 
 import aiohttp
 from aiohttp import ClientResponseError
+from dateutil.tz import gettz
 
 from myPyllant.const import (
     API_URL_BASE,
     AUTHENTICATE_URL,
     BRANDS,
     CLIENT_ID,
     COUNTRIES,
+    DEFAULT_CONTROL_IDENTIFIER,
     DEFAULT_QUICK_VETO_DURATION,
     LOGIN_URL,
     TOKEN_URL,
 )
 from myPyllant.models import (
+    Claim,
     Device,
     DeviceData,
     DeviceDataBucketResolution,
     DHWOperationMode,
     DomesticHotWater,
     System,
     Zone,
@@ -95,14 +98,21 @@
             raise
         return self
 
     async def __aexit__(self, exc_type, exc, tb) -> None:
         if not self.aiohttp_session.closed:
             await self.aiohttp_session.close()
 
+    @classmethod
+    def get_system_id(cls, system: System | str) -> str:
+        if isinstance(system, System):
+            return system.id
+        else:
+            return system
+
     async def login(self):
         """
         This should really be done in the browser with OIDC, but that's not easy without support from Vaillant
 
         So instead, we grab the login endpoint from the HTML form of the login website and send username + password
         to obtain a session
         """
@@ -211,63 +221,56 @@
             "x-client-locale": "en-GB",
             "x-idm-identifier": "KEYCLOAK",
             "ocp-apim-subscription-key": "1e0a2f3511fb4c5bbb1c7f9fedd20b1c",
             "User-Agent": "okhttp/4.9.2",
             "Connection": "keep-alive",
         }
 
-    async def get_systems(self) -> AsyncGenerator[System, int]:
-        systems_url = f"{API_URL_BASE}/systems"
+    async def get_claims(self) -> AsyncIterator[Claim]:
         async with self.aiohttp_session.get(
-            systems_url, headers=self.get_authorized_headers()
-        ) as systems_resp:
-            for system_json in await systems_resp.json():
-                system_id = system_json["systemId"]
-                system_url = f"{API_URL_BASE}/emf/v2/{system_id}/currentSystem"
-
-                async with self.aiohttp_session.get(
-                    system_url, headers=self.get_authorized_headers()
-                ) as current_system_resp:
-                    current_system_json = await current_system_resp.json()
-                system = System(
-                    id=system_id,
-                    current_system=dict_to_snake_case(current_system_json),
-                    **dict_to_snake_case(system_json),
-                )
-                yield system
-
-    @staticmethod
-    async def get_devices_by_system(
-        system: System,
-    ) -> AsyncGenerator[Device, None]:
-        for device_raw in system.current_system.values():
-            if not (isinstance(device_raw, dict) and "device_uuid" in device_raw):
-                continue
-            device = Device(
-                system=system,
-                **device_raw,
+            f"{API_URL_BASE}/claims", headers=self.get_authorized_headers()
+        ) as claims_resp:
+            for claim_json in await claims_resp.json():
+                yield Claim(**dict_to_snake_case(claim_json))
+
+    async def get_systems(self) -> AsyncIterator[System]:
+        claims = self.get_claims()
+        async for claim in claims:
+            control_identifier = await self.get_control_identifier(claim.system_id)
+            system_url = (
+                f"{API_URL_BASE}/systems/{claim.system_id}/{control_identifier}"
+            )
+            current_system_url = (
+                f"{API_URL_BASE}/emf/v2/{claim.system_id}/currentSystem"
             )
 
-            serial_nos = {d.serial_number: d for d in system.devices}
-            if device.device_serial_number in serial_nos.keys():
-                device_info = serial_nos[device.device_serial_number]
-                device.operational_data = dict_to_snake_case(
-                    device_info.operational_data
-                )
-                device.name = device_info.name
+            async with self.aiohttp_session.get(
+                system_url, headers=self.get_authorized_headers()
+            ) as system_resp:
+                system_json = await system_resp.json()
 
-            yield device
+            async with self.aiohttp_session.get(
+                current_system_url, headers=self.get_authorized_headers()
+            ) as current_system_resp:
+                current_system_json = await current_system_resp.json()
+
+            system = System(
+                claim=claim,
+                current_system=dict_to_snake_case(current_system_json),
+                **dict_to_snake_case(system_json),
+            )
+            yield system
 
     async def get_data_by_device(
         self,
         device: Device,
         data_resolution: DeviceDataBucketResolution = DeviceDataBucketResolution.DAY,
         data_from: datetime.datetime | None = None,
         data_to: datetime.datetime | None = None,
-    ) -> AsyncGenerator[DeviceData, None]:
+    ) -> AsyncIterator[DeviceData]:
         for data in device.data:
             data_from = data_from or data.data_from
             if not data_from:
                 raise ValueError(
                     "No data_from set, and no data_from found in device data"
                 )
             data_to = data_to or data.data_to
@@ -279,15 +282,15 @@
                 "resolution": str(data_resolution),
                 "operationMode": data.operation_mode,
                 "energyType": data.value_type,
                 "startDate": start_date,
                 "endDate": end_date,
             }
             device_buckets_url = (
-                f"{API_URL_BASE}/emf/v2/{device.system.id}/"
+                f"{API_URL_BASE}/emf/v2/{device.system_id}/"
                 f"devices/{device.device_uuid}/buckets?{urlencode(querystring)}"
             )
             async with self.aiohttp_session.get(
                 device_buckets_url, headers=self.get_authorized_headers()
             ) as device_buckets_resp:
                 device_buckets_json = await device_buckets_resp.json()
                 yield DeviceData(
@@ -422,7 +425,44 @@
         return await self.aiohttp_session.post(
             url,
             json={
                 "operationMode": str(mode),
             },
             headers=self.get_authorized_headers(),
         )
+
+    async def get_connection_status(self, system: System | str) -> bool:
+        url = f"{API_URL_BASE}/systems/{self.get_system_id(system)}/meta-info/connection-status"
+        response = await self.aiohttp_session.get(
+            url,
+            headers=self.get_authorized_headers(),
+        )
+        try:
+            return (await response.json())["connected"]
+        except KeyError:
+            logger.warning("Couldn't get connection status")
+            return False
+
+    async def get_control_identifier(self, system: System | str) -> str | None:
+        url = f"{API_URL_BASE}/systems/{self.get_system_id(system)}/meta-info/control-identifier"
+        response = await self.aiohttp_session.get(
+            url,
+            headers=self.get_authorized_headers(),
+        )
+        try:
+            return (await response.json())["controlIdentifier"]
+        except KeyError:
+            logger.warning("Couldn't get control identifier")
+            return DEFAULT_CONTROL_IDENTIFIER
+
+    async def get_time_zone(self, system: System | str) -> datetime.tzinfo | None:
+        url = f"{API_URL_BASE}/systems/{self.get_system_id(system)}/meta-info/time-zone"
+        response = await self.aiohttp_session.get(
+            url,
+            headers=self.get_authorized_headers(),
+        )
+        try:
+            tz = (await response.json())["timeZone"]
+            return gettz(tz)
+        except KeyError:
+            logger.warning("Couldn't get timezone from API")
+            return None
```

### Comparing `mypyllant-0.2.3/src/myPyllant/const.py` & `mypyllant-0.3.0/src/myPyllant/const.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,7 +53,8 @@
         "portugal": "Portugal",
         "romania": "Romania",
         "slovakia": "Slovakia",
         "spain": "Spain",
     },
 }
 DEFAULT_QUICK_VETO_DURATION = 3
+DEFAULT_CONTROL_IDENTIFIER = "tli"
```

### Comparing `mypyllant-0.2.3/src/myPyllant/export.py` & `mypyllant-0.3.0/src/myPyllant/export.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 
 import argparse
 import asyncio
 import json
+import logging
 import sys
 from datetime import datetime
 
 from myPyllant.api import MyPyllantAPI
 from myPyllant.const import BRANDS, COUNTRIES, DEFAULT_BRAND
 from myPyllant.models import DeviceDataBucketResolution
 
@@ -46,44 +47,47 @@
 )
 parser.add_argument(
     "-e",
     "--end",
     type=datetime.fromisoformat,
     help="Date where the data should end (ISO format)",
 )
+parser.add_argument(
+    "-v", "--verbose", help="increase output verbosity", action="store_true"
+)
 
 
 async def main(
     user, password, country, brand, data=False, resolution=None, start=None, end=None
 ):
     async with MyPyllantAPI(user, password, country, brand) as api:
         async for system in api.get_systems():
             if data:
-                data_list = [
-                    {
-                        "device": d.dict()
-                        | {
-                            "data": [
-                                d
-                                async for d in api.get_data_by_device(
-                                    d, resolution, start, end
-                                )
-                            ]
-                        }
-                    }
-                    async for d in api.get_devices_by_system(system)
-                ]
+                data_list = []
+                for device in system.devices:
+                    data = [
+                        d.dict()
+                        async for d in api.get_data_by_device(
+                            device, resolution, start, end
+                        )
+                    ]
+                    data_list.append(dict(device=device.dict(), data=data))
                 sys.stdout.write(
                     json.dumps(
                         data_list,
                         indent=2,
                         default=str,
                     )
                 )
             else:
                 sys.stdout.write(json.dumps(system.dict(), indent=2, default=str))
                 sys.stdout.write("\n")
 
 
 if __name__ == "__main__":
     args = parser.parse_args()
-    asyncio.run(main(**vars(args)))
+    kwargs = vars(args)
+    verbose = kwargs.pop("verbose")
+    if verbose:
+        logging.basicConfig(level=logging.DEBUG)
+
+    asyncio.run(main(**kwargs))
```

### Comparing `mypyllant-0.2.3/src/myPyllant/models.py` & `mypyllant-0.3.0/src/myPyllant/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import datetime
+import json
 import logging
+from collections.abc import Iterator
 from enum import Enum
-from typing import Any
+from typing import Any, Optional
 
 from pydantic import BaseModel
 
+from myPyllant.utils import datetime_parse
+
 logger = logging.getLogger(__name__)
 
 
 class MyPyllantEnum(Enum):
     def __str__(self):
         """
         Return 'HOUR' instead of 'DeviceDataBucketResolution.HOUR'
@@ -55,28 +59,61 @@
 
 class DHWOperationMode(MyPyllantEnum):
     MANUAL = "MANUAL"
     TIME_CONTROLLED = "TIME_CONTROLLED"
     OFF = "OFF"
 
 
+class Claim(BaseModel):
+    country_code: str
+    nomenclature: str
+    serial_number: str
+    state: str
+    system_id: str
+
+
+class ZoneHeating(BaseModel):
+    manual_mode_setpoint_heating: float
+    operation_mode_heating: ZoneHeatingOperatingMode
+    time_program_heating: dict
+    set_back_temperature: float
+
+
 class Zone(BaseModel):
     system_id: str
-    name: str
+    general: dict
     index: int
-    active: bool
+    is_active: bool
+    is_cooling_allowed: bool
+    zone_binding: str
     current_room_temperature: float | None
     current_special_function: ZoneCurrentSpecialFunction
+    desired_room_temperature_setpoint_heating: float
     desired_room_temperature_setpoint: float
-    manual_mode_setpoint: float
-    heating_operation_mode: ZoneHeatingOperatingMode
     heating_state: ZoneHeatingState
-    humidity: float | None
-    set_back_temperature: float
-    time_windows: dict
+    current_room_humidity: float | None
+    heating: ZoneHeating
+    associated_circuit_index: int | None
+    quick_veto_start_date_time: datetime.datetime | None
+    quick_veto_end_date_time: datetime.datetime | None
+
+    def __init__(self, **data: Any):
+        if "quick_veto_start_date_time" in data:
+            data["quick_veto_start_date_time"] = datetime_parse(
+                data["quick_veto_start_date_time"]
+            )
+        if "quick_veto_end_date_time" in data:
+            data["quick_veto_end_date_time"] = datetime_parse(
+                data["quick_veto_end_date_time"]
+            )
+        super().__init__(**data)
+
+    @property
+    def name(self):
+        return self.general["name"]
 
 
 class Circuit(BaseModel):
     system_id: str
     index: int
     circuit_state: CircuitState
     current_circuit_flow_temperature: float | None
@@ -87,164 +124,132 @@
     set_back_mode_enabled: bool
     zones: list = []
 
 
 class DomesticHotWater(BaseModel):
     system_id: str
     index: int
-    current_dhw_tank_temperature: float | None
+    current_dhw_temperature: float | None
     current_special_function: DHWCurrentSpecialFunction
-    max_set_point: float
-    min_set_point: float
-    operation_mode: DHWOperationMode
-    set_point: float
-    time_windows: dict
+    max_setpoint: float
+    min_setpoint: float
+    operation_mode_dhw: DHWOperationMode
+    tapping_setpoint: float
+    time_program_dhw: dict
+    time_program_circulation_pump: dict
 
 
 class System(BaseModel):
     id: str
-    status: dict[str, bool]
-    devices: list["SystemDevice"]
+    claim: Claim | None
     current_system: dict = {}
-    system_configuration: dict = {}
-    system_control_state: dict = {}
-    gateway: dict = {}
-    has_ownership: bool
+    state: dict
+    properties: dict
+    configuration: dict
     zones: list[Zone] = []
     circuits: list[Circuit] = []
     domestic_hot_water: list[DomesticHotWater] = []
+    devices: list["Device"] = []
 
     def __init__(self, **data: Any) -> None:
-        if len(data["devices"]) > 0 and isinstance(data["devices"][0], dict):
-            data["devices"] = [SystemDevice(**d) for d in data.pop("devices")]
+        if "claim" in data and "id" not in data:
+            data["id"] = data["claim"].system_id
         super().__init__(**data)
-        logger.debug(
-            f'Creating related models from control_state: {self.system_control_state["control_state"]}'
-        )
-        self.zones = [Zone(system_id=self.id, **z) for z in self._raw_zones]
-        self.circuits = [Circuit(system_id=self.id, **c) for c in self._raw_circuits]
+        logger.debug(f"Creating related models from state: {data}")
+        self.zones = [Zone(system_id=self.id, **z) for z in self._merged_zones]
+        self.circuits = [Circuit(system_id=self.id, **c) for c in self._merged_circuits]
         self.domestic_hot_water = [
             DomesticHotWater(system_id=self.id, **d)
-            for d in self._raw_domestic_hot_water
+            for d in self._merged_domestic_hot_water
+        ]
+        self.devices = [
+            Device(system_id=self.id, type=k, **v) for k, v in self._raw_devices
         ]
 
     @property
-    def _raw_zones(self) -> list:
-        try:
-            return self.system_control_state["control_state"].get("zones", [])
-        except KeyError:
-            logger.info("Could not get zones from system control state")
-            return []
+    def _raw_devices(self) -> Iterator[tuple[str, dict]]:
+        for key, device in self.current_system.items():
+            if isinstance(device, dict) and "device_uuid" in device:
+                yield key, device
+
+    @property
+    def primary_heat_generator(self) -> Optional["Device"]:
+        devices = [d for d in self.devices if d.type == "primary_heat_generator"]
+        if len(devices) > 0:
+            return devices[0]
+        return None
+
+    def _merge_object(self, obj_name) -> Iterator[dict]:
+        indexes = [o["index"] for o in self.configuration.get(obj_name, [])]
+        for idx in indexes:
+            configuration = [
+                c for c in self.configuration.get(obj_name, []) if c["index"] == idx
+            ][0]
+            state = [c for c in self.state.get(obj_name, []) if c["index"] == idx][0]
+            properties = [
+                c for c in self.properties.get(obj_name, []) if c["index"] == idx
+            ][0]
+            del state["index"]
+            del properties["index"]
+            logger.debug(
+                f"Merging {obj_name} into results: {json.dumps(configuration, indent=2)}"
+            )
+            logger.debug(json.dumps(state, indent=2))
+            logger.debug(json.dumps(properties, indent=2))
+            merged = dict(**state, **properties, **configuration)
+            yield merged
 
     @property
-    def _raw_circuits(self) -> list:
-        try:
-            return self.system_control_state["control_state"].get("circuits", [])
-        except KeyError:
-            logger.info("Could not get circuits from system control state")
-            return []
+    def _merged_zones(self) -> Iterator[dict]:
+        return self._merge_object("zones")
 
     @property
-    def _raw_domestic_hot_water(self) -> list:
-        try:
-            return self.system_control_state["control_state"].get(
-                "domestic_hot_water", []
-            )
-        except KeyError:
-            logger.info("Could not get domestic hot water from system control state")
-            return []
+    def _merged_circuits(self) -> Iterator[dict]:
+        return self._merge_object("circuits")
+
+    @property
+    def _merged_domestic_hot_water(self) -> Iterator[dict]:
+        return self._merge_object("dhw")
 
     @property
     def outdoor_temperature(self) -> float | None:
         try:
-            return self.system_control_state["control_state"]["general"][
-                "outdoor_temperature"
-            ]
+            return self.state["system"]["outdoor_temperature"]
         except KeyError:
             logger.info(
                 "Could not get outdoor temperature from system control state",
             )
             return None
 
     @property
-    def status_online(self) -> bool | None:
-        return self.status["online"] if "online" in self.status else None
-
-    @property
-    def status_error(self) -> bool | None:
-        return self.status["error"] if "error" in self.status else None
-
-    @property
     def water_pressure(self) -> float | None:
         try:
-            return self.system_control_state["control_state"]["general"][
-                "system_water_pressure"
-            ]
+            return self.state["system"]["system_water_pressure"]
         except KeyError:
             logger.info("Could not get water pressure from system control state")
             return None
 
-    @property
-    def mode(self) -> str | None:
-        try:
-            return self.system_control_state["control_state"]["general"]["system_mode"]
-        except KeyError:
-            logger.info("Could not get mode from system control state")
-            return None
-
-
-class SystemDevice(BaseModel):
-    """
-    The System contains some information about devices already, this is saved in SystemDevice
-    The currentSystem API call returns more device info, which is saved in Device
-    """
 
+class Device(BaseModel):
     system_id: str
-    device_id: str | None
-    name: str = ""
-    type: str = ""
-    diagnostic_trouble_codes: list = []
-    properties: list = []
-    serial_number: str | None
-    article_number: str | None
-    operational_data: dict = {}
-    data: list["DeviceData"] = []
-
-    @property
-    def name_display(self) -> str:
-        if self.name:
-            return self.name
-        elif self.device_id:
-            return f"Device {self.device_id}"
-        elif self.serial_number:
-            return f"Device {self.serial_number}"
-        else:
-            return "System Device"
-
-
-class Device(SystemDevice):
-    system: System
     device_uuid: str
     name: str = ""
     product_name: str
     diagnostic_trouble_codes: list = []
     properties: list = []
     ebus_id: str
     article_number: str
     device_serial_number: str
+    type: str
     device_type: str
     first_data: datetime.datetime
     last_data: datetime.datetime
     operational_data: dict = {}
     data: list["DeviceData"] = []
 
-    def __init__(self, **data):
-        data["system_id"] = data["system"].id
-        super().__init__(**data)
-
     @property
     def name_display(self) -> str:
         return self.name if self.name else self.product_name.title()
 
 
 class DeviceDataBucket(BaseModel):
     start_date: datetime.datetime
```

### Comparing `mypyllant-0.2.3/src/myPyllant/sample.py` & `mypyllant-0.3.0/src/myPyllant/sample.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
 
 import argparse
 import asyncio
+import logging
 from datetime import datetime, timedelta
 
 from myPyllant.api import MyPyllantAPI
 from myPyllant.const import BRANDS, COUNTRIES, DEFAULT_BRAND
 
 parser = argparse.ArgumentParser(description="Export data from myVaillant API   .")
 parser.add_argument("user", help="Username (email address) for the myVaillant app")
@@ -17,25 +18,30 @@
 )
 parser.add_argument(
     "brand",
     help="Brand your account is registered in, i.e. 'vaillant'",
     default=DEFAULT_BRAND,
     choices=BRANDS.keys(),
 )
+parser.add_argument(
+    "-v", "--verbose", help="increase output verbosity", action="store_true"
+)
 
 
 async def main(user, password, country, brand):
     async with MyPyllantAPI(user, password, country, brand) as api:
         async for system in api.get_systems():
+            print(await api.get_time_zone(system))
             print(await api.set_holiday(system))
             print(
                 await api.set_holiday(
                     system, datetime.now(), datetime.now() + timedelta(days=7)
                 )
             )
+            print(await api.get_time_zone(system))
             print(await api.cancel_holiday(system))
             print(await api.boost_domestic_hot_water(system.domestic_hot_water[0]))
             print(await api.cancel_hot_water_boost(system.domestic_hot_water[0]))
             print(
                 await api.set_domestic_hot_water_temperature(
                     system.domestic_hot_water[0], 46
                 )
@@ -43,8 +49,10 @@
             print(await api.set_set_back_temperature(system.zones[0], 15.5))
             print(await api.quick_veto_zone_temperature(system.zones[0], 21, 5))
             print(await api.cancel_quick_veto_zone_temperature(system.zones[0]))
 
 
 if __name__ == "__main__":
     args = parser.parse_args()
+    if args.verbose:
+        logging.basicConfig(level=logging.DEBUG)
     asyncio.run(main(args.user, args.password, args.country, args.brand))
```

### Comparing `mypyllant-0.2.3/src/myPyllant/utils.py` & `mypyllant-0.3.0/src/myPyllant/utils.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.3/src/myPyllant/tests/find_countries.py` & `mypyllant-0.3.0/src/myPyllant/tests/find_countries.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.3/src/myPyllant/tests/generate_test_data.py` & `mypyllant-0.3.0/src/myPyllant/tests/generate_test_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import argparse
 import asyncio
 import copy
 import hashlib
 import json
 import logging
 import secrets
+import signal
+import sys
 from datetime import datetime, timedelta
 from pathlib import Path
 from urllib.parse import urlencode
 
 from myPyllant.const import BRANDS, COUNTRIES, DEFAULT_BRAND
 
 logger = logging.getLogger(__name__)
@@ -43,14 +45,21 @@
     "device_serial_number",
     "deviceId",
     "serialNumber",
     "systemId",
 )
 
 
+def user_json_dir(user: str) -> Path:
+    return (
+        JSON_DIR
+        / hashlib.sha1(user.encode("UTF-8") + SALT, usedforsecurity=False).hexdigest()
+    )
+
+
 async def main(user, password, country, brand):
     """
     Generate json data for running testcases.
 
     :param user:
     :param password:
     :param country:
@@ -58,63 +67,95 @@
     :return:
     """
     from myPyllant.api import MyPyllantAPI
     from myPyllant.const import API_URL_BASE
     from myPyllant.models import DeviceDataBucketResolution
     from myPyllant.utils import datetime_format
 
-    user_json_dir = (
-        JSON_DIR
-        / hashlib.sha1(user.encode("UTF-8") + SALT, usedforsecurity=False).hexdigest()
-    )
-    user_json_dir.mkdir(parents=True, exist_ok=True)
+    json_dir = user_json_dir(user)
+    json_dir.mkdir(parents=True, exist_ok=True)
 
     async with MyPyllantAPI(user, password, country, brand) as api:
-        systems_url = f"{API_URL_BASE}/systems"
+        claims_url = f"{API_URL_BASE}/claims"
         async with api.aiohttp_session.get(
-            systems_url, headers=api.get_authorized_headers()
-        ) as systems_resp:
-            system = await systems_resp.json()
-            with open(user_json_dir / "systems.json", "w") as fh:
+            claims_url, headers=api.get_authorized_headers()
+        ) as claims_resp:
+            claims = await claims_resp.json()
+            with open(json_dir / "claims.json", "w") as fh:
                 anonymized_system = _recursive_data_anonymize(
-                    copy.deepcopy(system), SALT
+                    copy.deepcopy(claims), SALT
                 )
                 fh.write(json.dumps(anonymized_system, indent=2))
 
-        system_url = f"{API_URL_BASE}/emf/v2/{system[0]['systemId']}/currentSystem"
+        control_identifier_url = f"{API_URL_BASE}/systems/{claims[0]['systemId']}/meta-info/control-identifier"
+        async with api.aiohttp_session.get(
+            control_identifier_url, headers=api.get_authorized_headers()
+        ) as ci_response:
+            with open(json_dir / "control_identifier.json", "w") as fh:
+                control_identifier = await ci_response.json()
+                fh.write(json.dumps(control_identifier, indent=2))
+
+        tz_url = f"{API_URL_BASE}/systems/{claims[0]['systemId']}/meta-info/time-zone"
+        async with api.aiohttp_session.get(
+            tz_url, headers=api.get_authorized_headers()
+        ) as tz_response:
+            with open(json_dir / "time_zone.json", "w") as fh:
+                fh.write(json.dumps(await tz_response.json(), indent=2))
+
+        connection_status_url = f"{API_URL_BASE}/systems/{claims[0]['systemId']}/meta-info/connection-status"
+        async with api.aiohttp_session.get(
+            connection_status_url, headers=api.get_authorized_headers()
+        ) as status_resp:
+            with open(json_dir / "connection_status.json", "w") as fh:
+                fh.write(json.dumps(await status_resp.json(), indent=2))
+
+        system_url = f"{API_URL_BASE}/systems/{claims[0]['systemId']}/{control_identifier['controlIdentifier']}"
         async with api.aiohttp_session.get(
             system_url, headers=api.get_authorized_headers()
+        ) as system_resp:
+            with open(json_dir / "system.json", "w") as fh:
+                system = await system_resp.json()
+                anonymized_system = _recursive_data_anonymize(
+                    copy.deepcopy(system), SALT
+                )
+                fh.write(json.dumps(anonymized_system, indent=2))
+
+        current_system_url = (
+            f"{API_URL_BASE}/emf/v2/{claims[0]['systemId']}/currentSystem"
+        )
+        async with api.aiohttp_session.get(
+            current_system_url, headers=api.get_authorized_headers()
         ) as current_system_resp:
-            with open(user_json_dir / "current_system.json", "w") as fh:
+            with open(json_dir / "current_system.json", "w") as fh:
                 current_system = await current_system_resp.json()
                 anonymized_current_system = _recursive_data_anonymize(
                     copy.deepcopy(current_system), SALT
                 )
                 fh.write(json.dumps(anonymized_current_system, indent=2))
 
         device = current_system["primary_heat_generator"]
         start = datetime.now().replace(
             microsecond=0, second=0, minute=0, hour=0
         ) - timedelta(days=1)
         end = datetime.now().replace(microsecond=0, second=0, minute=0, hour=0)
         querystring = {
-            "resolution": DeviceDataBucketResolution.DAY,
+            "resolution": DeviceDataBucketResolution.HOUR,
             "operationMode": device["data"][0]["operation_mode"],
             "energyType": device["data"][0]["value_type"],
             "startDate": datetime_format(start),
             "endDate": datetime_format(end),
         }
         device_buckets_url = (
-            f"{API_URL_BASE}/emf/v2/{system[0]['systemId']}/"
+            f"{API_URL_BASE}/emf/v2/{claims[0]['systemId']}/"
             f"devices/{device['device_uuid']}/buckets?{urlencode(querystring)}"
         )
         async with api.aiohttp_session.get(
             device_buckets_url, headers=api.get_authorized_headers()
         ) as device_buckets_resp:
-            with open(user_json_dir / "device_buckets.json", "w") as fh:
+            with open(json_dir / "device_buckets.json", "w") as fh:
                 device_buckets = await device_buckets_resp.json()
                 fh.write(json.dumps(device_buckets, indent=2))
 
 
 def _recursive_data_anonymize(
     data: str | dict | list, salt: bytes = b""
 ) -> str | dict | list:
@@ -134,8 +175,15 @@
     return data
 
 
 if __name__ == "__main__":
     args = parser.parse_args()
     if args.debug:
         logging.basicConfig(level="DEBUG")
+
+    def signal_handler(sig, frame):
+        user_json_dir(args.user).rmdir()
+        sys.exit(sig)
+
+    signal.signal(signal.SIGINT, signal_handler)
+
     asyncio.run(main(args.user, args.password, args.country, args.brand))
```

### Comparing `mypyllant-0.2.3/src/myPyllant/tests/test_api.py` & `mypyllant-0.3.0/src/myPyllant/tests/test_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import json
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, tzinfo
 
 import pytest
 from freezegun import freeze_time
 
 from myPyllant.api import MyPyllantAPI
-from myPyllant.export import main as export_main
 from myPyllant.models import (
     Device,
     DeviceData,
     DeviceDataBucket,
     System,
     Zone,
     ZoneCurrentSpecialFunction,
@@ -52,54 +51,69 @@
 
 @pytest.mark.parametrize("test_data", get_test_data())
 async def test_systems(mypyllant_aioresponses, mocked_api, test_data) -> None:
     with mypyllant_aioresponses(test_data) as _:
         system = await anext(mocked_api.get_systems())
 
         assert isinstance(system, System), "Expected System return type"
-        assert isinstance(system.status_online, bool)
-        assert isinstance(system.status_error, bool)
         assert isinstance(system.outdoor_temperature, (float | None))
-        assert isinstance(system.mode, str)
         assert isinstance(system.water_pressure, float)
         await mocked_api.aiohttp_session.close()
 
 
 @pytest.mark.parametrize("test_data", get_test_data())
+async def test_meta_info(mypyllant_aioresponses, mocked_api, test_data) -> None:
+    with mypyllant_aioresponses(test_data) as _:
+        system = await anext(mocked_api.get_systems())
+        status = await mocked_api.get_connection_status(system)
+        assert isinstance(status, bool)
+        time_zone = await mocked_api.get_time_zone(system)
+        assert isinstance(time_zone, tzinfo)
+        await mocked_api.aiohttp_session.close()
+
+
+@pytest.mark.parametrize("test_data", get_test_data())
+async def test_meta_info_system_id(
+    mypyllant_aioresponses, mocked_api, test_data
+) -> None:
+    with mypyllant_aioresponses(test_data) as _:
+        system = await anext(mocked_api.get_systems())
+        control_identifier = await mocked_api.get_control_identifier(system.id)
+        assert isinstance(control_identifier, str)
+        status = await mocked_api.get_connection_status(system.id)
+        assert isinstance(status, bool)
+        time_zone = await mocked_api.get_time_zone(system.id)
+        assert isinstance(time_zone, tzinfo)
+        await mocked_api.aiohttp_session.close()
+
+
+@pytest.mark.parametrize("test_data", get_test_data())
 async def test_devices(mypyllant_aioresponses, mocked_api, test_data) -> None:
     with mypyllant_aioresponses(test_data) as _:
         system = await anext(mocked_api.get_systems())
-        device = await anext(mocked_api.get_devices_by_system(system))
+        device = system.devices[0]
 
         assert isinstance(device, Device)
         assert isinstance(device.name_display, str)
         await mocked_api.aiohttp_session.close()
 
 
 @pytest.mark.parametrize("test_data", get_test_data())
 async def test_device_data(mypyllant_aioresponses, mocked_api, test_data) -> None:
     with mypyllant_aioresponses(test_data) as _:
         system = await anext(mocked_api.get_systems())
-        device = await anext(mocked_api.get_devices_by_system(system))
+        device = system.devices[0]
         device_data = await anext(mocked_api.get_data_by_device(device))
 
         assert isinstance(device_data, DeviceData)
         assert isinstance(device_data.data[0], DeviceDataBucket)
         await mocked_api.aiohttp_session.close()
 
 
 @pytest.mark.parametrize("test_data", get_test_data())
-async def test_export(mypyllant_aioresponses, capsys, test_data) -> None:
-    with mypyllant_aioresponses(test_data) as _:
-        await export_main("test@example.com", "test", "germany", "vaillant")
-        captured = capsys.readouterr()
-        assert isinstance(json.loads(captured.out), dict)
-
-
-@pytest.mark.parametrize("test_data", get_test_data())
 async def test_quick_veto(mypyllant_aioresponses, mocked_api, test_data) -> None:
     with mypyllant_aioresponses(test_data) as aio:
         system = await anext(mocked_api.get_systems())
         zone: Zone = system.zones[0]
         # Activating quick veto
         zone.current_special_function = ZoneCurrentSpecialFunction.NONE
         await mocked_api.quick_veto_zone_temperature(zone, 20.0)
```

### Comparing `mypyllant-0.2.3/src/myPyllant/tests/test_countries.py` & `mypyllant-0.3.0/src/myPyllant/tests/test_countries.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.3/src/myPyllant/tests/test_generate_test_data.py` & `mypyllant-0.3.0/src/myPyllant/tests/test_generate_test_data.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.3/src/myPyllant/tests/update_sample.py` & `mypyllant-0.3.0/src/myPyllant/tests/update_sample.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.3/src/myPyllant/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/systems.json` & `mypyllant-0.3.0/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/system.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('state', OrderedDict([('system', OrderedDict([('outdoorTemperature', "*

 * *            "15.199219), ('systemWaterPressure', 1.1)])), ('zones', [OrderedDict([('index', 0), "*

 * *            "('desiredRoomTemperatureSetpointHeating', 20.5), ('desiredRoomTemperatureSetpoint', "*

 * *            "20.5), ('currentRoomTemperature', 20.35), ('currentRoomHumidity', 60.0), "*

 * *            "('currentSpecialFunction', 'QUICK_VETO'), ('heatingState', 'HEATING_UP'), "*

 * *            "('quickVetoStartDateTime',  […]*

```diff
@@ -1,215 +1,247 @@
-[
-    {
-        "devices": [
-            {
-                "articleNumber": "0020260951",
-                "deviceId": "efe2e60090348d9946d94b7aee1f73c8e84d9ed9",
-                "diagnosticTroubleCodes": [],
-                "name": "sensoHOME",
-                "serialNumber": "5e382a467a1f1515ecb191c9734135a01836593d",
-                "systemId": "35b6c3ca1d6131af0505e674b55c0976069170ee",
-                "type": "CONTROL"
-            },
-            {
-                "articleNumber": "0010022040",
-                "deviceId": "1441dd725ae6f7555633c6f76cca1eee8cf9f388",
-                "diagnosticTroubleCodes": [],
-                "name": "ecoTEC",
-                "operationalData": {
-                    "waterPressure": {
-                        "stepSize": 0.1,
-                        "unit": "BAR",
-                        "value": 2.0
-                    }
-                },
-                "properties": [
-                    "EMF"
-                ],
-                "serialNumber": "7f78b8657f10d635161a070c71a7c6cc0cefc316",
-                "systemId": "35b6c3ca1d6131af0505e674b55c0976069170ee",
-                "type": "HEAT_GENERATOR"
+{
+    "configuration": {
+        "circuits": [
+            {
+                "heatingCurve": 0.5549309,
+                "heatingFlowTemperatureMinimumSetpoint": 35.0,
+                "index": 0,
+                "setBackModeEnabled": false
             }
         ],
-        "gateway": {
-            "deviceId": "92be1ee4ab00440ffbc781682d234faa6489dc3e",
-            "diagnosticTroubleCodes": [],
-            "serialNumber": "0d07c8a809d56aef4c41e4c7023965634cf71274",
-            "systemId": "35b6c3ca1d6131af0505e674b55c0976069170ee"
-        },
-        "hasOwnership": true,
-        "status": {
-            "error": false,
-            "online": true
-        },
-        "systemConfiguration": {
-            "timeZoneId": "Europe/Madrid"
-        },
-        "systemControlState": {
-            "controlIdentifier": "TLI",
-            "controlState": {
-                "circuits": [
-                    {
-                        "circuitState": "HEATING",
-                        "currentCircuitFlowTemperature": 37.5,
-                        "index": 0,
-                        "isCoolingAllowed": false,
-                        "mixerCircuitTypeExternal": "HEATING",
-                        "setBackModeEnabled": false,
-                        "zones": []
-                    }
-                ],
-                "domesticHotWater": [
-                    {
-                        "currentSpecialFunction": "REGULAR",
-                        "index": 255,
-                        "maxSetPoint": 65.0,
-                        "minSetPoint": 35.0,
-                        "operationMode": "TIME_CONTROLLED",
-                        "setPoint": 45.0,
-                        "timeWindows": {
-                            "dhw": {
-                                "friday": [
-                                    {
-                                        "endTime": "22:00",
-                                        "startTime": "05:30"
-                                    }
-                                ],
-                                "metaInfo": {
-                                    "maxSlotsPerDay": 3,
-                                    "minSlotsPerDay": 0,
-                                    "setPointRequiredPerSlot": false
-                                },
-                                "monday": [
-                                    {
-                                        "endTime": "22:00",
-                                        "startTime": "05:30"
-                                    }
-                                ],
-                                "saturday": [
-                                    {
-                                        "endTime": "23:30",
-                                        "startTime": "07:00"
-                                    }
-                                ],
-                                "sunday": [
-                                    {
-                                        "endTime": "22:00",
-                                        "startTime": "07:00"
-                                    }
-                                ],
-                                "thursday": [
-                                    {
-                                        "endTime": "22:00",
-                                        "startTime": "05:30"
-                                    }
-                                ],
-                                "tuesday": [
-                                    {
-                                        "endTime": "22:00",
-                                        "startTime": "05:30"
-                                    }
-                                ],
-                                "wednesday": [
-                                    {
-                                        "endTime": "22:00",
-                                        "startTime": "05:30"
-                                    }
-                                ]
-                            }
+        "dhw": [
+            {
+                "index": 255,
+                "operationModeDhw": "TIME_CONTROLLED",
+                "tappingSetpoint": 49.0,
+                "timeProgramCirculationPump": {
+                    "friday": [
+                        {
+                            "endTime": 1320,
+                            "startTime": 360
                         }
-                    }
-                ],
-                "general": {
-                    "systemMode": "REGULAR",
-                    "systemWaterPressure": 2.0
+                    ],
+                    "metaInfo": {
+                        "maxSlotsPerDay": 3,
+                        "minSlotsPerDay": 0,
+                        "setpointRequiredPerSlot": false
+                    },
+                    "monday": [
+                        {
+                            "endTime": 1320,
+                            "startTime": 360
+                        }
+                    ],
+                    "saturday": [
+                        {
+                            "endTime": 1410,
+                            "startTime": 450
+                        }
+                    ],
+                    "sunday": [
+                        {
+                            "endTime": 1320,
+                            "startTime": 450
+                        }
+                    ],
+                    "thursday": [
+                        {
+                            "endTime": 1320,
+                            "startTime": 360
+                        }
+                    ],
+                    "tuesday": [
+                        {
+                            "endTime": 1320,
+                            "startTime": 360
+                        }
+                    ],
+                    "wednesday": [
+                        {
+                            "endTime": 1320,
+                            "startTime": 360
+                        }
+                    ]
                 },
-                "properties": {
-                    "circuits": [
+                "timeProgramDhw": {
+                    "friday": [
                         {
-                            "index": 0,
-                            "isCoolingAllowed": false,
-                            "mixerCircuitTypeExternal": "HEATING"
+                            "endTime": 1260,
+                            "startTime": 330
                         }
                     ],
-                    "controlType": "VRT380",
-                    "general": {
-                        "isCoolingAllowed": false
-                    }
+                    "metaInfo": {
+                        "maxSlotsPerDay": 3,
+                        "minSlotsPerDay": 0,
+                        "setpointRequiredPerSlot": false
+                    },
+                    "monday": [
+                        {
+                            "endTime": 1260,
+                            "startTime": 330
+                        }
+                    ],
+                    "saturday": [
+                        {
+                            "endTime": 1260,
+                            "startTime": 450
+                        }
+                    ],
+                    "sunday": [
+                        {
+                            "endTime": 1260,
+                            "startTime": 450
+                        }
+                    ],
+                    "thursday": [
+                        {
+                            "endTime": 1260,
+                            "startTime": 330
+                        }
+                    ],
+                    "tuesday": [
+                        {
+                            "endTime": 1260,
+                            "startTime": 330
+                        }
+                    ],
+                    "wednesday": [
+                        {
+                            "endTime": 1260,
+                            "startTime": 330
+                        }
+                    ]
+                }
+            }
+        ],
+        "zones": [
+            {
+                "general": {
+                    "name": "Zone 1"
                 },
-                "zones": [
-                    {
-                        "active": true,
-                        "currentRoomTemperature": 18.5,
-                        "currentSpecialFunction": "NONE",
-                        "desiredRoomTemperatureSetpoint": 18.0,
-                        "heatingOperationMode": "TIME_CONTROLLED",
-                        "heatingState": "IDLE",
-                        "index": 0,
-                        "manualModeSetpoint": 18.0,
-                        "name": "Zone 1",
-                        "setBackTemperature": 14.0,
-                        "timeWindows": {
-                            "heating": {
-                                "friday": [
-                                    {
-                                        "endTime": "20:00",
-                                        "setPoint": 18.0,
-                                        "startTime": "07:30"
-                                    }
-                                ],
-                                "metaInfo": {
-                                    "maxSlotsPerDay": 12,
-                                    "minSlotsPerDay": 0,
-                                    "setPointRequiredPerSlot": true
-                                },
-                                "monday": [
-                                    {
-                                        "endTime": "20:00",
-                                        "setPoint": 18.0,
-                                        "startTime": "07:30"
-                                    }
-                                ],
-                                "saturday": [
-                                    {
-                                        "endTime": "20:00",
-                                        "setPoint": 18.0,
-                                        "startTime": "07:30"
-                                    }
-                                ],
-                                "sunday": [
-                                    {
-                                        "endTime": "20:00",
-                                        "setPoint": 18.0,
-                                        "startTime": "07:30"
-                                    }
-                                ],
-                                "thursday": [
-                                    {
-                                        "endTime": "20:00",
-                                        "setPoint": 18.0,
-                                        "startTime": "07:30"
-                                    }
-                                ],
-                                "tuesday": [
-                                    {
-                                        "endTime": "20:00",
-                                        "setPoint": 18.0,
-                                        "startTime": "07:30"
-                                    }
-                                ],
-                                "wednesday": [
-                                    {
-                                        "endTime": "20:00",
-                                        "setPoint": 18.0,
-                                        "startTime": "07:30"
-                                    }
-                                ]
+                "heating": {
+                    "manualModeSetpointHeating": 21.0,
+                    "operationModeHeating": "TIME_CONTROLLED",
+                    "setBackTemperature": 15.5,
+                    "timeProgramHeating": {
+                        "friday": [
+                            {
+                                "endTime": 1290,
+                                "setpoint": 19.5,
+                                "startTime": 420
                             }
-                        }
+                        ],
+                        "metaInfo": {
+                            "maxSlotsPerDay": 12,
+                            "minSlotsPerDay": 0,
+                            "setpointRequiredPerSlot": true
+                        },
+                        "monday": [
+                            {
+                                "endTime": 1290,
+                                "setpoint": 19.5,
+                                "startTime": 420
+                            }
+                        ],
+                        "saturday": [
+                            {
+                                "endTime": 1290,
+                                "setpoint": 19.5,
+                                "startTime": 450
+                            }
+                        ],
+                        "sunday": [
+                            {
+                                "endTime": 1290,
+                                "setpoint": 19.5,
+                                "startTime": 450
+                            }
+                        ],
+                        "thursday": [
+                            {
+                                "endTime": 1290,
+                                "setpoint": 19.5,
+                                "startTime": 420
+                            }
+                        ],
+                        "tuesday": [
+                            {
+                                "endTime": 1290,
+                                "setpoint": 19.5,
+                                "startTime": 420
+                            }
+                        ],
+                        "wednesday": [
+                            {
+                                "endTime": 1290,
+                                "setpoint": 19.5,
+                                "startTime": 420
+                            }
+                        ]
                     }
-                ]
+                },
+                "index": 0
+            }
+        ]
+    },
+    "properties": {
+        "circuits": [
+            {
+                "index": 0,
+                "isCoolingAllowed": false,
+                "mixerCircuitTypeExternal": "HEATING"
+            }
+        ],
+        "dhw": [
+            {
+                "index": 255,
+                "maxSetpoint": 70.0,
+                "minSetpoint": 35.0
             }
+        ],
+        "system": {
+            "controllerType": "VRC720"
         },
-        "systemId": "35b6c3ca1d6131af0505e674b55c0976069170ee"
+        "zones": [
+            {
+                "associatedCircuitIndex": 0,
+                "index": 0,
+                "isActive": true,
+                "isCoolingAllowed": false,
+                "zoneBinding": "CENTRAL_CONTROL"
+            }
+        ]
+    },
+    "state": {
+        "circuits": [
+            {
+                "circuitState": "HEATING",
+                "currentCircuitFlowTemperature": 52.5,
+                "index": 0
+            }
+        ],
+        "dhw": [
+            {
+                "currentDhwTemperature": 45.5,
+                "currentSpecialFunction": "REGULAR",
+                "index": 255
+            }
+        ],
+        "system": {
+            "outdoorTemperature": 15.199219,
+            "systemWaterPressure": 1.1
+        },
+        "zones": [
+            {
+                "currentRoomHumidity": 60.0,
+                "currentRoomTemperature": 20.35,
+                "currentSpecialFunction": "QUICK_VETO",
+                "desiredRoomTemperatureSetpoint": 20.5,
+                "desiredRoomTemperatureSetpointHeating": 20.5,
+                "heatingState": "HEATING_UP",
+                "index": 0,
+                "quickVetoEndDateTime": "2023-04-24T12:35:00Z",
+                "quickVetoStartDateTime": "2023-04-24T09:35:28Z"
+            }
+        ]
     }
-]
+}
```

### Comparing `mypyllant-0.2.3/src/myPyllant/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/current_system.json` & `mypyllant-0.3.0/src/myPyllant/tests/json/91b3ac21d0e3060c99d117422bede91c3fe1cb51/current_system.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8386904761904762%*

 * *Differences: {"'electric_backup_heater'": "{'device_uuid': '51e8d5f067005d0731e0a347eae3d881ff492b05', "*

 * *                             "'device_serial_number': 'dac5856554b37f1755cc28f041d32417e17c2b46', "*

 * *                             "'last_data': '2023-04-24T09:51:54Z', 'data': {0: {'to': "*

 * *                             "'2023-04-24T09:51:54Z'}, 1: {'to': '2023-04-24T09:51:54Z'}}}",*

 * * "'has_emf_capable_devices'": 'True',*

 * * "'primary_heat_generator'": "{'device_uuid': 'baf4a5d5cc9d4277c54316a1dfcd9f3cbf1970de', "*

 * *          […]*

```diff
@@ -3,89 +3,90 @@
         "article_number": "0010023609",
         "bus_coupler_address": 0,
         "data": [
             {
                 "calculated": false,
                 "from": "2022-10-11T16:16:40Z",
                 "operation_mode": "DOMESTIC_HOT_WATER",
-                "to": "2023-03-10T20:20:07Z",
+                "to": "2023-04-24T09:51:54Z",
                 "value_type": "CONSUMED_ELECTRICAL_ENERGY"
             },
             {
                 "calculated": false,
                 "from": "2022-10-11T16:16:40Z",
                 "operation_mode": "HEATING",
-                "to": "2023-03-10T20:20:07Z",
+                "to": "2023-04-24T09:51:54Z",
                 "value_type": "CONSUMED_ELECTRICAL_ENERGY"
             }
         ],
-        "device_serial_number": "6b009882bd3c51826ff3ff10d8d079e9daa160ff",
+        "device_serial_number": "dac5856554b37f1755cc28f041d32417e17c2b46",
         "device_type": "ELECTRIC_AUXILIARY_HEATER",
-        "device_uuid": "9d349b068602cb1ec420ffffccf9417a7a1faf6d",
+        "device_uuid": "51e8d5f067005d0731e0a347eae3d881ff492b05",
         "ebus_id": "VWZ02",
         "emfValid": true,
         "first_data": "2022-10-11T16:16:40Z",
-        "last_data": "2023-03-10T20:20:07Z",
+        "last_data": "2023-04-24T09:51:54Z",
         "product_name": "hydraulic station",
         "spn": 351
     },
+    "has_emf_capable_devices": true,
     "primary_heat_generator": {
         "article_number": "0010021118",
         "bus_coupler_address": 0,
         "data": [
             {
                 "calculated": false,
                 "from": "2022-10-11T16:16:40Z",
                 "operation_mode": "DOMESTIC_HOT_WATER",
-                "to": "2023-03-10T20:20:05Z",
+                "to": "2023-04-24T09:51:52Z",
                 "value_type": "CONSUMED_ELECTRICAL_ENERGY"
             },
             {
                 "calculated": false,
                 "from": "2022-10-11T16:16:40Z",
                 "operation_mode": "HEATING",
-                "to": "2023-03-10T20:20:05Z",
+                "to": "2023-04-24T09:51:52Z",
                 "value_type": "CONSUMED_ELECTRICAL_ENERGY"
             },
             {
                 "calculated": false,
                 "from": "2022-10-11T16:16:40Z",
                 "operation_mode": "DOMESTIC_HOT_WATER",
-                "to": "2023-03-10T20:20:04Z",
+                "to": "2023-04-24T09:51:51Z",
                 "value_type": "EARNED_ENVIRONMENT_ENERGY"
             },
             {
                 "calculated": false,
                 "from": "2022-10-11T16:16:40Z",
                 "operation_mode": "HEATING",
-                "to": "2023-03-10T20:20:04Z",
+                "to": "2023-04-24T09:51:52Z",
                 "value_type": "EARNED_ENVIRONMENT_ENERGY"
             },
             {
                 "calculated": true,
                 "from": "2022-10-11T16:16:40Z",
                 "operation_mode": "HEATING",
-                "to": "2023-03-10T20:20:04Z",
+                "to": "2023-04-24T09:51:52Z",
                 "value_type": "HEAT_GENERATED"
             },
             {
                 "calculated": true,
                 "from": "2022-10-11T16:16:40Z",
                 "operation_mode": "DOMESTIC_HOT_WATER",
-                "to": "2023-03-10T20:20:04Z",
+                "to": "2023-04-24T09:51:51Z",
                 "value_type": "HEAT_GENERATED"
             }
         ],
-        "device_serial_number": "c44c81ac0c29f1fa713d65907708ae4cfeb73e56",
+        "device_serial_number": "761cc85068c3cb2fb11c490a81ce537dc99425d4",
         "device_type": "HEATPUMP",
-        "device_uuid": "a82a4e76cc3dede37d9050139e5b1e4db66576dd",
+        "device_uuid": "baf4a5d5cc9d4277c54316a1dfcd9f3cbf1970de",
         "ebus_id": "HMU03",
         "emfValid": true,
         "first_data": "2022-10-11T16:16:40Z",
-        "last_data": "2023-03-10T20:20:05Z",
+        "last_data": "2023-04-24T09:51:52Z",
         "product_name": "aroTHERM plus",
         "spn": 351
     },
     "secondary_heat_generators": [],
     "solar_station": null,
     "system_type": "HEATPUMP",
     "ventilation": null
```

### Comparing `mypyllant-0.2.3/.gitignore` & `mypyllant-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.3/LICENSE` & `mypyllant-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.3/README.md` & `mypyllant-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 ## Usage
 
 ```python
 #!/usr/bin/env python3
 
 import argparse
 import asyncio
+import logging
 from datetime import datetime, timedelta
 
 from myPyllant.api import MyPyllantAPI
 from myPyllant.const import BRANDS, COUNTRIES, DEFAULT_BRAND
 
 parser = argparse.ArgumentParser(description="Export data from myVaillant API   .")
 parser.add_argument("user", help="Username (email address) for the myVaillant app")
@@ -46,25 +47,30 @@
 )
 parser.add_argument(
     "brand",
     help="Brand your account is registered in, i.e. 'vaillant'",
     default=DEFAULT_BRAND,
     choices=BRANDS.keys(),
 )
+parser.add_argument(
+    "-v", "--verbose", help="increase output verbosity", action="store_true"
+)
 
 
 async def main(user, password, country, brand):
     async with MyPyllantAPI(user, password, country, brand) as api:
         async for system in api.get_systems():
+            print(await api.get_time_zone(system))
             print(await api.set_holiday(system))
             print(
                 await api.set_holiday(
                     system, datetime.now(), datetime.now() + timedelta(days=7)
                 )
             )
+            print(await api.get_time_zone(system))
             print(await api.cancel_holiday(system))
             print(await api.boost_domestic_hot_water(system.domestic_hot_water[0]))
             print(await api.cancel_hot_water_boost(system.domestic_hot_water[0]))
             print(
                 await api.set_domestic_hot_water_temperature(
                     system.domestic_hot_water[0], 46
                 )
@@ -72,14 +78,16 @@
             print(await api.set_set_back_temperature(system.zones[0], 15.5))
             print(await api.quick_veto_zone_temperature(system.zones[0], 21, 5))
             print(await api.cancel_quick_veto_zone_temperature(system.zones[0]))
 
 
 if __name__ == "__main__":
     args = parser.parse_args()
+    if args.verbose:
+        logging.basicConfig(level=logging.DEBUG)
     asyncio.run(main(args.user, args.password, args.country, args.brand))
 
 ```
 
 ### Tested Configurations
 
 See https://github.com/signalkraft/mypyllant-component/blob/main/README.md#tested-setups
@@ -103,28 +111,28 @@
 
 ### Supporting new Countries
 
 The myVAILLANT app uses Keycloak and OIDC for authentication, with a realm for each country and brand.
 There is a script to check which countries are supported:
 
 ```shell
-python3 tests/find_countries.py
+python3 -m myPyllant.tests.find_countries
 ```
 
 Copy the resulting dictionary into [src/myPyllant/const.py](src/myPyllant/const.py)
 
 ### Contributing Test Data
 
 Because the myVAILLANT API isn't documented, you can help the development of this library by contributing test data:
 
 ```shell
-python3 tests/generate_test_data.py username password country brand
+python3 -m myPyllant.tests.generate_test_data username password country brand
 ```
 
-Create a fork of this repository and create a PR with the newly created folder in `test/json`.
+Create a fork of this repository and create a PR with the newly created folder in `src/myPyllant/tests/json`.
 
 ## Notes
 
 * Auth is loosely based on https://github.com/TA2k/ioBroker.vaillant
 * Most API endpoints are reverse-engineered from the myVaillant app, using https://github.com/mitmproxy/mitmproxy
 * Setting weekly time tables for heating and domestic hot water is still missing
 * There is a home assistant component based on this library here: https://github.com/signalkraft/mypyllant-component
```

### Comparing `mypyllant-0.2.3/pyproject.toml` & `mypyllant-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.3/PKG-INFO` & `mypyllant-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myPyllant
-Version: 0.2.3
+Version: 0.3.0
 Summary: A Python library to interact with the API behind the myVAILLANT app
 Project-URL: Homepage, https://github.com/signalkraft/myPyllant
 Project-URL: Bug Tracker, https://github.com/signalkraft/myPyllant/issues
 Author-email: Philipp <pd@signalkraft.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -43,14 +43,15 @@
 ## Usage
 
 ```python
 #!/usr/bin/env python3
 
 import argparse
 import asyncio
+import logging
 from datetime import datetime, timedelta
 
 from myPyllant.api import MyPyllantAPI
 from myPyllant.const import BRANDS, COUNTRIES, DEFAULT_BRAND
 
 parser = argparse.ArgumentParser(description="Export data from myVaillant API   .")
 parser.add_argument("user", help="Username (email address) for the myVaillant app")
@@ -62,25 +63,30 @@
 )
 parser.add_argument(
     "brand",
     help="Brand your account is registered in, i.e. 'vaillant'",
     default=DEFAULT_BRAND,
     choices=BRANDS.keys(),
 )
+parser.add_argument(
+    "-v", "--verbose", help="increase output verbosity", action="store_true"
+)
 
 
 async def main(user, password, country, brand):
     async with MyPyllantAPI(user, password, country, brand) as api:
         async for system in api.get_systems():
+            print(await api.get_time_zone(system))
             print(await api.set_holiday(system))
             print(
                 await api.set_holiday(
                     system, datetime.now(), datetime.now() + timedelta(days=7)
                 )
             )
+            print(await api.get_time_zone(system))
             print(await api.cancel_holiday(system))
             print(await api.boost_domestic_hot_water(system.domestic_hot_water[0]))
             print(await api.cancel_hot_water_boost(system.domestic_hot_water[0]))
             print(
                 await api.set_domestic_hot_water_temperature(
                     system.domestic_hot_water[0], 46
                 )
@@ -88,14 +94,16 @@
             print(await api.set_set_back_temperature(system.zones[0], 15.5))
             print(await api.quick_veto_zone_temperature(system.zones[0], 21, 5))
             print(await api.cancel_quick_veto_zone_temperature(system.zones[0]))
 
 
 if __name__ == "__main__":
     args = parser.parse_args()
+    if args.verbose:
+        logging.basicConfig(level=logging.DEBUG)
     asyncio.run(main(args.user, args.password, args.country, args.brand))
 
 ```
 
 ### Tested Configurations
 
 See https://github.com/signalkraft/mypyllant-component/blob/main/README.md#tested-setups
@@ -119,28 +127,28 @@
 
 ### Supporting new Countries
 
 The myVAILLANT app uses Keycloak and OIDC for authentication, with a realm for each country and brand.
 There is a script to check which countries are supported:
 
 ```shell
-python3 tests/find_countries.py
+python3 -m myPyllant.tests.find_countries
 ```
 
 Copy the resulting dictionary into [src/myPyllant/const.py](src/myPyllant/const.py)
 
 ### Contributing Test Data
 
 Because the myVAILLANT API isn't documented, you can help the development of this library by contributing test data:
 
 ```shell
-python3 tests/generate_test_data.py username password country brand
+python3 -m myPyllant.tests.generate_test_data username password country brand
 ```
 
-Create a fork of this repository and create a PR with the newly created folder in `test/json`.
+Create a fork of this repository and create a PR with the newly created folder in `src/myPyllant/tests/json`.
 
 ## Notes
 
 * Auth is loosely based on https://github.com/TA2k/ioBroker.vaillant
 * Most API endpoints are reverse-engineered from the myVaillant app, using https://github.com/mitmproxy/mitmproxy
 * Setting weekly time tables for heating and domestic hot water is still missing
 * There is a home assistant component based on this library here: https://github.com/signalkraft/mypyllant-component
```


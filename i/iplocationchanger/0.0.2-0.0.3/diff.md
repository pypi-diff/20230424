# Comparing `tmp/iplocationchanger-0.0.2.tar.gz` & `tmp/iplocationchanger-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iplocationchanger-0.0.2.tar", last modified: Mon Apr 10 17:17:35 2023, max compression
+gzip compressed data, was "iplocationchanger-0.0.3.tar", last modified: Mon Apr 24 17:45:37 2023, max compression
```

## Comparing `iplocationchanger-0.0.2.tar` & `iplocationchanger-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,32 @@
-drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-04-10 17:17:35.650354 iplocationchanger-0.0.2/
--rw-r--r--   0 faaizz     (501) staff       (20)     1076 2023-03-01 19:20:31.000000 iplocationchanger-0.0.2/LICENSE
--rw-r--r--   0 faaizz     (501) staff       (20)     4140 2023-04-10 17:17:35.649622 iplocationchanger-0.0.2/PKG-INFO
--rw-r--r--   0 faaizz     (501) staff       (20)     2267 2023-03-31 20:37:55.000000 iplocationchanger-0.0.2/README.md
--rw-r--r--   0 faaizz     (501) staff       (20)      923 2023-04-10 17:13:33.000000 iplocationchanger-0.0.2/pyproject.toml
--rw-r--r--   0 faaizz     (501) staff       (20)       38 2023-04-10 17:17:35.650546 iplocationchanger-0.0.2/setup.cfg
-drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-04-10 17:17:35.635991 iplocationchanger-0.0.2/src/
-drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-04-10 17:17:35.639912 iplocationchanger-0.0.2/src/iplocationchanger/
--rw-r--r--   0 faaizz     (501) staff       (20)       22 2023-03-05 11:44:17.000000 iplocationchanger-0.0.2/src/iplocationchanger/__init__.py
--rw-r--r--   0 faaizz     (501) staff       (20)     2136 2023-04-10 17:02:45.000000 iplocationchanger-0.0.2/src/iplocationchanger/__main__.py
-drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-04-10 17:17:35.643853 iplocationchanger-0.0.2/src/iplocationchanger/model/
--rw-r--r--   0 faaizz     (501) staff       (20)        0 2023-03-02 20:33:14.000000 iplocationchanger-0.0.2/src/iplocationchanger/model/__init__.py
--rw-r--r--   0 faaizz     (501) staff       (20)      570 2023-03-02 21:42:30.000000 iplocationchanger-0.0.2/src/iplocationchanger/model/openvpn_credentials.py
-drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-04-10 17:17:35.647151 iplocationchanger-0.0.2/src/iplocationchanger/service/
--rw-r--r--   0 faaizz     (501) staff       (20)        0 2023-03-02 20:33:19.000000 iplocationchanger-0.0.2/src/iplocationchanger/service/__init__.py
--rw-r--r--   0 faaizz     (501) staff       (20)     1665 2023-04-10 16:40:59.000000 iplocationchanger-0.0.2/src/iplocationchanger/service/location_changer_service.py
--rw-r--r--   0 faaizz     (501) staff       (20)     1639 2023-03-05 13:31:53.000000 iplocationchanger-0.0.2/src/iplocationchanger/service/openvpn_service.py
--rw-r--r--   0 faaizz     (501) staff       (20)     1505 2023-04-09 14:25:52.000000 iplocationchanger-0.0.2/src/iplocationchanger/service/whatismyip_service.py
-drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-04-10 17:17:35.648610 iplocationchanger-0.0.2/src/iplocationchanger/utils/
--rw-r--r--   0 faaizz     (501) staff       (20)        0 2023-03-02 20:33:22.000000 iplocationchanger-0.0.2/src/iplocationchanger/utils/__init__.py
--rw-r--r--   0 faaizz     (501) staff       (20)     1492 2023-04-10 17:06:15.000000 iplocationchanger-0.0.2/src/iplocationchanger/utils/utils.py
-drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-04-10 17:17:35.642970 iplocationchanger-0.0.2/src/iplocationchanger.egg-info/
--rw-r--r--   0 faaizz     (501) staff       (20)     4140 2023-04-10 17:17:35.000000 iplocationchanger-0.0.2/src/iplocationchanger.egg-info/PKG-INFO
--rw-r--r--   0 faaizz     (501) staff       (20)      693 2023-04-10 17:17:35.000000 iplocationchanger-0.0.2/src/iplocationchanger.egg-info/SOURCES.txt
--rw-r--r--   0 faaizz     (501) staff       (20)        1 2023-04-10 17:17:35.000000 iplocationchanger-0.0.2/src/iplocationchanger.egg-info/dependency_links.txt
--rw-r--r--   0 faaizz     (501) staff       (20)       40 2023-04-10 17:17:35.000000 iplocationchanger-0.0.2/src/iplocationchanger.egg-info/requires.txt
--rw-r--r--   0 faaizz     (501) staff       (20)       18 2023-04-10 17:17:35.000000 iplocationchanger-0.0.2/src/iplocationchanger.egg-info/top_level.txt
+drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-04-24 17:45:37.936456 iplocationchanger-0.0.3/
+-rw-r--r--   0 faaizz     (501) staff       (20)     1076 2023-03-01 19:20:31.000000 iplocationchanger-0.0.3/LICENSE
+-rw-r--r--   0 faaizz     (501) staff       (20)     4234 2023-04-24 17:45:37.936014 iplocationchanger-0.0.3/PKG-INFO
+-rw-r--r--   0 faaizz     (501) staff       (20)     2361 2023-04-24 17:44:14.000000 iplocationchanger-0.0.3/README.md
+-rw-r--r--   0 faaizz     (501) staff       (20)      923 2023-04-24 17:45:08.000000 iplocationchanger-0.0.3/pyproject.toml
+-rw-r--r--   0 faaizz     (501) staff       (20)       38 2023-04-24 17:45:37.936593 iplocationchanger-0.0.3/setup.cfg
+drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-04-24 17:45:37.920349 iplocationchanger-0.0.3/src/
+drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-04-24 17:45:37.923934 iplocationchanger-0.0.3/src/iplocationchanger/
+-rw-r--r--   0 faaizz     (501) staff       (20)       22 2023-03-05 11:44:17.000000 iplocationchanger-0.0.3/src/iplocationchanger/__init__.py
+-rw-r--r--   0 faaizz     (501) staff       (20)     2264 2023-04-24 17:44:14.000000 iplocationchanger-0.0.3/src/iplocationchanger/__main__.py
+drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-04-24 17:45:37.930791 iplocationchanger-0.0.3/src/iplocationchanger/exception/
+-rw-r--r--   0 faaizz     (501) staff       (20)      106 2023-04-24 17:44:14.000000 iplocationchanger-0.0.3/src/iplocationchanger/exception/iplocationchanger_exception.py
+-rw-r--r--   0 faaizz     (501) staff       (20)      171 2023-04-24 17:44:14.000000 iplocationchanger-0.0.3/src/iplocationchanger/exception/location_changer_service_exception.py
+-rw-r--r--   0 faaizz     (501) staff       (20)      163 2023-04-24 17:44:14.000000 iplocationchanger-0.0.3/src/iplocationchanger/exception/openvpn_service_exception.py
+-rw-r--r--   0 faaizz     (501) staff       (20)      166 2023-04-24 17:44:14.000000 iplocationchanger-0.0.3/src/iplocationchanger/exception/whatismyip_service_exception.py
+drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-04-24 17:45:37.931708 iplocationchanger-0.0.3/src/iplocationchanger/model/
+-rw-r--r--   0 faaizz     (501) staff       (20)        0 2023-03-02 20:33:14.000000 iplocationchanger-0.0.3/src/iplocationchanger/model/__init__.py
+-rw-r--r--   0 faaizz     (501) staff       (20)      570 2023-03-02 21:42:30.000000 iplocationchanger-0.0.3/src/iplocationchanger/model/openvpn_credentials.py
+drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-04-24 17:45:37.933725 iplocationchanger-0.0.3/src/iplocationchanger/service/
+-rw-r--r--   0 faaizz     (501) staff       (20)        0 2023-03-02 20:33:19.000000 iplocationchanger-0.0.3/src/iplocationchanger/service/__init__.py
+-rw-r--r--   0 faaizz     (501) staff       (20)     2078 2023-04-24 17:44:14.000000 iplocationchanger-0.0.3/src/iplocationchanger/service/location_changer_service.py
+-rw-r--r--   0 faaizz     (501) staff       (20)     1839 2023-04-24 17:44:14.000000 iplocationchanger-0.0.3/src/iplocationchanger/service/openvpn_service.py
+-rw-r--r--   0 faaizz     (501) staff       (20)     3013 2023-04-24 17:44:14.000000 iplocationchanger-0.0.3/src/iplocationchanger/service/whatismyip_service.py
+drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-04-24 17:45:37.935327 iplocationchanger-0.0.3/src/iplocationchanger/utils/
+-rw-r--r--   0 faaizz     (501) staff       (20)        0 2023-03-02 20:33:22.000000 iplocationchanger-0.0.3/src/iplocationchanger/utils/__init__.py
+-rw-r--r--   0 faaizz     (501) staff       (20)      852 2023-04-24 17:44:14.000000 iplocationchanger-0.0.3/src/iplocationchanger/utils/utils.py
+drwxr-xr-x   0 faaizz     (501) staff       (20)        0 2023-04-24 17:45:37.928283 iplocationchanger-0.0.3/src/iplocationchanger.egg-info/
+-rw-r--r--   0 faaizz     (501) staff       (20)     4234 2023-04-24 17:45:37.000000 iplocationchanger-0.0.3/src/iplocationchanger.egg-info/PKG-INFO
+-rw-r--r--   0 faaizz     (501) staff       (20)      951 2023-04-24 17:45:37.000000 iplocationchanger-0.0.3/src/iplocationchanger.egg-info/SOURCES.txt
+-rw-r--r--   0 faaizz     (501) staff       (20)        1 2023-04-24 17:45:37.000000 iplocationchanger-0.0.3/src/iplocationchanger.egg-info/dependency_links.txt
+-rw-r--r--   0 faaizz     (501) staff       (20)       40 2023-04-24 17:45:37.000000 iplocationchanger-0.0.3/src/iplocationchanger.egg-info/requires.txt
+-rw-r--r--   0 faaizz     (501) staff       (20)       18 2023-04-24 17:45:37.000000 iplocationchanger-0.0.3/src/iplocationchanger.egg-info/top_level.txt
```

### Comparing `iplocationchanger-0.0.2/LICENSE` & `iplocationchanger-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `iplocationchanger-0.0.2/PKG-INFO` & `iplocationchanger-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iplocationchanger
-Version: 0.0.2
+Version: 0.0.3
 Summary: Reliable IP location changer using OpenVPN and WhatIsMyIP
 Author-email: Faizudeen Kajogbola <faizudeen@codecreek.cc>
 License: MIT License
         
         Copyright (c) 2023 Faizudeen Kajogbola
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -41,33 +41,36 @@
 Reliable IP location changer using [OpenVPN](https://openvpn.net/) and [WhatIsMyIP](https://www.whatismyip.com/).
 
 This package allows changing the IP of the host machine by using openvpn configuration files (and optionally credentials), and verifying the IP location change using WhatIsMyIP.
 
 ## Usage
 ```python
 from iplocationchanger.service.location_changer_service import LocationChangerService
+from iplocationchanger.exception.location_changer_service_exception import LocationChangerServiceException
+
 
 try:
   lcs = LocationChangerService(
     'reoiotiyotrkc77690543031b421b',
     {
       'TR': '/assets/NCVPN-TR-Istanbul-TCP.ovpn',
     },
     '/usr/local/openvpn',
     '/assets/openvpncredentials',
   )
 
   country = 'TR'
-  success, msg = lcs.connect_region(country)
-  if not success:
-    logging.error(msg)
-    raise Exception(
-      f'could not connect location: {country}. {msg}.'
-    )
-  # Other code logic
+  try:
+    lcs.connect_region(country)
+    # Other code logic...
+
+  except LocationChangerServiceException as e:
+    # locaiton change failed
+    logging.error(e)
+    exit(1)
 finally:
   lcs.disconnect_region()
 ```
 ### Standalone Execution
 ```shell
 # Sample execution
 python3 src/iplocationchanger/__main__.py \
```

### Comparing `iplocationchanger-0.0.2/README.md` & `iplocationchanger-0.0.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -2,33 +2,36 @@
 Reliable IP location changer using [OpenVPN](https://openvpn.net/) and [WhatIsMyIP](https://www.whatismyip.com/).
 
 This package allows changing the IP of the host machine by using openvpn configuration files (and optionally credentials), and verifying the IP location change using WhatIsMyIP.
 
 ## Usage
 ```python
 from iplocationchanger.service.location_changer_service import LocationChangerService
+from iplocationchanger.exception.location_changer_service_exception import LocationChangerServiceException
+
 
 try:
   lcs = LocationChangerService(
     'reoiotiyotrkc77690543031b421b',
     {
       'TR': '/assets/NCVPN-TR-Istanbul-TCP.ovpn',
     },
     '/usr/local/openvpn',
     '/assets/openvpncredentials',
   )
 
   country = 'TR'
-  success, msg = lcs.connect_region(country)
-  if not success:
-    logging.error(msg)
-    raise Exception(
-      f'could not connect location: {country}. {msg}.'
-    )
-  # Other code logic
+  try:
+    lcs.connect_region(country)
+    # Other code logic...
+
+  except LocationChangerServiceException as e:
+    # locaiton change failed
+    logging.error(e)
+    exit(1)
 finally:
   lcs.disconnect_region()
 ```
 ### Standalone Execution
 ```shell
 # Sample execution
 python3 src/iplocationchanger/__main__.py \
```

### Comparing `iplocationchanger-0.0.2/pyproject.toml` & `iplocationchanger-0.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "iplocationchanger"
-version = "0.0.2"
+version = "0.0.3"
 description = "Reliable IP location changer using OpenVPN and WhatIsMyIP"
 readme = "README.md"
 authors = [{ name = "Faizudeen Kajogbola", email = "faizudeen@codecreek.cc" }]
 license = { file = "LICENSE" }
 classifiers = [
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python",
```

### Comparing `iplocationchanger-0.0.2/src/iplocationchanger/__main__.py` & `iplocationchanger-0.0.3/src/iplocationchanger/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import argparse
 import logging
 import json
 import atexit
 
 from iplocationchanger.model.openvpn_credentials import OpenVPNCredentials
 from iplocationchanger.service.location_changer_service import LocationChangerService
+from iplocationchanger.exception.location_changer_service_exception import LocationChangerServiceException
 
 parser = argparse.ArgumentParser(
   prog = 'iplocationchanger',
   description = 'Reliable IP location changer using OpenVPN and WhatIsMyIP.',
 )
 
 parser.add_argument(
@@ -81,17 +82,18 @@
     args.api_key,
     config_to_country_map,
     args.openvpn,
     openvpn_credentials_path=ovnc_path,
   )
   atexit.register(lcs.disconnect_region)
 
-  success, msg = lcs.connect_region(args.country)
-  if not success:
-    logging.error(msg)
+  try:
+    lcs.connect_region(args.country)
+  except LocationChangerServiceException as e:
+    logging.error(e)
     exit(1)
   # Keep running
   logging.info(f'connected to {args.country}')
   input('Press ENTER to disconnect\n')
 
 if __name__ == '__main__':
   args = parser.parse_args()
```

### Comparing `iplocationchanger-0.0.2/src/iplocationchanger/model/openvpn_credentials.py` & `iplocationchanger-0.0.3/src/iplocationchanger/model/openvpn_credentials.py`

 * *Files identical despite different names*

### Comparing `iplocationchanger-0.0.2/src/iplocationchanger/service/location_changer_service.py` & `iplocationchanger-0.0.3/src/iplocationchanger/service/location_changer_service.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from __future__ import annotations
 
 import logging
 import time
 
 from iplocationchanger.service.openvpn_service import OpenVPNService
 from iplocationchanger.service.whatismyip_service import WhatIsMyIPService
+from iplocationchanger.exception.location_changer_service_exception import LocationChangerServiceException
+from iplocationchanger.exception.whatismyip_service_exception import WhatIsMyIPServiceException
+from iplocationchanger.exception.openvpn_service_exception import OpenVPNServiceException
 
 logger = logging.getLogger(__name__)
 
 class LocationChangerService:
   def __init__(
     self: LocationChangerService,
     whatismyip_api_key: str,
@@ -34,23 +37,28 @@
       openvpn_config_to_country_map,
       openvpn_executable_path,
       credentials_path=openvpn_credentials_path,
     )
 
   def disconnect_region(
     self: LocationChangerService,
-  ) -> tuple[bool, str]:
-    logger.info('disconnecting...')
-    success, stdout, stderr = self.ovs.disconnect()
-    return success, (stdout + stderr)
+  ) -> None:
+    logger.debug('disconnecting...')
+    self.ovs.disconnect()
 
   def connect_region(
     self: LocationChangerService,
     country: str,
     OPENVPN_DELAY: int = 5,
-  ) -> tuple[bool, str]:
-    logger.info(f'connecting to {country}...')
-    success, stdout, stderr = self.ovs.connect(country)
+  ) -> None:
+    logger.debug(f'connecting to {country}...')
+    try:
+      self.ovs.connect(country)
+    except OpenVPNServiceException as e:
+      raise LocationChangerServiceException(f'Could not connect to {country}') from e
     # buy openvpn some time
     time.sleep(OPENVPN_DELAY)
-    valid_connection, out = self.wms.validate_connection(country)
-    return (success and valid_connection), (stdout + stderr + out)
+    try:
+      self.wms.validate_connection(country)
+    except WhatIsMyIPServiceException as e:
+      raise LocationChangerServiceException(f'Could not connect to {country}') from e
+    logger.debug(f'connected to {country}')
```

### Comparing `iplocationchanger-0.0.2/src/iplocationchanger/utils/utils.py` & `iplocationchanger-0.0.3/src/iplocationchanger/utils/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -33,24 +33,7 @@
       if expect_error:
         return (
           True,
           'execution failed',
           '',
         )
       raise e
-
-  @classmethod
-  def exec_get_request(cls: Utils, url: str) -> tuple[bool, str]:
-    logger.debug(f'URL: {url}')
-    res = requests.get(url)
-    success = res.status_code > 199 and res.status_code < 300
-    res_body = res.content.decode('utf-8')
-    logger.debug(f'RESPONSE: {res_body}')
-    return success, res_body
-
-  @classmethod
-  def extract_location(cls: Utils, location_str: str) -> str:
-    logger.debug(f'LOCATION STR: {location_str}')
-    cty_idx = location_str.find('country')
-    country_code = location_str[cty_idx:].split(':')[1].split('\r\n')[0].strip()
-    logger.debug(f'CTR CODE: {country_code}')
-    return country_code
```

### Comparing `iplocationchanger-0.0.2/src/iplocationchanger.egg-info/PKG-INFO` & `iplocationchanger-0.0.3/src/iplocationchanger.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iplocationchanger
-Version: 0.0.2
+Version: 0.0.3
 Summary: Reliable IP location changer using OpenVPN and WhatIsMyIP
 Author-email: Faizudeen Kajogbola <faizudeen@codecreek.cc>
 License: MIT License
         
         Copyright (c) 2023 Faizudeen Kajogbola
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -41,33 +41,36 @@
 Reliable IP location changer using [OpenVPN](https://openvpn.net/) and [WhatIsMyIP](https://www.whatismyip.com/).
 
 This package allows changing the IP of the host machine by using openvpn configuration files (and optionally credentials), and verifying the IP location change using WhatIsMyIP.
 
 ## Usage
 ```python
 from iplocationchanger.service.location_changer_service import LocationChangerService
+from iplocationchanger.exception.location_changer_service_exception import LocationChangerServiceException
+
 
 try:
   lcs = LocationChangerService(
     'reoiotiyotrkc77690543031b421b',
     {
       'TR': '/assets/NCVPN-TR-Istanbul-TCP.ovpn',
     },
     '/usr/local/openvpn',
     '/assets/openvpncredentials',
   )
 
   country = 'TR'
-  success, msg = lcs.connect_region(country)
-  if not success:
-    logging.error(msg)
-    raise Exception(
-      f'could not connect location: {country}. {msg}.'
-    )
-  # Other code logic
+  try:
+    lcs.connect_region(country)
+    # Other code logic...
+
+  except LocationChangerServiceException as e:
+    # locaiton change failed
+    logging.error(e)
+    exit(1)
 finally:
   lcs.disconnect_region()
 ```
 ### Standalone Execution
 ```shell
 # Sample execution
 python3 src/iplocationchanger/__main__.py \
```

### Comparing `iplocationchanger-0.0.2/src/iplocationchanger.egg-info/SOURCES.txt` & `iplocationchanger-0.0.3/src/iplocationchanger.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 src/iplocationchanger/__init__.py
 src/iplocationchanger/__main__.py
 src/iplocationchanger.egg-info/PKG-INFO
 src/iplocationchanger.egg-info/SOURCES.txt
 src/iplocationchanger.egg-info/dependency_links.txt
 src/iplocationchanger.egg-info/requires.txt
 src/iplocationchanger.egg-info/top_level.txt
+src/iplocationchanger/exception/iplocationchanger_exception.py
+src/iplocationchanger/exception/location_changer_service_exception.py
+src/iplocationchanger/exception/openvpn_service_exception.py
+src/iplocationchanger/exception/whatismyip_service_exception.py
 src/iplocationchanger/model/__init__.py
 src/iplocationchanger/model/openvpn_credentials.py
 src/iplocationchanger/service/__init__.py
 src/iplocationchanger/service/location_changer_service.py
 src/iplocationchanger/service/openvpn_service.py
 src/iplocationchanger/service/whatismyip_service.py
 src/iplocationchanger/utils/__init__.py
```


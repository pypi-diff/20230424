# Comparing `tmp/python_orbuculum_bad-0.1.0.tar.gz` & `tmp/python_orbuculum_bad-0.1.1.tar.gz`

## Comparing `python_orbuculum_bad-0.1.0.tar` & `python_orbuculum_bad-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 python_orbuculum_bad-0.1.0/.python-version
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 python_orbuculum_bad-0.1.0/requirements-dev.lock
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 python_orbuculum_bad-0.1.0/requirements.lock
--rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 python_orbuculum_bad-0.1.0/orbuculum_bad/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_orbuculum_bad-0.1.0/orbuculum_bad/protos/__init__.py
--rw-r--r--   0        0        0     6111 2020-02-02 00:00:00.000000 python_orbuculum_bad-0.1.0/orbuculum_bad/protos/network.py
--rw-r--r--   0        0        0     7904 2020-02-02 00:00:00.000000 python_orbuculum_bad-0.1.0/orbuculum_bad/protos/network.pyi
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 python_orbuculum_bad-0.1.0/.gitignore
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 python_orbuculum_bad-0.1.0/README.md
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 python_orbuculum_bad-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 python_orbuculum_bad-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 python_orbuculum_bad-0.1.1/.python-version
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 python_orbuculum_bad-0.1.1/requirements-dev.lock
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 python_orbuculum_bad-0.1.1/requirements.lock
+-rw-r--r--   0        0        0     6235 2020-02-02 00:00:00.000000 python_orbuculum_bad-0.1.1/orbuculum_bad/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_orbuculum_bad-0.1.1/orbuculum_bad/protos/__init__.py
+-rw-r--r--   0        0        0     6111 2020-02-02 00:00:00.000000 python_orbuculum_bad-0.1.1/orbuculum_bad/protos/network.py
+-rw-r--r--   0        0        0     7904 2020-02-02 00:00:00.000000 python_orbuculum_bad-0.1.1/orbuculum_bad/protos/network.pyi
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 python_orbuculum_bad-0.1.1/.gitignore
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 python_orbuculum_bad-0.1.1/README.md
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 python_orbuculum_bad-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 python_orbuculum_bad-0.1.1/PKG-INFO
```

### Comparing `python_orbuculum_bad-0.1.0/requirements-dev.lock` & `python_orbuculum_bad-0.1.1/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `python_orbuculum_bad-0.1.0/orbuculum_bad/__init__.py` & `python_orbuculum_bad-0.1.1/orbuculum_bad/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 This module is a subproject for orbuculum, it implentments the simplest function,
 like get first network port or get the last network port for commerimal projects.
 """
-from typing import Any, List
+from typing import Any, Dict, List
 from grpc_requests import Client
 from orbuculum_bad.protos.network import DevicesReplyBody
 
 def get_all_ether_devices(client: Client) -> List[DevicesReplyBody]:
     """Get all devices from orbuculum grpc service
 
     Args:
@@ -137,14 +137,36 @@
             The interface name of the last network card without fibre linkmode.
             If there're no interfaces without fibre linkmode, returns an empty string.
         """
         if len(self.fibre_devices) > 0:
             return self.fibre_devices[-1].name
         return ''
 
+    def get_connection_mapping(self) -> Dict[str, str]:
+        """Retrive connection names' mapping.
+
+        Returns:
+            The mapping of connection names to interfaces.
+        """
+        mapping = {}
+        for device in self.devices:
+            mapping[device.connection.id.value] = device.name
+        return mapping
+
+    def get_interface_mapping(self) -> Dict[str, str]:
+        """Retrive interfaces' mapping.
+
+        Returns:
+            The mapping of interfaces to connection names.
+        """
+        mapping = {}
+        for device in self.devices:
+            mapping[device.name] = device.connection.id.value
+        return mapping
+
     def get_all_ip_addresses(self) -> List[str]:
         """retrive all ip addresses from all the ethernet devices
 
         Returns:
             List of ip addresses, including ipv4 or ipv6.
         """
         ipaddrs = []
```

### Comparing `python_orbuculum_bad-0.1.0/orbuculum_bad/protos/network.py` & `python_orbuculum_bad-0.1.1/orbuculum_bad/protos/network.py`

 * *Files identical despite different names*

### Comparing `python_orbuculum_bad-0.1.0/orbuculum_bad/protos/network.pyi` & `python_orbuculum_bad-0.1.1/orbuculum_bad/protos/network.pyi`

 * *Files identical despite different names*

### Comparing `python_orbuculum_bad-0.1.0/PKG-INFO` & `python_orbuculum_bad-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-orbuculum-bad
-Version: 0.1.0
+Version: 0.1.1
 Summary: A really solo and ungly client for orbuculum service.
 Author-email: ssfdust <ssfdust@gmail.com>
 License: MIT
 Requires-Python: >=3.7
 Requires-Dist: grpc-requests~=0.1.10
 Description-Content-Type: text/markdown
```


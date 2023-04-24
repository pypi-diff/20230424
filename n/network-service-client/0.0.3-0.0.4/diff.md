# Comparing `tmp/network_service_client-0.0.3.tar.gz` & `tmp/network_service_client-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "network_service_client-0.0.3.tar", last modified: Wed Jan 18 09:24:57 2023, max compression
+gzip compressed data, was "network_service_client-0.0.4.tar", last modified: Mon Apr 24 11:38:10 2023, max compression
```

## Comparing `network_service_client-0.0.3.tar` & `network_service_client-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-01-18 09:24:57.962939 network_service_client-0.0.3/
--rw-rw-rw-   0        0        0     1091 2022-12-18 08:33:31.000000 network_service_client-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1336 2023-01-18 09:24:57.960547 network_service_client-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      933 2023-01-18 09:23:49.000000 network_service_client-0.0.3/README.md
--rw-rw-rw-   0        0        0      541 2023-01-18 09:23:54.000000 network_service_client-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-18 09:24:57.965312 network_service_client-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-01-18 09:24:57.835646 network_service_client-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-01-18 09:24:57.910982 network_service_client-0.0.3/src/network_service_client/
--rw-rw-rw-   0        0        0        0 2022-12-18 08:33:31.000000 network_service_client-0.0.3/src/network_service_client/__init__.py
--rw-rw-rw-   0        0        0      227 2023-01-16 16:00:54.000000 network_service_client-0.0.3/src/network_service_client/abstractions.py
--rw-rw-rw-   0        0        0      740 2023-01-17 07:21:37.000000 network_service_client-0.0.3/src/network_service_client/client.py
--rw-rw-rw-   0        0        0      914 2023-01-16 16:36:26.000000 network_service_client-0.0.3/src/network_service_client/enums.py
--rw-rw-rw-   0        0        0      415 2023-01-16 16:00:36.000000 network_service_client-0.0.3/src/network_service_client/models.py
-drwxrwxrwx   0        0        0        0 2023-01-18 09:24:57.958564 network_service_client-0.0.3/src/network_service_client.egg-info/
--rw-rw-rw-   0        0        0     1336 2023-01-18 09:24:57.000000 network_service_client-0.0.3/src/network_service_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      473 2023-01-18 09:24:57.000000 network_service_client-0.0.3/src/network_service_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-18 09:24:57.000000 network_service_client-0.0.3/src/network_service_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-01-18 09:24:57.000000 network_service_client-0.0.3/src/network_service_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-01-18 09:24:57.000000 network_service_client-0.0.3/src/network_service_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 11:38:10.584797 network_service_client-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-04-24 06:48:21.000000 network_service_client-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1370 2023-04-24 11:38:10.582795 network_service_client-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      933 2023-04-24 06:48:21.000000 network_service_client-0.0.4/README.md
+-rw-rw-rw-   0        0        0      595 2023-04-24 10:24:47.000000 network_service_client-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-24 11:38:10.585794 network_service_client-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-24 11:38:10.539830 network_service_client-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-24 11:38:10.565799 network_service_client-0.0.4/src/network_service_client/
+-rw-rw-rw-   0        0        0        0 2023-04-24 06:48:21.000000 network_service_client-0.0.4/src/network_service_client/__init__.py
+-rw-rw-rw-   0        0        0      227 2023-04-24 06:48:21.000000 network_service_client-0.0.4/src/network_service_client/abstractions.py
+-rw-rw-rw-   0        0        0      740 2023-04-24 06:48:21.000000 network_service_client-0.0.4/src/network_service_client/client.py
+-rw-rw-rw-   0        0        0      946 2023-04-24 10:24:47.000000 network_service_client-0.0.4/src/network_service_client/enums.py
+-rw-rw-rw-   0        0        0      415 2023-04-24 06:48:21.000000 network_service_client-0.0.4/src/network_service_client/models.py
+drwxrwxrwx   0        0        0        0 2023-04-24 11:38:10.578796 network_service_client-0.0.4/src/network_service_client.egg-info/
+-rw-rw-rw-   0        0        0     1370 2023-04-24 11:38:10.000000 network_service_client-0.0.4/src/network_service_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      473 2023-04-24 11:38:10.000000 network_service_client-0.0.4/src/network_service_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 11:38:10.000000 network_service_client-0.0.4/src/network_service_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-04-24 11:38:10.000000 network_service_client-0.0.4/src/network_service_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-04-24 11:38:10.000000 network_service_client-0.0.4/src/network_service_client.egg-info/top_level.txt
```

### Comparing `network_service_client-0.0.3/LICENSE` & `network_service_client-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `network_service_client-0.0.3/PKG-INFO` & `network_service_client-0.0.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: network_service_client
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small client for network service
-Author-email: Alejandro <agarrido@izertis.com>
+Author-email: Alejandro <agarrido@izertis.com>, Iraia <iolabarrieta@izertis.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `network_service_client-0.0.3/README.md` & `network_service_client-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `network_service_client-0.0.3/pyproject.toml` & `network_service_client-0.0.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "network_service_client"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
-  { name="Alejandro", email="agarrido@izertis.com" },
+  { name="Alejandro", email="agarrido@izertis.com"},
+  { name="Iraia", email="iolabarrieta@izertis.com" },
 ]
 description = "A small client for network service"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `network_service_client-0.0.3/src/network_service_client/client.py` & `network_service_client-0.0.4/src/network_service_client/client.py`

 * *Files identical despite different names*

### Comparing `network_service_client-0.0.3/src/network_service_client/enums.py` & `network_service_client-0.0.4/src/network_service_client/enums.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from enum import Enum
 
 
 class NetworksNames(str, Enum):
     AlastriaDefaultName = "Alastria"
     LacchainDefaultName = "Lacchain"
+    EbsiDefaultName = "Ebsi"
 
     @classmethod
     def choices(cls):
         return tuple((i.name, i.value) for i in cls)
 
 
 class ContractsNames(str, Enum):
@@ -20,8 +21,8 @@
     AlastriaIdentityManager = "AlastriaIdentityManager"
     LacchainDIDRegistry = "LacchainDIDRegistry"
     LacchainCredentialRegistry = "LacchainCredentialRegistry"
     LacchainClaimsVerifier = "LacchainClaimsVerifier"
 
     @classmethod
     def choices(cls):
-        return tuple((i.name, i.value) for i in cls)
+        return tuple((i.name, i.value) for i in cls)
```

### Comparing `network_service_client-0.0.3/src/network_service_client.egg-info/PKG-INFO` & `network_service_client-0.0.4/src/network_service_client.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: network-service-client
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small client for network service
-Author-email: Alejandro <agarrido@izertis.com>
+Author-email: Alejandro <agarrido@izertis.com>, Iraia <iolabarrieta@izertis.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```


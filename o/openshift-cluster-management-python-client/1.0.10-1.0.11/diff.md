# Comparing `tmp/openshift-cluster-management-python-client-1.0.10.tar.gz` & `tmp/openshift-cluster-management-python-client-1.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openshift-cluster-management-python-client-1.0.10.tar", last modified: Thu Mar 30 10:21:05 2023, max compression
+gzip compressed data, was "openshift-cluster-management-python-client-1.0.11.tar", last modified: Mon Apr 24 08:49:19 2023, max compression
```

## Comparing `openshift-cluster-management-python-client-1.0.10.tar` & `openshift-cluster-management-python-client-1.0.11.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 10:21:05.363125 openshift-cluster-management-python-client-1.0.10/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-03-30 10:21:01.000000 openshift-cluster-management-python-client-1.0.10/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2147 2023-03-30 10:21:05.363125 openshift-cluster-management-python-client-1.0.10/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1270 2023-03-30 10:21:01.000000 openshift-cluster-management-python-client-1.0.10/README.md
--rw-r--r--   0 root         (0) root         (0)        7 2023-03-30 10:21:01.000000 openshift-cluster-management-python-client-1.0.10/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 10:21:05.362125 openshift-cluster-management-python-client-1.0.10/ocm_python_wrapper/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 10:21:01.000000 openshift-cluster-management-python-client-1.0.10/ocm_python_wrapper/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12588 2023-03-30 10:21:01.000000 openshift-cluster-management-python-client-1.0.10/ocm_python_wrapper/cluster.py
--rw-r--r--   0 root         (0) root         (0)      554 2023-03-30 10:21:01.000000 openshift-cluster-management-python-client-1.0.10/ocm_python_wrapper/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2432 2023-03-30 10:21:01.000000 openshift-cluster-management-python-client-1.0.10/ocm_python_wrapper/logger.py
--rw-r--r--   0 root         (0) root         (0)     2791 2023-03-30 10:21:01.000000 openshift-cluster-management-python-client-1.0.10/ocm_python_wrapper/ocm_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 10:21:05.363125 openshift-cluster-management-python-client-1.0.10/openshift_cluster_management_python_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2147 2023-03-30 10:21:05.000000 openshift-cluster-management-python-client-1.0.10/openshift_cluster_management_python_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      525 2023-03-30 10:21:05.000000 openshift-cluster-management-python-client-1.0.10/openshift_cluster_management_python_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-30 10:21:05.000000 openshift-cluster-management-python-client-1.0.10/openshift_cluster_management_python_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       95 2023-03-30 10:21:05.000000 openshift-cluster-management-python-client-1.0.10/openshift_cluster_management_python_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-03-30 10:21:05.000000 openshift-cluster-management-python-client-1.0.10/openshift_cluster_management_python_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1570 2023-03-30 10:21:01.000000 openshift-cluster-management-python-client-1.0.10/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-30 10:21:05.363125 openshift-cluster-management-python-client-1.0.10/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:49:19.615628 openshift-cluster-management-python-client-1.0.11/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-04-24 08:49:17.000000 openshift-cluster-management-python-client-1.0.11/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2147 2023-04-24 08:49:19.615628 openshift-cluster-management-python-client-1.0.11/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1270 2023-04-24 08:49:17.000000 openshift-cluster-management-python-client-1.0.11/README.md
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-24 08:49:17.000000 openshift-cluster-management-python-client-1.0.11/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:49:19.615628 openshift-cluster-management-python-client-1.0.11/ocm_python_wrapper/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 08:49:17.000000 openshift-cluster-management-python-client-1.0.11/ocm_python_wrapper/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13664 2023-04-24 08:49:17.000000 openshift-cluster-management-python-client-1.0.11/ocm_python_wrapper/cluster.py
+-rw-r--r--   0 root         (0) root         (0)      554 2023-04-24 08:49:17.000000 openshift-cluster-management-python-client-1.0.11/ocm_python_wrapper/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2432 2023-04-24 08:49:17.000000 openshift-cluster-management-python-client-1.0.11/ocm_python_wrapper/logger.py
+-rw-r--r--   0 root         (0) root         (0)     2791 2023-04-24 08:49:17.000000 openshift-cluster-management-python-client-1.0.11/ocm_python_wrapper/ocm_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 08:49:19.615628 openshift-cluster-management-python-client-1.0.11/openshift_cluster_management_python_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2147 2023-04-24 08:49:19.000000 openshift-cluster-management-python-client-1.0.11/openshift_cluster_management_python_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      525 2023-04-24 08:49:19.000000 openshift-cluster-management-python-client-1.0.11/openshift_cluster_management_python_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 08:49:19.000000 openshift-cluster-management-python-client-1.0.11/openshift_cluster_management_python_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       95 2023-04-24 08:49:19.000000 openshift-cluster-management-python-client-1.0.11/openshift_cluster_management_python_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-04-24 08:49:19.000000 openshift-cluster-management-python-client-1.0.11/openshift_cluster_management_python_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1570 2023-04-24 08:49:17.000000 openshift-cluster-management-python-client-1.0.11/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 08:49:19.615628 openshift-cluster-management-python-client-1.0.11/setup.cfg
```

### Comparing `openshift-cluster-management-python-client-1.0.10/LICENSE` & `openshift-cluster-management-python-client-1.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `openshift-cluster-management-python-client-1.0.10/PKG-INFO` & `openshift-cluster-management-python-client-1.0.11/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openshift-cluster-management-python-client
-Version: 1.0.10
+Version: 1.0.11
 Summary: Wrapper around https://github.com/openshift/openshift-cluster-management-python-client
 Author-email: Meni Yakove <myakove@gmail.com>, Ruth Netser <rnetser@gmail.com>
 Project-URL: Homepage, https://github.com/RedHatQE/openshift-cluster-management-python-client
 Project-URL: Download, https://pypi.org/project/openshift-cluster-management-python-client/
 Project-URL: Bug Tracker, https://github.com/RedHatQE/oopenshift-cluster-management-python-client/issues
 Project-URL: Documentation, https://github.com/rnetser/openshift-cluster-management-python-wrapper/blob/main/README.md
 Keywords: Openshift,OCM
```

### Comparing `openshift-cluster-management-python-client-1.0.10/README.md` & `openshift-cluster-management-python-client-1.0.11/README.md`

 * *Files identical despite different names*

### Comparing `openshift-cluster-management-python-client-1.0.10/ocm_python_wrapper/cluster.py` & `openshift-cluster-management-python-client-1.0.11/ocm_python_wrapper/cluster.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 from ocm_python_client.exceptions import NotFoundException
 from ocm_python_client.model.add_on import AddOn
 from ocm_python_client.model.add_on_installation import AddOnInstallation
 from ocm_python_client.model.add_on_installation_parameter import (
     AddOnInstallationParameter,
 )
 from ocm_python_client.model.upgrade_policy import UpgradePolicy
+from ocp_resources.constants import NOT_FOUND_ERROR_EXCEPTION_DICT
+from ocp_resources.resource import ResourceEditor
+from ocp_resources.rhmi import RHMI
 from ocp_resources.utils import TimeoutExpiredError, TimeoutSampler
 from ocp_utilities.infra import get_client
 
 from ocm_python_wrapper.exceptions import MissingResourceError
 from ocm_python_wrapper.logger import get_logger
 
 LOGGER = get_logger(__name__)
@@ -208,14 +211,18 @@
         Returns cluster instance if cluster exists else returns None
         """
         try:
             return self.instance
         except NotFoundException:
             return None
 
+    @property
+    def cloud_provider(self):
+        return self.instance.cloud_provider.id if self.exists else None
+
 
 class ClusterAddOn(Cluster):
     """
     manage cluster addon
 
     Example:
          _client = OCMPythonClient(
@@ -297,14 +304,21 @@
         LOGGER.info(f"Installing addon {self.addon_name}")
         res = self.client.api_clusters_mgmt_v1_clusters_cluster_id_addons_post(
             cluster_id=self.cluster_id,
             add_on_installation=AddOnInstallation(
                 _check_type=False, **_addon_installation_dict
             ),
         )
+
+        if (
+            self.addon_name == "managed-api-service"
+            and "stage" in self.client.api_client.configuration.host
+        ):
+            self.update_rhoam_cluster_storage_config()
+
         if wait:
             self.wait_for_install_state(
                 state=self.State.READY, wait_timeout=wait_timeout
             )
 
         LOGGER.info(f"{self.addon_name} successfully installed")
         return res
@@ -350,7 +364,24 @@
             for (
                 _addon_installation_instance
             ) in self.addon_installation_instance_sampler(wait_timeout=wait_timeout):
                 if not _addon_installation_instance:
                     return True
         LOGGER.info(f"{self.addon_name} was successfully removed")
         return res
+
+    @staticmethod
+    def update_rhoam_cluster_storage_config():
+        def _wait_for_rhmi_resource():
+            for sample in TimeoutSampler(
+                wait_timeout=TIMEOUT_30MIN,
+                sleep=SLEEP_1SEC,
+                func=lambda: RHMI(name="rhoam", namespace="redhat-rhoam-operator"),
+                exceptions_dict=NOT_FOUND_ERROR_EXCEPTION_DICT,
+            ):
+                if sample:
+                    return sample
+
+        rhmi = _wait_for_rhmi_resource()
+        ResourceEditor(
+            patches={rhmi: {"spec": {"useClusterStorage": "false"}}}
+        ).update()
```

### Comparing `openshift-cluster-management-python-client-1.0.10/ocm_python_wrapper/exceptions.py` & `openshift-cluster-management-python-client-1.0.11/ocm_python_wrapper/exceptions.py`

 * *Files identical despite different names*

### Comparing `openshift-cluster-management-python-client-1.0.10/ocm_python_wrapper/logger.py` & `openshift-cluster-management-python-client-1.0.11/ocm_python_wrapper/logger.py`

 * *Files identical despite different names*

### Comparing `openshift-cluster-management-python-client-1.0.10/ocm_python_wrapper/ocm_client.py` & `openshift-cluster-management-python-client-1.0.11/ocm_python_wrapper/ocm_client.py`

 * *Files identical despite different names*

### Comparing `openshift-cluster-management-python-client-1.0.10/openshift_cluster_management_python_client.egg-info/PKG-INFO` & `openshift-cluster-management-python-client-1.0.11/openshift_cluster_management_python_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openshift-cluster-management-python-client
-Version: 1.0.10
+Version: 1.0.11
 Summary: Wrapper around https://github.com/openshift/openshift-cluster-management-python-client
 Author-email: Meni Yakove <myakove@gmail.com>, Ruth Netser <rnetser@gmail.com>
 Project-URL: Homepage, https://github.com/RedHatQE/openshift-cluster-management-python-client
 Project-URL: Download, https://pypi.org/project/openshift-cluster-management-python-client/
 Project-URL: Bug Tracker, https://github.com/RedHatQE/oopenshift-cluster-management-python-client/issues
 Project-URL: Documentation, https://github.com/rnetser/openshift-cluster-management-python-wrapper/blob/main/README.md
 Keywords: Openshift,OCM
```

### Comparing `openshift-cluster-management-python-client-1.0.10/openshift_cluster_management_python_client.egg-info/SOURCES.txt` & `openshift-cluster-management-python-client-1.0.11/openshift_cluster_management_python_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openshift-cluster-management-python-client-1.0.10/pyproject.toml` & `openshift-cluster-management-python-client-1.0.11/pyproject.toml`

 * *Files identical despite different names*


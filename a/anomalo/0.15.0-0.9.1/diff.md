# Comparing `tmp/anomalo-0.15.0.tar.gz` & `tmp/anomalo-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anomalo-0.15.0.tar", last modified: Mon Apr 24 21:00:42 2023, max compression
+gzip compressed data, was "dist/anomalo-0.9.1.tar", last modified: Wed Sep  7 16:54:04 2022, max compression
```

## Comparing `anomalo-0.15.0.tar` & `anomalo-0.9.1.tar`

### file list

```diff
@@ -1,31 +1,22 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-24 21:00:42.020671 anomalo-0.15.0/
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-04-07 11:00:44.000000 anomalo-0.15.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)    11344 2023-04-07 11:00:44.000000 anomalo-0.15.0/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)      330 2023-04-24 21:00:42.020671 anomalo-0.15.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      211 2023-04-07 11:00:44.000000 anomalo-0.15.0/README.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-24 21:00:42.016671 anomalo-0.15.0/anomalo/
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-04-24 18:27:57.000000 anomalo-0.15.0/anomalo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-04-07 11:00:44.000000 anomalo-0.15.0/anomalo/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)       23 2023-04-24 21:00:40.000000 anomalo-0.15.0/anomalo/_version.py
--rwxrwxrwx   0 root         (0) root         (0)      250 2023-04-24 18:09:34.000000 anomalo-0.15.0/anomalo/anomalo.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-24 21:00:42.016671 anomalo-0.15.0/anomalo/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-24 18:09:34.000000 anomalo-0.15.0/anomalo/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      699 2023-04-24 18:09:34.000000 anomalo-0.15.0/anomalo/cli/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     7878 2023-04-24 18:09:34.000000 anomalo-0.15.0/anomalo/cli/models.py
--rw-rw-rw-   0 root         (0) root         (0)     6134 2023-04-24 18:09:34.000000 anomalo-0.15.0/anomalo/cli/state.py
--rw-rw-rw-   0 root         (0) root         (0)     9946 2023-04-24 18:09:34.000000 anomalo-0.15.0/anomalo/client.py
--rw-rw-rw-   0 root         (0) root         (0)     3425 2023-04-07 11:00:44.000000 anomalo-0.15.0/anomalo/encoder.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-24 21:00:42.016671 anomalo-0.15.0/anomalo.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)      330 2023-04-24 21:00:41.000000 anomalo-0.15.0/anomalo.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      519 2023-04-24 21:00:41.000000 anomalo-0.15.0/anomalo.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-24 21:00:41.000000 anomalo-0.15.0/anomalo.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-04-24 21:00:41.000000 anomalo-0.15.0/anomalo.egg-info/entry_points.txt
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-04-24 21:00:41.000000 anomalo-0.15.0/anomalo.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        8 2023-04-24 21:00:41.000000 anomalo-0.15.0/anomalo.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-24 21:00:42.020671 anomalo-0.15.0/examples/
--rw-rw-rw-   0 root         (0) root         (0)     3642 2023-04-07 11:00:44.000000 anomalo-0.15.0/examples/bulk_rerun.py
--rw-rw-rw-   0 root         (0) root         (0)     1284 2023-04-07 11:00:44.000000 anomalo-0.15.0/examples/sample.py
--rw-rw-rw-   0 root         (0) root         (0)     3575 2023-04-07 11:00:44.000000 anomalo-0.15.0/examples/table_save_load.py
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-04-07 11:00:44.000000 anomalo-0.15.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-24 21:00:42.020671 anomalo-0.15.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      934 2023-04-24 20:56:26.000000 anomalo-0.15.0/setup.py
+drwxr-xr-x   0 johnjoo    (501) staff       (20)        0 2022-09-07 16:54:04.000000 anomalo-0.9.1/
+-rw-r--r--   0 johnjoo    (501) staff       (20)       33 2022-09-06 04:48:18.000000 anomalo-0.9.1/.gitignore
+-rw-r--r--   0 johnjoo    (501) staff       (20)    11344 2022-09-06 04:48:18.000000 anomalo-0.9.1/LICENSE.txt
+-rw-r--r--   0 johnjoo    (501) staff       (20)      308 2022-09-07 16:54:04.000000 anomalo-0.9.1/PKG-INFO
+-rw-r--r--   0 johnjoo    (501) staff       (20)      211 2022-09-06 04:48:18.000000 anomalo-0.9.1/README.txt
+drwxr-xr-x   0 johnjoo    (501) staff       (20)        0 2022-09-07 16:54:04.000000 anomalo-0.9.1/anomalo/
+-rw-r--r--   0 johnjoo    (501) staff       (20)       57 2022-09-06 04:48:18.000000 anomalo-0.9.1/anomalo/__init__.py
+-rw-r--r--   0 johnjoo    (501) staff       (20)       22 2022-09-07 16:54:02.000000 anomalo-0.9.1/anomalo/_version.py
+-rwxr-xr-x   0 johnjoo    (501) staff       (20)     7444 2022-09-06 04:48:18.000000 anomalo-0.9.1/anomalo/anomalo.py
+drwxr-xr-x   0 johnjoo    (501) staff       (20)        0 2022-09-07 16:54:04.000000 anomalo-0.9.1/anomalo.egg-info/
+-rw-r--r--   0 johnjoo    (501) staff       (20)      308 2022-09-07 16:54:04.000000 anomalo-0.9.1/anomalo.egg-info/PKG-INFO
+-rw-r--r--   0 johnjoo    (501) staff       (20)      348 2022-09-07 16:54:04.000000 anomalo-0.9.1/anomalo.egg-info/SOURCES.txt
+-rw-r--r--   0 johnjoo    (501) staff       (20)        1 2022-09-07 16:54:04.000000 anomalo-0.9.1/anomalo.egg-info/dependency_links.txt
+-rw-r--r--   0 johnjoo    (501) staff       (20)       41 2022-09-07 16:54:04.000000 anomalo-0.9.1/anomalo.egg-info/entry_points.txt
+-rw-r--r--   0 johnjoo    (501) staff       (20)       14 2022-09-07 16:54:04.000000 anomalo-0.9.1/anomalo.egg-info/requires.txt
+-rw-r--r--   0 johnjoo    (501) staff       (20)        8 2022-09-07 16:54:04.000000 anomalo-0.9.1/anomalo.egg-info/top_level.txt
+drwxr-xr-x   0 johnjoo    (501) staff       (20)        0 2022-09-07 16:54:04.000000 anomalo-0.9.1/examples/
+-rw-r--r--   0 johnjoo    (501) staff       (20)     3701 2022-09-06 04:48:18.000000 anomalo-0.9.1/examples/bulk_rerun.py
+-rw-r--r--   0 johnjoo    (501) staff       (20)     1284 2022-09-06 04:48:18.000000 anomalo-0.9.1/examples/sample.py
+-rw-r--r--   0 johnjoo    (501) staff       (20)       29 2022-08-01 21:30:00.000000 anomalo-0.9.1/requirements.txt
+-rw-r--r--   0 johnjoo    (501) staff       (20)       38 2022-09-07 16:54:04.000000 anomalo-0.9.1/setup.cfg
+-rw-r--r--   0 johnjoo    (501) staff       (20)      899 2022-09-07 16:46:35.000000 anomalo-0.9.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `anomalo-0.15.0/LICENSE.txt` & `anomalo-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anomalo-0.15.0/anomalo/client.py` & `anomalo-0.9.1/anomalo/anomalo.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,20 @@
-from __future__ import annotations
+#!/usr/bin/env python
 
 import os
-from typing import Any
 from urllib.parse import urlparse
 
 import requests
 
 
 class Client:
+
     output_style = "json"
 
-    def __init__(
-        self,
-        api_token=None,
-        host=None,
-        proto=None,
-        ssl_cert_verify=None,
-        output_style=None,
-    ):
-        if output_style:
-            self.output_style = output_style
+    def __init__(self, api_token=None, host=None, proto=None, ssl_cert_verify=None):
         self.host = host if host else os.environ.get("ANOMALO_INSTANCE_HOST")
         self.api_token = (
             api_token if api_token else os.environ.get("ANOMALO_API_SECRET_TOKEN")
         )
 
         if not self.host:
             raise RuntimeError(
@@ -42,54 +33,48 @@
         else:
             self.proto = proto if proto else "https"
 
         self.request_headers = {"X-Anomalo-Token": self.api_token}
 
         self.verify = ssl_cert_verify
 
-    def _api_call(self, endpoint, method="GET", empty_response=False, **kwargs) -> Any:
+    def _api_call(self, endpoint, method="GET", **kwargs):
 
         endpoint_url = "{proto}://{host}/api/public/v1/{endpoint}".format(
             proto=self.proto, host=self.host, endpoint=endpoint
         )
 
-        if method in ["PUT", "POST", "PATCH", "DELETE"]:
+        if method in ["PUT", "POST"]:
             request_args = dict(json=kwargs)
         else:
             request_args = dict(params=kwargs)
-
         r = requests.request(
             method,
             endpoint_url,
             headers=self.request_headers,
             verify=self.verify,
             allow_redirects=False,
             **request_args,
         )
 
         if not r.ok:
             raise RuntimeError(r.text)
-        if empty_response:
-            return r
         return r.json() if self.output_style == "json" else r.text
 
     def ping(self):
         return self._api_call("ping")
 
     def get_active_organization_id(self):
         return self._api_call("organization").get("id")
 
     def set_active_organization_id(self, organization_id):
         return self._api_call("organization", method="PUT", id=organization_id).get(
             "id"
         )
 
-    def get_all_organizations(self):
-        return self._api_call("organizations")
-
     def list_warehouses(self):
         return self._api_call("list_warehouses")
 
     def refresh_warehouse(self, warehouse_id):
         return self._api_call(f"warehouse/{warehouse_id}/refresh", method="PUT")
 
     def refresh_warehouse_tables(self, warehouse_id, table_full_names):
@@ -103,56 +88,34 @@
 
     def refresh_warehouse_new_tables(self, warehouse_id):
         return self._api_call(f"warehouse/{warehouse_id}/refresh/new", method="PUT")
 
     def list_notification_channels(self):
         return self._api_call("list_notification_channels")
 
-    def configured_tables(
-        self, check_cadence_type=None, warehouse_id=None, details=True
-    ):
+    def configured_tables(self, check_cadence_type=None, warehouse_id=None):
         return self._api_call(
             "configured_tables",
             check_cadence_type=check_cadence_type,
             warehouse_id=warehouse_id,
-            details=True,
         )
 
-    def tables(self):
-        return self._api_call("tables")
-
-    def filter_tables_by_label(self, label_id):
-        return self._api_call(f"tables?label_id={label_id}")
-
     def get_table_information(self, warehouse_id=None, table_id=None, table_name=None):
         if (not table_id or not warehouse_id) and not table_name:
             raise RuntimeError(
                 "Must specify either warehouse_id & table_id or table_name for get_table_information"
             )
         else:
             return self._api_call(
                 "get_table_information",
                 warehouse_id=warehouse_id,
                 table_id=table_id,
                 table_name=table_name,
             )
 
-    def get_table_profile(self, warehouse_id=None, table_id=None, table_name=None):
-        if (not table_id or not warehouse_id) and not table_name:
-            raise RuntimeError(
-                "Must specify either warehouse_id & table_id or table_name for get_table_profile"
-            )
-        else:
-            return self._api_call(
-                "get_table_profile",
-                warehouse_id=warehouse_id,
-                table_id=table_id,
-                table_name=table_name,
-            )
-
     def get_check_intervals(self, table_id=None, start=None, end=None):
         if not table_id:
             raise RuntimeError("Must specify a table_id for get_check_intervals")
         else:
             results = []
             page = 0
             paged_results = None
@@ -222,88 +185,48 @@
             new_table_id=new_table_id,
             method="POST",
         )
 
     def configure_table(
         self,
         table_id,
-        *,
         check_cadence_type=None,
         definition=None,
         time_column_type=None,
         notify_after=None,
         time_columns=None,
         fresh_after=None,
         interval_skip_expr=None,
         notification_channel_id=None,
         slack_users=None,
         check_cadence_run_at_duration=None,
-        always_alert_on_errors=False,
     ):
         time_columns = [] if time_columns is None else time_columns
         slack_users = {} if slack_users is None else slack_users
 
         return self._api_call(
             "configure_table",
             table_id=table_id,
             method="POST",
             check_cadence_type=check_cadence_type,
             definition=definition,
             time_column_type=time_column_type,
             notify_after=notify_after,
-            notification_channel_id=notification_channel_id,
+            selected_channel=notification_channel_id,
             time_columns=time_columns,
             fresh_after=fresh_after,
             interval_skip_expr=interval_skip_expr,
             slack_users=slack_users,
             check_cadence_run_at_duration=check_cadence_run_at_duration,
-            always_alert_on_errors=always_alert_on_errors,
         )
 
-    def create_table_label_for_organization(self, name):
-        return self._api_call(
-            "table-labels",
-            method="POST",
-            name=name,
-        )
 
-    def list_table_labels_for_organization(self):
-        return self._api_call("table-labels")
+def main():
+    import fire
 
-    def update_table_label_name_for_organization(self, label_id, new_name):
-        return self._api_call(
-            f"table-labels/{label_id}",
-            method="PUT",
-            name=new_name,
-        )
+    Client.output_style = "text"
 
-    def delete_table_label_for_organization(self, label_id):
-        self._api_call(
-            f"table-labels/{label_id}",
-            method="DELETE",
-            empty_response=True,
-        )
+    fire.Fire(Client)
 
-    def merge_table_labels_for_organization(
-        self, source_label_id, destination_label_id
-    ):
-        return self._api_call(
-            f"table-labels/{destination_label_id}/merge",
-            method="POST",
-            source_label_id=source_label_id,
-        )
-
-    def replace_labels_for_table(self, table_id, labels):
-        return self._api_call(
-            f"tables/{table_id}/labels",
-            method="PUT",
-            empty_response=True,
-            labels=labels,
-        )
 
-    def add_new_labels_to_table(self, table_id, labels):
-        return self._api_call(
-            f"tables/{table_id}/labels",
-            method="PATCH",
-            empty_response=True,
-            labels=labels,
-        )
+if __name__ == "__main__":
+    main()
```

### Comparing `anomalo-0.15.0/examples/bulk_rerun.py` & `anomalo-0.9.1/examples/bulk_rerun.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 ML_CHECKS = {
     "MLTime": -100,
     "MLNull": -101,
 }
 ANALYZE_CHECKS = {"ANALYZE_SAMPLE": -103}
 
+# TODO[jason]: this allows them to easily skip cycle dates
 DEFAULT_DAYS_OF_MONTH_TO_SKIP = [1, 7, 14, 21, 28, 29, 30, 31]
 
 api_client = anomalo.Client()
 
 # Run checks against table for all completed intervals from "start" to "end" (defaults to now)
 def _run_checks_sync(table_id, interval_id=None, check_ids=None):
     run_resp = api_client.run_checks(
```

### Comparing `anomalo-0.15.0/examples/sample.py` & `anomalo-0.9.1/examples/sample.py`

 * *Files identical despite different names*

### Comparing `anomalo-0.15.0/setup.py` & `anomalo-0.9.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import re
 
-from setuptools import find_packages, setup
+from setuptools import setup
+
+
+PACKAGE_NAME = "anomalo"
 
 
 def get_version():
     try:
-        f = open(f"anomalo/_version.py")
+        f = open(f"{PACKAGE_NAME}/_version.py")
     except OSError:
         return None
     for line in f.readlines():
         mo = re.match('__version__ = "([^\']+)"', line)
         if mo:
             ver = mo.group(1)
             return ver
@@ -21,18 +24,17 @@
     version=get_version(),
     description="Python bindings for the Anomalo API",
     long_description="A basic REST API client and command line client for Anomalo",
     url="https://anomalo.com",
     author="Anomalo",
     author_email="support@anomalo.com",
     license="license.txt",
-    package=find_packages(),
+    packages=[PACKAGE_NAME],
     install_requires=["requests", "fire"],
     tests_require=[],
-    python_requires=">=3.8",
+    python_requires=">=3.6",
     entry_points={
         "console_scripts": [
-            "anomalo = anomalo:anomalo.main",
+            "anomalo = anomalo:main",
         ]
     },
-    extras_require={"yaml": ["pyyaml>=5.2"]},
 )
```


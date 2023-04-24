# Comparing `tmp/cmem-cmempy-22.3rc3.tar.gz` & `tmp/cmem_cmempy-23.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmem-cmempy-22.3rc3.tar", max compression
+gzip compressed data, was "cmem_cmempy-23.1.tar", max compression
```

## Comparing `cmem-cmempy-22.3rc3.tar` & `cmem_cmempy-23.1.tar`

### file list

```diff
@@ -1,54 +1,55 @@
--rw-r--r--   0        0        0    11357 2022-12-09 08:07:28.451296 cmem-cmempy-22.3rc3/LICENSE
--rw-r--r--   0        0        0      672 2022-12-12 10:27:45.356566 cmem-cmempy-22.3rc3/README-public.md
--rw-r--r--   0        0        0      110 2022-12-13 05:48:01.476674 cmem-cmempy-22.3rc3/cmem/__init__.py
--rw-r--r--   0        0        0       40 2022-12-11 06:08:21.556175 cmem-cmempy-22.3rc3/cmem/cmempy/__init__.py
--rw-r--r--   0        0        0     4426 2022-12-22 22:07:11.323733 cmem-cmempy-22.3rc3/cmem/cmempy/api.py
--rw-r--r--   0        0        0     4288 2022-12-13 05:48:01.476674 cmem-cmempy-22.3rc3/cmem/cmempy/config.py
--rw-r--r--   0        0        0     1062 2022-12-13 05:48:01.476674 cmem-cmempy-22.3rc3/cmem/cmempy/custom_tasks/__init__.py
--rw-r--r--   0        0        0       36 2022-12-11 06:08:21.556175 cmem-cmempy-22.3rc3/cmem/cmempy/dp/__init__.py
--rw-r--r--   0        0        0     1029 2022-12-13 05:48:01.476674 cmem-cmempy-22.3rc3/cmem/cmempy/dp/admin/__init__.py
--rw-r--r--   0        0        0     1014 2022-12-13 06:51:25.936217 cmem-cmempy-22.3rc3/cmem/cmempy/dp/admin/backup.py
--rw-r--r--   0        0        0       42 2022-12-11 06:08:21.560276 cmem-cmempy-22.3rc3/cmem/cmempy/dp/authorization/__init__.py
--rw-r--r--   0        0        0     1232 2022-12-13 05:48:01.476674 cmem-cmempy-22.3rc3/cmem/cmempy/dp/authorization/conditions.py
--rw-r--r--   0        0        0      477 2022-12-13 05:48:01.476674 cmem-cmempy-22.3rc3/cmem/cmempy/dp/authorization/refresh.py
--rw-r--r--   0        0        0      380 2022-12-13 05:48:01.476674 cmem-cmempy-22.3rc3/cmem/cmempy/dp/proxy/__init__.py
--rw-r--r--   0        0        0     6036 2022-12-13 05:48:01.476674 cmem-cmempy-22.3rc3/cmem/cmempy/dp/proxy/graph.py
--rw-r--r--   0        0        0     4159 2022-12-13 05:48:01.476674 cmem-cmempy-22.3rc3/cmem/cmempy/dp/proxy/sparql.py
--rw-r--r--   0        0        0     1244 2022-12-13 05:48:01.476674 cmem-cmempy-22.3rc3/cmem/cmempy/dp/proxy/update.py
--rw-r--r--   0        0        0     1011 2022-12-13 05:48:01.476674 cmem-cmempy-22.3rc3/cmem/cmempy/dp/titles/__init__.py
--rw-r--r--   0        0        0     5905 2022-12-13 07:12:18.385469 cmem-cmempy-22.3rc3/cmem/cmempy/health/__init__.py
--rw-r--r--   0        0        0       31 2022-12-11 06:08:21.560276 cmem-cmempy-22.3rc3/cmem/cmempy/linking/__init__.py
--rw-r--r--   0        0        0     2588 2022-12-13 05:48:01.476674 cmem-cmempy-22.3rc3/cmem/cmempy/linking/linkingtask.py
--rw-r--r--   0        0        0       26 2022-12-11 06:08:21.560276 cmem-cmempy-22.3rc3/cmem/cmempy/plugins/__init__.py
--rw-r--r--   0        0        0     1939 2022-12-13 05:48:01.476674 cmem-cmempy-22.3rc3/cmem/cmempy/plugins/marshalling.py
--rw-r--r--   0        0        0    11191 2022-12-13 06:51:25.940217 cmem-cmempy-22.3rc3/cmem/cmempy/queries/__init__.py
--rw-r--r--   0        0        0       33 2022-12-11 06:08:21.560276 cmem-cmempy-22.3rc3/cmem/cmempy/transform/__init__.py
--rw-r--r--   0        0        0     1090 2022-12-13 05:48:01.476674 cmem-cmempy-22.3rc3/cmem/cmempy/transform/rules/__init__.py
--rw-r--r--   0        0        0     1075 2022-12-13 05:48:01.476674 cmem-cmempy-22.3rc3/cmem/cmempy/transform/rules/transformationrule.py
--rw-r--r--   0        0        0     1240 2022-12-13 05:48:01.476674 cmem-cmempy-22.3rc3/cmem/cmempy/transform/transformationtask.py
--rw-r--r--   0        0        0     3587 2022-12-22 22:03:49.464356 cmem-cmempy-22.3rc3/cmem/cmempy/vocabularies/__init__.py
--rw-r--r--   0        0        0      500 2022-12-13 05:48:01.476674 cmem-cmempy-22.3rc3/cmem/cmempy/workflow/__init__.py
--rw-r--r--   0        0        0     4502 2022-12-13 05:48:01.476674 cmem-cmempy-22.3rc3/cmem/cmempy/workflow/workflow.py
--rw-r--r--   0        0        0      131 2022-12-13 06:51:25.940217 cmem-cmempy-22.3rc3/cmem/cmempy/workflow/workflows.py
--rw-r--r--   0        0        0     1873 2022-12-13 05:48:01.476674 cmem-cmempy-22.3rc3/cmem/cmempy/workspace/__init__.py
--rw-r--r--   0        0        0      340 2022-12-13 05:48:01.476674 cmem-cmempy-22.3rc3/cmem/cmempy/workspace/activities/__init__.py
--rw-r--r--   0        0        0      914 2022-12-13 05:48:01.476674 cmem-cmempy-22.3rc3/cmem/cmempy/workspace/activities/projectactivities.py
--rw-r--r--   0        0        0     2281 2022-12-13 05:48:01.476674 cmem-cmempy-22.3rc3/cmem/cmempy/workspace/activities/projectactivity.py
--rw-r--r--   0        0        0     3164 2022-12-13 05:48:01.476674 cmem-cmempy-22.3rc3/cmem/cmempy/workspace/activities/taskactivities.py
--rw-r--r--   0        0        0     2323 2022-12-13 05:48:01.476674 cmem-cmempy-22.3rc3/cmem/cmempy/workspace/activities/taskactivity.py
--rw-r--r--   0        0        0      744 2022-12-13 05:48:01.476674 cmem-cmempy-22.3rc3/cmem/cmempy/workspace/export_/__init__.py
--rw-r--r--   0        0        0     1540 2022-12-13 05:48:01.480665 cmem-cmempy-22.3rc3/cmem/cmempy/workspace/import_/__init__.py
--rw-r--r--   0        0        0      454 2022-12-13 05:48:01.480665 cmem-cmempy-22.3rc3/cmem/cmempy/workspace/projects/__init__.py
--rw-r--r--   0        0        0       45 2022-12-11 06:08:21.560276 cmem-cmempy-22.3rc3/cmem/cmempy/workspace/projects/datasets/__init__.py
--rw-r--r--   0        0        0     2369 2022-12-13 05:48:01.480665 cmem-cmempy-22.3rc3/cmem/cmempy/workspace/projects/datasets/dataset.py
--rw-r--r--   0        0        0      748 2022-12-13 05:48:01.480665 cmem-cmempy-22.3rc3/cmem/cmempy/workspace/projects/export_.py
--rw-r--r--   0        0        0     4945 2022-12-13 05:48:01.480665 cmem-cmempy-22.3rc3/cmem/cmempy/workspace/projects/import_.py
--rw-r--r--   0        0        0     2007 2022-12-13 05:48:01.480665 cmem-cmempy-22.3rc3/cmem/cmempy/workspace/projects/project.py
--rw-r--r--   0        0        0      956 2022-12-13 05:48:01.480665 cmem-cmempy-22.3rc3/cmem/cmempy/workspace/projects/resources/__init__.py
--rw-r--r--   0        0        0     4963 2022-12-13 05:48:01.480665 cmem-cmempy-22.3rc3/cmem/cmempy/workspace/projects/resources/resource.py
--rw-r--r--   0        0        0     2292 2022-12-13 06:51:25.940217 cmem-cmempy-22.3rc3/cmem/cmempy/workspace/python.py
--rw-r--r--   0        0        0     1075 2022-12-13 05:48:01.480665 cmem-cmempy-22.3rc3/cmem/cmempy/workspace/search/__init__.py
--rw-r--r--   0        0        0     1078 2022-12-13 05:48:01.480665 cmem-cmempy-22.3rc3/cmem/cmempy/workspace/tasks/__init__.py
--rw-r--r--   0        0        0     1898 2022-12-23 07:30:21.831209 cmem-cmempy-22.3rc3/pyproject.toml
--rw-r--r--   0        0        0     2160 1970-01-01 00:00:00.000000 cmem-cmempy-22.3rc3/setup.py
--rw-r--r--   0        0        0     1948 1970-01-01 00:00:00.000000 cmem-cmempy-22.3rc3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-01-18 07:28:45.599930 cmem_cmempy-23.1/LICENSE
+-rw-r--r--   0        0        0      651 2023-04-24 07:06:13.952436 cmem_cmempy-23.1/README-public.md
+-rw-r--r--   0        0        0      110 2023-04-24 07:06:13.952744 cmem_cmempy-23.1/cmem/__init__.py
+-rw-r--r--   0        0        0       40 2023-04-24 07:06:13.952818 cmem_cmempy-23.1/cmem/cmempy/__init__.py
+-rw-r--r--   0        0        0     4456 2023-04-24 07:06:13.953043 cmem_cmempy-23.1/cmem/cmempy/api.py
+-rw-r--r--   0        0        0     4970 2023-04-24 07:06:13.953161 cmem_cmempy-23.1/cmem/cmempy/config.py
+-rw-r--r--   0        0        0     1062 2023-04-24 07:06:13.953244 cmem_cmempy-23.1/cmem/cmempy/custom_tasks/__init__.py
+-rw-r--r--   0        0        0       36 2023-04-24 07:06:13.953307 cmem_cmempy-23.1/cmem/cmempy/dp/__init__.py
+-rw-r--r--   0        0        0     1029 2023-04-24 07:06:13.953384 cmem_cmempy-23.1/cmem/cmempy/dp/admin/__init__.py
+-rw-r--r--   0        0        0     1014 2023-04-24 07:06:13.953446 cmem_cmempy-23.1/cmem/cmempy/dp/admin/backup.py
+-rw-r--r--   0        0        0       42 2023-04-24 07:06:13.953524 cmem_cmempy-23.1/cmem/cmempy/dp/authorization/__init__.py
+-rw-r--r--   0        0        0     1232 2023-04-24 07:06:13.953586 cmem_cmempy-23.1/cmem/cmempy/dp/authorization/conditions.py
+-rw-r--r--   0        0        0      477 2023-04-24 07:06:13.953641 cmem_cmempy-23.1/cmem/cmempy/dp/authorization/refresh.py
+-rw-r--r--   0        0        0      380 2023-04-24 07:06:13.953720 cmem_cmempy-23.1/cmem/cmempy/dp/proxy/__init__.py
+-rw-r--r--   0        0        0     6036 2023-04-24 07:06:13.953793 cmem_cmempy-23.1/cmem/cmempy/dp/proxy/graph.py
+-rw-r--r--   0        0        0     4159 2023-04-24 07:06:13.953863 cmem_cmempy-23.1/cmem/cmempy/dp/proxy/sparql.py
+-rw-r--r--   0        0        0     1244 2023-04-24 07:06:13.953918 cmem_cmempy-23.1/cmem/cmempy/dp/proxy/update.py
+-rw-r--r--   0        0        0     1011 2023-04-24 07:06:13.954002 cmem_cmempy-23.1/cmem/cmempy/dp/titles/__init__.py
+-rw-r--r--   0        0        0     5905 2023-04-24 07:06:13.954105 cmem_cmempy-23.1/cmem/cmempy/health/__init__.py
+-rw-r--r--   0        0        0      519 2023-04-24 07:06:13.954373 cmem_cmempy-23.1/cmem/cmempy/keycloak/group.py
+-rw-r--r--   0        0        0     3630 2023-04-24 07:06:13.954464 cmem_cmempy-23.1/cmem/cmempy/keycloak/user.py
+-rw-r--r--   0        0        0       31 2023-04-24 07:06:13.954530 cmem_cmempy-23.1/cmem/cmempy/linking/__init__.py
+-rw-r--r--   0        0        0     2588 2023-04-24 07:06:13.954585 cmem_cmempy-23.1/cmem/cmempy/linking/linkingtask.py
+-rw-r--r--   0        0        0       26 2023-04-24 07:06:13.954658 cmem_cmempy-23.1/cmem/cmempy/plugins/__init__.py
+-rw-r--r--   0        0        0     1939 2023-04-24 07:06:13.954716 cmem_cmempy-23.1/cmem/cmempy/plugins/marshalling.py
+-rw-r--r--   0        0        0    11190 2023-04-24 07:06:13.955001 cmem_cmempy-23.1/cmem/cmempy/queries/__init__.py
+-rw-r--r--   0        0        0       33 2023-04-24 07:06:13.955070 cmem_cmempy-23.1/cmem/cmempy/transform/__init__.py
+-rw-r--r--   0        0        0     1090 2023-04-24 07:06:13.955142 cmem_cmempy-23.1/cmem/cmempy/transform/rules/__init__.py
+-rw-r--r--   0        0        0     1075 2023-04-24 07:06:13.955192 cmem_cmempy-23.1/cmem/cmempy/transform/rules/transformationrule.py
+-rw-r--r--   0        0        0     1240 2023-04-24 07:06:13.955247 cmem_cmempy-23.1/cmem/cmempy/transform/transformationtask.py
+-rw-r--r--   0        0        0     3597 2023-04-24 07:06:13.955338 cmem_cmempy-23.1/cmem/cmempy/vocabularies/__init__.py
+-rw-r--r--   0        0        0      500 2023-04-24 07:06:13.955412 cmem_cmempy-23.1/cmem/cmempy/workflow/__init__.py
+-rw-r--r--   0        0        0     4502 2023-04-24 07:06:13.955473 cmem_cmempy-23.1/cmem/cmempy/workflow/workflow.py
+-rw-r--r--   0        0        0      131 2023-04-24 07:06:13.955517 cmem_cmempy-23.1/cmem/cmempy/workflow/workflows.py
+-rw-r--r--   0        0        0     1873 2023-04-24 07:06:13.955597 cmem_cmempy-23.1/cmem/cmempy/workspace/__init__.py
+-rw-r--r--   0        0        0      340 2023-04-24 07:06:13.955666 cmem_cmempy-23.1/cmem/cmempy/workspace/activities/__init__.py
+-rw-r--r--   0        0        0      914 2023-04-24 07:06:13.955719 cmem_cmempy-23.1/cmem/cmempy/workspace/activities/projectactivities.py
+-rw-r--r--   0        0        0     2281 2023-04-24 07:06:13.955774 cmem_cmempy-23.1/cmem/cmempy/workspace/activities/projectactivity.py
+-rw-r--r--   0        0        0     3164 2023-04-24 07:06:13.955836 cmem_cmempy-23.1/cmem/cmempy/workspace/activities/taskactivities.py
+-rw-r--r--   0        0        0     2323 2023-04-24 07:06:13.955884 cmem_cmempy-23.1/cmem/cmempy/workspace/activities/taskactivity.py
+-rw-r--r--   0        0        0      744 2023-04-24 07:06:13.955973 cmem_cmempy-23.1/cmem/cmempy/workspace/export_/__init__.py
+-rw-r--r--   0        0        0     1540 2023-04-24 07:06:13.956048 cmem_cmempy-23.1/cmem/cmempy/workspace/import_/__init__.py
+-rw-r--r--   0        0        0      454 2023-04-24 07:06:13.956113 cmem_cmempy-23.1/cmem/cmempy/workspace/projects/__init__.py
+-rw-r--r--   0        0        0       45 2023-04-24 07:06:13.956183 cmem_cmempy-23.1/cmem/cmempy/workspace/projects/datasets/__init__.py
+-rw-r--r--   0        0        0     2369 2023-04-24 07:06:13.956242 cmem_cmempy-23.1/cmem/cmempy/workspace/projects/datasets/dataset.py
+-rw-r--r--   0        0        0      748 2023-04-24 07:06:13.956330 cmem_cmempy-23.1/cmem/cmempy/workspace/projects/export_.py
+-rw-r--r--   0        0        0     4945 2023-04-24 07:06:13.956394 cmem_cmempy-23.1/cmem/cmempy/workspace/projects/import_.py
+-rw-r--r--   0        0        0     2007 2023-04-24 07:06:13.956449 cmem_cmempy-23.1/cmem/cmempy/workspace/projects/project.py
+-rw-r--r--   0        0        0      960 2023-04-24 07:06:13.956713 cmem_cmempy-23.1/cmem/cmempy/workspace/projects/resources/__init__.py
+-rw-r--r--   0        0        0     6089 2023-04-24 07:06:13.956822 cmem_cmempy-23.1/cmem/cmempy/workspace/projects/resources/resource.py
+-rw-r--r--   0        0        0     2292 2023-04-24 07:06:13.956887 cmem_cmempy-23.1/cmem/cmempy/workspace/python.py
+-rw-r--r--   0        0        0     1075 2023-04-24 07:06:13.956970 cmem_cmempy-23.1/cmem/cmempy/workspace/search/__init__.py
+-rw-r--r--   0        0        0     1078 2023-04-24 07:06:13.957053 cmem_cmempy-23.1/cmem/cmempy/workspace/tasks/__init__.py
+-rw-r--r--   0        0        0     2048 2023-04-24 11:55:27.286209 cmem_cmempy-23.1/pyproject.toml
+-rw-r--r--   0        0        0     2005 1970-01-01 00:00:00.000000 cmem_cmempy-23.1/PKG-INFO
```

### Comparing `cmem-cmempy-22.3rc3/LICENSE` & `cmem_cmempy-23.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cmem-cmempy-22.3rc3/README-public.md` & `cmem_cmempy-23.1/README-public.md`

 * *Files 27% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 
 cmempy is intended for Linked Data Experts to interface with the eccenca Corporate Memory backend components DataIntegration and DataPlatform.
 
 The cmempy manual including basic usage patterns and configuration is available at:
 
 [https://eccenca.com/go/cmempy](https://eccenca.com/go/cmempy)
 
-cmempy works with Python 2.7 as well as with Python 3.
+cmempy is tests with python >3.9.
```

### Comparing `cmem-cmempy-22.3rc3/cmem/cmempy/api.py` & `cmem_cmempy-23.1/cmem/cmempy/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         params=params,
         files=files,
     ).content
     return json.loads(response.decode("utf-8"))
 
 
 def _request(method=None, url=None, **kwargs):
-    # pylint: disable=E0012
+    # pylint: disable=missing-timeout
     return requests.api.request(method, url, verify=config.get_ssl_verify(), **kwargs)
 
 
 # pylint: disable-msg=too-many-arguments
 def request(
     uri,
     method="GET",
@@ -136,15 +136,15 @@
             headers=headers,
             data=data,
             params=params,
             files=files,
             stream=stream,
         )
     else:
-        raise Exception("Unknown HTTP request method")
+        raise requests.exceptions.HTTPError("Unknown HTTP request method")
     if response.status_code not in [
         requests.status_codes.codes.ok,
         requests.status_codes.codes.no_content,
         requests.status_codes.codes.created,
     ]:
         if config.is_chatty():
             print(
```

### Comparing `cmem-cmempy-22.3rc3/cmem/cmempy/config.py` & `cmem_cmempy-23.1/cmem/cmempy/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,14 +27,26 @@
     return str(
         os.environ.get(
             "CMEM_BASE_URI", f"{get_cmem_base_protocol()}://{get_cmem_base_domain()}"
         ).strip("/")
     )
 
 
+def get_keycloak_base_uri():
+    """Get the KEYCLOAK_BASE_URI config value (no ending slash)."""
+    return str(
+        os.environ.get("KEYCLOAK_BASE_URI", f"{get_cmem_base_uri()}/auth").strip("/")
+    )
+
+
+def get_keycloak_realm_id():
+    """Get the KEYCLOAK_REALM_NAME config value (no ending slash)."""
+    return str(os.environ.get("KEYCLOAK_REALM_ID", "cmem").strip("/"))
+
+
 def get_ssl_verify():
     """Get the SSL_VERIFY config value."""
     ssl_verify = os.environ.get("SSL_VERIFY", "True")
     if ssl_verify.lower() == "false":
         ssl_verify = False
     else:
         ssl_verify = True
@@ -63,15 +75,25 @@
     return os.environ.get("DP_API_ENDPOINT", f"{get_cmem_base_uri()}/dataplatform")
 
 
 def get_oauth_token_uri():
     """Get the OAUTH_TOKEN_URI config value."""
     return os.environ.get(
         "OAUTH_TOKEN_URI",
-        f"{get_cmem_base_uri()}/auth/realms/cmem/protocol/openid-connect/token",
+        f"{get_keycloak_base_uri()}/realms/{get_keycloak_realm_id()}/protocol/"
+        "openid-connect/token",
+    )
+
+
+def get_oauth_authorization_uri():
+    """Get the OAUTH_AUTHORIZATION_URI config value."""
+    return os.environ.get(
+        "OAUTH_AUTHORIZATION_URI",
+        f"{get_keycloak_base_uri()}/realms/{get_keycloak_realm_id()}/protocol/"
+        "openid-connect/auth",
     )
 
 
 def get_oauth_grant_type():
     """Get the OAUTH_GRANT_TYPE config value."""
     valid_values = ("password", "client_credentials", "prefetched_token")
     value = os.environ.get("OAUTH_GRANT_TYPE", "client_credentials")
```

### Comparing `cmem-cmempy-22.3rc3/cmem/cmempy/custom_tasks/__init__.py` & `cmem_cmempy-23.1/cmem/cmempy/custom_tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem-cmempy-22.3rc3/cmem/cmempy/dp/admin/__init__.py` & `cmem_cmempy-23.1/cmem/cmempy/dp/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem-cmempy-22.3rc3/cmem/cmempy/dp/admin/backup.py` & `cmem_cmempy-23.1/cmem/cmempy/dp/admin/backup.py`

 * *Files identical despite different names*

### Comparing `cmem-cmempy-22.3rc3/cmem/cmempy/dp/authorization/conditions.py` & `cmem_cmempy-23.1/cmem/cmempy/dp/authorization/conditions.py`

 * *Files identical despite different names*

### Comparing `cmem-cmempy-22.3rc3/cmem/cmempy/dp/proxy/graph.py` & `cmem_cmempy-23.1/cmem/cmempy/dp/proxy/graph.py`

 * *Files identical despite different names*

### Comparing `cmem-cmempy-22.3rc3/cmem/cmempy/dp/proxy/sparql.py` & `cmem_cmempy-23.1/cmem/cmempy/dp/proxy/sparql.py`

 * *Files identical despite different names*

### Comparing `cmem-cmempy-22.3rc3/cmem/cmempy/dp/proxy/update.py` & `cmem_cmempy-23.1/cmem/cmempy/dp/proxy/update.py`

 * *Files identical despite different names*

### Comparing `cmem-cmempy-22.3rc3/cmem/cmempy/dp/titles/__init__.py` & `cmem_cmempy-23.1/cmem/cmempy/dp/titles/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem-cmempy-22.3rc3/cmem/cmempy/health/__init__.py` & `cmem_cmempy-23.1/cmem/cmempy/health/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem-cmempy-22.3rc3/cmem/cmempy/linking/linkingtask.py` & `cmem_cmempy-23.1/cmem/cmempy/linking/linkingtask.py`

 * *Files identical despite different names*

### Comparing `cmem-cmempy-22.3rc3/cmem/cmempy/plugins/marshalling.py` & `cmem_cmempy-23.1/cmem/cmempy/plugins/marshalling.py`

 * *Files identical despite different names*

### Comparing `cmem-cmempy-22.3rc3/cmem/cmempy/queries/__init__.py` & `cmem_cmempy-23.1/cmem/cmempy/queries/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,15 +270,15 @@
         """Initialize the catalog."""
         self.queries = None
 
     def get_query(self, identifier, placeholder=None):
         """Get a query by giving an url, a short_url or a file name."""
         if os.path.isfile(identifier):
             # do not fetch the catalog in case a file is requested
-            with open(identifier, "rU", encoding="UTF-8") as file_handle:
+            with open(identifier, "r", encoding="UTF-8") as file_handle:
                 return SparqlQuery(
                     file_handle.read(),
                     label="query from file " + identifier,
                     origin="file",
                     placeholder=placeholder,
                 )
         queries = self.get_queries()
```

### Comparing `cmem-cmempy-22.3rc3/cmem/cmempy/transform/rules/__init__.py` & `cmem_cmempy-23.1/cmem/cmempy/transform/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem-cmempy-22.3rc3/cmem/cmempy/transform/rules/transformationrule.py` & `cmem_cmempy-23.1/cmem/cmempy/transform/rules/transformationrule.py`

 * *Files identical despite different names*

### Comparing `cmem-cmempy-22.3rc3/cmem/cmempy/transform/transformationtask.py` & `cmem_cmempy-23.1/cmem/cmempy/transform/transformationtask.py`

 * *Files identical despite different names*

### Comparing `cmem-cmempy-22.3rc3/cmem/cmempy/vocabularies/__init__.py` & `cmem_cmempy-23.1/cmem/cmempy/vocabularies/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
 
 def install_vocabulary(iri, catalog_uri=DEFAULT_CATALOG_GRAPH):
     """Install a vocabulary."""
     vocab = get_vocabulary(iri, catalog_uri=catalog_uri)
     if "downloadUrl" not in vocab:
         raise KeyError("no downloadable URL found")
-    # pylint: disable=E0012
+    # pylint: disable=missing-timeout
     response = requests.api.request(
         "GET",
         vocab["downloadUrl"],
         verify=True,
     )
     if response.status_code is requests.status_codes.codes.ok:
         response.raise_for_status()
```

### Comparing `cmem-cmempy-22.3rc3/cmem/cmempy/workflow/workflow.py` & `cmem_cmempy-23.1/cmem/cmempy/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `cmem-cmempy-22.3rc3/cmem/cmempy/workspace/__init__.py` & `cmem_cmempy-23.1/cmem/cmempy/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem-cmempy-22.3rc3/cmem/cmempy/workspace/activities/projectactivities.py` & `cmem_cmempy-23.1/cmem/cmempy/workspace/activities/projectactivities.py`

 * *Files identical despite different names*

### Comparing `cmem-cmempy-22.3rc3/cmem/cmempy/workspace/activities/projectactivity.py` & `cmem_cmempy-23.1/cmem/cmempy/workspace/activities/projectactivity.py`

 * *Files identical despite different names*

### Comparing `cmem-cmempy-22.3rc3/cmem/cmempy/workspace/activities/taskactivities.py` & `cmem_cmempy-23.1/cmem/cmempy/workspace/activities/taskactivities.py`

 * *Files identical despite different names*

### Comparing `cmem-cmempy-22.3rc3/cmem/cmempy/workspace/activities/taskactivity.py` & `cmem_cmempy-23.1/cmem/cmempy/workspace/activities/taskactivity.py`

 * *Files identical despite different names*

### Comparing `cmem-cmempy-22.3rc3/cmem/cmempy/workspace/export_/__init__.py` & `cmem_cmempy-23.1/cmem/cmempy/workspace/export_/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem-cmempy-22.3rc3/cmem/cmempy/workspace/import_/__init__.py` & `cmem_cmempy-23.1/cmem/cmempy/workspace/import_/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem-cmempy-22.3rc3/cmem/cmempy/workspace/projects/datasets/dataset.py` & `cmem_cmempy-23.1/cmem/cmempy/workspace/projects/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `cmem-cmempy-22.3rc3/cmem/cmempy/workspace/projects/export_.py` & `cmem_cmempy-23.1/cmem/cmempy/workspace/projects/export_.py`

 * *Files identical despite different names*

### Comparing `cmem-cmempy-22.3rc3/cmem/cmempy/workspace/projects/import_.py` & `cmem_cmempy-23.1/cmem/cmempy/workspace/projects/import_.py`

 * *Files identical despite different names*

### Comparing `cmem-cmempy-22.3rc3/cmem/cmempy/workspace/projects/project.py` & `cmem_cmempy-23.1/cmem/cmempy/workspace/projects/project.py`

 * *Files identical despite different names*

### Comparing `cmem-cmempy-22.3rc3/cmem/cmempy/workspace/projects/resources/__init__.py` & `cmem_cmempy-23.1/cmem/cmempy/workspace/projects/resources/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,10 +21,10 @@
 
 def get_all_resources():
     """Get all resources of all projects."""
     resources = []
     for project_id in [_["name"] for _ in get_projects()]:
         for resource in list(get_resources(project_id)):
             resource["project"] = project_id
-            resource["id"] = project_id + ":" + resource["name"]
+            resource["id"] = project_id + ":" + resource["fullPath"]
             resources.append(resource)
     return resources
```

### Comparing `cmem-cmempy-22.3rc3/cmem/cmempy/workspace/projects/resources/resource.py` & `cmem_cmempy-23.1/cmem/cmempy/workspace/projects/resources/resource.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,63 @@
 """API methods for working with single resources."""
 import json
+from typing import Optional
+from urllib.parse import quote_plus
 
 import requests
 from cmem.cmempy import config
 
 from cmem.cmempy.api import request, send_request
 
 
-def get_resource_uri():
-    """Get endpoint URI pattern for a resource."""
-    path = "/workspace/projects/{}/resources/{}"
-    return config.get_di_api_endpoint() + path
-
-
-def get_metadata_uri():
-    """Get metadata endpoint URI pattern for a resource."""
-    path = "/workspace/projects/{}/resources/{}/metadata"
-    return config.get_di_api_endpoint() + path
+def get_resource_uri(
+    project_name: Optional[str] = None,
+    resource_name: Optional[str] = None,
+    sub_path: Optional[str] = None,
+) -> str:
+    """
+    Get the endpoint URI pattern for a resource OR get
+    the full URI in case project and resource is given.
+
+    Args:
+        project_name: the project ID as a string
+        resource_name: the resource path
+        sub_path: None, "metadata" or "usage"
+
+    Note: resource_name will be URL encoded before request.
+    """
+    path = "/workspace/projects/{}/files?path={}"
+    # sub_path can be used to request a sub-API of the files API
+    if sub_path:
+        path = path.replace("files?", f"files/{sub_path}?")
+    path = config.get_di_api_endpoint() + path
+    if not project_name and not resource_name:
+        return path
+    if project_name and resource_name:
+        return path.format(project_name, quote_plus(resource_name))
+    raise ValueError(
+        "Either give project_name AND resource_name or give none of them"
+        " and get the pattern only."
+    )
 
 
 def get_resource(project_name, resource_name):
     """GET resource.
 
     Args:
         project_name (str): The project ID in the workspace.
         resource_name (str): The resource ID/name in the workspace.
 
     Returns:
         requests.Response object
     """
-    response = send_request(
-        get_resource_uri().format(project_name, resource_name), method="GET"
+    resource_url = get_resource_uri(
+        project_name=project_name, resource_name=resource_name
     )
+    response = send_request(resource_url, method="GET")
     return response
 
 
 def resource_exist(project_name, resource_name):
     """Check if a resource exist.
 
     A return value of true means the resource exists. A return value of true
@@ -63,29 +85,34 @@
     Args:
         project_name (str): The project ID in the workspace.
         resource_name (str): The resource ID/name in the workspace.
 
     Returns:
         requests.Response object
     """
-    resource_url = get_resource_uri().format(project_name, resource_name)
+    resource_url = get_resource_uri(
+        project_name=project_name, resource_name=resource_name
+    )
     return request(resource_url, method="GET", stream=True)
 
 
 def make_new_resource(project_name, resource_name, data=None, files=None):
     """PUT create new resource.
 
     Args:
         project_name (str): The project ID in the workspace.
         resource_name (str): The resource ID/name in the workspace.
         data (dict): Dictionary (see requests.request) for the body
         files (dict): Dictionary (see requests.request) for multipart upload
     """
+    resource_url = get_resource_uri(
+        project_name=project_name, resource_name=resource_name
+    )
     send_request(
-        get_resource_uri().format(project_name, resource_name),
+        resource_url,
         method="PUT",
         data=data,
         files=files,
     )
 
 
 def create_resource(project_name, resource_name, file_resource=None, replace=False):
@@ -106,60 +133,66 @@
     """
     if not file_resource:
         raise ValueError("Parameter file_name is needed.")
     if not replace and resource_exist(project_name, resource_name):
         raise ValueError(
             f"Resource {resource_name} already exists " f"in project {project_name}."
         )
+    resource_url = get_resource_uri(
+        project_name=project_name, resource_name=resource_name
+    )
     # https://requests.readthedocs.io/en/latest/user/advanced/#streaming-uploads
     with file_resource as file:
         response = request(
-            get_resource_uri().format(project_name, resource_name),
+            resource_url,
             method="PUT",
             stream=True,
             data=file,
         )
     return response
 
 
 def delete_resource(project_name, resource_name):
     """DELETE remove existing resource.
 
     Args:
         project_name (str): The project ID in the workspace.
         resource_name (str): The resource ID/name in the workspace.
     """
-    send_request(
-        get_resource_uri().format(project_name, resource_name), method="DELETE"
+    resource_url = get_resource_uri(
+        project_name=project_name, resource_name=resource_name
     )
+    send_request(resource_url, method="DELETE")
 
 
 def get_resource_metadata(project_name, resource_name):
     """GET retrieve resource metadata.
 
     Args:
         project_name (str): The project ID in the workspace.
         resource_name (str): The resource ID/name in the workspace.
 
     Returns:
         Depends on what json.loads gives back
     """
-    response = send_request(
-        get_metadata_uri().format(project_name, resource_name), method="GET"
+    resource_url = get_resource_uri(
+        project_name=project_name, resource_name=resource_name, sub_path="metadata"
     )
+    response = send_request(resource_url, method="GET")
     return json.loads(response.decode("utf-8"))
 
 
 def get_resource_usage_data(project_name, resource_name):
     """GET retrieve the usage data of a resource.
 
     Args:
         project_name (str): The project ID in the workspace.
         resource_name (str): The resource ID/name in the workspace.
 
     Returns:
         Depends on what json.loads gives back
     """
-    response = send_request(
-        get_resource_uri().format(project_name, resource_name) + "/usage", method="GET"
+    resource_url = get_resource_uri(
+        project_name=project_name, resource_name=resource_name, sub_path="usage"
     )
+    response = send_request(resource_url, method="GET")
     return json.loads(response.decode("utf-8"))
```

### Comparing `cmem-cmempy-22.3rc3/cmem/cmempy/workspace/python.py` & `cmem_cmempy-23.1/cmem/cmempy/workspace/python.py`

 * *Files identical despite different names*

### Comparing `cmem-cmempy-22.3rc3/cmem/cmempy/workspace/search/__init__.py` & `cmem_cmempy-23.1/cmem/cmempy/workspace/search/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem-cmempy-22.3rc3/cmem/cmempy/workspace/tasks/__init__.py` & `cmem_cmempy-23.1/cmem/cmempy/workspace/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem-cmempy-22.3rc3/pyproject.toml` & `cmem_cmempy-23.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmem-cmempy"
-version = "22.3rc3"
+version = "23.1"
 license = "Apache-2.0"
 description = "API wrapper for eccenca Corporate Memory"
 authors = ["eccenca GmbH <cmempy-developer@eccenca.com>"]
 maintainers = ["Sebastian Tramp <sebastian.tramp@eccenca.com>"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
@@ -20,40 +20,43 @@
 homepage = "https://eccenca.com/go/cmempy"
 readme = "README-public.md"
 packages = [
     { include = "cmem" }
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-certifi = "*"
-pyparsing = "*"
-pysocks = "*"
-rdflib = "*"
-requests = "*"
-requests-toolbelt = "*"
-six = "*"
+python = "^3.9"
+certifi = "^2022.12.7"
+pyparsing = "^3.0.9"
+pysocks = "^1.7.1"
+rdflib = "^6.2.0"
+requests = "^2.28.1"
+requests-toolbelt = "^0.10.1"
+six = "^1.16.0"
 
-[tool.poetry.dev-dependencies]
-bandit = "*"
-black = "*"
-coverage = "*"
+[tool.poetry.group.dev.dependencies]
+bandit = "^1.7.2"
+black = "^22.1.0"
+coverage = "^6.3.2"
+coverage-badge = "^1.1.0"
 defusedxml = "^0.7.1"
+flake8 = "^6.0.0"
 genbadge = "^1.0.6"
-mypy = "*"
-nose = "^1.3.7"
-pre-commit = "*"
+mypy = "^0.931"
+pre-commit = "2.20.0"
 pylint-junit = "^0.3.2"
-pytest = "*"
-pytest-cov = "*"
+pytest = "^7.0"
+pytest-cov = "^4.0.0"
+pytest-memray = "^1.3.0"
 safety = "^1.10.3"
 types-requests = "^2.28.11.5"
+wheel = "^0.38.4"
 
 [build-system]
-requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
+requires = ["poetry-core>=1.2.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 dirty = true
```

### Comparing `cmem-cmempy-22.3rc3/PKG-INFO` & `cmem_cmempy-23.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 Metadata-Version: 2.1
 Name: cmem-cmempy
-Version: 22.3rc3
+Version: 23.1
 Summary: API wrapper for eccenca Corporate Memory
 Home-page: https://eccenca.com/go/cmempy
 License: Apache-2.0
 Author: eccenca GmbH
 Author-email: cmempy-developer@eccenca.com
 Maintainer: Sebastian Tramp
 Maintainer-email: sebastian.tramp@eccenca.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
-Requires-Dist: certifi
-Requires-Dist: pyparsing
-Requires-Dist: pysocks
-Requires-Dist: rdflib
-Requires-Dist: requests
-Requires-Dist: requests-toolbelt
-Requires-Dist: six
+Requires-Dist: certifi (>=2022.12.7,<2023.0.0)
+Requires-Dist: pyparsing (>=3.0.9,<4.0.0)
+Requires-Dist: pysocks (>=1.7.1,<2.0.0)
+Requires-Dist: rdflib (>=6.2.0,<7.0.0)
+Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: requests-toolbelt (>=0.10.1,<0.11.0)
+Requires-Dist: six (>=1.16.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # cmempy
 
 cmempy is a Python API wrapper for [eccenca Corporate Memory](https://documentation.eccenca.com/).
 
 ## Installation
@@ -51,9 +50,9 @@
 
 cmempy is intended for Linked Data Experts to interface with the eccenca Corporate Memory backend components DataIntegration and DataPlatform.
 
 The cmempy manual including basic usage patterns and configuration is available at:
 
 [https://eccenca.com/go/cmempy](https://eccenca.com/go/cmempy)
 
-cmempy works with Python 2.7 as well as with Python 3.
+cmempy is tests with python >3.9.
```


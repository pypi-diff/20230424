# Comparing `tmp/py_seasnake-0.1.0.tar.gz` & `tmp/py_seasnake-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_seasnake-0.1.0.tar", max compression
+gzip compressed data, was "py_seasnake-0.2.0.tar", max compression
```

## Comparing `py_seasnake-0.1.0.tar` & `py_seasnake-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1070 2023-04-21 21:00:11.124489 py_seasnake-0.1.0/LICENSE
--rw-r--r--   0        0        0      729 2023-04-22 00:46:32.535636 py_seasnake-0.1.0/README.md
--rw-r--r--   0        0        0     1164 2023-04-22 00:46:34.305163 py_seasnake-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-16 18:55:51.792232 py_seasnake-0.1.0/seasnake/__init__.py
--rw-r--r--   0        0        0     6830 2023-04-20 16:05:44.296893 py_seasnake-0.1.0/seasnake/auth.py
--rw-r--r--   0        0        0     3572 2023-04-21 23:01:16.416392 py_seasnake-0.1.0/seasnake/base.py
--rw-r--r--   0        0        0     2380 2023-04-21 22:30:38.616574 py_seasnake-0.1.0/seasnake/projects.py
--rw-r--r--   0        0        0      386 2023-04-20 15:10:20.566010 py_seasnake-0.1.0/seasnake/summaries/__init__.py
--rw-r--r--   0        0        0     1738 2023-04-21 22:31:29.461277 py_seasnake-0.1.0/seasnake/summaries/benthic_lit.py
--rw-r--r--   0        0        0     1845 2023-04-21 22:32:25.433137 py_seasnake-0.1.0/seasnake/summaries/benthic_photo_quadrat.py
--rw-r--r--   0        0        0     1738 2023-04-21 22:32:24.635527 py_seasnake-0.1.0/seasnake/summaries/benthic_pit.py
--rw-r--r--   0        0        0     2245 2023-04-21 22:32:24.635238 py_seasnake-0.1.0/seasnake/summaries/bleaching.py
--rw-r--r--   0        0        0     1502 2023-04-21 22:32:24.635454 py_seasnake-0.1.0/seasnake/summaries/fish_belt.py
--rw-r--r--   0        0        0     1841 2023-04-21 22:32:24.648601 py_seasnake-0.1.0/seasnake/summaries/habitat_complexity.py
--rw-r--r--   0        0        0     2188 2023-04-21 22:54:26.201337 py_seasnake-0.1.0/seasnake/summaries/sample_event.py
--rw-r--r--   0        0        0     1744 1970-01-01 00:00:00.000000 py_seasnake-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-21 21:00:11.124489 py_seasnake-0.2.0/LICENSE
+-rw-r--r--   0        0        0      745 2023-04-24 00:19:44.535505 py_seasnake-0.2.0/README.md
+-rw-r--r--   0        0        0     1281 2023-04-24 00:21:39.084869 py_seasnake-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       85 2023-04-24 00:27:43.083762 py_seasnake-0.2.0/seasnake/__init__.py
+-rw-r--r--   0        0        0     3842 2023-04-23 23:22:06.341470 py_seasnake-0.2.0/seasnake/auth.py
+-rw-r--r--   0        0        0     3737 2023-04-23 23:24:46.487674 py_seasnake-0.2.0/seasnake/base.py
+-rw-r--r--   0        0        0     2799 2023-04-24 00:35:16.376053 py_seasnake-0.2.0/seasnake/projects.py
+-rw-r--r--   0        0        0      386 2023-04-20 15:10:20.566010 py_seasnake-0.2.0/seasnake/summaries/__init__.py
+-rw-r--r--   0        0        0     2686 2023-04-24 02:28:36.470201 py_seasnake-0.2.0/seasnake/summaries/benthic_lit.py
+-rw-r--r--   0        0        0     2800 2023-04-24 02:29:09.113535 py_seasnake-0.2.0/seasnake/summaries/benthic_photo_quadrat.py
+-rw-r--r--   0        0        0     2679 2023-04-24 02:29:37.511042 py_seasnake-0.2.0/seasnake/summaries/benthic_pit.py
+-rw-r--r--   0        0        0     3518 2023-04-24 02:30:11.893367 py_seasnake-0.2.0/seasnake/summaries/bleaching.py
+-rw-r--r--   0        0        0     2467 2023-04-24 02:30:40.146808 py_seasnake-0.2.0/seasnake/summaries/fish_belt.py
+-rw-r--r--   0        0        0     2770 2023-04-24 02:31:04.924193 py_seasnake-0.2.0/seasnake/summaries/habitat_complexity.py
+-rw-r--r--   0        0        0     2360 2023-04-24 02:31:07.718517 py_seasnake-0.2.0/seasnake/summaries/sample_event.py
+-rw-r--r--   0        0        0     1802 1970-01-01 00:00:00.000000 py_seasnake-0.2.0/PKG-INFO
```

### Comparing `py_seasnake-0.1.0/LICENSE` & `py_seasnake-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.1.0/README.md` & `py_seasnake-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 
 
 # Quick Start
 
 ```
 from seasnake import auth
 from seasnake.auth import MermaidAuth
-from seasnake.summaries import FishBelt
+from seasnake.summaries import FishBeltTransect
 
 auth = MermaidAuth()
 token = auth.request_token()
 
 project_id = "<YOUR PROJECT ID>"
-fb = FishBelt(token=token)
+fb = FishBeltTransect(token=token)
 df_obs = fb.observations(project_id)
 
 print(df_obs)
 
 ```
 
 ## Testing
```

### Comparing `py_seasnake-0.1.0/pyproject.toml` & `py_seasnake-0.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "py-seasnake"
 packages = [
     { include = "seasnake" },
 ]
-version = "0.1.0"
+version = "0.2.0"
 description = "A Python wrapper for accessing and managing MERMAID (Marine Ecological Research Management Aid) data with ease."
 authors = ["Dustin Sampson <gridcell@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://gridcell.github.io/py-seasnake/"
 repository = "https://github.com/gridcell/py-seasnake"
 documentation = "https://gridcell.github.io/py-seasnake/"
@@ -15,25 +15,30 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 pandas = "^2.0.0"
 PyJWT = "^2.6.0"
 mkdocs-material = "^9.1.6"
 mkdocstrings = {extras = ["python"], version = "^0.21.2"}
+requests = "^2.28.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2"
 black = "^23.3.0"
 isort = "^5.12.0"
 ruff = "^0.0.261"
 mypy = "^1.2.0"
 pytest-mypy = "^0.10.3"
 pandas-stubs = "^1.5.3"
 mkdocs = "^1.4.2"
 pytest-ruff = "^0.0.5"
+types-requests = "^2.28.11.17"
+
+[tool.poetry.group.examples.dependencies]
+jupyterlab = "^3.6.3"
 
 [build-system]
 requires = ["poetry-core>=1.2.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 ignore_missing_imports = true
```

### Comparing `py_seasnake-0.1.0/seasnake/base.py` & `py_seasnake-0.2.0/seasnake/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,17 @@
-import json
-import os
-import urllib.request
 from typing import Any, Dict, Generator, List, Optional, Tuple, Union
 
+import requests
 import pandas as pd
 from pandas import DataFrame
 
 PROJECT_STATUS_OPEN = 90
 PROJECT_STATUS_TEST = 80
 PROJECT_STATUS_LOCKED = 10
-
-if str(os.environ.get("ENV")).lower() == "local":
-    MERMAID_API_URL = "http://localhost:8080/v1"
-elif str(os.environ.get("ENV")).lower() == "dev":
-    MERMAID_API_URL = "https://dev-api.datamermaid.org/v1"
-else:
-    MERMAID_API_URL = "https://api.datamermaid.org/v1"
+MERMAID_API_URL = "https://api.datamermaid.org/v1"
 
 
 def requires_token(func):
     def wrapper(self, *args, **kwargs):
         if not hasattr(self, "token"):
             raise Exception("Class does not have a `self.token` attribute")
         return func(self, *args, **kwargs)
@@ -31,45 +23,58 @@
     def __init__(self, token: Optional[str] = None):
         self.token = token
 
     def fetch(
         self,
         url: str,
         payload: Optional[Dict[str, Any]] = None,
+        params: Optional[Dict[str, Any]] = None,
         headers: Optional[Dict[str, str]] = None,
         method: str = "GET",
-    ):
+    ) -> Dict[str, Any]:
         _headers = {"Content-Type": "application/json", "User-Agent": "python"}
         _headers |= headers or {}
         payload = payload or {}
 
         if not url.startswith("http"):
             url = f"{MERMAID_API_URL}{url}"
 
-        req = urllib.request.Request(
+        method = method.upper()
+        if method == "GET":
+            request_method = requests.get  # type: ignore
+        elif method == "POST":
+            request_method = requests.post  # type: ignore
+        else:
+            raise requests.RequestException(f"Unsupported method: {method}")
+
+        resp = request_method(
             url,
-            data=json.dumps(payload).encode("utf-8"),
-            method=method,
+            data=payload,
+            params=params,
             headers=_headers,
         )
-        with urllib.request.urlopen(req) as response:
-            return json.loads(response.read())
+        if resp.status_code != 200:
+            raise Exception(f"Error fetching data: {resp.text}")
+
+        return resp.json()
 
     def fetch_list(
         self,
         url: str,
         query_params: Optional[Dict[str, Any]] = None,
         payload: Optional[Dict[str, Any]] = None,
         headers: Optional[Dict[str, str]] = None,
         method: str = "GET",
     ) -> Generator[Dict[str, Any], None, None]:
         query_params = query_params or {}
-        url = f"{url}?{'&'.join(f'{k}={v}' for k, v in query_params.items())}"
         while True:
-            result = self.fetch(url, payload, headers=headers, method=method)
+            result = self.fetch(
+                url, payload, params=query_params, headers=headers, method=method
+            )
+
             yield from result.get("results") or []
             if result["next"] is None:
                 break
             url = result["next"]
 
     def data_frame_from_url(
         self,
@@ -87,23 +92,27 @@
 
         if "limit" not in query_params:
             query_params["limit"] = 1000
 
         if requires_auth and "Authorization" not in headers:
             headers["Authorization"] = f"Bearer {self.token}"
 
-        df = DataFrame(
+        data = list(
             self.fetch_list(
                 url,
                 query_params=query_params,
                 payload=payload,
                 headers=headers,
                 method=method,
             )
         )
+        if not data:
+            return DataFrame()
+
+        df = DataFrame(data)
 
         if rename_columns:
             df = df.rename(columns=rename_columns)
 
         if columns:
             df = DataFrame(df[columns])
```

### Comparing `py_seasnake-0.1.0/seasnake/projects.py` & `py_seasnake-0.2.0/seasnake/projects.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,15 +20,25 @@
         """
         Get a list of your projects.
 
         This method retrieves a list of your projects.
 
         Returns:
             DataFrame
+        
+        Examples:
+        ```
+        from seasnake import MermaidAuth, Project    
+        
+        auth = MermaidAuth()
+        project = Project(token=auth.get_token())
+        print(project.my_projects())
+        ```
         """
+
         url = "/projects/"
         return self.data_frame_from_url(url)
 
     def search_projects(
         self,
         name: Optional[str] = None,
         countries: Union[None, str, List[str]] = None,
@@ -46,14 +56,22 @@
             tags (Union[None, str, List[str]], optional): A tag or list of tags to search
             for in projects. Defaults to None.
             include_test_projects (bool, optional): Whether to include test projects in
             the search results. Defaults to False.
 
         Returns:
             DataFrame
+        
+        Examples:
+        ```
+        from seasnake import Project    
+        
+        project = Project()
+        print(project.search_projects(tags=["WCS Fiji""]))
+        ```
         """
 
         url = "/projects/"
 
         query_params = {"showall": "t"}
         if tags:
             query_params["tags"] = tags if isinstance(tags, str) else ",".join(tags)
```

### Comparing `py_seasnake-0.1.0/seasnake/summaries/benthic_lit.py` & `py_seasnake-0.2.0/seasnake/summaries/benthic_pit.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,54 +1,84 @@
 from ..base import DataFrame, MermaidBase, requires_token
 
 
-class BenthicLIT(MermaidBase):
+class BenthicPIT(MermaidBase):
     """
-    A class for handling Benthic Line Intercept Transect (LIT) data from MERMAID.
+    A class for handling Benthic Point Intercept Transect (PIT) data from MERMAID.
 
-    The BenthicLIT class is responsible for fetching Benthic LIT data, including observations,
+    The BenthicPIT class is responsible for fetching Benthic PIT data, including observations,
     observations aggregated by sample units, and observations aggregated by sample events,
     for a specified project.
     """
 
     @requires_token
     def observations(self, project_id: str) -> DataFrame:
         """
-        Retrieves a project's Benthic LIT observations.
+        Retrieves a project's Benthic PIT observations.
 
         Args:
-            project_id (str): The ID of the project for which to fetch Benthic LIT observations.
+            project_id (str): The ID of the project for which to fetch Benthic PIT observations.
 
         Returns:
             DataFrame
+        
+        Examples:
+        ```
+        from seasnake import MermaidAuth, BenthicPIT    
+        
+        auth = MermaidAuth()
+        benthic_pit = BenthicPIT(token=auth.get_token())
+        project_id = "AAAAAAAA-BBBB-CCCC-DDDD-EEEEEEEEEEEE"
+        print(benthic_pit.sample_events(project_id))
+        ```
         """
-        url = f"/projects/{project_id}/benthiclits/obstransectbenthiclits/"
+        url = f"/projects/{project_id}/benthicpits/obstransectbenthicpits/"
         return self.data_frame_from_url(url)
 
     @requires_token
     def sample_units(self, project_id: str) -> DataFrame:
         """
-        Retrieves a project's Benthic LIT observations aggregated by sample units.
+        Retrieves a project's Benthic PIT observations aggregated by sample units.
 
         Args:
-            project_id (str): The ID of the project for which to fetch Benthic LIT sample units.
+            project_id (str): The ID of the project for which to fetch Benthic PIT sample units.
 
         Returns:
             DataFrame
+        Examples:
+        ```
+        from seasnake import MermaidAuth, BenthicPIT    
+        
+        auth = MermaidAuth()
+        benthic_pit = BenthicPIT(token=auth.get_token())
+        project_id = "AAAAAAAA-BBBB-CCCC-DDDD-EEEEEEEEEEEE"
+        print(benthic_pit.sample_events(project_id))
+        ```
         """
 
-        url = f"/projects/{project_id}/benthiclits/sampleunits/"
+        url = f"/projects/{project_id}/benthicpits/sampleunits/"
         return self.data_frame_from_url(url)
 
     @requires_token
     def sample_events(self, project_id: str) -> DataFrame:
         """
-        Retrieves a project's Benthic LIT observations aggregated by sample events.
+        Retrieves a project's Benthic PIT observations aggregated by sample events.
 
         Args:
-            project_id (str): The ID of the project for which to fetch Benthic LIT sample events.
+            project_id (str): The ID of the project for which to fetch Benthic PIT sample events.
 
         Returns:
             DataFrame
+        
+        Examples:
+        ```
+        from seasnake import MermaidAuth, BenthicPIT    
+        
+        auth = MermaidAuth()
+        benthic_pit = BenthicPIT(token=auth.get_token())
+        project_id = "AAAAAAAA-BBBB-CCCC-DDDD-EEEEEEEEEEEE"
+        print(benthic_pit.sample_events(project_id))
+        ```
         """
-        url = f"/projects/{project_id}/benthiclits/sampleevents/"
+
+        url = f"/projects/{project_id}/benthicpits/sampleevents/"
         return self.data_frame_from_url(url)
```

### Comparing `py_seasnake-0.1.0/seasnake/summaries/benthic_photo_quadrat.py` & `py_seasnake-0.2.0/seasnake/summaries/benthic_photo_quadrat.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,40 +17,73 @@
 
         Args:
             project_id (str): The ID of the project for which to fetch
             Benthic Photo Quadrat observations.
 
         Returns:
             DataFrame
+        
+        Examples:
+        ```
+        from seasnake import MermaidAuth, BenthicPhotoQuadrat    
+        
+        auth = MermaidAuth()
+        bpq = BenthicPhotoQuadrat(token=auth.get_token())
+        project_id = "AAAAAAAA-BBBB-CCCC-DDDD-EEEEEEEEEEEE"
+        print(bpq.observations(project_id))
+        ```
         """
+
         url = f"/projects/{project_id}/benthicpqts/obstransectbenthicpqts/"
         return self.data_frame_from_url(url)
 
     @requires_token
     def sample_units(self, project_id: str) -> DataFrame:
         """
         Retrieves a project's Benthic Photo Quadrat observations aggregated by sample units.
 
         Args:
             project_id (str): The ID of the project for which to fetch
             Benthic Photo Quadrat sample units.
 
         Returns:
             DataFrame
+        
+        Examples:
+        ```
+        from seasnake import MermaidAuth, BenthicPhotoQuadrat    
+        
+        auth = MermaidAuth()
+        bpq = BenthicPhotoQuadrat(token=auth.get_token())
+        project_id = "AAAAAAAA-BBBB-CCCC-DDDD-EEEEEEEEEEEE"
+        print(bpq.sample_units(project_id))
+        ```
         """
+
         url = f"/projects/{project_id}/benthicpqts/sampleunits/"
         return self.data_frame_from_url(url)
 
     @requires_token
     def sample_events(self, project_id: str) -> DataFrame:
         """
         Retrieves a project's Benthic Photo Quadrat observations aggregated by sample events.
 
         Args:
             project_id (str): The ID of the project for which to fetch
             Benthic Photo Quadrat sample events.
 
         Returns:
             DataFrame
+        
+        Examples:
+        ```
+        from seasnake import MermaidAuth, BenthicPhotoQuadrat    
+        
+        auth = MermaidAuth()
+        bpq = BenthicPhotoQuadrat(token=auth.get_token())
+        project_id = "AAAAAAAA-BBBB-CCCC-DDDD-EEEEEEEEEEEE"
+        print(bpq.sample_events(project_id))
+        ```
         """
+
         url = f"/projects/{project_id}/benthicpqts/sampleevents/"
         return self.data_frame_from_url(url)
```

### Comparing `py_seasnake-0.1.0/seasnake/summaries/bleaching.py` & `py_seasnake-0.2.0/seasnake/summaries/bleaching.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,53 +16,97 @@
         Retrieves a project's Bleaching colonies bleached observations.
 
         Args:
             project_id (str): The ID of the project for which to fetch Bleaching observations.
 
         Returns:
             DataFrame
+        
+        Examples:
+        ```
+        from seasnake import MermaidAuth, Bleaching    
+        
+        auth = MermaidAuth()
+        bleaching = Bleaching(token=auth.get_token())
+        project_id = "AAAAAAAA-BBBB-CCCC-DDDD-EEEEEEEEEEEE"
+        print(bleaching.colonies_bleached_observations(project_id))
+        ```
         """
+
         url = f"/projects/{project_id}/bleachingqcs/obscoloniesbleacheds/"
         return self.data_frame_from_url(url)
 
     @requires_token
     def percent_cover_observations(self, project_id: str) -> DataFrame:
         """
         Retrieves a project's Bleaching percent cover of hard coral, macroalgae and
         soft coral observations.
 
         Args:
             project_id (str): The ID of the project for which to fetch Bleaching observations.
 
         Returns:
             DataFrame
+        
+        Examples:
+        ```
+        from seasnake import MermaidAuth, Bleaching    
+        
+        auth = MermaidAuth()
+        bleaching = Bleaching(token=auth.get_token())
+        project_id = "AAAAAAAA-BBBB-CCCC-DDDD-EEEEEEEEEEEE"
+        print(bleaching.percent_cover_observations(project_id))
+        ```
         """
+
         url = f"/projects/{project_id}/bleachingqcs/obsquadratbenthicpercents/"
         return self.data_frame_from_url(url)
 
     @requires_token
     def sample_units(self, project_id: str) -> DataFrame:
         """
         Retrieves a project's Bleaching observations aggregated by sample units.
 
         Args:
             project_id (str): The ID of the project for which to fetch Bleaching sample units.
 
         Returns:
             DataFrame
+        
+        Examples:
+        ```
+        from seasnake import MermaidAuth, Bleaching    
+        
+        auth = MermaidAuth()
+        bleaching = Bleaching(token=auth.get_token())
+        project_id = "AAAAAAAA-BBBB-CCCC-DDDD-EEEEEEEEEEEE"
+        print(bleaching.sample_units(project_id))
+        ```
         """
+
         url = f"/projects/{project_id}/bleachingqcs/sampleunits/"
         return self.data_frame_from_url(url)
 
     @requires_token
     def sample_events(self, project_id: str) -> DataFrame:
         """
         Retrieves a project's Bleaching observations aggregated by sample events.
 
         Args:
             project_id (str): The ID of the project for which to fetch Bleaching sample events.
 
         Returns:
             DataFrame
+        
+        Examples:
+        ```
+        from seasnake import MermaidAuth, Bleaching    
+        
+        auth = MermaidAuth()
+        bleaching = Bleaching(token=auth.get_token())
+        project_id = "AAAAAAAA-BBBB-CCCC-DDDD-EEEEEEEEEEEE"
+        print(bleaching.sample_events(project_id))
+        ```
         """
+
         url = f"/projects/{project_id}/bleachingqcs/sampleevents/"
         return self.data_frame_from_url(url)
```

### Comparing `py_seasnake-0.1.0/seasnake/summaries/sample_event.py` & `py_seasnake-0.2.0/seasnake/summaries/sample_event.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,22 @@
             limit_columns (bool, optional): Whether to limit the columns included
             in the DataFrame. Defaults to True.
             flatten (bool, optional): Whether to flatten the 'protocols' column in
             the DataFrame. Defaults to True.
 
         Returns:
             DataFrame
+        
+        Examples:
+        ```
+        from seasnake import SampleEvent    
+
+        sample_event = SampleEvent()
+        print(sample_event.summary())
+        ```
         """
         columns = [
             "project",
             "tags",
             "country",
             "site",
             "latitude",
```

### Comparing `py_seasnake-0.1.0/PKG-INFO` & `py_seasnake-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-seasnake
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Python wrapper for accessing and managing MERMAID (Marine Ecological Research Management Aid) data with ease.
 Home-page: https://gridcell.github.io/py-seasnake/
 License: MIT
 Keywords: MERMAID,coral,fish,API
 Author: Dustin Sampson
 Author-email: gridcell@gmail.com
 Requires-Python: >=3.8,<3.12
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyJWT (>=2.6.0,<3.0.0)
 Requires-Dist: mkdocs-material (>=9.1.6,<10.0.0)
 Requires-Dist: mkdocstrings[python] (>=0.21.2,<0.22.0)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Documentation, https://gridcell.github.io/py-seasnake/
 Project-URL: Repository, https://github.com/gridcell/py-seasnake
 Description-Content-Type: text/markdown
 
 SeaSnake
 --------
 
@@ -34,21 +35,21 @@
 
 
 # Quick Start
 
 ```
 from seasnake import auth
 from seasnake.auth import MermaidAuth
-from seasnake.summaries import FishBelt
+from seasnake.summaries import FishBeltTransect
 
 auth = MermaidAuth()
 token = auth.request_token()
 
 project_id = "<YOUR PROJECT ID>"
-fb = FishBelt(token=token)
+fb = FishBeltTransect(token=token)
 df_obs = fb.observations(project_id)
 
 print(df_obs)
 
 ```
 
 ## Testing
```


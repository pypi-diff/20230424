# Comparing `tmp/PyKagi-0.0.1.tar.gz` & `tmp/PyKagi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyKagi-0.0.1.tar", last modified: Thu Mar 30 05:04:11 2023, max compression
+gzip compressed data, was "PyKagi-0.0.2.tar", last modified: Mon Apr 24 01:28:25 2023, max compression
```

## Comparing `PyKagi-0.0.1.tar` & `PyKagi-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 05:04:11.767382 PyKagi-0.0.1/
--rw-rw-rw-   0        0        0    11558 2023-03-29 23:46:55.000000 PyKagi-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1766 2023-03-30 05:04:11.767382 PyKagi-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-30 05:04:11.748433 PyKagi-0.0.1/PyKagi/
--rw-rw-rw-   0        0        0      262 2023-03-30 01:22:53.000000 PyKagi-0.0.1/PyKagi/__init__.py
--rw-rw-rw-   0        0        0     2558 2023-03-30 01:22:25.000000 PyKagi-0.0.1/PyKagi/api.py
-drwxrwxrwx   0        0        0        0 2023-03-30 05:04:11.766385 PyKagi-0.0.1/PyKagi/config/
--rw-rw-rw-   0        0        0        0 2022-10-13 08:58:13.000000 PyKagi-0.0.1/PyKagi/config/__init__.py
--rw-rw-rw-   0        0        0      172 2023-03-29 23:49:12.000000 PyKagi-0.0.1/PyKagi/config/info.py
-drwxrwxrwx   0        0        0        0 2023-03-30 05:04:11.764390 PyKagi-0.0.1/PyKagi.egg-info/
--rw-rw-rw-   0        0        0     1766 2023-03-30 05:04:11.000000 PyKagi-0.0.1/PyKagi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2023-03-30 05:04:11.000000 PyKagi-0.0.1/PyKagi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 05:04:11.000000 PyKagi-0.0.1/PyKagi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-03-30 05:04:11.000000 PyKagi-0.0.1/PyKagi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-30 05:04:11.000000 PyKagi-0.0.1/PyKagi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1315 2023-03-30 05:03:15.000000 PyKagi-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-03-30 05:04:11.767382 PyKagi-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      891 2023-03-30 01:33:40.000000 PyKagi-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:28:25.258896 PyKagi-0.0.2/
+-rw-rw-rw-   0        0        0    11558 2023-03-29 23:46:55.000000 PyKagi-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3194 2023-04-24 01:28:25.257900 PyKagi-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-24 01:28:25.239947 PyKagi-0.0.2/PyKagi/
+-rw-rw-rw-   0        0        0      262 2023-03-30 01:22:53.000000 PyKagi-0.0.2/PyKagi/__init__.py
+-rw-rw-rw-   0        0        0     2400 2023-04-24 01:04:11.000000 PyKagi-0.0.2/PyKagi/api.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:28:25.256901 PyKagi-0.0.2/PyKagi/config/
+-rw-rw-rw-   0        0        0        0 2022-10-13 08:58:13.000000 PyKagi-0.0.2/PyKagi/config/__init__.py
+-rw-rw-rw-   0        0        0      172 2023-04-24 01:13:34.000000 PyKagi-0.0.2/PyKagi/config/info.py
+drwxrwxrwx   0        0        0        0 2023-04-24 01:28:25.254907 PyKagi-0.0.2/PyKagi.egg-info/
+-rw-rw-rw-   0        0        0     3194 2023-04-24 01:28:25.000000 PyKagi-0.0.2/PyKagi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2023-04-24 01:28:25.000000 PyKagi-0.0.2/PyKagi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 01:28:25.000000 PyKagi-0.0.2/PyKagi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-04-24 01:28:25.000000 PyKagi-0.0.2/PyKagi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-24 01:28:25.000000 PyKagi-0.0.2/PyKagi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2731 2023-04-24 01:22:21.000000 PyKagi-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-24 01:28:25.258896 PyKagi-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      903 2023-04-24 01:28:03.000000 PyKagi-0.0.2/setup.py
```

### Comparing `PyKagi-0.0.1/LICENSE` & `PyKagi-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyKagi-0.0.1/PyKagi/api.py` & `PyKagi-0.0.2/PyKagi/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,48 +3,45 @@
 
 class UniversalSummarizer:
 
     def __init__(self, api_token=None):
         self.api_token = api_token
         self.base_url = "https://kagi.com/api/v0/summarize"
 
-    def summarize(self, method="GET", url=None, text=None, engine="agnes", summary_type="summary", target_language=None, cache=True):
+    def summarize(self, url=None, text=None, engine="agnes", summary_type="summary", target_language=None, cache=True):
         if url is None and text is None:
             raise ValueError("Either 'url' or 'text' must be provided.")
         if url is not None and text is not None:
             raise ValueError(
                 "'url' and 'text' are exclusive. Provide only one of them.")
-        if method not in ["GET", "POST"]:
-            raise ValueError("Invalid method. Choose either 'GET' or 'POST'.")
 
         headers = {
             "Authorization": f"Bot {self.api_token}"
         }
 
-        if method == "GET":
+        if text is None:
             headers["Content-Type"] = "application/json"
             params = {
                 "url": url,
-                "text": text,
                 "engine": engine,
                 "summary_type": summary_type,
                 "target_language": target_language,
-                "cache": cache
+                "cache": str(cache).lower()
             }
             response = requests.get(
                 self.base_url, headers=headers, params=params)
-        elif method == "POST":
+            print(response.url)
+        else:
             headers["Content-Type"] = "application/json"
             data = {
-                "url": url,
                 "text": text,
                 "engine": engine,
                 "summary_type": summary_type,
                 "target_language": target_language,
-                "cache": cache
+                "cache": str(cache).lower()
             }
             response = requests.post(self.base_url, headers=headers, json=data)
 
         if response.status_code == 200:
             return response.json()
         else:
             raise Exception(
```

### Comparing `PyKagi-0.0.1/setup.py` & `PyKagi-0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,12 +17,12 @@
     description="Kagi API Python Wrapper",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=__github__,
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
+        'License :: OSI Approved :: Apache Software License',
         "Operating System :: OS Independent"
     ],
     install_requires=install_requires,
 )
```


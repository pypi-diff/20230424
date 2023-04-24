# Comparing `tmp/aiotubes-3.1.tar.gz` & `tmp/aiotubes-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotubes-3.1.tar", last modified: Sun Apr 23 17:45:02 2023, max compression
+gzip compressed data, was "aiotubes-3.2.tar", last modified: Mon Apr 24 06:32:40 2023, max compression
```

## Comparing `aiotubes-3.1.tar` & `aiotubes-3.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 17:45:02.854676 aiotubes-3.1/
--rw-rw-rw-   0        0        0     1084 2022-10-11 08:30:57.000000 aiotubes-3.1/LICENSE
--rw-rw-rw-   0        0        0      697 2023-04-23 17:45:02.853677 aiotubes-3.1/PKG-INFO
--rw-rw-rw-   0        0        0      361 2023-04-23 14:57:43.000000 aiotubes-3.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-23 17:45:02.827747 aiotubes-3.1/aiotube/
--rw-rw-rw-   0        0        0       58 2023-04-23 14:53:51.000000 aiotubes-3.1/aiotube/__init__.py
--rw-rw-rw-   0        0        0     1766 2023-04-23 17:42:57.000000 aiotubes-3.1/aiotube/client.py
--rw-rw-rw-   0        0        0      994 2023-04-23 12:02:05.000000 aiotubes-3.1/aiotube/constants.py
--rw-rw-rw-   0        0        0     2511 2023-04-23 14:53:45.000000 aiotubes-3.1/aiotube/exceptions.py
--rw-rw-rw-   0        0        0     5405 2023-04-23 14:53:51.000000 aiotubes-3.1/aiotube/extractors.py
--rw-rw-rw-   0        0        0     1487 2023-02-24 20:59:01.000000 aiotubes-3.1/aiotube/helpers.py
--rw-rw-rw-   0        0        0     4427 2023-02-24 13:57:51.000000 aiotubes-3.1/aiotube/itags.py
--rw-rw-rw-   0        0        0     2226 2023-04-23 14:53:51.000000 aiotubes-3.1/aiotube/playlist.py
--rw-rw-rw-   0        0        0     8051 2023-04-23 17:42:43.000000 aiotubes-3.1/aiotube/streams.py
--rw-rw-rw-   0        0        0     5029 2023-04-23 14:53:51.000000 aiotubes-3.1/aiotube/video.py
-drwxrwxrwx   0        0        0        0 2023-04-23 17:45:02.852681 aiotubes-3.1/aiotubes.egg-info/
--rw-rw-rw-   0        0        0      697 2023-04-23 17:45:02.000000 aiotubes-3.1/aiotubes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-04-23 17:45:02.000000 aiotubes-3.1/aiotubes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 17:45:02.000000 aiotubes-3.1/aiotubes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-23 17:45:02.000000 aiotubes-3.1/aiotubes.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-23 17:45:02.000000 aiotubes-3.1/aiotubes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 17:45:02.854676 aiotubes-3.1/setup.cfg
--rw-rw-rw-   0        0        0      666 2023-04-23 17:44:53.000000 aiotubes-3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:32:40.031362 aiotubes-3.2/
+-rw-rw-rw-   0        0        0     1084 2022-10-11 08:30:57.000000 aiotubes-3.2/LICENSE
+-rw-rw-rw-   0        0        0      697 2023-04-24 06:32:40.030363 aiotubes-3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2023-04-23 14:57:43.000000 aiotubes-3.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-24 06:32:40.006302 aiotubes-3.2/aiotube/
+-rw-rw-rw-   0        0        0       58 2023-04-23 14:53:51.000000 aiotubes-3.2/aiotube/__init__.py
+-rw-rw-rw-   0        0        0     1766 2023-04-23 17:42:57.000000 aiotubes-3.2/aiotube/client.py
+-rw-rw-rw-   0        0        0      994 2023-04-23 12:02:05.000000 aiotubes-3.2/aiotube/constants.py
+-rw-rw-rw-   0        0        0     2511 2023-04-23 14:53:45.000000 aiotubes-3.2/aiotube/exceptions.py
+-rw-rw-rw-   0        0        0     5405 2023-04-23 14:53:51.000000 aiotubes-3.2/aiotube/extractors.py
+-rw-rw-rw-   0        0        0     2015 2023-04-24 06:32:12.000000 aiotubes-3.2/aiotube/helpers.py
+-rw-rw-rw-   0        0        0     4427 2023-02-24 13:57:51.000000 aiotubes-3.2/aiotube/itags.py
+-rw-rw-rw-   0        0        0     2226 2023-04-23 14:53:51.000000 aiotubes-3.2/aiotube/playlist.py
+-rw-rw-rw-   0        0        0     8051 2023-04-23 17:42:43.000000 aiotubes-3.2/aiotube/streams.py
+-rw-rw-rw-   0        0        0     5107 2023-04-24 06:32:12.000000 aiotubes-3.2/aiotube/video.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:32:40.030363 aiotubes-3.2/aiotubes.egg-info/
+-rw-rw-rw-   0        0        0      697 2023-04-24 06:32:39.000000 aiotubes-3.2/aiotubes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-04-24 06:32:39.000000 aiotubes-3.2/aiotubes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 06:32:39.000000 aiotubes-3.2/aiotubes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-24 06:32:39.000000 aiotubes-3.2/aiotubes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-24 06:32:39.000000 aiotubes-3.2/aiotubes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 06:32:40.031362 aiotubes-3.2/setup.cfg
+-rw-rw-rw-   0        0        0      666 2023-04-24 06:32:22.000000 aiotubes-3.2/setup.py
```

### Comparing `aiotubes-3.1/LICENSE` & `aiotubes-3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotubes-3.1/PKG-INFO` & `aiotubes-3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotubes
-Version: 3.1
+Version: 3.2
 Summary: Asynchronous Youtube API
 Home-page: https://github.com/sheldygg/aiotube
 Author: sheldy
 License: MIT
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

### Comparing `aiotubes-3.1/aiotube/client.py` & `aiotubes-3.2/aiotube/client.py`

 * *Files identical despite different names*

### Comparing `aiotubes-3.1/aiotube/constants.py` & `aiotubes-3.2/aiotube/constants.py`

 * *Files identical despite different names*

### Comparing `aiotubes-3.1/aiotube/exceptions.py` & `aiotubes-3.2/aiotube/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiotubes-3.1/aiotube/extractors.py` & `aiotubes-3.2/aiotube/extractors.py`

 * *Files identical despite different names*

### Comparing `aiotubes-3.1/aiotube/helpers.py` & `aiotubes-3.2/aiotube/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import re
-from typing import Optional
+import asyncio
 
 
-def target_directory(output_path: Optional[str] = None) -> str:
+def target_directory(output_path: str | None = None) -> str:
     if output_path:
         if not os.path.isabs(output_path):
             output_path = os.path.join(os.getcwd(), output_path)
     else:
         output_path = os.getcwd()
     os.makedirs(output_path, exist_ok=True)
     return output_path
@@ -51,7 +51,23 @@
         r"\~",
         r"\\\\",
     ]
     pattern = "|".join(ntfs_characters + characters)
     regex = re.compile(pattern, re.UNICODE)
     filename = regex.sub("", s)
     return filename[:max_length].rsplit(" ", 0)[0]
+
+
+def retry_if_none(max_retries: int):
+    def decorator(func):
+        async def wrapper(*args, **kwargs):
+            retries = 0
+            while True:
+                result = await func(*args, **kwargs)
+                if result is not None:
+                    return result
+                retries += 1
+                if retries > max_retries:
+                    raise ValueError(f"{func.__name__} failed after {max_retries} retries")
+                await asyncio.sleep(1)
+        return wrapper
+    return decorator
```

### Comparing `aiotubes-3.1/aiotube/itags.py` & `aiotubes-3.2/aiotube/itags.py`

 * *Files identical despite different names*

### Comparing `aiotubes-3.1/aiotube/playlist.py` & `aiotubes-3.2/aiotube/playlist.py`

 * *Files identical despite different names*

### Comparing `aiotubes-3.1/aiotube/streams.py` & `aiotubes-3.2/aiotube/streams.py`

 * *Files identical despite different names*

### Comparing `aiotubes-3.1/aiotube/video.py` & `aiotubes-3.2/aiotube/video.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from aiotube.client import HttpMethod, RequestClient
 from aiotube.exceptions import (LiveStreamError, MembersOnly,
                                 RecordingUnavailable, VideoPrivate,
                                 VideoUnavailable)
 from aiotube.extractors import (apply_descrambler, extract_video_id,
                                 playability_status)
 from aiotube.streams import Stream, StreamQuery
+from aiotube.helpers import retry_if_none
 
 
 class Video:
     def __init__(self, url: str):
         self.video_id = extract_video_id(url)
         self.base_url = "https://www.youtube.com/youtubei/v1"
         self.watch_url = f"https://youtube.com/watch?v={self.video_id}"
@@ -39,14 +40,15 @@
                 params=query,
                 headers=headers,
                 data=self.client.base_data,
             )
             self._video_info = response.get("response")
         return self._video_info
 
+    @retry_if_none(max_retries=5)
     async def streaming_data(self):
         await self.check_availability()
         data = await self.video_info()
         if "streamingData" in data:
             return data["streamingData"]
         await self.bypass_age_gate()
         return self._video_info
```

### Comparing `aiotubes-3.1/aiotubes.egg-info/PKG-INFO` & `aiotubes-3.2/aiotubes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotubes
-Version: 3.1
+Version: 3.2
 Summary: Asynchronous Youtube API
 Home-page: https://github.com/sheldygg/aiotube
 Author: sheldy
 License: MIT
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

### Comparing `aiotubes-3.1/setup.py` & `aiotubes-3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def get_description():
     with open('README.rst', 'r', encoding='utf-8') as f:
         return f.read()
 
 
 setuptools.setup(
     name="aiotubes",
-    version="3.1",
+    version="3.2",
     license='MIT',
     author="sheldy",
     description="Asynchronous Youtube API",
     url="https://github.com/sheldygg/aiotube",
     packages=setuptools.find_packages(),
     long_description_content_type='text/markdown',
     long_description=get_description(),
```


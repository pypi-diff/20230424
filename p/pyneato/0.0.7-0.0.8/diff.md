# Comparing `tmp/pyneato-0.0.7.tar.gz` & `tmp/pyneato-0.0.8.tar.gz`

## Comparing `pyneato-0.0.7.tar` & `pyneato-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 pyneato-0.0.7/setup.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pyneato-0.0.7/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 pyneato-0.0.7/pyneato/__init__.py
--rw-r--r--   0        0        0     5087 2020-02-02 00:00:00.000000 pyneato-0.0.7/pyneato/account.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 pyneato-0.0.7/pyneato/enum.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 pyneato-0.0.7/pyneato/exception.py
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 pyneato-0.0.7/pyneato/floorplan.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 pyneato-0.0.7/pyneato/neato.py
--rw-r--r--   0        0        0     8963 2020-02-02 00:00:00.000000 pyneato-0.0.7/pyneato/robot.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 pyneato-0.0.7/pyneato/robot_state.py
--rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 pyneato-0.0.7/pyneato/session.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 pyneato-0.0.7/pyneato/version.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 pyneato-0.0.7/sample/sample.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pyneato-0.0.7/LICENSE
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 pyneato-0.0.7/README.md
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 pyneato-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 pyneato-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 pyneato-0.0.8/setup.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pyneato-0.0.8/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 pyneato-0.0.8/pyneato/__init__.py
+-rw-r--r--   0        0        0     5219 2020-02-02 00:00:00.000000 pyneato-0.0.8/pyneato/account.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 pyneato-0.0.8/pyneato/enum.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 pyneato-0.0.8/pyneato/exception.py
+-rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 pyneato-0.0.8/pyneato/floorplan.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 pyneato-0.0.8/pyneato/neato.py
+-rw-r--r--   0        0        0     8963 2020-02-02 00:00:00.000000 pyneato-0.0.8/pyneato/robot.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 pyneato-0.0.8/pyneato/robot_state.py
+-rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 pyneato-0.0.8/pyneato/session.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 pyneato-0.0.8/pyneato/version.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 pyneato-0.0.8/sample/sample.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pyneato-0.0.8/LICENSE
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 pyneato-0.0.8/README.md
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 pyneato-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 pyneato-0.0.8/PKG-INFO
```

### Comparing `pyneato-0.0.7/setup.py` & `pyneato-0.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pyneato",
-    version="0.0.7",
+    version="0.0.8",
     description="Python package for controlling Neato pyneato Connected vacuum robot",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Benjamin Paap",
     author_email="benjamin.paap@gmail.com",
     url="https://github.com/benjaminpaap/pyneato",
     license="Licensed under the MIT license. See LICENSE file for details",
```

### Comparing `pyneato-0.0.7/.github/workflows/python-publish.yml` & `pyneato-0.0.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pyneato-0.0.7/pyneato/__init__.py` & `pyneato-0.0.8/pyneato/__init__.py`

 * *Files identical despite different names*

### Comparing `pyneato-0.0.7/pyneato/account.py` & `pyneato-0.0.8/pyneato/account.py`

 * *Files 4% similar despite different names*

```diff
@@ -170,14 +170,16 @@
         for floorplan in resp.json():
             FLOORPLAN_SCHEMA(floorplan)
             floorplan_object = Floorplan(
                 session = self._session,
                 uuid = floorplan["floorplan_uuid"],
                 name = floorplan["name"],
                 rank_uuid = floorplan["rank_uuid"],
+                rank_binary = floorplan["processed_rank_binary"],
+                last_modified_at = floorplan["last_modified_at"],
             )
             self._floorplans.append(floorplan_object)
 
     def get_userdata(self):
         resp = self._session.get("/users/me")
 
         json = resp.json()
```

### Comparing `pyneato-0.0.7/pyneato/enum.py` & `pyneato-0.0.8/pyneato/enum.py`

 * *Files identical despite different names*

### Comparing `pyneato-0.0.7/pyneato/exception.py` & `pyneato-0.0.8/pyneato/exception.py`

 * *Files identical despite different names*

### Comparing `pyneato-0.0.7/pyneato/floorplan.py` & `pyneato-0.0.8/pyneato/floorplan.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import base64
 import logging
 
 from .session import Session
 from .enum import TrackTypeEnum, CleaningModeEnum
 
 from voluptuous import (
     ALLOW_EXTRA,
@@ -33,20 +34,39 @@
         },
         extra=ALLOW_EXTRA,
     ),
     extra=ALLOW_EXTRA,
 )
 
 class Floorplan:
-    def __init__(self, session: Session, uuid: str, name: str | None, rank_uuid: str):
+    def __init__(
+        self,
+        session: Session,
+        uuid: str,
+        name: str | None,
+        rank_uuid: str,
+        rank_binary: str,
+        last_modified_at: str,
+    ):
         self._session = session
         self.name = name
         self.uuid = uuid
         self.rank_uuid = rank_uuid
         self._tracks = set()
+        self.last_modified_at = last_modified_at
+        self._rank_binary = rank_binary
+
+    @property
+    def rank_image(self) -> str:
+        """
+        Get the binary image of the floorplan
+
+        :return: The image of the floorplan
+        """
+        return base64.b64decode(self._rank_binary)
 
     @property
     def tracks(self):
         """
         Return set of tracks for this floorplan
 
         :return:
```

### Comparing `pyneato-0.0.7/pyneato/neato.py` & `pyneato-0.0.8/pyneato/neato.py`

 * *Files identical despite different names*

### Comparing `pyneato-0.0.7/pyneato/robot.py` & `pyneato-0.0.8/pyneato/robot.py`

 * *Files identical despite different names*

### Comparing `pyneato-0.0.7/pyneato/robot_state.py` & `pyneato-0.0.8/pyneato/robot_state.py`

 * *Files identical despite different names*

### Comparing `pyneato-0.0.7/pyneato/session.py` & `pyneato-0.0.8/pyneato/session.py`

 * *Files identical despite different names*

### Comparing `pyneato-0.0.7/sample/sample.py` & `pyneato-0.0.8/sample/sample.py`

 * *Files identical despite different names*

### Comparing `pyneato-0.0.7/LICENSE` & `pyneato-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyneato-0.0.7/README.md` & `pyneato-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pyneato-0.0.7/PKG-INFO` & `pyneato-0.0.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneato
-Version: 0.0.7
+Version: 0.0.8
 Summary: Package to control a neato vacuum robot
 Author-email: Benjamin Paap <benjamin.paap@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```


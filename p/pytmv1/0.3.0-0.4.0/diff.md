# Comparing `tmp/pytmv1-0.3.0.tar.gz` & `tmp/pytmv1-0.4.0.tar.gz`

## Comparing `pytmv1-0.3.0.tar` & `pytmv1-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 pytmv1-0.3.0/.coveragerc
--rwxr-xr-x   0        0        0      142 2020-02-02 00:00:00.000000 pytmv1-0.3.0/tox.ini
--rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 pytmv1-0.3.0/src/pytmv1/__about__.py
--rwxr-xr-x   0        0        0     3504 2020-02-02 00:00:00.000000 pytmv1-0.3.0/src/pytmv1/__init__.py
--rwxr-xr-x   0        0        0    26132 2020-02-02 00:00:00.000000 pytmv1-0.3.0/src/pytmv1/caller.py
--rwxr-xr-x   0        0        0    10922 2020-02-02 00:00:00.000000 pytmv1-0.3.0/src/pytmv1/core.py
--rwxr-xr-x   0        0        0     1479 2020-02-02 00:00:00.000000 pytmv1-0.3.0/src/pytmv1/exceptions.py
--rwxr-xr-x   0        0        0      662 2020-02-02 00:00:00.000000 pytmv1-0.3.0/src/pytmv1/logger.py
--rwxr-xr-x   0        0        0     3967 2020-02-02 00:00:00.000000 pytmv1-0.3.0/src/pytmv1/mapper.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pytmv1-0.3.0/src/pytmv1/py.typed
--rwxr-xr-x   0        0        0     3916 2020-02-02 00:00:00.000000 pytmv1-0.3.0/src/pytmv1/results.py
--rwxr-xr-x   0        0        0     3183 2020-02-02 00:00:00.000000 pytmv1-0.3.0/src/pytmv1/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytmv1-0.3.0/src/pytmv1/model/__init__.py
--rw-r--r--   0        0        0     5737 2020-02-02 00:00:00.000000 pytmv1-0.3.0/src/pytmv1/model/commons.py
--rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 pytmv1-0.3.0/src/pytmv1/model/enums.py
--rwxr-xr-x   0        0        0     1816 2020-02-02 00:00:00.000000 pytmv1-0.3.0/src/pytmv1/model/requests.py
--rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 pytmv1-0.3.0/src/pytmv1/model/responses.py
--rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 pytmv1-0.3.0/.gitignore
--rwxr-xr-x   0        0        0    11540 2020-02-02 00:00:00.000000 pytmv1-0.3.0/LICENSE.txt
--rwxr-xr-x   0        0        0    14766 2020-02-02 00:00:00.000000 pytmv1-0.3.0/README.md
--rwxr-xr-x   0        0        0     1932 2020-02-02 00:00:00.000000 pytmv1-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    16031 2020-02-02 00:00:00.000000 pytmv1-0.3.0/PKG-INFO
+-rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 pytmv1-0.4.0/.coveragerc
+-rwxr-xr-x   0        0        0      142 2020-02-02 00:00:00.000000 pytmv1-0.4.0/tox.ini
+-rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 pytmv1-0.4.0/src/pytmv1/__about__.py
+-rwxr-xr-x   0        0        0     3504 2020-02-02 00:00:00.000000 pytmv1-0.4.0/src/pytmv1/__init__.py
+-rwxr-xr-x   0        0        0    26132 2020-02-02 00:00:00.000000 pytmv1-0.4.0/src/pytmv1/caller.py
+-rwxr-xr-x   0        0        0    10922 2020-02-02 00:00:00.000000 pytmv1-0.4.0/src/pytmv1/core.py
+-rwxr-xr-x   0        0        0     1479 2020-02-02 00:00:00.000000 pytmv1-0.4.0/src/pytmv1/exceptions.py
+-rwxr-xr-x   0        0        0      662 2020-02-02 00:00:00.000000 pytmv1-0.4.0/src/pytmv1/logger.py
+-rwxr-xr-x   0        0        0     3967 2020-02-02 00:00:00.000000 pytmv1-0.4.0/src/pytmv1/mapper.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pytmv1-0.4.0/src/pytmv1/py.typed
+-rwxr-xr-x   0        0        0     3916 2020-02-02 00:00:00.000000 pytmv1-0.4.0/src/pytmv1/results.py
+-rwxr-xr-x   0        0        0     3183 2020-02-02 00:00:00.000000 pytmv1-0.4.0/src/pytmv1/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytmv1-0.4.0/src/pytmv1/model/__init__.py
+-rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 pytmv1-0.4.0/src/pytmv1/model/commons.py
+-rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 pytmv1-0.4.0/src/pytmv1/model/enums.py
+-rwxr-xr-x   0        0        0     1816 2020-02-02 00:00:00.000000 pytmv1-0.4.0/src/pytmv1/model/requests.py
+-rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 pytmv1-0.4.0/src/pytmv1/model/responses.py
+-rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 pytmv1-0.4.0/.gitignore
+-rwxr-xr-x   0        0        0    11540 2020-02-02 00:00:00.000000 pytmv1-0.4.0/LICENSE.txt
+-rwxr-xr-x   0        0        0    14766 2020-02-02 00:00:00.000000 pytmv1-0.4.0/README.md
+-rwxr-xr-x   0        0        0     1932 2020-02-02 00:00:00.000000 pytmv1-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    16031 2020-02-02 00:00:00.000000 pytmv1-0.4.0/PKG-INFO
```

### Comparing `pytmv1-0.3.0/src/pytmv1/__init__.py` & `pytmv1-0.4.0/src/pytmv1/__init__.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.3.0/src/pytmv1/caller.py` & `pytmv1-0.4.0/src/pytmv1/caller.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.3.0/src/pytmv1/core.py` & `pytmv1-0.4.0/src/pytmv1/core.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.3.0/src/pytmv1/exceptions.py` & `pytmv1-0.4.0/src/pytmv1/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.3.0/src/pytmv1/logger.py` & `pytmv1-0.4.0/src/pytmv1/logger.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.3.0/src/pytmv1/mapper.py` & `pytmv1-0.4.0/src/pytmv1/mapper.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.3.0/src/pytmv1/results.py` & `pytmv1-0.4.0/src/pytmv1/results.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.3.0/src/pytmv1/utils.py` & `pytmv1-0.4.0/src/pytmv1/utils.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.3.0/src/pytmv1/model/commons.py` & `pytmv1-0.4.0/src/pytmv1/model/commons.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.utils import to_lower_camel
 
 from .enums import (
     EntityType,
     Iam,
@@ -242,15 +242,28 @@
 
 
 class SandboxSuspiciousObject(BaseModel):
     risk_level: RiskLevel
     analysis_completion_date_time: str
     expired_date_time: str
     root_sha1: str
-    ip: str
+    type: ObjectType
+    value: str
+
+    def __init__(self, **data: str) -> None:
+        obj: Tuple[str, str] = self._map(data)
+        super().__init__(type=obj[0], value=obj[1], **data)
+
+    @staticmethod
+    def _map(args: Dict[str, str]) -> Tuple[str, str]:
+        return {
+            (k, v)
+            for k, v in args.items()
+            if k in map(lambda ot: ot.value, ObjectType)
+        }.pop()
 
 
 class SuspiciousObject(ExceptionObject):
     scan_action: ScanAction
     risk_level: RiskLevel
     in_exception_list: bool
     expired_date_time: str
```

### Comparing `pytmv1-0.3.0/src/pytmv1/model/enums.py` & `pytmv1-0.4.0/src/pytmv1/model/enums.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.3.0/src/pytmv1/model/requests.py` & `pytmv1-0.4.0/src/pytmv1/model/requests.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.3.0/src/pytmv1/model/responses.py` & `pytmv1-0.4.0/src/pytmv1/model/responses.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.3.0/LICENSE.txt` & `pytmv1-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytmv1-0.3.0/README.md` & `pytmv1-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pytmv1-0.3.0/pyproject.toml` & `pytmv1-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytmv1-0.3.0/PKG-INFO` & `pytmv1-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytmv1
-Version: 0.3.0
+Version: 0.4.0
 Summary: Python library for Trend Micro Vision One
 Project-URL: Source, https://github.com/TrendATI/pytmv1
 Project-URL: Issues, https://github.com/TrendATI/pytmv1/issues
 Author-email: Thomas Legros <thomas_legros@trendmicro.com>
 Maintainer-email: TrendATI <ati-integration@trendmicro.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
```


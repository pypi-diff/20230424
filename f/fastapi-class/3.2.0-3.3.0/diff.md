# Comparing `tmp/fastapi_class-3.2.0.tar.gz` & `tmp/fastapi_class-3.3.0.tar.gz`

## Comparing `fastapi_class-3.2.0.tar` & `fastapi_class-3.3.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/codecov.yml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/.github/dependabot.yml
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/.github/workflows/lint.yaml
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/fastapi_class/__init__.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/fastapi_class/logger.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/fastapi_class/openapi.py
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/fastapi_class/routers.py
--rw-r--r--   0        0        0     3554 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/fastapi_class/views.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/fastapi_class/exception/__init__.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/fastapi_class/exception/handler.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/scripts/clean.sh
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/scripts/format.sh
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/scripts/lint.sh
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/scripts/test.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/tests/__init__.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/tests/factory.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/tests/test_exceptions.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/tests/test_logger.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/tests/test_metadata.py
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/tests/test_openapi.py
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/tests/test_routers.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/tests/test_version.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/tests/test_views.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/LICENSE
--rw-r--r--   0        0        0     5189 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/README.md
--rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/pyproject.toml
--rw-r--r--   0        0        0     6648 2020-02-02 00:00:00.000000 fastapi_class-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 fastapi_class-3.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 fastapi_class-3.3.0/codecov.yml
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 fastapi_class-3.3.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 fastapi_class-3.3.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 fastapi_class-3.3.0/.github/workflows/lint.yaml
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 fastapi_class-3.3.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 fastapi_class-3.3.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 fastapi_class-3.3.0/fastapi_class/__init__.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 fastapi_class-3.3.0/fastapi_class/logger.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 fastapi_class-3.3.0/fastapi_class/openapi.py
+-rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 fastapi_class-3.3.0/fastapi_class/routers.py
+-rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 fastapi_class-3.3.0/fastapi_class/views.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 fastapi_class-3.3.0/fastapi_class/exception/__init__.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 fastapi_class-3.3.0/fastapi_class/exception/handler.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 fastapi_class-3.3.0/scripts/clean.sh
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 fastapi_class-3.3.0/scripts/format.sh
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 fastapi_class-3.3.0/scripts/lint.sh
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fastapi_class-3.3.0/scripts/test.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_class-3.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 fastapi_class-3.3.0/tests/factory.py
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 fastapi_class-3.3.0/tests/test_exceptions.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 fastapi_class-3.3.0/tests/test_logger.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 fastapi_class-3.3.0/tests/test_metadata.py
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 fastapi_class-3.3.0/tests/test_openapi.py
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 fastapi_class-3.3.0/tests/test_routers.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 fastapi_class-3.3.0/tests/test_version.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 fastapi_class-3.3.0/tests/test_views.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 fastapi_class-3.3.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fastapi_class-3.3.0/LICENSE
+-rw-r--r--   0        0        0     5189 2020-02-02 00:00:00.000000 fastapi_class-3.3.0/README.md
+-rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 fastapi_class-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6747 2020-02-02 00:00:00.000000 fastapi_class-3.3.0/PKG-INFO
```

### Comparing `fastapi_class-3.2.0/.pre-commit-config.yaml` & `fastapi_class-3.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fastapi_class-3.2.0/.github/workflows/lint.yaml` & `fastapi_class-3.3.0/.github/workflows/lint.yaml`

 * *Files identical despite different names*

### Comparing `fastapi_class-3.2.0/.github/workflows/publish.yml` & `fastapi_class-3.3.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fastapi_class-3.2.0/.github/workflows/test.yml` & `fastapi_class-3.3.0/.github/workflows/test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 jobs:
   tests:
     runs-on: ubuntu-latest
     timeout-minutes: 30
     strategy:
       matrix:
-        python-version: ["3.10", "3.11"]
+        python-version: ["3.8", "3.9", "3.10", "3.11"]
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `fastapi_class-3.2.0/fastapi_class/__init__.py` & `fastapi_class-3.3.0/fastapi_class/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     def post(self, user: ItemModel):
         pass
 ```
 
 """
 
 
-__version__ = "3.2.0"
+__version__ = "3.3.0"
 
 from fastapi_class.exception import FormattedMessageException
 from fastapi_class.openapi import ExceptionModel, _exceptions_to_responses
 from fastapi_class.routers import Metadata, Method, endpoint
 from fastapi_class.views import View
 
 __all__ = [
```

### Comparing `fastapi_class-3.2.0/fastapi_class/openapi.py` & `fastapi_class-3.3.0/fastapi_class/openapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import logging
 from collections.abc import Callable, Iterable
 
 from fastapi import HTTPException, status
 from pydantic import BaseModel, Field
 
 logger = logging.getLogger("fastapi_class")
@@ -36,15 +38,16 @@
     mapping = {}
 
     for exception in exceptions:
         try:
             exc = exception if isinstance(exception, HTTPException) else exception()
         except TypeError:
             logger.warning(
-                "Exception %s was failed to be parsed. Make sure it's either an HTTPException instance or it's a factory function with arguments having default values."
+                "Exception %s was failed to be parsed. Make sure it's either an HTTPException instance or it's a "
+                "factory function with arguments having default values."
             )
             exc = HTTPException(status.HTTP_400_BAD_REQUEST, detail=str(exception))
         if exc.status_code not in mapping:
             mapping[exc.status_code] = {
                 "description": exc.detail,
                 "model": ExceptionModel,
             }
```

### Comparing `fastapi_class-3.2.0/fastapi_class/routers.py` & `fastapi_class-3.3.0/fastapi_class/routers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from collections.abc import Callable, Iterable
 from dataclasses import dataclass
 from enum import Enum
 from functools import wraps
 from typing import Any, ClassVar
 
 from fastapi.responses import Response
@@ -14,25 +16,25 @@
     PATCH = "patch"
     DELETE = "delete"
     PUT = "put"
 
 
 @dataclass(frozen=True, init=True, repr=True)
 class Metadata:
-    methods: Iterable[Method]
+    methods: Iterable[str | Method]
     name: str | None = None
     path: str | None = None
     status_code: int | None = None
     response_model: type[BaseModel] | None = None
     response_class: type[Response] | None = None
     __default_method_suffix: ClassVar[str] = "_or_default"
 
     def __getattr__(self, __name: str) -> Any | Callable[[Any], Any]:
         if __name.endswith(Metadata.__default_method_suffix):
-            prefix = __name.removesuffix(Metadata.__default_method_suffix)
+            prefix = __name.replace(Metadata.__default_method_suffix, "")
             if hasattr(self, prefix):
                 return lambda _default: getattr(self, prefix, None) or _default
             return getattr(self, prefix)
         raise AttributeError(f"{self.__class__.__name__} has no attribute {__name}")
 
 
 def endpoint(
```

### Comparing `fastapi_class-3.2.0/fastapi_class/views.py` & `fastapi_class-3.3.0/fastapi_class/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,18 @@
+from __future__ import annotations
+
 import re
 from collections.abc import Callable, Iterable
 
 from fastapi import APIRouter, FastAPI, HTTPException, status
 from fastapi.responses import JSONResponse
 
 from fastapi_class.openapi import _exceptions_to_responses
 from fastapi_class.routers import Metadata, Method
 
-
-def _view_class_name_default_parser(cls: object, method: str):
-    class_name = " ".join(re.findall(r"[A-Z][^A-Z]*", cls.__name__.replace("View", "")))
-    return f"{method.capitalize()} {class_name}"
-
-
 COMMON_KEYWORD = "common"
 RESPONSE_MODEL_ATTRIBUTE_NAME = "RESPONSE_MODEL"
 RESPONSE_CLASS_ATTRIBUTE_NAME = "RESPONSE_CLASS"
 ENDPOINT_METADATA_ATTRIBUTE_NAME = "ENDPOINT_METADATA"
 EXCEPTIONS_ATTRIBUTE_NAME = "EXCEPTIONS"
```

### Comparing `fastapi_class-3.2.0/fastapi_class/exception/handler.py` & `fastapi_class-3.3.0/fastapi_class/exception/handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from abc import ABC, abstractmethod
 from collections.abc import Iterable
 from typing import Any
 
 from fastapi import HTTPException, status
 
 UNKOWN_SERVER_ERROR_DETAIL = "Unknown server error"
```

### Comparing `fastapi_class-3.2.0/scripts/clean.sh` & `fastapi_class-3.3.0/scripts/clean.sh`

 * *Files identical despite different names*

### Comparing `fastapi_class-3.2.0/tests/test_exceptions.py` & `fastapi_class-3.3.0/tests/test_exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from unittest.mock import patch
 
 import pytest
 
 from fastapi_class.exception import (
     UNKOWN_SERVER_ERROR_DETAIL,
     ExceptionAbstract,
```

### Comparing `fastapi_class-3.2.0/tests/test_metadata.py` & `fastapi_class-3.3.0/tests/test_metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import Any
 
 import pytest
 from fastapi.responses import Response
 from pydantic import BaseModel
 
 from fastapi_class import Metadata
```

### Comparing `fastapi_class-3.2.0/tests/test_openapi.py` & `fastapi_class-3.3.0/tests/test_openapi.py`

 * *Files identical despite different names*

### Comparing `fastapi_class-3.2.0/tests/test_routers.py` & `fastapi_class-3.3.0/tests/test_routers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+from __future__ import annotations
+
 from collections.abc import Callable, Iterable
 from types import FunctionType
 
 import pytest
 
 from fastapi_class import Method, endpoint
 
 
 async def dummy_function():
     pass  # pragma: no cover
 
 
-def assert_methods_in_metadata(_endpoint: Callable, methods: Iterable[Method]):
+def assert_methods_in_metadata(_endpoint: Callable, methods: Iterable[str | Method]):
     assert _endpoint.__endpoint_metadata
     assert len(_endpoint.__endpoint_metadata.methods) == len(methods)
     assert all(method in _endpoint.__endpoint_metadata.methods for method in methods)
 
 
 @pytest.mark.parametrize("method", Method)
 def test_endpoint__correct(method: Method):
```

### Comparing `fastapi_class-3.2.0/tests/test_views.py` & `fastapi_class-3.3.0/tests/test_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import pytest
 from fastapi import APIRouter, FastAPI, status
 
 from fastapi_class import Method, View
 from tests.factory import Factory
```

### Comparing `fastapi_class-3.2.0/.gitignore` & `fastapi_class-3.3.0/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -123,7 +123,10 @@
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
+
+# Pycharm
+.idea/
```

### Comparing `fastapi_class-3.2.0/LICENSE` & `fastapi_class-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_class-3.2.0/README.md` & `fastapi_class-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_class-3.2.0/pyproject.toml` & `fastapi_class-3.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fastapi_class"
 description = "Simplifies class-based views for more organized and maintainable code in FastAPI."
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.8"
 license = "MIT"
 authors = [
     { name = "Yasser Tahiri", email = "hello@yezz.me" },
 ]
 
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
     "Framework :: FastAPI",
     "Framework :: Pydantic",
     "Framework :: AsyncIO",
     "Programming Language :: Python",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Internet :: WWW/HTTP :: Session",
     "Typing :: Typed",
 ]
```

### Comparing `fastapi_class-3.2.0/PKG-INFO` & `fastapi_class-3.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: fastapi_class
-Version: 3.2.0
+Version: 3.3.0
 Summary: Simplifies class-based views for more organized and maintainable code in FastAPI.
 Project-URL: Homepage, https://github.com/yezz123/fastapi-class
 Project-URL: Funding, https://github.com/sponsors/yezz123
 Author-email: Yasser Tahiri <hello@yezz.me>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Framework :: AsyncIO
 Classifier: Framework :: FastAPI
 Classifier: Framework :: Pydantic
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Classifier: Typing :: Typed
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Requires-Dist: fastapi<0.96.0,>=0.65.2
 Requires-Dist: pydantic!=1.7,!=1.7.1,!=1.7.2,!=1.7.3,!=1.8,!=1.8.1,<2.0.0,>=1.6.2
 Provides-Extra: lint
 Requires-Dist: mypy==1.2.0; extra == 'lint'
 Requires-Dist: pre-commit==3.2.2; extra == 'lint'
 Provides-Extra: test
 Requires-Dist: pytest-asyncio==0.21.0; extra == 'test'
```


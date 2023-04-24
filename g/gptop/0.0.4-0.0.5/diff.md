# Comparing `tmp/gptop-0.0.4.tar.gz` & `tmp/gptop-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptop-0.0.4.tar", last modified: Mon Apr 24 03:14:01 2023, max compression
+gzip compressed data, was "gptop-0.0.5.tar", last modified: Mon Apr 24 03:37:52 2023, max compression
```

## Comparing `gptop-0.0.4.tar` & `gptop-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 nickcrews   (501) staff       (20)        0 2023-04-24 03:14:01.850331 gptop-0.0.4/
--rw-r--r--   0 nickcrews   (501) staff       (20)     1066 2023-04-21 22:10:41.000000 gptop-0.0.4/LICENSE
--rw-r--r--   0 nickcrews   (501) staff       (20)     2109 2023-04-24 03:14:01.850053 gptop-0.0.4/PKG-INFO
--rw-r--r--   0 nickcrews   (501) staff       (20)     1732 2023-04-22 16:38:46.000000 gptop-0.0.4/README.md
-drwxr-xr-x   0 nickcrews   (501) staff       (20)        0 2023-04-24 03:14:01.847303 gptop-0.0.4/gptop/
--rw-r--r--   0 nickcrews   (501) staff       (20)      286 2023-04-23 22:25:39.000000 gptop-0.0.4/gptop/__init__.py
--rw-r--r--   0 nickcrews   (501) staff       (20)     3779 2023-04-23 21:47:39.000000 gptop-0.0.4/gptop/operation.py
--rw-r--r--   0 nickcrews   (501) staff       (20)     4318 2023-04-23 22:08:45.000000 gptop-0.0.4/gptop/operation_utils.py
--rw-r--r--   0 nickcrews   (501) staff       (20)     5060 2023-04-23 21:10:02.000000 gptop-0.0.4/gptop/operator.py
--rw-r--r--   0 nickcrews   (501) staff       (20)      459 2023-04-23 21:06:19.000000 gptop-0.0.4/gptop/utils.py
-drwxr-xr-x   0 nickcrews   (501) staff       (20)        0 2023-04-24 03:14:01.849649 gptop-0.0.4/gptop.egg-info/
--rw-r--r--   0 nickcrews   (501) staff       (20)     2109 2023-04-24 03:14:01.000000 gptop-0.0.4/gptop.egg-info/PKG-INFO
--rw-r--r--   0 nickcrews   (501) staff       (20)      265 2023-04-24 03:14:01.000000 gptop-0.0.4/gptop.egg-info/SOURCES.txt
--rw-r--r--   0 nickcrews   (501) staff       (20)        1 2023-04-24 03:14:01.000000 gptop-0.0.4/gptop.egg-info/dependency_links.txt
--rw-r--r--   0 nickcrews   (501) staff       (20)      277 2023-04-24 03:14:01.000000 gptop-0.0.4/gptop.egg-info/requires.txt
--rw-r--r--   0 nickcrews   (501) staff       (20)        6 2023-04-24 03:14:01.000000 gptop-0.0.4/gptop.egg-info/top_level.txt
--rw-r--r--   0 nickcrews   (501) staff       (20)       38 2023-04-24 03:14:01.850418 gptop-0.0.4/setup.cfg
--rw-r--r--   0 nickcrews   (501) staff       (20)     1258 2023-04-24 03:13:38.000000 gptop-0.0.4/setup.py
+drwxr-xr-x   0 nickcrews   (501) staff       (20)        0 2023-04-24 03:37:52.042684 gptop-0.0.5/
+-rw-r--r--   0 nickcrews   (501) staff       (20)     1066 2023-04-21 22:10:41.000000 gptop-0.0.5/LICENSE
+-rw-r--r--   0 nickcrews   (501) staff       (20)     2109 2023-04-24 03:37:52.042390 gptop-0.0.5/PKG-INFO
+-rw-r--r--   0 nickcrews   (501) staff       (20)     1732 2023-04-22 16:38:46.000000 gptop-0.0.5/README.md
+drwxr-xr-x   0 nickcrews   (501) staff       (20)        0 2023-04-24 03:37:52.040251 gptop-0.0.5/gptop/
+-rw-r--r--   0 nickcrews   (501) staff       (20)      400 2023-04-24 03:37:07.000000 gptop-0.0.5/gptop/__init__.py
+-rw-r--r--   0 nickcrews   (501) staff       (20)     3818 2023-04-24 03:33:45.000000 gptop-0.0.5/gptop/operation.py
+-rw-r--r--   0 nickcrews   (501) staff       (20)     4409 2023-04-24 03:35:21.000000 gptop-0.0.5/gptop/operation_utils.py
+-rw-r--r--   0 nickcrews   (501) staff       (20)     5065 2023-04-24 03:32:59.000000 gptop-0.0.5/gptop/operator.py
+-rw-r--r--   0 nickcrews   (501) staff       (20)      471 2023-04-24 03:32:01.000000 gptop-0.0.5/gptop/utils.py
+drwxr-xr-x   0 nickcrews   (501) staff       (20)        0 2023-04-24 03:37:52.041961 gptop-0.0.5/gptop.egg-info/
+-rw-r--r--   0 nickcrews   (501) staff       (20)     2109 2023-04-24 03:37:51.000000 gptop-0.0.5/gptop.egg-info/PKG-INFO
+-rw-r--r--   0 nickcrews   (501) staff       (20)      265 2023-04-24 03:37:52.000000 gptop-0.0.5/gptop.egg-info/SOURCES.txt
+-rw-r--r--   0 nickcrews   (501) staff       (20)        1 2023-04-24 03:37:51.000000 gptop-0.0.5/gptop.egg-info/dependency_links.txt
+-rw-r--r--   0 nickcrews   (501) staff       (20)      277 2023-04-24 03:37:51.000000 gptop-0.0.5/gptop.egg-info/requires.txt
+-rw-r--r--   0 nickcrews   (501) staff       (20)        6 2023-04-24 03:37:51.000000 gptop-0.0.5/gptop.egg-info/top_level.txt
+-rw-r--r--   0 nickcrews   (501) staff       (20)       38 2023-04-24 03:37:52.042773 gptop-0.0.5/setup.cfg
+-rw-r--r--   0 nickcrews   (501) staff       (20)     1258 2023-04-24 03:37:47.000000 gptop-0.0.5/setup.py
```

### Comparing `gptop-0.0.4/LICENSE` & `gptop-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gptop-0.0.4/PKG-INFO` & `gptop-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptop
-Version: 0.0.4
+Version: 0.0.5
 Summary: Handles communication with GPTs
 Author: Nick Crews
 Keywords: gptop GPT operator llm ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `gptop-0.0.4/README.md` & `gptop-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `gptop-0.0.4/gptop/operation.py` & `gptop-0.0.5/gptop/operation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-import json
-import requests
-from enum import Enum
+import json as _json
+import requests as _requests
+from enum import Enum as _Enum
 
 
-class OperationType(str, Enum):
+class OperationType(str, _Enum):
     POST = "POST"
     GET = "GET"
     PUT = "PUT"
     PATCH = "PATCH"
     DELETE = "DELETE"
 
 
@@ -33,15 +33,15 @@
         self.description = description
         self.url = url
         self.path = path
         self.requires_auth = requires_auth
         self.schema = schema
 
     def __repr__(self) -> str:
-        return json.dumps(self.__dict__)
+        return _json.dumps(self.__dict__)
 
     @classmethod
     def from_obj(self, obj):
         """
         Returns an instance of an operation from a dict object
         """
 
@@ -78,57 +78,57 @@
         """
         Executes the command.
 
         Returns: The response provided by the execution API
         """
 
         result = None
-        data = json.dumps(body).encode('utf-8')
+        data = _json.dumps(body).encode('utf-8')
 
         headers = {
             'Accept': 'application/json',
             'Content-Type': 'application/json'
         }
         if self.requires_auth:
             headers["Authorization"] = f"Bearer {auth_token}"
 
         if self.type == OperationType.POST:
-            result = requests.post(
+            result = _requests.post(
                 self.endpoint(),
                 headers=headers,
                 params=params,
                 data=data
             )
 
         elif self.type == OperationType.GET:
-            result = requests.get(
+            result = _requests.get(
                 self.endpoint(),
                 headers=headers,
                 params=params,
                 data=data
             )
 
         elif self.type == OperationType.PUT:
-            result = requests.put(
+            result = _requests.put(
                 self.endpoint(),
                 headers=headers,
                 params=params,
                 data=data
             )
 
         elif self.type == OperationType.PATCH:
-            result = requests.patch(
+            result = _requests.patch(
                 self.endpoint(),
                 headers=headers,
                 params=params,
                 data=data
             )
 
         elif self.type == OperationType.DELETE:
-            result = requests.delete(
+            result = _requests.delete(
                 self.endpoint(),
                 headers=headers,
                 params=params,
                 data=data
             )
 
         if not result:
```

### Comparing `gptop-0.0.4/gptop/operation_utils.py` & `gptop-0.0.5/gptop/operation_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-import os
-import json
-from uuid import uuid4
-import pinecone
-from openai.embeddings_utils import get_embedding
-from .operation import Operation
+import os as _os
+import json as _json
+from uuid import uuid4 as _uuid4
+import pinecone as _pinecone
+from openai.embeddings_utils import get_embedding as _get_embedding
+from .operation import Operation as _Operation
 
 
 class Utils():
     """
     A set of utility objects for managing operations
     """
 
@@ -25,30 +25,30 @@
         - schema: The schema of the operation
 
         Also writes the operation ID to the `ops_list.txt` file
 
         Returns: The created operation
         """
 
-        index = pinecone.Index(os.getenv("PINECONE_INDEX"))
+        index = _pinecone.Index(_os.getenv("PINECONE_INDEX"))
 
-        id = str(uuid4())
+        id = str(_uuid4())
 
-        operation = Operation(
+        operation = _Operation(
             id=id,
             type=type,
             name=name,
             description=description,
             url=url,
             path=path,
             requires_auth=requires_auth,
-            schema=json.dumps(json.loads(schema), separators=(',', ': '))
+            schema=_json.dumps(_json.loads(schema), separators=(',', ': '))
         )
 
-        embedding = get_embedding(operation.embedding_obj(),
+        embedding = _get_embedding(operation.embedding_obj(),
                                   engine="text-embedding-ada-002")
 
         to_upsert = zip([id], [embedding], [operation.metadata()])
 
         index.upsert(vectors=list(to_upsert), namespace=namespace)
 
         return operation
@@ -58,25 +58,25 @@
         """
         Fetches an existing operation from the vector database.
         - namespace: The namespace to store the embedding
         - id: The identifier of the operation
 
         Returns: The operation represented
         """
-        index = pinecone.Index(os.getenv("PINECONE_INDEX"))
+        index = _pinecone.Index(_os.getenv("PINECONE_INDEX"))
 
         result = index.fetch([id], namespace=namespace)
         vectors = result.get('vectors')
         vector = vectors.get(id)
 
         if not vector:
             return None
 
         obj = vector.get('metadata')
-        return Operation.from_obj(obj)
+        return _Operation.from_obj(obj)
 
     @classmethod
     def update_operation(self, namespace, id, type, name, description,
                          url, path, requires_auth, schema):
         """
         Updates an existing operation, creates a new embedding, and
         overrides the existing operation in the vector database.
@@ -87,28 +87,28 @@
         - path: The path to the operation
         - requires_auth: If the operation requires authentication
         - schema: The schema of the operation
 
         Returns: The updated operation
         """
 
-        operation = Operation(
+        operation = _Operation(
             id=id,
             type=type,
             name=name,
             description=description,
             url=url,
             path=path,
             requires_auth=requires_auth,
-            schema=json.dumps(json.loads(schema), separators=(',', ': '))
+            schema=_json.dumps(_json.loads(schema), separators=(',', ': '))
         )
 
-        index = pinecone.Index(os.getenv("PINECONE_INDEX"))
+        index = _pinecone.Index(_os.getenv("PINECONE_INDEX"))
 
-        embedding = get_embedding(operation.embedding_obj(),
+        embedding = _get_embedding(operation.embedding_obj(),
                                   engine="text-embedding-ada-002")
 
         to_upsert = zip([id], [embedding], [operation.metadata()])
 
         index.upsert(vectors=list(to_upsert), namespace=namespace)
 
         return operation
@@ -119,20 +119,20 @@
         Removes an existing operation from the vector database.
         - namespace: The namespace to store the embedding
         - id: The identifier of the operation
 
         Also removes the operation ID from `ops_list.txt` file.
         """
 
-        index = pinecone.Index(os.getenv("PINECONE_INDEX"))
+        index = _pinecone.Index(_os.getenv("PINECONE_INDEX"))
 
         index.delete(ids=[id], namespace=namespace)
 
     @classmethod
     def remove_namespace(self, namespace: str):
         """
         [DANGEROUS] Deletes an entire namespace of operations.
         - namespace: The namespace in the vector database
         """
-        index = pinecone.Index(os.getenv("PINECONE_INDEX"))
+        index = _pinecone.Index(_os.getenv("PINECONE_INDEX"))
 
         index.delete(deleteAll='true', namespace=namespace)
```

### Comparing `gptop-0.0.4/gptop/operator.py` & `gptop-0.0.5/gptop/operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import json
 import pinecone
 from openai.embeddings_utils import get_embedding
 from openai import ChatCompletion
 from .operation import Operation
 from .operation_utils import Utils
-from .utils import llm_response, llm_json
+from .utils import _llm_json, _llm_response
 
 
 class Operator():
 
     def __init__(self, namespace: str) -> None:
         self.namespace = namespace
 
@@ -72,15 +72,15 @@
                 {"role": "user", "content": f"Operations: {json.dumps(clean_ops)}"},
                 {"role": "user", "content": f"Prompt: {prompt}"},
                 {"role": "user", "content": "Output the ID of the operation and nothing more."}
             ],
             temperature=0.0
         )
 
-        op_id = llm_response(response)
+        op_id = _llm_response(response)
         operation = None
         for op in operations:
             if op.id == op_id:
                 operation = op
                 break
 
         return operation
@@ -106,15 +106,15 @@
                 {"role": "user", "content": f"Operation: {operation.__dict__}"},
                 {"role": "user", "content": f"Prompt: {prompt}"},
                 {"role": "user", "content": "Output the params and body in JSON format and nothing more."}
             ],
             temperature=0.0
         )
 
-        return llm_json(response)
+        return _llm_json(response)
 
     def execute(self, operation: Operation, params: any, body: any, auth_token: str=None):
         """
         Executes the provided operation.
 
         Returns: Value from operation
         """
@@ -139,8 +139,8 @@
                 {"role": "user", "content": f"Operation: {operation.__dict__}"},
                 {"role": "user", "content": f"Values passed to operation: {values}"},
                 {"role": "user", "content": f"Execution result: {result}"}
             ],
             temperature=0.0
         )
 
-        return llm_response(response)
+        return _llm_response(response)
```

### Comparing `gptop-0.0.4/gptop.egg-info/PKG-INFO` & `gptop-0.0.5/gptop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptop
-Version: 0.0.4
+Version: 0.0.5
 Summary: Handles communication with GPTs
 Author: Nick Crews
 Keywords: gptop GPT operator llm ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `gptop-0.0.4/setup.py` & `gptop-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gptop",
-    version="0.0.4",
+    version="0.0.5",
     author="Nick Crews",
     description="Handles communication with GPTs",
     keywords="gptop GPT operator llm ai",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(exclude=[
         "tests",
```


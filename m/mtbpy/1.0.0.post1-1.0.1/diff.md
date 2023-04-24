# Comparing `tmp/mtbpy-1.0.0.post1.tar.gz` & `tmp/mtbpy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mtbpy-1.0.0.post1.tar", last modified: Thu Feb 25 02:27:01 2021, max compression
+gzip compressed data, was "mtbpy-1.0.1.tar", last modified: Fri Apr 21 15:52:59 2023, max compression
```

## Comparing `mtbpy-1.0.0.post1.tar` & `mtbpy-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2021-02-25 02:27:01.000000 mtbpy-1.0.0.post1/
--rw-rw-rw-   0        0        0     1090 2020-04-06 19:47:21.000000 mtbpy-1.0.0.post1/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2021-02-25 02:27:01.000000 mtbpy-1.0.0.post1/mtbpy/
--rw-rw-rw-   0        0        0     4886 2020-03-05 13:56:14.000000 mtbpy-1.0.0.post1/mtbpy/mtbpy.py
--rw-rw-rw-   0        0        0    21894 2021-02-25 02:26:55.000000 mtbpy-1.0.0.post1/mtbpy/mtb_command_rpc_pb2.py
--rw-rw-rw-   0        0        0     5897 2021-02-25 02:26:55.000000 mtbpy-1.0.0.post1/mtbpy/mtb_command_rpc_pb2_grpc.py
--rw-rw-rw-   0        0        0        0 2019-11-13 19:44:08.000000 mtbpy-1.0.0.post1/mtbpy/__init__.py
-drwxrwxrwx   0        0        0        0 2021-02-25 02:27:01.000000 mtbpy-1.0.0.post1/mtbpy.egg-info/
--rw-rw-rw-   0        0        0        1 2021-02-25 02:27:01.000000 mtbpy-1.0.0.post1/mtbpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      993 2021-02-25 02:27:01.000000 mtbpy-1.0.0.post1/mtbpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       55 2021-02-25 02:27:01.000000 mtbpy-1.0.0.post1/mtbpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0      280 2021-02-25 02:27:01.000000 mtbpy-1.0.0.post1/mtbpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        6 2021-02-25 02:27:01.000000 mtbpy-1.0.0.post1/mtbpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      993 2021-02-25 02:27:01.000000 mtbpy-1.0.0.post1/PKG-INFO
--rw-rw-rw-   0        0        0      202 2019-11-13 19:44:08.000000 mtbpy-1.0.0.post1/README.md
--rw-rw-rw-   0        0        0       85 2021-02-25 02:27:01.000000 mtbpy-1.0.0.post1/setup.cfg
--rw-rw-rw-   0        0        0     1115 2021-02-24 20:33:31.000000 mtbpy-1.0.0.post1/setup.py
+drwxr-xr-x   0 AzDevOps_azpcontainer  (1001) AzDevOps_azpcontainer  (1001)        0 2023-04-21 15:52:59.601247 mtbpy-1.0.1/
+-rw-r--r--   0 AzDevOps_azpcontainer  (1001) AzDevOps_azpcontainer  (1001)     1069 2023-04-11 20:11:12.000000 mtbpy-1.0.1/LICENSE.txt
+-rw-r--r--   0 AzDevOps_azpcontainer  (1001) AzDevOps_azpcontainer  (1001)     2168 2023-04-21 15:52:59.601247 mtbpy-1.0.1/PKG-INFO
+-rw-r--r--   0 AzDevOps_azpcontainer  (1001) AzDevOps_azpcontainer  (1001)      199 2023-04-11 20:11:12.000000 mtbpy-1.0.1/README.md
+drwxr-xr-x   0 AzDevOps_azpcontainer  (1001) AzDevOps_azpcontainer  (1001)        0 2023-04-21 15:52:59.601247 mtbpy-1.0.1/mtbpy/
+-rw-r--r--   0 AzDevOps_azpcontainer  (1001) AzDevOps_azpcontainer  (1001)        0 2023-04-11 20:11:12.000000 mtbpy-1.0.1/mtbpy/__init__.py
+-rw-r--r--   0 AzDevOps_azpcontainer  (1001) AzDevOps_azpcontainer  (1001)     3877 2023-04-21 15:52:54.000000 mtbpy-1.0.1/mtbpy/mtb_command_rpc_pb2.py
+-rw-r--r--   0 AzDevOps_azpcontainer  (1001) AzDevOps_azpcontainer  (1001)    10882 2023-04-21 15:52:54.000000 mtbpy-1.0.1/mtbpy/mtb_command_rpc_pb2_grpc.py
+-rw-r--r--   0 AzDevOps_azpcontainer  (1001) AzDevOps_azpcontainer  (1001)     4756 2023-04-11 20:11:12.000000 mtbpy-1.0.1/mtbpy/mtbpy.py
+drwxr-xr-x   0 AzDevOps_azpcontainer  (1001) AzDevOps_azpcontainer  (1001)        0 2023-04-21 15:52:59.601247 mtbpy-1.0.1/mtbpy.egg-info/
+-rw-r--r--   0 AzDevOps_azpcontainer  (1001) AzDevOps_azpcontainer  (1001)     2168 2023-04-21 15:52:59.000000 mtbpy-1.0.1/mtbpy.egg-info/PKG-INFO
+-rw-r--r--   0 AzDevOps_azpcontainer  (1001) AzDevOps_azpcontainer  (1001)      276 2023-04-21 15:52:59.000000 mtbpy-1.0.1/mtbpy.egg-info/SOURCES.txt
+-rw-r--r--   0 AzDevOps_azpcontainer  (1001) AzDevOps_azpcontainer  (1001)        1 2023-04-21 15:52:59.000000 mtbpy-1.0.1/mtbpy.egg-info/dependency_links.txt
+-rw-r--r--   0 AzDevOps_azpcontainer  (1001) AzDevOps_azpcontainer  (1001)       60 2023-04-21 15:52:59.000000 mtbpy-1.0.1/mtbpy.egg-info/requires.txt
+-rw-r--r--   0 AzDevOps_azpcontainer  (1001) AzDevOps_azpcontainer  (1001)        6 2023-04-21 15:52:59.000000 mtbpy-1.0.1/mtbpy.egg-info/top_level.txt
+-rw-r--r--   0 AzDevOps_azpcontainer  (1001) AzDevOps_azpcontainer  (1001)      938 2023-04-21 15:51:44.000000 mtbpy-1.0.1/pyproject.toml
+-rw-r--r--   0 AzDevOps_azpcontainer  (1001) AzDevOps_azpcontainer  (1001)       38 2023-04-21 15:52:59.601247 mtbpy-1.0.1/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mtbpy-1.0.0.post1/mtbpy/mtbpy.py` & `mtbpy-1.0.1/mtbpy/mtbpy.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,130 +1,130 @@
-import os
-from itertools import cycle
-from numbers import Number
-
-import grpc
-from mtbpy import mtb_command_rpc_pb2
-from mtbpy import mtb_command_rpc_pb2_grpc
-
-
-class mtb_instance(object):
-    def __init__(self):
-        address = "127.0.0.1:{0}".format(os.getenv("MTB_RPC_PORT"))
-        self.channel = grpc.insecure_channel(address, options=[
-            ("grpc.max_receive_message_length", -1)
-        ])
-        try:
-            grpc.channel_ready_future(self.channel).result(timeout=5)
-        except grpc.FutureTimeoutError:
-            raise RuntimeError(
-                "Error connecting to Minitab at {0}".format(address))
-        self.rpc_stub = mtb_command_rpc_pb2_grpc.MtbCommandStub(self.channel)
-
-    def __enter__(self):
-        return self
-
-    def __exit__(self, exc_type, exc_value, traceback):
-        self.channel.close()
-
-    def get_column(self, column_name):
-        request = mtb_command_rpc_pb2.VariableRequest()
-        request.var_type = mtb_command_rpc_pb2.VariableType.VAR_COLUMN
-        request.var_id = column_name
-        try:
-            response = self.rpc_stub.GetVariable(request)
-        except grpc.RpcError as e:
-            if e.code() != grpc.StatusCode.NOT_FOUND:
-                raise
-        else:
-            if response.found:
-                if len(response.numeric_data) > 0:
-                    return response.numeric_data
-                elif len(response.text_data) > 0:
-                    return response.text_data
-
-    def get_constant(self, constant_name):
-        request = mtb_command_rpc_pb2.VariableRequest()
-        request.var_type = mtb_command_rpc_pb2.VariableType.VAR_CONSTANT
-        request.var_id = constant_name
-        try:
-            response = self.rpc_stub.GetVariable(request)
-        except grpc.RpcError as e:
-            if e.code() != grpc.StatusCode.NOT_FOUND:
-                raise
-        else:
-            if response.found:
-                if len(response.numeric_data) > 0:
-                    return response.numeric_data[0]
-                elif len(response.text_data) > 0:
-                    return response.text_data[0]
-
-    def get_matrix(self, matrix_name):
-        request = mtb_command_rpc_pb2.VariableRequest()
-        request.var_type = mtb_command_rpc_pb2.VariableType.VAR_MATRIX
-        request.var_id = matrix_name
-        try:
-            response = self.rpc_stub.GetVariable(request)
-        except grpc.RpcError as e:
-            if e.code() != grpc.StatusCode.NOT_FOUND:
-                raise
-        else:
-            if response.found and len(response.numeric_data) > 0:
-                lists = [[] for i in range(response.m)]
-                for d, m in zip(response.numeric_data, cycle(range(response.m))):
-                    lists[m].append(d)
-                return lists
-
-    def add_message(self, content):
-        request = mtb_command_rpc_pb2.AddMessageRequest()
-        request.content = content
-        self.rpc_stub.AddMessage(request)
-
-    def set_note(self, content):
-        request = mtb_command_rpc_pb2.SetCommandNoteRequest()
-        request.content = content
-        self.rpc_stub.SetCommandNote(request)
-
-    def set_command_title(self, content):
-        request = mtb_command_rpc_pb2.SetCommandTitleRequest()
-        request.content = content
-        try:
-            self.rpc_stub.SetCommandTitle(request)
-        except grpc.RpcError as e:
-            if e.code() != grpc.StatusCode.INVALID_ARGUMENT:
-                raise
-
-    def add_image(self, path):
-        image_data = None
-        with open(path, "rb") as f:
-            image_data = f.read()
-        self.add_image_bytes(image_data)
-
-    def add_image_bytes(self, bytes):
-        request = mtb_command_rpc_pb2.AddImageRequest()
-        request.image_data = bytes
-        self.rpc_stub.AddImage(request)
-
-    def add_table(self, columns, headers=[], title="", footnote=""):
-        request = mtb_command_rpc_pb2.AddTableRequest()
-        if isinstance(title, str):
-            request.title = title
-        if isinstance(footnote, str):
-            request.footnote = footnote
-
-        for column in columns:
-            data = request.columns.add()
-            if len(column) == 0:
-                # empty column, but still need to 'set' the oneof
-                data.numeric_data.data[:] = []
-                continue
-            if isinstance(column[0], Number):
-                data.numeric_data.data[:] = map(float, column)
-            elif isinstance(column[0], str):
-                data.text_data.data[:] = map(str, column)
-            else:
-                raise TypeError(
-                    "Table data values must be of type str or a subclass of `numbers.Number`.")
-
-        request.headers[:] = map(str, headers)
-
-        self.rpc_stub.AddTable(request)
+import os
+from itertools import cycle
+from numbers import Number
+
+import grpc
+from mtbpy import mtb_command_rpc_pb2
+from mtbpy import mtb_command_rpc_pb2_grpc
+
+
+class mtb_instance(object):
+    def __init__(self):
+        address = "127.0.0.1:{0}".format(os.getenv("MTB_RPC_PORT"))
+        self.channel = grpc.insecure_channel(address, options=[
+            ("grpc.max_receive_message_length", -1)
+        ])
+        try:
+            grpc.channel_ready_future(self.channel).result(timeout=5)
+        except grpc.FutureTimeoutError:
+            raise RuntimeError(
+                "Error connecting to Minitab at {0}".format(address))
+        self.rpc_stub = mtb_command_rpc_pb2_grpc.MtbCommandStub(self.channel)
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        self.channel.close()
+
+    def get_column(self, column_name):
+        request = mtb_command_rpc_pb2.VariableRequest()
+        request.var_type = mtb_command_rpc_pb2.VariableType.VAR_COLUMN
+        request.var_id = column_name
+        try:
+            response = self.rpc_stub.GetVariable(request)
+        except grpc.RpcError as e:
+            if e.code() != grpc.StatusCode.NOT_FOUND:
+                raise
+        else:
+            if response.found:
+                if len(response.numeric_data) > 0:
+                    return response.numeric_data
+                elif len(response.text_data) > 0:
+                    return response.text_data
+
+    def get_constant(self, constant_name):
+        request = mtb_command_rpc_pb2.VariableRequest()
+        request.var_type = mtb_command_rpc_pb2.VariableType.VAR_CONSTANT
+        request.var_id = constant_name
+        try:
+            response = self.rpc_stub.GetVariable(request)
+        except grpc.RpcError as e:
+            if e.code() != grpc.StatusCode.NOT_FOUND:
+                raise
+        else:
+            if response.found:
+                if len(response.numeric_data) > 0:
+                    return response.numeric_data[0]
+                elif len(response.text_data) > 0:
+                    return response.text_data[0]
+
+    def get_matrix(self, matrix_name):
+        request = mtb_command_rpc_pb2.VariableRequest()
+        request.var_type = mtb_command_rpc_pb2.VariableType.VAR_MATRIX
+        request.var_id = matrix_name
+        try:
+            response = self.rpc_stub.GetVariable(request)
+        except grpc.RpcError as e:
+            if e.code() != grpc.StatusCode.NOT_FOUND:
+                raise
+        else:
+            if response.found and len(response.numeric_data) > 0:
+                lists = [[] for i in range(response.m)]
+                for d, m in zip(response.numeric_data, cycle(range(response.m))):
+                    lists[m].append(d)
+                return lists
+
+    def add_message(self, content):
+        request = mtb_command_rpc_pb2.AddMessageRequest()
+        request.content = content
+        self.rpc_stub.AddMessage(request)
+
+    def set_note(self, content):
+        request = mtb_command_rpc_pb2.SetCommandNoteRequest()
+        request.content = content
+        self.rpc_stub.SetCommandNote(request)
+
+    def set_command_title(self, content):
+        request = mtb_command_rpc_pb2.SetCommandTitleRequest()
+        request.content = content
+        try:
+            self.rpc_stub.SetCommandTitle(request)
+        except grpc.RpcError as e:
+            if e.code() != grpc.StatusCode.INVALID_ARGUMENT:
+                raise
+
+    def add_image(self, path):
+        image_data = None
+        with open(path, "rb") as f:
+            image_data = f.read()
+        self.add_image_bytes(image_data)
+
+    def add_image_bytes(self, bytes):
+        request = mtb_command_rpc_pb2.AddImageRequest()
+        request.image_data = bytes
+        self.rpc_stub.AddImage(request)
+
+    def add_table(self, columns, headers=[], title="", footnote=""):
+        request = mtb_command_rpc_pb2.AddTableRequest()
+        if isinstance(title, str):
+            request.title = title
+        if isinstance(footnote, str):
+            request.footnote = footnote
+
+        for column in columns:
+            data = request.columns.add()
+            if len(column) == 0:
+                # empty column, but still need to 'set' the oneof
+                data.numeric_data.data[:] = []
+                continue
+            if isinstance(column[0], Number):
+                data.numeric_data.data[:] = map(float, column)
+            elif isinstance(column[0], str):
+                data.text_data.data[:] = map(str, column)
+            else:
+                raise TypeError(
+                    "Table data values must be of type str or a subclass of `numbers.Number`.")
+
+        request.headers[:] = map(str, headers)
+
+        self.rpc_stub.AddTable(request)
```


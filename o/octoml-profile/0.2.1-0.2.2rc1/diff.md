# Comparing `tmp/octoml_profile-0.2.1.tar.gz` & `tmp/octoml_profile-0.2.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octoml_profile-0.2.1.tar", max compression
+gzip compressed data, was "octoml_profile-0.2.2rc1.tar", max compression
```

## Comparing `octoml_profile-0.2.1.tar` & `octoml_profile-0.2.2rc1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    11358 2023-03-29 21:52:57.058588 octoml_profile-0.2.1/LICENSE
--rw-r--r--   0        0        0      319 2023-03-29 21:52:57.058588 octoml_profile-0.2.1/octoml_profile/README.md
--rw-r--r--   0        0        0     1204 2023-03-29 21:52:57.058588 octoml_profile-0.2.1/octoml_profile/__init__.py
--rw-r--r--   0        0        0      656 2023-03-29 21:53:02.958161 octoml_profile-0.2.1/octoml_profile/_about.py
--rw-r--r--   0        0        0    29087 2023-03-29 21:52:57.058588 octoml_profile-0.2.1/octoml_profile/client.py
--rw-r--r--   0        0        0     1757 2023-03-29 21:52:57.058588 octoml_profile-0.2.1/octoml_profile/conversion_util.py
--rw-r--r--   0        0        0    29697 2023-03-29 21:52:57.058588 octoml_profile-0.2.1/octoml_profile/dynamo.py
--rw-r--r--   0        0        0     1312 2023-03-29 21:52:57.058588 octoml_profile-0.2.1/octoml_profile/errors.py
--rw-r--r--   0        0        0    15441 2023-03-29 21:52:57.058588 octoml_profile-0.2.1/octoml_profile/fx2proto.py
--rw-r--r--   0        0        0     6199 2023-03-29 21:52:57.058588 octoml_profile-0.2.1/octoml_profile/inference_session.py
--rw-r--r--   0        0        0      576 2023-03-29 21:52:57.058588 octoml_profile-0.2.1/octoml_profile/interceptors/__init__.py
--rw-r--r--   0        0        0     1498 2023-03-29 21:52:57.058588 octoml_profile-0.2.1/octoml_profile/interceptors/auth.py
--rw-r--r--   0        0        0     2497 2023-03-29 21:52:57.058588 octoml_profile-0.2.1/octoml_profile/interceptors/base.py
--rw-r--r--   0        0        0      997 2023-03-29 21:52:57.058588 octoml_profile-0.2.1/octoml_profile/interceptors/cookie.py
--rw-r--r--   0        0        0     1190 2023-03-29 21:52:57.058588 octoml_profile-0.2.1/octoml_profile/log_util.py
--rw-r--r--   0        0        0     1025 2023-03-29 21:52:57.058588 octoml_profile-0.2.1/octoml_profile/patches/__init__.py
--rw-r--r--   0        0        0     2048 2023-03-29 21:52:57.059589 octoml_profile-0.2.1/octoml_profile/patches/build_map_unpack.py
--rw-r--r--   0        0        0     1860 2023-03-29 21:52:57.059589 octoml_profile-0.2.1/octoml_profile/patches/diffusers_output_type.py
--rw-r--r--   0        0        0     1064 2023-03-29 21:52:57.059589 octoml_profile-0.2.1/octoml_profile/patches/dyn_shape_call_neg.py
--rw-r--r--   0        0        0     1175 2023-03-29 21:52:57.059589 octoml_profile-0.2.1/octoml_profile/patches/iadd_tuple_tuple.py
--rw-r--r--   0        0        0     1028 2023-03-29 21:52:57.059589 octoml_profile-0.2.1/octoml_profile/patches/user_defined_call.py
--rw-r--r--   0        0        0      705 2023-03-29 21:52:57.059589 octoml_profile-0.2.1/octoml_profile/pricing.py
--rw-r--r--   0        0        0    11193 2023-03-29 21:52:57.508632 octoml_profile-0.2.1/octoml_profile/protos/fxgraph_pb2.py
--rw-r--r--   0        0        0      159 2023-03-29 21:52:57.508632 octoml_profile-0.2.1/octoml_profile/protos/fxgraph_pb2_grpc.py
--rw-r--r--   0        0        0    22704 2023-03-29 21:52:57.508632 octoml_profile-0.2.1/octoml_profile/protos/inference_base_pb2.py
--rw-r--r--   0        0        0      159 2023-03-29 21:52:57.508632 octoml_profile-0.2.1/octoml_profile/protos/inference_base_pb2_grpc.py
--rw-r--r--   0        0        0     4290 2023-03-29 21:52:57.508632 octoml_profile-0.2.1/octoml_profile/protos/remote_inference_pb2.py
--rw-r--r--   0        0        0    19277 2023-03-29 21:52:57.508632 octoml_profile-0.2.1/octoml_profile/protos/remote_inference_pb2_grpc.py
--rw-r--r--   0        0        0    14027 2023-03-29 21:52:57.059589 octoml_profile-0.2.1/octoml_profile/report.py
--rw-r--r--   0        0        0     2475 2023-03-29 21:52:57.059589 octoml_profile-0.2.1/octoml_profile/shape.py
--rw-r--r--   0        0        0     1667 2023-03-29 21:52:57.059589 octoml_profile-0.2.1/octoml_profile/workaround.py
--rw-r--r--   0        0        0     1126 2023-03-29 21:53:02.940160 octoml_profile-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      742 2023-03-29 21:53:04.858103 octoml_profile-0.2.1/setup.py
--rw-r--r--   0        0        0      547 2023-03-29 21:53:04.858329 octoml_profile-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-04-24 16:31:45.319711 octoml_profile-0.2.2rc1/LICENSE
+-rw-r--r--   0        0        0      319 2023-04-24 16:31:45.319711 octoml_profile-0.2.2rc1/octoml_profile/README.md
+-rw-r--r--   0        0        0     1242 2023-04-24 16:31:45.319711 octoml_profile-0.2.2rc1/octoml_profile/__init__.py
+-rw-r--r--   0        0        0      659 2023-04-24 16:31:51.810191 octoml_profile-0.2.2rc1/octoml_profile/_about.py
+-rw-r--r--   0        0        0    29912 2023-04-24 16:31:45.319711 octoml_profile-0.2.2rc1/octoml_profile/client.py
+-rw-r--r--   0        0        0     1757 2023-04-24 16:31:45.319711 octoml_profile-0.2.2rc1/octoml_profile/conversion_util.py
+-rw-r--r--   0        0        0    37765 2023-04-24 16:31:45.319711 octoml_profile-0.2.2rc1/octoml_profile/dynamo.py
+-rw-r--r--   0        0        0     1312 2023-04-24 16:31:45.319711 octoml_profile-0.2.2rc1/octoml_profile/errors.py
+-rw-r--r--   0        0        0    15537 2023-04-24 16:31:45.319711 octoml_profile-0.2.2rc1/octoml_profile/fx2proto.py
+-rw-r--r--   0        0        0     8422 2023-04-24 16:31:45.319711 octoml_profile-0.2.2rc1/octoml_profile/inference_session.py
+-rw-r--r--   0        0        0      576 2023-04-24 16:31:45.319711 octoml_profile-0.2.2rc1/octoml_profile/interceptors/__init__.py
+-rw-r--r--   0        0        0     1498 2023-04-24 16:31:45.319711 octoml_profile-0.2.2rc1/octoml_profile/interceptors/auth.py
+-rw-r--r--   0        0        0     2497 2023-04-24 16:31:45.320711 octoml_profile-0.2.2rc1/octoml_profile/interceptors/base.py
+-rw-r--r--   0        0        0      997 2023-04-24 16:31:45.320711 octoml_profile-0.2.2rc1/octoml_profile/interceptors/cookie.py
+-rw-r--r--   0        0        0     1182 2023-04-24 16:31:45.320711 octoml_profile-0.2.2rc1/octoml_profile/log_util.py
+-rw-r--r--   0        0        0     1025 2023-04-24 16:31:45.320711 octoml_profile-0.2.2rc1/octoml_profile/patches/__init__.py
+-rw-r--r--   0        0        0     2048 2023-04-24 16:31:45.320711 octoml_profile-0.2.2rc1/octoml_profile/patches/build_map_unpack.py
+-rw-r--r--   0        0        0     1860 2023-04-24 16:31:45.320711 octoml_profile-0.2.2rc1/octoml_profile/patches/diffusers_output_type.py
+-rw-r--r--   0        0        0     1064 2023-04-24 16:31:45.320711 octoml_profile-0.2.2rc1/octoml_profile/patches/dyn_shape_call_neg.py
+-rw-r--r--   0        0        0     1175 2023-04-24 16:31:45.320711 octoml_profile-0.2.2rc1/octoml_profile/patches/iadd_tuple_tuple.py
+-rw-r--r--   0        0        0     1115 2023-04-24 16:31:45.320711 octoml_profile-0.2.2rc1/octoml_profile/patches/user_defined_call.py
+-rw-r--r--   0        0        0      705 2023-04-24 16:31:45.320711 octoml_profile-0.2.2rc1/octoml_profile/pricing.py
+-rw-r--r--   0        0        0    11193 2023-04-24 16:31:45.914755 octoml_profile-0.2.2rc1/octoml_profile/protos/fxgraph_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-24 16:31:45.914755 octoml_profile-0.2.2rc1/octoml_profile/protos/fxgraph_pb2_grpc.py
+-rw-r--r--   0        0        0    23668 2023-04-24 16:31:45.914755 octoml_profile-0.2.2rc1/octoml_profile/protos/inference_base_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-24 16:31:45.914755 octoml_profile-0.2.2rc1/octoml_profile/protos/inference_base_pb2_grpc.py
+-rw-r--r--   0        0        0     4290 2023-04-24 16:31:45.914755 octoml_profile-0.2.2rc1/octoml_profile/protos/remote_inference_pb2.py
+-rw-r--r--   0        0        0    19277 2023-04-24 16:31:45.914755 octoml_profile-0.2.2rc1/octoml_profile/protos/remote_inference_pb2_grpc.py
+-rw-r--r--   0        0        0    19878 2023-04-24 16:31:45.320711 octoml_profile-0.2.2rc1/octoml_profile/report.py
+-rw-r--r--   0        0        0     2475 2023-04-24 16:31:45.320711 octoml_profile-0.2.2rc1/octoml_profile/shape.py
+-rw-r--r--   0        0        0     2955 2023-04-24 16:31:45.320711 octoml_profile-0.2.2rc1/octoml_profile/workaround.py
+-rw-r--r--   0        0        0     1149 2023-04-24 16:31:51.722185 octoml_profile-0.2.2rc1/pyproject.toml
+-rw-r--r--   0        0        0      772 2023-04-24 16:31:53.597915 octoml_profile-0.2.2rc1/setup.py
+-rw-r--r--   0        0        0      592 2023-04-24 16:31:53.598195 octoml_profile-0.2.2rc1/PKG-INFO
```

### Comparing `octoml_profile-0.2.1/LICENSE` & `octoml_profile-0.2.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.1/octoml_profile/__init__.py` & `octoml_profile-0.2.2rc1/octoml_profile/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from . import report
 from ._about import version
 from .client import RemoteInferenceSession, get_default_backends, get_supported_backends, \
     BackendSpec
-from .dynamo import accelerate, remote_profile, ProfileHandle
+from .dynamo import accelerate, remote_profile, ProfileHandle, remote_inference
 from .inference_session import InferenceSession
 from .patches import apply_patches
 
 
 __version__ = version
 
 __all__ = [
-    "accelerate", "remote_profile",
+    "accelerate", "remote_profile", "remote_inference",
     "get_default_backends", "get_supported_backends", "BackendSpec",
     "InferenceSession", "RemoteInferenceSession",
     "report", "ProfileHandle",
 ]
 
 try:
     import octoml_profile_private  # noqa: F401
```

### Comparing `octoml_profile-0.2.1/octoml_profile/_about.py` & `octoml_profile-0.2.2rc1/octoml_profile/_about.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-version = "0.2.1"
-git_commit_hash = "2e79d869e39c896de51a074f716b9777e9a15767"
+version = "0.2.2rc1"
+git_commit_hash = "009309ea2408255db27d3a9050fc79837ba86810"
```

### Comparing `octoml_profile-0.2.1/octoml_profile/client.py` & `octoml_profile-0.2.2rc1/octoml_profile/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,61 +21,74 @@
 import traceback
 import weakref
 from collections import defaultdict
 from contextlib import ExitStack
 from functools import partial
 from getpass import getpass
 from os.path import expanduser
-from typing import Iterator, Mapping, Optional, Sequence, Tuple, Union, Iterable, NamedTuple
+from typing import (Callable, Iterator, Mapping, Optional, Sequence, Tuple,
+                    Union, Iterable, NamedTuple)
 from uuid import UUID
 
 import grpc
 
 from .conversion_util import numpy_to_proto
 from .errors import LoadModelError, CreateSessionError
-from .inference_session import (BackendSpec, InferenceSession, ModelRunner,
+from .inference_session import (BackendSpec, BackendOptions, InferenceSession, ModelRunner,
                                 RunResult, FileDescription)
 from .interceptors.auth import AuthInterceptor, StreamAuthInterceptor
 from .interceptors.cookie import CookieInterceptor, StreamCookieInterceptor
 from .log_util import LOGFILE, get_file_logger
 from .protos import remote_inference_pb2 as pb, remote_inference_pb2_grpc as rpc
 
 BackendSpecType = Union[str, BackendSpec, Sequence[Union[str, BackendSpec,
                                                          pb.BackendSpec]]]
 
 MODEL_FORMAT_ONNX = pb.MODEL_FORMAT_ONNX
 MODEL_FORMAT_FXPROTO = pb.MODEL_FORMAT_FXPROTO
+RUN_MODE = pb.RunMode
 
 
 MAX_GRPC_MESSAGE_SIZE = 1024 * 1024 * 1024   # 1GiB
 
 
 class RemoteModelRunner(ModelRunner):
     def __init__(self,
                  session: 'RemoteInferenceSession',
                  model_id: int,
                  input_map_per_backend: Sequence[pb.InputMap]):
         self._session = weakref.ref(session)
         self._model_id = model_id
         self._input_map_per_backend = input_map_per_backend
 
-    def run(self, inputs, num_repeats=None) -> Mapping[BackendSpec, RunResult]:
+    def submit_run(self, inputs,
+                   *,
+                   num_repeats=None,
+                   num_warmups=None,
+                   mode=None) -> Callable[[], Mapping[BackendSpec, RunResult]]:
         session = self._session()
         input_protos = [numpy_to_proto(x) for x in inputs]
         request = pb.RunRequest(session_uuid=session._session_uuid.bytes,
                                 model_id=self._model_id,
                                 inputs=input_protos,
                                 num_repeats=num_repeats,
-                                input_map_per_backend=self._input_map_per_backend)
-        reply = session._client.stub.Run(request)
-        assert len(reply.result_per_backend) == len(session._backends)
-        return {
-            backend: RunResult.from_pb(result)
-            for backend, result in zip(session._backends, reply.result_per_backend)
-        }
+                                num_warmups=num_warmups,
+                                input_map_per_backend=self._input_map_per_backend,
+                                mode=mode)
+        future = session._client.stub.Run.future(request)
+
+        def get_result_fn():
+            reply = future.result()
+            assert len(reply.result_per_backend) == len(session._backends)
+            return {
+                backend: RunResult.from_pb(result)
+                for backend, result in zip(session._backends, reply.result_per_backend)
+            }
+
+        return get_result_fn
 
 
 def _get_backend_specs(backends: Optional[BackendSpecType] = None)\
         -> Sequence[BackendSpec]:
     if backends is None:
         return []
     if isinstance(backends, str):
@@ -286,15 +299,15 @@
         self._access_token_source = access_token_source
 
     @staticmethod
     def create(server_addr: Optional[str] = None,
                insecure: Optional[bool] = False,
                access_token: Optional[str] = None) -> '_Client':
         # FIXME: shouldn't explicitly given args take priority over env variables?
-        server_addr = os.environ.get("OCTOML_PROFILE_ENDPOINT", None) or server_addr
+        server_addr = server_addr or os.environ.get("OCTOML_PROFILE_ENDPOINT", None)
         if server_addr is None:
             server_addr = "dynamite.prod.aws.octoml.ai"
         if insecure is None:
             insecure = False
 
         access_token, token_src = _get_access_token(access_token, server_addr, insecure)
         return _Client(server_addr, insecure, access_token, token_src)
@@ -340,47 +353,54 @@
                 cookie = item.value
                 self._channel = grpc.intercept_channel(self._channel,
                                                        CookieInterceptor(cookie),
                                                        StreamCookieInterceptor(cookie))
                 self._stub = rpc.RemoteInferenceStub(self._channel)
 
         if reply.WhichOneof('result') == 'error_value':
-            raise ValueError(f"Error starting a remote inference session:"
-                             f" {reply.error_value.message}")
+            raise RuntimeError(f"Error creating a remote inference session. "
+                               f"{reply.error_value.message}")
         return reply.result_value
 
     def wait_until_session_ready(self, session_uuid: UUID):
         print('Waiting for an available remote worker...', file=sys.stderr)
         while True:
             reply = self.stub.WaitUntilSessionReady(
                 pb.WaitUntilSessionReadyRequest(session_uuid=session_uuid.bytes))
 
             if reply.ready:
                 print('Acquired all workers, session is now ready.', file=sys.stderr)
                 break
 
 
 def _backend_spec_from_proto(b: pb.BackendSpec) -> BackendSpec:
-    return BackendSpec(hardware_platform=b.hardware_platform, software_backend=b.software_backend)
+    backend_options = BackendOptions.from_pb(b.backend_options)
+    return BackendSpec(hardware_platform=b.hardware_platform,
+                       software_backend=b.software_backend,
+                       backend_options=backend_options)
 
 
 def _backend_spec_to_proto(b: BackendSpec) -> pb.BackendSpec:
     return pb.BackendSpec(hardware_platform=b.hardware_platform,
-                          software_backend=b.software_backend)
+                          software_backend=b.software_backend,
+                          backend_options=[pb.BackendOption(key=k, value=v)
+                                           for k, v in b.backend_options.items()])
 
 
 def _get_backends(backends: Sequence[BackendSpec], client: _Client):
     # Before creating the session, check that requested backends are valid
     if len(backends) == 0:
         backends = client.get_default_backends()
         backends_str = ', '.join(str(b) for b in backends)
         print(f'No backends were requested, using defaults: {backends_str}', file=sys.stderr)
     else:
         supported_backends = client.get_supported_backends()
-        unsupported = [b for b in backends if b not in supported_backends]
+        unsupported = [b for b in backends
+                       if BackendSpec(b.hardware_platform, b.software_backend)
+                       not in supported_backends]
         if len(unsupported) > 0:
             unsupported_str = ', '.join(str(b) for b in unsupported)
             supported_str = '\n\t'.join(str(b) for b in supported_backends)
             raise ValueError(f'Some of the requested backends ({unsupported_str})'
                              f' are not supported.\n'
                              f'The supported, valid backends are:\n\t{supported_str}')
     return backends
@@ -411,15 +431,14 @@
         if status_code == grpc.StatusCode.UNAVAILABLE:
             status_details = "Connection can't be established between client and server. " \
                              "This could be caused by incorrect ip addresses or port " \
                              "numbers"
         elif status_code == grpc.StatusCode.INTERNAL:
             status_details = "An internal error ocurred, typically due to starting " \
                              "the remote session with wrong configuration(s)"
-
         # use from None to suppress stack trace from rpc_error
         raise CreateSessionError(f"Error {status_code.name}:"
                                  f" {status_details}. See full client-side"
                                  f" trace at {LOGFILE}") from None
 
 
 class RemoteInferenceSession(InferenceSession):
```

### Comparing `octoml_profile-0.2.1/octoml_profile/conversion_util.py` & `octoml_profile-0.2.2rc1/octoml_profile/conversion_util.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.1/octoml_profile/dynamo.py` & `octoml_profile-0.2.2rc1/octoml_profile/dynamo.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,51 +10,62 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import contextlib
 import functools
+import inspect
 import os
 import sys
 import tempfile
 import threading
 import time
 import traceback
 import warnings
 import weakref
-from collections import OrderedDict
-from dataclasses import dataclass, field
+from collections import OrderedDict, defaultdict
+from dataclasses import dataclass
 from typing import (Callable, Dict, Optional, Sequence, TextIO, Tuple, List,
                     Union, Any)
 
 import numpy as np
 import onnx
 import torch
 import torch._dynamo as torchdynamo
 import torch._guards
 import torch.fx
-from torch._dynamo.backends.common import fake_tensor_unsupported
 from torch.jit import TracerWarning
 
-from .client import RemoteInferenceSession, MODEL_FORMAT_ONNX, MODEL_FORMAT_FXPROTO, BackendSpecType
+from .client import (
+    get_supported_backends,
+    BackendSpecType,
+    RemoteInferenceSession,
+    MODEL_FORMAT_ONNX,
+    MODEL_FORMAT_FXPROTO,
+    RUN_MODE)
 from .errors import CompilationError, LoadModelError
 from .fx2proto import SerializedFxProtoModel, fx_graph_to_proto
 from .inference_session import BackendSpec, InferenceSession, ModelRunner, \
     OnDiskFile, FileDescription, LazyInMemoryFile
-from .log_util import LOGFILE, get_file_logger
-from .report import (PerBackendResult, Profile, ProfileReport, Segment,
+from .log_util import LOGFILE, LOGDIR, get_file_logger
+from .report import (GraphResult, PerBackendResult, Profile, ProfileReport, Segment,
                      TotalPerBackendResult, PerBackendError)
 from .shape import get_dynamic_axes
 from .workaround import (_in_torch_dynamo,
-                         _onnx_export_diagnostic_patch)
+                         _onnx_export_diagnostic_patch,
+                         fake_tensor_unsupported)
 
 filelog = get_file_logger(__name__)
 
 
+RAISE_ON_COMPILATION_ERROR = False
+RAISE_ON_RUNTIME_ERROR = False
+
+
 @dataclass
 class _OnnxModel:
     path: str
     active_input_names: Sequence[str]
     active_input_mask: Sequence[bool]
 
     def get_file_descriptions(self) -> Sequence[FileDescription]:
@@ -100,23 +111,17 @@
 
 @dataclass
 class _Context:
     session: weakref.ReferenceType
     trace_recorder: '_TraceRecorder'
     last_graph_id: int
     num_repeats: int
-    num_runs: int = field(default=0)
-
-    def start_run(self):
-        self.num_runs += 1
-        if self.num_runs == 1:
-            print("Accelerated function is being compiled on its first run:",
-                  file=sys.stderr)
-        else:
-            print(f"Running function, iteration {self.num_runs}", file=sys.stderr)
+    num_warmups: int
+    run_mode: RUN_MODE
+    ctx_id: int = 0
 
     def new_graph_id(self) -> int:
         self.last_graph_id += 1
         return self.last_graph_id
 
     def dec_graph_id(self):
         self.last_graph_id -= 1
@@ -167,40 +172,58 @@
                 if err not in agg.unique_errors_to_count:
                     agg.unique_errors_to_count[err] = 0
                 agg.unique_errors_to_count[err] += err_count
 
 
 @dataclass
 class _AggregatedResult:
+    func_name: str
     sums: Sequence[Union[_LocalCpuSegment, _CompiledSegment]]
     num_runs: int
     compilation_occurred: bool
+    compilation_errors: Sequence[str]
+    num_disgarded_runs: int = 0
 
-    def add(self, sample: Sequence[Union[_LocalCpuSegment, _CompiledSegment]]):
-        assert self.compilation_occurred is False, \
-            "Should not aggregate to result that has compilation occurred"
+    def add(self,
+            sample: Sequence[Union[_LocalCpuSegment, _CompiledSegment]],
+            compilation_occurred: bool):
         assert len(self.sums) == len(sample)
-        for agg, new in zip(self.sums, sample):
-            agg.add(new)
-        self.num_runs += 1
+        # Cases when adding two aggs:
+        # - no-compile + no-compile: merge
+        # - compile + compile: merge
+        # - compile + no-compile: replace compile with no compile, disgard compile
+        # - no-compile + compile: ignore and disgard
+        if self.compilation_occurred and not compilation_occurred:
+            self.compilation_occurred = False
+            self.num_disgarded_runs = self.num_runs
+            self.num_runs = 1
+            self.sums = [s for s in sample]
+        elif not self.compilation_occurred and compilation_occurred:
+            self.num_disgarded_runs += 1
+        else:
+            for agg, new in zip(self.sums, sample):
+                agg.add(new)
+            self.num_runs += 1
 
     def report(self, num_repeats):
         segments = []
         total_uncompiled_ms = 0.0
         total_per_backend = OrderedDict()
+        graph_results = []
         for segment_idx, segment in enumerate(self.sums):
             if isinstance(segment, _LocalCpuSegment):
                 mean_ms = segment.run_time_nanos / 1.0e6 / self.num_runs
                 total_uncompiled_ms += mean_ms
                 r = PerBackendResult(mean_ms=mean_ms,
                                      num_samples=self.num_runs,
                                      num_failures=0)
                 segments.append(Segment(graph_id=None,
                                         results_per_backend=OrderedDict(Uncompiled=r)))
             elif isinstance(segment, _CompiledSegment):
+                graph_id = segment.graph.graph_id
                 results_per_backend = OrderedDict()
                 for backend, run_times in segment.run_times_per_backend.items():
                     backend_str = str(backend)
                     if backend_str not in total_per_backend:
                         total_per_backend[backend_str] = TotalPerBackendResult(
                                 estimated_total_ms=0.0,
                                 errors=[])
@@ -213,46 +236,55 @@
                     else:
                         mean_ms = None
                         backend_total.estimated_total_ms = None
 
                     err = segment.errors_per_backend[backend]
                     if err.count > 0:
                         total_per_backend[backend_str].errors.append(PerBackendError(
-                                graph_id=segment.graph.graph_id,
+                                graph_id=graph_id,
                                 error_messages_to_count=err.unique_errors_to_count))
                     results_per_backend[backend_str] = PerBackendResult(
                             mean_ms=mean_ms,
                             num_samples=len(run_times),
                             num_failures=err.count)
 
-                segments.append(Segment(graph_id=segment.graph.graph_id,
+                segments.append(Segment(graph_id=graph_id,
                                         results_per_backend=results_per_backend))
+                mod = segment.graph.graph_module
+                graph_results.append(GraphResult(graph_id, mod,
+                                                 mod.compile_subgraph_reason))
             else:
                 assert False
 
         for backend_total in total_per_backend.values():
             if backend_total.estimated_total_ms is not None:
                 backend_total.estimated_total_ms += total_uncompiled_ms
 
-        return Profile(segments=segments,
+        return Profile(func_name=self.func_name,
+                       segments=segments,
                        total_uncompiled_ms=total_uncompiled_ms,
                        total_per_backend=total_per_backend,
                        compilation_occurred=self.compilation_occurred,
+                       compilation_errors=self.compilation_errors,
                        num_runs=self.num_runs,
-                       num_repeats=num_repeats)
+                       num_repeats=num_repeats,
+                       graph_results=graph_results,
+                       num_disgarded_runs=self.num_disgarded_runs)
 
 
 class _TraceRecorder:
     def __init__(self):
         self._start_nanos = None
         self._segments = []
         self._result_by_footprint = OrderedDict()
         self._compilation_occurred = False
-        self._num_discarded_runs = 0
-        self._compile_errors = []
+        self._compilation_errors = []
+        self._func_name = ""
+        self._num_runs = defaultdict(int)
+        self._dynamo_error_occurred = False
 
     def start_cpu(self):
         start = time.perf_counter_ns()
         assert self._start_nanos is None
         self._start_nanos = start
 
     def stop_cpu(self):
@@ -270,60 +302,74 @@
         self._segments.append(_LocalCpuSegment(end_nanos - self._start_nanos))
         self._start_nanos = None
         try:
             yield
         finally:
             self.start_cpu()
 
+    @property
+    def func_name(self):
+        return self._func_name
+
+    def begin_run(self, func_name):
+        self._func_name = func_name
+        self._num_runs[func_name] += 1
+        print(f'Running function `{func_name}` iteration {self._num_runs[func_name]}')
+
     def add_compiled_segment(self, segment: _CompiledSegment):
         assert self._start_nanos is None
         self._segments.append(segment)
 
     def compilation_occurred(self):
         self._compilation_occurred = True
 
+    def dynamo_error_occurred(self):
+        self._dynamo_error_occurred = True
+
     def add_compile_error(self, error: str):
-        self._compile_errors.append(error)
+        self._compilation_errors.append(error)
 
     def end_run(self):
         run_footprint = tuple(s.footprint() for s in self._segments)
         agg_result = self._result_by_footprint.get(run_footprint, None)
-        if self._compilation_occurred:
-            assert agg_result is None
+        if agg_result is None:
             self._result_by_footprint[run_footprint] = \
-                _AggregatedResult(tuple(self._segments), 1, True)
-        elif agg_result is not None:
-            if agg_result.compilation_occurred:
-                self._result_by_footprint[run_footprint] = \
-                    _AggregatedResult(tuple(self._segments), 1, False)
-            else:
-                agg_result.add(self._segments)
+                _AggregatedResult(self.func_name,
+                                  tuple(self._segments),
+                                  num_runs=1,
+                                  compilation_occurred=self._compilation_occurred,
+                                  compilation_errors=self._compilation_errors,
+                                  num_disgarded_runs=0)
         else:
-            # got here with compilation_occurred False
-            # and no agg_result means torchdynamo failed
-            pass
+            agg_result.add(self._segments, self._compilation_occurred)
 
         if self._compilation_occurred:
             self._compilation_occurred = False
-            self._num_discarded_runs += 1
         self._segments.clear()
 
-    def report(self, num_repeats):
+    def report(self, num_repeats, report_dir: str):
         profiles = [r.report(num_repeats)
                     for r in self._result_by_footprint.values()]
         return ProfileReport(profiles=profiles,
-                             num_discarded_runs=self._num_discarded_runs,
-                             compile_errors=self._compile_errors)
+                             compilation_errors=self._compilation_errors,
+                             report_dir=report_dir)
 
-    def print_results(self, num_repeats: int, file=sys.stdout):
-        self.report(num_repeats).print(file=file)
+    def print_results(self, num_repeats: int, report_dir: str, file=sys.stdout):
+        if self._dynamo_error_occurred:
+            print(f'ERROR: Encountered TorchDynamoError:\n'
+                  f'  Please file an issue at https://github.com/octoml/octoml-profile/issues\n'
+                  f'  or set torch._dynamo.config.suppress_errors = True to ignore this error.',
+                  file=sys.stderr)
+        else:
+            self.report(num_repeats, report_dir).print(file=file)
 
 
 class _ThreadLocalState(threading.local):
     profiling_ctx: _Context = None
+    next_profiling_ctx_id: int = 0
 
 
 _thread_local_state = _ThreadLocalState()
 
 
 def _run(runner: ModelRunner, graph_info: _GraphInfo, active_input_mask: Sequence[bool],
          *inputs: torch.Tensor):
@@ -332,46 +378,76 @@
         # for verifying correctness. This adds user overhead and also has side
         # effects to recorder. We can just pretend to run eager because remote
         # run with benchmark side effect is strongly undesirable. The flip side
         # is that `verify_correctness` is not repsected, which we do not care.
         return graph_info.graph_module(*inputs)
 
     ctx = _thread_local_state.profiling_ctx
+    if ctx.run_mode == RUN_MODE.PROFILING:
+        return _run_profile(runner, graph_info, active_input_mask, *inputs)
+    else:
+        return _run_inference(runner, graph_info, active_input_mask, *inputs)
+
+
+def _run_profile(runner: ModelRunner, graph_info: _GraphInfo, active_input_mask: Sequence[bool],
+                 *inputs: torch.Tensor):
+    ctx = _thread_local_state.profiling_ctx
     recorder = ctx.trace_recorder
     with recorder.pause_cpu():
         assert len(inputs) == len(active_input_mask), "invalid number of inputs for runner"
-        inputs = tuple(x if isinstance(x, torch.Tensor) else torch.tensor(x) for x in inputs)
-        numpy_inputs = (x.data.cpu().numpy() for x, is_active in zip(inputs, active_input_mask)
-                        if is_active)
-        num_repeats = ctx.num_repeats
-
-        if ctx.num_runs == 1 and ctx.last_graph_id == graph_info.graph_id:
-            print(f"\tCompiling and running graph {graph_info.graph_id} on remote...",
-                  file=sys.stderr)
-        result_by_backend = runner.run(numpy_inputs, num_repeats=num_repeats)
+        input_tensors = tuple(x if isinstance(x, torch.Tensor) else torch.tensor(x) for x in inputs)
+        numpy_inputs = (x.data.cpu().numpy()
+                        for x, is_active in zip(input_tensors, active_input_mask) if is_active)
+
+        get_result = runner.submit_run(numpy_inputs,
+                                       num_repeats=ctx.num_repeats,
+                                       num_warmups=ctx.num_warmups,
+                                       mode=RUN_MODE.PROFILING)
+        local_outputs = graph_info.graph_module(*inputs)
+        result_by_backend = get_result()
         errors_per_backend = {}
         run_times_per_backend = {}
         for backend, r in result_by_backend.items():
             if r.error_value is None:
                 err = _BackendErrors(0, {})
             else:
-                err = _BackendErrors(num_repeats, {r.error_value.message: num_repeats})
+                err = _BackendErrors(ctx.num_repeats,
+                                     {r.error_value.message: ctx.num_repeats})
                 log = get_file_logger(__name__)
                 log.error("Error in run graph %d for backend %s: %s",
                           graph_info.graph_id, backend, r.error_value.message)
             errors_per_backend[backend] = err
-
             run_times_per_backend[backend] = \
                 r.result_value.run_times_nanos if r.result_value is not None else []
         recorder.add_compiled_segment(_CompiledSegment(
             graph=graph_info,
             run_times_per_backend=run_times_per_backend,
             errors_per_backend=errors_per_backend
         ))
-        return graph_info.graph_module(*inputs)
+        if any(x.count for x in errors_per_backend.values()) and RAISE_ON_RUNTIME_ERROR:
+            raise RuntimeError(f"Error running graph #{graph_info.graph_id}:\n{errors_per_backend}")
+
+        return local_outputs
+
+
+def _run_inference(runner: ModelRunner, graph_info: _GraphInfo, active_input_mask: Sequence[bool],
+                   *inputs: torch.Tensor):
+    assert len(inputs) == len(active_input_mask), "invalid number of inputs for runner"
+    assert all(active_input_mask), "all inputs should be active for inference mode"
+    inputs = tuple(x if isinstance(x, torch.Tensor) else torch.tensor(x) for x in inputs)
+    get_result = runner.submit_run((x.data.cpu().numpy() for x in inputs),
+                                   num_repeats=1, num_warmups=0,
+                                   mode=RUN_MODE.INFERENCE)
+    result_by_backend = get_result()
+    assert len(result_by_backend) == 1
+    result = next(iter(result_by_backend.values()))
+    if result.result_value is None:
+        raise RuntimeError(f"Error running graph #{graph_info.graph_id}: {result.error_value}")
+    else:
+        return tuple(torch.tensor(o) for o in result.result_value.outputs)
 
 
 # Follows torch/_dynamo/backends/onnxrt.py to disable fake tensor
 def _safe_dynamo_backend(_compile_func: Callable, gm: torch.fx.GraphModule,
                          example_inputs: Tuple[torch.Tensor, ...]):
     try:
         return _compile_func(gm, example_inputs)
@@ -391,14 +467,16 @@
             graph_id = ctx.last_graph_id
             error = f"Graph #{graph_id} ran locally because "
             message = error + message
             ctx.trace_recorder.add_compile_error(message)
         trace = traceback.format_exc()
         graph_dump = f"Graph #{graph_id} dump:\n{gm.print_readable(print_output=False)}"
         filelog.error("%s\n%s\n%s", message, graph_dump, trace)
+        if RAISE_ON_COMPILATION_ERROR:
+            raise
     return gm.forward
 
 
 @dataclass
 class _LoadedModelInfo:
     active_input_mask: Sequence[bool]
 
@@ -546,62 +624,69 @@
 
         if gm.training:
             gm.eval()
 
         graph_info = _GraphInfo(graph_id=_thread_local_state.profiling_ctx.new_graph_id(),
                                 num_nodes=len(gm.graph.nodes),
                                 graph_module=gm)
-
         graph_outputs = _get_graph_outputs(gm)
+
         if _is_empty_output(graph_outputs):
             _thread_local_state.profiling_ctx.dec_graph_id()
             return gm.forward
 
+        print(f"\tCompiling and running graph {graph_info.graph_id} on remote...",
+              file=sys.stderr)
+
         session = _thread_local_state.profiling_ctx.session()
         loaded_infos = []
         for loader, backend_indices in _group_backends_by_loader(session.backends):
             loaded_info = loader(session, graph_info.graph_id, backend_indices, gm, example_inputs)
             loaded_infos.append((loaded_info, backend_indices))
 
         active_input_mask = _get_overall_active_input_mask(loaded_infos, len(example_inputs))
         input_maps = _get_input_maps_per_backend(loaded_infos, active_input_mask,
                                                  len(session.backends))
 
         runner = session.create_runner(graph_info.graph_id, input_maps)
-        ret = functools.partial(_run, runner, graph_info, active_input_mask)
-        return ret
+        return functools.partial(_run, runner, graph_info, active_input_mask)
 
 
 class ProfileHandle:
     def __init__(self, ctx: _Context):
         self._ctx = ctx
 
     def report(self) -> ProfileReport:
-        return self._ctx.trace_recorder.report(self._ctx.num_repeats)
+        report_dir = f'{LOGDIR}/{self._ctx.ctx_id}'
+        return self._ctx.trace_recorder.report(self._ctx.num_repeats, report_dir)
 
 
 def _set_profiling_ctx(ctx: Optional[_Context]):
     _thread_local_state.profiling_ctx = ctx
+    if ctx is not None:
+        _thread_local_state.next_profiling_ctx_id += 1
 
 
 def _print_results_if_requested(ctx: _Context, file: Optional[TextIO]):
     if file is not None:
-        ctx.trace_recorder.print_results(ctx.num_repeats, file=file)
+        report_dir = f'{LOGDIR}/{ctx.ctx_id}'
+        ctx.trace_recorder.print_results(ctx.num_repeats, report_dir, file=file)
 
 
 @contextlib.contextmanager
 def remote_profile(session: Optional[InferenceSession] = None,
                    *,
                    # Session parameters:
                    backends: Optional[BackendSpecType] = None,
                    server_addr: Optional[str] = None,
                    insecure: Optional[bool] = None,
                    access_token: Optional[str] = None,
                    # Profiling options:
                    num_repeats: int = 10,
+                   num_warmups: int = 1,
                    print_results_to: Optional[TextIO] = sys.stdout) -> ProfileHandle:
     if _thread_local_state.profiling_ctx is not None:
         raise RuntimeError("Nested remote_profile() contexts are not allowed")
 
     with contextlib.ExitStack() as guard:
         if session is not None:
             for session_arg in ["backends", "access_token", "server_addr", "insecure"]:
@@ -614,15 +699,19 @@
             session = RemoteInferenceSession(backends=backends,
                                              server_addr=server_addr,
                                              insecure=insecure,
                                              access_token=access_token)
             guard.enter_context(session)
 
         ctx = _Context(session=weakref.ref(session), trace_recorder=_TraceRecorder(),
-                       last_graph_id=0, num_repeats=num_repeats)
+                       last_graph_id=0,
+                       num_repeats=num_repeats,
+                       num_warmups=num_warmups,
+                       run_mode=RUN_MODE.PROFILING,
+                       ctx_id=_thread_local_state.next_profiling_ctx_id)
         try:
             _set_profiling_ctx(ctx)
             guard.enter_context(torch.no_grad())
             guard.enter_context(_onnx_export_diagnostic_patch())
             guard.callback(_set_profiling_ctx, None)
             guard.callback(_print_results_if_requested, ctx, print_results_to)
 
@@ -632,17 +721,77 @@
             yield ProfileHandle(ctx)
         finally:
             # Remove from frame so that the traceback doesn't hold a strong reference to the session
             del session
 
 
 @contextlib.contextmanager
-def _profile_run():
+def remote_inference(session: Optional[InferenceSession] = None,
+                     *,
+                     # Session parameters:
+                     backend: Optional[Union[str, BackendSpec]] = None,
+                     server_addr: Optional[str] = None,
+                     insecure: Optional[bool] = None,
+                     access_token: Optional[str] = None):
+
+    if _thread_local_state.profiling_ctx is not None:
+        raise RuntimeError("Nested remote_inference() contexts are not allowed")
+
+    with contextlib.ExitStack() as guard:
+        if session is not None:
+            for session_arg in ["backend", "access_token", "server_addr", "insecure"]:
+                if locals()[session_arg] is None:
+                    continue
+                raise ValueError(f"`session` cannot be set at the same time as `{session_arg}`."
+                                 f" Please either specify an already existing session or"
+                                 f" parameters for a new session, but not both at the same time.")
+
+            if isinstance(session, RemoteInferenceSession):
+                if len(session.backends) > 1:
+                    raise ValueError(f"remote_inference `session` can only have 1 "
+                                     f"backend, got {session.backends}.")
+        else:
+            if backend is None:
+                supported_backends = get_supported_backends(server_addr, insecure, access_token)
+                raise RuntimeError(f"`backend` must be specified for remote_inference. "
+                                   f"Available backends are: {supported_backends}.")
+            elif not isinstance(backend, (str, BackendSpec)):
+                raise TypeError(f"`backend` must be type str or BackendSpec, got {type(backend)}.")
+
+            session = RemoteInferenceSession(backends=(backend,),
+                                             server_addr=server_addr,
+                                             insecure=insecure,
+                                             access_token=access_token)
+            guard.enter_context(session)
+
+        ctx = _Context(session=weakref.ref(session), trace_recorder=_TraceRecorder(),
+                       last_graph_id=0,
+                       num_repeats=1,
+                       num_warmups=0,
+                       run_mode=RUN_MODE.INFERENCE,
+                       ctx_id=_thread_local_state.next_profiling_ctx_id)
+        try:
+            _set_profiling_ctx(ctx)
+            guard.enter_context(torch.no_grad())
+            guard.enter_context(_onnx_export_diagnostic_patch())
+            guard.callback(_set_profiling_ctx, None)
+
+            # Invalidated dynamo cache because session has changed
+            torchdynamo.reset()
+
+            yield
+        finally:
+            # Remove from frame so that the traceback doesn't hold a strong reference to the session
+            del session
+
+
+@contextlib.contextmanager
+def _profile_run(func_name):
     recorder = _thread_local_state.profiling_ctx.trace_recorder
-    _thread_local_state.profiling_ctx.start_run()
+    recorder.begin_run(func_name)
     recorder.start_cpu()
     try:
         yield
     finally:
         recorder.stop_cpu()
         recorder.end_run()
 
@@ -700,47 +849,73 @@
     dynamic = kwargs.get('dynamic', False)
     # TODO(yuanjing): don't fall back to eager once inductor's coverage is decent
     if local_backend == "inductor":
         # For some strange reason, importing inductor can mess up CUDA state, so import it lazily
         from torch._inductor.compile_fx import compile_fx
         local_backend = functools.partial(_safe_dynamo_backend, compile_fx)
     regular_dynamo_decorator = torchdynamo.optimize(local_backend, dynamic=dynamic)
-    profiling_dynamo_decorator = torchdynamo.optimize(_remote_backend, dynamic=dynamic)
+    remote_dynamo_decorator = torchdynamo.optimize(_remote_backend, dynamic=dynamic)
+
+    # https://stackoverflow.com/questions/3589311/get-defining-class-of-unbound-method-object-in-python-3/25959545#25959545
+    def _get_class_that_defined_method(meth):
+        if isinstance(meth, functools.partial):
+            return _get_class_that_defined_method(meth.func)
+        if (inspect.ismethod(meth)
+                or (inspect.isbuiltin(meth)
+                    and getattr(meth, '__self__', None)
+                    and getattr(meth.__self__, '__class__', None))):
+            for cls in inspect.getmro(meth.__self__.__class__):
+                if meth.__name__ in cls.__dict__:
+                    return cls
+            meth = getattr(meth, '__func__', meth)  # fallback to __qualname__ parsing
+        if inspect.isfunction(meth):
+            cls = getattr(inspect.getmodule(meth),
+                          meth.__qualname__.split('.<locals>', 1)[0].rsplit('.', 1)[0],
+                          None)
+            if isinstance(cls, type):
+                return cls
+        return getattr(meth, '__objclass__', None)  # handle special descriptor objectsc
+
+    def _get_func_name(func):
+        cls = _get_class_that_defined_method(func)
+        if cls is not None:
+            return f'{cls.__name__}.{func.__name__}'
+        else:
+            return func.__name__
 
     def decorate(func):
         if isinstance(func, torch.nn.Module):
             decorated_forward = decorate(func.forward)
             return _AcceleratedModule(func, decorated_forward)
         regular_dynamo_decorated = regular_dynamo_decorator(func)
-        profiling_dynamo_decorated = profiling_dynamo_decorator(func)
+        remote_dynamo_decorated = remote_dynamo_decorator(func)
 
         @functools.wraps(regular_dynamo_decorated)
         def decorated_func(*args, **kwargs):
             exception = None
             try:
                 if _thread_local_state.profiling_ctx is None:
                     return regular_dynamo_decorated(*args, **kwargs)
-                with _profile_run():
-                    return profiling_dynamo_decorated(*args, **kwargs)
+                elif _thread_local_state.profiling_ctx.run_mode == RUN_MODE.PROFILING:
+                    with _profile_run(_get_func_name(func)):
+                        return remote_dynamo_decorated(*args, **kwargs)
+                else:
+                    return remote_dynamo_decorated(*args, **kwargs)
             except torchdynamo.exc.TorchDynamoException as e:
                 exception = type(e).__name__.split(".")[-1]
                 trace = traceback.format_exc()
             except Exception as e:
                 exception = type(e).__name__
                 trace = traceback.format_exc()
 
+            # Unrecoverable Dynamo Error
             if exception:
-                action = "The error above may be caused by user code error in "\
-                         "the decorated function "\
-                         "or a bug in TorchDynamo. In the former case, please "\
-                         "check the trace for user code error; "\
-                         "in the latter case, please "\
-                         "try refining the scope of @accelerate closer to "\
-                         "model inference."
-                filelog.error("%s\n%s", trace, action)
+                if _thread_local_state.profiling_ctx is not None:
+                    _thread_local_state.profiling_ctx.trace_recorder.dynamo_error_occurred()
+                filelog.error("%s", trace)
                 raise CompilationError(exception, {'details': LOGFILE})
 
         return decorated_func
 
     if direct_application:
         return decorate(args[0])
     else:
```

### Comparing `octoml_profile-0.2.1/octoml_profile/errors.py` & `octoml_profile-0.2.2rc1/octoml_profile/errors.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.1/octoml_profile/fx2proto.py` & `octoml_profile-0.2.2rc1/octoml_profile/fx2proto.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,15 +213,19 @@
         if n.op == 'call_function' and n.target is torch.ops.aten.lift_fresh_copy.default:
             if len(n.args) != 1 or not _is_constant_arg(n.args[0]) or len(n.kwargs) > 0:
                 log.warning("Graph has a call to %s with a non-constant argument", n.target)
                 continue
             c = getattr(gm, n.args[0].target)
             data = c.data.cpu().numpy().tolist()
             with gm.graph.inserting_after(n):
-                new_node = gm.graph.call_function(torch.tensor, (data,), dict(dtype=c.dtype))
+                new_node = gm.graph.call_function(
+                    torch.tensor,
+                    (data,),
+                    dict(dtype=c.dtype, device=c.device),
+                )
             n.replace_all_uses_with(new_node)
             gm.graph.erase_node(n)
 
     # Remove all getattr nodes that are now unused
     gm.graph.eliminate_dead_code()
 
     gm.recompile()
```

### Comparing `octoml_profile-0.2.1/octoml_profile/inference_session.py` & `octoml_profile-0.2.2rc1/octoml_profile/inference_session.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,39 +11,98 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import functools
 import hashlib
 import os
 from contextlib import contextmanager
-from dataclasses import dataclass
-from typing import Sequence, Mapping, NamedTuple, Tuple, Callable, Iterator, Union
+from dataclasses import dataclass, field
+from typing import Sequence, Mapping, Tuple, Callable, Iterator, Optional, Union
+from collections import OrderedDict
 
 import numpy as np
 
 from .conversion_util import proto_to_numpy
 from .protos import remote_inference_pb2 as pb
 
 
-class BackendSpec(NamedTuple):
+class BackendOptions(OrderedDict):
+
+    @staticmethod
+    def parse(spec: str) -> 'BackendOptions':
+        """
+        Args:
+            spec: option string "k1,k2=v2,..."
+
+        `spec` is comma separated. Each token is either a `k` (key) or a `k=v` (key, value) pairs.
+        """
+        opts = BackendOptions()
+        for token in spec.split(","):
+            key_value = token.split("=")
+            if len(key_value) == 1:
+                key, value = key_value[0], ""
+            elif len(key_value) == 2:
+                key, value = key_value
+            else:
+                raise ValueError(f"Malformed backend option: {spec}. Backend options"
+                                 f" have the form of \"k1,k2=v2,k3=v3\".")
+            opts[key.strip()] = value.strip()
+        return opts
+
+    @staticmethod
+    def from_pb(options: Sequence[pb.BackendOption]) -> "BackendOptions":
+        opts = BackendOptions()
+        for kv in options:
+            opts[kv.key] = kv.value
+        return opts
+
+    def __str__(self):
+        if len(self) == 0:
+            return ""
+        else:
+            return "[" + ",".join(f"{k}={v}" if v != "" else k for k, v in self.items()) + "]"
+
+    def __repr__(self):
+        return str(self)
+
+    def __hash__(self):
+        return hash(str(sorted(self.items())))
+
+    def __eq__(self, other):
+        return dict(self) == dict(other)
+
+
+@dataclass(eq=True, frozen=True)
+class BackendSpec:
     hardware_platform: str
     software_backend: str
+    backend_options: BackendOptions = field(default_factory=BackendOptions)
 
     @staticmethod
     def parse(spec: str) -> 'BackendSpec':
         hw_and_sw = spec.split('/', maxsplit=1)
         if len(hw_and_sw) != 2:
             raise ValueError('Backend spec string must contain a hardware platform name'
                              ' and a software backend name, separated by a slash,'
                              ' e.g. "aws-v100/onnxrt-cuda"')
         hardware_platform, software_backend = hw_and_sw
-        return BackendSpec(hardware_platform, software_backend)
+        if software_backend.endswith("]"):
+            option_begin = software_backend.find("[")
+            if option_begin < 0:
+                raise ValueError('Backend options must be included in [],'
+                                 ' e.g. "g5.xlarge/torch-eager-cuda[fp16]')
+            option_spec = software_backend[option_begin + 1: -1]
+            software_backend = software_backend[:option_begin]
+            backend_options = BackendOptions.parse(option_spec)
+        else:
+            backend_options = BackendOptions()
+        return BackendSpec(hardware_platform, software_backend, backend_options)
 
     def __str__(self):
-        return f"{self.hardware_platform}/{self.software_backend}"
+        return f"{self.hardware_platform}/{self.software_backend}{self.backend_options}"
 
     def __repr__(self):
         return str(self)
 
     def __format__(self, format_spec):
         return format(str(self), format_spec)
 
@@ -52,16 +111,16 @@
 class ResultValue:
     outputs: Tuple[np.ndarray, ...]
     run_times_nanos: np.ndarray  # 1D array of int64
 
 
 @dataclass
 class RunResult:
-    result_value: ResultValue
-    error_value: str
+    result_value: Optional[ResultValue]
+    error_value: Optional[str]
 
     @staticmethod
     def from_pb(result: pb.RunResult) -> "RunResult":
         result_value, error_value = None, None
         if result.HasField("result_value"):
             result_value = ResultValue(
                 outputs=tuple(proto_to_numpy(x) for x in result.result_value.outputs),
@@ -69,15 +128,18 @@
             )
         else:
             error_value = result.error_value
         return RunResult(result_value, error_value)
 
 
 class ModelRunner:
-    def run(self, inputs, num_repeats=None) -> Mapping[BackendSpec, RunResult]:
+    def submit_run(self, inputs,
+                   num_repeats=None,
+                   num_warmups=None,
+                   mode=None) -> Callable[[], Mapping[BackendSpec, RunResult]]:
         raise NotImplementedError
 
 
 BytesLike = Union[bytes, bytearray, memoryview]
 
 
 class FileDescription:
```

### Comparing `octoml_profile-0.2.1/octoml_profile/interceptors/__init__.py` & `octoml_profile-0.2.2rc1/octoml_profile/interceptors/__init__.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.1/octoml_profile/interceptors/auth.py` & `octoml_profile-0.2.2rc1/octoml_profile/interceptors/auth.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.1/octoml_profile/interceptors/base.py` & `octoml_profile-0.2.2rc1/octoml_profile/interceptors/base.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.1/octoml_profile/interceptors/cookie.py` & `octoml_profile-0.2.2rc1/octoml_profile/interceptors/cookie.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.1/octoml_profile/log_util.py` & `octoml_profile-0.2.2rc1/octoml_profile/log_util.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
-from datetime import datetime
+import tempfile
 
-LOGFILE = f'/tmp/octoml-profile-{datetime.now().strftime("%Y-%m-%d-%H:%M:%S")}.log'
+LOGDIR = tempfile.mkdtemp(prefix='octoml_profile_')
+LOGFILE = LOGDIR + "/" + "client.log"
 
 
 def get_file_logger(name, filename=LOGFILE):
     fh = logging.FileHandler(filename)
     fh.setLevel(logging.DEBUG)
     fh.setFormatter(logging.Formatter('%(asctime)s %(levelname)s %(name)s %(message)s'))
     # Manually configure logging instead of invoking logging.basicConfig
```

### Comparing `octoml_profile-0.2.1/octoml_profile/patches/__init__.py` & `octoml_profile-0.2.2rc1/octoml_profile/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.1/octoml_profile/patches/build_map_unpack.py` & `octoml_profile-0.2.2rc1/octoml_profile/patches/build_map_unpack.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.1/octoml_profile/patches/diffusers_output_type.py` & `octoml_profile-0.2.2rc1/octoml_profile/patches/diffusers_output_type.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.1/octoml_profile/patches/dyn_shape_call_neg.py` & `octoml_profile-0.2.2rc1/octoml_profile/patches/dyn_shape_call_neg.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.1/octoml_profile/patches/iadd_tuple_tuple.py` & `octoml_profile-0.2.2rc1/octoml_profile/patches/iadd_tuple_tuple.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.1/octoml_profile/pricing.py` & `octoml_profile-0.2.2rc1/octoml_profile/pricing.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.1/octoml_profile/protos/fxgraph_pb2.py` & `octoml_profile-0.2.2rc1/octoml_profile/protos/fxgraph_pb2.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.1/octoml_profile/protos/inference_base_pb2.py` & `octoml_profile-0.2.2rc1/octoml_profile/protos/inference_base_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,22 +11,24 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*octoml_profile/protos/inference_base.proto\x12\x0eoctoml_profile\"\r\n\x0bPingRequest\"\x0b\n\tPingReply\"B\n\x0b\x42\x61\x63kendSpec\x12\x19\n\x11hardware_platform\x18\x01 \x02(\t\x12\x18\n\x10software_backend\x18\x02 \x02(\t\"[\n\x14\x43reateSessionRequest\x12\x14\n\x0csession_uuid\x18\x01 \x01(\x0c\x12-\n\x08\x62\x61\x63kends\x18\x02 \x03(\x0b\x32\x1b.octoml_profile.BackendSpec\"?\n\x18\x43reateSessionResultValue\x12\x14\n\x0csession_uuid\x18\x01 \x02(\x0c\x12\r\n\x05ready\x18\x02 \x02(\x08\"\x93\x01\n\x12\x43reateSessionReply\x12@\n\x0cresult_value\x18\x01 \x01(\x0b\x32(.octoml_profile.CreateSessionResultValueH\x00\x12\x31\n\x0b\x65rror_value\x18\x02 \x01(\x0b\x32\x1a.octoml_profile.ErrorValueH\x00\x42\x08\n\x06result\"4\n\x1cWaitUntilSessionReadyRequest\x12\x14\n\x0csession_uuid\x18\x01 \x02(\x0c\"+\n\x1aWaitUntilSessionReadyReply\x12\r\n\x05ready\x18\x01 \x02(\x08\"(\n\x10HeartbeatRequest\x12\x14\n\x0csession_uuid\x18\x01 \x02(\x0c\"\x10\n\x0eHeartbeatReply\"+\n\x13\x43loseSessionRequest\x12\x14\n\x0csession_uuid\x18\x01 \x02(\x0c\"\x13\n\x11\x43loseSessionReply\"\xa2\x01\n\x19LoadModelComponentRequest\x12\x14\n\x0csession_uuid\x18\x01 \x01(\x0c\x12\x10\n\x08model_id\x18\x02 \x01(\x04\x12\x1a\n\x12model_component_id\x18\x03 \x01(\x04\x12\x10\n\x08\x66ilename\x18\x04 \x01(\t\x12 \n\x18\x62\x61\x63kends_to_skip_bitmask\x18\x06 \x01(\x0c\x12\r\n\x05\x63hunk\x18\x05 \x02(\x0c\"\x1f\n\x1dLoadModelComponentResultValue\"\x1b\n\x19LoadModelComponentSkipped\"\xdc\x01\n\x18LoadModelComponentResult\x12\x45\n\x0cresult_value\x18\x01 \x01(\x0b\x32-.octoml_profile.LoadModelComponentResultValueH\x00\x12\x31\n\x0b\x65rror_value\x18\x02 \x01(\x0b\x32\x1a.octoml_profile.ErrorValueH\x00\x12<\n\x07skipped\x18\x03 \x01(\x0b\x32).octoml_profile.LoadModelComponentSkippedH\x00\x42\x08\n\x06result\"_\n\x17LoadModelComponentReply\x12\x44\n\x12result_per_backend\x18\x01 \x03(\x0b\x32(.octoml_profile.LoadModelComponentResult\"\xae\x01\n\x1fLoadCachedModelComponentRequest\x12\x14\n\x0csession_uuid\x18\x01 \x02(\x0c\x12\x10\n\x08model_id\x18\x02 \x02(\x04\x12\x1a\n\x12model_component_id\x18\x03 \x02(\x04\x12\x13\n\x0bsha256_hash\x18\x04 \x02(\x0c\x12\x10\n\x08\x66ilename\x18\x05 \x02(\t\x12 \n\x18\x62\x61\x63kends_to_skip_bitmask\x18\x06 \x01(\x0c\"e\n\x1dLoadCachedModelComponentReply\x12\x44\n\x12result_per_backend\x18\x01 \x03(\x0b\x32(.octoml_profile.LoadModelComponentResult\"\xba\x01\n\x10LoadModelRequest\x12\x14\n\x0csession_uuid\x18\x01 \x02(\x0c\x12\x10\n\x08model_id\x18\x02 \x02(\x04\x12\x31\n\x0cmodel_format\x18\x03 \x02(\x0e\x32\x1b.octoml_profile.ModelFormat\x12\x13\n\x0binput_names\x18\x04 \x03(\t\x12\x14\n\x0coutput_names\x18\x05 \x03(\t\x12 \n\x18\x62\x61\x63kends_to_skip_bitmask\x18\x06 \x01(\x0c\"\x16\n\x14LoadModelResultValue\"\x12\n\x10LoadModelSkipped\"\xc1\x01\n\x0fLoadModelResult\x12<\n\x0cresult_value\x18\x01 \x01(\x0b\x32$.octoml_profile.LoadModelResultValueH\x00\x12\x31\n\x0b\x65rror_value\x18\x02 \x01(\x0b\x32\x1a.octoml_profile.ErrorValueH\x00\x12\x33\n\x07skipped\x18\x03 \x01(\x0b\x32 .octoml_profile.LoadModelSkippedH\x00\x42\x08\n\x06result\"M\n\x0eLoadModelReply\x12;\n\x12result_per_backend\x18\x01 \x03(\x0b\x32\x1f.octoml_profile.LoadModelResult\"Q\n\x06Tensor\x12*\n\x05\x64type\x18\x01 \x02(\x0e\x32\x1b.octoml_profile.TensorDtype\x12\r\n\x05shape\x18\x02 \x03(\x03\x12\x0c\n\x04\x64\x61ta\x18\x03 \x02(\x0c\":\n\x05Value\x12(\n\x06tensor\x18\x01 \x01(\x0b\x32\x16.octoml_profile.TensorH\x00\x42\x07\n\x05value\"F\n\nErrorValue\x12\x0f\n\x07message\x18\x01 \x02(\t\x12\'\n\x04\x63ode\x18\x02 \x02(\x0e\x32\x19.octoml_profile.ErrorCode\"\'\n\x08InputMap\x12\x1b\n\x13input_value_indices\x18\x01 \x03(\x05\"\xdf\x01\n\nRunRequest\x12\x14\n\x0csession_uuid\x18\x01 \x02(\x0c\x12\x10\n\x08model_id\x18\x02 \x02(\x04\x12%\n\x06inputs\x18\x03 \x03(\x0b\x32\x15.octoml_profile.Value\x12\x37\n\x15input_map_per_backend\x18\x06 \x03(\x0b\x32\x18.octoml_profile.InputMap\x12\x13\n\x0bnum_repeats\x18\x04 \x01(\x04\x12\x1f\n\x17repeat_for_milliseconds\x18\x05 \x01(\x04\x12\x13\n\x0bnum_warmups\x18\x07 \x01(\x04\"N\n\x0bResultValue\x12&\n\x07outputs\x18\x01 \x03(\x0b\x32\x15.octoml_profile.Value\x12\x17\n\x0frun_times_nanos\x18\x02 \x03(\x04\"}\n\tRunResult\x12\x33\n\x0cresult_value\x18\x01 \x01(\x0b\x32\x1b.octoml_profile.ResultValueH\x00\x12\x31\n\x0b\x65rror_value\x18\x02 \x01(\x0b\x32\x1a.octoml_profile.ErrorValueH\x00\x42\x08\n\x06result\"A\n\x08RunReply\x12\x35\n\x12result_per_backend\x18\x01 \x03(\x0b\x32\x19.octoml_profile.RunResult*>\n\x0bModelFormat\x12\x15\n\x11MODEL_FORMAT_ONNX\x10\x01\x12\x18\n\x14MODEL_FORMAT_FXPROTO\x10\x02*\xa0\x02\n\x0bTensorDtype\x12\x14\n\x10TENSOR_DTYPE_F16\x10\x01\x12\x14\n\x10TENSOR_DTYPE_F32\x10\x02\x12\x14\n\x10TENSOR_DTYPE_F64\x10\x03\x12\x13\n\x0fTENSOR_DTYPE_I8\x10\x04\x12\x14\n\x10TENSOR_DTYPE_I16\x10\x05\x12\x14\n\x10TENSOR_DTYPE_I32\x10\x06\x12\x14\n\x10TENSOR_DTYPE_I64\x10\x07\x12\x16\n\x12TENSOR_DTYPE_UINT8\x10\x08\x12\x17\n\x13TENSOR_DTYPE_UINT16\x10\t\x12\x17\n\x13TENSOR_DTYPE_UINT32\x10\n\x12\x17\n\x13TENSOR_DTYPE_UINT64\x10\x0b\x12\x15\n\x11TENSOR_DTYPE_BOOL\x10\x0c*\x8d\x01\n\tErrorCode\x12\x12\n\x0e\x45RROR_INTERNAL\x10\x00\x12\x19\n\x15\x45RROR_MODEL_INFERENCE\x10\x01\x12\x14\n\x10\x45RROR_MODEL_LOAD\x10\x02\x12\x1d\n\x19\x45RROR_BACKEND_NONEXISTENT\x10\x03\x12\x1c\n\x18\x45RROR_INSUFFICIENT_QUOTA\x10\x04')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*octoml_profile/protos/inference_base.proto\x12\x0eoctoml_profile\"\r\n\x0bPingRequest\"\x0b\n\tPingReply\"+\n\rBackendOption\x12\x0b\n\x03key\x18\x01 \x02(\t\x12\r\n\x05value\x18\x02 \x02(\t\"z\n\x0b\x42\x61\x63kendSpec\x12\x19\n\x11hardware_platform\x18\x01 \x02(\t\x12\x18\n\x10software_backend\x18\x02 \x02(\t\x12\x36\n\x0f\x62\x61\x63kend_options\x18\x03 \x03(\x0b\x32\x1d.octoml_profile.BackendOption\"[\n\x14\x43reateSessionRequest\x12\x14\n\x0csession_uuid\x18\x01 \x01(\x0c\x12-\n\x08\x62\x61\x63kends\x18\x02 \x03(\x0b\x32\x1b.octoml_profile.BackendSpec\"?\n\x18\x43reateSessionResultValue\x12\x14\n\x0csession_uuid\x18\x01 \x02(\x0c\x12\r\n\x05ready\x18\x02 \x02(\x08\"\x93\x01\n\x12\x43reateSessionReply\x12@\n\x0cresult_value\x18\x01 \x01(\x0b\x32(.octoml_profile.CreateSessionResultValueH\x00\x12\x31\n\x0b\x65rror_value\x18\x02 \x01(\x0b\x32\x1a.octoml_profile.ErrorValueH\x00\x42\x08\n\x06result\"4\n\x1cWaitUntilSessionReadyRequest\x12\x14\n\x0csession_uuid\x18\x01 \x02(\x0c\"+\n\x1aWaitUntilSessionReadyReply\x12\r\n\x05ready\x18\x01 \x02(\x08\"(\n\x10HeartbeatRequest\x12\x14\n\x0csession_uuid\x18\x01 \x02(\x0c\"\x10\n\x0eHeartbeatReply\"+\n\x13\x43loseSessionRequest\x12\x14\n\x0csession_uuid\x18\x01 \x02(\x0c\"\x13\n\x11\x43loseSessionReply\"\xa2\x01\n\x19LoadModelComponentRequest\x12\x14\n\x0csession_uuid\x18\x01 \x01(\x0c\x12\x10\n\x08model_id\x18\x02 \x01(\x04\x12\x1a\n\x12model_component_id\x18\x03 \x01(\x04\x12\x10\n\x08\x66ilename\x18\x04 \x01(\t\x12 \n\x18\x62\x61\x63kends_to_skip_bitmask\x18\x06 \x01(\x0c\x12\r\n\x05\x63hunk\x18\x05 \x02(\x0c\"\x1f\n\x1dLoadModelComponentResultValue\"\x1b\n\x19LoadModelComponentSkipped\"\xdc\x01\n\x18LoadModelComponentResult\x12\x45\n\x0cresult_value\x18\x01 \x01(\x0b\x32-.octoml_profile.LoadModelComponentResultValueH\x00\x12\x31\n\x0b\x65rror_value\x18\x02 \x01(\x0b\x32\x1a.octoml_profile.ErrorValueH\x00\x12<\n\x07skipped\x18\x03 \x01(\x0b\x32).octoml_profile.LoadModelComponentSkippedH\x00\x42\x08\n\x06result\"_\n\x17LoadModelComponentReply\x12\x44\n\x12result_per_backend\x18\x01 \x03(\x0b\x32(.octoml_profile.LoadModelComponentResult\"\xae\x01\n\x1fLoadCachedModelComponentRequest\x12\x14\n\x0csession_uuid\x18\x01 \x02(\x0c\x12\x10\n\x08model_id\x18\x02 \x02(\x04\x12\x1a\n\x12model_component_id\x18\x03 \x02(\x04\x12\x13\n\x0bsha256_hash\x18\x04 \x02(\x0c\x12\x10\n\x08\x66ilename\x18\x05 \x02(\t\x12 \n\x18\x62\x61\x63kends_to_skip_bitmask\x18\x06 \x01(\x0c\"e\n\x1dLoadCachedModelComponentReply\x12\x44\n\x12result_per_backend\x18\x01 \x03(\x0b\x32(.octoml_profile.LoadModelComponentResult\"\xba\x01\n\x10LoadModelRequest\x12\x14\n\x0csession_uuid\x18\x01 \x02(\x0c\x12\x10\n\x08model_id\x18\x02 \x02(\x04\x12\x31\n\x0cmodel_format\x18\x03 \x02(\x0e\x32\x1b.octoml_profile.ModelFormat\x12\x13\n\x0binput_names\x18\x04 \x03(\t\x12\x14\n\x0coutput_names\x18\x05 \x03(\t\x12 \n\x18\x62\x61\x63kends_to_skip_bitmask\x18\x06 \x01(\x0c\"\x16\n\x14LoadModelResultValue\"\x12\n\x10LoadModelSkipped\"\xc1\x01\n\x0fLoadModelResult\x12<\n\x0cresult_value\x18\x01 \x01(\x0b\x32$.octoml_profile.LoadModelResultValueH\x00\x12\x31\n\x0b\x65rror_value\x18\x02 \x01(\x0b\x32\x1a.octoml_profile.ErrorValueH\x00\x12\x33\n\x07skipped\x18\x03 \x01(\x0b\x32 .octoml_profile.LoadModelSkippedH\x00\x42\x08\n\x06result\"M\n\x0eLoadModelReply\x12;\n\x12result_per_backend\x18\x01 \x03(\x0b\x32\x1f.octoml_profile.LoadModelResult\"Q\n\x06Tensor\x12*\n\x05\x64type\x18\x01 \x02(\x0e\x32\x1b.octoml_profile.TensorDtype\x12\r\n\x05shape\x18\x02 \x03(\x03\x12\x0c\n\x04\x64\x61ta\x18\x03 \x02(\x0c\":\n\x05Value\x12(\n\x06tensor\x18\x01 \x01(\x0b\x32\x16.octoml_profile.TensorH\x00\x42\x07\n\x05value\"F\n\nErrorValue\x12\x0f\n\x07message\x18\x01 \x02(\t\x12\'\n\x04\x63ode\x18\x02 \x02(\x0e\x32\x19.octoml_profile.ErrorCode\"\'\n\x08InputMap\x12\x1b\n\x13input_value_indices\x18\x01 \x03(\x05\"\x86\x02\n\nRunRequest\x12\x14\n\x0csession_uuid\x18\x01 \x02(\x0c\x12\x10\n\x08model_id\x18\x02 \x02(\x04\x12%\n\x06inputs\x18\x03 \x03(\x0b\x32\x15.octoml_profile.Value\x12\x37\n\x15input_map_per_backend\x18\x06 \x03(\x0b\x32\x18.octoml_profile.InputMap\x12\x13\n\x0bnum_repeats\x18\x04 \x01(\x04\x12\x1f\n\x17repeat_for_milliseconds\x18\x05 \x01(\x04\x12\x13\n\x0bnum_warmups\x18\x07 \x01(\x04\x12%\n\x04mode\x18\x08 \x01(\x0e\x32\x17.octoml_profile.RunMode\"N\n\x0bResultValue\x12&\n\x07outputs\x18\x01 \x03(\x0b\x32\x15.octoml_profile.Value\x12\x17\n\x0frun_times_nanos\x18\x02 \x03(\x04\"}\n\tRunResult\x12\x33\n\x0cresult_value\x18\x01 \x01(\x0b\x32\x1b.octoml_profile.ResultValueH\x00\x12\x31\n\x0b\x65rror_value\x18\x02 \x01(\x0b\x32\x1a.octoml_profile.ErrorValueH\x00\x42\x08\n\x06result\"A\n\x08RunReply\x12\x35\n\x12result_per_backend\x18\x01 \x03(\x0b\x32\x19.octoml_profile.RunResult*>\n\x0bModelFormat\x12\x15\n\x11MODEL_FORMAT_ONNX\x10\x01\x12\x18\n\x14MODEL_FORMAT_FXPROTO\x10\x02*\xa0\x02\n\x0bTensorDtype\x12\x14\n\x10TENSOR_DTYPE_F16\x10\x01\x12\x14\n\x10TENSOR_DTYPE_F32\x10\x02\x12\x14\n\x10TENSOR_DTYPE_F64\x10\x03\x12\x13\n\x0fTENSOR_DTYPE_I8\x10\x04\x12\x14\n\x10TENSOR_DTYPE_I16\x10\x05\x12\x14\n\x10TENSOR_DTYPE_I32\x10\x06\x12\x14\n\x10TENSOR_DTYPE_I64\x10\x07\x12\x16\n\x12TENSOR_DTYPE_UINT8\x10\x08\x12\x17\n\x13TENSOR_DTYPE_UINT16\x10\t\x12\x17\n\x13TENSOR_DTYPE_UINT32\x10\n\x12\x17\n\x13TENSOR_DTYPE_UINT64\x10\x0b\x12\x15\n\x11TENSOR_DTYPE_BOOL\x10\x0c*\x8d\x01\n\tErrorCode\x12\x12\n\x0e\x45RROR_INTERNAL\x10\x00\x12\x19\n\x15\x45RROR_MODEL_INFERENCE\x10\x01\x12\x14\n\x10\x45RROR_MODEL_LOAD\x10\x02\x12\x1d\n\x19\x45RROR_BACKEND_NONEXISTENT\x10\x03\x12\x1c\n\x18\x45RROR_INSUFFICIENT_QUOTA\x10\x04*\'\n\x07RunMode\x12\r\n\tPROFILING\x10\x01\x12\r\n\tINFERENCE\x10\x02')
 
 _MODELFORMAT = DESCRIPTOR.enum_types_by_name['ModelFormat']
 ModelFormat = enum_type_wrapper.EnumTypeWrapper(_MODELFORMAT)
 _TENSORDTYPE = DESCRIPTOR.enum_types_by_name['TensorDtype']
 TensorDtype = enum_type_wrapper.EnumTypeWrapper(_TENSORDTYPE)
 _ERRORCODE = DESCRIPTOR.enum_types_by_name['ErrorCode']
 ErrorCode = enum_type_wrapper.EnumTypeWrapper(_ERRORCODE)
+_RUNMODE = DESCRIPTOR.enum_types_by_name['RunMode']
+RunMode = enum_type_wrapper.EnumTypeWrapper(_RUNMODE)
 MODEL_FORMAT_ONNX = 1
 MODEL_FORMAT_FXPROTO = 2
 TENSOR_DTYPE_F16 = 1
 TENSOR_DTYPE_F32 = 2
 TENSOR_DTYPE_F64 = 3
 TENSOR_DTYPE_I8 = 4
 TENSOR_DTYPE_I16 = 5
@@ -38,18 +40,21 @@
 TENSOR_DTYPE_UINT64 = 11
 TENSOR_DTYPE_BOOL = 12
 ERROR_INTERNAL = 0
 ERROR_MODEL_INFERENCE = 1
 ERROR_MODEL_LOAD = 2
 ERROR_BACKEND_NONEXISTENT = 3
 ERROR_INSUFFICIENT_QUOTA = 4
+PROFILING = 1
+INFERENCE = 2
 
 
 _PINGREQUEST = DESCRIPTOR.message_types_by_name['PingRequest']
 _PINGREPLY = DESCRIPTOR.message_types_by_name['PingReply']
+_BACKENDOPTION = DESCRIPTOR.message_types_by_name['BackendOption']
 _BACKENDSPEC = DESCRIPTOR.message_types_by_name['BackendSpec']
 _CREATESESSIONREQUEST = DESCRIPTOR.message_types_by_name['CreateSessionRequest']
 _CREATESESSIONRESULTVALUE = DESCRIPTOR.message_types_by_name['CreateSessionResultValue']
 _CREATESESSIONREPLY = DESCRIPTOR.message_types_by_name['CreateSessionReply']
 _WAITUNTILSESSIONREADYREQUEST = DESCRIPTOR.message_types_by_name['WaitUntilSessionReadyRequest']
 _WAITUNTILSESSIONREADYREPLY = DESCRIPTOR.message_types_by_name['WaitUntilSessionReadyReply']
 _HEARTBEATREQUEST = DESCRIPTOR.message_types_by_name['HeartbeatRequest']
@@ -86,14 +91,21 @@
 PingReply = _reflection.GeneratedProtocolMessageType('PingReply', (_message.Message,), {
   'DESCRIPTOR' : _PINGREPLY,
   '__module__' : 'octoml_profile.protos.inference_base_pb2'
   # @@protoc_insertion_point(class_scope:octoml_profile.PingReply)
   })
 _sym_db.RegisterMessage(PingReply)
 
+BackendOption = _reflection.GeneratedProtocolMessageType('BackendOption', (_message.Message,), {
+  'DESCRIPTOR' : _BACKENDOPTION,
+  '__module__' : 'octoml_profile.protos.inference_base_pb2'
+  # @@protoc_insertion_point(class_scope:octoml_profile.BackendOption)
+  })
+_sym_db.RegisterMessage(BackendOption)
+
 BackendSpec = _reflection.GeneratedProtocolMessageType('BackendSpec', (_message.Message,), {
   'DESCRIPTOR' : _BACKENDSPEC,
   '__module__' : 'octoml_profile.protos.inference_base_pb2'
   # @@protoc_insertion_point(class_scope:octoml_profile.BackendSpec)
   })
 _sym_db.RegisterMessage(BackendSpec)
 
@@ -299,78 +311,82 @@
   # @@protoc_insertion_point(class_scope:octoml_profile.RunReply)
   })
 _sym_db.RegisterMessage(RunReply)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _MODELFORMAT._serialized_start=2782
-  _MODELFORMAT._serialized_end=2844
-  _TENSORDTYPE._serialized_start=2847
-  _TENSORDTYPE._serialized_end=3135
-  _ERRORCODE._serialized_start=3138
-  _ERRORCODE._serialized_end=3279
+  _MODELFORMAT._serialized_start=2922
+  _MODELFORMAT._serialized_end=2984
+  _TENSORDTYPE._serialized_start=2987
+  _TENSORDTYPE._serialized_end=3275
+  _ERRORCODE._serialized_start=3278
+  _ERRORCODE._serialized_end=3419
+  _RUNMODE._serialized_start=3421
+  _RUNMODE._serialized_end=3460
   _PINGREQUEST._serialized_start=62
   _PINGREQUEST._serialized_end=75
   _PINGREPLY._serialized_start=77
   _PINGREPLY._serialized_end=88
-  _BACKENDSPEC._serialized_start=90
-  _BACKENDSPEC._serialized_end=156
-  _CREATESESSIONREQUEST._serialized_start=158
-  _CREATESESSIONREQUEST._serialized_end=249
-  _CREATESESSIONRESULTVALUE._serialized_start=251
-  _CREATESESSIONRESULTVALUE._serialized_end=314
-  _CREATESESSIONREPLY._serialized_start=317
-  _CREATESESSIONREPLY._serialized_end=464
-  _WAITUNTILSESSIONREADYREQUEST._serialized_start=466
-  _WAITUNTILSESSIONREADYREQUEST._serialized_end=518
-  _WAITUNTILSESSIONREADYREPLY._serialized_start=520
-  _WAITUNTILSESSIONREADYREPLY._serialized_end=563
-  _HEARTBEATREQUEST._serialized_start=565
-  _HEARTBEATREQUEST._serialized_end=605
-  _HEARTBEATREPLY._serialized_start=607
-  _HEARTBEATREPLY._serialized_end=623
-  _CLOSESESSIONREQUEST._serialized_start=625
-  _CLOSESESSIONREQUEST._serialized_end=668
-  _CLOSESESSIONREPLY._serialized_start=670
-  _CLOSESESSIONREPLY._serialized_end=689
-  _LOADMODELCOMPONENTREQUEST._serialized_start=692
-  _LOADMODELCOMPONENTREQUEST._serialized_end=854
-  _LOADMODELCOMPONENTRESULTVALUE._serialized_start=856
-  _LOADMODELCOMPONENTRESULTVALUE._serialized_end=887
-  _LOADMODELCOMPONENTSKIPPED._serialized_start=889
-  _LOADMODELCOMPONENTSKIPPED._serialized_end=916
-  _LOADMODELCOMPONENTRESULT._serialized_start=919
-  _LOADMODELCOMPONENTRESULT._serialized_end=1139
-  _LOADMODELCOMPONENTREPLY._serialized_start=1141
-  _LOADMODELCOMPONENTREPLY._serialized_end=1236
-  _LOADCACHEDMODELCOMPONENTREQUEST._serialized_start=1239
-  _LOADCACHEDMODELCOMPONENTREQUEST._serialized_end=1413
-  _LOADCACHEDMODELCOMPONENTREPLY._serialized_start=1415
-  _LOADCACHEDMODELCOMPONENTREPLY._serialized_end=1516
-  _LOADMODELREQUEST._serialized_start=1519
-  _LOADMODELREQUEST._serialized_end=1705
-  _LOADMODELRESULTVALUE._serialized_start=1707
-  _LOADMODELRESULTVALUE._serialized_end=1729
-  _LOADMODELSKIPPED._serialized_start=1731
-  _LOADMODELSKIPPED._serialized_end=1749
-  _LOADMODELRESULT._serialized_start=1752
-  _LOADMODELRESULT._serialized_end=1945
-  _LOADMODELREPLY._serialized_start=1947
-  _LOADMODELREPLY._serialized_end=2024
-  _TENSOR._serialized_start=2026
-  _TENSOR._serialized_end=2107
-  _VALUE._serialized_start=2109
-  _VALUE._serialized_end=2167
-  _ERRORVALUE._serialized_start=2169
-  _ERRORVALUE._serialized_end=2239
-  _INPUTMAP._serialized_start=2241
-  _INPUTMAP._serialized_end=2280
-  _RUNREQUEST._serialized_start=2283
-  _RUNREQUEST._serialized_end=2506
-  _RESULTVALUE._serialized_start=2508
-  _RESULTVALUE._serialized_end=2586
-  _RUNRESULT._serialized_start=2588
-  _RUNRESULT._serialized_end=2713
-  _RUNREPLY._serialized_start=2715
-  _RUNREPLY._serialized_end=2780
+  _BACKENDOPTION._serialized_start=90
+  _BACKENDOPTION._serialized_end=133
+  _BACKENDSPEC._serialized_start=135
+  _BACKENDSPEC._serialized_end=257
+  _CREATESESSIONREQUEST._serialized_start=259
+  _CREATESESSIONREQUEST._serialized_end=350
+  _CREATESESSIONRESULTVALUE._serialized_start=352
+  _CREATESESSIONRESULTVALUE._serialized_end=415
+  _CREATESESSIONREPLY._serialized_start=418
+  _CREATESESSIONREPLY._serialized_end=565
+  _WAITUNTILSESSIONREADYREQUEST._serialized_start=567
+  _WAITUNTILSESSIONREADYREQUEST._serialized_end=619
+  _WAITUNTILSESSIONREADYREPLY._serialized_start=621
+  _WAITUNTILSESSIONREADYREPLY._serialized_end=664
+  _HEARTBEATREQUEST._serialized_start=666
+  _HEARTBEATREQUEST._serialized_end=706
+  _HEARTBEATREPLY._serialized_start=708
+  _HEARTBEATREPLY._serialized_end=724
+  _CLOSESESSIONREQUEST._serialized_start=726
+  _CLOSESESSIONREQUEST._serialized_end=769
+  _CLOSESESSIONREPLY._serialized_start=771
+  _CLOSESESSIONREPLY._serialized_end=790
+  _LOADMODELCOMPONENTREQUEST._serialized_start=793
+  _LOADMODELCOMPONENTREQUEST._serialized_end=955
+  _LOADMODELCOMPONENTRESULTVALUE._serialized_start=957
+  _LOADMODELCOMPONENTRESULTVALUE._serialized_end=988
+  _LOADMODELCOMPONENTSKIPPED._serialized_start=990
+  _LOADMODELCOMPONENTSKIPPED._serialized_end=1017
+  _LOADMODELCOMPONENTRESULT._serialized_start=1020
+  _LOADMODELCOMPONENTRESULT._serialized_end=1240
+  _LOADMODELCOMPONENTREPLY._serialized_start=1242
+  _LOADMODELCOMPONENTREPLY._serialized_end=1337
+  _LOADCACHEDMODELCOMPONENTREQUEST._serialized_start=1340
+  _LOADCACHEDMODELCOMPONENTREQUEST._serialized_end=1514
+  _LOADCACHEDMODELCOMPONENTREPLY._serialized_start=1516
+  _LOADCACHEDMODELCOMPONENTREPLY._serialized_end=1617
+  _LOADMODELREQUEST._serialized_start=1620
+  _LOADMODELREQUEST._serialized_end=1806
+  _LOADMODELRESULTVALUE._serialized_start=1808
+  _LOADMODELRESULTVALUE._serialized_end=1830
+  _LOADMODELSKIPPED._serialized_start=1832
+  _LOADMODELSKIPPED._serialized_end=1850
+  _LOADMODELRESULT._serialized_start=1853
+  _LOADMODELRESULT._serialized_end=2046
+  _LOADMODELREPLY._serialized_start=2048
+  _LOADMODELREPLY._serialized_end=2125
+  _TENSOR._serialized_start=2127
+  _TENSOR._serialized_end=2208
+  _VALUE._serialized_start=2210
+  _VALUE._serialized_end=2268
+  _ERRORVALUE._serialized_start=2270
+  _ERRORVALUE._serialized_end=2340
+  _INPUTMAP._serialized_start=2342
+  _INPUTMAP._serialized_end=2381
+  _RUNREQUEST._serialized_start=2384
+  _RUNREQUEST._serialized_end=2646
+  _RESULTVALUE._serialized_start=2648
+  _RESULTVALUE._serialized_end=2726
+  _RUNRESULT._serialized_start=2728
+  _RUNRESULT._serialized_end=2853
+  _RUNREPLY._serialized_start=2855
+  _RUNREPLY._serialized_end=2920
 # @@protoc_insertion_point(module_scope)
```

### Comparing `octoml_profile-0.2.1/octoml_profile/protos/remote_inference_pb2.py` & `octoml_profile-0.2.2rc1/octoml_profile/protos/remote_inference_pb2.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.1/octoml_profile/protos/remote_inference_pb2_grpc.py` & `octoml_profile-0.2.2rc1/octoml_profile/protos/remote_inference_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.1/octoml_profile/shape.py` & `octoml_profile-0.2.2rc1/octoml_profile/shape.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.1/pyproject.toml` & `octoml_profile-0.2.2rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -10,27 +10,28 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 [tool.poetry]
 name = "octoml_profile"
-version = "0.2.1"
+version = "0.2.2rc1"
 description = "Client package for OctoML Profile service"
 authors = ["Greg Bonik <gbonik@octoml.ai>"]
 license = "Apache-2.0"
 include = ["octoml_profile/protos/*_pb2.py", "octoml_profile/protos/*_pb2_grpc.py"]
 exclude = ["octoml_profile/private"]
 
 [tool.pytest.ini_options]
 log_cli = false
 
 [tool.poetry.dependencies]
 python = "^3.8"
 onnx = "^1.12.0"
 grpcio = "^1.42.0"
+tabulate = "^0.9.0"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `octoml_profile-0.2.1/setup.py` & `octoml_profile-0.2.2rc1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,19 +7,19 @@
  'octoml_profile.patches',
  'octoml_profile.protos']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['grpcio>=1.42.0,<2.0.0', 'onnx>=1.12.0,<2.0.0']
+['grpcio>=1.42.0,<2.0.0', 'onnx>=1.12.0,<2.0.0', 'tabulate>=0.9.0,<0.10.0']
 
 setup_kwargs = {
     'name': 'octoml-profile',
-    'version': '0.2.1',
+    'version': '0.2.2rc1',
     'description': 'Client package for OctoML Profile service',
     'long_description': None,
     'author': 'Greg Bonik',
     'author_email': 'gbonik@octoml.ai',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```


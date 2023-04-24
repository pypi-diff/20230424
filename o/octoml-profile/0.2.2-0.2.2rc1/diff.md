# Comparing `tmp/octoml_profile-0.2.2.tar.gz` & `tmp/octoml_profile-0.2.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octoml_profile-0.2.2.tar", max compression
+gzip compressed data, was "octoml_profile-0.2.2rc1.tar", max compression
```

## Comparing `octoml_profile-0.2.2.tar` & `octoml_profile-0.2.2rc1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    11358 2023-04-24 17:30:29.201378 octoml_profile-0.2.2/LICENSE
--rw-r--r--   0        0        0      319 2023-04-24 17:30:29.201378 octoml_profile-0.2.2/octoml_profile/README.md
--rw-r--r--   0        0        0     1242 2023-04-24 17:30:29.201378 octoml_profile-0.2.2/octoml_profile/__init__.py
--rw-r--r--   0        0        0      656 2023-04-24 17:30:34.492774 octoml_profile-0.2.2/octoml_profile/_about.py
--rw-r--r--   0        0        0    29912 2023-04-24 17:30:29.201378 octoml_profile-0.2.2/octoml_profile/client.py
--rw-r--r--   0        0        0     1757 2023-04-24 17:30:29.201378 octoml_profile-0.2.2/octoml_profile/conversion_util.py
--rw-r--r--   0        0        0    37765 2023-04-24 17:30:29.201378 octoml_profile-0.2.2/octoml_profile/dynamo.py
--rw-r--r--   0        0        0     1312 2023-04-24 17:30:29.201378 octoml_profile-0.2.2/octoml_profile/errors.py
--rw-r--r--   0        0        0    15537 2023-04-24 17:30:29.201378 octoml_profile-0.2.2/octoml_profile/fx2proto.py
--rw-r--r--   0        0        0     8422 2023-04-24 17:30:29.201378 octoml_profile-0.2.2/octoml_profile/inference_session.py
--rw-r--r--   0        0        0      576 2023-04-24 17:30:29.201378 octoml_profile-0.2.2/octoml_profile/interceptors/__init__.py
--rw-r--r--   0        0        0     1498 2023-04-24 17:30:29.201378 octoml_profile-0.2.2/octoml_profile/interceptors/auth.py
--rw-r--r--   0        0        0     2497 2023-04-24 17:30:29.201378 octoml_profile-0.2.2/octoml_profile/interceptors/base.py
--rw-r--r--   0        0        0      997 2023-04-24 17:30:29.201378 octoml_profile-0.2.2/octoml_profile/interceptors/cookie.py
--rw-r--r--   0        0        0     1182 2023-04-24 17:30:29.201378 octoml_profile-0.2.2/octoml_profile/log_util.py
--rw-r--r--   0        0        0     1025 2023-04-24 17:30:29.201378 octoml_profile-0.2.2/octoml_profile/patches/__init__.py
--rw-r--r--   0        0        0     2048 2023-04-24 17:30:29.202378 octoml_profile-0.2.2/octoml_profile/patches/build_map_unpack.py
--rw-r--r--   0        0        0     1860 2023-04-24 17:30:29.202378 octoml_profile-0.2.2/octoml_profile/patches/diffusers_output_type.py
--rw-r--r--   0        0        0     1064 2023-04-24 17:30:29.202378 octoml_profile-0.2.2/octoml_profile/patches/dyn_shape_call_neg.py
--rw-r--r--   0        0        0     1175 2023-04-24 17:30:29.202378 octoml_profile-0.2.2/octoml_profile/patches/iadd_tuple_tuple.py
--rw-r--r--   0        0        0     1115 2023-04-24 17:30:29.202378 octoml_profile-0.2.2/octoml_profile/patches/user_defined_call.py
--rw-r--r--   0        0        0      705 2023-04-24 17:30:29.202378 octoml_profile-0.2.2/octoml_profile/pricing.py
--rw-r--r--   0        0        0    11193 2023-04-24 17:30:30.052441 octoml_profile-0.2.2/octoml_profile/protos/fxgraph_pb2.py
--rw-r--r--   0        0        0      159 2023-04-24 17:30:30.052441 octoml_profile-0.2.2/octoml_profile/protos/fxgraph_pb2_grpc.py
--rw-r--r--   0        0        0    23668 2023-04-24 17:30:30.052441 octoml_profile-0.2.2/octoml_profile/protos/inference_base_pb2.py
--rw-r--r--   0        0        0      159 2023-04-24 17:30:30.052441 octoml_profile-0.2.2/octoml_profile/protos/inference_base_pb2_grpc.py
--rw-r--r--   0        0        0     4290 2023-04-24 17:30:30.052441 octoml_profile-0.2.2/octoml_profile/protos/remote_inference_pb2.py
--rw-r--r--   0        0        0    19277 2023-04-24 17:30:30.052441 octoml_profile-0.2.2/octoml_profile/protos/remote_inference_pb2_grpc.py
--rw-r--r--   0        0        0    19878 2023-04-24 17:30:29.202378 octoml_profile-0.2.2/octoml_profile/report.py
--rw-r--r--   0        0        0     2475 2023-04-24 17:30:29.202378 octoml_profile-0.2.2/octoml_profile/shape.py
--rw-r--r--   0        0        0     2955 2023-04-24 17:30:29.202378 octoml_profile-0.2.2/octoml_profile/workaround.py
--rw-r--r--   0        0        0     1146 2023-04-24 17:30:34.486773 octoml_profile-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      769 2023-04-24 17:30:35.917704 octoml_profile-0.2.2/setup.py
--rw-r--r--   0        0        0      589 2023-04-24 17:30:35.917970 octoml_profile-0.2.2/PKG-INFO
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

### Comparing `octoml_profile-0.2.2/LICENSE` & `octoml_profile-0.2.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.2/octoml_profile/__init__.py` & `octoml_profile-0.2.2rc1/octoml_profile/__init__.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.2/octoml_profile/_about.py` & `octoml_profile-0.2.2rc1/octoml_profile/_about.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-version = "0.2.2"
-git_commit_hash = "47dcea45087f347b6ed9fcab24e856ede28bd578"
+version = "0.2.2rc1"
+git_commit_hash = "009309ea2408255db27d3a9050fc79837ba86810"
```

### Comparing `octoml_profile-0.2.2/octoml_profile/client.py` & `octoml_profile-0.2.2rc1/octoml_profile/client.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.2/octoml_profile/conversion_util.py` & `octoml_profile-0.2.2rc1/octoml_profile/conversion_util.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.2/octoml_profile/dynamo.py` & `octoml_profile-0.2.2rc1/octoml_profile/dynamo.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,32 +177,32 @@
 @dataclass
 class _AggregatedResult:
     func_name: str
     sums: Sequence[Union[_LocalCpuSegment, _CompiledSegment]]
     num_runs: int
     compilation_occurred: bool
     compilation_errors: Sequence[str]
-    num_discarded_runs: int = 0
+    num_disgarded_runs: int = 0
 
     def add(self,
             sample: Sequence[Union[_LocalCpuSegment, _CompiledSegment]],
             compilation_occurred: bool):
         assert len(self.sums) == len(sample)
         # Cases when adding two aggs:
         # - no-compile + no-compile: merge
         # - compile + compile: merge
         # - compile + no-compile: replace compile with no compile, disgard compile
         # - no-compile + compile: ignore and disgard
         if self.compilation_occurred and not compilation_occurred:
             self.compilation_occurred = False
-            self.num_discarded_runs = self.num_runs
+            self.num_disgarded_runs = self.num_runs
             self.num_runs = 1
             self.sums = [s for s in sample]
         elif not self.compilation_occurred and compilation_occurred:
-            self.num_discarded_runs += 1
+            self.num_disgarded_runs += 1
         else:
             for agg, new in zip(self.sums, sample):
                 agg.add(new)
             self.num_runs += 1
 
     def report(self, num_repeats):
         segments = []
@@ -264,15 +264,15 @@
                        total_uncompiled_ms=total_uncompiled_ms,
                        total_per_backend=total_per_backend,
                        compilation_occurred=self.compilation_occurred,
                        compilation_errors=self.compilation_errors,
                        num_runs=self.num_runs,
                        num_repeats=num_repeats,
                        graph_results=graph_results,
-                       num_discarded_runs=self.num_discarded_runs)
+                       num_disgarded_runs=self.num_disgarded_runs)
 
 
 class _TraceRecorder:
     def __init__(self):
         self._start_nanos = None
         self._segments = []
         self._result_by_footprint = OrderedDict()
@@ -334,15 +334,15 @@
         if agg_result is None:
             self._result_by_footprint[run_footprint] = \
                 _AggregatedResult(self.func_name,
                                   tuple(self._segments),
                                   num_runs=1,
                                   compilation_occurred=self._compilation_occurred,
                                   compilation_errors=self._compilation_errors,
-                                  num_discarded_runs=0)
+                                  num_disgarded_runs=0)
         else:
             agg_result.add(self._segments, self._compilation_occurred)
 
         if self._compilation_occurred:
             self._compilation_occurred = False
         self._segments.clear()
```

### Comparing `octoml_profile-0.2.2/octoml_profile/errors.py` & `octoml_profile-0.2.2rc1/octoml_profile/errors.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.2/octoml_profile/fx2proto.py` & `octoml_profile-0.2.2rc1/octoml_profile/fx2proto.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.2/octoml_profile/inference_session.py` & `octoml_profile-0.2.2rc1/octoml_profile/inference_session.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.2/octoml_profile/interceptors/__init__.py` & `octoml_profile-0.2.2rc1/octoml_profile/interceptors/__init__.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.2/octoml_profile/interceptors/auth.py` & `octoml_profile-0.2.2rc1/octoml_profile/interceptors/auth.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.2/octoml_profile/interceptors/base.py` & `octoml_profile-0.2.2rc1/octoml_profile/interceptors/base.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.2/octoml_profile/interceptors/cookie.py` & `octoml_profile-0.2.2rc1/octoml_profile/interceptors/cookie.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.2/octoml_profile/log_util.py` & `octoml_profile-0.2.2rc1/octoml_profile/log_util.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.2/octoml_profile/patches/__init__.py` & `octoml_profile-0.2.2rc1/octoml_profile/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.2/octoml_profile/patches/build_map_unpack.py` & `octoml_profile-0.2.2rc1/octoml_profile/patches/build_map_unpack.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.2/octoml_profile/patches/diffusers_output_type.py` & `octoml_profile-0.2.2rc1/octoml_profile/patches/diffusers_output_type.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.2/octoml_profile/patches/dyn_shape_call_neg.py` & `octoml_profile-0.2.2rc1/octoml_profile/patches/dyn_shape_call_neg.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.2/octoml_profile/patches/iadd_tuple_tuple.py` & `octoml_profile-0.2.2rc1/octoml_profile/patches/iadd_tuple_tuple.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.2/octoml_profile/patches/user_defined_call.py` & `octoml_profile-0.2.2rc1/octoml_profile/patches/user_defined_call.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.2/octoml_profile/pricing.py` & `octoml_profile-0.2.2rc1/octoml_profile/pricing.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.2/octoml_profile/protos/fxgraph_pb2.py` & `octoml_profile-0.2.2rc1/octoml_profile/protos/fxgraph_pb2.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.2/octoml_profile/protos/inference_base_pb2.py` & `octoml_profile-0.2.2rc1/octoml_profile/protos/inference_base_pb2.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.2/octoml_profile/protos/remote_inference_pb2.py` & `octoml_profile-0.2.2rc1/octoml_profile/protos/remote_inference_pb2.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.2/octoml_profile/protos/remote_inference_pb2_grpc.py` & `octoml_profile-0.2.2rc1/octoml_profile/protos/remote_inference_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.2/octoml_profile/report.py` & `octoml_profile-0.2.2rc1/octoml_profile/report.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
     total_uncompiled_ms: float
     total_per_backend: OrderedDict[str, TotalPerBackendResult]
     compilation_occurred: bool
     compilation_errors: Sequence[str]
     num_runs: int
     num_repeats: int
     graph_results: Sequence[GraphResult]
-    num_discarded_runs: int
+    num_disgarded_runs: int
 
     def _should_abridge(self, verbose):
         return not verbose and \
                len(self._compiled_segments()) > MAX_COMPILED_SEGMENTS_DISPLAYED_DEFAULT
 
     def _compiled_segments(self):
         return [s for s in self.segments if s.graph_id is not None]
@@ -401,19 +401,19 @@
             profiles = profiles_by_func[func]
 
             num_profiles = "1 profile" if len(profiles) == 1 else f"{len(profiles)} profiles"
             print(file=file)
             print(f'Function `{func}` has {num_profiles}:', file=file)
             for i, p in enumerate(profiles):
                 profile_id = f'{func}[{i+1}/{len(profiles)}]'
-                total_runs = p.num_runs + p.num_discarded_runs
+                total_runs = p.num_runs + p.num_disgarded_runs
                 runs = "1 time" if total_runs == 1 else f'{total_runs} times'
                 header = f'- Profile `{profile_id}` ran {runs}.'
-                if p.num_discarded_runs > 0:
-                    header += f' ({p.num_discarded_runs} discarded because compilation happened)'
+                if p.num_disgarded_runs > 0:
+                    header += f' ({p.num_disgarded_runs} disgarded because compilation happened)'
                 elif p.compilation_occurred:
                     header += f' (compilation occurred)'
                 print(header + "\n", file=file)
                 path_prefix = f'{self.report_dir}/{func}_{i+1}'
                 p.print(file=file, report_path_prefix=path_prefix, verbose=verbose)
                 print(file=file)
```

### Comparing `octoml_profile-0.2.2/octoml_profile/shape.py` & `octoml_profile-0.2.2rc1/octoml_profile/shape.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.2/octoml_profile/workaround.py` & `octoml_profile-0.2.2rc1/octoml_profile/workaround.py`

 * *Files identical despite different names*

### Comparing `octoml_profile-0.2.2/pyproject.toml` & `octoml_profile-0.2.2rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 [tool.poetry]
 name = "octoml_profile"
-version = "0.2.2"
+version = "0.2.2rc1"
 description = "Client package for OctoML Profile service"
 authors = ["Greg Bonik <gbonik@octoml.ai>"]
 license = "Apache-2.0"
 include = ["octoml_profile/protos/*_pb2.py", "octoml_profile/protos/*_pb2_grpc.py"]
 exclude = ["octoml_profile/private"]
 
 [tool.pytest.ini_options]
```

### Comparing `octoml_profile-0.2.2/setup.py` & `octoml_profile-0.2.2rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['grpcio>=1.42.0,<2.0.0', 'onnx>=1.12.0,<2.0.0', 'tabulate>=0.9.0,<0.10.0']
 
 setup_kwargs = {
     'name': 'octoml-profile',
-    'version': '0.2.2',
+    'version': '0.2.2rc1',
     'description': 'Client package for OctoML Profile service',
     'long_description': None,
     'author': 'Greg Bonik',
     'author_email': 'gbonik@octoml.ai',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `octoml_profile-0.2.2/PKG-INFO` & `octoml_profile-0.2.2rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octoml-profile
-Version: 0.2.2
+Version: 0.2.2rc1
 Summary: Client package for OctoML Profile service
 License: Apache-2.0
 Author: Greg Bonik
 Author-email: gbonik@octoml.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```


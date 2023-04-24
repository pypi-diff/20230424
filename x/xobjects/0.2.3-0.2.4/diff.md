# Comparing `tmp/xobjects-0.2.3.tar.gz` & `tmp/xobjects-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xobjects-0.2.3.tar", last modified: Mon Apr  3 19:21:27 2023, max compression
+gzip compressed data, was "xobjects-0.2.4.tar", last modified: Mon Apr 24 06:51:24 2023, max compression
```

## Comparing `xobjects-0.2.3.tar` & `xobjects-0.2.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-04-03 19:21:27.705291 xobjects-0.2.3/
--rw-r--r--   0 giadarol   (503) staff       (20)    11356 2023-03-23 11:04:29.000000 xobjects-0.2.3/LICENSE
--rw-r--r--   0 giadarol   (503) staff       (20)      613 2023-04-03 19:21:27.705374 xobjects-0.2.3/PKG-INFO
--rw-r--r--   0 giadarol   (503) staff       (20)       92 2023-03-23 11:04:29.000000 xobjects-0.2.3/pyproject.toml
--rw-r--r--   0 giadarol   (503) staff       (20)      180 2023-04-03 19:21:27.705621 xobjects-0.2.3/setup.cfg
--rw-r--r--   0 giadarol   (503) staff       (20)     1231 2023-03-23 11:04:29.000000 xobjects-0.2.3/setup.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-04-03 19:21:27.704321 xobjects-0.2.3/xobjects/
--rw-r--r--   0 giadarol   (503) staff       (20)      915 2023-04-03 19:20:50.000000 xobjects-0.2.3/xobjects/__init__.py
--rw-r--r--   0 giadarol   (503) staff       (20)     6443 2023-03-23 11:04:29.000000 xobjects-0.2.3/xobjects/_patch_pyopencl_array.py
--rw-r--r--   0 giadarol   (503) staff       (20)       22 2023-04-03 19:21:04.000000 xobjects-0.2.3/xobjects/_version.py
--rw-r--r--   0 giadarol   (503) staff       (20)    23020 2023-03-23 11:04:29.000000 xobjects-0.2.3/xobjects/array.py
--rw-r--r--   0 giadarol   (503) staff       (20)    15856 2023-03-23 11:04:29.000000 xobjects-0.2.3/xobjects/capi.py
--rw-r--r--   0 giadarol   (503) staff       (20)    21690 2023-03-29 07:05:06.000000 xobjects-0.2.3/xobjects/context.py
--rw-r--r--   0 giadarol   (503) staff       (20)    27575 2023-04-03 19:20:50.000000 xobjects-0.2.3/xobjects/context_cpu.py
--rw-r--r--   0 giadarol   (503) staff       (20)    23940 2023-03-29 07:05:06.000000 xobjects-0.2.3/xobjects/context_cupy.py
--rw-r--r--   0 giadarol   (503) staff       (20)    17221 2023-03-29 07:05:06.000000 xobjects-0.2.3/xobjects/context_pyopencl.py
--rw-r--r--   0 giadarol   (503) staff       (20)      160 2023-04-03 19:20:50.000000 xobjects-0.2.3/xobjects/general.py
--rw-r--r--   0 giadarol   (503) staff       (20)    12265 2023-03-23 11:04:29.000000 xobjects-0.2.3/xobjects/hybrid_class.py
--rw-r--r--   0 giadarol   (503) staff       (20)     1504 2023-03-23 11:04:29.000000 xobjects-0.2.3/xobjects/linkedarray.py
--rw-r--r--   0 giadarol   (503) staff       (20)     8921 2023-03-23 11:04:29.000000 xobjects-0.2.3/xobjects/ref.py
--rw-r--r--   0 giadarol   (503) staff       (20)     2550 2023-03-23 11:04:29.000000 xobjects-0.2.3/xobjects/scalar.py
--rw-r--r--   0 giadarol   (503) staff       (20)     4601 2023-03-23 11:04:29.000000 xobjects-0.2.3/xobjects/specialize_source.py
--rw-r--r--   0 giadarol   (503) staff       (20)     4996 2023-03-23 11:04:29.000000 xobjects-0.2.3/xobjects/string.py
--rw-r--r--   0 giadarol   (503) staff       (20)    16297 2023-04-03 19:20:50.000000 xobjects-0.2.3/xobjects/struct.py
--rw-r--r--   0 giadarol   (503) staff       (20)     2652 2023-03-23 11:04:29.000000 xobjects-0.2.3/xobjects/test_helpers.py
--rw-r--r--   0 giadarol   (503) staff       (20)     2846 2023-03-23 11:04:29.000000 xobjects-0.2.3/xobjects/typeutils.py
--rw-r--r--   0 giadarol   (503) staff       (20)     4269 2023-03-23 11:04:29.000000 xobjects-0.2.3/xobjects/union.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-04-03 19:21:27.705166 xobjects-0.2.3/xobjects.egg-info/
--rw-r--r--   0 giadarol   (503) staff       (20)      613 2023-04-03 19:21:27.000000 xobjects-0.2.3/xobjects.egg-info/PKG-INFO
--rw-r--r--   0 giadarol   (503) staff       (20)      646 2023-04-03 19:21:27.000000 xobjects-0.2.3/xobjects.egg-info/SOURCES.txt
--rw-r--r--   0 giadarol   (503) staff       (20)        1 2023-04-03 19:21:27.000000 xobjects-0.2.3/xobjects.egg-info/dependency_links.txt
--rw-r--r--   0 giadarol   (503) staff       (20)       27 2023-04-03 19:21:27.000000 xobjects-0.2.3/xobjects.egg-info/requires.txt
--rw-r--r--   0 giadarol   (503) staff       (20)        9 2023-04-03 19:21:27.000000 xobjects-0.2.3/xobjects.egg-info/top_level.txt
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-04-24 06:51:24.545729 xobjects-0.2.4/
+-rw-r--r--   0 giadarol   (503) staff       (20)    11356 2023-03-23 11:04:29.000000 xobjects-0.2.4/LICENSE
+-rw-r--r--   0 giadarol   (503) staff       (20)      613 2023-04-24 06:51:24.545799 xobjects-0.2.4/PKG-INFO
+-rw-r--r--   0 giadarol   (503) staff       (20)       92 2023-03-23 11:04:29.000000 xobjects-0.2.4/pyproject.toml
+-rw-r--r--   0 giadarol   (503) staff       (20)      180 2023-04-24 06:51:24.546328 xobjects-0.2.4/setup.cfg
+-rw-r--r--   0 giadarol   (503) staff       (20)     1231 2023-03-23 11:04:29.000000 xobjects-0.2.4/setup.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-04-24 06:51:24.544925 xobjects-0.2.4/xobjects/
+-rw-r--r--   0 giadarol   (503) staff       (20)      915 2023-04-03 19:20:50.000000 xobjects-0.2.4/xobjects/__init__.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     6443 2023-03-23 11:04:29.000000 xobjects-0.2.4/xobjects/_patch_pyopencl_array.py
+-rw-r--r--   0 giadarol   (503) staff       (20)       22 2023-04-24 06:51:14.000000 xobjects-0.2.4/xobjects/_version.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    23020 2023-03-23 11:04:29.000000 xobjects-0.2.4/xobjects/array.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    15856 2023-03-23 11:04:29.000000 xobjects-0.2.4/xobjects/capi.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    21914 2023-04-24 06:51:14.000000 xobjects-0.2.4/xobjects/context.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    28238 2023-04-24 06:51:14.000000 xobjects-0.2.4/xobjects/context_cpu.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    23940 2023-03-29 07:05:06.000000 xobjects-0.2.4/xobjects/context_cupy.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    17221 2023-03-29 07:05:06.000000 xobjects-0.2.4/xobjects/context_pyopencl.py
+-rw-r--r--   0 giadarol   (503) staff       (20)      160 2023-04-03 19:20:50.000000 xobjects-0.2.4/xobjects/general.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    12265 2023-03-23 11:04:29.000000 xobjects-0.2.4/xobjects/hybrid_class.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     1504 2023-03-23 11:04:29.000000 xobjects-0.2.4/xobjects/linkedarray.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     8921 2023-03-23 11:04:29.000000 xobjects-0.2.4/xobjects/ref.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     2550 2023-03-23 11:04:29.000000 xobjects-0.2.4/xobjects/scalar.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     4601 2023-03-23 11:04:29.000000 xobjects-0.2.4/xobjects/specialize_source.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     4996 2023-03-23 11:04:29.000000 xobjects-0.2.4/xobjects/string.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    16297 2023-04-03 19:20:50.000000 xobjects-0.2.4/xobjects/struct.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     2638 2023-04-24 06:51:14.000000 xobjects-0.2.4/xobjects/test_helpers.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     2846 2023-03-23 11:04:29.000000 xobjects-0.2.4/xobjects/typeutils.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     4269 2023-03-23 11:04:29.000000 xobjects-0.2.4/xobjects/union.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-04-24 06:51:24.545624 xobjects-0.2.4/xobjects.egg-info/
+-rw-r--r--   0 giadarol   (503) staff       (20)      613 2023-04-24 06:51:24.000000 xobjects-0.2.4/xobjects.egg-info/PKG-INFO
+-rw-r--r--   0 giadarol   (503) staff       (20)      646 2023-04-24 06:51:24.000000 xobjects-0.2.4/xobjects.egg-info/SOURCES.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)        1 2023-04-24 06:51:24.000000 xobjects-0.2.4/xobjects.egg-info/dependency_links.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)       27 2023-04-24 06:51:24.000000 xobjects-0.2.4/xobjects.egg-info/requires.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)        9 2023-04-24 06:51:24.000000 xobjects-0.2.4/xobjects.egg-info/top_level.txt
```

### Comparing `xobjects-0.2.3/LICENSE` & `xobjects-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.3/PKG-INFO` & `xobjects-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xobjects
-Version: 0.2.3
+Version: 0.2.4
 Summary: In-memory serialization and code generator for CPU and GPU
 Home-page: https://xsuite.readthedocs.io/
 Download-URL: https://pypi.python.org/pypi/xobjects
 Author: Riccardo De Maria
 Author-email: riccardo.de.maria@cern.ch
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/xsuite/xsuite/issues
```

### Comparing `xobjects-0.2.3/setup.py` & `xobjects-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.3/xobjects/__init__.py` & `xobjects-0.2.4/xobjects/__init__.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.3/xobjects/_patch_pyopencl_array.py` & `xobjects-0.2.4/xobjects/_patch_pyopencl_array.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.3/xobjects/array.py` & `xobjects-0.2.4/xobjects/array.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.3/xobjects/capi.py` & `xobjects-0.2.4/xobjects/capi.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.3/xobjects/context.py` & `xobjects-0.2.4/xobjects/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,14 +229,17 @@
 class XContext(ABC):
     minimum_alignment = 1
 
     def __init__(self):
         self._kernels = KernelDict()
         self._buffers = []
 
+    def __str__(self):
+        return type(self).__name__
+
     def new_buffer(self, capacity=1048576):
         buf = self._make_buffer(capacity=capacity)
         self.buffers.append(weakref.finalize(buf, log.debug, "free buf"))
         return buf
 
     @property
     def buffers(self):
@@ -645,14 +648,16 @@
             option = []
         else:
             ctxtype, options = ctxstr.split(":")
             option = options.split(",")
     if ctxtype == "ContextCpu":
         if len(option) == 0:
             return xo.ContextCpu()
+        elif option[0] == "auto":
+            return xo.ContextCpu(omp_num_threads="auto")
         else:
             return xo.ContextCpu(omp_num_threads=int(option[0]))
     elif ctxtype == "ContextCupy":
         if len(option) == 0:
             return xo.ContextCupy()
         else:
             return xo.ContextCupy(device=int(option[0]))
@@ -668,22 +673,22 @@
 def get_test_contexts():
     import os
     import xobjects as xo
 
     ctxstr = os.environ.get("XOBJECTS_TEST_CONTEXTS")
     if ctxstr is None:
         yield xo.ContextCpu()
-        # yield xo.ContextCpu(omp_num_threads=2)
+        yield xo.ContextCpu(omp_num_threads="auto")
         if xo.ContextCupy in xo.context.available:
             yield xo.ContextCupy()
         if xo.ContextPyopencl in xo.context.available:
             yield xo.ContextPyopencl()
     elif ctxstr == "all":
         yield xo.ContextCpu()
-        yield xo.ContextCpu(omp_num_threads=2)
+        yield xo.ContextCpu(omp_num_threads="auto")
         if xo.ContextCupy in xo.context.available:
             yield xo.ContextCupy()
         if xo.ContextPyopencl in xo.context.available:
             for dd in xo.ContextPyopencl.get_devices():
                 yield xo.ContextPyopencl(device=dd)
 
     else:
@@ -698,13 +703,14 @@
 
     Examples:
        ContextPyopencl:0.0  -> ContextPyopencl(device="0.0")
        ContextPyopencl:1.0  -> ContextPyopencl(device="1.0")
        ContextPyopencl      -> ContextPyopencl()
        ContextCpu           -> ContextCpu()
        ContextCpu:2         -> ContextCpu(omp_num_threads=2)
+       ContextCpu:auto      -> ContextCpu(omp_num_threads='auto')
        ContextCupy:0        -> ContextCupy(device=0)
     """
     import os
 
     ctxstr = os.environ.get("XOBJECTS_USER_CONTEXT")
     return get_context_from_string(ctxstr)
```

### Comparing `xobjects-0.2.3/xobjects/context_cpu.py` & `xobjects-0.2.4/xobjects/context_cpu.py`

 * *Files 4% similar despite different names*

```diff
@@ -129,21 +129,29 @@
         return np.ndarray
 
     @property
     def linked_array_type(self):
         return LinkedArrayCpu
 
     def __init__(self, omp_num_threads=0):
+        """
+        Create a new CPU context, serial or with parallelization using OpenMP.
+        Args:
+            omp_num_threads (int | Literal['auto']): Number of threads to be
+            used by OpenMP. If 0, no parallelization is used. If 'auto', the
+            number of threads is selected automatically by OpenMP.
+        """
         super().__init__()
         self.omp_num_threads = omp_num_threads
 
-        if self.omp_num_threads > 1:
-            raise NotImplementedError(
-                "OpenMP parallelization not yet supported!"
-            )
+    def __str__(self):
+        if not self.openmp_enabled:
+            return super().__str__()
+        else:
+            return f"{type(self).__name__}:{self.omp_num_threads}"
 
     def _make_buffer(self, capacity):
         return BufferNumpy(capacity=capacity, context=self)
 
     def add_kernels(
         self,
         sources=None,
@@ -380,24 +388,25 @@
 
         for pyname, kernel in kernel_descriptions.items():
             if pyname not in cdefs:  # check if kernel not already declared
                 signature = cdef_from_kernel(kernel, pyname)
                 ffi_interface.cdef(signature)
                 log.debug(f"cffi def {pyname} {signature}")
 
-        if self.omp_num_threads > 0:
+        if self.openmp_enabled:
             ffi_interface.cdef("void omp_set_num_threads(int);")
+            ffi_interface.cdef("int omp_get_max_threads();")
 
         # Compile
         xtr_compile_args = ["-std=c99"]
         xtr_link_args = ["-std=c99"]
         xtr_compile_args += extra_compile_args
         xtr_link_args += extra_link_args
 
-        if self.omp_num_threads > 0:
+        if self.openmp_enabled:
             xtr_compile_args.append("-fopenmp")
             xtr_link_args.append("-fopenmp")
 
         if os.name == "nt":  # windows
             # TODO: to be handled properly
             xtr_compile_args = []
             xtr_link_args = []
@@ -440,23 +449,23 @@
     ) -> Tuple[str, str]:
         sources = sources or []
         classes = classes or []
         cls_sources = sources_from_classes(classes)
 
         headers = ["#include <stdint.h>"]
 
-        if self.omp_num_threads > 0:
+        if self.openmp_enabled:
             headers = ["#include <omp.h>"] + headers
 
         headers += extra_headers
         sources = headers + cls_sources + sources
         source, folders = _concatenate_sources(sources, apply_to_source)
 
         if specialize:
-            if self.omp_num_threads > 0:
+            if self.openmp_enabled:
                 specialize_for = "cpu_openmp"
             else:
                 specialize_for = "cpu_serial"
 
             # included files are searched in the same folders od the src_filed
             specialized_source = specialize_source(
                 source,
@@ -477,17 +486,17 @@
         """
         so_path = _so_for_module_name(name, containing_dir)
         # Import the compiled module
         spec = importlib.util.spec_from_file_location(name, so_path)
         module = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(module)
 
-        if self.omp_num_threads > 0:
-            raise NotImplementedError("OpenMP not supported for now!")
+        if self.openmp_enabled:
             self.omp_set_num_threads = module.lib.omp_set_num_threads
+            self.omp_get_max_threads = module.lib.omp_get_max_threads
 
         return module
 
     def nparray_to_context_array(self, arr):
         """
         Moves a numpy array to the device memory. No action is performed by
         this function in the CPU context. The method is provided
@@ -562,25 +571,33 @@
 
             # Forward tranform (in place)
             plan.transform(data2)
 
             # Inverse tranform (in place)
             plan.itransform(data2)
         """
-        return FFTCpu(data, axes, threads=self.omp_num_threads)
+        try:
+            num_threads = self.omp_get_max_threads()
+        except AttributeError:
+            num_threads = 1
+        return FFTCpu(data, axes, threads=num_threads)
 
     @property
     def kernels(self):
         """
         Dictionary containing all the kernels that have been imported to the context.
         The syntax ``context.kernels.mykernel`` can also be used.
         """
 
         return self._kernels
 
+    @property
+    def openmp_enabled(self):
+        return self.omp_num_threads != 0
+
 
 class BufferByteArray(XBuffer):
     def _make_context(self):
         return ContextCpu()
 
     def _new_buffer(self, capacity):
         return bytearray(capacity)
@@ -756,16 +773,17 @@
             )
         assert len(kwargs.keys()) == self.num_args
         arg_list = []
         for arg in self.description.args:
             vv = kwargs[arg.name]
             arg_list.append(self.to_function_arg(arg, vv))
 
-        if self.context.omp_num_threads > 0:
-            self.context.omp_set_num_threads(self.context.omp_num_threads)
+        if self.context.openmp_enabled:
+            if isinstance(self.context.omp_num_threads, int):
+                self.context.omp_set_num_threads(self.context.omp_num_threads)
 
         ret = self.function(*arg_list)
 
         if self.description.ret is not None:
             return self.from_function_arg(self.description.ret, ret)
```

### Comparing `xobjects-0.2.3/xobjects/context_cupy.py` & `xobjects-0.2.4/xobjects/context_cupy.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.3/xobjects/context_pyopencl.py` & `xobjects-0.2.4/xobjects/context_pyopencl.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.3/xobjects/hybrid_class.py` & `xobjects-0.2.4/xobjects/hybrid_class.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.3/xobjects/linkedarray.py` & `xobjects-0.2.4/xobjects/linkedarray.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.3/xobjects/ref.py` & `xobjects-0.2.4/xobjects/ref.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.3/xobjects/scalar.py` & `xobjects-0.2.4/xobjects/scalar.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.3/xobjects/specialize_source.py` & `xobjects-0.2.4/xobjects/specialize_source.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.3/xobjects/string.py` & `xobjects-0.2.4/xobjects/string.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.3/xobjects/struct.py` & `xobjects-0.2.4/xobjects/struct.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.3/xobjects/test_helpers.py` & `xobjects-0.2.4/xobjects/test_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 ) -> Callable:
     """Parametrize the decorated test over all test contexts with the argument
     `test_context`, excluding those contexts whose names are in ``excluding."""
     if isinstance(excluding, str):
         excluding = (excluding,)
 
     test_context_names = tuple(
-        ctx_name
+        str(ctx)
         for ctx in get_test_contexts()
-        if (ctx_name := type(ctx).__name__) not in excluding
+        if type(ctx).__name__ not in excluding
     )
 
     @wraps(test_function)
     def actual_test(*args, **kwargs):
         kwargs["test_context"] = get_context_from_string(
             kwargs["test_context"]
         )
```

### Comparing `xobjects-0.2.3/xobjects/typeutils.py` & `xobjects-0.2.4/xobjects/typeutils.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.3/xobjects/union.py` & `xobjects-0.2.4/xobjects/union.py`

 * *Files identical despite different names*

### Comparing `xobjects-0.2.3/xobjects.egg-info/PKG-INFO` & `xobjects-0.2.4/xobjects.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xobjects
-Version: 0.2.3
+Version: 0.2.4
 Summary: In-memory serialization and code generator for CPU and GPU
 Home-page: https://xsuite.readthedocs.io/
 Download-URL: https://pypi.python.org/pypi/xobjects
 Author: Riccardo De Maria
 Author-email: riccardo.de.maria@cern.ch
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/xsuite/xsuite/issues
```

### Comparing `xobjects-0.2.3/xobjects.egg-info/SOURCES.txt` & `xobjects-0.2.4/xobjects.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/rombus-1.0.5.tar.gz` & `tmp/rombus-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rombus-1.0.5.tar", max compression
+gzip compressed data, was "rombus-1.0.6.tar", max compression
```

## Comparing `rombus-1.0.5.tar` & `rombus-1.0.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1094 2023-04-03 06:16:26.281571 rombus-1.0.5/LICENSE
--rw-r--r--   0        0        0     1939 2023-04-03 06:16:26.281571 rombus-1.0.5/README.md
--rw-r--r--   0        0        0     1920 2023-04-03 06:17:29.545755 rombus-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     1266 2023-04-03 06:16:26.285571 rombus-1.0.5/python/rombus/__init__.py
--rw-r--r--   0        0        0        0 2023-04-03 06:16:26.285571 rombus-1.0.5/python/rombus/_core/__init__.py
--rw-r--r--   0        0        0      777 2023-04-03 06:16:26.285571 rombus-1.0.5/python/rombus/_core/hdf5.py
--rw-r--r--   0        0        0       46 2023-04-03 06:16:26.285571 rombus-1.0.5/python/rombus/_core/log/__init__.py
--rw-r--r--   0        0        0    28317 2023-04-03 06:16:26.285571 rombus-1.0.5/python/rombus/_core/log/log.py
--rw-r--r--   0        0        0      141 2023-04-03 06:16:26.285571 rombus-1.0.5/python/rombus/_core/mpi.py
--rw-r--r--   0        0        0     6213 2023-04-03 06:16:26.285571 rombus-1.0.5/python/rombus/cli.py
--rw-r--r--   0        0        0    10206 2023-04-03 06:16:26.285571 rombus-1.0.5/python/rombus/ei.py
--rw-r--r--   0        0        0     2229 2023-04-03 06:16:26.285571 rombus-1.0.5/python/rombus/exceptions.py
--rw-r--r--   0        0        0    13884 2023-04-03 06:16:26.285571 rombus-1.0.5/python/rombus/model.py
--rw-r--r--   0        0        0     3155 2023-04-03 06:16:26.285571 rombus-1.0.5/python/rombus/models/PhenomP.py
--rw-r--r--   0        0        0    23639 2023-04-03 06:16:26.285571 rombus-1.0.5/python/rombus/models/PhenomP_samples.csv
--rw-r--r--   0        0        0        0 2023-04-03 06:16:26.285571 rombus-1.0.5/python/rombus/models/__init__.py
--rw-r--r--   0        0        0     2887 2023-04-03 06:16:26.285571 rombus-1.0.5/python/rombus/models/sinc.py
--rw-r--r--   0        0        0       25 2023-04-03 06:16:26.285571 rombus-1.0.5/python/rombus/models/sinc_samples.csv
--rw-r--r--   0        0        0     4659 2023-04-03 06:16:26.285571 rombus-1.0.5/python/rombus/params.py
--rw-r--r--   0        0        0     3768 2023-04-03 06:16:26.285571 rombus-1.0.5/python/rombus/plots.py
--rw-r--r--   0        0        0     9176 2023-04-03 06:16:26.285571 rombus-1.0.5/python/rombus/reduced_basis.py
--rw-r--r--   0        0        0    10418 2023-04-03 06:16:26.285571 rombus-1.0.5/python/rombus/rom.py
--rw-r--r--   0        0        0     5236 2023-04-03 06:16:26.285571 rombus-1.0.5/python/rombus/samples.py
--rw-r--r--   0        0        0        0 2023-04-03 06:16:26.285571 rombus-1.0.5/python/rombus/tests/__init__.py
--rw-r--r--   0        0        0      393 2023-04-03 06:16:26.285571 rombus-1.0.5/python/rombus/tests/conftest.py
--rw-r--r--   0        0        0       24 2023-04-03 06:16:26.285571 rombus-1.0.5/python/rombus/tests/resources/.gitignore
--rw-r--r--   0        0        0        0 2023-04-03 06:16:26.285571 rombus-1.0.5/python/rombus/tests/resources/__init__.py
--rw-r--r--   0        0        0     1234 2023-04-03 06:16:26.285571 rombus-1.0.5/python/rombus/tests/test_PhenomP.py
--rw-r--r--   0        0        0      245 2023-04-03 06:16:26.285571 rombus-1.0.5/python/rombus/tests/test_reduced_basis.py
--rw-r--r--   0        0        0     3349 1970-01-01 00:00:00.000000 rombus-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-04-24 09:29:57.236307 rombus-1.0.6/LICENSE
+-rw-r--r--   0        0        0     1987 2023-04-24 09:29:57.236307 rombus-1.0.6/README.md
+-rw-r--r--   0        0        0     1920 2023-04-24 09:30:28.372651 rombus-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1266 2023-04-24 09:29:57.240307 rombus-1.0.6/python/rombus/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-24 09:29:57.240307 rombus-1.0.6/python/rombus/_core/__init__.py
+-rw-r--r--   0        0        0      777 2023-04-24 09:29:57.240307 rombus-1.0.6/python/rombus/_core/hdf5.py
+-rw-r--r--   0        0        0       46 2023-04-24 09:29:57.240307 rombus-1.0.6/python/rombus/_core/log/__init__.py
+-rw-r--r--   0        0        0    28381 2023-04-24 09:29:57.240307 rombus-1.0.6/python/rombus/_core/log/log.py
+-rw-r--r--   0        0        0      141 2023-04-24 09:29:57.240307 rombus-1.0.6/python/rombus/_core/mpi.py
+-rw-r--r--   0        0        0     6728 2023-04-24 09:29:57.240307 rombus-1.0.6/python/rombus/cli.py
+-rw-r--r--   0        0        0    10699 2023-04-24 09:29:57.240307 rombus-1.0.6/python/rombus/ei.py
+-rw-r--r--   0        0        0     2446 2023-04-24 09:29:57.240307 rombus-1.0.6/python/rombus/exceptions.py
+-rw-r--r--   0        0        0    15270 2023-04-24 09:29:57.240307 rombus-1.0.6/python/rombus/model.py
+-rw-r--r--   0        0        0     3242 2023-04-24 09:29:57.240307 rombus-1.0.6/python/rombus/models/PhenomP.py
+-rw-r--r--   0        0        0    23639 2023-04-24 09:29:57.240307 rombus-1.0.6/python/rombus/models/PhenomP_samples.csv
+-rw-r--r--   0        0        0        0 2023-04-24 09:29:57.240307 rombus-1.0.6/python/rombus/models/__init__.py
+-rw-r--r--   0        0        0     3354 2023-04-24 09:29:57.240307 rombus-1.0.6/python/rombus/models/sinc.py
+-rw-r--r--   0        0        0       25 2023-04-24 09:29:57.240307 rombus-1.0.6/python/rombus/models/sinc_samples.csv
+-rw-r--r--   0        0        0     4747 2023-04-24 09:29:57.240307 rombus-1.0.6/python/rombus/params.py
+-rw-r--r--   0        0        0     4514 2023-04-24 09:29:57.240307 rombus-1.0.6/python/rombus/plots.py
+-rw-r--r--   0        0        0     9311 2023-04-24 09:29:57.240307 rombus-1.0.6/python/rombus/reduced_basis.py
+-rw-r--r--   0        0        0    10810 2023-04-24 09:29:57.240307 rombus-1.0.6/python/rombus/rom.py
+-rw-r--r--   0        0        0     5236 2023-04-24 09:29:57.240307 rombus-1.0.6/python/rombus/samples.py
+-rw-r--r--   0        0        0        0 2023-04-24 09:29:57.240307 rombus-1.0.6/python/rombus/tests/__init__.py
+-rw-r--r--   0        0        0      393 2023-04-24 09:29:57.240307 rombus-1.0.6/python/rombus/tests/conftest.py
+-rw-r--r--   0        0        0       24 2023-04-24 09:29:57.240307 rombus-1.0.6/python/rombus/tests/resources/.gitignore
+-rw-r--r--   0        0        0        0 2023-04-24 09:29:57.240307 rombus-1.0.6/python/rombus/tests/resources/__init__.py
+-rw-r--r--   0        0        0     1311 2023-04-24 09:29:57.240307 rombus-1.0.6/python/rombus/tests/test_PhenomP.py
+-rw-r--r--   0        0        0      245 2023-04-24 09:29:57.240307 rombus-1.0.6/python/rombus/tests/test_reduced_basis.py
+-rw-r--r--   0        0        0     3397 1970-01-01 00:00:00.000000 rombus-1.0.6/PKG-INFO
```

### Comparing `rombus-1.0.5/LICENSE` & `rombus-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rombus-1.0.5/README.md` & `rombus-1.0.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 Rombus: Helps you qucikly and easily compute slow and complex models
 ====================================================================
 
 Rombus is a tool for building reduced order models (ROMs): matrix representations of arbitrary
 models which can be rapidly and easily computed for arbitrary parameter sets.
 
-Building a ROM with Rombus is easy.  All you need to do is define your model like this (in this trivial case, a file named `my_model.py` specifying a simple second-order polynomial):
+Building a ROM with Rombus is easy.  All you need to do is install it like so:
+```console
+$ pip install rombus
 ```
+define your model like this (in this trivial case, a file named `my_model.py` specifying a simple second-order polynomial):
+``` python
 from numpy import ndarray, polyval, linspace
 from rombus.model import RombusModel
 from typing import NamedTuple
 
 
-class model(RombusModel):
-    """Class for creating a ROM for the function y=a2*x^2+a1*x+a0"""
+class Model(RombusModel):
+    """Class for creating a ROM for the function y(x)=a2*x^2+a1*x+a0"""
+
+    coordinate.set("x", 0.0, 10.0, 11, label="$x$")
+
+    ordinate.set("y", label="$y(x)$")
 
     params.add("a0", -10, 10)
     params.add("a1", -10, 10)
     params.add("a2", -10, 10)
 
-    # Set the domain over-and-on which the ROM will be defined
-    def set_domain(self) -> ndarray:
-        return linspace(0, 10, 11)
-
     def compute(self, p: NamedTuple, x: ndarray) -> ndarray:
         """Compute the model for a given parameter set."""
         return polyval([p.a2, p.a1, p.a0], x)
 ```
 and specify a set of points (in this case, the file `my_model_samples.py`) to build your ROM from:
 ```
 -10, -10,-10
@@ -35,34 +39,33 @@
  10, -10,-10
  10,  10,-10
  10, -10, 10
  10,  10, 10
 ```
 You build your ROM like this:
 ```
-$ rombus build my_model:model my_model_samples.csv
+$ rombus build my_model:Model my_model_samples.csv
 ```
-This produces an _HDF5_ file named `my_model.hdf5`.  You can then use your new ROM in
-your Python projects like this:
+This produces an _HDF5_ file named `my_model.hdf5`.  You can then use your new ROM in your Python projects like this:
 ```
 from rombus.rom import ReducedOrderModel
 
 ROM = ReducedOrderModel.from_file('my_model.hdf5')
 sample = ROM.model.sample({"a0":0,"a1":0,"a2":1})
 model_ROM = ROM.evaluate(sample)
 for x, y in zip(ROM.model.domain,model_ROM):
-    print(f"{x:.2f} {y:.2f}")
+    print(f"{x:5.2f} {y:6.2f}")
 ```
 which generates the output:
 ```
-0.00 0.00
-1.00 1.00
-2.00 4.00
-3.00 9.00
-4.00 16.00
-5.00 25.00
-6.00 36.00
-7.00 49.00
-8.00 64.00
-9.00 81.00
+ 0.00   0.00
+ 1.00   1.00
+ 2.00   4.00
+ 3.00   9.00
+ 4.00  16.00
+ 5.00  25.00
+ 6.00  36.00
+ 7.00  49.00
+ 8.00  64.00
+ 9.00  81.00
 10.00 100.00
 ```
```

### Comparing `rombus-1.0.5/pyproject.toml` & `rombus-1.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rombus"
-version = "v1.0.5"
+version = "v1.0.6"
 description = "Reduced order modeling for the masses"
 authors = [
             "Gregory Poole <gbpoole@gmail.com>",
             "J. Hu <jitinghu@swin.edu.au>",
             ]
 license = "MIT-expat"
```

### Comparing `rombus-1.0.5/python/rombus/__init__.py` & `rombus-1.0.6/python/rombus/__init__.py`

 * *Files identical despite different names*

### Comparing `rombus-1.0.5/python/rombus/_core/hdf5.py` & `rombus-1.0.6/python/rombus/_core/hdf5.py`

 * *Files identical despite different names*

### Comparing `rombus-1.0.5/python/rombus/_core/log/log.py` & `rombus-1.0.6/python/rombus/_core/log/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # For legacy-Python compatibility
 from __future__ import print_function
 from functools import update_wrapper
 import traceback
 
 from typing import List
 
+import os
 import sys
 import time
 import datetime
 
 import inspect
 from functools import wraps
 
@@ -28,15 +29,15 @@
     ("hours", 3600),  # 60 * 60
     ("minutes", 60),
     ("seconds", 1),
 )
 
 string_types = (str, bytes)
 
-TIMING_AUTO_SECONDS_DEFAULT = 0
+TIMING_AUTO_SECONDS_DEFAULT = 0.5
 
 
 def is_nonstring_iterable(object_in):
     """Determine if an object is a non-string iterable.
 
     :param object: An object of any type.
     :return: Boolean.  True if object is a non-string iterable.
@@ -195,14 +196,16 @@
 
         # Print exception and stack trace then exit
         traceback.print_exception(exception)
 
         # Halt the logger, in case we're inside nested log.contexts
         self.halt()
 
+        raise
+
     def callable(
         self,
         msg=None,
         dump_args=False,
         dump_returns=False,
         time_elapsed="auto",
         default_verbosity="unset",
@@ -449,18 +452,19 @@
     def set_fp(self, fp_out=None):
         """Set the file pointer to be used for logging.  Default is
         `sys.stderr`.
 
         :param fp_out: File pointer
         :return: None
         """
-        if fp_out is None:
-            self.fp = sys.stderr
+
+        if "PYTEST_CURRENT_TEST" in os.environ:
+            self.fp = open(os.devnull, "w")
         else:
-            self.fp = fp_out
+            self.fp = sys.stderr
 
     def set_verbosity(self, verbosity=True):
         """Add a new (and make it current) verbosity state to the stream's
         stack of verbosity states.
 
         This method takes either a boolean flag indicating whether logging is active, or an integer indicating
         the maximum indenting level that will be rendered.  It can be removed using the
```

### Comparing `rombus-1.0.5/python/rombus/cli.py` & `rombus-1.0.6/python/rombus/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 
 @cli.command(context_settings=CONTEXT_SETTINGS)
 @click.argument("project_name", type=str)
 def quickstart(project_name: str) -> None:
     """Write a project template to kickstart the creation of a new project."""
 
-    with log.context("Creating new project from template"):
+    with log.context("Creating new project from template", time_elapsed=True):
         RombusModel.write_project_template(project_name)
 
 
 @cli.command(context_settings=CONTEXT_SETTINGS)
 @click.argument("model", type=str)
 @click.argument("filename_samples", type=click.Path(exists=True))
 @click.option(
@@ -80,15 +80,15 @@
     model: str,
     filename_samples: str,
     out: str,
     do_step: click.Choice,
 ) -> None:
     """Build a Reduced Order Model."""
 
-    with log.context("Building ROM"):
+    with log.context("Building ROM", time_elapsed=True):
         log.comment(f"Model:   {model}")
         log.comment(f"Samples: {filename_samples}")
 
         # Load model
         model_loaded = RombusModel.load(model)
 
         # Load samples
@@ -96,50 +96,68 @@
 
         # Build ROM
         assert do_step is None or type(do_step) == str  # keeping mypy happy
         ROM = ReducedOrderModel(model_loaded, samples).build(do_step=do_step)
 
         # Write ROM
         if out == "MODEL_BASENAME.hdf5":
-            filename_out = f"{model_loaded.model_basename}.hdf5"
+            filename_out = f"{model_loaded.basename}.hdf5"
         else:
             filename_out = out
         ROM.write(filename_out)
 
 
 @cli.command(context_settings=CONTEXT_SETTINGS)
 @click.argument("filename_ROM", type=click.Path(exists=True))
 @click.pass_context
 def refine(ctx: click.core.Context, filename_rom: str) -> None:
     """Refine parameter sampling to improve an established reduced order model."""
 
-    with log.context(f"Refining ROM ({filename_rom})"):
+    with log.context(f"Refining ROM ({filename_rom})", time_elapsed=True):
 
         # Build model and refine it
         ROM = ReducedOrderModel.from_file(filename_rom).refine()
 
         # Write results
-        filename_split = filename_rom.rsplit(".", 1)
-        filename_out = f"{filename_split[0]}_refined.{filename_split[1]}"
+        filename_out = f"{ROM.basename}_refined.hdf5"
         ROM.write(filename_out)
 
 
 @cli.command(context_settings=FLEX_CONTEXT_SETTINGS)
 @click.argument("filename_ROM", type=str)
+@click.pass_context
+def plot_bases(
+    ctx: click.core.Context,
+    filename_rom: str,
+) -> None:
+    """Plot the bases (and their errors) of a reduced order model."""
+
+    with log.context("Plotting bases", time_elapsed=True):
+
+        # Read ROM
+        ROM = ReducedOrderModel.from_file(filename_rom)
+
+        # Generate plots
+        plots.bases(ROM)
+        plots.bases_errors(ROM)
+
+
+@cli.command(context_settings=FLEX_CONTEXT_SETTINGS)
+@click.argument("filename_ROM", type=str)
 @click.argument("parameters", nargs=-1, type=click.UNPROCESSED)
 @click.pass_context
 def evaluate(
     ctx: click.core.Context, filename_rom: str, parameters: Tuple[str, ...]
 ) -> None:
     """Evaluate a reduced order model and compare it to truth.
 
     PARAMETERS is a list of parameter values of the form A=VAL B=VAL ...
     """
 
-    with log.context("Evaluating ROM"):
+    with log.context("Evaluating ROM", time_elapsed=True):
 
         # Read ROM
         ROM = ReducedOrderModel.from_file(filename_rom)
 
         # Parse the model parameters, which should have been given as arguments
         model_params = ROM.model.parse_cli_params(parameters)
 
@@ -156,15 +174,17 @@
     default=100,
     help="Number of samples to use for timing",
 )
 @click.pass_context
 def timing(ctx: click.core.Context, filename_rom: str, n_samples: int) -> None:
     """Compute timing information for a ROM and it's source model."""
 
-    with log.context(f"Creating timing information for ROM {filename_rom}"):
+    with log.context(
+        f"Creating timing information for ROM {filename_rom}", time_elapsed=True
+    ):
         # Read ROM
         ROM = ReducedOrderModel.from_file(filename_rom)
 
         # Generate the samples to be used
         timing_sample = Samples(ROM.model, n_random=n_samples)
 
         # Generate timing information for model
```

### Comparing `rombus-1.0.5/python/rombus/ei.py` & `rombus-1.0.6/python/rombus/ei.py`

 * *Files 6% similar despite different names*

```diff
@@ -152,16 +152,14 @@
 
     def next_invV_col(self, R, indices, check_finite=False):
         b = np.zeros(len(indices), dtype=R.dtype)
         b[-1] = 1.0
         return self.solve_triangular(
             R[:, indices], b, lower=False, check_finite=check_finite
         )
-        # return solve_triangular(
-        #    R[:,indices], b, lower=False, check_finite=check_finite)
 
     def eim_interpolant(self, invV, R):
         """The empirical interpolation matrix 'B'"""
         return np.dot(invV, R)
 
     def eim_interpolate(self, h, indices, B):
         """Empirically interpolate a function"""
@@ -270,20 +268,36 @@
         Self
             A reference to self, to allow for chaining of method calls
         """
 
         eim = _StandardEIM(
             reduced_basis.matrix_shape[0],
             reduced_basis.matrix_shape[1],
-            dtype=reduced_basis.model.model_dtype,
+            dtype=reduced_basis.model.ordinate.dtype,
         )
         eim.make(reduced_basis.matrix)
 
         domain = reduced_basis.model.domain
         self.nodes = domain[eim.indices]
+
+        # #########################################################
+        # import sys
+        # last_j = -1
+        # sorted_zipped = sorted(enumerate(eim.indices), key=lambda x: x[1])
+        # print(sorted_zipped)
+        # for i,j in sorted_zipped:
+        #     if j==last_j:
+        #         print(i,j)
+        #     last_j = j
+        # sys.exit()
+        # zipped = list(zip(self.nodes, eim.B))
+        # sorted_zipped = sorted(zipped, key=lambda x: x[0])
+        # self.nodes, self.B_matrix = zip(*sorted_zipped)
+        # #########################################################
+
         self.nodes, self.B_matrix = zip(*sorted(zip(self.nodes, eim.B)))
 
         return self
 
     @log.callable("Writing empirical interpolant")
     def write(self, h5file: hdf5.File) -> None:
         """Write empirical interpolant to an open HDF5 file
```

### Comparing `rombus-1.0.5/python/rombus/exceptions.py` & `rombus-1.0.6/python/rombus/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,14 +23,26 @@
 
     pass
 
 
 # rombus.model exceptions
 
 
+class RombusModelOrdinateError(RombusException):
+    """Raised when an error is encountered when initialising a RombusModel ordinate."""
+
+    pass
+
+
+class RombusModelCoordinateError(RombusException):
+    """Raised when an error is encountered when initialising a RombusModel coordinate."""
+
+    pass
+
+
 class RombusModelParamsError(RombusException):
     """Raised when a Rombus model is instantiated with no parameters specified."""
 
     pass
 
 
 class RombusModelImportFromStringError(RombusException):
@@ -41,30 +53,21 @@
 
 class RombusModelInitError(RombusException):
     """Raised when the instantiation of a RombusModel fails."""
 
     pass
 
 
-# rombus.params exceptions
-
-
-# class ReducedParamsError(RombusException):
-#    """Raised when ."""
-#
-#    pass
-
-
 # rombus.plots exceptions
 
 
-# class ReducedPlotsError(RombusException):
-#    """Raised when ."""
-#
-#    pass
+class RombusPlotError(RombusException):
+    """Raised when there is an error generating a plot."""
+
+    pass
 
 
 # rombus.samples exceptions
 
 
 # class ReducedSamplesError(RombusException):
 #    """Raised when ."""
```

### Comparing `rombus-1.0.5/python/rombus/model.py` & `rombus-1.0.6/python/rombus/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,123 @@
 import importlib
 import sys
 import os
 import shutil
 import timeit
 from abc import ABCMeta, abstractmethod
 from collections import Counter
-from typing import Any, Dict, Self, Tuple, TYPE_CHECKING
+from typing import Any, Dict, Self, Optional, Tuple, TYPE_CHECKING
 
 import numpy as np
 
 import rombus._core.hdf5 as hdf5
 import rombus.exceptions as exceptions
 from rombus.params import Params
 from rombus._core.log import log
 from typing import NamedTuple
 
+import warnings
+
+warnings.simplefilter("ignore", np.ComplexWarning)
+
 # Need to put Samples in quotes below and check TYPE_CHECKING here to
 # manage circular imports with models.py
 if TYPE_CHECKING:
     from rombus.samples import Samples
 
 
+class _Ordinate(object):
+    def __init__(self):
+        self.name = None
+        self.dtype = float
+        self.label = None
+
+    def set(
+        self, name: Optional[str], dtype: type | np.dtype = float, label: str = ""
+    ) -> None:
+        """Set the details of the model's ordinate.
+
+        Parameters
+        ----------
+        name : str
+            Name of ordinate
+        dtype : type|np.dtype
+            Datatype used to represent ordinate values
+        label : str
+            A n optional label to use for the ordinate in plots, etc.
+        """
+        self.name = name
+        self.dtype = dtype
+        if label == "":
+            self.label = self.name
+        else:
+            self.label = label
+
+
+class _Coordinate(object):
+    def __init__(self):
+        self.name = None
+        self.dtype = float
+        self.min = None
+        self.max = None
+        self.label = None
+        self._values = None
+        self._n_values = 0
+
+    def set(
+        self,
+        name: str,
+        min: Any,
+        max: Any,
+        n_values: int,
+        dtype: type | np.dtype = float,
+        label: str = "",
+    ) -> None:
+        self.name = name
+        self.dtype = dtype
+        self.min = min
+        self.max = max
+        if label == "":
+            self.label = self.name
+        else:
+            self.label = label
+        if self.dtype != type(min):
+            raise exceptions.RombusModelCoordinateError(
+                f"Coordinate datatype ({self.dtype}) and min-value datatype ({type(self.min)}) don't match."
+            )
+        if self.dtype != type(max):
+            raise exceptions.RombusModelCoordinateError(
+                f"Coordinate datatype ({self.dtype}) and max-value datatype ({type(self.max)}) don't match."
+            )
+        self._n_values = n_values
+        self._values = np.linspace(self.min, self.max, self._n_values, self.dtype)
+
+    def get(self):
+        return self._values
+
+    def __len__(self):
+        return self._n_values
+
+
 class _RombusModelMeta(type):
     def __prepare__(name, *args, **kwargs):
         """Initialise the dictionary that gets passed to __new___.
 
         This is needed here because we don't want the user to have to
         initialise the member(s) that we are adding.  This is the only
         method that gets sourced before the class code is executed, so
         it needs to be done here, not in __new__.
         """
 
         result = dict()
 
         # Initialise the following members↵
+        result["coordinate"] = _Coordinate()
+        result["ordinate"] = _Ordinate()
         result["params"] = Params()
-        result["model_dtype"] = np.dtype("float64")
 
         return result
 
     def __new__(mcs, name, bases, dct):
 
         # Perform super-metaclass construction↵
         return super(_RombusModelMeta, mcs).__new__(mcs, name, bases, dct)
@@ -50,69 +128,51 @@
 
     pass
 
 
 class RombusModel(metaclass=_RombusModelABCMeta):
     """Baseclass from which all RombusModels must inherit."""
 
-    # These two members are instantiated by the metaclass
+    # These members are instantiated by the metaclass
+    coordinate: _Coordinate
+    """The domain on which this model is defined."""
+    ordinate: _Ordinate
+    """The ordinate that this model maps its domain to."""
     params: Params
     """The parameters defined for this model"""
-    model_dtype: type | np.dtype
-    """The datatype used to represent the model"""
-
-    domain: np.ndarray
-    """The domain on which the model will be defined"""
-
-    n_domain: int
-    """The number of elements in the domain"""
 
     def __init__(self, model: str):
 
         # Keep track of the model string so we can reinstantiate from a saved state
         self.model_str = model
-        self.model_basename = self.model_str.split(":")[0].split(".")[-1]
-
-        # Run an optional cache() method
-        self.cache()
+        self.basename = self.model_str.split(":")[0].split(".")[-1]
 
         # Initialise the domain
-        self.domain = self.set_domain()
-        self.n_domain = len(self.domain)
+        self.domain = self.coordinate.get()
+        self.n_domain = len(self.coordinate)
 
         # Check that the domain has been suitably set
         assert self.n_domain > 0
 
         # Check that at least one parameter has beed defined
         if self.params.count <= 0:
             raise exceptions.RombusModelParamsError(
                 f"Invalid number of parameters ({self.params.count}) specified for Rombus model ({self})."
             )
 
     def __str__(self):
         return f"<RombusModel from {self.model_str}>"
 
     @abstractmethod  # make sure this is the inner-most decorator
-    def set_domain(self) -> np.ndarray:
-        """Abstract method which sets the domain on which the ROM will be defined.
-
-        Returns
-        -------
-        np.ndarray
-            Numpy array on which the ROM will be defined.
-        """
-        pass
-
-    @abstractmethod  # make sure this is the inner-most decorator
     def compute(self, params: NamedTuple, domain: np.ndarray) -> np.ndarray:
         """Abstract method which computes the user's model.
 
         This method does all the work of computing the user's model.  It takes a parameter set as a named tuple
         with N elements given by the names given to the N calls made to params.add() as well as the array set
-        by self.set_domain() and returns a numpy array.
+        by coordinate.set() and returns a numpy array.
 
         Parameters
         ----------
         params : NamedTuple
             The parameters to be used when computing the model
         domain : np.ndarray
             The domain on which the model is to be computed
@@ -120,20 +180,14 @@
         Returns
         -------
         np.ndarray
             The user's model, computed for the given parameter set and domain
         """
         pass
 
-    def cache(self):
-        """This method gets called once before any calls to compute().  Users can override this method and add
-        members to the class which will be available in compute().  This provides a way to perform expensive
-        one-time calculations, reducing runtime."""
-        pass
-
     @classmethod
     @log.callable("Instantiating model from file")
     def from_file(cls, file_in: hdf5.FileOrFilename) -> Self:
         """Generate a RombusModel instance from a Rombus HDF5 file.
 
         Parameters
         ----------
@@ -213,20 +267,20 @@
         Returns
         -------
         np.ndarray
             An array of model results: 1 for each given sample.
         """
 
         my_ts: np.ndarray = np.zeros(
-            shape=(samples.n_samples, self.n_domain), dtype=self.model_dtype
+            shape=(samples.n_samples, self.n_domain), dtype=self.ordinate.dtype
         )
         with log.progress("Generating training set", samples.n_samples) as progress:
             for i, params_numpy in enumerate(samples.samples):
                 model_i = self.compute(self.params.np2param(params_numpy), self.domain)
-                my_ts[i] = model_i / np.sqrt(np.vdot(model_i, model_i))
+                my_ts[i] = model_i / np.sqrt(np.vdot(model_i, model_i).real)
                 progress.update(i)
 
         return my_ts
 
     def parse_cli_params(self, args: Tuple[str, ...]) -> Dict[str, Any]:
         """Parse parameters given as a tuple of form 'param0=val0', 'param1=val1', ... etc to a dictionary of
         form {'param0':val0, 'param1':val1, ... }.
@@ -291,15 +345,16 @@
         Returns
         -------
         float
             Seconds elapsed
         """
 
         with log.context(
-            f"Computing timing information for model using {samples.n_samples} samples"
+            f"Computing timing information for model using {samples.n_samples} samples",
+            time_elapsed=False,
         ):
             start_time = timeit.default_timer()
             for i, sample in enumerate(samples.samples):
                 params_numpy = self.params.np2param(sample)
                 _ = self.compute(params_numpy, self.domain)
         return timeit.default_timer() - start_time
```

### Comparing `rombus-1.0.5/python/rombus/models/PhenomP.py` & `rombus-1.0.6/python/rombus/models/PhenomP.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,48 +3,47 @@
 import lal  # type: ignore
 import lalsimulation  # type: ignore
 import numpy as np
 
 from rombus.model import RombusModel
 
 
-class model(RombusModel):
+class Model(RombusModel):
 
-    model_dtype = complex
+    # Set some constants
+    l_1 = 0
+    l_2 = 0
+    f_min = 20.0
+    f_max = 1024.0
+    delta_F = 1.0 / 4.0
+    n_f = int((f_max - f_min) / delta_F) + 1
+    f_min_index = int(f_min / delta_F)
+    WFdict = lal.CreateDict()
+
+    # Set the domain over-and-on which the ROM will be defined
+    coordinate.set("f", f_min, f_max, n_f, label="$f$", dtype=np.dtype("float64"))  # type: ignore # noqa F821
+
+    # Set the ordinate the model will map the domain to
+    ordinate.set("h", label="$h$", dtype=complex)  # type: ignore # noqa F821
 
     # N.B.: mypy struggles with NamedTuples, so typing is turned off for the following
     params.add("m1", 30, 35)  # type: ignore # noqa F821
     params.add("m2", 30, 35)  # type: ignore # noqa F821
     params.add("chi1L", 0, 0.1)  # type: ignore # noqa F821
     params.add("chi2L", 0, 0.1)  # type: ignore # noqa F821
     params.add("chip", 0, 0.1)  # type: ignore # noqa F821
     params.add("thetaJ", -np.pi / 2, np.pi / 2)  # type: ignore # noqa F821
     params.add("alpha", 0, np.pi / 2)  # type: ignore # noqa F821
     params.set_validation(lambda p: p.m1 >= p.m2)  # type: ignore # noqa F821
 
-    def cache(self):
-        self.l1 = 0
-        self.l2 = 0
-        self.fmin = 20
-        self.fmax = 1024
-        self.deltaF = 1.0 / 4.0
-        self.nf = int((self.fmax - self.fmin) / self.deltaF) + 1
-        self.fseries = np.linspace(self.fmin, self.fmax, self.nf)
-        self.fmin_index = int(self.fmin / self.deltaF)
-        self.WFdict = lal.CreateDict()
-
-    def set_domain(self) -> np.ndarray:
-        return self.fseries
-
     def compute(self, params: NamedTuple, domain: np.ndarray) -> np.ndarray:
 
-        lalsimulation.SimInspiralWaveformParamsInsertTidalLambda1(self.WFdict, self.l1)
-        lalsimulation.SimInspiralWaveformParamsInsertTidalLambda2(self.WFdict, self.l2)
-
-        if not np.array_equiv(domain, self.fseries):
+        lalsimulation.SimInspiralWaveformParamsInsertTidalLambda1(self.WFdict, self.l_1)
+        lalsimulation.SimInspiralWaveformParamsInsertTidalLambda2(self.WFdict, self.l_2)
+        if not np.array_equiv(domain, self.domain):
             h = lalsimulation.SimIMRPhenomPFrequencySequence(
                 domain,
                 params.chi1L,  # type: ignore
                 params.chi2L,  # type: ignore
                 params.chip,  # type: ignore
                 params.thetaJ,  # type: ignore
                 params.m1 * lal.lal.MSUN_SI,  # type: ignore
@@ -65,20 +64,20 @@
                 params.chip,  # type: ignore
                 params.thetaJ,  # type: ignore
                 params.m1 * lal.lal.MSUN_SI,  # type: ignore
                 params.m2 * lal.lal.MSUN_SI,  # type: ignore
                 1e6 * lal.lal.PC_SI * 100,
                 params.alpha,  # type: ignore
                 0,
-                self.deltaF,
-                self.fmin,
-                self.fmax,
+                self.delta_F,
+                self.f_min,
+                self.f_max,
                 40,
                 lalsimulation.IMRPhenomPv2NRTidal_V,
                 lalsimulation.NRTidalv2_V,
                 self.WFdict,
             )
-            h = h[0].data.data[self.fmin_index : len(h[0].data.data)]
-            if len(h) < self.nf:
-                h = np.append(h, np.zeros(self.nf - len(h), dtype=complex))
+            h = h[0].data.data[self.f_min_index : len(h[0].data.data)]
+            if len(h) < self.n_domain:
+                h = np.append(h, np.zeros(self.n_domain - len(h), dtype=complex))
 
         return h
```

### Comparing `rombus-1.0.5/python/rombus/models/PhenomP_samples.csv` & `rombus-1.0.6/python/rombus/models/PhenomP_samples.csv`

 * *Files identical despite different names*

### Comparing `rombus-1.0.5/python/rombus/models/sinc.py` & `rombus-1.0.6/python/rombus/models/sinc.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,54 +3,58 @@
 from typing import NamedTuple
 import math
 
 # This sample code provides a starting point for building your own Reduced Order Models
 # Edit it to suit your needs.  In its initial form, it provides a model for building
 # a reduced order model (ROM) of the function sinc(x)=sin(x)/x
 
-# The following class is the essential element needed to define a model for RombusModel
-# It must inherit from the RombusModel Class (which needs to be imported above).  The class
-# must include one-or-more calls to 'params.add_param()' to define the names and limits of
-# the parameters of the model and define the following methods:
+# *** The following class demonstrates the elements needed to define a model for Rombus ***
 #
-#   1) set_domain(): sets the domain over-and-on which the ROM will be defined
-#
-#   2) compute(): returns a model for a given parameter set for each value of domain
-#
-class model(RombusModel):
+# It must do the following:
+#    1. inherit from the RombusModel Class (which is imported above);
+#    2. call `coordinate.set()` to define the domain on which the ROM will be defined;
+#    3. call `ordinate.set()` to define the name and type of the space the model will
+#       map the domain onto
+#    4. include one-or-more calls to 'params.add_param()' to define the names and
+#       limits of the parameters of the model; over-and-on
+#    5. define a 'compute' method which takes a parameter set as a named tuple, a
+#       domain specified as a numpy array, and returns a numpy array of the type
+#       specified by `ordinate.set()`.
+
+
+class Model(RombusModel):
     """Class for creating a ROM for the function sinc(x)=sin(x)/x"""
 
-    # This sets the datatype generated by the model (default: 'float64')
-    model_dtype = np.dtype("float64")
+    # Set the domain over-and-on which the ROM will be defined
+    # coordinate.set() takes a name, a minimum value, a maximum value,
+    # an integer number of values and optional keyword values 'label' -
+    # which is used for plots, etc. - and dtype, which must match the type
+    # of min_value and max_value
+    coordinate.set("x", 0.0, 100.0, 1024, label="$x$", dtype=np.dtype("float64"))  # type: ignore # noqa F821
+
+    # Set the ordinate the model will map the domain to
+    # ordinate.set() takes a name and optional keyword values 'label' -
+    # which is used for plots, etc. - and dtype, which must match the type
+    # returned by the compute() method defined below.
+    ordinate.set("y", label="$sinc(x)$", dtype=np.dtype("float64"))  # type: ignore # noqa F821
 
     # Add as many calls to params.add() as your model has parameters.
     # Samples will be sent to the 'compute()' method (see below) as
     # named tuples and will be addressable using the names you give them.
     #
     # Note that you may need to silence linting errors by adding a '# noqa F821'
     # directive at the end.  params is initialised, it's just done in a way that
     # IDEs and linters have troubles following.
     #
     # Syntax: params.add(name, min_value_allowed,max_value_allowed)
     params.add("A", 0, 10)  # type: ignore # noqa F821
 
-    # Anything added as a class member here will just be computed once and will
-    # be accessible in the 'compute()' and 'set-domain()' methods below.
-    def cache(self):
-        self.x_min = 0
-        self.x_max = 100
-        self.n_x = 1024
-
-    # Set the domain over-and-on which the ROM will be defined
-    def set_domain(self) -> np.ndarray:
-        return np.linspace(self.x_min, self.x_max, self.n_x)
-
     # Compute the model.  This function should accept a named tuple with
-    # member names given by the params.add() calls above and iter should
-    # return a numpy array of type given my 'model_dtype' given above
+    # member names given by the params.add() calls above and should
+    # return a numpy array of type given my ordinate.set() above
     def compute(self, params: NamedTuple, x) -> np.ndarray:
         """Compute the model for a given parameter set."""
 
         return sinc_vectorized(params.A * x)  # type: ignore
 
 
 # Create the function that will compute our model
@@ -61,10 +65,10 @@
     if x == 0.0:
         return 1.0
     else:
         return math.sin(x) / x
 
 
 # Use np.vectorize() to create a function that accepts a
-# numpy array and returns a numpy array.  This will be them
-# function that Rombus actually calls to compute the model
+# numpy array and returns a numpy array.  This will be the
+# function the model calls to do the actual work
 sinc_vectorized = np.vectorize(sinc_scalar)
```

### Comparing `rombus-1.0.5/python/rombus/params.py` & `rombus-1.0.6/python/rombus/params.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,23 +29,24 @@
             The minimum-allowed value for this parameter
         range_max : float
             The maximum-allowed value for this parameter
         dtype : type
             The datatype used to represent this parameter
         """
 
-        # N.B.: mypy struggles with NamedTuples, so typing is turned off for the following
-        Param = NamedTuple(f"Param{len(self.params)}", [("name", str), ("min", dtype), ("max", dtype), ("dtype", dtype)])  # type: ignore
-        self.params.append(Param(name, dtype(range_min), dtype(range_max), dtype))  # type: ignore
-        self.count = self.count + 1
-        self.names.append(name)
+        with log.context(f"Adding parameter ({name})"):
+            # N.B.: mypy struggles with NamedTuples, so typing is turned off for the following
+            Param = NamedTuple(f"Param{len(self.params)}", [("name", str), ("min", dtype), ("max", dtype), ("dtype", dtype)])  # type: ignore
+            self.params.append(Param(name, dtype(range_min), dtype(range_max), dtype))  # type: ignore
+            self.count = self.count + 1
+            self.names.append(name)
 
-        # Update the named tuple that will be used to convert numpy arrays to Param objects
-        # N.B.: mypy struggles with NamedTuples, so typing is turned off for the following
-        self.params_dtype = NamedTuple("params_dtype", [(name, dtype) for name in self.names])  # type: ignore
+            # Update the named tuple that will be used to convert numpy arrays to Param objects
+            # N.B.: mypy struggles with NamedTuples, so typing is turned off for the following
+            self.params_dtype = NamedTuple("params_dtype", [(name, dtype) for name in self.names])  # type: ignore
 
     def set_validation(self, func: Callable[[NamedTuple], bool]) -> None:
         """Specify a callable which accepts a parameter set (in the form of a NamedTuple) and
         returns a bool indicating if the parameter set is valid.
 
         By default, no validation is performed and all passed samples are assumed to be valid.
```

### Comparing `rombus-1.0.5/python/rombus/plots.py` & `rombus-1.0.6/python/rombus/plots.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,64 @@
 import numpy as np
 
-from typing import Any, Dict, List
+from typing import Any, Dict
 
 import pylab as plt  # type: ignore
 
 import rombus.exceptions as exceptions
 from rombus.rom import ReducedOrderModel
 from rombus._core.log import log
 
+import warnings
 
-def errors(err_list: List[float]) -> None:
+warnings.simplefilter("ignore", np.ComplexWarning)
+
+
+def bases_errors(ROM: ReducedOrderModel) -> None:
     """Generate plot of errors.
 
     Parameters
     ----------
     err_list : List[float]
         List of errors
     """
 
-    filename_out = "basis_error.png"
+    filename_out = f"{ROM.basename}_bases_errors.pdf"
 
     with log.context("Generating plot of errors"):
+        if ROM is None or ROM.reduced_basis is None:
+            raise exceptions.RombusPlotError(
+                "Basis plots can not be generated for uninitialised ROM."
+            )
+        err_list = ROM.reduced_basis.error_list
         plt.plot(err_list)
         plt.xlabel("# Basis elements")
         plt.ylabel("Error")
         plt.yscale("log")
         plt.tight_layout()
         plt.savefig(filename_out)
         log.append(f"written to {filename_out}")
 
 
-def basis(rb_matrix: List[np.ndarray]) -> None:
+def bases(ROM: ReducedOrderModel) -> None:
     """Generate a plot of the Reduced Bases.
 
     Parameters
     ----------
     rb_matrix : List[np.ndarray]
         List of reduced bases
     """
-    filename_out = "basis.png"
+    filename_out = f"{ROM.basename}_bases.pdf"
 
-    with log.context("Generating plot of errors"):
+    with log.context("Generating plot of bases"):
+        if ROM is None or ROM.reduced_basis is None:
+            raise exceptions.RombusPlotError(
+                "Basis plots can not be generated for uninitialised ROM."
+            )
+        rb_matrix = ROM.reduced_basis.matrix
         num_elements = len(rb_matrix)
         total_frames = 125
         n_models_per_frame = int(num_elements / total_frames)
         if n_models_per_frame < 1:
             n_models_per_frame = 1
         fig, ax = plt.subplots(total_frames, 1, figsize=(4.5, 2.5 * total_frames))
         for i in range(total_frames):
@@ -69,15 +83,16 @@
     ----------
     ROM : ReducedOrderModel
         The Reduced Order Model to make the comparison for
     model_params_in : Dict[str, Any]
         A dictionary of parameters to use as the input parameters
     """
 
-    filename_out = "comparison.png"
+    filename_out = f"{ROM.basename}_comparison.pdf"
+    filename_diff_out = f"{ROM.basename}_ROM_diff"
 
     with log.context("Generating comparison plot"):
         if ROM.model is None or ROM.empirical_interpolant is None:
             raise exceptions.RomNotInitialised(
                 "ROM not initialised when generating comparison plot."
             )
         else:
@@ -96,15 +111,17 @@
                 )
             else:
                 model_nodes = ROM.model.compute(
                     model_params, ROM.empirical_interpolant.nodes
                 )
                 model_rom = ROM.evaluate(model_params)
 
+                plt.xlabel(ROM.model.coordinate.label)
+                plt.ylabel(ROM.model.ordinate.label)
                 plt.semilogx(domain, model_rom, label="ROM", alpha=0.5, linestyle="--")
                 plt.semilogx(domain, model_full, label="Full model", alpha=0.5)
                 plt.scatter(ROM.empirical_interpolant.nodes, model_nodes, s=1)
                 plt.legend()
 
-                np.save("ROM_diff", np.subtract(model_rom, model_full))
+                np.save(filename_diff_out, np.subtract(model_rom, model_full))
                 plt.savefig(filename_out, bbox_inches="tight")
                 log.append(f"written to {filename_out}")
```

### Comparing `rombus-1.0.5/python/rombus/reduced_basis.py` & `rombus-1.0.6/python/rombus/reduced_basis.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,26 +125,29 @@
             pc_matrix: List[np.ndarray] = []
             while error > tol:
                 self.matrix, pc_matrix, error_data = self._add_next_model_to_basis(
                     pc_matrix, my_ts, iter
                 )
                 self.matrix_shape[0] = len(self.matrix)
                 err_rnk, err_idx, error = error_data
+
+                # Set a sensible starting value for the progress counter
+                log10_error = log10(max(tol, error))
                 if iter == 1:
-                    progress.reset_next(error)
+                    progress.reset_next(log10_error)
 
                 basis_index = self._convert_to_basis_index(
                     err_rnk, err_idx, samples.n_samples
                 )
                 self.error_list.append(error)
                 basis_indicies.append(basis_index)
 
                 # update iteration count
                 iter += 1
-                progress.update(log10(error))
+                progress.update(log10_error)
 
         self.greedypoints = [samples.samples[i] for i in basis_indicies]
 
         return self
 
     def write(self, h5file: hdf5.File) -> None:
         """Save reduced basis to file.
@@ -241,15 +244,15 @@
             next_vec -= self.matrix[i] * L2
         norm = np.sqrt(np.vdot(next_vec, next_vec))
         next_vec /= norm
         return next_vec, norm
 
     def _project_onto_basis(self, integration_weights, my_ts, iter):
 
-        pc = np.zeros(len(my_ts), dtype=self.model.model_dtype)
+        pc = np.zeros(len(my_ts), dtype=self.model.ordinate.dtype)
         for j in range(len(my_ts)):
             pc[j] = _dot_product(integration_weights, self.matrix[iter], my_ts[j])
         return pc
 
     def _convert_to_basis_index(self, rank_number, rank_idx, rank_count):
         ranks_till_err_rank = [i for i in range(rank_number)]
         idx_till_err_rank = np.sum([rank_count[i] for i in ranks_till_err_rank])
```

### Comparing `rombus-1.0.5/python/rombus/rom.py` & `rombus-1.0.6/python/rombus/rom.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import timeit
 
 
 import h5py  # type: ignore
 import mpi4py
 import numpy as np
 
@@ -25,14 +26,15 @@
 
     def __init__(
         self,
         model: RombusModelType,
         samples: Samples,
         reduced_basis: Optional[ReducedBasis] = None,
         empirical_interpolant: Optional[EmpiricalInterpolant] = None,
+        basename: Optional[str] = None,
         tol: float = DEFAULT_TOLERANCE,
     ):
 
         self.model: RombusModel = RombusModel.load(model)
         """Model used to generate the ROM"""
 
         self.samples = samples
@@ -40,14 +42,19 @@
 
         self.reduced_basis = reduced_basis
         """ReducedBasis generated for the ROM"""
 
         self.empirical_interpolant = empirical_interpolant
         """EmpiricalInterpolant generated for the ROM"""
 
+        if basename is None:
+            basename = model.basename
+        self.basename = basename
+        """Set when reading from files and provides a base name for writing plots to file, etc."""
+
     @classmethod
     @log.callable("Instantiating ROM from file")
     def from_file(cls, file_in: hdf5.FileOrFilename) -> Self:
         """Instantiate a ROM from a Rombus HDF5 file.
 
         Parameters
         ----------
@@ -65,22 +72,25 @@
         model: RombusModel = RombusModel.from_file(h5file)
         samples: Samples = Samples.from_file(h5file)
         reduced_basis: ReducedBasis = ReducedBasis.from_file(h5file)
         empirical_interpolant: EmpiricalInterpolant = EmpiricalInterpolant.from_file(
             h5file
         )
 
+        basename = os.path.splitext(os.path.basename(h5file.filename))[0]
+
         if close_file:
             h5file.close()
 
         return cls(
             model,
             samples,
             reduced_basis=reduced_basis,
             empirical_interpolant=empirical_interpolant,
+            basename=basename,
         )
 
     @log.callable("Building ROM")
     def build(
         self, do_step: Optional[str] = None, tol: float = DEFAULT_TOLERANCE
     ) -> Self:
         """(Re)build a ReducedOrderModel.
@@ -202,15 +212,16 @@
         Returns
         -------
         float
             Seconds elapsed
         """
 
         with log.context(
-            f"Computing timing information for ROM using {samples.n_samples} samples"
+            f"Computing timing information for ROM using {samples.n_samples} samples",
+            time_elapsed=False,
         ):
             start_time = timeit.default_timer()
             for i, sample in enumerate(samples.samples):
                 params_numpy = self.model.params.np2param(sample)
                 _ = self.evaluate(params_numpy)
         return timeit.default_timer() - start_time
 
@@ -247,15 +258,15 @@
                 new_samples = Samples(self.model, n_random=n_random)
                 my_vs = self.model.generate_model_set(new_samples)
 
                 # test validation set
                 RB_transpose = np.transpose(self.reduced_basis.matrix)
                 selected_greedy_points = []
                 for i, validation_sample in enumerate(new_samples.samples):
-                    if self.model.model_dtype == complex:
+                    if self.model.ordinate.dtype == complex:
                         proj_error = 1 - np.sum(
                             [
                                 np.real(np.conjugate(d_i) * d_i)
                                 for d_i in np.dot(my_vs[i], RB_transpose)
                             ]
                         )
                     else:
```

### Comparing `rombus-1.0.5/python/rombus/samples.py` & `rombus-1.0.6/python/rombus/samples.py`

 * *Files identical despite different names*

### Comparing `rombus-1.0.5/python/rombus/tests/test_PhenomP.py` & `rombus-1.0.6/python/rombus/tests/test_PhenomP.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import numpy as np
 import importlib
 import pytest
 from click.testing import CliRunner
 
 from rombus.cli import cli
 
+import warnings
+
+warnings.simplefilter("ignore", np.ComplexWarning)
+
 
 @pytest.mark.lalsuite
 def test_PhenomP(tmp_path):
 
     atol = 1e-12
     rtol = 1e-12
 
@@ -18,15 +22,15 @@
         greedy_filename = str(
             importlib.resources.files("rombus.models").joinpath("PhenomP_samples.csv")
         )
         result = runner.invoke(
             cli,
             [
                 "build",
-                "rombus.models.PhenomP:model",
+                "rombus.models.PhenomP:Model",
                 greedy_filename,
             ],
         )
         assert result.exit_code == 0
         result = runner.invoke(
             cli,
             [
@@ -38,10 +42,10 @@
                 "chi2L=0.266269755913278",
                 "chip=0.5458029422691579",
                 "thetaJ=1.7621026471916568",
                 "alpha=2.765791991075064",
             ],
         )
         assert result.exit_code == 0
-        delta_diff = np.load("ROM_diff.npy")
+        delta_diff = np.load("PhenomP_ROM_diff.npy")
 
     assert np.allclose(delta_diff, 0.0, rtol=rtol, atol=atol)
```

### Comparing `rombus-1.0.5/PKG-INFO` & `rombus-1.0.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rombus
-Version: 1.0.5
+Version: 1.0.6
 Summary: Reduced order modeling for the masses
 Home-page: https://github.com/ADACS-Australia/rombus
 License: MIT-expat
 Author: Gregory Poole
 Author-email: gbpoole@gmail.com
 Requires-Python: >=3.11
 Classifier: License :: Other/Proprietary License
@@ -34,32 +34,36 @@
 
 Rombus: Helps you qucikly and easily compute slow and complex models
 ====================================================================
 
 Rombus is a tool for building reduced order models (ROMs): matrix representations of arbitrary
 models which can be rapidly and easily computed for arbitrary parameter sets.
 
-Building a ROM with Rombus is easy.  All you need to do is define your model like this (in this trivial case, a file named `my_model.py` specifying a simple second-order polynomial):
+Building a ROM with Rombus is easy.  All you need to do is install it like so:
+```console
+$ pip install rombus
 ```
+define your model like this (in this trivial case, a file named `my_model.py` specifying a simple second-order polynomial):
+``` python
 from numpy import ndarray, polyval, linspace
 from rombus.model import RombusModel
 from typing import NamedTuple
 
 
-class model(RombusModel):
-    """Class for creating a ROM for the function y=a2*x^2+a1*x+a0"""
+class Model(RombusModel):
+    """Class for creating a ROM for the function y(x)=a2*x^2+a1*x+a0"""
+
+    coordinate.set("x", 0.0, 10.0, 11, label="$x$")
+
+    ordinate.set("y", label="$y(x)$")
 
     params.add("a0", -10, 10)
     params.add("a1", -10, 10)
     params.add("a2", -10, 10)
 
-    # Set the domain over-and-on which the ROM will be defined
-    def set_domain(self) -> ndarray:
-        return linspace(0, 10, 11)
-
     def compute(self, p: NamedTuple, x: ndarray) -> ndarray:
         """Compute the model for a given parameter set."""
         return polyval([p.a2, p.a1, p.a0], x)
 ```
 and specify a set of points (in this case, the file `my_model_samples.py`) to build your ROM from:
 ```
 -10, -10,-10
@@ -69,35 +73,34 @@
  10, -10,-10
  10,  10,-10
  10, -10, 10
  10,  10, 10
 ```
 You build your ROM like this:
 ```
-$ rombus build my_model:model my_model_samples.csv
+$ rombus build my_model:Model my_model_samples.csv
 ```
-This produces an _HDF5_ file named `my_model.hdf5`.  You can then use your new ROM in
-your Python projects like this:
+This produces an _HDF5_ file named `my_model.hdf5`.  You can then use your new ROM in your Python projects like this:
 ```
 from rombus.rom import ReducedOrderModel
 
 ROM = ReducedOrderModel.from_file('my_model.hdf5')
 sample = ROM.model.sample({"a0":0,"a1":0,"a2":1})
 model_ROM = ROM.evaluate(sample)
 for x, y in zip(ROM.model.domain,model_ROM):
-    print(f"{x:.2f} {y:.2f}")
+    print(f"{x:5.2f} {y:6.2f}")
 ```
 which generates the output:
 ```
-0.00 0.00
-1.00 1.00
-2.00 4.00
-3.00 9.00
-4.00 16.00
-5.00 25.00
-6.00 36.00
-7.00 49.00
-8.00 64.00
-9.00 81.00
+ 0.00   0.00
+ 1.00   1.00
+ 2.00   4.00
+ 3.00   9.00
+ 4.00  16.00
+ 5.00  25.00
+ 6.00  36.00
+ 7.00  49.00
+ 8.00  64.00
+ 9.00  81.00
 10.00 100.00
 ```
```


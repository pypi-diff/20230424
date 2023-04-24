# Comparing `tmp/quera-ahs-utils-0.3.2.tar.gz` & `tmp/quera-ahs-utils-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quera-ahs-utils-0.3.2.tar", last modified: Fri Apr 14 15:55:55 2023, max compression
+gzip compressed data, was "quera-ahs-utils-0.4.0.tar", last modified: Mon Apr 24 04:44:52 2023, max compression
```

## Comparing `quera-ahs-utils-0.3.2.tar` & `quera-ahs-utils-0.4.0.tar`

### file list

```diff
@@ -1,32 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:55:55.692035 quera-ahs-utils-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-14 15:55:55.692035 quera-ahs-utils-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-14 15:55:55.692035 quera-ahs-utils-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:55:55.688035 quera-ahs-utils-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:55:55.688035 quera-ahs-utils-0.3.2/src/quera_ahs_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/src/quera_ahs_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/src/quera_ahs_utils/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/src/quera_ahs_utils/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    14705 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/src/quera_ahs_utils/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     9226 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/src/quera_ahs_utils/ir.py
--rw-r--r--   0 runner    (1001) docker     (123)    11676 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/src/quera_ahs_utils/parallelize.py
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/src/quera_ahs_utils/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:55:55.692035 quera-ahs-utils-0.3.2/src/quera_ahs_utils/quera_ir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/src/quera_ahs_utils/quera_ir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/src/quera_ahs_utils/quera_ir/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/src/quera_ahs_utils/quera_ir/task_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/src/quera_ahs_utils/quera_ir/task_specification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:55:55.688035 quera-ahs-utils-0.3.2/src/quera_ahs_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-14 15:55:55.000000 quera-ahs-utils-0.3.2/src/quera_ahs_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-14 15:55:55.000000 quera-ahs-utils-0.3.2/src/quera_ahs_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:55:55.000000 quera-ahs-utils-0.3.2/src/quera_ahs_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-14 15:55:55.000000 quera-ahs-utils-0.3.2/src/quera_ahs_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 15:55:55.000000 quera-ahs-utils-0.3.2/src/quera_ahs_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:55:55.692035 quera-ahs-utils-0.3.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/test/test_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/test/test_ir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/test/test_parallelize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-14 15:55:09.000000 quera-ahs-utils-0.3.2/test/test_plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 04:44:52.190166 quera-ahs-utils-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-04-24 04:43:45.000000 quera-ahs-utils-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-24 04:44:52.190166 quera-ahs-utils-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-24 04:43:45.000000 quera-ahs-utils-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-24 04:43:45.000000 quera-ahs-utils-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 04:44:52.190166 quera-ahs-utils-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 04:44:52.186166 quera-ahs-utils-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 04:44:52.190166 quera-ahs-utils-0.4.0/src/quera_ahs_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-24 04:43:45.000000 quera-ahs-utils-0.4.0/src/quera_ahs_utils/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-04-24 04:43:45.000000 quera-ahs-utils-0.4.0/src/quera_ahs_utils/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9226 2023-04-24 04:43:45.000000 quera-ahs-utils-0.4.0/src/quera_ahs_utils/ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11676 2023-04-24 04:43:45.000000 quera-ahs-utils-0.4.0/src/quera_ahs_utils/parallelize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-04-24 04:43:45.000000 quera-ahs-utils-0.4.0/src/quera_ahs_utils/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 04:44:52.190166 quera-ahs-utils-0.4.0/src/quera_ahs_utils/quera_ir/
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-24 04:43:45.000000 quera-ahs-utils-0.4.0/src/quera_ahs_utils/quera_ir/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-04-24 04:43:45.000000 quera-ahs-utils-0.4.0/src/quera_ahs_utils/quera_ir/task_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-04-24 04:43:45.000000 quera-ahs-utils-0.4.0/src/quera_ahs_utils/quera_ir/task_specification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 04:44:52.190166 quera-ahs-utils-0.4.0/src/quera_ahs_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-24 04:44:52.000000 quera-ahs-utils-0.4.0/src/quera_ahs_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-24 04:44:52.000000 quera-ahs-utils-0.4.0/src/quera_ahs_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 04:44:52.000000 quera-ahs-utils-0.4.0/src/quera_ahs_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-24 04:44:52.000000 quera-ahs-utils-0.4.0/src/quera_ahs_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-24 04:44:52.000000 quera-ahs-utils-0.4.0/src/quera_ahs_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 04:44:52.190166 quera-ahs-utils-0.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-24 04:43:45.000000 quera-ahs-utils-0.4.0/test/test_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-24 04:43:45.000000 quera-ahs-utils-0.4.0/test/test_ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-24 04:43:45.000000 quera-ahs-utils-0.4.0/test/test_parallelize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-24 04:43:45.000000 quera-ahs-utils-0.4.0/test/test_plotting.py
```

### Comparing `quera-ahs-utils-0.3.2/LICENSE` & `quera-ahs-utils-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.3.2/PKG-INFO` & `quera-ahs-utils-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: quera-ahs-utils
-Version: 0.3.2
+Version: 0.4.0
 Summary: Various tools to interact with Braket Analog Hamiltonian Computing
-Home-page: https://github.com/QuEraComputing/quera-ahs-utils
-Author: QuEra Computing Inc. + Braket Science Team
 Author-email: Phillip Weinberg <pweinberg@quera.com>, John Long <jlong@quera.com>
 Maintainer-email: Phillip Weinberg <pweinberg@quera.com>, John Long <jlong@quera.com>
 Project-URL: Homepage, https://github.com/QuEraComputing/quera-ahs-utils
 Project-URL: Bug Tracker, https://github.com/QuEraComputing/quera-ahs-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # quera-ahs-utils
 This python package is a collection of tools that can be used to program QuEra's **neutral atom Analog Hamiltonian Simulator** (**ahs**). These tools are primarily targeted towards the usage of [Amazon's Braket quantum computing service](https://aws.amazon.com/braket/). The Braket Python SDK can be found [here](https://github.com/aws/amazon-braket-sdk-python) along with some examples of how to use their service through a collection of examples from both [Braket](https://github.com/aws/amazon-braket-examples/tree/main/examples/analog_hamiltonian_simulation) and [QuEra](https://github.com/QuEraComputing/QuEra-braket-examples).
 
 Some of the source code contained in this package originates from [this](https://github.com/aws/amazon-braket-examples/blob/main/examples/analog_hamiltonian_simulation/ahs_utils.py) module which was co-authered by the Braket science team.
```

### Comparing `quera-ahs-utils-0.3.2/README.md` & `quera-ahs-utils-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.3.2/pyproject.toml` & `quera-ahs-utils-0.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quera-ahs-utils"
-version = "0.3.2"
+version = "0.4.0"
 authors = [
   { name="Phillip Weinberg", email="pweinberg@quera.com" },
   { name="John Long", email="jlong@quera.com" }
 ]
 maintainers = [
   { name="Phillip Weinberg", email="pweinberg@quera.com" },
   { name="John Long", email="jlong@quera.com" }
 ]
 description = "Various tools to interact with Braket Analog Hamiltonian Computing"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+  "amazon-braket-sdk",
+  "networkx",
+  "numpy",
+  "scipy",
+  "matplotlib",
+  "pydantic",
+]
 
 [project.urls]
 "Homepage" = "https://github.com/QuEraComputing/quera-ahs-utils"
-"Bug Tracker" = "https://github.com/QuEraComputing/quera-ahs-utils/issues"
+"Bug Tracker" = "https://github.com/QuEraComputing/quera-ahs-utils/issues"
+
+[tool.setuptools.packages.find]
+where = ["src"]
```

### Comparing `quera-ahs-utils-0.3.2/src/quera_ahs_utils/analysis.py` & `quera-ahs-utils-0.4.0/src/quera_ahs_utils/analysis.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.3.2/src/quera_ahs_utils/drive.py` & `quera-ahs-utils-0.4.0/src/quera_ahs_utils/drive.py`

 * *Files 12% similar despite different names*

```diff
@@ -138,28 +138,32 @@
     for t, v in zip(times, values):
         magnitude.put(t, v)
     shift = ShiftingField(Field(magnitude, Pattern(pattern)))
 
     return shift
 
 
-def get_time_series_value(time_series: TimeSeries, time: float, piecewise_constant: bool = False) -> float:
+def get_time_series_value(series: Union[TimeSeries,Field], time: float, piecewise_constant: bool = False) -> float:
     """obtain value of a time series at a specific time
 
     Args:
         time_series (TimeSeries): The `TimeSeries` object to sample from.
         time (float): The time point to sample `times_series` at. 
         piecewise_constant (bool, optional): Interpolate `time_series` assuming piecewise constant, 
             otherwise use piecewise linear. Defaults to False.
 
     Returns:
         float: the resulting sampled point. 
     """
-    times = time_series.times()
-    values = time_series.values()
+    if isinstance(series, TimeSeries):
+        times = series.times()
+        values = series.values()
+    elif isinstance(series, Field):
+        times = series.time_series.times()
+        values = series.time_series.values()
 
     if piecewise_constant:
         index = max(0, min(len(times) - 1, np.searchsorted(times, time, side="right") - 1))
         return values[index]
     else:
         return np.interp(
             time,
@@ -404,7 +408,87 @@
     amplitudes = [0, Omega_max, Omega_max, 0]
     
     return DrivingField(
         amplitude=time_series(times,amplitudes),
         detuning=time_series(times,detunings),
         phase=time_series([0,times[-1]],[0, 0])
     )
+
+
+def local_detuning_state_prep(register_state: List[int], local_detuning_max: float=150.0e6) -> Tuple[DrivingField, ShiftingField]:
+    """Generate the DrivingField and ShiftingField required to use local detuning to prepare the register in a product state. 
+
+    Args:
+        register_state (List[int]): The product state you would like to prepare
+        local_detuning_max (float, optional): The value of local detuning to apply to atoms which NOT to excit. Defaults to 150.0e6.
+
+    Raises:
+        ValueError: register_state must be a list of integers with values 0 or 1. 
+
+    Returns:
+        Tuple[DrivingField, ShiftingField]: the driving and shifting fields respectively that contains the pulses for the state preparation. 
+    """
+    
+    pattern = []
+    for state in register_state:
+        if state == 0:
+            pattern.append(1.0)
+        elif state == 1:
+            pattern.append(0.0)
+        else:
+            raise ValueError("`register_state` must be a list of integers with values 0 or 1 representing the ground and rydberg states respectively.")
+    
+    # initial ramp up of local detuning
+    ramp_up = time_series([0.0,0.07e-6],[0.0,local_detuning_max])
+    shifting_field_start = ShiftingField(
+        Field(
+            time_series=ramp_up,
+            pattern=Pattern(pattern)
+        )
+    )
+    
+    driving_field_start = DrivingField(
+        amplitude=constant_time_series(ramp_up, 0.0),
+        phase=constant_time_series(ramp_up, 0.0),
+        detuning=constant_time_series(ramp_up, 0.0)
+    )
+    
+    # resonant pi/2 pulse
+    amplitude_max =  14.28e6 # these parameters have a 
+    amplitude = time_series(
+        times = [0.0, 0.05e-6, 0.11e-6, 0.16e-6],
+        values = [0.0,amplitude_max, amplitude_max, 0.0]
+    )
+    
+    driving_field_middle = DrivingField(
+        amplitude=amplitude,
+        phase=constant_time_series(amplitude, 0.0),
+        detuning = constant_time_series(amplitude, 0.0)
+    )
+    
+    shifting_field_middle = ShiftingField(
+        Field(
+            time_series=constant_time_series(amplitude,local_detuning_max),
+            pattern=Pattern(pattern)
+        )
+    )
+    
+    # ramp down of local detuning
+    
+    ramp_down = time_series([0.0,0.07e-6],[local_detuning_max,0.0])
+    shifting_field_end = ShiftingField(
+        Field(
+            time_series=ramp_down,
+            pattern=Pattern(pattern)
+        )
+    )
+    
+    driving_field_end = DrivingField(
+        amplitude=constant_time_series(ramp_down, 0.0),
+        phase=constant_time_series(ramp_down, 0.0),
+        detuning=constant_time_series(ramp_down, 0.0)
+    )
+    
+    total_shifting_field=concatenate_shift_list([shifting_field_start, shifting_field_middle, shifting_field_end])
+    total_driving_field=concatenate_drive_list([driving_field_start, driving_field_middle, driving_field_end])
+    
+    return total_driving_field, total_shifting_field
```

### Comparing `quera-ahs-utils-0.3.2/src/quera_ahs_utils/ir.py` & `quera-ahs-utils-0.4.0/src/quera_ahs_utils/ir.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.3.2/src/quera_ahs_utils/parallelize.py` & `quera-ahs-utils-0.4.0/src/quera_ahs_utils/parallelize.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.3.2/src/quera_ahs_utils/plotting.py` & `quera-ahs-utils-0.4.0/src/quera_ahs_utils/plotting.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.3.2/src/quera_ahs_utils/quera_ir/capabilities.py` & `quera-ahs-utils-0.4.0/src/quera_ahs_utils/quera_ir/capabilities.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.3.2/src/quera_ahs_utils/quera_ir/task_specification.py` & `quera-ahs-utils-0.4.0/src/quera_ahs_utils/quera_ir/task_specification.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from quera_ahs_utils.quera_ir.capabilities import QuEraCapabilities
 
 
 __all__ = [
     "QuEraTaskSpecification"
 ]
 
+# TODO: add version to these models.
+
 FloatType = Union[Decimal, float]
 
 def discretize_list(list_of_values: list, resolution: FloatType):
     resolution = Decimal(str(float(resolution)))
     return [Decimal(value).quantize(resolution) for value in list_of_values]
 
 class GlobalField(BaseModel):
```

### Comparing `quera-ahs-utils-0.3.2/src/quera_ahs_utils.egg-info/PKG-INFO` & `quera-ahs-utils-0.4.0/src/quera_ahs_utils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: quera-ahs-utils
-Version: 0.3.2
+Version: 0.4.0
 Summary: Various tools to interact with Braket Analog Hamiltonian Computing
-Home-page: https://github.com/QuEraComputing/quera-ahs-utils
-Author: QuEra Computing Inc. + Braket Science Team
 Author-email: Phillip Weinberg <pweinberg@quera.com>, John Long <jlong@quera.com>
 Maintainer-email: Phillip Weinberg <pweinberg@quera.com>, John Long <jlong@quera.com>
 Project-URL: Homepage, https://github.com/QuEraComputing/quera-ahs-utils
 Project-URL: Bug Tracker, https://github.com/QuEraComputing/quera-ahs-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # quera-ahs-utils
 This python package is a collection of tools that can be used to program QuEra's **neutral atom Analog Hamiltonian Simulator** (**ahs**). These tools are primarily targeted towards the usage of [Amazon's Braket quantum computing service](https://aws.amazon.com/braket/). The Braket Python SDK can be found [here](https://github.com/aws/amazon-braket-sdk-python) along with some examples of how to use their service through a collection of examples from both [Braket](https://github.com/aws/amazon-braket-examples/tree/main/examples/analog_hamiltonian_simulation) and [QuEra](https://github.com/QuEraComputing/QuEra-braket-examples).
 
 Some of the source code contained in this package originates from [this](https://github.com/aws/amazon-braket-examples/blob/main/examples/analog_hamiltonian_simulation/ahs_utils.py) module which was co-authered by the Braket science team.
```

### Comparing `quera-ahs-utils-0.3.2/src/quera_ahs_utils.egg-info/SOURCES.txt` & `quera-ahs-utils-0.4.0/src/quera_ahs_utils.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 LICENSE
 README.md
 pyproject.toml
-setup.cfg
-setup.py
-src/quera_ahs_utils/__init__.py
-src/quera_ahs_utils/_version.py
 src/quera_ahs_utils/analysis.py
 src/quera_ahs_utils/drive.py
 src/quera_ahs_utils/ir.py
 src/quera_ahs_utils/parallelize.py
 src/quera_ahs_utils/plotting.py
 src/quera_ahs_utils.egg-info/PKG-INFO
 src/quera_ahs_utils.egg-info/SOURCES.txt
 src/quera_ahs_utils.egg-info/dependency_links.txt
 src/quera_ahs_utils.egg-info/requires.txt
 src/quera_ahs_utils.egg-info/top_level.txt
-src/quera_ahs_utils/quera_ir/__init__.py
 src/quera_ahs_utils/quera_ir/capabilities.py
 src/quera_ahs_utils/quera_ir/task_results.py
 src/quera_ahs_utils/quera_ir/task_specification.py
 test/test_drive.py
 test/test_ir.py
 test/test_parallelize.py
 test/test_plotting.py
```

### Comparing `quera-ahs-utils-0.3.2/test/test_drive.py` & `quera-ahs-utils-0.4.0/test/test_drive.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.3.2/test/test_ir.py` & `quera-ahs-utils-0.4.0/test/test_ir.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.3.2/test/test_parallelize.py` & `quera-ahs-utils-0.4.0/test/test_parallelize.py`

 * *Files identical despite different names*

### Comparing `quera-ahs-utils-0.3.2/test/test_plotting.py` & `quera-ahs-utils-0.4.0/test/test_plotting.py`

 * *Files identical despite different names*


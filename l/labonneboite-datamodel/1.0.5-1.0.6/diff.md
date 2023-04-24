# Comparing `tmp/labonneboite_datamodel-1.0.5.tar.gz` & `tmp/labonneboite_datamodel-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labonneboite_datamodel-1.0.5.tar", max compression
+gzip compressed data, was "labonneboite_datamodel-1.0.6.tar", max compression
```

## Comparing `labonneboite_datamodel-1.0.5.tar` & `labonneboite_datamodel-1.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      224 2023-04-04 13:45:03.269004 labonneboite_datamodel-1.0.5/labonneboite_datamodel/__init__.py
--rw-r--r--   0        0        0      697 2023-04-05 09:46:10.763862 labonneboite_datamodel-1.0.5/labonneboite_datamodel/crud.py
--rw-r--r--   0        0        0     2185 2023-04-05 09:46:10.763862 labonneboite_datamodel-1.0.5/labonneboite_datamodel/job.py
--rw-r--r--   0        0        0     7672 2023-04-06 11:40:38.459864 labonneboite_datamodel-1.0.5/labonneboite_datamodel/office.py
--rw-r--r--   0        0        0        0 2023-04-04 13:25:50.527619 labonneboite_datamodel-1.0.5/labonneboite_datamodel/tests/__init__.py
--rw-r--r--   0        0        0     3589 2023-04-06 09:31:09.039521 labonneboite_datamodel-1.0.5/labonneboite_datamodel/tests/data/test.csv
--rw-r--r--   0        0        0     1026 2023-04-04 13:25:50.531619 labonneboite_datamodel-1.0.5/labonneboite_datamodel/tests/test_job.py
--rw-r--r--   0        0        0     5612 2023-04-06 11:40:38.459864 labonneboite_datamodel-1.0.5/labonneboite_datamodel/tests/test_office.py
--rw-r--r--   0        0        0     1205 2023-04-06 11:43:57.658443 labonneboite_datamodel-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 labonneboite_datamodel-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0      224 2023-04-24 11:55:25.743704 labonneboite_datamodel-1.0.6/labonneboite_datamodel/__init__.py
+-rw-r--r--   0        0        0      697 2023-04-24 11:55:25.743704 labonneboite_datamodel-1.0.6/labonneboite_datamodel/crud.py
+-rw-r--r--   0        0        0     2022 2023-04-24 11:55:25.743704 labonneboite_datamodel-1.0.6/labonneboite_datamodel/job.py
+-rw-r--r--   0        0        0     7672 2023-04-24 11:55:25.743704 labonneboite_datamodel-1.0.6/labonneboite_datamodel/office.py
+-rw-r--r--   0        0        0        0 2023-04-24 11:55:25.743704 labonneboite_datamodel-1.0.6/labonneboite_datamodel/tests/__init__.py
+-rw-r--r--   0        0        0     3589 2023-04-24 11:55:25.743704 labonneboite_datamodel-1.0.6/labonneboite_datamodel/tests/data/test.csv
+-rw-r--r--   0        0        0      997 2023-04-24 11:55:25.743704 labonneboite_datamodel-1.0.6/labonneboite_datamodel/tests/test_job.py
+-rw-r--r--   0        0        0     5612 2023-04-24 11:55:25.743704 labonneboite_datamodel-1.0.6/labonneboite_datamodel/tests/test_office.py
+-rw-r--r--   0        0        0     1205 2023-04-24 11:56:38.875328 labonneboite_datamodel-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 labonneboite_datamodel-1.0.6/PKG-INFO
```

### Comparing `labonneboite_datamodel-1.0.5/labonneboite_datamodel/crud.py` & `labonneboite_datamodel-1.0.6/labonneboite_datamodel/crud.py`

 * *Files identical despite different names*

### Comparing `labonneboite_datamodel-1.0.5/labonneboite_datamodel/job.py` & `labonneboite_datamodel-1.0.6/labonneboite_datamodel/job.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,31 +35,29 @@
     hirings: int
 
     @validator("naf", pre=True)
     def is_naf(cls, v):
         """Validator for `naf`
 
         Rules:
-            - should be made up of 5 characters
-            - the first 4 values should be numeric
-            - the last value should be a letter
+            - should be made up of 2 numbers
 
         Raises:
             ValueError:
 
         """
-        error = "a NAF should be made up of 4 numbers and a letter"
-        if len(v) != 5:
-            raise ValueError(error)
+        error = "a NAF should be made up of 2 numbers"
+        v = str(v)
 
-        if not v[:4].isdigit():
+        if len(v) != 2:
             raise ValueError(error)
 
-        if v[-1].isdigit():
+        if not v.isdigit():
             raise ValueError(error)
+
         return v
 
     @validator("rome", pre=True)
     def is_rome(cls, v):
         """Validator for `rome`
 
         Rules:
```

### Comparing `labonneboite_datamodel-1.0.5/labonneboite_datamodel/office.py` & `labonneboite_datamodel-1.0.6/labonneboite_datamodel/office.py`

 * *Files identical despite different names*

### Comparing `labonneboite_datamodel-1.0.5/labonneboite_datamodel/tests/data/test.csv` & `labonneboite_datamodel-1.0.6/labonneboite_datamodel/tests/data/test.csv`

 * *Files identical despite different names*

### Comparing `labonneboite_datamodel-1.0.5/labonneboite_datamodel/tests/test_job.py` & `labonneboite_datamodel-1.0.6/labonneboite_datamodel/tests/test_job.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 class TestOffice(TestCase):
 
     def _get_valid_job(self) -> dict:
         return {
             "rome": "M1234",
-            "naf": "1234Z",
+            "naf": "12",
             "label_naf": "Something",
             "label_rome": "Something",
             "hirings": 60
 
         }
 
     # valid job
@@ -20,15 +20,15 @@
         self.assertTrue(Job.validate(data).rome == "M1234")
 
     # invalid naf
 
     def test_naf_invalid(self) -> None:
         data = self._get_valid_job()
 
-        for value in ["1".zfill(5), "0".zfill(4), "abc2".zfill(5)]:
+        for value in ["1f", "0", "abc2"]:
 
             data["naf"] = value
 
             with self.assertRaises(ValueError):
                 Job.validate(data)
 
     # invalid naf
```

### Comparing `labonneboite_datamodel-1.0.5/labonneboite_datamodel/tests/test_office.py` & `labonneboite_datamodel-1.0.6/labonneboite_datamodel/tests/test_office.py`

 * *Files identical despite different names*

### Comparing `labonneboite_datamodel-1.0.5/pyproject.toml` & `labonneboite_datamodel-1.0.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "labonneboite-datamodel"
-version = "1.0.5"
+version = "1.0.6"
 description = "Datamodel for labonneboite"
 authors = ["Sylvain Touret"]
 license = "MIT"
 packages = [{include = "labonneboite_datamodel"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```


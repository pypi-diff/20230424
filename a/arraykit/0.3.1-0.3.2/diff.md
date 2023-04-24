# Comparing `tmp/arraykit-0.3.1.tar.gz` & `tmp/arraykit-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arraykit-0.3.1.tar", last modified: Thu Mar 30 21:17:34 2023, max compression
+gzip compressed data, was "arraykit-0.3.2.tar", last modified: Mon Apr 24 15:28:22 2023, max compression
```

## Comparing `arraykit-0.3.1.tar` & `arraykit-0.3.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 21:17:34.227836 arraykit-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-03-30 21:17:28.000000 arraykit-0.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-03-30 21:17:28.000000 arraykit-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1166 2023-03-30 21:17:34.227836 arraykit-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3016 2023-03-30 21:17:28.000000 arraykit-0.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 21:17:34.227836 arraykit-0.3.1/arraykit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1166 2023-03-30 21:17:34.000000 arraykit-0.3.1/arraykit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      470 2023-03-30 21:17:34.000000 arraykit-0.3.1/arraykit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-30 21:17:34.000000 arraykit-0.3.1/arraykit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-03-30 21:17:34.000000 arraykit-0.3.1/arraykit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-03-30 21:17:34.000000 arraykit-0.3.1/arraykit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-30 21:17:34.227836 arraykit-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2686 2023-03-30 21:17:28.000000 arraykit-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 21:17:34.227836 arraykit-0.3.1/src/
--rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-03-30 21:17:28.000000 arraykit-0.3.1/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   144179 2023-03-30 21:17:28.000000 arraykit-0.3.1/src/_arraykit.c
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 21:17:34.227836 arraykit-0.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (122)     3129 2023-03-30 21:17:28.000000 arraykit-0.3.1/test/test_array_go.py
--rw-r--r--   0 runner    (1001) docker     (122)    48941 2023-03-30 21:17:28.000000 arraykit-0.3.1/test/test_delimited_to_arrays.py
--rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-03-30 21:17:28.000000 arraykit-0.3.1/test/test_delimited_to_arrays_integration.py
--rw-r--r--   0 runner    (1001) docker     (122)     2205 2023-03-30 21:17:28.000000 arraykit-0.3.1/test/test_delimited_to_arrays_property.py
--rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-03-30 21:17:28.000000 arraykit-0.3.1/test/test_pyi.py
--rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-03-30 21:17:28.000000 arraykit-0.3.1/test/test_split_after_count.py
--rw-r--r--   0 runner    (1001) docker     (122)    28073 2023-03-30 21:17:28.000000 arraykit-0.3.1/test/test_type_discovery.py
--rw-r--r--   0 runner    (1001) docker     (122)    26066 2023-03-30 21:17:28.000000 arraykit-0.3.1/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 15:28:22.452730 arraykit-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-04-24 15:28:16.000000 arraykit-0.3.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-04-24 15:28:16.000000 arraykit-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1178 2023-04-24 15:28:22.452730 arraykit-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3324 2023-04-24 15:28:16.000000 arraykit-0.3.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 15:28:22.452730 arraykit-0.3.2/arraykit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1178 2023-04-24 15:28:22.000000 arraykit-0.3.2/arraykit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      470 2023-04-24 15:28:22.000000 arraykit-0.3.2/arraykit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-24 15:28:22.000000 arraykit-0.3.2/arraykit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-04-24 15:28:22.000000 arraykit-0.3.2/arraykit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-24 15:28:22.000000 arraykit-0.3.2/arraykit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-24 15:28:22.452730 arraykit-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2698 2023-04-24 15:28:16.000000 arraykit-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 15:28:22.452730 arraykit-0.3.2/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-04-24 15:28:16.000000 arraykit-0.3.2/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   145128 2023-04-24 15:28:16.000000 arraykit-0.3.2/src/_arraykit.c
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 15:28:22.452730 arraykit-0.3.2/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     3129 2023-04-24 15:28:16.000000 arraykit-0.3.2/test/test_array_go.py
+-rw-r--r--   0 runner    (1001) docker     (122)    49054 2023-04-24 15:28:16.000000 arraykit-0.3.2/test/test_delimited_to_arrays.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-04-24 15:28:16.000000 arraykit-0.3.2/test/test_delimited_to_arrays_integration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2205 2023-04-24 15:28:16.000000 arraykit-0.3.2/test/test_delimited_to_arrays_property.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-04-24 15:28:16.000000 arraykit-0.3.2/test/test_pyi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-04-24 15:28:16.000000 arraykit-0.3.2/test/test_split_after_count.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28073 2023-04-24 15:28:16.000000 arraykit-0.3.2/test/test_type_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26066 2023-04-24 15:28:16.000000 arraykit-0.3.2/test/test_util.py
```

### Comparing `arraykit-0.3.1/LICENSE.txt` & `arraykit-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arraykit-0.3.1/PKG-INFO` & `arraykit-0.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 1.2
 Name: arraykit
-Version: 0.3.1
+Version: 0.3.2
 Summary: Array utilities for StaticFrame
 Home-page: https://github.com/static-frame/arraykit
 Author: Christopher Ariza, Brandt Bucher, Charles Burkland
 License: MIT
 Description: The ArrayKit library provides utilities for creating and transforming NumPy arrays, implementing performance-critical StaticFrame operations as Python C extensions.
         
         Code: https://github.com/static-frame/arraykit
         
         Packages: https://pypi.org/project/arraykit
         
 Keywords: numpy array
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `arraykit-0.3.1/README.rst` & `arraykit-0.3.2/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -33,28 +33,44 @@
 - NumPy >= 1.18.5
 
 
 
 What is New in ArrayKit
 -------------------------
 
+0.3.2
+............
+
+Optimization to ``delimited_to_arrays()`` character reading pre line.
+
+
+0.3.1
+............
+
+Improvements to ``delimited_to_arrays()``, including proper loading of ``float16`` types.
+
+Extended ``deepcopy_array()`` to permit ``memo`` as None.
+
+Corrected all compiler warnings on Windows.
+
+
 0.3.0
-------------
+............
 
 Added ``first_true_1d()``, ``first_true_2d()``. Added tools for performance graphing.
 
 
 0.2.9
-------------
+............
 
 Corrected segmentation fault resulting from attempting to parse invalid ``datetime64`` strings in ``AK_CPL_to_array_via_cast``.
 
 
 0.2.8
-------------
+............
 
 Added ``include_none`` argument to ``isna_element()``; implemented identification of Pandas pd.Timestamp NaT.
 
 
 0.2.7
 ............
```

### Comparing `arraykit-0.3.1/arraykit.egg-info/PKG-INFO` & `arraykit-0.3.2/arraykit.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 1.2
 Name: arraykit
-Version: 0.3.1
+Version: 0.3.2
 Summary: Array utilities for StaticFrame
 Home-page: https://github.com/static-frame/arraykit
 Author: Christopher Ariza, Brandt Bucher, Charles Burkland
 License: MIT
 Description: The ArrayKit library provides utilities for creating and transforming NumPy arrays, implementing performance-critical StaticFrame operations as Python C extensions.
         
         Code: https://github.com/static-frame/arraykit
         
         Packages: https://pypi.org/project/arraykit
         
 Keywords: numpy array
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `arraykit-0.3.1/setup.py` & `arraykit-0.3.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import site
 import os
 import typing as tp
 from setuptools import Extension  # type: ignore
 from setuptools import setup
 from pathlib import Path
 
-AK_VERSION = '0.3.1'
+AK_VERSION = '0.3.2'
 
 def get_long_description() -> str:
     return '''The ArrayKit library provides utilities for creating and transforming NumPy arrays, implementing performance-critical StaticFrame operations as Python C extensions.
 
 Code: https://github.com/static-frame/arraykit
 
 Packages: https://pypi.org/project/arraykit
@@ -48,15 +48,15 @@
     python_requires='>3.7.0',
     install_requires=['numpy>=1.18.5'],
     url='https://github.com/static-frame/arraykit',
     author='Christopher Ariza, Brandt Bucher, Charles Burkland',
     license='MIT',
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Topic :: Software Development',
         'License :: OSI Approved :: MIT License',
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: Microsoft :: Windows',
         'Operating System :: POSIX',
         'Programming Language :: Python :: 3.7',
```

### Comparing `arraykit-0.3.1/src/__init__.py` & `arraykit-0.3.2/src/__init__.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.3.1/src/_arraykit.c` & `arraykit-0.3.2/src/_arraykit.c`

 * *Files 2% similar despite different names*

```diff
@@ -2608,16 +2608,15 @@
 // Using AK_DelimitedReader's state, process one record (via next(input_iter)); call AK_DR_process_char on each char in that line, loading individual fields into AK_CodePointGrid. Returns 1 when there are more lines to process, 0 when there are no lines to process, and -1 for error.
 static int
 AK_DR_ProcessRecord(AK_DelimitedReader *dr,
         AK_CodePointGrid *cpg,
         PyObject *line_select
         )
 {
-    Py_UCS4 c;
-    Py_ssize_t pos, linelen;
+    Py_ssize_t linelen;
     unsigned int kind;
     const void *data;
     PyObject *record;
 
     AK_DR_line_reset(dr);
     do {
         // get a string, representing one record, to parse
@@ -2663,28 +2662,51 @@
         }
         // NOTE: record_number should reflect the processed line count, and exlude any skipped lines. The value is initialized to -1 such the first line is number 0
         ++dr->record_number;
         // AK_DEBUG_MSG_OBJ("processing line", PyLong_FromLong(dr->record_number));
 
         kind = PyUnicode_KIND(record);
         data = PyUnicode_DATA(record);
-        pos = 0;
         linelen = PyUnicode_GET_LENGTH(record);
-        while (linelen--) {
-            c = PyUnicode_READ(kind, data, pos);
-            if (c == '\0') {
-                Py_DECREF(record);
-                PyErr_Format(PyExc_RuntimeError, "line contains NUL");
-                return -1;
+
+        // NOTE: we used to check that the read character was not \0; this seems rare enough to not be necessary to handle explicit, as AK_DR_process_char will treat it as an end of record
+        switch (kind) {
+            case PyUnicode_1BYTE_KIND: {
+                Py_UCS1* uc = (Py_UCS1*)data;
+                Py_UCS1* uc_end = uc + linelen;
+                while (uc < uc_end) {
+                    if (AK_DR_process_char(dr, cpg, *uc++)) {
+                        Py_DECREF(record);
+                        return -1;
+                    }
+                }
+                break;
             }
-            if (AK_DR_process_char(dr, cpg, c)) {
-                Py_DECREF(record);
-                return -1;
+            case PyUnicode_2BYTE_KIND: {
+                Py_UCS2* uc = (Py_UCS2*)data;
+                Py_UCS2* uc_end = uc + linelen;
+                while (uc < uc_end) {
+                    if (AK_DR_process_char(dr, cpg, *uc++)) {
+                        Py_DECREF(record);
+                        return -1;
+                    }
+                }
+                break;
+            }
+            case PyUnicode_4BYTE_KIND: {
+                Py_UCS4* uc = (Py_UCS4*)data;
+                Py_UCS4* uc_end = uc + linelen;
+                while (uc < uc_end) {
+                    if (AK_DR_process_char(dr, cpg, *uc++)) {
+                        Py_DECREF(record);
+                        return -1;
+                    }
+                }
+                break;
             }
-            pos++;
         }
         Py_DECREF(record);
         // force signaling we are at the end of a line
         if (AK_DR_process_char(dr, cpg, '\0')) return -1;
 
     } while (dr->state != START_RECORD);
     return 1; // more lines to process
```

### Comparing `arraykit-0.3.1/test/test_array_go.py` & `arraykit-0.3.2/test/test_array_go.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.3.1/test/test_delimited_to_arrays.py` & `arraykit-0.3.2/test/test_delimited_to_arrays.py`

 * *Files 1% similar despite different names*

```diff
@@ -684,21 +684,22 @@
         # dtypes fails for argument 2
         with self.assertRaises(RuntimeError):
             _ = delimited_to_arrays(msg, axis=1, dtypes=dtypes)
 
 
     def test_delimited_to_arrays_parse_g(self) -> None:
         msg = [
-            'a, 10, foo',
-            'b,  20, \0',
+            'a,10,foo',
+            'b,20,\0',
             ]
-        # if a null character is encountered
-        with self.assertRaises(RuntimeError):
-            _ = delimited_to_arrays(msg, axis=1)
-
+        # if a null character is encountered it used to raise; this seemed unnecessary
+        post = delimited_to_arrays(msg, axis=1)
+        self.assertEqual( [a.tolist() for a in post],
+                [['a', 'b'], [10, 20], ['foo', '']]
+                )
 
     def test_delimited_to_arrays_parse_h(self) -> None:
         msg = [',0', 'False,1']
         post1 = delimited_to_arrays(msg, axis=1)
         # without specifying dtypes we get bool and int
         self.assertEqual([a.tolist() for a in post1], [[False, False], [0, 1]])
```

### Comparing `arraykit-0.3.1/test/test_delimited_to_arrays_integration.py` & `arraykit-0.3.2/test/test_delimited_to_arrays_integration.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.3.1/test/test_delimited_to_arrays_property.py` & `arraykit-0.3.2/test/test_delimited_to_arrays_property.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.3.1/test/test_pyi.py` & `arraykit-0.3.2/test/test_pyi.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.3.1/test/test_split_after_count.py` & `arraykit-0.3.2/test/test_split_after_count.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.3.1/test/test_type_discovery.py` & `arraykit-0.3.2/test/test_type_discovery.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.3.1/test/test_util.py` & `arraykit-0.3.2/test/test_util.py`

 * *Files identical despite different names*


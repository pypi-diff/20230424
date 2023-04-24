# Comparing `tmp/pybotics-3.1.1.tar.gz` & `tmp/pybotics-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybotics-3.1.1.tar", max compression
+gzip compressed data, was "pybotics-3.1.2.tar", max compression
```

## Comparing `pybotics-3.1.1.tar` & `pybotics-3.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1072 2023-04-19 15:36:49.545798 pybotics-3.1.1/LICENSE
--rw-r--r--   0        0        0    13486 2023-04-19 15:36:49.545798 pybotics-3.1.1/README.md
--rw-r--r--   0        0        0       24 2023-04-19 15:36:49.557798 pybotics-3.1.1/pybotics/__init__.py
--rw-r--r--   0        0        0      315 2023-04-19 15:36:49.557798 pybotics-3.1.1/pybotics/errors.py
--rw-r--r--   0        0        0     4996 2023-04-19 15:36:49.557798 pybotics-3.1.1/pybotics/geometry.py
--rw-r--r--   0        0        0      941 2023-04-19 15:36:49.557798 pybotics-3.1.1/pybotics/json_encoder.py
--rw-r--r--   0        0        0     5438 2023-04-19 15:36:49.557798 pybotics-3.1.1/pybotics/kinematic_chain.py
--rw-r--r--   0        0        0     4282 2023-04-19 15:36:49.557798 pybotics-3.1.1/pybotics/link.py
--rw-r--r--   0        0        0     5369 2023-04-19 15:36:49.557798 pybotics-3.1.1/pybotics/optimization.py
--rw-r--r--   0        0        0     2046 2023-04-19 15:36:49.557798 pybotics-3.1.1/pybotics/predefined_models.py
--rw-r--r--   0        0        0     9324 2023-04-19 15:36:49.557798 pybotics-3.1.1/pybotics/robot.py
--rw-r--r--   0        0        0     1101 2023-04-19 15:36:49.557798 pybotics-3.1.1/pybotics/tool.py
--rw-r--r--   0        0        0     3552 2023-04-19 15:37:03.405912 pybotics-3.1.1/pyproject.toml
--rw-r--r--   0        0        0    16180 1970-01-01 00:00:00.000000 pybotics-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-24 14:16:40.138595 pybotics-3.1.2/LICENSE
+-rw-r--r--   0        0        0    13486 2023-04-24 14:16:40.138595 pybotics-3.1.2/README.md
+-rw-r--r--   0        0        0       24 2023-04-24 14:16:40.146595 pybotics-3.1.2/pybotics/__init__.py
+-rw-r--r--   0        0        0      315 2023-04-24 14:16:40.146595 pybotics-3.1.2/pybotics/errors.py
+-rw-r--r--   0        0        0     4996 2023-04-24 14:16:40.150595 pybotics-3.1.2/pybotics/geometry.py
+-rw-r--r--   0        0        0      941 2023-04-24 14:16:40.150595 pybotics-3.1.2/pybotics/json_encoder.py
+-rw-r--r--   0        0        0     5438 2023-04-24 14:16:40.150595 pybotics-3.1.2/pybotics/kinematic_chain.py
+-rw-r--r--   0        0        0     4282 2023-04-24 14:16:40.150595 pybotics-3.1.2/pybotics/link.py
+-rw-r--r--   0        0        0     5369 2023-04-24 14:16:40.150595 pybotics-3.1.2/pybotics/optimization.py
+-rw-r--r--   0        0        0     2046 2023-04-24 14:16:40.150595 pybotics-3.1.2/pybotics/predefined_models.py
+-rw-r--r--   0        0        0     9324 2023-04-24 14:16:40.150595 pybotics-3.1.2/pybotics/robot.py
+-rw-r--r--   0        0        0     1101 2023-04-24 14:16:40.150595 pybotics-3.1.2/pybotics/tool.py
+-rw-r--r--   0        0        0     3552 2023-04-24 14:16:50.394812 pybotics-3.1.2/pyproject.toml
+-rw-r--r--   0        0        0    16180 1970-01-01 00:00:00.000000 pybotics-3.1.2/PKG-INFO
```

### Comparing `pybotics-3.1.1/LICENSE` & `pybotics-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pybotics-3.1.1/README.md` & `pybotics-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pybotics-3.1.1/pybotics/geometry.py` & `pybotics-3.1.2/pybotics/geometry.py`

 * *Files identical despite different names*

### Comparing `pybotics-3.1.1/pybotics/json_encoder.py` & `pybotics-3.1.2/pybotics/json_encoder.py`

 * *Files identical despite different names*

### Comparing `pybotics-3.1.1/pybotics/kinematic_chain.py` & `pybotics-3.1.2/pybotics/kinematic_chain.py`

 * *Files identical despite different names*

### Comparing `pybotics-3.1.1/pybotics/link.py` & `pybotics-3.1.2/pybotics/link.py`

 * *Files identical despite different names*

### Comparing `pybotics-3.1.1/pybotics/optimization.py` & `pybotics-3.1.2/pybotics/optimization.py`

 * *Files identical despite different names*

### Comparing `pybotics-3.1.1/pybotics/predefined_models.py` & `pybotics-3.1.2/pybotics/predefined_models.py`

 * *Files identical despite different names*

### Comparing `pybotics-3.1.1/pybotics/robot.py` & `pybotics-3.1.2/pybotics/robot.py`

 * *Files identical despite different names*

### Comparing `pybotics-3.1.1/pybotics/tool.py` & `pybotics-3.1.2/pybotics/tool.py`

 * *Files identical despite different names*

### Comparing `pybotics-3.1.1/pyproject.toml` & `pybotics-3.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybotics"
-version = "3.1.1"
+version = "3.1.2"
 description = "Python Toolbox for Robotics"
 authors = ["Nicholas Nadeau <nicholas.nadeau@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/engnadeau/pybotics"
 repository = "https://github.com/engnadeau/pybotics"
 documentation = "https://github.com/engnadeau/pybotics"
 keywords = ["robot", "research", "automation", "kinematics", "geometry"]
```

### Comparing `pybotics-3.1.1/PKG-INFO` & `pybotics-3.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybotics
-Version: 3.1.1
+Version: 3.1.2
 Summary: Python Toolbox for Robotics
 Home-page: https://github.com/engnadeau/pybotics
 Keywords: robot,research,automation,kinematics,geometry
 Author: Nicholas Nadeau
 Author-email: nicholas.nadeau@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```


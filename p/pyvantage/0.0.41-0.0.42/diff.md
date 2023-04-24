# Comparing `tmp/pyvantage-0.0.41.tar.gz` & `tmp/pyvantage-0.0.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvantage-0.0.41.tar", last modified: Sun Apr 23 18:11:38 2023, max compression
+gzip compressed data, was "pyvantage-0.0.42.tar", last modified: Mon Apr 24 16:02:50 2023, max compression
```

## Comparing `pyvantage-0.0.41.tar` & `pyvantage-0.0.42.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-04-23 18:11:38.019250 pyvantage-0.0.41/
--rw-r--r--   0 greg       (501) staff       (20)     1179 2021-06-03 17:37:04.000000 pyvantage-0.0.41/LICENSE
--rw-r--r--   0 greg       (501) staff       (20)      604 2023-04-23 18:11:38.019412 pyvantage-0.0.41/PKG-INFO
--rw-r--r--   0 greg       (501) staff       (20)     2164 2023-04-23 17:44:30.000000 pyvantage-0.0.41/README.md
-drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-04-23 18:11:38.015777 pyvantage-0.0.41/pyvantage/
--rw-r--r--   0 greg       (501) staff       (20)    99570 2023-04-23 18:09:02.000000 pyvantage-0.0.41/pyvantage/__init__.py
-drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-04-23 18:11:38.018688 pyvantage-0.0.41/pyvantage.egg-info/
--rw-r--r--   0 greg       (501) staff       (20)      604 2023-04-23 18:11:38.000000 pyvantage-0.0.41/pyvantage.egg-info/PKG-INFO
--rw-r--r--   0 greg       (501) staff       (20)      218 2023-04-23 18:11:38.000000 pyvantage-0.0.41/pyvantage.egg-info/SOURCES.txt
--rw-r--r--   0 greg       (501) staff       (20)        1 2023-04-23 18:11:38.000000 pyvantage-0.0.41/pyvantage.egg-info/dependency_links.txt
--rw-r--r--   0 greg       (501) staff       (20)       10 2023-04-23 18:11:38.000000 pyvantage-0.0.41/pyvantage.egg-info/top_level.txt
--rw-r--r--   0 greg       (501) staff       (20)        1 2023-04-23 18:11:37.000000 pyvantage-0.0.41/pyvantage.egg-info/zip-safe
--rw-r--r--   0 greg       (501) staff       (20)       79 2023-04-23 18:11:38.019945 pyvantage-0.0.41/setup.cfg
--rw-r--r--   0 greg       (501) staff       (20)      769 2023-04-23 17:49:39.000000 pyvantage-0.0.41/setup.py
+drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-04-24 16:02:50.398539 pyvantage-0.0.42/
+-rw-r--r--   0 greg       (501) staff       (20)     1179 2021-06-03 17:37:04.000000 pyvantage-0.0.42/LICENSE
+-rw-r--r--   0 greg       (501) staff       (20)      604 2023-04-24 16:02:50.398643 pyvantage-0.0.42/PKG-INFO
+-rw-r--r--   0 greg       (501) staff       (20)     2164 2023-04-23 17:44:30.000000 pyvantage-0.0.42/README.md
+drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-04-24 16:02:50.396263 pyvantage-0.0.42/pyvantage/
+-rw-r--r--   0 greg       (501) staff       (20)    99569 2023-04-24 16:00:56.000000 pyvantage-0.0.42/pyvantage/__init__.py
+drwxr-xr-x   0 greg       (501) staff       (20)        0 2023-04-24 16:02:50.397921 pyvantage-0.0.42/pyvantage.egg-info/
+-rw-r--r--   0 greg       (501) staff       (20)      604 2023-04-24 16:02:50.000000 pyvantage-0.0.42/pyvantage.egg-info/PKG-INFO
+-rw-r--r--   0 greg       (501) staff       (20)      218 2023-04-24 16:02:50.000000 pyvantage-0.0.42/pyvantage.egg-info/SOURCES.txt
+-rw-r--r--   0 greg       (501) staff       (20)        1 2023-04-24 16:02:50.000000 pyvantage-0.0.42/pyvantage.egg-info/dependency_links.txt
+-rw-r--r--   0 greg       (501) staff       (20)       10 2023-04-24 16:02:50.000000 pyvantage-0.0.42/pyvantage.egg-info/top_level.txt
+-rw-r--r--   0 greg       (501) staff       (20)        1 2023-04-23 18:11:37.000000 pyvantage-0.0.42/pyvantage.egg-info/zip-safe
+-rw-r--r--   0 greg       (501) staff       (20)       79 2023-04-24 16:02:50.399045 pyvantage-0.0.42/setup.cfg
+-rw-r--r--   0 greg       (501) staff       (20)      769 2023-04-24 16:01:39.000000 pyvantage-0.0.42/setup.py
```

### Comparing `pyvantage-0.0.41/LICENSE` & `pyvantage-0.0.42/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvantage-0.0.41/PKG-INFO` & `pyvantage-0.0.42/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvantage
-Version: 0.0.41
+Version: 0.0.42
 Summary: Python library for Vantage Controller (for Home Assistant)
 Home-page: http://github.com/gjbadros/pyvantage
 Author: Greg J. Badros
 Author-email: badros@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyvantage-0.0.41/README.md` & `pyvantage-0.0.42/README.md`

 * *Files identical despite different names*

### Comparing `pyvantage-0.0.41/pyvantage/__init__.py` & `pyvantage-0.0.42/pyvantage/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -431,15 +431,15 @@
         irzones = objects.findall("Object/IRZone[@VID]")
         for irzone_xml in irzones:
             area = self._parse_irzone(irzone_xml)
             _LOGGER.debug("IRZone = %s", area)
             self.vid_to_area[area.vid] = area
 
         # note the extra '/' after 'Object/ -- the Vantage.DDGColorLoad elements aren't always direct descendents of Object
-        loads = objects.findall("Object/Load[@VID]") + objects.findall("Object//Vantage.DDGColorLoad[@VID]")
+        loads = objects.findall("Object/Load[@VID]") + objects.findall("Object/Vantage.DDGColorLoad[@VID]")
         other_loads = []
         color_loads = []
         open_loads = []
         for ld in loads:
             t = ld.findtext('Name')
             if t.endswith(' COLOR'):
                 color_loads.append(ld)
@@ -1395,28 +1395,28 @@
         _LOGGER.info("Loaded xml db")
         # print(xml_db[0:10000])
         self.do_parse(xml_db)
 
     def do_parse(self, xml_db):
         """Call the parser and copy its output here."""
         parser = VantageXmlDbParser(vantage=self, xml_db_str=xml_db)
-        parser.parse()
-        self.outputs = parser.outputs
-        self.variables = parser.variables
-        self.tasks = parser.tasks
-        self.buttons = parser.buttons
-        self.keypads = parser.keypads
-        self.sensors = parser.sensors
         self._vid_to_load = parser.vid_to_load
         self._vid_to_variable = parser.vid_to_variable
         self._vid_to_shade = parser.vid_to_shade
         self._vid_to_task = parser.vid_to_task
         self._vid_to_sensor = parser.vid_to_sensor
         self._name_to_task = parser.name_to_task
         self._name = parser.project_name
+        parser.parse()
+        self.outputs = parser.outputs
+        self.variables = parser.variables
+        self.tasks = parser.tasks
+        self.buttons = parser.buttons
+        self.keypads = parser.keypads
+        self.sensors = parser.sensors
 
         _LOGGER.info("Found Vantage project: %s, %d areas, %d loads, "
                      "%d variables, and %d shades",
                      self._name,
                      len(self._vid_to_area.keys()),
                      len(self._vid_to_load.keys()),
                      len(self._vid_to_variable.keys()),
```

### Comparing `pyvantage-0.0.41/pyvantage.egg-info/PKG-INFO` & `pyvantage-0.0.42/pyvantage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvantage
-Version: 0.0.41
+Version: 0.0.42
 Summary: Python library for Vantage Controller (for Home Assistant)
 Home-page: http://github.com/gjbadros/pyvantage
 Author: Greg J. Badros
 Author-email: badros@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyvantage-0.0.41/setup.py` & `pyvantage-0.0.42/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(
     name='pyvantage',
-    version='0.0.41',
+    version='0.0.42',
     license='MIT',
     description='Python library for Vantage Controller (for Home Assistant)',
     author='Greg J. Badros',
     author_email='badros@gmail.com',
     url='http://github.com/gjbadros/pyvantage',
     packages=find_packages(),
     classifiers=[
```


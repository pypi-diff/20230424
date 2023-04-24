# Comparing `tmp/jpconvert-0.3.8.tar.gz` & `tmp/jpconvert-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jpconvert-0.3.8.tar", last modified: Fri Dec  9 10:21:43 2022, max compression
+gzip compressed data, was "jpconvert-0.3.9.tar", last modified: Tue Dec 20 11:51:13 2022, max compression
```

## Comparing `jpconvert-0.3.8.tar` & `jpconvert-0.3.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2022-12-09 10:21:43.159774 jpconvert-0.3.8/
--rw-rw-r--   0 eric      (1000) eric      (1000)     1068 2022-07-14 06:24:08.000000 jpconvert-0.3.8/LICENSE
--rw-rw-r--   0 eric      (1000) eric      (1000)     2793 2022-12-09 10:21:43.159774 jpconvert-0.3.8/PKG-INFO
--rw-r--r--   0 eric      (1000) eric      (1000)     2286 2022-08-15 10:41:14.000000 jpconvert-0.3.8/README.md
--rw-rw-r--   0 eric      (1000) eric      (1000)       38 2022-12-09 10:21:43.159774 jpconvert-0.3.8/setup.cfg
--rw-r--r--   0 eric      (1000) eric      (1000)      903 2022-12-09 09:59:15.000000 jpconvert-0.3.8/setup.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2022-12-09 10:21:43.147774 jpconvert-0.3.8/src/
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2022-12-09 10:21:43.151774 jpconvert-0.3.8/src/jpconvert/
--rw-rw-r--   0 eric      (1000) eric      (1000)      909 2022-07-05 12:32:25.000000 jpconvert-0.3.8/src/jpconvert/Pipeline.py
--rw-r--r--   0 eric      (1000) eric      (1000)      879 2022-08-12 14:27:01.000000 jpconvert-0.3.8/src/jpconvert/__init__.py
--rw-r--r--   0 eric      (1000) eric      (1000)     2431 2022-08-15 10:41:44.000000 jpconvert-0.3.8/src/jpconvert/__main__.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2022-12-09 10:21:43.159774 jpconvert-0.3.8/src/jpconvert/implementations/
--rw-rw-r--   0 eric      (1000) eric      (1000)     3540 2022-09-14 08:33:57.000000 jpconvert-0.3.8/src/jpconvert/implementations/EmbedImages.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     1390 2022-12-09 10:08:52.000000 jpconvert-0.3.8/src/jpconvert/implementations/RemoveCellByMacro.py
--rw-rw-r--   0 eric      (1000) eric      (1000)      184 2022-07-01 13:06:08.000000 jpconvert-0.3.8/src/jpconvert/implementations/RemoveEmptyCell.py
--rw-rw-r--   0 eric      (1000) eric      (1000)      170 2022-12-09 10:11:52.000000 jpconvert-0.3.8/src/jpconvert/implementations/RemoveMacros.py
--rw-rw-r--   0 eric      (1000) eric      (1000)      233 2022-07-01 07:55:34.000000 jpconvert-0.3.8/src/jpconvert/implementations/RemovePyCharm.py
--rw-rw-r--   0 eric      (1000) eric      (1000)      404 2022-07-05 13:36:15.000000 jpconvert-0.3.8/src/jpconvert/implementations/RemoveTrailingLines.py
--rw-rw-r--   0 eric      (1000) eric      (1000)      769 2022-12-09 10:08:52.000000 jpconvert-0.3.8/src/jpconvert/implementations/SetReadonly.py
--rw-rw-r--   0 eric      (1000) eric      (1000)      201 2022-07-01 12:39:16.000000 jpconvert-0.3.8/src/jpconvert/implementations/SetUndeletable.py
--rw-rw-r--   0 eric      (1000) eric      (1000)      223 2022-07-05 13:24:15.000000 jpconvert-0.3.8/src/jpconvert/implementations/StripLines.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     2684 2022-12-09 10:10:48.000000 jpconvert-0.3.8/src/jpconvert/implementations/TableOfContents.py
--rw-rw-r--   0 eric      (1000) eric      (1000)      424 2022-08-12 14:27:35.000000 jpconvert-0.3.8/src/jpconvert/implementations/__init__.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2022-12-09 10:21:43.159774 jpconvert-0.3.8/src/jpconvert/operations/
--rw-rw-r--   0 eric      (1000) eric      (1000)      282 2022-07-01 07:55:34.000000 jpconvert-0.3.8/src/jpconvert/operations/FilterCell.py
--rw-rw-r--   0 eric      (1000) eric      (1000)      406 2022-07-01 07:55:34.000000 jpconvert-0.3.8/src/jpconvert/operations/FilterLine.py
--rw-rw-r--   0 eric      (1000) eric      (1000)      255 2022-07-01 12:39:16.000000 jpconvert-0.3.8/src/jpconvert/operations/MapCell.py
--rw-rw-r--   0 eric      (1000) eric      (1000)      352 2022-07-05 13:23:07.000000 jpconvert-0.3.8/src/jpconvert/operations/MapLine.py
--rw-rw-r--   0 eric      (1000) eric      (1000)      175 2022-07-05 12:32:20.000000 jpconvert-0.3.8/src/jpconvert/operations/Operation.py
--rw-rw-r--   0 eric      (1000) eric      (1000)      161 2022-07-01 07:50:41.000000 jpconvert-0.3.8/src/jpconvert/operations/__init__.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2022-12-09 10:21:43.155774 jpconvert-0.3.8/src/jpconvert.egg-info/
--rw-r--r--   0 eric      (1000) eric      (1000)     2793 2022-12-09 10:21:43.000000 jpconvert-0.3.8/src/jpconvert.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) eric      (1000)     1050 2022-12-09 10:21:43.000000 jpconvert-0.3.8/src/jpconvert.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) eric      (1000)        1 2022-12-09 10:21:43.000000 jpconvert-0.3.8/src/jpconvert.egg-info/dependency_links.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)       38 2022-12-09 10:21:43.000000 jpconvert-0.3.8/src/jpconvert.egg-info/requires.txt
--rw-r--r--   0 eric      (1000) eric      (1000)       10 2022-12-09 10:21:43.000000 jpconvert-0.3.8/src/jpconvert.egg-info/top_level.txt
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2022-12-09 10:21:43.159774 jpconvert-0.3.8/test/
--rw-r--r--   0 eric      (1000) eric      (1000)    16895 2022-09-14 08:45:05.000000 jpconvert-0.3.8/test/test_main.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2022-12-20 11:51:13.206148 jpconvert-0.3.9/
+-rw-rw-r--   0 eric      (1000) eric      (1000)     1068 2022-07-14 06:24:08.000000 jpconvert-0.3.9/LICENSE
+-rw-rw-r--   0 eric      (1000) eric      (1000)     2793 2022-12-20 11:51:13.206148 jpconvert-0.3.9/PKG-INFO
+-rw-r--r--   0 eric      (1000) eric      (1000)     2286 2022-08-15 10:41:14.000000 jpconvert-0.3.9/README.md
+-rw-rw-r--   0 eric      (1000) eric      (1000)       38 2022-12-20 11:51:13.206148 jpconvert-0.3.9/setup.cfg
+-rw-r--r--   0 eric      (1000) eric      (1000)      903 2022-12-20 11:49:30.000000 jpconvert-0.3.9/setup.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2022-12-20 11:51:13.198148 jpconvert-0.3.9/src/
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2022-12-20 11:51:13.198148 jpconvert-0.3.9/src/jpconvert/
+-rw-rw-r--   0 eric      (1000) eric      (1000)      909 2022-07-05 12:32:25.000000 jpconvert-0.3.9/src/jpconvert/Pipeline.py
+-rw-r--r--   0 eric      (1000) eric      (1000)      990 2022-12-20 11:03:14.000000 jpconvert-0.3.9/src/jpconvert/__init__.py
+-rw-r--r--   0 eric      (1000) eric      (1000)     2812 2022-12-20 11:50:51.000000 jpconvert-0.3.9/src/jpconvert/__main__.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2022-12-20 11:51:13.202148 jpconvert-0.3.9/src/jpconvert/implementations/
+-rw-rw-r--   0 eric      (1000) eric      (1000)     3540 2022-09-14 08:33:57.000000 jpconvert-0.3.9/src/jpconvert/implementations/EmbedImages.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     1390 2022-12-09 10:08:52.000000 jpconvert-0.3.9/src/jpconvert/implementations/RemoveCellByMacro.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)      184 2022-07-01 13:06:08.000000 jpconvert-0.3.9/src/jpconvert/implementations/RemoveEmptyCell.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)      170 2022-12-09 10:11:52.000000 jpconvert-0.3.9/src/jpconvert/implementations/RemoveMacros.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)      233 2022-07-01 07:55:34.000000 jpconvert-0.3.9/src/jpconvert/implementations/RemovePyCharm.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)      404 2022-07-05 13:36:15.000000 jpconvert-0.3.9/src/jpconvert/implementations/RemoveTrailingLines.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)      883 2022-12-20 11:44:09.000000 jpconvert-0.3.9/src/jpconvert/implementations/SetReadonly.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)      201 2022-07-01 12:39:16.000000 jpconvert-0.3.9/src/jpconvert/implementations/SetUndeletable.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)      223 2022-07-05 13:24:15.000000 jpconvert-0.3.9/src/jpconvert/implementations/StripLines.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     2684 2022-12-09 10:10:48.000000 jpconvert-0.3.9/src/jpconvert/implementations/TableOfContents.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)      424 2022-08-12 14:27:35.000000 jpconvert-0.3.9/src/jpconvert/implementations/__init__.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2022-12-20 11:51:13.206148 jpconvert-0.3.9/src/jpconvert/operations/
+-rw-rw-r--   0 eric      (1000) eric      (1000)      282 2022-07-01 07:55:34.000000 jpconvert-0.3.9/src/jpconvert/operations/FilterCell.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)      406 2022-07-01 07:55:34.000000 jpconvert-0.3.9/src/jpconvert/operations/FilterLine.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)      255 2022-07-01 12:39:16.000000 jpconvert-0.3.9/src/jpconvert/operations/MapCell.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)      352 2022-07-05 13:23:07.000000 jpconvert-0.3.9/src/jpconvert/operations/MapLine.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)      175 2022-07-05 12:32:20.000000 jpconvert-0.3.9/src/jpconvert/operations/Operation.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)      161 2022-07-01 07:50:41.000000 jpconvert-0.3.9/src/jpconvert/operations/__init__.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2022-12-20 11:51:13.198148 jpconvert-0.3.9/src/jpconvert.egg-info/
+-rw-r--r--   0 eric      (1000) eric      (1000)     2793 2022-12-20 11:51:13.000000 jpconvert-0.3.9/src/jpconvert.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) eric      (1000)     1050 2022-12-20 11:51:13.000000 jpconvert-0.3.9/src/jpconvert.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) eric      (1000)        1 2022-12-20 11:51:13.000000 jpconvert-0.3.9/src/jpconvert.egg-info/dependency_links.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)       38 2022-12-20 11:51:13.000000 jpconvert-0.3.9/src/jpconvert.egg-info/requires.txt
+-rw-r--r--   0 eric      (1000) eric      (1000)       10 2022-12-20 11:51:13.000000 jpconvert-0.3.9/src/jpconvert.egg-info/top_level.txt
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2022-12-20 11:51:13.206148 jpconvert-0.3.9/test/
+-rw-r--r--   0 eric      (1000) eric      (1000)    17003 2022-12-20 11:37:25.000000 jpconvert-0.3.9/test/test_main.py
```

### Comparing `jpconvert-0.3.8/LICENSE` & `jpconvert-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jpconvert-0.3.8/PKG-INFO` & `jpconvert-0.3.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jpconvert
-Version: 0.3.8
+Version: 0.3.9
 Summary: macros for Jupyter Notebooks
 Home-page: https://github.com/erictroebs/jpconvert
 Author: Eric Tröbs
 Author-email: eric.troebs@tu-ilmenau.de
 Project-URL: Bug Tracker, https://github.com/erictroebs/jpconvert/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jpconvert-0.3.8/README.md` & `jpconvert-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `jpconvert-0.3.8/setup.py` & `jpconvert-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
     name='jpconvert',
-    version='0.3.8',
+    version='0.3.9',
     author='Eric Tröbs',
     author_email='eric.troebs@tu-ilmenau.de',
     description='macros for Jupyter Notebooks',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/erictroebs/jpconvert',
     project_urls={
```

### Comparing `jpconvert-0.3.8/src/jpconvert/Pipeline.py` & `jpconvert-0.3.9/src/jpconvert/Pipeline.py`

 * *Files identical despite different names*

### Comparing `jpconvert-0.3.8/src/jpconvert/__init__.py` & `jpconvert-0.3.9/src/jpconvert/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from .Pipeline import Pipeline
 from .implementations import *
 
 
 def build_pipeline(practice: bool, solution: bool, teaching: bool,
                    remove_without_macros: bool, remove_empty: bool,
                    strip_lines: bool, remove_trailing_lines: bool,
-                   embed_images: bool) -> Pipeline:
+                   embed_images: bool,
+                   force_readonly: bool, force_undeletable: bool) -> Pipeline:
     pipeline = Pipeline()
 
     pipeline.add(RemoveCellByMacro(practice, solution, teaching, remove_without_macros))
     pipeline.add(RemovePyCharm())
 
     pipeline.add(TableOfContents())
 
-    pipeline.add(SetReadonly())
-    pipeline.add(SetUndeletable())
+    pipeline.add(SetReadonly(force_readonly))
+
+    if force_undeletable:
+        pipeline.add(SetUndeletable())
 
     pipeline.add(RemoveMacros())
 
     if strip_lines:
         pipeline.add(StripLines())
 
     if remove_trailing_lines:
```

### Comparing `jpconvert-0.3.8/src/jpconvert/__main__.py` & `jpconvert-0.3.9/src/jpconvert/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,14 +21,18 @@
                     help='keep empty cells')
 parser.add_argument('--no-strip-lines', action='store_true', default=False,
                     help='do not strip lines')
 parser.add_argument('--keep-trailing', action='store_true', default=False,
                     help='keep empty trailing lines')
 parser.add_argument('--no-embed-images', action='store_true', default=False,
                     help='do not embed images in output file')
+parser.add_argument('--no-force-readonly', action='store_true', default=False,
+                    help='do not automatically set code cells to readonly')
+parser.add_argument('--no-set-undeletable', action='store_true', default=False,
+                    help='do not protect cells from deletion')
 parser.add_argument('output', nargs='?', default='-',
                     help='output file (.ipynb) or - (stdout, default)')
 
 args = parser.parse_args()
 
 # ensure exclusivity of some parameters
 practice = args.practice
@@ -54,15 +58,16 @@
     with open(args.input, 'r', encoding='utf-8') as file:
         input_data = json.load(file)
 
 # run pipeline
 pipeline = build_pipeline(practice, solution, teaching,
                           args.remove_without_macros, not args.keep_empty,
                           not args.no_strip_lines, not args.keep_trailing,
-                          not args.no_embed_images)
+                          not args.no_embed_images,
+                          not args.no_force_readonly, not args.no_set_undeletable)
 output_data = pipeline.run(input_data)
 
 # write output
 if args.output == '-':
     print(json.dumps(output_data, indent=4))
 else:
     with open(args.output, 'w') as file:
```

### Comparing `jpconvert-0.3.8/src/jpconvert/implementations/EmbedImages.py` & `jpconvert-0.3.9/src/jpconvert/implementations/EmbedImages.py`

 * *Files identical despite different names*

### Comparing `jpconvert-0.3.8/src/jpconvert/implementations/RemoveCellByMacro.py` & `jpconvert-0.3.9/src/jpconvert/implementations/RemoveCellByMacro.py`

 * *Files identical despite different names*

### Comparing `jpconvert-0.3.8/src/jpconvert/implementations/SetReadonly.py` & `jpconvert-0.3.9/src/jpconvert/implementations/SetReadonly.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 from typing import Dict
 
 from ..operations import MapCell
 
 
 class SetReadonly(MapCell):
+    def __init__(self, force: bool):
+        self._force: bool = force
+
     def map_cell(self, cell: Dict) -> Dict:
         # set all markdown cells to readonly
         if cell['cell_type'] != 'code':
             cell['metadata']['editable'] = False
+            return cell
 
         # find practice macro
         practice = False
         readonly = False
 
         for line in cell['source']:
             line = line.strip()
 
             if line in ['#jp-practice', '--jp-practice']:
                 practice = True
             elif line in ['#jp-practice-ro', '--jp-practice-ro', '#jp-readonly', '--jp-readonly']:
                 readonly = True
 
         # set readonly
-        if not practice or readonly:
+        if (not practice and self._force) or readonly:
             cell['metadata']['editable'] = False
 
         return cell
```

### Comparing `jpconvert-0.3.8/src/jpconvert/implementations/TableOfContents.py` & `jpconvert-0.3.9/src/jpconvert/implementations/TableOfContents.py`

 * *Files identical despite different names*

### Comparing `jpconvert-0.3.8/src/jpconvert.egg-info/PKG-INFO` & `jpconvert-0.3.9/src/jpconvert.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jpconvert
-Version: 0.3.8
+Version: 0.3.9
 Summary: macros for Jupyter Notebooks
 Home-page: https://github.com/erictroebs/jpconvert
 Author: Eric Tröbs
 Author-email: eric.troebs@tu-ilmenau.de
 Project-URL: Bug Tracker, https://github.com/erictroebs/jpconvert/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jpconvert-0.3.8/src/jpconvert.egg-info/SOURCES.txt` & `jpconvert-0.3.9/src/jpconvert.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jpconvert-0.3.8/test/test_main.py` & `jpconvert-0.3.9/test/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         json.dump(output, file)
 
     return output['cells']
 
 
 def test_practice():
     cells = run('ExampleCode.ipynb',
-                build_pipeline(True, False, False, False, False, False, False, False))
+                build_pipeline(True, False, False, False, False, False, False, False, True, True))
 
     # len
     assert len(cells) == 13
 
     # 0
     cell = cells[0]
     assert cell['cell_type'] == 'markdown'
@@ -116,15 +116,15 @@
     assert cell['source'] == ["z = 'readonly'"]
     assert 'deletable' in cell['metadata'] and not cell['metadata']['deletable']
     assert 'editable' in cell['metadata'] and not cell['metadata']['editable']
 
 
 def test_solution():
     cells = run('ExampleCode.ipynb',
-                build_pipeline(False, True, False, False, False, False, False, False))
+                build_pipeline(False, True, False, False, False, False, False, False, True, True))
 
     # len
     assert len(cells) == 10
 
     # 0
     cell = cells[0]
     assert cell['cell_type'] == 'markdown'
@@ -194,15 +194,15 @@
     assert cell['source'] == ['Und eine leere Zelle zum Schluss:']
     assert 'deletable' in cell['metadata'] and not cell['metadata']['deletable']
     assert 'editable' in cell['metadata'] and not cell['metadata']['editable']
 
 
 def test_teaching():
     cells = run('ExampleCode.ipynb',
-                build_pipeline(False, False, True, False, False, False, False, False))
+                build_pipeline(False, False, True, False, False, False, False, False, True, True))
 
     # len
     assert len(cells) == 8
 
     # 0
     cell = cells[0]
     assert cell['cell_type'] == 'markdown'
@@ -258,15 +258,15 @@
     assert cell['source'] == ['Und eine leere Zelle zum Schluss:']
     assert 'deletable' in cell['metadata'] and not cell['metadata']['deletable']
     assert 'editable' in cell['metadata'] and not cell['metadata']['editable']
 
 
 def test_remove_without_macros():
     cells = run('ExampleCode.ipynb',
-                build_pipeline(True, False, False, True, False, False, False, False))
+                build_pipeline(True, False, False, True, False, False, False, False, True, True))
 
     # len
     assert len(cells) == 11
 
     # 5
     cell = cells[5]
     assert cell['source'] != []
@@ -274,27 +274,27 @@
     # 8
     cell = cells[8]
     assert cell['source'] != ['e = a']
 
 
 def test_remove_empty():
     cells = run('ExampleCode.ipynb',
-                build_pipeline(True, False, False, False, True, False, False, False))
+                build_pipeline(True, False, False, False, True, False, False, False, True, True))
 
     # len
     assert len(cells) == 11
 
     # check for empty cells
     for cell in cells:
         assert len(cell['source']) > 0
 
 
 def test_toc():
     cells = run('ExampleToc.ipynb',
-                build_pipeline(True, False, False, True, True, False, False, False))
+                build_pipeline(True, False, False, True, True, False, False, False, True, True))
 
     # 1
     assert cells[1]['cell_type'] == 'markdown'
     assert cells[1]['source'] == ['# Inhaltsverzeichnis\n',
                                   '- [TOC Test](#TOC-Test)\n',
                                   '  - [Code](#Code)\n',
                                   '  - [Text](#Text)\n',
@@ -326,15 +326,15 @@
                                   '  - [Code](#Code)\n',
                                   '  - [Text](#Text)\n',
                                   '  - [Mix](#Mix)']
 
 
 def test_strip_lines():
     cells = run('ExampleLines.ipynb',
-                build_pipeline(True, False, False, False, False, True, False, False))
+                build_pipeline(True, False, False, False, False, True, False, False, True, True))
 
     # len
     assert len(cells) == 12
 
     # 1
     assert cells[1]['source'] == ['this = 1\n',
                                   "my = 'code'"]
@@ -356,15 +356,15 @@
 
     # 11
     assert cells[11]['source'] == ['\n', '']
 
 
 def test_trailing_lines():
     cells = run('ExampleLines.ipynb',
-                build_pipeline(True, False, False, False, False, True, True, False))
+                build_pipeline(True, False, False, False, False, True, True, False, True, True))
 
     # len
     assert len(cells) == 12
 
     # 1
     assert cells[1]['source'] == ['this = 1\n',
                                   "my = 'code'"]
@@ -386,15 +386,15 @@
 
     # 11
     assert cells[11]['source'] == []
 
 
 def test_embed_image():
     cells = run('ExampleImages.ipynb',
-                build_pipeline(True, False, False, False, False, False, False, True))
+                build_pipeline(True, False, False, False, False, False, False, True, True, True))
 
     # 0
     assert 'attachments' in cells[0]
     assert cells[0]['source'] == [
         "# ExampleImages\n",
         "![png description](attachment:1.png)"
     ]
```


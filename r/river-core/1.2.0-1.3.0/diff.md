# Comparing `tmp/river_core-1.2.0.tar.gz` & `tmp/river_core-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/river_core-1.2.0.tar", last modified: Mon May 23 10:00:44 2022, max compression
+gzip compressed data, was "dist/river_core-1.3.0.tar", last modified: Mon Apr 24 05:13:21 2023, max compression
```

## Comparing `river_core-1.2.0.tar` & `river_core-1.3.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:00:44.000000 river_core-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1992 2022-05-23 10:00:17.000000 river_core-1.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1533 2022-05-23 10:00:17.000000 river_core-1.2.0/LICENSE.incore
--rw-r--r--   0 runner    (1001) docker     (121)     1535 2022-05-23 10:00:17.000000 river_core-1.2.0/LICENSE.tessolve
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-05-23 10:00:17.000000 river_core-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-05-23 10:00:44.000000 river_core-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      333 2022-05-23 10:00:17.000000 river_core-1.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:00:44.000000 river_core-1.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     2091 2022-05-23 10:00:17.000000 river_core-1.2.0/examples/sample-config.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:00:44.000000 river_core-1.2.0/river_core/
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-05-23 10:00:17.000000 river_core-1.2.0/river_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2968 2022-05-23 10:00:17.000000 river_core-1.2.0/river_core/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     4005 2022-05-23 10:00:17.000000 river_core-1.2.0/river_core/log.py
--rw-r--r--   0 runner    (1001) docker     (121)     7495 2022-05-23 10:00:17.000000 river_core-1.2.0/river_core/main.py
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-05-23 10:00:17.000000 river_core-1.2.0/river_core/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)    41427 2022-05-23 10:00:17.000000 river_core-1.2.0/river_core/rivercore.py
--rw-r--r--   0 runner    (1001) docker     (121)     6401 2022-05-23 10:00:17.000000 river_core-1.2.0/river_core/sim_hookspecs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:00:44.000000 river_core-1.2.0/river_core/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     1589 2022-05-23 10:00:17.000000 river_core-1.2.0/river_core/templates/coverage_report.html
--rw-r--r--   0 runner    (1001) docker     (121)    14432 2022-05-23 10:00:17.000000 river_core-1.2.0/river_core/templates/report.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:00:44.000000 river_core-1.2.0/river_core/templates/setup/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:00:44.000000 river_core-1.2.0/river_core/templates/setup/dut/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-23 10:00:17.000000 river_core-1.2.0/river_core/templates/setup/dut/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:00:44.000000 river_core-1.2.0/river_core/templates/setup/dut/boot/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-05-23 10:00:17.000000 river_core-1.2.0/river_core/templates/setup/dut/boot/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-05-23 10:00:17.000000 river_core-1.2.0/river_core/templates/setup/dut/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2129 2022-05-23 10:00:17.000000 river_core-1.2.0/river_core/templates/setup/dut/gen_framework.py
--rw-r--r--   0 runner    (1001) docker     (121)     8461 2022-05-23 10:00:17.000000 river_core-1.2.0/river_core/templates/setup/dut/sample_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:00:44.000000 river_core-1.2.0/river_core/templates/setup/generator/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-23 10:00:17.000000 river_core-1.2.0/river_core/templates/setup/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      315 2022-05-23 10:00:17.000000 river_core-1.2.0/river_core/templates/setup/generator/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2023 2022-05-23 10:00:17.000000 river_core-1.2.0/river_core/templates/setup/generator/gen_framework.py
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-05-23 10:00:17.000000 river_core-1.2.0/river_core/templates/setup/generator/sample_gen_config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6026 2022-05-23 10:00:17.000000 river_core-1.2.0/river_core/templates/setup/generator/sample_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:00:44.000000 river_core-1.2.0/river_core/templates/setup/reference/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-23 10:00:17.000000 river_core-1.2.0/river_core/templates/setup/reference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      325 2022-05-23 10:00:17.000000 river_core-1.2.0/river_core/templates/setup/reference/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2129 2022-05-23 10:00:17.000000 river_core-1.2.0/river_core/templates/setup/reference/gen_framework.py
--rw-r--r--   0 runner    (1001) docker     (121)     5699 2022-05-23 10:00:17.000000 river_core-1.2.0/river_core/templates/setup/reference/sample_plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     4074 2022-05-23 10:00:17.000000 river_core-1.2.0/river_core/templates/style.css
--rw-r--r--   0 runner    (1001) docker     (121)    18363 2022-05-23 10:00:17.000000 river_core-1.2.0/river_core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-23 10:00:44.000000 river_core-1.2.0/river_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-05-23 10:00:44.000000 river_core-1.2.0/river_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1347 2022-05-23 10:00:44.000000 river_core-1.2.0/river_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-23 10:00:44.000000 river_core-1.2.0/river_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-05-23 10:00:44.000000 river_core-1.2.0/river_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-23 10:00:44.000000 river_core-1.2.0/river_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-05-23 10:00:44.000000 river_core-1.2.0/river_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-05-23 10:00:44.000000 river_core-1.2.0/river_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-05-23 10:00:44.000000 river_core-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1937 2022-05-23 10:00:17.000000 river_core-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:13:21.000000 river_core-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-24 05:13:01.000000 river_core-1.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-24 05:13:01.000000 river_core-1.3.0/LICENSE.incore
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-24 05:13:01.000000 river_core-1.3.0/LICENSE.tessolve
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-24 05:13:01.000000 river_core-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-24 05:13:21.000000 river_core-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-24 05:13:01.000000 river_core-1.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:13:21.000000 river_core-1.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-24 05:13:01.000000 river_core-1.3.0/examples/sample-config.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:13:21.000000 river_core-1.3.0/river_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    42036 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/rivercore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/sim_hookspecs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:13:21.000000 river_core-1.3.0/river_core/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/templates/coverage_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14432 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/templates/report.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:13:21.000000 river_core-1.3.0/river_core/templates/setup/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:13:21.000000 river_core-1.3.0/river_core/templates/setup/dut/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/templates/setup/dut/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:13:21.000000 river_core-1.3.0/river_core/templates/setup/dut/boot/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/templates/setup/dut/boot/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/templates/setup/dut/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/templates/setup/dut/gen_framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/templates/setup/dut/sample_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:13:21.000000 river_core-1.3.0/river_core/templates/setup/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/templates/setup/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/templates/setup/generator/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/templates/setup/generator/gen_framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/templates/setup/generator/sample_gen_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/templates/setup/generator/sample_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:13:21.000000 river_core-1.3.0/river_core/templates/setup/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/templates/setup/reference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/templates/setup/reference/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/templates/setup/reference/gen_framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/templates/setup/reference/sample_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/templates/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)    18787 2023-04-24 05:13:01.000000 river_core-1.3.0/river_core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 05:13:21.000000 river_core-1.3.0/river_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-24 05:13:20.000000 river_core-1.3.0/river_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-24 05:13:21.000000 river_core-1.3.0/river_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 05:13:20.000000 river_core-1.3.0/river_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-24 05:13:20.000000 river_core-1.3.0/river_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 05:13:20.000000 river_core-1.3.0/river_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-24 05:13:20.000000 river_core-1.3.0/river_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-24 05:13:20.000000 river_core-1.3.0/river_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-24 05:13:21.000000 river_core-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-24 05:13:01.000000 river_core-1.3.0/setup.py
```

### Comparing `river_core-1.2.0/CONTRIBUTING.rst` & `river_core-1.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `river_core-1.2.0/LICENSE.incore` & `river_core-1.3.0/LICENSE.incore`

 * *Files identical despite different names*

### Comparing `river_core-1.2.0/LICENSE.tessolve` & `river_core-1.3.0/LICENSE.tessolve`

 * *Files identical despite different names*

### Comparing `river_core-1.2.0/PKG-INFO` & `river_core-1.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: river_core
-Version: 1.2.0
+Version: 1.3.0
 Summary: RiVer Core Verification Framework
 Home-page: https://github.com/incoresemi/river_core
 Author: InCore Semiconductors Pvt. Ltd.; Tessolve
 Author-email: neelgala@incoresemi.com
 License: BSD-3-Clause
 Description: **RiVer Core** : RISC-V Core Verification Framework 
         ###################################################################################
```

### Comparing `river_core-1.2.0/examples/sample-config.ini` & `river_core-1.3.0/examples/sample-config.ini`

 * *Files identical despite different names*

### Comparing `river_core-1.2.0/river_core/constants.py` & `river_core-1.3.0/river_core/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,17 @@
     type: string
     nullable: True
     check_with: dircheck
   empty: True
 ignore_lines:
     type: integer
     default: 4
+self_checking:
+  type: boolean
+  default: False
 ''' #: This contains the schema for validation
 
 sample_config = '''
 [river_core]
 # Main directory for all files generated by river_core
 work_dir = mywork
```

### Comparing `river_core-1.2.0/river_core/log.py` & `river_core-1.3.0/river_core/log.py`

 * *Files identical despite different names*

### Comparing `river_core-1.2.0/river_core/main.py` & `river_core-1.3.0/river_core/main.py`

 * *Files identical despite different names*

### Comparing `river_core-1.2.0/river_core/rivercore.py` & `river_core-1.3.0/river_core/rivercore.py`

 * *Files 1% similar despite different names*

```diff
@@ -354,33 +354,36 @@
                 'Test List returned by the gen hook of Generator is of type: ' +
                 str(type(test_list)) + '. Expected Dict')
             raise SystemExit(1)
 
         generatorpm.hook.post_gen(
             output_dir='{0}/{1}'.format(output_dir, suite))
 
-    test_list_file = output_dir + '/test_list.yaml'
-    logger.info('Dumping generated Test-List at: ' + str(test_list_file))
-    testfile = open(test_list_file, 'w')
-    utils.yaml.dump(test_list, testfile)
-    testfile.close()
-
     logger.info('Validating Generated Test-List')
     testschema = yaml.load(testlist_schema)
     validator = YamlValidator(testschema)
     validator.allow_unknown = False
     for test, fields in test_list.items():
         valid = validator.validate(fields)
         if not valid:
             logger.error('Test List Validation failed:')
             error_list = validator.errors
             for x in error_list:
                 logger.error('{0} [ {1} ] : {2}'.format(test, x, error_list[x]))
             raise SystemExit(1)
+        test_list[test] = validator.normalized(fields, testschema)
     logger.info('Test List Validated successfully')
+    logger.info(f'Total Tests : {len(test_list)}')
+    
+    test_list_file = output_dir + '/test_list.yaml'
+    logger.info('Dumping generated Test-List at: ' + str(test_list_file))
+    testfile = open(test_list_file, 'w')
+    utils.yaml.dump(test_list, testfile)
+    testfile.close()
+
 
     # Open generation report in browser
     for suite in suite_list:
         report_html = str(output_dir) + '/reports/{0}.html'.format(suite)
         if utils.str_2_bool(config['river_core']['open_browser']):
             try:
                 import webbrowser
@@ -603,28 +606,36 @@
         if compare:
             test_dict = utils.load_yaml(test_list)
             gen_json_data = []
             target_json_data = []
             ref_json_data = []
             for test, attr in test_dict.items():
                 test_wd = attr['work_dir']
-                if not os.path.isfile(test_wd + '/dut.dump'):
-                    logger.error(f'{test:<30} : DUT dump is missing')
-                    test_dict[test]['result'] = 'Unavailable'
-                    test_dict[test]['log'] = "DUT dump is missing"
-                    success = False
-                    continue
-                if not os.path.isfile(test_wd + '/ref.dump'):
-                    logger.error(f'{test:<30} : REF dump is missing')
-                    test_dict[test]['result'] = 'Unavailable'
-                    test_dict[test]['log'] = "REF dump is missing"
-                    success = False
-                    continue
-                result, log = utils.compare_signature(test_wd + '/dut.dump',
-                                     test_wd + '/ref.dump')
+                if not attr['self_checking']:
+                  if not os.path.isfile(test_wd + '/dut.dump'):
+                      logger.error(f'{test:<30} : DUT dump is missing')
+                      test_dict[test]['result'] = 'Unavailable'
+                      test_dict[test]['log'] = "DUT dump is missing"
+                      success = False
+                      continue
+                  if not os.path.isfile(test_wd + '/ref.dump'):
+                      logger.error(f'{test:<30} : REF dump is missing')
+                      test_dict[test]['result'] = 'Unavailable'
+                      test_dict[test]['log'] = "REF dump is missing"
+                      success = False
+                      continue
+                  result, log = utils.compare_signature(test_wd + '/dut.dump', test_wd + '/ref.dump')
+                else:
+                  if not os.path.isfile(test_wd + 'dut.signature'):
+                      logger.error(f'{test:<30} : DUT signature is missing')
+                      test_dict[test]['result'] = 'Unavailable'
+                      test_dict[test]['log'] = "DUT signature is missing"
+                      success = False
+                      continue
+                  result, log = utils.self_check(test_wd + '/dut.signature')
                 test_dict[test]['result'] = result
                 test_dict[test]['log'] = log
                 if result == 'Passed':
                     logger.info(f"{test:<30} : TEST {result.upper()}")
                 else:
                     success = False
                     logger.error(f"{test:<30} : TEST {result.upper()}")
```

### Comparing `river_core-1.2.0/river_core/sim_hookspecs.py` & `river_core-1.3.0/river_core/sim_hookspecs.py`

 * *Files identical despite different names*

### Comparing `river_core-1.2.0/river_core/templates/coverage_report.html` & `river_core-1.3.0/river_core/templates/coverage_report.html`

 * *Files identical despite different names*

### Comparing `river_core-1.2.0/river_core/templates/report.html` & `river_core-1.3.0/river_core/templates/report.html`

 * *Files identical despite different names*

### Comparing `river_core-1.2.0/river_core/templates/setup/dut/gen_framework.py` & `river_core-1.3.0/river_core/templates/setup/dut/gen_framework.py`

 * *Files identical despite different names*

### Comparing `river_core-1.2.0/river_core/templates/setup/dut/sample_plugin.py` & `river_core-1.3.0/river_core/templates/setup/dut/sample_plugin.py`

 * *Files identical despite different names*

### Comparing `river_core-1.2.0/river_core/templates/setup/generator/gen_framework.py` & `river_core-1.3.0/river_core/templates/setup/generator/gen_framework.py`

 * *Files identical despite different names*

### Comparing `river_core-1.2.0/river_core/templates/setup/generator/sample_plugin.py` & `river_core-1.3.0/river_core/templates/setup/generator/sample_plugin.py`

 * *Files identical despite different names*

### Comparing `river_core-1.2.0/river_core/templates/setup/reference/gen_framework.py` & `river_core-1.3.0/river_core/templates/setup/reference/gen_framework.py`

 * *Files identical despite different names*

### Comparing `river_core-1.2.0/river_core/templates/setup/reference/sample_plugin.py` & `river_core-1.3.0/river_core/templates/setup/reference/sample_plugin.py`

 * *Files identical despite different names*

### Comparing `river_core-1.2.0/river_core/templates/style.css` & `river_core-1.3.0/river_core/templates/style.css`

 * *Files identical despite different names*

### Comparing `river_core-1.2.0/river_core/utils.py` & `river_core-1.3.0/river_core/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,29 @@
 import difflib
 import shlex
 
 yaml = YAML(typ="safe")
 yaml.default_flow_style = False
 yaml.allow_unicode = True
 
+def self_check(file1):
+  '''
+  Function to check if all values in the signature are 0s to indicate a pass,
+  else the test has failed.
+  '''
+  result = 'Passed'
+  rout = ''
+  with open('file1','r') as f:
+    for lineno, line in enumerate(f):
+      line_val = f'0x{line}'
+      if int(line_val,0) != 0:
+        result = 'Failed'
+        rout = f'\nLine:{lineno} has a non-zero value indicating a fail'
+  return result, rout
+
 def compare_signature(file1, file2):
     '''
         Function to check whether two signature files are equivalent. This funcion uses the
         :py:mod:`difflib` to perform the comparision and obtain the difference.
         :param file1: The path to the first signature.
         :param file2: The path to the second signature.
         :type file1: str
```

### Comparing `river_core-1.2.0/river_core.egg-info/PKG-INFO` & `river_core-1.3.0/river_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: river-core
-Version: 1.2.0
+Version: 1.3.0
 Summary: RiVer Core Verification Framework
 Home-page: https://github.com/incoresemi/river_core
 Author: InCore Semiconductors Pvt. Ltd.; Tessolve
 Author-email: neelgala@incoresemi.com
 License: BSD-3-Clause
 Description: **RiVer Core** : RISC-V Core Verification Framework 
         ###################################################################################
```

### Comparing `river_core-1.2.0/river_core.egg-info/SOURCES.txt` & `river_core-1.3.0/river_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `river_core-1.2.0/setup.py` & `river_core-1.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,10 +58,10 @@
         ]
     },
     setup_requires=setup_requirements,
     test_suite='',
     tests_require=test_requirements,
     url=
     'https://github.com/incoresemi/river_core',
-    version='1.2.0',
+    version='1.3.0',
     zip_safe=False,
 )
```


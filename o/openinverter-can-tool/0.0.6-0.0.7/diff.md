# Comparing `tmp/openinverter-can-tool-0.0.6.tar.gz` & `tmp/openinverter-can-tool-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openinverter-can-tool-0.0.6.tar", last modified: Fri Feb 24 16:38:48 2023, max compression
+gzip compressed data, was "openinverter-can-tool-0.0.7.tar", last modified: Mon Apr 24 16:59:17 2023, max compression
```

## Comparing `openinverter-can-tool-0.0.6.tar` & `openinverter-can-tool-0.0.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 16:38:48.404503 openinverter-can-tool-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-02-24 16:38:34.000000 openinverter-can-tool-0.0.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-02-24 16:38:48.404503 openinverter-can-tool-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-02-24 16:38:34.000000 openinverter-can-tool-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 16:38:48.400503 openinverter-can-tool-0.0.6/parameter-databases/
--rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-02-24 16:38:34.000000 openinverter-can-tool-0.0.6/parameter-databases/c2000-sine.5.14.R.C2000-foc.json
--rw-r--r--   0 runner    (1001) docker     (123)    13368 2023-02-24 16:38:34.000000 openinverter-can-tool-0.0.6/parameter-databases/c2000-sine.5.24.R.C2000-foc.json
--rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-02-24 16:38:34.000000 openinverter-can-tool-0.0.6/parameter-databases/stm32-sine.5.24.R-foc.json
--rw-r--r--   0 runner    (1001) docker     (123)    13596 2023-02-24 16:38:34.000000 openinverter-can-tool-0.0.6/parameter-databases/stm32-sine.5.24.R-sine.json
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-02-24 16:38:34.000000 openinverter-can-tool-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-24 16:38:48.404503 openinverter-can-tool-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-02-24 16:38:34.000000 openinverter-can-tool-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 16:38:48.400503 openinverter-can-tool-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 16:38:48.400503 openinverter-can-tool-0.0.6/src/openinverter_can_tool/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 16:38:34.000000 openinverter-can-tool-0.0.6/src/openinverter_can_tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-24 16:38:34.000000 openinverter-can-tool-0.0.6/src/openinverter_can_tool/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15026 2023-02-24 16:38:34.000000 openinverter-can-tool-0.0.6/src/openinverter_can_tool/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-02-24 16:38:34.000000 openinverter-can-tool-0.0.6/src/openinverter_can_tool/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-02-24 16:38:34.000000 openinverter-can-tool-0.0.6/src/openinverter_can_tool/fpfloat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-02-24 16:38:34.000000 openinverter-can-tool-0.0.6/src/openinverter_can_tool/paramdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 16:38:48.404503 openinverter-can-tool-0.0.6/src/openinverter_can_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-02-24 16:38:48.000000 openinverter-can-tool-0.0.6/src/openinverter_can_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-02-24 16:38:48.000000 openinverter-can-tool-0.0.6/src/openinverter_can_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 16:38:48.000000 openinverter-can-tool-0.0.6/src/openinverter_can_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-02-24 16:38:48.000000 openinverter-can-tool-0.0.6/src/openinverter_can_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-24 16:38:48.000000 openinverter-can-tool-0.0.6/src/openinverter_can_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-24 16:38:48.000000 openinverter-can-tool-0.0.6/src/openinverter_can_tool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 16:38:48.404503 openinverter-can-tool-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    12428 2023-02-24 16:38:34.000000 openinverter-can-tool-0.0.6/tests/test_paramdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:59:17.177675 openinverter-can-tool-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-24 16:59:06.000000 openinverter-can-tool-0.0.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-04-24 16:59:17.177675 openinverter-can-tool-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-04-24 16:59:06.000000 openinverter-can-tool-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:59:17.177675 openinverter-can-tool-0.0.7/parameter-databases/
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-04-24 16:59:06.000000 openinverter-can-tool-0.0.7/parameter-databases/c2000-sine.5.14.R.C2000-foc.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13703 2023-04-24 16:59:06.000000 openinverter-can-tool-0.0.7/parameter-databases/c2000-sine.5.24.R.C2000-foc.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13598 2023-04-24 16:59:06.000000 openinverter-can-tool-0.0.7/parameter-databases/stm32-sine.5.24.R-foc.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-04-24 16:59:06.000000 openinverter-can-tool-0.0.7/parameter-databases/stm32-sine.5.24.R-sine.json
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-24 16:59:06.000000 openinverter-can-tool-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-24 16:59:17.177675 openinverter-can-tool-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-24 16:59:06.000000 openinverter-can-tool-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:59:17.173675 openinverter-can-tool-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:59:17.177675 openinverter-can-tool-0.0.7/src/openinverter_can_tool/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 16:59:06.000000 openinverter-can-tool-0.0.7/src/openinverter_can_tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-24 16:59:06.000000 openinverter-can-tool-0.0.7/src/openinverter_can_tool/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15879 2023-04-24 16:59:06.000000 openinverter-can-tool-0.0.7/src/openinverter_can_tool/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-24 16:59:06.000000 openinverter-can-tool-0.0.7/src/openinverter_can_tool/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-24 16:59:06.000000 openinverter-can-tool-0.0.7/src/openinverter_can_tool/fpfloat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-04-24 16:59:06.000000 openinverter-can-tool-0.0.7/src/openinverter_can_tool/paramdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:59:17.177675 openinverter-can-tool-0.0.7/src/openinverter_can_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-04-24 16:59:17.000000 openinverter-can-tool-0.0.7/src/openinverter_can_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-24 16:59:17.000000 openinverter-can-tool-0.0.7/src/openinverter_can_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 16:59:17.000000 openinverter-can-tool-0.0.7/src/openinverter_can_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-24 16:59:17.000000 openinverter-can-tool-0.0.7/src/openinverter_can_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-24 16:59:17.000000 openinverter-can-tool-0.0.7/src/openinverter_can_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-24 16:59:17.000000 openinverter-can-tool-0.0.7/src/openinverter_can_tool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:59:17.177675 openinverter-can-tool-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17659 2023-04-24 16:59:06.000000 openinverter-can-tool-0.0.7/tests/test_paramdb.py
```

### Comparing `openinverter-can-tool-0.0.6/LICENSE.txt` & `openinverter-can-tool-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openinverter-can-tool-0.0.6/PKG-INFO` & `openinverter-can-tool-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openinverter-can-tool
-Version: 0.0.6
+Version: 0.0.7
 Summary: Tool to configure and operate openinverter systems over CAN
 Home-page: https://github.com/davefiddes/openinverter-can-tool
 Author: David J. Fiddes
 Author-email: D.J@fiddes.net
 Project-URL: Bug Reports, https://github.com/davefiddes/openinverter-can-tool/issues
 Project-URL: Source, https://github.com/davefiddes/openinverter-can-tool
 Keywords: openinverter,canopen
```

### Comparing `openinverter-can-tool-0.0.6/README.md` & `openinverter-can-tool-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `openinverter-can-tool-0.0.6/parameter-databases/c2000-sine.5.14.R.C2000-foc.json` & `openinverter-can-tool-0.0.7/parameter-databases/c2000-sine.5.14.R.C2000-foc.json`

 * *Files identical despite different names*

### Comparing `openinverter-can-tool-0.0.6/parameter-databases/c2000-sine.5.24.R.C2000-foc.json` & `openinverter-can-tool-0.0.7/parameter-databases/stm32-sine.5.24.R-foc.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986338797814208%*

 * *Differences: {"'lasterr'": "{'unit': '0=NONE, 1=OVERCURRENT, 2=THROTTLE1, 3=THROTTLE2, 4=CANTIMEOUT, "*

 * *              '5=EMCYSTOP, 6=MPROT, 7=DESAT, 8=OVERVOLTAGE, 9=ENCODER, 10=PRECHARGE, 11=TMPHSMAX, '*

 * *              '12=CURRENTLIMIT, 13=PWMSTUCK, 14=HICUROFS1, 15=HICUROFS2, 16=HIRESOFS, 17=LORESAMP, '*

 * *              "18=TMPMMAX,'}",*

 * * "'version'": "{'unit': '4=5.24.R-foc'}"}*

```diff
@@ -433,15 +433,15 @@
         "id": "2004",
         "isparam": false,
         "unit": "A"
     },
     "lasterr": {
         "id": "2038",
         "isparam": false,
-        "unit": "Empty"
+        "unit": "0=NONE, 1=OVERCURRENT, 2=THROTTLE1, 3=THROTTLE2, 4=CANTIMEOUT, 5=EMCYSTOP, 6=MPROT, 7=DESAT, 8=OVERVOLTAGE, 9=ENCODER, 10=PRECHARGE, 11=TMPHSMAX, 12=CURRENTLIMIT, 13=PWMSTUCK, 14=HICUROFS1, 15=HICUROFS2, 16=HIRESOFS, 17=LORESAMP, 18=TMPMMAX,"
     },
     "lqminusld": {
         "category": "Motor",
         "default": "0",
         "id": "139",
         "isparam": true,
         "maximum": "1000",
@@ -913,15 +913,15 @@
         "id": "2047",
         "isparam": false,
         "unit": "dig"
     },
     "version": {
         "id": "2039",
         "isparam": false,
-        "unit": "4=5.24.R.C2000-foc"
+        "unit": "4=5.24.R-foc"
     },
     "vlimflt": {
         "category": "Motor",
         "default": "10",
         "id": "145",
         "isparam": true,
         "maximum": "16",
```

### Comparing `openinverter-can-tool-0.0.6/parameter-databases/stm32-sine.5.24.R-foc.json` & `openinverter-can-tool-0.0.7/parameter-databases/c2000-sine.5.24.R.C2000-foc.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986338797814208%*

 * *Differences: {"'lasterr'": "{'unit': '0=NONE, 1=OVERCURRENT, 2=THROTTLE1, 3=THROTTLE2, 4=CANTIMEOUT, "*

 * *              '5=EMCYSTOP, 6=MPROT, 7=DESAT, 8=OVERVOLTAGE, 9=ENCODER, 10=PRECHARGE, 11=TMPHSMAX, '*

 * *              '12=CURRENTLIMIT, 13=PWMSTUCK, 14=HICUROFS1, 15=HICUROFS2, 16=HIRESOFS, 17=LORESAMP, '*

 * *              '18=TMPMMAX, 19=GATEDRIVEINITFAIL, 20=GATEDRIVEFAULT, 21=PMICINITFAIL, '*

 * *              "22=PMICRUNSTATEFAIL, 23=PMICSTROBEFAULT,'}",*

 * * "'version'": "{'unit': '4=5.24.R.C2000-foc'}"}*

```diff
@@ -433,15 +433,15 @@
         "id": "2004",
         "isparam": false,
         "unit": "A"
     },
     "lasterr": {
         "id": "2038",
         "isparam": false,
-        "unit": "Empty"
+        "unit": "0=NONE, 1=OVERCURRENT, 2=THROTTLE1, 3=THROTTLE2, 4=CANTIMEOUT, 5=EMCYSTOP, 6=MPROT, 7=DESAT, 8=OVERVOLTAGE, 9=ENCODER, 10=PRECHARGE, 11=TMPHSMAX, 12=CURRENTLIMIT, 13=PWMSTUCK, 14=HICUROFS1, 15=HICUROFS2, 16=HIRESOFS, 17=LORESAMP, 18=TMPMMAX, 19=GATEDRIVEINITFAIL, 20=GATEDRIVEFAULT, 21=PMICINITFAIL, 22=PMICRUNSTATEFAIL, 23=PMICSTROBEFAULT,"
     },
     "lqminusld": {
         "category": "Motor",
         "default": "0",
         "id": "139",
         "isparam": true,
         "maximum": "1000",
@@ -913,15 +913,15 @@
         "id": "2047",
         "isparam": false,
         "unit": "dig"
     },
     "version": {
         "id": "2039",
         "isparam": false,
-        "unit": "4=5.24.R-foc"
+        "unit": "4=5.24.R.C2000-foc"
     },
     "vlimflt": {
         "category": "Motor",
         "default": "10",
         "id": "145",
         "isparam": true,
         "maximum": "16",
```

### Comparing `openinverter-can-tool-0.0.6/parameter-databases/stm32-sine.5.24.R-sine.json` & `openinverter-can-tool-0.0.7/parameter-databases/stm32-sine.5.24.R-sine.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993333333333334%*

 * *Differences: {"'lasterr'": "{'unit': '0=NONE, 1=OVERCURRENT, 2=THROTTLE1, 3=THROTTLE2, 4=CANTIMEOUT, "*

 * *              '5=EMCYSTOP, 6=MPROT, 7=DESAT, 8=OVERVOLTAGE, 9=ENCODER, 10=PRECHARGE, 11=TMPHSMAX, '*

 * *              '12=CURRENTLIMIT, 13=PWMSTUCK, 14=HICUROFS1, 15=HICUROFS2, 16=HIRESOFS, 17=LORESAMP, '*

 * *              "18=TMPMMAX,'}"}*

```diff
@@ -524,15 +524,15 @@
         "id": "2005",
         "isparam": false,
         "unit": "A"
     },
     "lasterr": {
         "id": "2038",
         "isparam": false,
-        "unit": "Empty"
+        "unit": "0=NONE, 1=OVERCURRENT, 2=THROTTLE1, 3=THROTTLE2, 4=CANTIMEOUT, 5=EMCYSTOP, 6=MPROT, 7=DESAT, 8=OVERVOLTAGE, 9=ENCODER, 10=PRECHARGE, 11=TMPHSMAX, 12=CURRENTLIMIT, 13=PWMSTUCK, 14=HICUROFS1, 15=HICUROFS2, 16=HIRESOFS, 17=LORESAMP, 18=TMPMMAX,"
     },
     "nodeid": {
         "category": "Communication",
         "default": "1",
         "id": "129",
         "isparam": true,
         "maximum": "63",
```

### Comparing `openinverter-can-tool-0.0.6/setup.py` & `openinverter-can-tool-0.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 # Strip the build status as this only makes sense on github
 long_description = re.sub(r'\[!\[Build status.*\)\n\n', '', long_description)
 
 setup(
     name="openinverter-can-tool",
-    version="0.0.6",
+    version="0.0.7",
     description="Tool to configure and operate openinverter systems over CAN",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/davefiddes/openinverter-can-tool",
     author="David J. Fiddes",
     author_email="D.J@fiddes.net",
```

### Comparing `openinverter-can-tool-0.0.6/src/openinverter_can_tool/cli.py` & `openinverter-can-tool-0.0.7/src/openinverter_can_tool/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -172,41 +172,69 @@
                 f" - min: {fixed_to_float(item.min):g} "
                 f"max: {fixed_to_float(item.max):g} "
                 f"default: {fixed_to_float(item.default):g}")
         else:
             print(" - read-only value")
 
 
+def print_param(
+        variable: canopen.objectdictionary.Variable,
+        value: float) -> str:
+    """Print out the value of a parameter or outputs the enumeration value or
+    bits in a bitfield"""
+
+    click.echo(f"{variable.name:20}: ", nl=False)
+
+    if variable.value_descriptions:
+        if value in variable.value_descriptions:
+            click.echo(f"{variable.value_descriptions[value]}")
+        else:
+            click.echo(f"{value:g} (Unknown value)")
+    elif variable.bit_definitions:
+        value = int(value)
+        bit_str = ""
+        for bit, description in variable.bit_definitions.items():
+            if bit & value:
+                bit_str = bit_str + description + ", "
+        bit_str = bit_str.removesuffix(", ")
+
+        if len(bit_str) == 0:
+            bit_str = "0"
+
+        click.echo(f"{bit_str}")
+    else:
+        click.echo(
+            f"{value:g} [{variable.unit}]")
+
+
 @cli.command()
 @pass_cli_settings
 @db_action
 @can_action
 def dumpall(cli_settings: CliSettings):
     """Dump the values of all available parameters and values"""
 
     node = cli_settings.node
     for item in cli_settings.database.names.values():
-        click.echo(
-            f"{item.name:20}: {fixed_to_float(node.sdo[item.name].raw):10g} "
-            f"[{item.unit}]")
+        print_param(item, fixed_to_float(node.sdo[item.name].raw))
 
 
 @cli.command()
 @click.argument("param", required=True)
 @pass_cli_settings
 @db_action
 @can_action
 def read(cli_settings: CliSettings, param: str):
     """Read the value of PARAM from the device"""
 
     if param in cli_settings.database.names:
         node = cli_settings.node
-        click.echo(
-            f"{param}: {fixed_to_float(node.sdo[param].raw):g} "
-            f"[{cli_settings.database.names[param].unit}]")
+        print_param(
+            cli_settings.database.names[param],
+            fixed_to_float(node.sdo[param].raw))
     else:
         click.echo(f"Unknown parameter: {param}")
 
 
 @cli.command()
 @click.argument("params", required=True, nargs=-1)
 @click.argument("out_file", type=click.File("w"))
@@ -254,14 +282,15 @@
     while True:
         row = {}
         if timestamp:
             row["timestamp"] = str(datetime.datetime.now())
         for param in query_list:
             row[param] = f"{fixed_to_float(node.sdo[param].raw):g}"
         writer.writerow(row)
+        out_file.flush()
 
         time.sleep(step)
 
 
 @cli.command()
 @click.argument("out_file", type=click.File("w"))
 @pass_cli_settings
```

### Comparing `openinverter-can-tool-0.0.6/src/openinverter_can_tool/constants.py` & `openinverter-can-tool-0.0.7/src/openinverter_can_tool/constants.py`

 * *Files identical despite different names*

### Comparing `openinverter-can-tool-0.0.6/src/openinverter_can_tool/paramdb.py` & `openinverter-can-tool-0.0.7/src/openinverter_can_tool/paramdb.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,50 @@
 """
 openinverter parameter database functions
 """
 
 
 import json
-from typing import Tuple
+from typing import Tuple, Dict
 from canopen import objectdictionary, Network
 from canopen.sdo import SdoClient
 from .fpfloat import fixed_from_float
 from . import constants as oi
 
 
 def index_from_id(param_identifier: int) -> Tuple[int, int]:
     """Generate an index, subindex tuple from an openinverter parameter id"""
     index = 0x2100 | (param_identifier >> 8)
     subindex = param_identifier & 0xFF
     return (index, subindex)
 
 
+def is_power_of_two(num):
+    """Use some clever bitwise anding and arithmetic to determine wether a
+    number is a power of two"""
+    return (num != 0) and (num & (num - 1) == 0)
+
+
+def is_bitfield(values: Dict[int, str]) -> bool:
+    """Try to figure out if the dictionary of values is a bitfield or an
+    enumeration"""
+
+    for value in values:
+        # Ignore zero
+        if (value != 0) and (not is_power_of_two(value)):
+            return False
+
+    # When we only have two non-zero values we assume it's an enum not a
+    # bitfield
+    if len(values) <= 3:
+        return False
+    else:
+        return True
+
+
 def import_database_json(
         paramdb_json: dict) -> objectdictionary.ObjectDictionary:
     """Import an openinverter parameter database JSON.
 
     :param paramdb_json:
         A dictionary containing an openinverter parameter database
 
@@ -55,14 +78,34 @@
         var.isparam = param["isparam"]
 
         if "category" in param:
             var.category = param["category"]
         else:
             var.category = None
 
+        # parse units containing enumerations or bitfields
+        unit = param["unit"]
+        if '=' in unit:
+            # Some parameters like "lasterr" have trailing commas
+            unit = unit.rstrip(",")
+
+            values = {int(value): description for value, description in [
+                item.split('=') for item in unit.split(',')]}
+
+            # Ignore the expected type of the bit_definitions member and
+            # shove our dictionary in there if it is a bitfield otherwise treat
+            # as a list of value descriptions
+            if is_bitfield(values):
+                var.bit_definitions = values
+            else:
+                var.value_descriptions = values
+
+        # Store the unit text for all types of parameters
+        var.unit = unit
+
         # Parameters have additional required attributes
         if var.isparam:
             var.min = fixed_from_float(float(param["minimum"]))
             var.max = fixed_from_float(float(param["maximum"]))
             var.default = fixed_from_float(float(param["default"]))
 
         dictionary.add_object(var)
```

### Comparing `openinverter-can-tool-0.0.6/src/openinverter_can_tool.egg-info/PKG-INFO` & `openinverter-can-tool-0.0.7/src/openinverter_can_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openinverter-can-tool
-Version: 0.0.6
+Version: 0.0.7
 Summary: Tool to configure and operate openinverter systems over CAN
 Home-page: https://github.com/davefiddes/openinverter-can-tool
 Author: David J. Fiddes
 Author-email: D.J@fiddes.net
 Project-URL: Bug Reports, https://github.com/davefiddes/openinverter-can-tool/issues
 Project-URL: Source, https://github.com/davefiddes/openinverter-can-tool
 Keywords: openinverter,canopen
```

### Comparing `openinverter-can-tool-0.0.6/src/openinverter_can_tool.egg-info/SOURCES.txt` & `openinverter-can-tool-0.0.7/src/openinverter_can_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*


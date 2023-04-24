# Comparing `tmp/cagen-0.2.0a8.tar.gz` & `tmp/cagen-0.2.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cagen-0.2.0a8.tar", last modified: Mon Apr 24 07:43:26 2023, max compression
+gzip compressed data, was "cagen-0.2.0a9.tar", last modified: Mon Apr 24 07:50:58 2023, max compression
```

## Comparing `cagen-0.2.0a8.tar` & `cagen-0.2.0a9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-24 07:43:26.541017 cagen-0.2.0a8/
--rw-r--r--   0 xan       (1000) xan       (1000)      177 2023-03-28 18:54:19.000000 cagen-0.2.0a8/MANIFEST.in
--rw-r--r--   0 xan       (1000) xan       (1000)     4200 2023-04-24 07:43:26.541017 cagen-0.2.0a8/PKG-INFO
--rw-r--r--   0 xan       (1000) xan       (1000)     3465 2023-04-17 09:01:49.000000 cagen-0.2.0a8/README.md
--rw-r--r--   0 xan       (1000) xan       (1000)     1160 2023-04-17 09:02:06.000000 cagen-0.2.0a8/pyproject.toml
--rw-r--r--   0 xan       (1000) xan       (1000)       38 2023-04-24 07:43:26.541017 cagen-0.2.0a8/setup.cfg
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-24 07:43:26.537684 cagen-0.2.0a8/src/
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-24 07:43:26.537684 cagen-0.2.0a8/src/cagen/
--rw-r--r--   0 xan       (1000) xan       (1000)      112 2023-03-28 18:54:41.000000 cagen-0.2.0a8/src/cagen/__init__.py
--rw-r--r--   0 xan       (1000) xan       (1000)     4773 2023-04-16 21:18:58.000000 cagen-0.2.0a8/src/cagen/cmd.py
--rw-r--r--   0 xan       (1000) xan       (1000)     8539 2023-04-24 07:42:52.000000 cagen-0.2.0a8/src/cagen/libcagen.py
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-24 07:43:26.541017 cagen-0.2.0a8/src/cagen/templates/
--rw-r--r--   0 xan       (1000) xan       (1000)      414 2023-04-17 11:16:34.000000 cagen-0.2.0a8/src/cagen/templates/list.md.tmpl
--rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:41.000000 cagen-0.2.0a8/src/cagen/templates/list.md.tmpl.license
--rw-r--r--   0 xan       (1000) xan       (1000)     1782 2023-04-17 20:18:26.000000 cagen-0.2.0a8/src/cagen/templates/schema.tmpl
--rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:48.000000 cagen-0.2.0a8/src/cagen/templates/schema.tmpl.license
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-24 07:43:26.541017 cagen-0.2.0a8/src/cagen.egg-info/
--rw-r--r--   0 xan       (1000) xan       (1000)     4200 2023-04-24 07:43:26.000000 cagen-0.2.0a8/src/cagen.egg-info/PKG-INFO
--rw-r--r--   0 xan       (1000) xan       (1000)      443 2023-04-24 07:43:26.000000 cagen-0.2.0a8/src/cagen.egg-info/SOURCES.txt
--rw-r--r--   0 xan       (1000) xan       (1000)        1 2023-04-24 07:43:26.000000 cagen-0.2.0a8/src/cagen.egg-info/dependency_links.txt
--rw-r--r--   0 xan       (1000) xan       (1000)      114 2023-04-24 07:43:26.000000 cagen-0.2.0a8/src/cagen.egg-info/entry_points.txt
--rw-r--r--   0 xan       (1000) xan       (1000)       53 2023-04-24 07:43:26.000000 cagen-0.2.0a8/src/cagen.egg-info/requires.txt
--rw-r--r--   0 xan       (1000) xan       (1000)        6 2023-04-24 07:43:26.000000 cagen-0.2.0a8/src/cagen.egg-info/top_level.txt
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-24 07:50:58.233893 cagen-0.2.0a9/
+-rw-r--r--   0 xan       (1000) xan       (1000)      177 2023-03-28 18:54:19.000000 cagen-0.2.0a9/MANIFEST.in
+-rw-r--r--   0 xan       (1000) xan       (1000)     4200 2023-04-24 07:50:58.233893 cagen-0.2.0a9/PKG-INFO
+-rw-r--r--   0 xan       (1000) xan       (1000)     3465 2023-04-17 09:01:49.000000 cagen-0.2.0a9/README.md
+-rw-r--r--   0 xan       (1000) xan       (1000)     1160 2023-04-24 07:48:37.000000 cagen-0.2.0a9/pyproject.toml
+-rw-r--r--   0 xan       (1000) xan       (1000)       38 2023-04-24 07:50:58.233893 cagen-0.2.0a9/setup.cfg
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-24 07:50:58.233893 cagen-0.2.0a9/src/
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-24 07:50:58.233893 cagen-0.2.0a9/src/cagen/
+-rw-r--r--   0 xan       (1000) xan       (1000)      112 2023-03-28 18:54:41.000000 cagen-0.2.0a9/src/cagen/__init__.py
+-rw-r--r--   0 xan       (1000) xan       (1000)     4682 2023-04-24 07:50:44.000000 cagen-0.2.0a9/src/cagen/cmd.py
+-rw-r--r--   0 xan       (1000) xan       (1000)     8539 2023-04-24 07:42:52.000000 cagen-0.2.0a9/src/cagen/libcagen.py
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-24 07:50:58.233893 cagen-0.2.0a9/src/cagen/templates/
+-rw-r--r--   0 xan       (1000) xan       (1000)      414 2023-04-17 11:16:34.000000 cagen-0.2.0a9/src/cagen/templates/list.md.tmpl
+-rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:41.000000 cagen-0.2.0a9/src/cagen/templates/list.md.tmpl.license
+-rw-r--r--   0 xan       (1000) xan       (1000)     1782 2023-04-17 20:18:26.000000 cagen-0.2.0a9/src/cagen/templates/schema.tmpl
+-rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:48.000000 cagen-0.2.0a9/src/cagen/templates/schema.tmpl.license
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-24 07:50:58.233893 cagen-0.2.0a9/src/cagen.egg-info/
+-rw-r--r--   0 xan       (1000) xan       (1000)     4200 2023-04-24 07:50:58.000000 cagen-0.2.0a9/src/cagen.egg-info/PKG-INFO
+-rw-r--r--   0 xan       (1000) xan       (1000)      443 2023-04-24 07:50:58.000000 cagen-0.2.0a9/src/cagen.egg-info/SOURCES.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)        1 2023-04-24 07:50:58.000000 cagen-0.2.0a9/src/cagen.egg-info/dependency_links.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)      114 2023-04-24 07:50:58.000000 cagen-0.2.0a9/src/cagen.egg-info/entry_points.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)       53 2023-04-24 07:50:58.000000 cagen-0.2.0a9/src/cagen.egg-info/requires.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)        6 2023-04-24 07:50:58.000000 cagen-0.2.0a9/src/cagen.egg-info/top_level.txt
```

### Comparing `cagen-0.2.0a8/PKG-INFO` & `cagen-0.2.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cagen
-Version: 0.2.0a8
+Version: 0.2.0a9
 Summary: A static site generator for cmpalgorithms project
 Author: Xavier B.
 Project-URL: Homepage, https://repo.or.cz/cagen.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `cagen-0.2.0a8/README.md` & `cagen-0.2.0a9/README.md`

 * *Files identical despite different names*

### Comparing `cagen-0.2.0a8/pyproject.toml` & `cagen-0.2.0a9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 [project.scripts]
 cagen = "cagen.cmd:cagen_cli"
 cagen-list = "cagen.cmd:cagen_list"
 cagen-make = "cagen.cmd:cagen_make"
 
 [project]
 name = "cagen"
-version = "0.2.0.alpha-8"
+version = "0.2.0.alpha-9"
 authors = [{'name'="Xavier B."}]
 description = "A static site generator for cmpalgorithms project"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
         'Development Status :: 3 - Alpha',
         'Environment :: Console',
```

### Comparing `cagen-0.2.0a8/src/cagen/cmd.py` & `cagen-0.2.0a9/src/cagen/cmd.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,36 +9,32 @@
 import os.path
 from mako.template import Template
 
 def cagen_cli():
     """Defines the `cagen` command line script function to call from pyproject.toml"""
 
     parser = argparse.ArgumentParser(prog = "cagen", description="static site generator for cmpalgorithms project", epilog="For better processing, please put the options and the end of the call of the program.")
-    parser.add_argument("source", type=str, help="the source markdown file")
+    parser.add_argument("--source", type=str, help="the source markdown file. It could be None. In this case, it renders Template with --metadata fields to `to` path")
     parser.add_argument("to", type=str, help="destination file")
     parser.add_argument("template", type=str, help="Mako template file path")
     parser.add_argument("--syntax", type=str, default='html5', help="syntax of destination file. By default 'html5'")
     parser.add_argument("--metadata", type=str, nargs='*', help="extra metadata provided to template. In the form variable=value variable2=value2 ...")
     parser.add_argument("--evals", type=str, nargs='*', help="evals with `eval()` python function the specified metadata variables. Eg. if `--metadata foo=2.0` and `--eval foo`, then the foo variable is the float 2.0, not the string '2.0'.")
     args = parser.parse_args()
 
     # Conversion
-    entry = libcagen.Entry(args.source)
-    if os.path.exists(args.source):
-        if os.path.exists(args.template):
-            with open(args.to, "w") as f:
-                assignments=libcagen.extract_assignments(args.metadata)
-                evals=args.evals
-                eassignments=libcagen.evaluate_assignments(assignments, evals)
-                f.write(entry.to(mytemplatepath=args.template, additionalsearchlist=eassignments, destsyntax=args.syntax))
-                print("{} -> {} ({}) using {}".format(args.source, args.to, args.syntax, args.template))
-        else:
-            print("Template {} not found".format(args.template))
+    if os.path.exists(args.template):
+        with open(args.to, "w") as f:
+            assignments=libcagen.extract_assignments(args.metadata)
+            evals=args.evals
+            eassignments=libcagen.evaluate_assignments(assignments, evals)
+            f.write(entry.to(mytemplatepath=args.template, additionalsearchlist=eassignments, destsyntax=args.syntax))
+            print("{} -> {} ({}) using {}".format(args.source, args.to, args.syntax, args.template))
     else:
-        print("File {} does not exist".format(args.source))
+        print("Template {} not found".format(args.template))
 
 
 def cagen_list():
     """Defines the `cagen-list` command line script function to call from pyproject.toml"""
 
     parser = argparse.ArgumentParser(prog = "cagen-list", description="make a list of entries in Markdown format and it saves it in a file")
     parser.add_argument("template", type=str, help="Mako template to use")
```

### Comparing `cagen-0.2.0a8/src/cagen/libcagen.py` & `cagen-0.2.0a9/src/cagen/libcagen.py`

 * *Files identical despite different names*

### Comparing `cagen-0.2.0a8/src/cagen/templates/schema.tmpl` & `cagen-0.2.0a9/src/cagen/templates/schema.tmpl`

 * *Files identical despite different names*

### Comparing `cagen-0.2.0a8/src/cagen.egg-info/PKG-INFO` & `cagen-0.2.0a9/src/cagen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cagen
-Version: 0.2.0a8
+Version: 0.2.0a9
 Summary: A static site generator for cmpalgorithms project
 Author: Xavier B.
 Project-URL: Homepage, https://repo.or.cz/cagen.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```


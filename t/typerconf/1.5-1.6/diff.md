# Comparing `tmp/typerconf-1.5.tar.gz` & `tmp/typerconf-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typerconf-1.5.tar", max compression
+gzip compressed data, was "typerconf-1.6.tar", max compression
```

## Comparing `typerconf-1.5.tar` & `typerconf-1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1074 2023-03-22 18:19:29.446288 typerconf-1.5/LICENSE
--rw-r--r--   0        0        0     1363 2023-03-24 07:02:49.103915 typerconf-1.5/README.md
--rw-r--r--   0        0        0      934 2023-04-23 09:48:23.436444 typerconf-1.5/pyproject.toml
--rw-r--r--   0        0        0       30 2023-03-23 10:49:11.282231 typerconf-1.5/src/typerconf/.gitignore
--rw-r--r--   0        0        0      258 2023-03-22 14:14:56.966915 typerconf-1.5/src/typerconf/Makefile
--rw-r--r--   0        0        0     6567 2023-04-23 09:48:55.900330 typerconf-1.5/src/typerconf/__init__.py
--rw-r--r--   0        0        0    19038 2023-04-23 09:43:51.934399 typerconf-1.5/src/typerconf/init.nw
--rw-r--r--   0        0        0     2508 1970-01-01 00:00:00.000000 typerconf-1.5/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-03-22 18:19:29.446288 typerconf-1.6/LICENSE
+-rw-r--r--   0        0        0     1363 2023-03-24 07:02:49.103915 typerconf-1.6/README.md
+-rw-r--r--   0        0        0      934 2023-04-24 11:24:19.016149 typerconf-1.6/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-03-23 10:49:11.282231 typerconf-1.6/src/typerconf/.gitignore
+-rw-r--r--   0        0        0      258 2023-03-22 14:14:56.966915 typerconf-1.6/src/typerconf/Makefile
+-rw-r--r--   0        0        0     7868 2023-04-24 11:23:52.596126 typerconf-1.6/src/typerconf/__init__.py
+-rw-r--r--   0        0        0    21976 2023-04-24 11:22:10.264030 typerconf-1.6/src/typerconf/init.nw
+-rw-r--r--   0        0        0     2508 1970-01-01 00:00:00.000000 typerconf-1.6/PKG-INFO
```

### Comparing `typerconf-1.5/LICENSE` & `typerconf-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `typerconf-1.5/README.md` & `typerconf-1.6/README.md`

 * *Files identical despite different names*

### Comparing `typerconf-1.5/pyproject.toml` & `typerconf-1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "typerconf"
-version = "1.5"
+version = "1.6"
 description = "Library to read and write configs using API and CLI with Typer"
 authors = ["Daniel Bosk <daniel@bosk.se>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dbosk/typerconf"
 keywords = ["typer", "conf", "config", "git-like", "config lib", "write conf"]
 classifiers = [
```

### Comparing `typerconf-1.5/src/typerconf/__init__.py` & `typerconf-1.6/src/typerconf/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """The typerconf module and config subcommand"""
 
 import appdirs
+import io
 import json
 import logging
 import os
 import sys
 import typer
 import typing
 
@@ -116,43 +117,66 @@
 
         paths.append(path)
         paths += self.paths(from_root=path)
     elif isinstance(root, list):
       paths += [f"{from_root}.{x}" for x in range(len(root))]
 
     return paths
-  def read_config(self, conf_path=f"{dirs.user_config_dir}/config.json"):
+  def read_config(self, conf_file=f"{dirs.user_config_dir}/config.json"):
     """
     Reads the config data structure (JSON) into the Config object.
-    `conf_path` is an optional argument providing the path to the config file.
-
-    
+    `conf_file` is an optional argument providing one of the following:
+    - an already opened file object (anything derived from `io.IOBase`);
+    - anything that `open` can handle, for instance:
+      - a string, which is the path to the config file;
+      - an integer, which is a file descriptor (see `os.open`).
+
+    Errors:
+
+    - The first is that the file doesn't exist ([[FileNotFoundError]]).
+    - There is also a related one, [[NotADirectoryError]]. The problem of 
+      [[NotADirectoryError]] occurs when a file on the path is used as a directory 
+      --- but only for reading, when trying to create a directory hierarchy, it 
+      will yield [[FileExistsError]]. We can't recover from this error, as an 
+      attempt to write to the file will also fail.
+    - Finally, the file exists, but it's not proper JSON ([[JSONDecodeError]]).
     """
-    try:
-      with open(conf_path) as conf_file:
-        self.__data = json.load(conf_file)
-        return
-    except FileNotFoundError as err:
-      logging.warning(f"Config file {conf_path} could not be found: {err}")
-    except NotADirectoryError as err:
-      logging.error(f"A part of the path is a file, but used as directory: {err}")
-      raise err
-    except json.decoder.JSONDecodeError as err:
-      logging.warning(f"Config file {conf_path} could not be decoded: {err}")
-  def write_config(self, conf_path=f"{dirs.user_config_dir}/config.json"):
+    if isinstance(conf_file, io.IOBase):
+      self.__data = json.load(conf_file)
+    else:
+      try:
+        with open(conf_file) as conf_file:
+          self.__data = json.load(conf_file)
+          return
+      except FileNotFoundError as err:
+        raise FileNotFoundError(f"Config file {conf_file} could not be found: {err}")
+      except NotADirectoryError as err:
+        raise NotADirectoryError(f"A part of the path is a file, "
+                                 f"but used as directory: {err}")
+      except json.decoder.JSONDecodeError as err:
+        raise ValueError(f"Config file {conf_file} "
+                         f"could not be decoded: {err}")
+  def write_config(self, conf_file=f"{dirs.user_config_dir}/config.json"):
     """
     Stores the config data (as JSON) in the config file.
-    `conf_path` is an optional argument providing the path to the config file.
+    `conf_file` is an optional argument providing one of the following:
+    - an already opened file object (anything derived from `io.IOBase`);
+    - anything that `open` can handle, for instance:
+      - a string, which is the path to the config file;
+      - an integer, which is a file descriptor (see `os.open`).
     """
-    conf_dir = os.path.dirname(conf_path)
-    if not os.path.isdir(conf_dir):
-      os.makedirs(conf_dir)
-
-    with open(conf_path, "w") as conf_file:
+    if isinstance(conf_file, io.IOBase):
       json.dump(self.__data, conf_file)
+    else:
+      conf_dir = os.path.dirname(conf_file)
+      if not os.path.isdir(conf_dir):
+        os.makedirs(conf_dir)
+
+      with open(conf_file, "w") as conf_file:
+        json.dump(self.__data, conf_file)
 def add_config_cmd(cli: typer.Typer):
   """
   Add config command to Typer cli
   """
   path_arg = typer.Argument(...,
                             help="Path in config, e.g. 'courses.datintro22'. "
                                  "Empty string is root of config.",
```

### Comparing `typerconf-1.5/src/typerconf/init.nw` & `typerconf-1.6/src/typerconf/init.nw`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 \section{Code outline}\label{configmodule}
 
 The base structure is standard.
 <<init.py>>=
 """The typerconf module and config subcommand"""
 
 import appdirs
+import io
 import json
 import logging
 import os
 import sys
 import typer
 import typing
 
@@ -129,22 +130,23 @@
   <<Config methods for get and set>>
   <<Config methods for available paths>>
   <<Config methods for reading from and writing to file>>
 @
 
 We will use the following test data for the test functions.
 <<test functions>>=
-conf = Config({
+test_data = {
   "courses": {
     "datintro22": {
       "url": "https://...",
       "TAs": ["Asse", "Assa"]
     }
   }
-})
+}
+conf = Config(test_data)
 @
 
 \subsection{Getting and setting values}
 
 We want to be able to get and set values at different paths in the config.
 <<Config methods for get and set>>=
 def get(self, path: str = "") -> typing.Any:
@@ -365,98 +367,196 @@
   assert "courses.datintro22.TAs" in conf.paths()
   for path in conf.paths():
     assert conf.get(path)
 @
 
 \subsection{Reading and writing the config file}\label{ConfigFile}
 
+We want to be able to read a config file stored in the system.
+We have two cases.
+
+The first case is the default config file.
 The configuration file is stored in a suitable system location.
 We use the AppDirs package for the default location, we have the [[dirs]] 
 instance above.
 We want to read the config and load the JSON structure as outlined above 
 (\cref{ConfigStructure}).
+
+The second case is that we want to open another file of our liking.
+
+We will take the file as an argument.
+The default will be the path to the default config file.
+Then we can just specify a different path to open another file.
+However, sometimes we want to read from an already opened file, so we will also 
+accept anything that [[open]] would accept.
+
+\subsubsection{Reading the config}
+
+Let's start with reading.
+Anything that is derived from [[io.IOBase]] is already opened.
+Anything else, we pass to [[open]] to handle.
 <<Config methods for reading from and writing to file>>=
-def read_config(self, conf_path=f"{dirs.user_config_dir}/config.json"):
+def read_config(self, conf_file=f"{dirs.user_config_dir}/config.json"):
   """
   Reads the config data structure (JSON) into the Config object.
-  `conf_path` is an optional argument providing the path to the config file.
+  <<[[conf_file]] argument doc>>
 
   <<documentation of config read error handling>>
   """
-  try:
-    with open(conf_path) as conf_file:
-      self.__data = json.load(conf_file)
-      return
-  <<handle read config file errors>>
+  if isinstance(conf_file, io.IOBase):
+    <<read the data into [[self.__data]]>>
+  else:
+    <<open and read the config file>>
+<<[[conf_file]] argument doc>>=
+`conf_file` is an optional argument providing one of the following:
+- an already opened file object (anything derived from `io.IOBase`);
+- anything that `open` can handle, for instance:
+  - a string, which is the path to the config file;
+  - an integer, which is a file descriptor (see `os.open`).
+@
+
+Let's start with the short one.
+To read the data, we simply use the [[json]] library to turn the file contents 
+into a dictionary.
+<<read the data into [[self.__data]]>>=
+self.__data = json.load(conf_file)
+@
+
+If we must open the file ourselves, we simply do that.
+But we do it in such a way that we can reuse
+[[<<read the data into [[self.__data]]>>]].
+<<open and read the config file>>=
+try:
+  with open(conf_file) as conf_file:
+    <<read the data into [[self.__data]]>>
+    return
+<<handle read config file errors>>
 @
 
-And conversely, write one to the config file as well.
-Here it's important to use the [[os.makedirs]] (not [[os.mkdir]]) to create the 
-entire hierarchy of parent directories too, if they don't exist.
-We don't need any error handling for writing though, because all errors are 
-fatal, we can't recover from any of the possible errors.
-<<Config methods for reading from and writing to file>>=
-def write_config(self, conf_path=f"{dirs.user_config_dir}/config.json"):
-  """
-  Stores the config data (as JSON) in the config file.
-  `conf_path` is an optional argument providing the path to the config file.
-  """
-  conf_dir = os.path.dirname(conf_path)
-  if not os.path.isdir(conf_dir):
-    os.makedirs(conf_dir)
+Let's test this functionality.
+<<test functions>>=
+def test_read_config():
+  tmp = tempfile.mkdtemp()
+  tmp_conf = f"{tmp}/config.json"
+  with open(tmp_conf, "w") as conf_file:
+    json.dump(test_data, conf_file)
 
-  with open(conf_path, "w") as conf_file:
-    json.dump(self.__data, conf_file)
+  conf = Config()
+  conf.read_config(tmp_conf)
+  assert "https://..." in conf.get("courses.datintro22.url")
+
+  conf = Config()
+  with open(tmp_conf) as conf_file:
+    conf.read_config(conf_file)
+  assert "https://..." in conf.get("courses.datintro22.url")
+<<test imports>>=
+import tempfile
 @
 
+\subsubsection{Reading errors}
+
 When reading the config file there are some errors that can occur.
-The first is that the file doesn't exist ([[FileNotFoundError]]).
-There is also a related one, [[NotADirectoryError]].
-The problem of [[NotADirectoryError]] occurs when a file on the path is used as 
-a directory --- but only for reading, when trying to create a directory 
-hierarchy, it will yield [[FileExistsError]].
-We can't recover from this error, as an attempt to write to the file will also 
-fail.
-Finally, the file exists, but it's not proper JSON ([[JSONDecodeError]]).
+We catch them and rephrase the error messages.
+We turn the [[json.JSONDecodeError]] into a [[ValueError]] too.
+<<documentation of config read error handling>>=
+Errors:
+
+- The first is that the file doesn't exist ([[FileNotFoundError]]).
+- There is also a related one, [[NotADirectoryError]]. The problem of 
+  [[NotADirectoryError]] occurs when a file on the path is used as a directory 
+  --- but only for reading, when trying to create a directory hierarchy, it 
+  will yield [[FileExistsError]]. We can't recover from this error, as an 
+  attempt to write to the file will also fail.
+- Finally, the file exists, but it's not proper JSON ([[JSONDecodeError]]).
 <<handle read config file errors>>=
 except FileNotFoundError as err:
-  logging.warning(f"Config file {conf_path} could not be found: {err}")
+  raise FileNotFoundError(f"Config file {conf_file} could not be found: {err}")
 except NotADirectoryError as err:
-  logging.error(f"A part of the path is a file, but used as directory: {err}")
-  raise err
+  raise NotADirectoryError(f"A part of the path is a file, "
+                           f"but used as directory: {err}")
 except json.decoder.JSONDecodeError as err:
-  logging.warning(f"Config file {conf_path} could not be decoded: {err}")
-@
-
-<<documentation of config read error handling>>=
+  raise ValueError(f"Config file {conf_file} "
+                   f"could not be decoded: {err}")
 @
 
 Now, let's test the read errors.
 <<test functions>>=
 def test_conf_read_errors():
-  """FileNotFoundError"""
   conf = Config()
-  conf.read_config("/this/path/should/never/exist/config.json")
-  """JSONDecodeError"""
-  conf.read_config("/dev/null")
-  """NotADirectoryError"""
+  try:
+    conf.read_config("/this/path/should/never/exist/config.json")
+  except FileNotFoundError:
+    assert True
+  else:
+    assert False
+  try:
+    conf.read_config("/dev/null")
+  except ValueError:
+    assert True
+  else:
+    assert False
   try:
     conf.read_config("/dev/null/config.json")
   except NotADirectoryError:
     assert True
   else:
     assert False
 @
 
+\subsubsection{Writing the config}
+
+Conversely, we want to write the data to the config file as well.
+We do the same things as above, but open for writing instead.
+<<Config methods for reading from and writing to file>>=
+def write_config(self, conf_file=f"{dirs.user_config_dir}/config.json"):
+  """
+  Stores the config data (as JSON) in the config file.
+  <<[[conf_file]] argument doc>>
+  """
+  if isinstance(conf_file, io.IOBase):
+    <<write the data from [[self.__data]]>>
+  else:
+    <<open and write the config file>>
+@
+
+Writing to the file is simply to use [[json.dump]].
+<<write the data from [[self.__data]]>>=
+json.dump(self.__data, conf_file)
+@
+
+Now, how do we open the file?
+We want to create the file if it doesn't exist.
+Here it's important to use the [[os.makedirs]] (not [[os.mkdir]]) to create the 
+entire hierarchy of parent directories too, if they don't exist.
+We don't need any error handling for writing though, because all errors are 
+fatal, we can't recover from any of the possible errors.
+<<open and write the config file>>=
+conf_dir = os.path.dirname(conf_file)
+if not os.path.isdir(conf_dir):
+  os.makedirs(conf_dir)
+
+with open(conf_file, "w") as conf_file:
+  <<write the data from [[self.__data]]>>
+@
+
+Let's test this.
+<<test functions>>=
+def test_write_config():
+  conf = Config(test_data)
+  conf.write_config("/dev/null")
+  with open("/dev/null", "w") as conf_file:
+    conf.write_config(conf_file)
+  with open(os.open("/dev/null", os.O_WRONLY), "w") as conf_file:
+    conf.write_config(conf_file)
+@
+
 Writing to the config file can also yield errors.
 <<test functions>>=
 def test_conf_write_errors():
   conf = Config({})
-  """Should succeed"""
-  conf.write_config("/dev/null")
   """Should yield FileExistsError"""
   try:
     conf.write_config("/dev/null/config.json")
   except NotADirectoryError:
     assert False
   except FileExistsError:
     assert True
@@ -468,16 +568,14 @@
   except PermissionError:
     assert True
   else:
     assert False
   """Should succeed"""
   path = tempfile.mkdtemp()
   conf.write_config(f"{path}/this/is/a/new/path/config.json")
-<<test imports>>=
-import tempfile
 @
 
 
 \section{Accessing the default configuration:
   the [[get]] and [[set]] functions}
 
 We will provide two module-level functions, [[get]] and [[set]], that allows
```

### Comparing `typerconf-1.5/PKG-INFO` & `typerconf-1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typerconf
-Version: 1.5
+Version: 1.6
 Summary: Library to read and write configs using API and CLI with Typer
 Home-page: https://github.com/dbosk/typerconf
 License: MIT
 Keywords: typer,conf,config,git-like,config lib,write conf
 Author: Daniel Bosk
 Author-email: daniel@bosk.se
 Requires-Python: >=3.7,<4.0
```


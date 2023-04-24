# Comparing `tmp/MomentumX-2.6.4.tar.gz` & `tmp/MomentumX-2.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MomentumX-2.6.4.tar", last modified: Wed Apr 12 13:24:07 2023, max compression
+gzip compressed data, was "MomentumX-2.6.5.tar", last modified: Mon Apr 24 15:55:41 2023, max compression
```

## Comparing `MomentumX-2.6.4.tar` & `MomentumX-2.6.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-04-12 13:24:07.301698 MomentumX-2.6.4/
--rw-rw-r--   0 developer  (1000) developer  (1000)      143 2023-02-05 03:27:25.000000 MomentumX-2.6.4/.clang-format
--rw-rw-r--   0 developer  (1000) developer  (1000)       39 2023-01-04 18:56:42.000000 MomentumX-2.6.4/.dockerignore
--rw-rw-r--   0 developer  (1000) developer  (1000)       93 2023-03-02 22:42:30.000000 MomentumX-2.6.4/.gitignore
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-04-12 13:24:07.295286 MomentumX-2.6.4/.vscode/
--rw-rw-r--   0 developer  (1000) developer  (1000)      280 2023-03-02 22:42:30.000000 MomentumX-2.6.4/.vscode/settings.json
--rw-rw-r--   0 developer  (1000) developer  (1000)     1968 2023-03-09 18:12:19.000000 MomentumX-2.6.4/CMakeLists.txt
--rw-rw-r--   0 developer  (1000) developer  (1000)    35149 2022-05-19 01:23:36.000000 MomentumX-2.6.4/LICENSE
--rwxrwxr-x   0 developer  (1000) developer  (1000)     6518 2023-01-10 14:44:56.000000 MomentumX-2.6.4/Logo.png
--rw-rw-r--   0 developer  (1000) developer  (1000)     1359 2023-03-09 18:12:19.000000 MomentumX-2.6.4/Makefile
--rw-rw-r--   0 developer  (1000) developer  (1000)     7125 2023-04-12 13:24:07.301698 MomentumX-2.6.4/PKG-INFO
--rw-rw-r--   0 developer  (1000) developer  (1000)     6667 2023-03-10 16:59:42.000000 MomentumX-2.6.4/README.md
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-04-12 13:24:07.297118 MomentumX-2.6.4/examples/
--rw-rw-r--   0 developer  (1000) developer  (1000)     1675 2023-03-09 18:12:19.000000 MomentumX-2.6.4/examples/multi.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     1120 2023-03-09 18:12:19.000000 MomentumX-2.6.4/examples/stream_reader.py
--rwxrwxr-x   0 developer  (1000) developer  (1000)      865 2023-03-09 18:12:19.000000 MomentumX-2.6.4/examples/stream_writer.py
--rw-rw-r--   0 developer  (1000) developer  (1000)      762 2023-04-12 13:12:35.000000 MomentumX-2.6.4/examples/sync_reader.py
--rwxrwxr-x   0 developer  (1000) developer  (1000)      583 2023-04-12 13:12:35.000000 MomentumX-2.6.4/examples/sync_writer.py
--rw-rw-r--   0 developer  (1000) developer  (1000)      943 2023-03-09 18:12:19.000000 MomentumX-2.6.4/examples/threaded.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-04-12 13:24:07.298950 MomentumX-2.6.4/ext/
--rw-rw-r--   0 developer  (1000) developer  (1000)    22185 2023-03-10 16:20:18.000000 MomentumX-2.6.4/ext/binding.cpp
--rw-rw-r--   0 developer  (1000) developer  (1000)     6517 2023-03-09 18:12:19.000000 MomentumX-2.6.4/ext/buffer.cpp
--rw-rw-r--   0 developer  (1000) developer  (1000)     4214 2023-03-09 18:12:19.000000 MomentumX-2.6.4/ext/buffer.h
--rw-rw-r--   0 developer  (1000) developer  (1000)     4748 2023-03-10 15:53:52.000000 MomentumX-2.6.4/ext/context.cpp
--rw-rw-r--   0 developer  (1000) developer  (1000)     1467 2023-03-10 15:53:52.000000 MomentumX-2.6.4/ext/context.h
--rw-rw-r--   0 developer  (1000) developer  (1000)    21067 2023-04-12 13:12:35.000000 MomentumX-2.6.4/ext/stream.cpp
--rw-rw-r--   0 developer  (1000) developer  (1000)     5141 2023-03-10 15:53:52.000000 MomentumX-2.6.4/ext/stream.h
--rw-rw-r--   0 developer  (1000) developer  (1000)     9498 2023-03-09 18:12:19.000000 MomentumX-2.6.4/ext/utils.h
--rw-rw-r--   0 developer  (1000) developer  (1000)      126 2023-01-05 01:48:10.000000 MomentumX-2.6.4/pyproject.toml
--rw-rw-r--   0 developer  (1000) developer  (1000)       38 2023-04-12 13:24:07.301698 MomentumX-2.6.4/setup.cfg
--rw-rw-r--   0 developer  (1000) developer  (1000)     1023 2023-04-12 13:13:27.000000 MomentumX-2.6.4/setup.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-04-12 13:24:07.290705 MomentumX-2.6.4/src/
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-04-12 13:24:07.299866 MomentumX-2.6.4/src/MomentumX.egg-info/
--rw-rw-r--   0 developer  (1000) developer  (1000)     7125 2023-04-12 13:24:07.000000 MomentumX-2.6.4/src/MomentumX.egg-info/PKG-INFO
--rw-rw-r--   0 developer  (1000) developer  (1000)      665 2023-04-12 13:24:07.000000 MomentumX-2.6.4/src/MomentumX.egg-info/SOURCES.txt
--rw-rw-r--   0 developer  (1000) developer  (1000)        1 2023-04-12 13:24:07.000000 MomentumX-2.6.4/src/MomentumX.egg-info/dependency_links.txt
--rw-rw-r--   0 developer  (1000) developer  (1000)       21 2023-04-12 13:24:07.000000 MomentumX-2.6.4/src/MomentumX.egg-info/requires.txt
--rw-rw-r--   0 developer  (1000) developer  (1000)       10 2023-04-12 13:24:07.000000 MomentumX-2.6.4/src/MomentumX.egg-info/top_level.txt
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-04-12 13:24:07.300782 MomentumX-2.6.4/src/momentumx/
--rw-rw-r--   0 developer  (1000) developer  (1000)       20 2023-03-02 22:39:27.000000 MomentumX-2.6.4/src/momentumx/__init__.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     4607 2023-04-12 13:16:01.000000 MomentumX-2.6.4/src/momentumx/_mx.pyi
--rw-rw-r--   0 developer  (1000) developer  (1000)        0 2023-03-17 18:13:12.000000 MomentumX-2.6.4/src/momentumx/cli.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-04-12 13:24:07.300782 MomentumX-2.6.4/tests/
--rw-rw-r--   0 developer  (1000) developer  (1000)    27378 2023-04-12 13:12:35.000000 MomentumX-2.6.4/tests/test_scenarios.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-04-24 15:55:41.847183 MomentumX-2.6.5/
+-rw-rw-r--   0 developer  (1000) developer  (1000)      143 2023-02-05 03:27:25.000000 MomentumX-2.6.5/.clang-format
+-rw-rw-r--   0 developer  (1000) developer  (1000)       39 2023-01-04 18:56:42.000000 MomentumX-2.6.5/.dockerignore
+-rw-rw-r--   0 developer  (1000) developer  (1000)       93 2023-03-02 22:42:30.000000 MomentumX-2.6.5/.gitignore
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-04-24 15:55:41.841183 MomentumX-2.6.5/.vscode/
+-rw-rw-r--   0 developer  (1000) developer  (1000)      280 2023-03-02 22:42:30.000000 MomentumX-2.6.5/.vscode/settings.json
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1968 2023-03-09 18:12:19.000000 MomentumX-2.6.5/CMakeLists.txt
+-rw-rw-r--   0 developer  (1000) developer  (1000)    35149 2022-05-19 01:23:36.000000 MomentumX-2.6.5/LICENSE
+-rwxrwxr-x   0 developer  (1000) developer  (1000)     6518 2023-01-10 14:44:56.000000 MomentumX-2.6.5/Logo.png
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1359 2023-03-09 18:12:19.000000 MomentumX-2.6.5/Makefile
+-rw-rw-r--   0 developer  (1000) developer  (1000)     7125 2023-04-24 15:55:41.847183 MomentumX-2.6.5/PKG-INFO
+-rw-rw-r--   0 developer  (1000) developer  (1000)     6667 2023-03-10 16:59:42.000000 MomentumX-2.6.5/README.md
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-04-24 15:55:41.844183 MomentumX-2.6.5/examples/
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1675 2023-03-09 18:12:19.000000 MomentumX-2.6.5/examples/multi.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1120 2023-03-09 18:12:19.000000 MomentumX-2.6.5/examples/stream_reader.py
+-rwxrwxr-x   0 developer  (1000) developer  (1000)      865 2023-03-09 18:12:19.000000 MomentumX-2.6.5/examples/stream_writer.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)      762 2023-04-12 13:12:35.000000 MomentumX-2.6.5/examples/sync_reader.py
+-rwxrwxr-x   0 developer  (1000) developer  (1000)      583 2023-04-12 13:12:35.000000 MomentumX-2.6.5/examples/sync_writer.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1024 2023-04-24 15:44:52.000000 MomentumX-2.6.5/examples/threaded.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-04-24 15:55:41.845183 MomentumX-2.6.5/ext/
+-rw-rw-r--   0 developer  (1000) developer  (1000)    22135 2023-04-24 15:44:52.000000 MomentumX-2.6.5/ext/binding.cpp
+-rw-rw-r--   0 developer  (1000) developer  (1000)     6517 2023-03-09 18:12:19.000000 MomentumX-2.6.5/ext/buffer.cpp
+-rw-rw-r--   0 developer  (1000) developer  (1000)     4214 2023-03-09 18:12:19.000000 MomentumX-2.6.5/ext/buffer.h
+-rw-rw-r--   0 developer  (1000) developer  (1000)     4748 2023-03-10 15:53:52.000000 MomentumX-2.6.5/ext/context.cpp
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1467 2023-03-10 15:53:52.000000 MomentumX-2.6.5/ext/context.h
+-rw-rw-r--   0 developer  (1000) developer  (1000)    21067 2023-04-12 13:12:35.000000 MomentumX-2.6.5/ext/stream.cpp
+-rw-rw-r--   0 developer  (1000) developer  (1000)     5141 2023-03-10 15:53:52.000000 MomentumX-2.6.5/ext/stream.h
+-rw-rw-r--   0 developer  (1000) developer  (1000)     9498 2023-03-09 18:12:19.000000 MomentumX-2.6.5/ext/utils.h
+-rw-rw-r--   0 developer  (1000) developer  (1000)      133 2023-04-24 15:44:52.000000 MomentumX-2.6.5/pyproject.toml
+-rw-rw-r--   0 developer  (1000) developer  (1000)       38 2023-04-24 15:55:41.847183 MomentumX-2.6.5/setup.cfg
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1023 2023-04-24 15:47:16.000000 MomentumX-2.6.5/setup.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-04-24 15:55:41.837183 MomentumX-2.6.5/src/
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-04-24 15:55:41.846183 MomentumX-2.6.5/src/MomentumX.egg-info/
+-rw-rw-r--   0 developer  (1000) developer  (1000)     7125 2023-04-24 15:55:41.000000 MomentumX-2.6.5/src/MomentumX.egg-info/PKG-INFO
+-rw-rw-r--   0 developer  (1000) developer  (1000)      665 2023-04-24 15:55:41.000000 MomentumX-2.6.5/src/MomentumX.egg-info/SOURCES.txt
+-rw-rw-r--   0 developer  (1000) developer  (1000)        1 2023-04-24 15:55:41.000000 MomentumX-2.6.5/src/MomentumX.egg-info/dependency_links.txt
+-rw-rw-r--   0 developer  (1000) developer  (1000)       21 2023-04-24 15:55:41.000000 MomentumX-2.6.5/src/MomentumX.egg-info/requires.txt
+-rw-rw-r--   0 developer  (1000) developer  (1000)       10 2023-04-24 15:55:41.000000 MomentumX-2.6.5/src/MomentumX.egg-info/top_level.txt
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-04-24 15:55:41.846183 MomentumX-2.6.5/src/momentumx/
+-rw-rw-r--   0 developer  (1000) developer  (1000)       20 2023-03-02 22:39:27.000000 MomentumX-2.6.5/src/momentumx/__init__.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     4607 2023-04-24 15:48:19.000000 MomentumX-2.6.5/src/momentumx/_mx.pyi
+-rw-rw-r--   0 developer  (1000) developer  (1000)        0 2023-03-17 18:13:12.000000 MomentumX-2.6.5/src/momentumx/cli.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-04-24 15:55:41.846183 MomentumX-2.6.5/tests/
+-rw-rw-r--   0 developer  (1000) developer  (1000)    27378 2023-04-12 13:12:35.000000 MomentumX-2.6.5/tests/test_scenarios.py
```

### Comparing `MomentumX-2.6.4/CMakeLists.txt` & `MomentumX-2.6.5/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.4/LICENSE` & `MomentumX-2.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.4/Logo.png` & `MomentumX-2.6.5/Logo.png`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.4/Makefile` & `MomentumX-2.6.5/Makefile`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.4/PKG-INFO` & `MomentumX-2.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MomentumX
-Version: 2.6.4
+Version: 2.6.5
 Summary: Zero-copy shared memory IPC library for building complex streaming data pipelines capable of processing large datasets
 Home-page: https://github.com/captivationsoftware/MomentumX
 Author: Captivation Software, LLC
 Keywords: shm,shared memory,zero-copy,numpy,big data,scipy,pubsub,pipeline
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `MomentumX-2.6.4/README.md` & `MomentumX-2.6.5/README.md`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.4/examples/multi.py` & `MomentumX-2.6.5/examples/multi.py`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.4/examples/stream_reader.py` & `MomentumX-2.6.5/examples/stream_reader.py`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.4/examples/stream_writer.py` & `MomentumX-2.6.5/examples/stream_writer.py`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.4/examples/sync_reader.py` & `MomentumX-2.6.5/examples/sync_reader.py`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.4/examples/sync_writer.py` & `MomentumX-2.6.5/examples/sync_writer.py`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.4/examples/threaded.py` & `MomentumX-2.6.5/examples/threaded.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,25 +3,28 @@
 
 import momentumx as mx
 
 STREAM = "mx://threaded"
 
 def consumer(cancel: threading.Event):
     time.sleep(1)
-    stream = mx.Consumer(STREAM, cancel, context='/tmp')
+    stream = mx.Consumer(STREAM, cancel)
 
-    while not cancel.is_set():
-        string = stream.receive_string()
-        if string:
-            print("Received:", string)
+    for string in iter(stream.receive_string, None):
+        print("Received:", string)
+        if cancel.is_set():
+            break
     cancel.set()
 
 
 def producer(cancel: threading.Event):
-    stream = mx.Producer(STREAM, 100, 10, True, cancel, context='/tmp')
+    stream = mx.Producer(STREAM, 100, 10, True, cancel)
+    while stream.subscriber_count == 0:
+        if cancel.wait(0.1):
+            raise Exception("Canceled")
     i = 0
     while i < 1000 and not cancel.is_set():
         if stream.send_string(str(i)):
             print("Sent: ", i)
             i += 1
     
     time.sleep(1)
```

### Comparing `MomentumX-2.6.4/ext/binding.cpp` & `MomentumX-2.6.5/ext/binding.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -29,16 +29,14 @@
 
 struct BufferShim;
 struct BufferShim;
 struct ReadBufferShim;
 struct StreamShim;
 struct WriteBufferShim;
 
-static py::bytes END_OF_STREAM{"END_OF_STREAM"};
-
 struct StreamExistsException : public std::exception {
     const char* what() const noexcept override { return "Stream already exists"; }
 };
 
 struct StreamUnavailableException : public std::exception {
     const char* what() const noexcept override { return "Failed to create stream subscription"; }
 };
```

### Comparing `MomentumX-2.6.4/ext/buffer.cpp` & `MomentumX-2.6.5/ext/buffer.cpp`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.4/ext/buffer.h` & `MomentumX-2.6.5/ext/buffer.h`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.4/ext/context.cpp` & `MomentumX-2.6.5/ext/context.cpp`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.4/ext/context.h` & `MomentumX-2.6.5/ext/context.h`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.4/ext/stream.cpp` & `MomentumX-2.6.5/ext/stream.cpp`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.4/ext/stream.h` & `MomentumX-2.6.5/ext/stream.h`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.4/ext/utils.h` & `MomentumX-2.6.5/ext/utils.h`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.4/setup.py` & `MomentumX-2.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages
 from skbuild import setup
 
-__version__ = "2.6.4"
+__version__ = "2.6.5"
 
 from pathlib import Path
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name="MomentumX",
     version=__version__,
```

### Comparing `MomentumX-2.6.4/src/MomentumX.egg-info/PKG-INFO` & `MomentumX-2.6.5/src/MomentumX.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MomentumX
-Version: 2.6.4
+Version: 2.6.5
 Summary: Zero-copy shared memory IPC library for building complex streaming data pipelines capable of processing large datasets
 Home-page: https://github.com/captivationsoftware/MomentumX
 Author: Captivation Software, LLC
 Keywords: shm,shared memory,zero-copy,numpy,big data,scipy,pubsub,pipeline
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `MomentumX-2.6.4/src/MomentumX.egg-info/SOURCES.txt` & `MomentumX-2.6.5/src/MomentumX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.4/src/momentumx/_mx.pyi` & `MomentumX-2.6.5/src/momentumx/_mx.pyi`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.4/tests/test_scenarios.py` & `MomentumX-2.6.5/tests/test_scenarios.py`

 * *Files identical despite different names*


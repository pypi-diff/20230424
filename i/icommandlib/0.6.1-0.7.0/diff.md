# Comparing `tmp/icommandlib-0.6.1.tar.gz` & `tmp/icommandlib-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icommandlib-0.6.1.tar", last modified: Sat Apr  8 16:26:27 2023, max compression
+gzip compressed data, was "icommandlib-0.7.0.tar", last modified: Mon Apr 24 14:37:06 2023, max compression
```

## Comparing `icommandlib-0.6.1.tar` & `icommandlib-0.7.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 16:26:27.233124 icommandlib-0.6.1/
--rw-r--r--   0 root         (0) root         (0)     1057 2023-04-08 16:26:00.000000 icommandlib-0.6.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      154 2023-04-08 16:26:00.000000 icommandlib-0.6.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1184 2023-04-08 16:26:27.233124 icommandlib-0.6.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      395 2023-04-08 16:26:00.000000 icommandlib-0.6.1/README.md
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-08 16:26:00.000000 icommandlib-0.6.1/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 16:26:27.233124 icommandlib-0.6.1/icommandlib/
--rw-r--r--   0 root         (0) root         (0)      216 2023-04-08 16:26:00.000000 icommandlib-0.6.1/icommandlib/__init__.py
--rw-r--r--   0 root         (0) root         (0)      919 2023-04-08 16:26:00.000000 icommandlib-0.6.1/icommandlib/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1416 2023-04-08 16:26:00.000000 icommandlib-0.6.1/icommandlib/icommand.py
--rw-r--r--   0 root         (0) root         (0)     8025 2023-04-08 16:26:00.000000 icommandlib-0.6.1/icommandlib/iprocess.py
--rw-r--r--   0 root         (0) root         (0)     1705 2023-04-08 16:26:00.000000 icommandlib-0.6.1/icommandlib/messages.py
--rw-r--r--   0 root         (0) root         (0)     1939 2023-04-08 16:26:00.000000 icommandlib-0.6.1/icommandlib/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 16:26:27.233124 icommandlib-0.6.1/icommandlib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1184 2023-04-08 16:26:27.000000 icommandlib-0.6.1/icommandlib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      382 2023-04-08 16:26:27.000000 icommandlib-0.6.1/icommandlib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-08 16:26:27.000000 icommandlib-0.6.1/icommandlib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       77 2023-04-08 16:26:27.000000 icommandlib-0.6.1/icommandlib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-08 16:26:27.000000 icommandlib-0.6.1/icommandlib.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1136 2023-04-08 16:26:00.000000 icommandlib-0.6.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-08 16:26:27.233124 icommandlib-0.6.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-08 16:26:00.000000 icommandlib-0.6.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 14:37:06.337705 icommandlib-0.7.0/
+-rw-r--r--   0 root         (0) root         (0)     1524 2023-04-24 14:36:39.000000 icommandlib-0.7.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     3861 2023-04-24 14:36:39.000000 icommandlib-0.7.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2023-04-24 14:36:39.000000 icommandlib-0.7.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3150 2023-04-24 14:37:06.337705 icommandlib-0.7.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2361 2023-04-24 14:36:39.000000 icommandlib-0.7.0/README.md
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-24 14:36:39.000000 icommandlib-0.7.0/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 14:37:06.333705 icommandlib-0.7.0/icommandlib/
+-rw-r--r--   0 root         (0) root         (0)      216 2023-04-24 14:36:39.000000 icommandlib-0.7.0/icommandlib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      919 2023-04-24 14:36:39.000000 icommandlib-0.7.0/icommandlib/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1416 2023-04-24 14:36:39.000000 icommandlib-0.7.0/icommandlib/icommand.py
+-rw-r--r--   0 root         (0) root         (0)     8395 2023-04-24 14:36:39.000000 icommandlib-0.7.0/icommandlib/iprocess.py
+-rw-r--r--   0 root         (0) root         (0)     1705 2023-04-24 14:36:39.000000 icommandlib-0.7.0/icommandlib/messages.py
+-rw-r--r--   0 root         (0) root         (0)     1939 2023-04-24 14:36:39.000000 icommandlib-0.7.0/icommandlib/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 14:37:06.337705 icommandlib-0.7.0/icommandlib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3150 2023-04-24 14:37:06.000000 icommandlib-0.7.0/icommandlib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      395 2023-04-24 14:37:06.000000 icommandlib-0.7.0/icommandlib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 14:37:06.000000 icommandlib-0.7.0/icommandlib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2023-04-24 14:37:06.000000 icommandlib-0.7.0/icommandlib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-24 14:37:06.000000 icommandlib-0.7.0/icommandlib.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1136 2023-04-24 14:36:39.000000 icommandlib-0.7.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 14:37:06.337705 icommandlib-0.7.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 14:36:39.000000 icommandlib-0.7.0/setup.py
```

### Comparing `icommandlib-0.6.1/icommandlib/exceptions.py` & `icommandlib-0.7.0/icommandlib/exceptions.py`

 * *Files identical despite different names*

### Comparing `icommandlib-0.6.1/icommandlib/icommand.py` & `icommandlib-0.7.0/icommandlib/icommand.py`

 * *Files identical despite different names*

### Comparing `icommandlib-0.6.1/icommandlib/iprocess.py` & `icommandlib-0.7.0/icommandlib/iprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,18 @@
         self.raw_bytes += string
 
     @property
     def display(self):
         return self.screen.display
 
     @property
+    def stripshot(self):
+        return stripshot(self.text)
+
+    @property
     def text(self):
         return "\n".join(self.display)
 
 
 class IProcess(object):
     """
     An interactive process.
@@ -171,14 +175,24 @@
         """
 
         def on_screen(iscreen):
             return len([line for line in iscreen.display if text in line]) > 0
 
         self.wait_until(on_screen, timeout)
 
+    def wait_for_stripshot_to_match(self, text, timeout=None):
+        """
+        Wait until the text specified matches exactly the
+        process's current stripshot.
+        """
+        self.wait_until(
+            lambda iscreen: text == iscreen.stripshot,
+            timeout,
+        )
+
     def send_keys(self, text):
         """
         Send keys to the terminal process.
         """
         if self.running:
             self._ptyprocess.write(text)
         else:
```

### Comparing `icommandlib-0.6.1/icommandlib/messages.py` & `icommandlib-0.7.0/icommandlib/messages.py`

 * *Files identical despite different names*

### Comparing `icommandlib-0.6.1/icommandlib/utils.py` & `icommandlib-0.7.0/icommandlib/utils.py`

 * *Files identical despite different names*

### Comparing `icommandlib-0.6.1/pyproject.toml` & `icommandlib-0.7.0/pyproject.toml`

 * *Files identical despite different names*


# Comparing `tmp/img-host-0.1.1.tar.gz` & `tmp/img-host-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "img-host-0.1.1.tar", last modified: Mon Apr 24 09:46:36 2023, max compression
+gzip compressed data, was "img-host-0.1.2.tar", last modified: Mon Apr 24 09:49:03 2023, max compression
```

## Comparing `img-host-0.1.1.tar` & `img-host-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       59 2023-04-24 09:44:17.976526 img-host-0.1.1/img_host/__init__.py
--rw-r--r--   0        0        0      924 2023-04-24 09:39:00.640631 img-host-0.1.1/img_host/editor.py
--rw-r--r--   0        0        0      680 2023-04-24 09:41:52.736557 img-host-0.1.1/img_host/load.py
--rw-r--r--   0        0        0      256 2023-04-24 09:22:44.438773 img-host-0.1.1/img_host/main.py
--rw-r--r--   0        0        0      515 2023-04-24 09:46:27.889144 img-host-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      124 2023-04-24 09:28:30.273623 img-host-0.1.1/README.md
--rw-r--r--   0        0        0      290 2023-04-24 09:46:19.335003 img-host-0.1.1/tests/__main__.py
--rw-r--r--   0        0        0      302 1970-01-01 00:00:00.000000 img-host-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       95 2023-04-24 09:48:56.545900 img-host-0.1.2/img_host/__init__.py
+-rw-r--r--   0        0        0      924 2023-04-24 09:48:56.561416 img-host-0.1.2/img_host/editor.py
+-rw-r--r--   0        0        0      680 2023-04-24 09:41:52.736557 img-host-0.1.2/img_host/load.py
+-rw-r--r--   0        0        0      256 2023-04-24 09:22:44.438773 img-host-0.1.2/img_host/main.py
+-rw-r--r--   0        0        0      515 2023-04-24 09:49:00.436447 img-host-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      124 2023-04-24 09:28:30.273623 img-host-0.1.2/README.md
+-rw-r--r--   0        0        0      290 2023-04-24 09:47:44.157591 img-host-0.1.2/tests/__main__.py
+-rw-r--r--   0        0        0      302 1970-01-01 00:00:00.000000 img-host-0.1.2/PKG-INFO
```

### Comparing `img-host-0.1.1/img_host/editor.py` & `img-host-0.1.2/img_host/editor.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,14 +22,14 @@
         box = int(left_edge), 0, int(right_edge), height
         self._img = self._img.crop(box)
 
     @property
     def crop_width(self) -> float:
         value = self._img.height * self._ratio
         if self._img.width < value:
-            raise PhotoTooNarrow
+            raise ImageTooNarrow
         return value
 
 
-class PhotoTooNarrow(ValueError):
+class ImageTooNarrow(ValueError):
     def __str__(self) -> str:
         return "Image is too narrow."
```

### Comparing `img-host-0.1.1/img_host/load.py` & `img-host-0.1.2/img_host/load.py`

 * *Files identical despite different names*

### Comparing `img-host-0.1.1/pyproject.toml` & `img-host-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "img-host"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = [
     { name = "levch", email = "levchenko.d.a1998@gmail.com" },
 ]
 dependencies = [
     "httpx>=0.24.0",
     "pillow>=9.5.0",
```


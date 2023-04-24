# Comparing `tmp/RFTLib-0.1.1.tar.gz` & `tmp/RFTLib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RFTLib-0.1.1.tar", last modified: Sat Apr 15 17:47:19 2023, max compression
+gzip compressed data, was "RFTLib-0.2.0.tar", last modified: Mon Apr 24 03:11:13 2023, max compression
```

## Comparing `RFTLib-0.1.1.tar` & `RFTLib-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 17:47:19.129803 RFTLib-0.1.1/
--rw-rw-rw-   0        0        0    35831 2023-04-15 17:07:00.000000 RFTLib-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      327 2023-04-15 17:47:19.128804 RFTLib-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-15 16:47:53.000000 RFTLib-0.1.1/README.md
--rw-rw-rw-   0        0        0      455 2023-04-15 17:44:48.000000 RFTLib-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-15 17:47:19.130804 RFTLib-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-15 17:47:18.890806 RFTLib-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 17:47:18.900801 RFTLib-0.1.1/src/RFTLib/
-drwxrwxrwx   0        0        0        0 2023-04-15 17:47:19.090801 RFTLib-0.1.1/src/RFTLib/Config/
--rw-rw-rw-   0        0        0     2144 2023-04-11 14:27:13.000000 RFTLib-0.1.1/src/RFTLib/Config/__init__.py
--rw-rw-rw-   0        0        0      922 2023-04-07 03:02:41.000000 RFTLib-0.1.1/src/RFTLib/Config/cv2.py
--rw-rw-rw-   0        0        0      608 2023-04-07 03:02:48.000000 RFTLib-0.1.1/src/RFTLib/Config/json.py
--rw-rw-rw-   0        0        0      275 2023-04-07 03:00:50.000000 RFTLib-0.1.1/src/RFTLib/Config/loader.py
--rw-rw-rw-   0        0        0     1003 2023-04-07 03:02:58.000000 RFTLib-0.1.1/src/RFTLib/Config/pillow.py
--rw-rw-rw-   0        0        0      671 2023-04-11 14:23:04.000000 RFTLib-0.1.1/src/RFTLib/Config/python.py
--rw-rw-rw-   0        0        0     1197 2023-04-07 03:03:04.000000 RFTLib-0.1.1/src/RFTLib/Config/qt.py
--rw-rw-rw-   0        0        0      662 2023-04-07 03:03:24.000000 RFTLib-0.1.1/src/RFTLib/Config/rypple.py
--rw-rw-rw-   0        0        0      451 2023-04-07 03:03:31.000000 RFTLib-0.1.1/src/RFTLib/Config/text.py
--rw-rw-rw-   0        0        0      514 2023-04-07 03:03:39.000000 RFTLib-0.1.1/src/RFTLib/Config/toml.py
--rw-rw-rw-   0        0        0      559 2023-04-07 03:03:47.000000 RFTLib-0.1.1/src/RFTLib/Config/yaml.py
-drwxrwxrwx   0        0        0        0 2023-04-15 17:47:19.122821 RFTLib-0.1.1/src/RFTLib/Core/
--rw-rw-rw-   0        0        0     1935 2023-04-07 03:04:01.000000 RFTLib-0.1.1/src/RFTLib/Core/Buffer.py
--rw-rw-rw-   0        0        0     3503 2023-04-07 03:04:46.000000 RFTLib-0.1.1/src/RFTLib/Core/Object.py
--rw-rw-rw-   0        0        0      403 2023-04-07 03:04:52.000000 RFTLib-0.1.1/src/RFTLib/Core/Parser.py
--rw-rw-rw-   0        0        0     3435 2023-04-13 14:09:32.000000 RFTLib-0.1.1/src/RFTLib/Core/Structure.py
--rw-rw-rw-   0        0        0      938 2023-04-07 03:04:57.000000 RFTLib-0.1.1/src/RFTLib/Core/Types.py
--rw-rw-rw-   0        0        0      172 2023-04-07 03:06:25.000000 RFTLib-0.1.1/src/RFTLib/Require.py
-drwxrwxrwx   0        0        0        0 2023-04-15 17:47:19.125811 RFTLib-0.1.1/src/RFTLib/Saves/
--rw-rw-rw-   0        0        0      205 2023-04-07 03:05:09.000000 RFTLib-0.1.1/src/RFTLib/Saves/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 17:47:18.931862 RFTLib-0.1.1/src/RFTLib.egg-info/
--rw-rw-rw-   0        0        0      327 2023-04-15 17:47:18.000000 RFTLib-0.1.1/src/RFTLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      646 2023-04-15 17:47:18.000000 RFTLib-0.1.1/src/RFTLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 17:47:18.000000 RFTLib-0.1.1/src/RFTLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-15 17:47:18.000000 RFTLib-0.1.1/src/RFTLib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 03:11:13.923050 RFTLib-0.2.0/
+-rw-rw-rw-   0        0        0    35831 2023-04-15 17:07:00.000000 RFTLib-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      327 2023-04-24 03:11:13.922051 RFTLib-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-15 16:47:53.000000 RFTLib-0.2.0/README.md
+-rw-rw-rw-   0        0        0      478 2023-04-24 03:09:44.000000 RFTLib-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-24 03:11:13.924050 RFTLib-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-24 03:11:13.536049 RFTLib-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-24 03:11:13.716049 RFTLib-0.2.0/src/RFTLib/
+drwxrwxrwx   0        0        0        0 2023-04-24 03:11:13.754093 RFTLib-0.2.0/src/RFTLib/Config/
+-rw-rw-rw-   0        0        0     2144 2023-04-11 14:27:13.000000 RFTLib-0.2.0/src/RFTLib/Config/__init__.py
+-rw-rw-rw-   0        0        0      924 2023-04-23 14:48:39.000000 RFTLib-0.2.0/src/RFTLib/Config/cv2.py
+-rw-rw-rw-   0        0        0      610 2023-04-23 14:48:36.000000 RFTLib-0.2.0/src/RFTLib/Config/json.py
+-rw-rw-rw-   0        0        0      275 2023-04-07 03:00:50.000000 RFTLib-0.2.0/src/RFTLib/Config/loader.py
+-rw-rw-rw-   0        0        0     1005 2023-04-23 14:48:31.000000 RFTLib-0.2.0/src/RFTLib/Config/pillow.py
+-rw-rw-rw-   0        0        0      673 2023-04-23 14:48:43.000000 RFTLib-0.2.0/src/RFTLib/Config/python.py
+-rw-rw-rw-   0        0        0     1199 2023-04-23 14:48:46.000000 RFTLib-0.2.0/src/RFTLib/Config/qt.py
+-rw-rw-rw-   0        0        0      664 2023-04-23 14:48:49.000000 RFTLib-0.2.0/src/RFTLib/Config/rypple.py
+-rw-rw-rw-   0        0        0      453 2023-04-23 14:48:54.000000 RFTLib-0.2.0/src/RFTLib/Config/text.py
+-rw-rw-rw-   0        0        0      522 2023-04-23 19:45:30.000000 RFTLib-0.2.0/src/RFTLib/Config/toml.py
+-rw-rw-rw-   0        0        0      561 2023-04-23 14:48:59.000000 RFTLib-0.2.0/src/RFTLib/Config/yaml.py
+drwxrwxrwx   0        0        0        0 2023-04-24 03:11:13.876049 RFTLib-0.2.0/src/RFTLib/Core/
+-rw-rw-rw-   0        0        0     2673 2023-04-23 15:48:26.000000 RFTLib-0.2.0/src/RFTLib/Core/Buffer.py
+drwxrwxrwx   0        0        0        0 2023-04-24 03:11:13.882050 RFTLib-0.2.0/src/RFTLib/Core/Gui/
+-rw-rw-rw-   0        0        0     2670 2023-04-23 21:59:43.000000 RFTLib-0.2.0/src/RFTLib/Core/Gui/Color.py
+-rw-rw-rw-   0        0        0     1751 2023-04-23 21:22:38.000000 RFTLib-0.2.0/src/RFTLib/Core/Gui/Text.py
+-rw-rw-rw-   0        0        0     3509 2023-04-23 19:38:57.000000 RFTLib-0.2.0/src/RFTLib/Core/Object.py
+-rw-rw-rw-   0        0        0     1822 2023-04-23 15:53:45.000000 RFTLib-0.2.0/src/RFTLib/Core/Parser.py
+-rw-rw-rw-   0        0        0     3882 2023-04-23 12:55:57.000000 RFTLib-0.2.0/src/RFTLib/Core/Structure.py
+-rw-rw-rw-   0        0        0     3688 2023-04-23 20:55:02.000000 RFTLib-0.2.0/src/RFTLib/Core/Types.py
+drwxrwxrwx   0        0        0        0 2023-04-24 03:11:13.907050 RFTLib-0.2.0/src/RFTLib/Graph/
+drwxrwxrwx   0        0        0        0 2023-04-24 03:11:13.918059 RFTLib-0.2.0/src/RFTLib/Graph/Window/
+-rw-rw-rw-   0        0        0      386 2023-04-23 14:46:37.000000 RFTLib-0.2.0/src/RFTLib/Graph/Window/KeyEvent.py
+-rw-rw-rw-   0        0        0      783 2023-04-23 14:46:52.000000 RFTLib-0.2.0/src/RFTLib/Graph/Window/MouseEvent.py
+-rw-rw-rw-   0        0        0     4045 2023-04-23 23:19:05.000000 RFTLib-0.2.0/src/RFTLib/Graph/Window/__init__.py
+-rw-rw-rw-   0        0        0      123 2023-04-23 23:19:53.000000 RFTLib-0.2.0/src/RFTLib/Graph/Window/closeEvent.py
+-rw-rw-rw-   0        0        0     2445 2023-04-23 23:17:24.000000 RFTLib-0.2.0/src/RFTLib/Graph/Window/paintEvent.py
+-rw-rw-rw-   0        0        0     2572 2023-04-23 21:52:20.000000 RFTLib-0.2.0/src/RFTLib/Graph/__init__.py
+-rw-rw-rw-   0        0        0      698 2023-04-23 17:01:38.000000 RFTLib-0.2.0/src/RFTLib/Graph/circle.py
+-rw-rw-rw-   0        0        0     1059 2023-04-23 17:01:53.000000 RFTLib-0.2.0/src/RFTLib/Graph/ellipse.py
+-rw-rw-rw-   0        0        0      409 2023-04-23 21:12:29.000000 RFTLib-0.2.0/src/RFTLib/Graph/geometry.py
+-rw-rw-rw-   0        0        0      767 2023-04-23 17:02:03.000000 RFTLib-0.2.0/src/RFTLib/Graph/line.py
+-rw-rw-rw-   0        0        0      364 2023-04-23 16:03:38.000000 RFTLib-0.2.0/src/RFTLib/Graph/nan.py
+-rw-rw-rw-   0        0        0      640 2023-04-23 17:02:10.000000 RFTLib-0.2.0/src/RFTLib/Graph/point.py
+-rw-rw-rw-   0        0        0      782 2023-04-23 17:02:18.000000 RFTLib-0.2.0/src/RFTLib/Graph/rectangle.py
+-rw-rw-rw-   0        0        0      478 2023-04-23 17:02:32.000000 RFTLib-0.2.0/src/RFTLib/Graph/velocity.py
+-rw-rw-rw-   0        0        0      266 2023-04-23 16:57:22.000000 RFTLib-0.2.0/src/RFTLib/Require.py
+drwxrwxrwx   0        0        0        0 2023-04-24 03:11:13.920050 RFTLib-0.2.0/src/RFTLib/Saves/
+-rw-rw-rw-   0        0        0     2008 2023-04-23 12:30:37.000000 RFTLib-0.2.0/src/RFTLib/Saves/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 03:11:13.726049 RFTLib-0.2.0/src/RFTLib.egg-info/
+-rw-rw-rw-   0        0        0      327 2023-04-24 03:11:13.000000 RFTLib-0.2.0/src/RFTLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1136 2023-04-24 03:11:13.000000 RFTLib-0.2.0/src/RFTLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 03:11:13.000000 RFTLib-0.2.0/src/RFTLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-24 03:11:13.000000 RFTLib-0.2.0/src/RFTLib.egg-info/top_level.txt
```

### Comparing `RFTLib-0.1.1/LICENSE` & `RFTLib-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `RFTLib-0.1.1/src/RFTLib/Config/__init__.py` & `RFTLib-0.2.0/src/RFTLib/Config/__init__.py`

 * *Files identical despite different names*

### Comparing `RFTLib-0.1.1/src/RFTLib/Config/cv2.py` & `RFTLib-0.2.0/src/RFTLib/Config/cv2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from ..Require import *
 
 import cv2
 
 from .loader import *
+
 from ..Core.Types import *
 
 
 
 
 
 __all__ = ("RFT_Config_CV2_IMAGE", "RFT_Config_CV2_VIDEO")
```

### Comparing `RFTLib-0.1.1/src/RFTLib/Config/json.py` & `RFTLib-0.2.0/src/RFTLib/Config/json.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from ..Require import *
 
 import json
 
 from .loader import *
+
 from ..Core.Types import *
 from ..Core.Structure import *
```

### Comparing `RFTLib-0.1.1/src/RFTLib/Config/pillow.py` & `RFTLib-0.2.0/src/RFTLib/Config/pillow.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from ..Require import *
 
 from PIL import Image
 
 from .loader import *
+
 from ..Core.Types import *
 from ..Core.Structure import *
```

### Comparing `RFTLib-0.1.1/src/RFTLib/Config/python.py` & `RFTLib-0.2.0/src/RFTLib/Config/python.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from ..Require import *
 
 import importlib
 
 from .loader import *
+
 from ..Core.Types import *
 from ..Core.Structure import *
```

### Comparing `RFTLib-0.1.1/src/RFTLib/Config/qt.py` & `RFTLib-0.2.0/src/RFTLib/Config/qt.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from ..Require import *
 
 from PyQt6.QtGui import QPixmap, QIcon, QImage
 
 from .loader import *
+
 from ..Core.Types import *
 from ..Core.Structure import *
```

### Comparing `RFTLib-0.1.1/src/RFTLib/Config/rypple.py` & `RFTLib-0.2.0/src/RFTLib/Config/rypple.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from ..Require import *
 
 import Rypple
 from Rypple.namespace import *
 
 from .loader import *
+
 from ..Core.Types import *
 from ..Core.Structure import *
```

### Comparing `RFTLib-0.1.1/src/RFTLib/Config/toml.py` & `RFTLib-0.2.0/src/RFTLib/Config/toml.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from ..Require import *
 
-import toml
+import tomllib
 
 from .loader import *
+
 from ..Core.Types import *
 from ..Core.Structure import *
 
 
 
 
 
@@ -25,15 +26,15 @@
 		# Convert to pathlib
 		path = Path(path)
 		path = path.resolve()
 		
 
 		# Read file
 		with path.open("r") as file:
-			dataT = toml.load(file)
+			dataT = tomllib.load(file)
 			
 			data = RFT_Structure(dataT)
 
 
 		# Return data
 		return data
```

### Comparing `RFTLib-0.1.1/src/RFTLib/Config/yaml.py` & `RFTLib-0.2.0/src/RFTLib/Config/yaml.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from ..Require import *
 
 import yaml
 
 from .loader import *
+
 from ..Core.Types import *
 from ..Core.Structure import *
```

### Comparing `RFTLib-0.1.1/src/RFTLib/Core/Object.py` & `RFTLib-0.2.0/src/RFTLib/Core/Object.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
 					# Get function return type
 					ret = sig.return_annotation
 
 
 
 					# Return type is void
-					if (ret in (inspect._empty, types.NoneType, typing.NoReturn)):
+					if (ret in (inspect._empty, types.NoneType, typing.NoReturn, None)):
 						retName = "void"
 
 					else:
 						# Get return type name
 						retName = ret.__name__
```

### Comparing `RFTLib-0.1.1/src/RFTLib/Core/Structure.py` & `RFTLib-0.2.0/src/RFTLib/Core/Buffer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,234 +1,176 @@
 from ..Require import *
 
-from .Object import *
 from .Types import *
+from .Object import *
+from .Structure import *
 
 
 
 
 
-__all__ = ("RFT_Structure",)
-
-
-
-
-
-class RFT_Structure(RFT_Object):
-	def __init__(self, struct:RFT_Typing.Dictionary):
-		if (isinstance(struct,RFT_Structure)):
-			struct = struct.data()
-
-
-		if (isinstance(struct,dict)):
-			data = dict(struct)
-			
-
-			for k in struct.keys():
-				v = struct[k]
-
-				if (isinstance(v,dict)):
-					v = RFT_Structure(v)
-					struct[k] = v
-
-
-			object.__setattr__(self,"__data__",struct)
-
-		else:
-			raise TypeError
-
-
-
+__all__ = ("RFT_Buffer",)
 
 
-	# ~~~~~~~~ Attr Assignment ~~~~~~~
-	def __getattr__(self, attr:str):
-		v = self.data()
 
-		return v[attr]
 
 
+class RFT_Buffer(RFT_Object):
+	def __init__(self, data:int | str | RFT_Typing.Buffer | tuple | list = None) -> None:
+		self.data = self.toBytes(data)
 
-	def __setattr__(self, attr:str, val:RFT_Typing.Any):
-		v = self.data()
-		
-		v[attr] = val
-	# ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 
 
-	# ~~~~~~~~ Item Assignment ~~~~~~~
-	def __getitem__(self, path:RFT_Typing.Array | str):
-		# If path is string then split into array
-		if (isinstance(path,str)):
-			path = path.split(".")
+	# ~~~~~~~~~ Magic Methods ~~~~~~~~
+	def __add__(self, val:int | str | RFT_Typing.Buffer | tuple | list) -> None:
+		self.data += self.toBytes(val)
 
+		return self
 
-		if (len(path) > 1):
-			# Get final attribute
-			attr = path[-1]
+	def __sub__(self, num:int) -> None:
+		for i in range(num):
+			self.pop(-1)
 
-			# Get parent
-			parent = self.parent(path)
+		return self
 
-			# If parent found
-			if (parent != None):
-				return RFT_Structure.__getattr__(parent,attr)
+	def __mul__(self, num:int) -> None:
+		self.data = self.data * num
 
+		return self
 
-		else:
-			attr = ".".join(path)
-			return self.__getattr__(attr)
 
 
+	def __len__(self) -> int:
+		return len(self.data)
 
-	def __setitem__(self, path:RFT_Typing.Array | str, value:RFT_Typing.Any):
-		# If path is string then split into array
-		if (isinstance(path,str)):
-			path = path.split(".")
 
 
-		if (len(path) > 1):
-			# Get final attribute
-			attr = path[-1]
+	def __iter__(self) -> iter:
+		return self.iter()
 
-			# Get parent
-			parent = self.parent(path)
 
-			# If parent found
-			if (parent != None):
-				return RFT_Structure.__setattr__(parent,attr,value)
 
+	def __getitem__(self, i:int) -> int:
+		return self.data[i]
 
-		else:
-			attr = ".".join(path)
-			self.__setattr__(attr,value)
+	def __setitem__(self, i:int, v:int | str) -> None:
+		self.data[i] = v
 	# ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 
 
-
-
-	def data(self):
-		d = self.__dict__
-		v = d["__data__"]
-
-		return v
+	# ~~~~~~~~~~~~ Methods ~~~~~~~~~~~
+	@classmethod
+	def toBytes(self, val:int | str | RFT_Typing.Buffer | RFT_Typing.Array | RFT_Typing.Dictionary) -> bytearray:
+		out = bytearray()
 
 
 
+		if (isinstance(val, RFT_Buffer)):
+			out = val.data
 
-	def toDict(self):
-		out = {}
 
-		for k,v in self.data().items():
-			if (isinstance(v, RFT_Structure)):
-				out[k] = v.toDict()
-			else:
-				out[k] = v
 
-		return out
+		elif (isinstance(val, int)):
+			size = (val.bit_length() + 7) // 8
+			
+			out = bytearray(size)
+			
+			for i in range(size):
+				out[size - i - 1] = (val >> (8 * i)) & 0xff
 
 
 
+		elif (isinstance(val, RFT_Types.Buffer)):
+			out = bytearray(val)
 
 
 
-	def keys(self):
-		d = self.data()
+		elif (isinstance(val, str)):
+			out = bytearray(val.encode("utf-8"))
 
-		return d.keys()
 
 
+		elif (isinstance(val, (tuple, list))):
+			for v in val:
+				out += self.toBytes(v)
 
-	def items(self):
-		d = self.data()
 
-		return d.items()
 
+		elif (isinstance(val, (dict, map, RFT_Structure))):
+			if (isinstance(val, RFT_Structure)):
+				val = val.toDict()
 
+			elif (isinstance(val, map)):
+				val = dict(val)
 
+			s = json.dumps(val)
+			out = s.encode("utf-8")
 
 
-	def contains(self, attr:str):
-		d = self.data()
 
-		return attr in d.keys()
+		elif (val is None):
+			...
 
 
 
+		return out
 
 
-	def pop(self, attr:str):
-		d = self.data()
 
-		return d.pop(attr)
 
 
+	# Manipulation methods
+	def iter(self) -> iter:
+		return iter(self.data)
 
 
+	def riter(self) -> iter:
+		return reversed(self.data)	
 
-	# Gets parent structure of given path
-	def parent(self, path:RFT_Typing.Array | str):
-		# If path is string then split into array
-		if (isinstance(path,str)):
-			path = path.split(".")
 
+	def pop(self,i:int) -> int:
+		return self.data.pop(i)
 
-		# Default parent
-		parent = None
 
 
-		if (len(path) > 0):
-			# Set parent
-			parent = self
-			
-			for i,a in enumerate(path[:-1]):
-				# Get value in namespace
-				val = parent[a]
 
-				if (isinstance(val,RFT_Structure)):
-					# Set new parent
-					parent = val
 
-				else:
-					# Doesn't exist or invalid value
-					parent = None
-					break
+	# Output methods
+	def hex(self) -> str:
+		return self.data.hex()
 
 
-		return parent
+	def int(self) -> int:
+		out = 0
 
+		for i,c in enumerate(self.riter()):
+			out += c << (i * 8)
 
+		return out
 
 
+	def str(self) -> str:
+		return self.data.decode("utf-8")
 
-	def allocate(self, path:RFT_Typing.Array | str):
-		# If path is string then split into array
-		if (isinstance(path,str)):
-			path = path.split(".")
 
 
-		parent = self
 
-		for p in path:
-			if (parent.contains(p)):
-				v = parent[p]
 
-				if (isinstance(v,RFT_Structure)):
-					parent = v
+	# Compression methods
+	def compress(self):
+		data = zlib.compress(self.data)
 
-				else:
-					return None
+		return RFT_Buffer(data)
 
-			else:
-				v = RFT_Structure({})
 
-				parent[p] = v
-				parent = v
+	def decompress(self):
+		data = zlib.decompress(self.data)
 
+		return RFT_Buffer(data)
+	# ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-		return parent
```


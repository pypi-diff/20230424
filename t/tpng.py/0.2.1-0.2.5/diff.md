# Comparing `tmp/tpng.py-0.2.1-py3-none-any.whl.zip` & `tmp/tpng.py-0.2.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,10 @@
-Zip file size: 4041 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat      253 b- defN 22-Nov-23 21:18 tpng/Types.py
--rw-rw-rw-  2.0 fat       45 b- defN 22-Nov-23 21:10 tpng/__init__.py
--rw-rw-rw-  2.0 fat      290 b- defN 22-Nov-23 21:30 tpng/__main__.py
--rw-rw-rw-  2.0 fat     2092 b- defN 22-Nov-23 21:29 tpng/tpng.py
--rw-rw-rw-  2.0 fat     1085 b- defN 22-Nov-23 21:31 tpng.py-0.2.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1184 b- defN 22-Nov-23 21:31 tpng.py-0.2.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Nov-23 21:31 tpng.py-0.2.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 22-Nov-23 21:31 tpng.py-0.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      666 b- defN 22-Nov-23 21:31 tpng.py-0.2.1.dist-info/RECORD
-9 files, 5712 bytes uncompressed, 2903 bytes compressed:  49.2%
+Zip file size: 3772 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat       24 b- defN 23-Apr-24 14:10 tpng/__init__.py
+-rw-rw-rw-  2.0 fat      346 b- defN 23-Apr-24 15:29 tpng/__main__.py
+-rw-rw-rw-  2.0 fat     2084 b- defN 23-Apr-24 16:48 tpng/tpng.py
+-rw-rw-rw-  2.0 fat     1085 b- defN 23-Apr-24 16:48 tpng.py-0.2.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1184 b- defN 23-Apr-24 16:48 tpng.py-0.2.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-24 16:48 tpng.py-0.2.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Apr-24 16:48 tpng.py-0.2.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      597 b- defN 23-Apr-24 16:48 tpng.py-0.2.5.dist-info/RECORD
+8 files, 5417 bytes uncompressed, 2736 bytes compressed:  49.5%
```

## zipnote {}

```diff
@@ -1,28 +1,25 @@
-Filename: tpng/Types.py
-Comment: 
-
 Filename: tpng/__init__.py
 Comment: 
 
 Filename: tpng/__main__.py
 Comment: 
 
 Filename: tpng/tpng.py
 Comment: 
 
-Filename: tpng.py-0.2.1.dist-info/LICENSE
+Filename: tpng.py-0.2.5.dist-info/LICENSE
 Comment: 
 
-Filename: tpng.py-0.2.1.dist-info/METADATA
+Filename: tpng.py-0.2.5.dist-info/METADATA
 Comment: 
 
-Filename: tpng.py-0.2.1.dist-info/WHEEL
+Filename: tpng.py-0.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: tpng.py-0.2.1.dist-info/top_level.txt
+Filename: tpng.py-0.2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: tpng.py-0.2.1.dist-info/RECORD
+Filename: tpng.py-0.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tpng/__init__.py

```diff
@@ -1,3 +1 @@
-from .tpng import (
-    TPNG, ImageInfo
-)
+from .tpng import TPNG
```

## tpng/__main__.py

```diff
@@ -1,12 +1,12 @@
 import tpng
 from rich.console import Console
 
 c = Console()
 
 try:
-    t = tpng.TPNG("D:\\Downloads\\Minecraft_missing_texture_block.svg.png")
+    t = tpng.TPNG("D:\Pictures\Rebecca\g-oIJG0T-b8Fsxm8BUef_Jnxh13Hymp8Gm7GWGrA7y7q2hrejcHOvrtFipRL50qVfxtbomMzb8874YAeVu-b-bCG.jpg")
     t.resize( (50, 25) )
-    text = t.get_rich_string()
+    text = t.to_rich_image()
     c.print(text)
 except:
     c.print_exception(show_locals=True, word_wrap=True)
```

## tpng/tpng.py

```diff
@@ -1,10 +1,9 @@
 from io import BufferedReader, BytesIO
 from PIL import Image
-from .Types import ImageInfo as ImageInfo
 
 class TPNG:
     def __init__(
         self,
         fp,
         mode=None,
         size=None,
@@ -19,39 +18,41 @@
             self.image = Image.frombuffer(mode, size, fp, *args, **kwargs)
         elif isinstance(fp, BytesIO):
             self.image = Image.frombuffer(mode, size, fp, *args, **kwargs)
         elif isinstance(fp, Image.Image):
             self.image = fp
         else:
             raise TypeError(f"Type parameter for 'fp' cannot be a '{type(fp)}'")
-        self.image = self.image.convert("RGBA")
+        
+        if self.image.mode != "RGB": self.image = self.image.convert("RGB")
+        self.use_image = self.image.copy()
     
-    def resize(self, new_size) -> None:
-        if self.image.size != new_size:
-            self.image = self.image.resize(new_size)
+    @staticmethod
+    def to_hex(pixel) -> str: return "#"+"".join(hex(i)[2:].rjust(2,"0") for i in pixel)
     
-    def get_info(self):
-        return ImageInfo(self.image.fp.name if hasattr(self, "fp") else None, self.image.size, self.image.info.get("dpi", (-1, -1)), self.image.mode)
+    @property
+    def size(self): return self.use_image.size
     
-    @staticmethod
-    def to_hex(pixel) -> str: return "#"+"".join([hex(i)[2:] for i in pixel])
+    def resize(self, size: tuple) -> None: self.use_image = self.use_image.resize(size)
+    def convert(self, mode: str) -> None: self.use_image = self.use_image.convert(mode)
+    def reset(self) -> None: self.use_image = self.image.copy()
     
-    def get_rich_string(
+    def to_rich_image(
         self,
-        pixel="█",
-        error_pixel="?",
-        alpha_pixel=" ",
-        alpha_colours=None
+        pixel: str="█",
+        error_pixel: str="?",
+        alpha_pixel: str=" ",
+        alpha_colors: list=[]
     ) -> str:
-        string, img, alpha_colours = "", self.image.convert("RGB"), alpha_colours or []
-        alpha_colours = [tuple(i) for i in alpha_colours]
+        timg = ""
+        img = self.use_image if self.use_image.mode == "RGB" else self.use_image.convert("RGB")
+        
         for y in range(img.size[1]):
             for x in range(img.size[0]):
                 try:
-                    if (p:=img.getpixel( (x, y) )) not in alpha_colours:
-                        string += f"[{self.to_hex(p)}]{pixel}[/]"
-                    else:
-                        string += alpha_pixel
-                except:
-                    string += error_pixel
-            string += "\n"
-        return string
+                    pix = img.getpixel((x, y))
+                    if pix not in alpha_colors: timg += f"[{self.to_hex(pix)}]{pixel}[/]"
+                    else: timg += alpha_pixel
+                except: timg += error_pixel
+            timg += "\n"
+        
+        return timg
```

## Comparing `tpng.py-0.2.1.dist-info/LICENSE` & `tpng.py-0.2.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tpng.py-0.2.1.dist-info/METADATA` & `tpng.py-0.2.5.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tpng.py
-Version: 0.2.1
+Version: 0.2.5
 Summary: A special file format for displaying images in the terminal.
 Home-page: https://github.com/romanin-rf/tpng.py
 Author: programmer-from-parlament
 Author-email: semina054@gmail.com
 License: MIT
 Keywords: tpng.py
 Platform: UNKNOWN
```

## Comparing `tpng.py-0.2.1.dist-info/RECORD` & `tpng.py-0.2.5.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-tpng/Types.py,sha256=Xzbp__z1zVwXZxgpg5YszCuoYjxJbcvTQYE--ptgw6s,253
-tpng/__init__.py,sha256=fNjERAHIW2vF340Ge1MqAug1plggC9L-savyMzTcUaE,45
-tpng/__main__.py,sha256=5aKnB3eNdgX5ivptY6zJFhK0p0zEqT9DQKFSk1AgINQ,290
-tpng/tpng.py,sha256=I8pS8gzV0Wqipihrmf6zwBivWmppQ9PCPRac4mvVDx0,2092
-tpng.py-0.2.1.dist-info/LICENSE,sha256=spNP9-xRNk_f344KMfxONAblI58MMrpPasaQ5sXdwe4,1085
-tpng.py-0.2.1.dist-info/METADATA,sha256=0pCBFsgkiKgdOTmaYHlDF2fdDjC59R1aD797w1whxmo,1184
-tpng.py-0.2.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-tpng.py-0.2.1.dist-info/top_level.txt,sha256=6LrTePJd7WFpKFiPYtM5d3tzIcKSf-LbRTR93YGOQyA,5
-tpng.py-0.2.1.dist-info/RECORD,,
+tpng/__init__.py,sha256=OMwgVLk0RHzjFMZDEP5It71HZQZSboKE7wOYpC7x_wc,24
+tpng/__main__.py,sha256=oHyNUzWlWh6WepVWW2tobN0vO5Tqv5Kws8N8UcYrlIY,346
+tpng/tpng.py,sha256=WQPB_Uwx4BU5auntSvL_H7vUx6S8ZCJFkLMqLLDmhtY,2084
+tpng.py-0.2.5.dist-info/LICENSE,sha256=spNP9-xRNk_f344KMfxONAblI58MMrpPasaQ5sXdwe4,1085
+tpng.py-0.2.5.dist-info/METADATA,sha256=Ta2mwDQ1A06wSj6kXmmurJsx59SmZfvc40DEi3nsNVE,1184
+tpng.py-0.2.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+tpng.py-0.2.5.dist-info/top_level.txt,sha256=6LrTePJd7WFpKFiPYtM5d3tzIcKSf-LbRTR93YGOQyA,5
+tpng.py-0.2.5.dist-info/RECORD,,
```


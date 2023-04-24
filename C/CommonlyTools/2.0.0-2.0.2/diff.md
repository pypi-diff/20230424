# Comparing `tmp/CommonlyTools-2.0.0.tar.gz` & `tmp/CommonlyTools-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CommonlyTools-2.0.0.tar", last modified: Sun Apr 23 06:41:52 2023, max compression
+gzip compressed data, was "CommonlyTools-2.0.2.tar", last modified: Mon Apr 24 13:51:47 2023, max compression
```

## Comparing `CommonlyTools-2.0.0.tar` & `CommonlyTools-2.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 06:41:52.390236 CommonlyTools-2.0.0/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 06:41:52.390236 CommonlyTools-2.0.0/CommonlyTools.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1650 2023-04-23 06:41:52.000000 CommonlyTools-2.0.0/CommonlyTools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      278 2023-04-23 06:41:52.000000 CommonlyTools-2.0.0/CommonlyTools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-23 06:41:52.000000 CommonlyTools-2.0.0/CommonlyTools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       18 2023-04-23 06:41:52.000000 CommonlyTools-2.0.0/CommonlyTools.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       14 2023-04-23 06:41:52.000000 CommonlyTools-2.0.0/CommonlyTools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     1062 2023-04-23 04:55:31.000000 CommonlyTools-2.0.0/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     1650 2023-04-23 06:41:52.390236 CommonlyTools-2.0.0/PKG-INFO
--rw-------   0 runner    (1000) runner    (1000)      910 2023-04-23 06:38:57.000000 CommonlyTools-2.0.0/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-23 06:41:52.390236 CommonlyTools-2.0.0/commonlytools/
--rw-------   0 runner    (1000) runner    (1000)       24 2023-04-23 04:55:26.000000 CommonlyTools-2.0.0/commonlytools/__init__.py
--rw-------   0 runner    (1000) runner    (1000)     2313 2023-04-23 04:55:26.000000 CommonlyTools-2.0.0/commonlytools/discohook.py
--rw-r--r--   0 runner    (1000) runner    (1000)      312 2023-04-23 02:53:39.000000 CommonlyTools-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-23 06:41:52.394236 CommonlyTools-2.0.0/setup.cfg
--rw-------   0 runner    (1000) runner    (1000)      740 2023-04-23 06:40:28.000000 CommonlyTools-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-24 13:51:47.120672 CommonlyTools-2.0.2/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-24 13:51:47.112672 CommonlyTools-2.0.2/CommonlyTools.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1651 2023-04-24 13:51:46.000000 CommonlyTools-2.0.2/CommonlyTools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      278 2023-04-24 13:51:47.000000 CommonlyTools-2.0.2/CommonlyTools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-24 13:51:46.000000 CommonlyTools-2.0.2/CommonlyTools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       18 2023-04-24 13:51:46.000000 CommonlyTools-2.0.2/CommonlyTools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       14 2023-04-24 13:51:46.000000 CommonlyTools-2.0.2/CommonlyTools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     1062 2023-04-23 04:55:31.000000 CommonlyTools-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     1651 2023-04-24 13:51:47.120672 CommonlyTools-2.0.2/PKG-INFO
+-rw-------   0 runner    (1000) runner    (1000)      911 2023-04-24 12:32:29.000000 CommonlyTools-2.0.2/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-24 13:51:47.112672 CommonlyTools-2.0.2/commonlytools/
+-rw-------   0 runner    (1000) runner    (1000)       24 2023-04-23 04:55:26.000000 CommonlyTools-2.0.2/commonlytools/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)     2704 2023-04-24 12:32:54.000000 CommonlyTools-2.0.2/commonlytools/discohook.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      312 2023-04-23 02:53:39.000000 CommonlyTools-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-24 13:51:47.120672 CommonlyTools-2.0.2/setup.cfg
+-rw-------   0 runner    (1000) runner    (1000)      740 2023-04-24 13:51:30.000000 CommonlyTools-2.0.2/setup.py
```

### Comparing `CommonlyTools-2.0.0/CommonlyTools.egg-info/PKG-INFO` & `CommonlyTools-2.0.2/CommonlyTools.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CommonlyTools
-Version: 2.0.0
+Version: 2.0.2
 Summary: You will use Python easily!
 Home-page: https://github.com/maxgamil110331/CommonlyTools
 Author: MaxPython110331
 Author-email: dengxiangcheng110331@gmail.com
 License: MIT
 Description: # CommonlyTools
         
@@ -16,15 +16,15 @@
         
         >commonlytools/discohook.py
         >>Discord Webhook Sender
         >>>Step 1(If you do not need to use embed, you can skip this step.)
         >>>```py
         >>>from commonlytools import discohook
         >>>
-        >>>embed=discohook.Embed(color=dc.Colour(...), title="...", description="...") #If you need, you can enter the colour, title or descriotion
+        >>>embed=discohook.Embed(color=..., colour=..., title="...", description="...") #If you need, you can enter the colour, title or descriotion
         >>>embed.author(name="...", url="...", icon_url="...") #author
         >>>embed.footer(text="...", icon_url="...") #footer
         >>>embed.image(image_url="...") #image
         >>>embed.thumbnail(thumbnail_url="...") #thumbnail
         >>>embed.add_field(name="...", value="...", inline=...) #add_field #This function can unlimited superposition.
         >>>```
         >>
```

### Comparing `CommonlyTools-2.0.0/LICENSE` & `CommonlyTools-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `CommonlyTools-2.0.0/PKG-INFO` & `CommonlyTools-2.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CommonlyTools
-Version: 2.0.0
+Version: 2.0.2
 Summary: You will use Python easily!
 Home-page: https://github.com/maxgamil110331/CommonlyTools
 Author: MaxPython110331
 Author-email: dengxiangcheng110331@gmail.com
 License: MIT
 Description: # CommonlyTools
         
@@ -16,15 +16,15 @@
         
         >commonlytools/discohook.py
         >>Discord Webhook Sender
         >>>Step 1(If you do not need to use embed, you can skip this step.)
         >>>```py
         >>>from commonlytools import discohook
         >>>
-        >>>embed=discohook.Embed(color=dc.Colour(...), title="...", description="...") #If you need, you can enter the colour, title or descriotion
+        >>>embed=discohook.Embed(color=..., colour=..., title="...", description="...") #If you need, you can enter the colour, title or descriotion
         >>>embed.author(name="...", url="...", icon_url="...") #author
         >>>embed.footer(text="...", icon_url="...") #footer
         >>>embed.image(image_url="...") #image
         >>>embed.thumbnail(thumbnail_url="...") #thumbnail
         >>>embed.add_field(name="...", value="...", inline=...) #add_field #This function can unlimited superposition.
         >>>```
         >>
```

### Comparing `CommonlyTools-2.0.0/README.md` & `CommonlyTools-2.0.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 >commonlytools/discohook.py
 >>Discord Webhook Sender
 >>>Step 1(If you do not need to use embed, you can skip this step.)
 >>>```py
 >>>from commonlytools import discohook
 >>>
->>>embed=discohook.Embed(color=dc.Colour(...), title="...", description="...") #If you need, you can enter the colour, title or descriotion
+>>>embed=discohook.Embed(color=..., colour=..., title="...", description="...") #If you need, you can enter the colour, title or descriotion
 >>>embed.author(name="...", url="...", icon_url="...") #author
 >>>embed.footer(text="...", icon_url="...") #footer
 >>>embed.image(image_url="...") #image
 >>>embed.thumbnail(thumbnail_url="...") #thumbnail
 >>>embed.add_field(name="...", value="...", inline=...) #add_field #This function can unlimited superposition.
 >>>```
 >>
```

### Comparing `CommonlyTools-2.0.0/commonlytools/discohook.py` & `CommonlyTools-2.0.2/commonlytools/discohook.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 import requests
 import datetime
 
 
-def Colour(colour:int=0):
-    colour=int(str(colour), 10)
-    return colour
-
-
 def Timestamp(timestamp:datetime.datetime):
     return f"{timestamp.year}-{timestamp.month}-{timestamp.day}T{timestamp.hour}:{timestamp.minute}:{timestamp.second}.{timestamp.microsecond}Z"
 
 
 class Embed:
-    def __init__(self, title:str=None, description:str=None, timestamp:Timestamp=None, color:Colour=None):
+    def __init__(self, title:str=None, description:str=None, timestamp:Timestamp=None, color:int=0xffffff, colour:int=0xffffff):
         self._title=title
         self._description=description
-        self._colour=color
+        self._colour=int(str(color), 10) or int(str(colour), 10)
         self._timestamp=timestamp
         self._image={}
         self._author={}
         self._footer={}
         self._thumbnail={}
         self._field=[]
         
@@ -40,35 +35,65 @@
         self._thumbnail={"url": thumbnail_url}
 
 
     def add_field(self, name:str=None, value:str=None, inline:bool=False):
         self._field.append({"name": name, "value": value, "inline": inline})
 
 
-    def to_dict(self):
-        result={}
-        if self._title != None:
-            result["title"]=self._title
-        if self._description != None:
-            result["description"]=self._description
-        result["color"]=self._colour
-        if self._field != {}:
-            result["fields"]=self._field
-        if self._author != {}:
-            result["author"]=self._author
-        if self._footer != {}:
-            result["footer"]=self._footer
-        if self._timestamp:
-            result["timestamp"]=self._timestamp
-        if self._image != {}:
-            result["image"]=self._image
-        if self._thumbnail != {}:
-            result["thumbnail"]=self._thumbnail
-        return result
+    def title(self):
+        return self._title
+
+    
+    def description(self):
+        return self._description
+
+    def colour(self):
+        return self._colour
+
+
+    def timestamp(self):
+        return self._timestamp
+
+
+    def image(self):
+        return self._image
+
+
+    def author(self):
+        return self._author
+        
+
+    def footer(self):
+        return self._footer
+
+
+    def thumbnail(self):
+        return self._thumbnail
+
+
+    def field(self):
+        return self._field
 
 
 def send(webhook_url:str, username:str=None, avatar_url:str=None, content:str=None, embeds:list=[]):
     embeds_dict=[]
     for embed in embeds:
-        embed_dict=embed.to_dict()
-        embeds_dict.append(embed_dict)
+        result={}
+        if embed.title != None:
+            result["title"]=embed.title
+        if embed.description != None:
+            result["description"]=embed.description
+        result["color"]=embed.colour
+        if embed.field != {}:
+            result["fields"]=embed.field
+        if embed.author != {}:
+            result["author"]=embed.author
+        if embed.footer != {}:
+            result["footer"]=embed.footer
+        if embed.timestamp:
+            result["timestamp"]=embed.timestamp
+        if embed.image != {}:
+            result["image"]=embed.image
+        if embed.thumbnail != {}:
+            result["thumbnail"]=embed.thumbnail
+        embeds_dict.append(result)
     requests.post(url=webhook_url, json={"username": username, "avatar_url": avatar_url, "content": content, "embeds": embeds_dict})
```

### Comparing `CommonlyTools-2.0.0/setup.py` & `CommonlyTools-2.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="CommonlyTools",
-    version="2.0.0",
+    version="2.0.2",
     author="MaxPython110331",
     author_email="dengxiangcheng110331@gmail.com",
     description="You will use Python easily!",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/maxgamil110331/CommonlyTools",
```


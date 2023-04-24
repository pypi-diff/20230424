# Comparing `tmp/Video_Audio_Image_Downloader-0.0.7.tar.gz` & `tmp/Video_Audio_Image_Downloader-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Video_Audio_Image_Downloader-0.0.7.tar", last modified: Tue Apr 18 14:51:59 2023, max compression
+gzip compressed data, was "Video_Audio_Image_Downloader-0.0.9.tar", last modified: Mon Apr 24 06:33:50 2023, max compression
```

## Comparing `Video_Audio_Image_Downloader-0.0.7.tar` & `Video_Audio_Image_Downloader-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-18 14:51:59.031646 Video_Audio_Image_Downloader-0.0.7/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      627 2023-04-18 14:51:59.031646 Video_Audio_Image_Downloader-0.0.7/PKG-INFO
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      232 2023-04-18 14:44:02.000000 Video_Audio_Image_Downloader-0.0.7/README.md
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-18 14:51:59.027646 Video_Audio_Image_Downloader-0.0.7/Video_Audio_Image_Downloader.egg-info/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      627 2023-04-18 14:51:58.000000 Video_Audio_Image_Downloader-0.0.7/Video_Audio_Image_Downloader.egg-info/PKG-INFO
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      413 2023-04-18 14:51:58.000000 Video_Audio_Image_Downloader-0.0.7/Video_Audio_Image_Downloader.egg-info/SOURCES.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        1 2023-04-18 14:51:58.000000 Video_Audio_Image_Downloader-0.0.7/Video_Audio_Image_Downloader.egg-info/dependency_links.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       51 2023-04-18 14:51:58.000000 Video_Audio_Image_Downloader-0.0.7/Video_Audio_Image_Downloader.egg-info/entry_points.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        7 2023-04-18 14:51:58.000000 Video_Audio_Image_Downloader-0.0.7/Video_Audio_Image_Downloader.egg-info/top_level.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       38 2023-04-18 14:51:59.031646 Video_Audio_Image_Downloader-0.0.7/setup.cfg
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      889 2023-04-18 14:50:44.000000 Video_Audio_Image_Downloader-0.0.7/setup.py
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-18 14:51:59.027646 Video_Audio_Image_Downloader-0.0.7/source/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-18 10:56:32.000000 Video_Audio_Image_Downloader-0.0.7/source/__init__.py
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-18 14:51:59.027646 Video_Audio_Image_Downloader-0.0.7/source/lib/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1284 2023-04-17 14:19:56.000000 Video_Audio_Image_Downloader-0.0.7/source/lib/Argument.py
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1901 2023-04-17 14:20:59.000000 Video_Audio_Image_Downloader-0.0.7/source/lib/Command_function.py
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       38 2023-04-17 14:19:56.000000 Video_Audio_Image_Downloader-0.0.7/source/lib/__init__.py
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     2742 2023-04-17 14:19:56.000000 Video_Audio_Image_Downloader-0.0.7/source/lib/help.py
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     4424 2023-04-18 11:03:45.000000 Video_Audio_Image_Downloader-0.0.7/source/source.py
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-24 06:33:50.772799 Video_Audio_Image_Downloader-0.0.9/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     2165 2023-04-24 06:33:50.772799 Video_Audio_Image_Downloader-0.0.9/PKG-INFO
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1770 2023-04-24 05:55:53.000000 Video_Audio_Image_Downloader-0.0.9/README.md
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-24 06:33:50.772799 Video_Audio_Image_Downloader-0.0.9/Video_Audio_Image_Downloader.egg-info/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     2165 2023-04-24 06:33:50.000000 Video_Audio_Image_Downloader-0.0.9/Video_Audio_Image_Downloader.egg-info/PKG-INFO
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      413 2023-04-24 06:33:50.000000 Video_Audio_Image_Downloader-0.0.9/Video_Audio_Image_Downloader.egg-info/SOURCES.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        1 2023-04-24 06:33:50.000000 Video_Audio_Image_Downloader-0.0.9/Video_Audio_Image_Downloader.egg-info/dependency_links.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       51 2023-04-24 06:33:50.000000 Video_Audio_Image_Downloader-0.0.9/Video_Audio_Image_Downloader.egg-info/entry_points.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        7 2023-04-24 06:33:50.000000 Video_Audio_Image_Downloader-0.0.9/Video_Audio_Image_Downloader.egg-info/top_level.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       38 2023-04-24 06:33:50.772799 Video_Audio_Image_Downloader-0.0.9/setup.cfg
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      889 2023-04-24 06:33:07.000000 Video_Audio_Image_Downloader-0.0.9/setup.py
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-24 06:33:50.772799 Video_Audio_Image_Downloader-0.0.9/source/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-18 10:56:32.000000 Video_Audio_Image_Downloader-0.0.9/source/__init__.py
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-24 06:33:50.772799 Video_Audio_Image_Downloader-0.0.9/source/lib/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1284 2023-04-17 14:19:56.000000 Video_Audio_Image_Downloader-0.0.9/source/lib/Argument.py
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     2209 2023-04-24 06:30:32.000000 Video_Audio_Image_Downloader-0.0.9/source/lib/Command_function.py
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       38 2023-04-17 14:19:56.000000 Video_Audio_Image_Downloader-0.0.9/source/lib/__init__.py
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     2748 2023-04-24 05:51:48.000000 Video_Audio_Image_Downloader-0.0.9/source/lib/help.py
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     4510 2023-04-24 06:23:30.000000 Video_Audio_Image_Downloader-0.0.9/source/source.py
```

### Comparing `Video_Audio_Image_Downloader-0.0.7/setup.py` & `Video_Audio_Image_Downloader-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 requirements = os.popen("/usr/local/bin/pipreqs main --print").read().splitlines()
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='Video_Audio_Image_Downloader',
-    version='0.0.7',
+    version='0.0.9',
     author='Sridhar',
     author_email='dcsvsridhar@gmail.com',
     #  to help download videos and audio files from Youtube
     description="In this tool is help to Download the Youtube Video,Audio and Any type of Google and other site's Images",
     packages=find_packages(),
     url='https://git.selfmade.ninja/SRIDHARDSCV/audio_video_image_downloder-1',
     install_requires=requirements,
```

### Comparing `Video_Audio_Image_Downloader-0.0.7/source/lib/Argument.py` & `Video_Audio_Image_Downloader-0.0.9/source/lib/Argument.py`

 * *Files identical despite different names*

### Comparing `Video_Audio_Image_Downloader-0.0.7/source/lib/Command_function.py` & `Video_Audio_Image_Downloader-0.0.9/source/lib/Command_function.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,40 @@
+#! /usr/bin/python
+import sys
+from pytube import YouTube
+import requests 
+import shutil
+import os
+import urllib.request
 class Command_function:
     
-    def Youtube_Download_video(url,resolution,user_path):
+    def Youtube_Download_video(self,url,resolution,user_path):
         print(f"Wait untill few seconds.. Your  Downloader is Processing..")
         yt = YouTube(url)
         stream = yt.streams.filter(res=resolution).first()
         return_value = stream.download(output_path=user_path)
         if return_value:
             return True
         else:
             return False
         
-    def Youtube_Download_video_Resolution(url):
+    def Youtube_Download_video_Resolution(self,url):
         yt = YouTube(url)
         streams = yt.streams.all()
         resolutions = []
         for stream in streams:
             if 'video/mp4' in str(stream.mime_type):
                 return_value = resolutions.append(stream.resolution)
         if resolutions is not None:
             return resolutions
         else:
             return False
     
 
-    def Youtube_Download_Audio(url,user_path,user_filename):
+    def Youtube_Download_Audio(self,url,user_path,user_filename):
         print(f"Wait untill few seconds.. Your Downloader is Processing..")
         yt = YouTube(url)
         audio = yt.streams.filter(only_audio=True).first()
         return_value = audio.download(output_path=user_path, filename=user_filename)
         if return_value:
             return True
         else:
@@ -39,15 +46,18 @@
     #     with youtube_dl.YoutubeDL(ydl_opts) as ydl:
     #         return_value = ydl.download(f"{[url]}")
     #     if return_value:
     #         return True
     #     else:
     #         return False
         
-    def Image_Download(url,path,filename):
+    def Image_Download(self,url,path,filename):
         print(f"Wait untill few seconds.. Your Downloader is Processing..")
-        return_value = urllib.request.urlretrieve(url, path + filename)
-        if return_value:
-            return True
+        response = requests.get(url)
+        if response.status_code == 200:
+            if not os.path.exists(path):
+                os.makedirs(path)
+            with open(os.path.join(path, filename), "wb") as f:
+                f.write(response.content)
+                return True
         else:
             return False
-
```

### Comparing `Video_Audio_Image_Downloader-0.0.7/source/lib/help.py` & `Video_Audio_Image_Downloader-0.0.9/source/lib/help.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         print("In this command is used to Download Youtube Video's with Specified Path with Specifed Resolution")
         print()
         print("Options  are :")
         print()
         print("positional arguments : ")
         print("   -source       Source of our Youtube Video")
         print("   -resolution   Resolution of our Youtube Video")
-        print("   -path         Where the Video's to be saved")
+        print("   -path         which path the file to be saved")
         print()
         print("Optional arguments : ")
         print("-h, --help   show this help message and exit")
         
     def Youtube_Download_Audio_help(self):
         print("Usage: <downloder> youtube audio [Options]...")
         print()
@@ -39,15 +39,15 @@
         print("In this command is used to Download Youtube Audio's with Specified Path with Specifed Resolution")
         print()
         print("Options  are :")
         print()
         print("positional arguments : ")
         print("   -source       Source of our Youtube Audio")
         print("   -filename     Name of the Audio File")
-        print("   -path         Where the Audio's to be saved")
+        print("   -path         which path the file to be saved")
         print()
         print("Optional arguments : ")
         print("   -h, --help   show this help message and exit")
 
     def Image_Download_help(self):
         print("Usage: <downloder> Image [Options]...")
         print()
@@ -55,15 +55,15 @@
         print("In this command is used to Download Image's with Specified Path with Filename")
         print()
         print("Options  are :")
         print()
         print("positional arguments : ")
         print("   -source       Source of our Image to be download")
         print("   -filename     Name of the Image File")
-        print("   -path         Where the Image's to be saved")
+        print("   -path         which path the file to be saved")
         print()
         print("Optional arguments : ")
         print()
         print("   -h, --help   show this help message and exit")
```

### Comparing `Video_Audio_Image_Downloader-0.0.7/source/source.py` & `Video_Audio_Image_Downloader-0.0.9/source/source.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 def Help():
     print("<Downloder> [Options].. ")
 
 
 
 def main():
     
-    if Argument.hasCommands(['youtube']):
+    if Argument.hasCommands(['Youtube']):
         if Argument.hasCommands(['video']): # Check the option has video or audio
             if Argument.hasOptionValue('-source'):
                 if Argument.hasOptionValue('-resolution'):
                     if Argument.hasOptionValue('-path'):
                         if Argument.hasOptionValue('-resolution'):
                             url = Argument.getoptionvalue('-source')
                             resolution = Argument.getoptionvalue('-resolution')
@@ -45,15 +45,15 @@
                 elif Argument.hasOption(['-h']) or Argument.hasOption(['--help']):
                     help.Youtube_Download_video_Resolution_help()
                     
         else:
             help.Youtube_Download_video_help()
         
                                 
-        if Argument.hasCommands(['audio']):
+        if Argument.hasCommands(['Audio']):
             if Argument.hasOptionValue('-source'):
                 if Argument.hasOptionValue('-filename'):
                     if Argument.hasOptionValue('-path'):
                         url = Argument.getoptionvalue('-source')
                         path = Argument.getoptionvalue('-path')
                         filename = Argument.getoptionvalue('-filename')
                         if Youtube_Download_Audio(url,path,filename):
@@ -63,22 +63,22 @@
                         else:
                             print("Your Audio downloading operation is failed")
             elif Argument.hasOption(['-h']) or Argument.hasOption(['--help']):
                 help.Youtube_Download_Audio_help()
             else:
                 help.Youtube_Download_Audio_help()
                     
-    if Argument.hasCommands(['Image']):
+    if Argument.hasCommands(['Image']):  #TODO: to download any type of picture formates like .png, .jpg ...
         if Argument.hasOptionValue('-source'):
             if Argument.hasOptionValue('-filename'):
                 if Argument.hasOptionValue('-path'):
                     url = Argument.getoptionvalue('-source')
                     path = Argument.getoptionvalue('-path')
                     filename = Argument.getoptionvalue('-filename')
-                    if Image_Download(url,filename,path):
+                    if Command_function.Image_Download(url,path,filename):
                         print("Your Image file is Successfully Downloaded")
                         print(f"Your Image file is saved in this Location :: {Argument.getoptionvalue('-path')}")
                         print(f"Your Image file name is :: {Argument.getoptionvalue('-filename')}")
                     else:
                         print("Your Image downloading operation is failed")
                         
         elif Argument.hasOption(['-h']) or Argument.hasOption(['--help']):
```


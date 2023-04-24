# Comparing `tmp/audio_extract-0.3.1.tar.gz` & `tmp/audio_extract-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audio_extract-0.3.1.tar", last modified: Sat Apr 22 22:25:02 2023, max compression
+gzip compressed data, was "audio_extract-0.3.2.tar", last modified: Mon Apr 24 06:55:18 2023, max compression
```

## Comparing `audio_extract-0.3.1.tar` & `audio_extract-0.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 22:25:02.133358 audio_extract-0.3.1/
--rw-rw-rw-   0        0        0     1090 2023-04-22 17:27:29.000000 audio_extract-0.3.1/LICENSE.md
--rw-rw-rw-   0        0        0     4308 2023-04-22 22:25:02.132357 audio_extract-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     3393 2023-04-22 22:01:19.000000 audio_extract-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 22:25:02.099357 audio_extract-0.3.1/audio_extract/
--rw-rw-rw-   0        0        0     1723 2023-04-22 22:19:55.000000 audio_extract-0.3.1/audio_extract/__init__.py
--rw-rw-rw-   0        0        0      142 2023-04-22 18:09:12.000000 audio_extract-0.3.1/audio_extract/exceptions.py
--rw-rw-rw-   0        0        0     1123 2023-04-22 21:31:51.000000 audio_extract-0.3.1/audio_extract/execute.py
--rw-rw-rw-   0        0        0     1798 2023-04-22 21:45:01.000000 audio_extract-0.3.1/audio_extract/ffmpeg_tools.py
--rw-rw-rw-   0        0        0     1314 2023-04-22 22:19:05.000000 audio_extract-0.3.1/audio_extract/utils.py
--rw-rw-rw-   0        0        0     2859 2023-04-22 19:49:07.000000 audio_extract-0.3.1/audio_extract/validators.py
-drwxrwxrwx   0        0        0        0 2023-04-22 22:25:02.129357 audio_extract-0.3.1/audio_extract.egg-info/
--rw-rw-rw-   0        0        0     4308 2023-04-22 22:25:01.000000 audio_extract-0.3.1/audio_extract.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2023-04-22 22:25:02.000000 audio_extract-0.3.1/audio_extract.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 22:25:01.000000 audio_extract-0.3.1/audio_extract.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-22 22:25:01.000000 audio_extract-0.3.1/audio_extract.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       86 2023-04-22 22:25:01.000000 audio_extract-0.3.1/audio_extract.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-22 22:25:01.000000 audio_extract-0.3.1/audio_extract.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 22:25:02.133358 audio_extract-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     2460 2023-04-22 22:24:32.000000 audio_extract-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:55:18.064015 audio_extract-0.3.2/
+-rw-rw-rw-   0        0        0     1090 2023-04-22 17:27:29.000000 audio_extract-0.3.2/LICENSE.md
+-rw-rw-rw-   0        0        0     4420 2023-04-24 06:55:18.063016 audio_extract-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3505 2023-04-24 06:53:56.000000 audio_extract-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 06:55:18.016018 audio_extract-0.3.2/audio_extract/
+-rw-rw-rw-   0        0        0     1723 2023-04-22 22:19:55.000000 audio_extract-0.3.2/audio_extract/__init__.py
+-rw-rw-rw-   0        0        0      142 2023-04-22 18:09:12.000000 audio_extract-0.3.2/audio_extract/exceptions.py
+-rw-rw-rw-   0        0        0     1123 2023-04-22 21:31:51.000000 audio_extract-0.3.2/audio_extract/execute.py
+-rw-rw-rw-   0        0        0     1798 2023-04-22 21:45:01.000000 audio_extract-0.3.2/audio_extract/ffmpeg_tools.py
+-rw-rw-rw-   0        0        0     1314 2023-04-22 22:19:05.000000 audio_extract-0.3.2/audio_extract/utils.py
+-rw-rw-rw-   0        0        0     2859 2023-04-22 19:49:07.000000 audio_extract-0.3.2/audio_extract/validators.py
+drwxrwxrwx   0        0        0        0 2023-04-24 06:55:18.061015 audio_extract-0.3.2/audio_extract.egg-info/
+-rw-rw-rw-   0        0        0     4420 2023-04-24 06:55:17.000000 audio_extract-0.3.2/audio_extract.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2023-04-24 06:55:17.000000 audio_extract-0.3.2/audio_extract.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 06:55:17.000000 audio_extract-0.3.2/audio_extract.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-24 06:55:17.000000 audio_extract-0.3.2/audio_extract.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       86 2023-04-24 06:55:17.000000 audio_extract-0.3.2/audio_extract.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-24 06:55:17.000000 audio_extract-0.3.2/audio_extract.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 06:55:18.064015 audio_extract-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     2460 2023-04-24 06:54:38.000000 audio_extract-0.3.2/setup.py
```

### Comparing `audio_extract-0.3.1/LICENSE.md` & `audio_extract-0.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `audio_extract-0.3.1/PKG-INFO` & `audio_extract-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audio_extract
-Version: 0.3.1
+Version: 0.3.2
 Summary: Extract and trim audio from videos or trim audios.
 Home-page: https://github.com/riad-azz/audio-extract
 Author: riad-azz
 Author-email: riadh.azzoun@hotmail.com
 License: MIT License
 Project-URL: Source, https://github.com/riad-azz/audio-extract
 Keywords: convert video,audio,ffmpeg,video to mp3
@@ -19,45 +19,45 @@
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Multimedia :: Video :: Conversion
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Audio Extract
 
-Extract and trim audio from videos or trim audios.
+audio-extract is a Python library that allows you to extract audio from video files and trim the audio according to your
+needs
 
 ## Description
 
-Audio Extract allows you to extract audio from video files and trim the audio according to your needs.
-It supports various video and audio formats and has a simple and user-friendly interface.
-
-It can also be used to trim audios.
+audio-extract is a Python library that allows you to extract audio from video files and trim the audio according to your
+needs. You can use it to create audio clips from movies, podcasts, or any other video source. It supports various audio
+and video formats, such as MP3, WAV, OGG, MP4, AVI, and MKV.
 
 ## Installing
 
 ```bash
 pip install audio-extract
 ```
 
 ## Executing the program
 
 #### Extract full audio
 
 ```python
-import audio_extract as audio_extract
+import audio_extract
 
 audio_extract.run(input_path="./video.mp4", output_path="./audio.mp3")
 ```
 
 This will create a mp3 file called `audio.mp3` that contains the full audio of the video file `video.mp4`.
 
 #### Extract sub clip audio
 
 ```python
-import audio_extract as audio_extract
+import audio_extract
 
 audio_extract.run(input_path="./video.mp4", output_path="./audio.mp3", start_time="00:30")
 ```
 
 This will create a mp3 file called `audio.mp3` that starts after the first 30 seconds of the video file `video.mp4`.
 
 #### Extract sub clip audio with custom duration
@@ -134,15 +134,14 @@
 ```bash
 audio-extract --input audio.mp3 --output new_audio.mp3 --start '00:05' --duration '01:15'
 ```
 
 This command trim the audio starting from `00:05` to `01:15` of the file `audio.mp3` to a mp3 file
 called `new_audio.mp3` that will have a duration of `01:10`.
 
-
 ## Authors
 
 Riadh Azzoun - [@riad-azz](https://github.com/riad-azz)
 
 ## License
 
 This project is licensed under the [MIT] License - see the LICENSE.md file for details
```

### Comparing `audio_extract-0.3.1/README.md` & `audio_extract-0.3.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # Audio Extract
 
-Extract and trim audio from videos or trim audios.
+audio-extract is a Python library that allows you to extract audio from video files and trim the audio according to your
+needs
 
 ## Description
 
-Audio Extract allows you to extract audio from video files and trim the audio according to your needs.
-It supports various video and audio formats and has a simple and user-friendly interface.
-
-It can also be used to trim audios.
+audio-extract is a Python library that allows you to extract audio from video files and trim the audio according to your
+needs. You can use it to create audio clips from movies, podcasts, or any other video source. It supports various audio
+and video formats, such as MP3, WAV, OGG, MP4, AVI, and MKV.
 
 ## Installing
 
 ```bash
 pip install audio-extract
 ```
 
 ## Executing the program
 
 #### Extract full audio
 
 ```python
-import audio_extract as audio_extract
+import audio_extract
 
 audio_extract.run(input_path="./video.mp4", output_path="./audio.mp3")
 ```
 
 This will create a mp3 file called `audio.mp3` that contains the full audio of the video file `video.mp4`.
 
 #### Extract sub clip audio
 
 ```python
-import audio_extract as audio_extract
+import audio_extract
 
 audio_extract.run(input_path="./video.mp4", output_path="./audio.mp3", start_time="00:30")
 ```
 
 This will create a mp3 file called `audio.mp3` that starts after the first 30 seconds of the video file `video.mp4`.
 
 #### Extract sub clip audio with custom duration
@@ -111,15 +111,14 @@
 ```bash
 audio-extract --input audio.mp3 --output new_audio.mp3 --start '00:05' --duration '01:15'
 ```
 
 This command trim the audio starting from `00:05` to `01:15` of the file `audio.mp3` to a mp3 file
 called `new_audio.mp3` that will have a duration of `01:10`.
 
-
 ## Authors
 
 Riadh Azzoun - [@riad-azz](https://github.com/riad-azz)
 
 ## License
 
 This project is licensed under the [MIT] License - see the LICENSE.md file for details
```

### Comparing `audio_extract-0.3.1/audio_extract/__init__.py` & `audio_extract-0.3.2/audio_extract/__init__.py`

 * *Files identical despite different names*

### Comparing `audio_extract-0.3.1/audio_extract/execute.py` & `audio_extract-0.3.2/audio_extract/execute.py`

 * *Files identical despite different names*

### Comparing `audio_extract-0.3.1/audio_extract/ffmpeg_tools.py` & `audio_extract-0.3.2/audio_extract/ffmpeg_tools.py`

 * *Files identical despite different names*

### Comparing `audio_extract-0.3.1/audio_extract/utils.py` & `audio_extract-0.3.2/audio_extract/utils.py`

 * *Files identical despite different names*

### Comparing `audio_extract-0.3.1/audio_extract/validators.py` & `audio_extract-0.3.2/audio_extract/validators.py`

 * *Files identical despite different names*

### Comparing `audio_extract-0.3.1/audio_extract.egg-info/PKG-INFO` & `audio_extract-0.3.2/audio_extract.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audio-extract
-Version: 0.3.1
+Version: 0.3.2
 Summary: Extract and trim audio from videos or trim audios.
 Home-page: https://github.com/riad-azz/audio-extract
 Author: riad-azz
 Author-email: riadh.azzoun@hotmail.com
 License: MIT License
 Project-URL: Source, https://github.com/riad-azz/audio-extract
 Keywords: convert video,audio,ffmpeg,video to mp3
@@ -19,45 +19,45 @@
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Multimedia :: Video :: Conversion
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Audio Extract
 
-Extract and trim audio from videos or trim audios.
+audio-extract is a Python library that allows you to extract audio from video files and trim the audio according to your
+needs
 
 ## Description
 
-Audio Extract allows you to extract audio from video files and trim the audio according to your needs.
-It supports various video and audio formats and has a simple and user-friendly interface.
-
-It can also be used to trim audios.
+audio-extract is a Python library that allows you to extract audio from video files and trim the audio according to your
+needs. You can use it to create audio clips from movies, podcasts, or any other video source. It supports various audio
+and video formats, such as MP3, WAV, OGG, MP4, AVI, and MKV.
 
 ## Installing
 
 ```bash
 pip install audio-extract
 ```
 
 ## Executing the program
 
 #### Extract full audio
 
 ```python
-import audio_extract as audio_extract
+import audio_extract
 
 audio_extract.run(input_path="./video.mp4", output_path="./audio.mp3")
 ```
 
 This will create a mp3 file called `audio.mp3` that contains the full audio of the video file `video.mp4`.
 
 #### Extract sub clip audio
 
 ```python
-import audio_extract as audio_extract
+import audio_extract
 
 audio_extract.run(input_path="./video.mp4", output_path="./audio.mp3", start_time="00:30")
 ```
 
 This will create a mp3 file called `audio.mp3` that starts after the first 30 seconds of the video file `video.mp4`.
 
 #### Extract sub clip audio with custom duration
@@ -134,15 +134,14 @@
 ```bash
 audio-extract --input audio.mp3 --output new_audio.mp3 --start '00:05' --duration '01:15'
 ```
 
 This command trim the audio starting from `00:05` to `01:15` of the file `audio.mp3` to a mp3 file
 called `new_audio.mp3` that will have a duration of `01:10`.
 
-
 ## Authors
 
 Riadh Azzoun - [@riad-azz](https://github.com/riad-azz)
 
 ## License
 
 This project is licensed under the [MIT] License - see the LICENSE.md file for details
```

### Comparing `audio_extract-0.3.1/setup.py` & `audio_extract-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 ]
 
 long_description = open('README.md').read()
 long_description_content_type = 'text/markdown'
 
 setup(
     name='audio_extract',
-    version='0.3.1',
+    version='0.3.2',
     author='riad-azz',
     author_email='riadh.azzoun@hotmail.com',
     description='Extract and trim audio from videos or trim audios.',
     long_description=long_description,
     long_description_content_type=long_description_content_type,
     url='https://github.com/riad-azz/audio-extract',
     project_urls={
```


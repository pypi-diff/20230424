# Comparing `tmp/mediacatch-s2t-0.0.4.tar.gz` & `tmp/mediacatch-s2t-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mediacatch-s2t-0.0.4.tar", last modified: Wed Apr 12 14:49:16 2023, max compression
+gzip compressed data, was "mediacatch-s2t-0.0.5.tar", last modified: Mon Apr 24 13:42:18 2023, max compression
```

## Comparing `mediacatch-s2t-0.0.4.tar` & `mediacatch-s2t-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 frederik  (1002) mc       (10000)        0 2023-04-12 14:49:16.312311 mediacatch-s2t-0.0.4/
--rw-rw-r--   0 frederik  (1002) mc       (10000)    10172 2023-03-30 10:39:28.000000 mediacatch-s2t-0.0.4/LICENSE
--rw-rw-r--   0 frederik  (1002) mc       (10000)       27 2023-03-30 10:39:28.000000 mediacatch-s2t-0.0.4/MANIFEST.in
--rw-rw-r--   0 frederik  (1002) mc       (10000)    12910 2023-04-12 14:49:16.312311 mediacatch-s2t-0.0.4/PKG-INFO
--rw-rw-r--   0 frederik  (1002) mc       (10000)      795 2023-03-30 10:39:28.000000 mediacatch-s2t-0.0.4/README.md
--rw-rw-r--   0 frederik  (1002) mc       (10000)      898 2023-04-03 09:19:14.000000 mediacatch-s2t-0.0.4/pyproject.toml
--rw-rw-r--   0 frederik  (1002) mc       (10000)       38 2023-04-12 14:49:16.312311 mediacatch-s2t-0.0.4/setup.cfg
-drwxrwxr-x   0 frederik  (1002) mc       (10000)        0 2023-04-12 14:49:16.312311 mediacatch-s2t-0.0.4/src/
-drwxrwxr-x   0 frederik  (1002) mc       (10000)        0 2023-04-12 14:49:16.312311 mediacatch-s2t-0.0.4/src/mediacatch_s2t/
--rw-rw-r--   0 frederik  (1002) mc       (10000)      546 2023-04-03 09:19:14.000000 mediacatch-s2t-0.0.4/src/mediacatch_s2t/__init__.py
--rw-rw-r--   0 frederik  (1002) mc       (10000)     1181 2023-03-30 10:39:28.000000 mediacatch-s2t-0.0.4/src/mediacatch_s2t/__main__.py
--rw-rw-r--   0 frederik  (1002) mc       (10000)     5622 2023-04-03 09:19:14.000000 mediacatch-s2t-0.0.4/src/mediacatch_s2t/uploader.py
-drwxrwxr-x   0 frederik  (1002) mc       (10000)        0 2023-04-12 14:49:16.312311 mediacatch-s2t-0.0.4/src/mediacatch_s2t.egg-info/
--rw-rw-r--   0 frederik  (1002) mc       (10000)    12910 2023-04-12 14:49:16.000000 mediacatch-s2t-0.0.4/src/mediacatch_s2t.egg-info/PKG-INFO
--rw-rw-r--   0 frederik  (1002) mc       (10000)      414 2023-04-12 14:49:16.000000 mediacatch-s2t-0.0.4/src/mediacatch_s2t.egg-info/SOURCES.txt
--rw-rw-r--   0 frederik  (1002) mc       (10000)        1 2023-04-12 14:49:16.000000 mediacatch-s2t-0.0.4/src/mediacatch_s2t.egg-info/dependency_links.txt
--rw-rw-r--   0 frederik  (1002) mc       (10000)       54 2023-04-12 14:49:16.000000 mediacatch-s2t-0.0.4/src/mediacatch_s2t.egg-info/entry_points.txt
--rw-rw-r--   0 frederik  (1002) mc       (10000)       80 2023-04-12 14:49:16.000000 mediacatch-s2t-0.0.4/src/mediacatch_s2t.egg-info/requires.txt
--rw-rw-r--   0 frederik  (1002) mc       (10000)       15 2023-04-12 14:49:16.000000 mediacatch-s2t-0.0.4/src/mediacatch_s2t.egg-info/top_level.txt
-drwxrwxr-x   0 frederik  (1002) mc       (10000)        0 2023-04-12 14:49:16.312311 mediacatch-s2t-0.0.4/tests/
--rw-rw-r--   0 frederik  (1002) mc       (10000)     2447 2023-04-03 09:19:14.000000 mediacatch-s2t-0.0.4/tests/test_uploader.py
+drwxrwxr-x   0 frederik  (1002) mc       (10000)        0 2023-04-24 13:42:18.717869 mediacatch-s2t-0.0.5/
+-rw-rw-r--   0 frederik  (1002) mc       (10000)    10172 2023-03-30 10:39:28.000000 mediacatch-s2t-0.0.5/LICENSE
+-rw-rw-r--   0 frederik  (1002) mc       (10000)       27 2023-03-30 10:39:28.000000 mediacatch-s2t-0.0.5/MANIFEST.in
+-rw-rw-r--   0 frederik  (1002) mc       (10000)    12910 2023-04-24 13:42:18.717869 mediacatch-s2t-0.0.5/PKG-INFO
+-rw-rw-r--   0 frederik  (1002) mc       (10000)      795 2023-04-24 13:27:43.000000 mediacatch-s2t-0.0.5/README.md
+-rw-rw-r--   0 frederik  (1002) mc       (10000)      899 2023-04-24 13:31:58.000000 mediacatch-s2t-0.0.5/pyproject.toml
+-rw-rw-r--   0 frederik  (1002) mc       (10000)       38 2023-04-24 13:42:18.717869 mediacatch-s2t-0.0.5/setup.cfg
+drwxrwxr-x   0 frederik  (1002) mc       (10000)        0 2023-04-24 13:42:18.717869 mediacatch-s2t-0.0.5/src/
+drwxrwxr-x   0 frederik  (1002) mc       (10000)        0 2023-04-24 13:42:18.717869 mediacatch-s2t-0.0.5/src/mediacatch_s2t/
+-rw-rw-r--   0 frederik  (1002) mc       (10000)      546 2023-04-03 09:19:14.000000 mediacatch-s2t-0.0.5/src/mediacatch_s2t/__init__.py
+-rw-rw-r--   0 frederik  (1002) mc       (10000)     1297 2023-04-24 13:27:43.000000 mediacatch-s2t-0.0.5/src/mediacatch_s2t/__main__.py
+-rw-rw-r--   0 frederik  (1002) mc       (10000)     5729 2023-04-24 13:27:43.000000 mediacatch-s2t-0.0.5/src/mediacatch_s2t/uploader.py
+drwxrwxr-x   0 frederik  (1002) mc       (10000)        0 2023-04-24 13:42:18.717869 mediacatch-s2t-0.0.5/src/mediacatch_s2t.egg-info/
+-rw-rw-r--   0 frederik  (1002) mc       (10000)    12910 2023-04-24 13:42:18.000000 mediacatch-s2t-0.0.5/src/mediacatch_s2t.egg-info/PKG-INFO
+-rw-rw-r--   0 frederik  (1002) mc       (10000)      414 2023-04-24 13:42:18.000000 mediacatch-s2t-0.0.5/src/mediacatch_s2t.egg-info/SOURCES.txt
+-rw-rw-r--   0 frederik  (1002) mc       (10000)        1 2023-04-24 13:42:18.000000 mediacatch-s2t-0.0.5/src/mediacatch_s2t.egg-info/dependency_links.txt
+-rw-rw-r--   0 frederik  (1002) mc       (10000)       54 2023-04-24 13:42:18.000000 mediacatch-s2t-0.0.5/src/mediacatch_s2t.egg-info/entry_points.txt
+-rw-rw-r--   0 frederik  (1002) mc       (10000)       80 2023-04-24 13:42:18.000000 mediacatch-s2t-0.0.5/src/mediacatch_s2t.egg-info/requires.txt
+-rw-rw-r--   0 frederik  (1002) mc       (10000)       15 2023-04-24 13:42:18.000000 mediacatch-s2t-0.0.5/src/mediacatch_s2t.egg-info/top_level.txt
+drwxrwxr-x   0 frederik  (1002) mc       (10000)        0 2023-04-24 13:42:18.717869 mediacatch-s2t-0.0.5/tests/
+-rw-rw-r--   0 frederik  (1002) mc       (10000)     2464 2023-04-24 13:27:43.000000 mediacatch-s2t-0.0.5/tests/test_uploader.py
```

### Comparing `mediacatch-s2t-0.0.4/LICENSE` & `mediacatch-s2t-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mediacatch-s2t-0.0.4/PKG-INFO` & `mediacatch-s2t-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mediacatch-s2t
-Version: 0.0.4
+Version: 0.0.5
 Summary: Upload a media file and get the transcription link.
 Author-email: MediaCatch <support@mediacatch.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -196,15 +196,15 @@
 mediacatch-s2t is the [MediaCatch](https://mediacatch.io/) service for uploading a file in python and get the transcription result in a link. This module requires python3.7 or above.
 
 
 You can use it on your CLI
 ```bash
 pip install mediacatch_s2t
 
-python -m mediacatch_s2t <path/to/your/media/file> <api_key>
+python -m mediacatch_s2t <api_key> <path/to/your/media/file>
 ```
 
 Or import it as a module
 ```bash
 from mediacatch_s2t.uploader import upload_and_get_transcription
 
 result = upload_and_get_transcription('path/to/your/media/file', 'api_key')
```

### Comparing `mediacatch-s2t-0.0.4/README.md` & `mediacatch-s2t-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 mediacatch-s2t is the [MediaCatch](https://mediacatch.io/) service for uploading a file in python and get the transcription result in a link. This module requires python3.7 or above.
 
 
 You can use it on your CLI
 ```bash
 pip install mediacatch_s2t
 
-python -m mediacatch_s2t <path/to/your/media/file> <api_key>
+python -m mediacatch_s2t <api_key> <path/to/your/media/file>
 ```
 
 Or import it as a module
 ```bash
 from mediacatch_s2t.uploader import upload_and_get_transcription
 
 result = upload_and_get_transcription('path/to/your/media/file', 'api_key')
```

### Comparing `mediacatch-s2t-0.0.4/src/mediacatch_s2t/__init__.py` & `mediacatch-s2t-0.0.5/src/mediacatch_s2t/__init__.py`

 * *Files identical despite different names*

### Comparing `mediacatch-s2t-0.0.4/src/mediacatch_s2t/__main__.py` & `mediacatch-s2t-0.0.5/src/mediacatch_s2t/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 from rich.console import Console
 from mediacatch_s2t import uploader
 
 
 def main() -> None:
     parser = argparse.ArgumentParser(
         prog='mediacatch_s2t',
-        usage='%(prog)s [options] file api_key',
+        usage='%(prog)s [options] api_key file',
         description='Upload a media file and get the transcription from MediaCatch.'
     )
-    parser.add_argument("file", type=str, help="A media file.")
     parser.add_argument("api_key", type=str, help="MediaCatch API key.")
+    parser.add_argument("file", type=str, help="A media file.")
+    parser.add_argument("--language", type=str, default='da', help="The main language in the file.")
     args = parser.parse_args()
 
     console = Console()
     with console.status(
             "[bold green]Uploading file to MediaCatch..."):
-        result = uploader.upload_and_get_transcription(args.file, args.api_key)
+        result = uploader.upload_and_get_transcription(args.file, args.api_key, args.language)
         if result['status'] == 'error':
             sys.exit(
                 f"Error occurred:\n{result['message']}. "
                 f"Please contact support@mediacatch.io for further information."
             )
         console.print(f"[bold]transcription url: {result['url']}")
         console.print(
```

### Comparing `mediacatch-s2t-0.0.4/src/mediacatch_s2t/uploader.py` & `mediacatch-s2t-0.0.5/src/mediacatch_s2t/uploader.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,18 @@
     error: str
 
 class UploaderException(Exception):
     pass
 
 
 class Uploader:
-    def __init__(self, file, api_key):
+    def __init__(self, file, api_key, language='da'):
         self.file = file
         self.api_key = api_key
+        self.language = language
         self.file_id = None
 
     def _is_file_exist(self):
         return pathlib.Path(self.file).is_file()
 
     def _is_response_error(self, response):
         if response.status_code >= 400:
@@ -149,14 +150,15 @@
             return result
 
         mime_file = {
             "duration": file_duration,
             "filename": pathlib.Path(self.file).name,
             "file_ext": pathlib.Path(self.file).suffix,
             "filesize": os.path.getsize(self.file),
+            "language": self.language,
         }
         try:
             _upload_url = self._get_upload_url(mime_file)
             url = _upload_url.get('url')
             data = _upload_url.get('fields')
             self.file_id = _upload_url.get('id')
 
@@ -172,9 +174,9 @@
             "status": "uploaded",
             "estimated_processing_time": self.estimated_result_time(file_duration),
             "message": "The file has been uploaded."
         }
         return result
 
 
-def upload_and_get_transcription(file, api_key):
-    return Uploader(file, api_key).upload_file()
+def upload_and_get_transcription(file, api_key, language):
+    return Uploader(file, api_key, language).upload_file()
```

### Comparing `mediacatch-s2t-0.0.4/src/mediacatch_s2t.egg-info/PKG-INFO` & `mediacatch-s2t-0.0.5/src/mediacatch_s2t.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mediacatch-s2t
-Version: 0.0.4
+Version: 0.0.5
 Summary: Upload a media file and get the transcription link.
 Author-email: MediaCatch <support@mediacatch.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -196,15 +196,15 @@
 mediacatch-s2t is the [MediaCatch](https://mediacatch.io/) service for uploading a file in python and get the transcription result in a link. This module requires python3.7 or above.
 
 
 You can use it on your CLI
 ```bash
 pip install mediacatch_s2t
 
-python -m mediacatch_s2t <path/to/your/media/file> <api_key>
+python -m mediacatch_s2t <api_key> <path/to/your/media/file>
 ```
 
 Or import it as a module
 ```bash
 from mediacatch_s2t.uploader import upload_and_get_transcription
 
 result = upload_and_get_transcription('path/to/your/media/file', 'api_key')
```

### Comparing `mediacatch-s2t-0.0.4/tests/test_uploader.py` & `mediacatch-s2t-0.0.5/tests/test_uploader.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,9 +59,9 @@
     )
     expected_output = {
         'estimated_processing_time': 10,
         'message': 'The file has been uploaded.',
         'status': 'uploaded',
         'url': 'https://s2t.mediacatch.io/result?id=some-id&api_key=fake-key'
     }
-    assert Uploader('fake-file', 'fake-key').upload_file() == expected_output
+    assert Uploader('fake-file', 'fake-key', 'fake-language').upload_file() == expected_output
```


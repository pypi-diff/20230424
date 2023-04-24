# Comparing `tmp/unwanted_content_detector-0.1.7.tar.gz` & `tmp/unwanted_content_detector-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unwanted_content_detector-0.1.7.tar", max compression
+gzip compressed data, was "unwanted_content_detector-0.1.8.tar", max compression
```

## Comparing `unwanted_content_detector-0.1.7.tar` & `unwanted_content_detector-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      928 2023-04-22 22:35:19.139135 unwanted_content_detector-0.1.7/README.md
--rw-r--r--   0        0        0      639 2023-04-22 22:33:34.904828 unwanted_content_detector-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       31 2023-04-13 21:09:25.299508 unwanted_content_detector-0.1.7/unwanted_content_detector/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 20:42:32.601085 unwanted_content_detector-0.1.7/unwanted_content_detector/data/__init__.py
--rw-r--r--   0        0        0    11051 2023-04-22 20:59:25.756725 unwanted_content_detector-0.1.7/unwanted_content_detector/data/data.csv
--rw-r--r--   0        0        0      936 2023-04-22 22:29:01.290289 unwanted_content_detector-0.1.7/unwanted_content_detector/data/data_loader.py
--rw-r--r--   0        0        0      490 2023-04-01 11:23:42.326632 unwanted_content_detector-0.1.7/unwanted_content_detector/data/generative_prompts.txt
--rw-r--r--   0        0        0      498 2023-04-22 21:44:07.359639 unwanted_content_detector-0.1.7/unwanted_content_detector/detector.py
--rw-r--r--   0        0        0      161 2023-04-02 10:45:59.495528 unwanted_content_detector-0.1.7/unwanted_content_detector/entities.py
--rw-r--r--   0        0        0     1350 2023-04-22 21:45:45.686191 unwanted_content_detector-0.1.7/unwanted_content_detector/evaluator/evaluator.py
--rw-r--r--   0        0        0        0 2023-04-01 11:49:01.792441 unwanted_content_detector-0.1.7/unwanted_content_detector/models/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 21:09:25.300529 unwanted_content_detector-0.1.7/unwanted_content_detector/models/distilbert_finetuned/__init__.py
--rw-r--r--   0        0        0     1017 2023-04-22 21:44:35.878588 unwanted_content_detector-0.1.7/unwanted_content_detector/models/distilbert_finetuned/inference.py
--rw-r--r--   0        0        0     3844 2023-04-22 21:45:56.970345 unwanted_content_detector-0.1.7/unwanted_content_detector/models/distilbert_finetuned/train.py
--rw-r--r--   0        0        0     1047 2023-04-22 22:26:56.548900 unwanted_content_detector-0.1.7/unwanted_content_detector/models/upload.py
--rw-r--r--   0        0        0     1636 1970-01-01 00:00:00.000000 unwanted_content_detector-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      928 2023-04-22 22:35:19.139135 unwanted_content_detector-0.1.8/README.md
+-rw-r--r--   0        0        0      656 2023-04-24 10:18:37.795722 unwanted_content_detector-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0       31 2023-04-13 21:09:25.299508 unwanted_content_detector-0.1.8/unwanted_content_detector/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 20:42:32.601085 unwanted_content_detector-0.1.8/unwanted_content_detector/data/__init__.py
+-rw-r--r--   0        0        0    11051 2023-04-22 20:59:25.756725 unwanted_content_detector-0.1.8/unwanted_content_detector/data/data.csv
+-rw-r--r--   0        0        0      936 2023-04-22 22:29:01.290289 unwanted_content_detector-0.1.8/unwanted_content_detector/data/data_loader.py
+-rw-r--r--   0        0        0      490 2023-04-01 11:23:42.326632 unwanted_content_detector-0.1.8/unwanted_content_detector/data/generative_prompts.txt
+-rw-r--r--   0        0        0      498 2023-04-22 21:44:07.359639 unwanted_content_detector-0.1.8/unwanted_content_detector/detector.py
+-rw-r--r--   0        0        0      161 2023-04-02 10:45:59.495528 unwanted_content_detector-0.1.8/unwanted_content_detector/entities.py
+-rw-r--r--   0        0        0     1350 2023-04-22 21:45:45.686191 unwanted_content_detector-0.1.8/unwanted_content_detector/evaluator/evaluator.py
+-rw-r--r--   0        0        0        0 2023-04-01 11:49:01.792441 unwanted_content_detector-0.1.8/unwanted_content_detector/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 21:09:25.300529 unwanted_content_detector-0.1.8/unwanted_content_detector/models/distilbert_finetuned/__init__.py
+-rw-r--r--   0        0        0     1017 2023-04-22 21:44:35.878588 unwanted_content_detector-0.1.8/unwanted_content_detector/models/distilbert_finetuned/inference.py
+-rw-r--r--   0        0        0     3844 2023-04-22 21:45:56.970345 unwanted_content_detector-0.1.8/unwanted_content_detector/models/distilbert_finetuned/train.py
+-rw-r--r--   0        0        0     1047 2023-04-22 22:26:56.548900 unwanted_content_detector-0.1.8/unwanted_content_detector/models/upload.py
+-rw-r--r--   0        0        0     1674 1970-01-01 00:00:00.000000 unwanted_content_detector-0.1.8/PKG-INFO
```

### Comparing `unwanted_content_detector-0.1.7/README.md` & `unwanted_content_detector-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `unwanted_content_detector-0.1.7/pyproject.toml` & `unwanted_content_detector-0.1.8/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "unwanted-content-detector"
-version = "0.1.7"
+version = "0.1.8"
 description = "A library to detect undesired, unbranded, or harmful content"
 authors = ["Jean Carlo Machado <jean.machado@getyourguide.com>"]
 license = "Apache"
 readme = "README.md"
 packages = [{include = "unwanted_content_detector"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 fire = "^0.5.0"
 pandas = "^2.0.0"
 transformers = "^4.28.0"
 evaluate = "^0.4.0"
+torch = "^2.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.0"
 black = "^23.3.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `unwanted_content_detector-0.1.7/unwanted_content_detector/data/data.csv` & `unwanted_content_detector-0.1.8/unwanted_content_detector/data/data.csv`

 * *Files identical despite different names*

### Comparing `unwanted_content_detector-0.1.7/unwanted_content_detector/data/data_loader.py` & `unwanted_content_detector-0.1.8/unwanted_content_detector/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `unwanted_content_detector-0.1.7/unwanted_content_detector/evaluator/evaluator.py` & `unwanted_content_detector-0.1.8/unwanted_content_detector/evaluator/evaluator.py`

 * *Files identical despite different names*

### Comparing `unwanted_content_detector-0.1.7/unwanted_content_detector/models/distilbert_finetuned/inference.py` & `unwanted_content_detector-0.1.8/unwanted_content_detector/models/distilbert_finetuned/inference.py`

 * *Files identical despite different names*

### Comparing `unwanted_content_detector-0.1.7/unwanted_content_detector/models/distilbert_finetuned/train.py` & `unwanted_content_detector-0.1.8/unwanted_content_detector/models/distilbert_finetuned/train.py`

 * *Files identical despite different names*

### Comparing `unwanted_content_detector-0.1.7/unwanted_content_detector/models/upload.py` & `unwanted_content_detector-0.1.8/unwanted_content_detector/models/upload.py`

 * *Files identical despite different names*

### Comparing `unwanted_content_detector-0.1.7/PKG-INFO` & `unwanted_content_detector-0.1.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: unwanted-content-detector
-Version: 0.1.7
+Version: 0.1.8
 Summary: A library to detect undesired, unbranded, or harmful content
 License: Apache
 Author: Jean Carlo Machado
 Author-email: jean.machado@getyourguide.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: evaluate (>=0.4.0,<0.5.0)
 Requires-Dist: fire (>=0.5.0,<0.6.0)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
+Requires-Dist: torch (>=2.0.0,<3.0.0)
 Requires-Dist: transformers (>=4.28.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Unwanted Content Detector
 
 A library to detect undesired, unbranded, or harmful content
```


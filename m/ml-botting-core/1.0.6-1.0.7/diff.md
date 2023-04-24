# Comparing `tmp/ml_botting_core-1.0.6.tar.gz` & `tmp/ml_botting_core-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_botting_core-1.0.6.tar", last modified: Sun Apr 23 16:28:27 2023, max compression
+gzip compressed data, was "ml_botting_core-1.0.7.tar", last modified: Mon Apr 24 01:20:47 2023, max compression
```

## Comparing `ml_botting_core-1.0.6.tar` & `ml_botting_core-1.0.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:28:27.522061 ml_botting_core-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-23 16:26:56.000000 ml_botting_core-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-04-23 16:28:27.522061 ml_botting_core-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-04-23 16:26:56.000000 ml_botting_core-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-23 16:26:56.000000 ml_botting_core-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-23 16:28:27.522061 ml_botting_core-1.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:28:27.514060 ml_botting_core-1.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:28:27.518060 ml_botting_core-1.0.6/src/ml_botting_core/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-23 16:26:56.000000 ml_botting_core-1.0.6/src/ml_botting_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-23 16:26:56.000000 ml_botting_core-1.0.6/src/ml_botting_core/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:28:27.518060 ml_botting_core-1.0.6/src/ml_botting_core/classification/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 16:26:56.000000 ml_botting_core-1.0.6/src/ml_botting_core/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-04-23 16:26:56.000000 ml_botting_core-1.0.6/src/ml_botting_core/classification/universal_classifier_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:28:27.518060 ml_botting_core-1.0.6/src/ml_botting_core/general/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 16:26:56.000000 ml_botting_core-1.0.6/src/ml_botting_core/general/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-23 16:26:56.000000 ml_botting_core-1.0.6/src/ml_botting_core/general/general.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:28:27.518060 ml_botting_core-1.0.6/src/ml_botting_core/model_management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 16:26:56.000000 ml_botting_core-1.0.6/src/ml_botting_core/model_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-23 16:26:56.000000 ml_botting_core-1.0.6/src/ml_botting_core/model_management/download_models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 16:26:56.000000 ml_botting_core-1.0.6/src/ml_botting_core/model_management/load_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-04-23 16:26:56.000000 ml_botting_core-1.0.6/src/ml_botting_core/model_management/model_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:28:27.522061 ml_botting_core-1.0.6/src/ml_botting_core/prediction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 16:26:56.000000 ml_botting_core-1.0.6/src/ml_botting_core/prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-23 16:26:56.000000 ml_botting_core-1.0.6/src/ml_botting_core/prediction/prediction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:28:27.522061 ml_botting_core-1.0.6/src/ml_botting_core/regression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 16:26:56.000000 ml_botting_core-1.0.6/src/ml_botting_core/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 16:26:56.000000 ml_botting_core-1.0.6/src/ml_botting_core/regression/universal_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:28:27.518060 ml_botting_core-1.0.6/src/ml_botting_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-04-23 16:28:27.000000 ml_botting_core-1.0.6/src/ml_botting_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-23 16:28:27.000000 ml_botting_core-1.0.6/src/ml_botting_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 16:28:27.000000 ml_botting_core-1.0.6/src/ml_botting_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-23 16:28:27.000000 ml_botting_core-1.0.6/src/ml_botting_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:28:27.522061 ml_botting_core-1.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-23 16:26:56.000000 ml_botting_core-1.0.6/tests/test_universal_predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:20:47.190830 ml_botting_core-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-24 01:18:57.000000 ml_botting_core-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-04-24 01:20:47.190830 ml_botting_core-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-04-24 01:18:57.000000 ml_botting_core-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-24 01:18:57.000000 ml_botting_core-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-24 01:20:47.190830 ml_botting_core-1.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:20:47.186830 ml_botting_core-1.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:20:47.186830 ml_botting_core-1.0.7/src/ml_botting_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-24 01:18:57.000000 ml_botting_core-1.0.7/src/ml_botting_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-24 01:18:57.000000 ml_botting_core-1.0.7/src/ml_botting_core/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:20:47.190830 ml_botting_core-1.0.7/src/ml_botting_core/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:18:57.000000 ml_botting_core-1.0.7/src/ml_botting_core/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-04-24 01:18:57.000000 ml_botting_core-1.0.7/src/ml_botting_core/classification/universal_classifier_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:20:47.190830 ml_botting_core-1.0.7/src/ml_botting_core/general/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:18:57.000000 ml_botting_core-1.0.7/src/ml_botting_core/general/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-24 01:18:57.000000 ml_botting_core-1.0.7/src/ml_botting_core/general/general.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:20:47.190830 ml_botting_core-1.0.7/src/ml_botting_core/model_management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:18:57.000000 ml_botting_core-1.0.7/src/ml_botting_core/model_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-24 01:18:57.000000 ml_botting_core-1.0.7/src/ml_botting_core/model_management/download_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:18:57.000000 ml_botting_core-1.0.7/src/ml_botting_core/model_management/load_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-04-24 01:18:57.000000 ml_botting_core-1.0.7/src/ml_botting_core/model_management/model_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:20:47.190830 ml_botting_core-1.0.7/src/ml_botting_core/prediction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:18:57.000000 ml_botting_core-1.0.7/src/ml_botting_core/prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-24 01:18:57.000000 ml_botting_core-1.0.7/src/ml_botting_core/prediction/prediction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:20:47.190830 ml_botting_core-1.0.7/src/ml_botting_core/regression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:18:57.000000 ml_botting_core-1.0.7/src/ml_botting_core/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 01:18:57.000000 ml_botting_core-1.0.7/src/ml_botting_core/regression/universal_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:20:47.186830 ml_botting_core-1.0.7/src/ml_botting_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-04-24 01:20:47.000000 ml_botting_core-1.0.7/src/ml_botting_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-24 01:20:47.000000 ml_botting_core-1.0.7/src/ml_botting_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 01:20:47.000000 ml_botting_core-1.0.7/src/ml_botting_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-24 01:20:47.000000 ml_botting_core-1.0.7/src/ml_botting_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 01:20:47.190830 ml_botting_core-1.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-24 01:18:57.000000 ml_botting_core-1.0.7/tests/test_universal_predictor.py
```

### Comparing `ml_botting_core-1.0.6/LICENSE` & `ml_botting_core-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ml_botting_core-1.0.6/PKG-INFO` & `ml_botting_core-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml_botting_core
-Version: 1.0.6
+Version: 1.0.7
 Summary: Making ML more accessible to botting apps. Solving Complex UI Challenges w/ ML.
 Home-page: https://github.com/darkmatter2222/ml_botting_core
 Author: Ryan Susman
 Author-email: ryansusman@gmail.com
 Project-URL: Bug Tracker, https://github.com/darkmatter2222/ml_botting_core/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml_botting_core-1.0.6/README.md` & `ml_botting_core-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ml_botting_core-1.0.6/setup.cfg` & `ml_botting_core-1.0.7/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ml_botting_core
-version = 1.0.6
+version = 1.0.7
 author = Ryan Susman
 author_email = ryansusman@gmail.com
 description = Making ML more accessible to botting apps. Solving Complex UI Challenges w/ ML.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/darkmatter2222/ml_botting_core
 project_urls =
```

### Comparing `ml_botting_core-1.0.6/src/ml_botting_core/base.py` & `ml_botting_core-1.0.7/src/ml_botting_core/base.py`

 * *Files identical despite different names*

### Comparing `ml_botting_core-1.0.6/src/ml_botting_core/classification/universal_classifier_trainer.py` & `ml_botting_core-1.0.7/src/ml_botting_core/classification/universal_classifier_trainer.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from PIL import Image, ImageDraw
 
 from tensorflow.keras import layers
 from tensorflow.keras.models import Sequential
 from sklearn.metrics import confusion_matrix
 from sklearn.utils.class_weight import compute_class_weight
 
+
 def build_and_train(root_image_directory, model_location,
                     model_name, epochs=10,
                     resize_ratio=0.2, auto_balance_data=True):
     data_dir = pathlib.Path(root_image_directory)
 
     image_list = list(data_dir.glob('*/*.png'))
     image_count = len(image_list)
@@ -48,17 +49,14 @@
         y_train = np.concatenate([y for x, y in train_ds], axis=0)
 
         class_weights = compute_class_weight(class_weight="balanced", classes=np.unique(y_train), y=y_train)
         class_weights = {i: w for i, w in enumerate(class_weights)}
 
         print(f"Class Weights: {class_weights}")
 
-
-
-
     AUTOTUNE = tf.data.AUTOTUNE
 
     train_ds = train_ds.cache().shuffle(1000).prefetch(buffer_size=AUTOTUNE)
     val_ds = val_ds.cache().prefetch(buffer_size=AUTOTUNE)
 
     num_classes = len(class_names)
 
@@ -80,29 +78,45 @@
                   loss=tf.keras.losses.SparseCategoricalCrossentropy(from_logits=True),
                   metrics=['accuracy'])
 
     history = model.fit(
         train_ds,
         validation_data=val_ds,
         epochs=epochs,
-        class_weight=class_weights
+        class_weight=class_weights,
+        shuffle=True
     )
+
     train_data = list(train_ds)
-    features = np.concatenate([train_data[n][0] for n in range(0, len(train_data))])
-    targets = np.concatenate([train_data[n][1] for n in range(0, len(train_data))])
-    print(targets)
-    predictions = model.predict(features)
-    print(predictions.argmax(1))
+    train_features = np.concatenate([train_data[n][0] for n in range(0, len(train_data))])
+    train_targets = np.concatenate([train_data[n][1] for n in range(0, len(train_data))])
+
+    val_data = list(val_ds)
+    val_features = np.concatenate([val_data[n][0] for n in range(0, len(val_data))])
+    val_targets = np.concatenate([val_data[n][1] for n in range(0, len(val_data))])
+
+    train_predictions = model.predict(train_features)
+    val_predictions = model.predict(val_features)
+
+    train_cf = confusion_matrix(train_targets, train_predictions.argmax(1).astype(int))
+    val_cf = confusion_matrix(val_targets, val_predictions.argmax(1).astype(int))
+
+    eval_results = model.evaluate(val_features, val_targets)
 
-    cf = confusion_matrix(targets, predictions.argmax(1).astype(int))
+    decision_threshold = 0.8
+    if eval_results[1] != 1.0:
+        decision_threshold = 1.0 - ((1.0 - eval_results[1]) * 2)
 
     model.save(model_location)
 
     stats = {
-        'cm': cf
+        'train_cm': train_cf,
+        'val_cm': val_cf,
+        "eval_results": eval_results
     }
     rendering = {
         'image_resize': [img_height, img_width],
-        'classes': class_names
+        'classes': class_names,
+        'decision_threshold': decision_threshold
     }
 
     return stats, rendering
```

### Comparing `ml_botting_core-1.0.6/src/ml_botting_core/model_management/download_models.py` & `ml_botting_core-1.0.7/src/ml_botting_core/model_management/download_models.py`

 * *Files identical despite different names*

### Comparing `ml_botting_core-1.0.6/src/ml_botting_core/model_management/model_manager.py` & `ml_botting_core-1.0.7/src/ml_botting_core/model_management/model_manager.py`

 * *Files identical despite different names*

### Comparing `ml_botting_core-1.0.6/src/ml_botting_core/prediction/prediction.py` & `ml_botting_core-1.0.7/src/ml_botting_core/prediction/prediction.py`

 * *Files identical despite different names*

### Comparing `ml_botting_core-1.0.6/src/ml_botting_core.egg-info/PKG-INFO` & `ml_botting_core-1.0.7/src/ml_botting_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-botting-core
-Version: 1.0.6
+Version: 1.0.7
 Summary: Making ML more accessible to botting apps. Solving Complex UI Challenges w/ ML.
 Home-page: https://github.com/darkmatter2222/ml_botting_core
 Author: Ryan Susman
 Author-email: ryansusman@gmail.com
 Project-URL: Bug Tracker, https://github.com/darkmatter2222/ml_botting_core/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml_botting_core-1.0.6/src/ml_botting_core.egg-info/SOURCES.txt` & `ml_botting_core-1.0.7/src/ml_botting_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*


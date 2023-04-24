# Comparing `tmp/lifeomic_patient_ml_types-7.4.3.tar.gz` & `tmp/lifeomic_patient_ml_types-7.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeomic_patient_ml_types-7.4.3.tar", max compression
+gzip compressed data, was "lifeomic_patient_ml_types-7.5.0.tar", max compression
```

## Comparing `lifeomic_patient_ml_types-7.4.3.tar` & `lifeomic_patient_ml_types-7.5.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    13961 2023-04-21 15:41:03.372321 lifeomic_patient_ml_types-7.4.3/lifeomic_patient_ml_types/schemas.py
--rw-r--r--   0        0        0      664 2023-04-21 15:42:21.140698 lifeomic_patient_ml_types-7.4.3/pyproject.toml
--rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.4.3/setup.py
--rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.4.3/PKG-INFO
+-rw-r--r--   0        0        0    14143 2023-04-24 14:01:40.035117 lifeomic_patient_ml_types-7.5.0/lifeomic_patient_ml_types/schemas.py
+-rw-r--r--   0        0        0      664 2023-04-24 14:02:54.210471 lifeomic_patient_ml_types-7.5.0/pyproject.toml
+-rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.5.0/setup.py
+-rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.5.0/PKG-INFO
```

### Comparing `lifeomic_patient_ml_types-7.4.3/lifeomic_patient_ml_types/schemas.py` & `lifeomic_patient_ml_types-7.5.0/lifeomic_patient_ml_types/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,14 +110,26 @@
     areas: List[ImageSegmentationArea]
 
 
 class LabelFileData(BaseModel):
     __root__: ImageSegmentationLabelData
 
 
+class Tag(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    name: str
+    value: str
+
+
+class Tags(BaseModel):
+    __root__: List[Tag]
+
+
 class LabelBase(BaseModel):
     class Config:
         extra = Extra.allow
 
     isConfirmed: Optional[bool] = None
     """
     A confirmed label is believed to be correct and may be used during training and evaluation.
@@ -126,14 +138,15 @@
     """
     The email address or other identifier of the user who last confirmed this label.
     """
     updatedAt: Optional[float] = None
     """
     Timestamp for when the label was last updated or created expressed as milliseconds since the UTC epoch.
     """
+    tags: Optional[Tags] = None
 
 
 class Mask(BaseModel):
     """
     The fileId of an image containing per-pixel labels
     """
```

### Comparing `lifeomic_patient_ml_types-7.4.3/pyproject.toml` & `lifeomic_patient_ml_types-7.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lifeomic-patient-ml-types"
-version = "7.4.3"
+version = "7.5.0"
 description = "Shared types for the patient-ml-service repos."
 authors = ["LifeOmic <development@lifeomic.com>"]
 license = "UNLICENSED"
 
 [tool.poe.tasks]
 format = "black lifeomic_patient_ml_types"
 lint = "pyright lifeomic_patient_ml_types"
```

### Comparing `lifeomic_patient_ml_types-7.4.3/setup.py` & `lifeomic_patient_ml_types-7.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['lifeomic_patient_ml_types']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'lifeomic-patient-ml-types',
-    'version': '7.4.3',
+    'version': '7.5.0',
     'description': 'Shared types for the patient-ml-service repos.',
     'long_description': 'None',
     'author': 'LifeOmic',
     'author_email': 'development@lifeomic.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```


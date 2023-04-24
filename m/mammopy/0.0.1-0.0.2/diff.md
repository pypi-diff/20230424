# Comparing `tmp/mammopy-0.0.1.tar.gz` & `tmp/mammopy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mammopy-0.0.1.tar", max compression
+gzip compressed data, was "mammopy-0.0.2.tar", max compression
```

## Comparing `mammopy-0.0.1.tar` & `mammopy-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       47 2023-04-24 11:29:48.761366 mammopy-0.0.1/MammoPy/__init__.py
--rw-r--r--   0        0        0     9407 2023-04-24 11:27:42.702682 mammopy-0.0.1/MammoPy/mammopy.py
--rw-r--r--   0        0        0      590 2023-04-24 11:33:38.818271 mammopy-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4036 2023-04-24 11:31:21.449211 mammopy-0.0.1/README.md
--rw-r--r--   0        0        0     4834 1970-01-01 00:00:00.000000 mammopy-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       47 2023-04-24 11:29:48.761366 mammopy-0.0.2/MammoPy/__init__.py
+-rw-r--r--   0        0        0     9407 2023-04-24 11:27:42.702682 mammopy-0.0.2/MammoPy/mammopy.py
+-rw-r--r--   0        0        0      590 2023-04-24 11:37:31.620818 mammopy-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3988 2023-04-24 11:37:20.210344 mammopy-0.0.2/README.md
+-rw-r--r--   0        0        0     4786 1970-01-01 00:00:00.000000 mammopy-0.0.2/PKG-INFO
```

### Comparing `mammopy-0.0.1/MammoPy/mammopy.py` & `mammopy-0.0.2/MammoPy/mammopy.py`

 * *Files identical despite different names*

### Comparing `mammopy-0.0.1/pyproject.toml` & `mammopy-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mammopy"
-version = "0.0.1"
+version = "0.0.2"
 description = "A unified solution for mammogram image analysis and interpretation"
 authors = ["UEF Cancer <uef.cancergroup@gmail.com>"]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `mammopy-0.0.1/README.md` & `mammopy-0.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,73 +1,73 @@
 <p align="center">
   <img src="https://cdn.imgbin.com/10/3/23/imgbin-breast-cancer-senology-mammography-diego-JcEW147fdbivCyrvC5vykSPj3.jpg" height="200">
 </p>
 
-# MamToolKit
+# MammoPy
 ### A Comprehensive Deep Learning Library for Mammogram Assessment
 [![PyPI version](https://badge.fury.io/py/mktoolkit.svg)](https://badge.fury.io/py/mktoolkit)
 ![GitHub](https://img.shields.io/github/license/mktoolkit/mktoolkit)
 [![Downloads](https://static.pepy.tech/badge/mktoolkit)](https://pepy.tech/project/mktoolkit)
 
-**[[Documentation]](https://github.com/uefcancer/mamtoolkit/)**
+**[[Documentation]](https://github.com/uefcancer/mammopy/)**
 | **[[Paper]]()** 
 | **[[Notebook examples]]()** 
 | **[[Web applications]]()** 
 
-**Welcome to `MamToolKit` Repository!** `MamToolKit` is a python-based library designed to facilitate the creation of mammogram image analysis pipelines . The library includes plug-and-play modules to perform:
+**Welcome to `MammoPy` Repository!** `MammoPy` is a python-based library designed to facilitate the creation of mammogram image analysis pipelines . The library includes plug-and-play modules to perform:
 - Standard mammogram image pre-processing (e.g., *normalization*, *bounding box cropping*, and *DICOM to jpeg conversion*)
 - Mammogram assessment pipelines (e.g., *breast area segmentation*, *dense tissue segmentation*, and *percentage density estimation*)
 - Modeling deep learning architectures for various downstream tasks  (e.g., *micro-calcification* and *mass detection*)
 - Feature attribution-based interpretability techniques (e.g., *GradCAM*, *GradCAM++*, and *LRP*)
 - Visualization 
 
 All the functionalities are grouped under a user-friendly API. 
 
-If you encounter any issue or have questions regarding the library, feel free to [open a GitHub issue](https://github.com/uefcancer/mamtoolkit/issues). We'll do our best to address it. 
+If you encounter any issue or have questions regarding the library, feel free to [open a GitHub issue](https://github.com/uefcancer/mammopy/issues). We'll do our best to address it. 
 
 # Installation 
 
 ## PyPI installer (recommended)
 
-`pip install -U mamtoolkit`
+`pip install -U mammopy`
 
 ## Development setup 
 
 - Clone the repo:
 
 ```
-git clone https://github.com/uefcancer/mktoolkit/mamtoolkit.git && cd mamtoolkit
+git clone https://github.com/uefcancer/mktoolkit/mammopy.git && cd mammopy
 ```
 
 - Create a conda environment:
 
 ```
 conda env create -f environment.yml
 ```
 **NOTE**: To use GPUs, install GPU compatible [Pytorch](https://pytorch.org/get-started/locally/), [Torchvision](https://pytorch.org/get-started/locally/) packages according to your OS, package manager, and CUDA.
 
 - Activate it:
 
 ```
-conda activate mamtoolkit
+conda activate mammopy
 ```
 
-- Add `MamToolKit` to your python path:
+- Add `MammoPy` to your python path:
 
 ```
-export PYTHONPATH="<PATH>/mamtoolkit:$PYTHONPATH"
+export PYTHONPATH="<PATH>/mammopy:$PYTHONPATH"
 ```
 
-# Using MamToolKit 
+# Using MammoPy 
 
-The `MamToolKit` library provides a set of helpers grouped in different modules, namely `preprocessing`, `assessment`, `interpretability`, and  `visualization`.  
+The `MammoPy` library provides a set of helpers grouped in different modules, namely `preprocessing`, `assessment`, `interpretability`, and  `visualization`.  
 
-For instance, with  `MamToolKit` library, we can load percentage mammogram density model (described in the [[Paper]](https://www.nature.com/articles/s41598-022-16141-2) ) and predict the non-dense area, dense tissue area, and estimate percentage density:
+For instance, with  `MammoPy` library, we can load percentage mammogram density model (described in the [[Paper]](https://www.nature.com/articles/s41598-022-16141-2) ) and predict the non-dense area, dense tissue area, and estimate percentage density:
 ```python
-import mamtoolkit as mg
+import mammopy as mg
 
 model = mg.load_model("base")
 result = mg.percentage_density(model, image_path) #path to mammogram image
 print(result)
 ```
 The `percentage_density()` method is a part of `assessment` module, which pre-processes the input image and converts it into the appropriate format and dimension accepted by the model. Then the model provides the analysis in forms of a dictionary with keys: non_dense_area, dense_area, and density.
 
@@ -77,15 +77,15 @@
 result['non_dense_area'] = 
 result['dense_area'] = 
 result['density']
 ```
 
 ## License
 
-The MamToolKit library is released under the MIT License. See [LICENSE] (https://github.com/openai/whisper/blob/main/LICENSE) for further details.
+The MammoPy library is released under the MIT License. See [LICENSE] (https://github.com/openai/whisper/blob/main/LICENSE) for further details.
 
 If you use this library, please consider citing:
 ```
 @article{gudhe2022area,
   title={Area-based breast percentage density estimation in mammograms using weight-adaptive multitask learning},
   author={Gudhe, Naga Raju and Behravan, Hamid and Sudah, Mazen and Okuma, Hidemi and Vanninen, Ritva and Kosma, Veli-Matti and Mannermaa, Arto},
   journal={Scientific reports},
```

### Comparing `mammopy-0.0.1/PKG-INFO` & `mammopy-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mammopy
-Version: 0.0.1
+Version: 0.0.2
 Summary: A unified solution for mammogram image analysis and interpretation
 Author: UEF Cancer
 Author-email: uef.cancergroup@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -23,76 +23,76 @@
 Requires-Dist: tqdm (==4.65.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://cdn.imgbin.com/10/3/23/imgbin-breast-cancer-senology-mammography-diego-JcEW147fdbivCyrvC5vykSPj3.jpg" height="200">
 </p>
 
-# MamToolKit
+# MammoPy
 ### A Comprehensive Deep Learning Library for Mammogram Assessment
 [![PyPI version](https://badge.fury.io/py/mktoolkit.svg)](https://badge.fury.io/py/mktoolkit)
 ![GitHub](https://img.shields.io/github/license/mktoolkit/mktoolkit)
 [![Downloads](https://static.pepy.tech/badge/mktoolkit)](https://pepy.tech/project/mktoolkit)
 
-**[[Documentation]](https://github.com/uefcancer/mamtoolkit/)**
+**[[Documentation]](https://github.com/uefcancer/mammopy/)**
 | **[[Paper]]()** 
 | **[[Notebook examples]]()** 
 | **[[Web applications]]()** 
 
-**Welcome to `MamToolKit` Repository!** `MamToolKit` is a python-based library designed to facilitate the creation of mammogram image analysis pipelines . The library includes plug-and-play modules to perform:
+**Welcome to `MammoPy` Repository!** `MammoPy` is a python-based library designed to facilitate the creation of mammogram image analysis pipelines . The library includes plug-and-play modules to perform:
 - Standard mammogram image pre-processing (e.g., *normalization*, *bounding box cropping*, and *DICOM to jpeg conversion*)
 - Mammogram assessment pipelines (e.g., *breast area segmentation*, *dense tissue segmentation*, and *percentage density estimation*)
 - Modeling deep learning architectures for various downstream tasks  (e.g., *micro-calcification* and *mass detection*)
 - Feature attribution-based interpretability techniques (e.g., *GradCAM*, *GradCAM++*, and *LRP*)
 - Visualization 
 
 All the functionalities are grouped under a user-friendly API. 
 
-If you encounter any issue or have questions regarding the library, feel free to [open a GitHub issue](https://github.com/uefcancer/mamtoolkit/issues). We'll do our best to address it. 
+If you encounter any issue or have questions regarding the library, feel free to [open a GitHub issue](https://github.com/uefcancer/mammopy/issues). We'll do our best to address it. 
 
 # Installation 
 
 ## PyPI installer (recommended)
 
-`pip install -U mamtoolkit`
+`pip install -U mammopy`
 
 ## Development setup 
 
 - Clone the repo:
 
 ```
-git clone https://github.com/uefcancer/mktoolkit/mamtoolkit.git && cd mamtoolkit
+git clone https://github.com/uefcancer/mktoolkit/mammopy.git && cd mammopy
 ```
 
 - Create a conda environment:
 
 ```
 conda env create -f environment.yml
 ```
 **NOTE**: To use GPUs, install GPU compatible [Pytorch](https://pytorch.org/get-started/locally/), [Torchvision](https://pytorch.org/get-started/locally/) packages according to your OS, package manager, and CUDA.
 
 - Activate it:
 
 ```
-conda activate mamtoolkit
+conda activate mammopy
 ```
 
-- Add `MamToolKit` to your python path:
+- Add `MammoPy` to your python path:
 
 ```
-export PYTHONPATH="<PATH>/mamtoolkit:$PYTHONPATH"
+export PYTHONPATH="<PATH>/mammopy:$PYTHONPATH"
 ```
 
-# Using MamToolKit 
+# Using MammoPy 
 
-The `MamToolKit` library provides a set of helpers grouped in different modules, namely `preprocessing`, `assessment`, `interpretability`, and  `visualization`.  
+The `MammoPy` library provides a set of helpers grouped in different modules, namely `preprocessing`, `assessment`, `interpretability`, and  `visualization`.  
 
-For instance, with  `MamToolKit` library, we can load percentage mammogram density model (described in the [[Paper]](https://www.nature.com/articles/s41598-022-16141-2) ) and predict the non-dense area, dense tissue area, and estimate percentage density:
+For instance, with  `MammoPy` library, we can load percentage mammogram density model (described in the [[Paper]](https://www.nature.com/articles/s41598-022-16141-2) ) and predict the non-dense area, dense tissue area, and estimate percentage density:
 ```python
-import mamtoolkit as mg
+import mammopy as mg
 
 model = mg.load_model("base")
 result = mg.percentage_density(model, image_path) #path to mammogram image
 print(result)
 ```
 The `percentage_density()` method is a part of `assessment` module, which pre-processes the input image and converts it into the appropriate format and dimension accepted by the model. Then the model provides the analysis in forms of a dictionary with keys: non_dense_area, dense_area, and density.
 
@@ -102,15 +102,15 @@
 result['non_dense_area'] = 
 result['dense_area'] = 
 result['density']
 ```
 
 ## License
 
-The MamToolKit library is released under the MIT License. See [LICENSE] (https://github.com/openai/whisper/blob/main/LICENSE) for further details.
+The MammoPy library is released under the MIT License. See [LICENSE] (https://github.com/openai/whisper/blob/main/LICENSE) for further details.
 
 If you use this library, please consider citing:
 ```
 @article{gudhe2022area,
   title={Area-based breast percentage density estimation in mammograms using weight-adaptive multitask learning},
   author={Gudhe, Naga Raju and Behravan, Hamid and Sudah, Mazen and Okuma, Hidemi and Vanninen, Ritva and Kosma, Veli-Matti and Mannermaa, Arto},
   journal={Scientific reports},
```


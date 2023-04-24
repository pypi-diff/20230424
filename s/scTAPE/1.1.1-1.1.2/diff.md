# Comparing `tmp/scTAPE-1.1.1.tar.gz` & `tmp/scTAPE-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scTAPE-1.1.1.tar", last modified: Wed Apr 19 13:59:09 2023, max compression
+gzip compressed data, was "scTAPE-1.1.2.tar", last modified: Mon Apr 24 16:01:07 2023, max compression
```

## Comparing `scTAPE-1.1.1.tar` & `scTAPE-1.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 chan       (501) staff       (20)        0 2023-04-19 13:59:09.815255 scTAPE-1.1.1/
--rw-r--r--   0 chan       (501) staff       (20)    35149 2023-04-19 13:46:34.000000 scTAPE-1.1.1/LICENSE
--rw-r--r--   0 chan       (501) staff       (20)      340 2023-04-19 13:59:09.815113 scTAPE-1.1.1/PKG-INFO
--rw-r--r--   0 chan       (501) staff       (20)     5180 2023-04-19 13:46:34.000000 scTAPE-1.1.1/README.md
-drwxr-xr-x   0 chan       (501) staff       (20)        0 2023-04-19 13:59:09.814243 scTAPE-1.1.1/TAPE/
--rw-r--r--   0 chan       (501) staff       (20)       88 2023-04-19 13:46:34.000000 scTAPE-1.1.1/TAPE/__init__.py
--rw-r--r--   0 chan       (501) staff       (20)     7521 2023-04-19 13:52:44.000000 scTAPE-1.1.1/TAPE/deconvolution.py
--rw-r--r--   0 chan       (501) staff       (20)     7953 2023-04-19 13:46:34.000000 scTAPE-1.1.1/TAPE/model.py
--rw-r--r--   0 chan       (501) staff       (20)     6097 2023-04-19 13:46:34.000000 scTAPE-1.1.1/TAPE/simulation.py
--rw-r--r--   0 chan       (501) staff       (20)     6727 2023-04-19 13:46:34.000000 scTAPE-1.1.1/TAPE/train.py
--rw-r--r--   0 chan       (501) staff       (20)     6421 2023-04-19 13:53:39.000000 scTAPE-1.1.1/TAPE/utils.py
-drwxr-xr-x   0 chan       (501) staff       (20)        0 2023-04-19 13:59:09.814915 scTAPE-1.1.1/scTAPE.egg-info/
--rw-r--r--   0 chan       (501) staff       (20)      340 2023-04-19 13:59:09.000000 scTAPE-1.1.1/scTAPE.egg-info/PKG-INFO
--rw-r--r--   0 chan       (501) staff       (20)      275 2023-04-19 13:59:09.000000 scTAPE-1.1.1/scTAPE.egg-info/SOURCES.txt
--rw-r--r--   0 chan       (501) staff       (20)        1 2023-04-19 13:59:09.000000 scTAPE-1.1.1/scTAPE.egg-info/dependency_links.txt
--rw-r--r--   0 chan       (501) staff       (20)      113 2023-04-19 13:59:09.000000 scTAPE-1.1.1/scTAPE.egg-info/requires.txt
--rw-r--r--   0 chan       (501) staff       (20)        5 2023-04-19 13:59:09.000000 scTAPE-1.1.1/scTAPE.egg-info/top_level.txt
--rw-r--r--   0 chan       (501) staff       (20)       38 2023-04-19 13:59:09.815311 scTAPE-1.1.1/setup.cfg
--rw-r--r--   0 chan       (501) staff       (20)      671 2023-04-19 13:58:02.000000 scTAPE-1.1.1/setup.py
+drwxr-xr-x   0 chan       (501) staff       (20)        0 2023-04-24 16:01:07.653273 scTAPE-1.1.2/
+-rw-r--r--   0 chan       (501) staff       (20)    35149 2023-04-19 13:46:34.000000 scTAPE-1.1.2/LICENSE
+-rw-r--r--   0 chan       (501) staff       (20)      340 2023-04-24 16:01:07.653144 scTAPE-1.1.2/PKG-INFO
+-rw-r--r--   0 chan       (501) staff       (20)     5488 2023-04-24 16:00:57.000000 scTAPE-1.1.2/README.md
+drwxr-xr-x   0 chan       (501) staff       (20)        0 2023-04-24 16:01:07.652366 scTAPE-1.1.2/TAPE/
+-rw-r--r--   0 chan       (501) staff       (20)       88 2023-04-19 13:46:34.000000 scTAPE-1.1.2/TAPE/__init__.py
+-rw-r--r--   0 chan       (501) staff       (20)     7522 2023-04-24 15:52:30.000000 scTAPE-1.1.2/TAPE/deconvolution.py
+-rw-r--r--   0 chan       (501) staff       (20)     7953 2023-04-19 13:46:34.000000 scTAPE-1.1.2/TAPE/model.py
+-rw-r--r--   0 chan       (501) staff       (20)     6097 2023-04-19 13:46:34.000000 scTAPE-1.1.2/TAPE/simulation.py
+-rw-r--r--   0 chan       (501) staff       (20)     6727 2023-04-19 13:46:34.000000 scTAPE-1.1.2/TAPE/train.py
+-rw-r--r--   0 chan       (501) staff       (20)     6421 2023-04-19 13:53:39.000000 scTAPE-1.1.2/TAPE/utils.py
+drwxr-xr-x   0 chan       (501) staff       (20)        0 2023-04-24 16:01:07.652983 scTAPE-1.1.2/scTAPE.egg-info/
+-rw-r--r--   0 chan       (501) staff       (20)      340 2023-04-24 16:01:07.000000 scTAPE-1.1.2/scTAPE.egg-info/PKG-INFO
+-rw-r--r--   0 chan       (501) staff       (20)      275 2023-04-24 16:01:07.000000 scTAPE-1.1.2/scTAPE.egg-info/SOURCES.txt
+-rw-r--r--   0 chan       (501) staff       (20)        1 2023-04-24 16:01:07.000000 scTAPE-1.1.2/scTAPE.egg-info/dependency_links.txt
+-rw-r--r--   0 chan       (501) staff       (20)      111 2023-04-24 16:01:07.000000 scTAPE-1.1.2/scTAPE.egg-info/requires.txt
+-rw-r--r--   0 chan       (501) staff       (20)        5 2023-04-24 16:01:07.000000 scTAPE-1.1.2/scTAPE.egg-info/top_level.txt
+-rw-r--r--   0 chan       (501) staff       (20)       38 2023-04-24 16:01:07.653328 scTAPE-1.1.2/setup.cfg
+-rw-r--r--   0 chan       (501) staff       (20)      669 2023-04-24 16:00:16.000000 scTAPE-1.1.2/setup.py
```

### Comparing `scTAPE-1.1.1/LICENSE` & `scTAPE-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scTAPE-1.1.1/README.md` & `scTAPE-1.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # TAPE: Tissue-AdaPtive autoEncoder for accurate deconvolution and gene expression analysis
 
-![scTAPE](https://img.shields.io/badge/scTAPE-v1.1.0-blue)![GPL](https://img.shields.io/github/license/poseidonchan/TAPE)[![DOI](https://zenodo.org/badge/386163911.svg)](https://zenodo.org/badge/latestdoi/386163911)
+![scTAPE](https://img.shields.io/badge/scTAPE-v1.1.2-blue)![GPL](https://img.shields.io/github/license/poseidonchan/TAPE)[![DOI](https://zenodo.org/badge/386163911.svg)](https://zenodo.org/badge/latestdoi/386163911)
 
 **This model is able to accurately deconvolve bulk RNA-seq data into cell fractions and predict cell-type-specific gene expression at cell-type level based on scRNA-seq data**.
 
 related article ***Deep autoencoder for interpretable tissue-adaptive deconvolution and cell-type-specific gene analysis*** is accepted by *Nature Communications*
 
 ## Setup
 
@@ -14,16 +14,18 @@
 
 ```bash
 pip install torch==1.8.0+cu111 torchvision==0.9.0+cu111 torchaudio==0.8.0 -f https://download.pytorch.org/whl/torch_stable.html
 ```
 
 If PyTorch is successfully installed, then TAPE could be installed from PyPI directly:
 
+***Update: I relax the dependece requirements to enable the compatibility with current packages***.
+
 ```bash
-pip install scTAPE
+pip install scTAPE==1.1.2
 ```
 Usually, the installation time depends on your downloading speed.
 ## Usage
 
 Required Files:
 1. single-cell reference: txt format, indices are cell types, columns are gene names
 2. bulk data: tabular format, needed to specify the seperation ('\t',','or others), indices are sample names, columns are gene names
@@ -31,29 +33,30 @@
 
 ***Warning: single-cell reference and bulk samples should contain the same cell types***
 
 ```python
 # basic example
 from TAPE import Deconvolution
 SignatureMatrix, CellFractionPrediction = \
-    Deconvolution(sc_ref, bulkdata, sep='\t',
+    Deconvolution(sc_ref, bulkdata, sep='\t', scaler='mms',
                   datatype='counts', genelenfile='./GeneLength.txt',
                   mode='overall', adaptive=True, variance_threshold=0.98,
                   save_model_name=None,
                   batch_size=128, epochs=128, seed=1)
 ```
 parameters:
 
-1. datatype: use '**TPM**', '**FPKM**' or '**counts**'. Users can choose different normalization method based on your single-cell seq technique, if single-cell data is from 10X Genomics, users should use '**counts**' to maintain a resonable procedure. The explanation could be found from the [webpage](https://kb.10xgenomics.com/hc/en-us/articles/115003684783-Should-I-calculate-TPM-RPKM-or-FPKM-instead-of-counts-for-10x-Genomics-data-).
-2. mode: '**overall**' or '**high-resolution**'. If you need signature matrix for each sample, use 'high-resolution' mode.
-3. adaptive: **True** or **False**. If this is False, then it would not predict signature matrix, the return will be ***None***
-4. variance_threshold: Float number from 0 to 1, it means how many genes you want to keep (in proportion) according to variance from high to low.
-5. batch_size: **int**, related to training result. 32-128 are recommended. Smaller batch_size leads to more time consumption.
-6. epochs: **int**, related to training result. Typically, *5000-10000* iterations are enough for TAPE, the relation is $epochs=\frac{iteration \times batch\_size}{sampleing\_num}$
-7. seed: now, TAPE supports pinning the random seed to make results being reproducible.
+1. scaler: use '**mms**' or '**ss**' scaler to preprocess datasets, 'mms' stands for min-max scaler, 'ss' stands for standard scaler. In the paper, all datasets were tested using 'mms'.
+2. datatype: use '**TPM**', '**FPKM**' or '**counts**'. Users can choose different normalization method based on your single-cell seq technique, if single-cell data is from 10X Genomics, users should use '**counts**' to maintain a resonable procedure. The explanation could be found from the [webpage](https://kb.10xgenomics.com/hc/en-us/articles/115003684783-Should-I-calculate-TPM-RPKM-or-FPKM-instead-of-counts-for-10x-Genomics-data-).
+3. mode: '**overall**' or '**high-resolution**'. If you need signature matrix for each sample, use 'high-resolution' mode.
+4. adaptive: **True** or **False**. If this is False, then it would not predict signature matrix, the return will be ***None***
+5. variance_threshold: Float number from 0 to 1, it means how many genes you want to keep (in proportion) according to variance from high to low.
+6. batch_size: **int**, related to training result. 32-128 are recommended. Smaller batch_size leads to more time consumption.
+7. epochs: **int**, related to training result. Typically, *5000-10000* iterations are enough for TAPE, the relation is $epochs=\frac{iteration \times batch\_size}{sampleing\_num}$
+8. seed: now, TAPE supports pinning the random seed to make results being reproducible.
 
 Since the original implementation of Scaden [[repository](https://github.com/KevinMenden/scaden)] [[paper](https://www.science.org/doi/10.1126/sciadv.aba2619)] is not easy for us to test, we implemented the PyTorch version of Scaden. If you want to use Scaden to deconvolve bulk RNA-seq data, you can use the following code:
 
 ```python
 from TAPE.deconvolution import ScadenDeconvolution
 Pred = ScadenDeconvolution(sc_ref, bulkdata, sep='\t',
                            batch_size=128, epochs=128)
```

### Comparing `scTAPE-1.1.1/TAPE/deconvolution.py` & `scTAPE-1.1.2/TAPE/deconvolution.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import anndata
 import pandas as pd
 from .simulation import generate_simulated_data
 from .utils import ProcessInputData
 from .train import train_model, predict, reproducibility
 from .model import scaden, AutoEncoder
 
-def Deconvolution(necessary_data, real_bulk, sep='\t', variance_threshold=0.8,
+def Deconvolution(necessary_data, real_bulk, sep='\t', variance_threshold=0.98,
                   scaler='mms',
                   datatype='counts', genelenfile=None, d_prior=None,
                   mode='overall', adaptive=True,
                   save_model_name=None, sparse=True,
                   batch_size=128, epochs=128, seed=0):
     """
     :param necessary_data: for single-cell data, txt file and dataframe are supported. for simulated data, file location
```

### Comparing `scTAPE-1.1.1/TAPE/model.py` & `scTAPE-1.1.2/TAPE/model.py`

 * *Files identical despite different names*

### Comparing `scTAPE-1.1.1/TAPE/simulation.py` & `scTAPE-1.1.2/TAPE/simulation.py`

 * *Files identical despite different names*

### Comparing `scTAPE-1.1.1/TAPE/train.py` & `scTAPE-1.1.2/TAPE/train.py`

 * *Files identical despite different names*

### Comparing `scTAPE-1.1.1/TAPE/utils.py` & `scTAPE-1.1.2/TAPE/utils.py`

 * *Files identical despite different names*

### Comparing `scTAPE-1.1.1/setup.py` & `scTAPE-1.1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 setup(
     name = 'scTAPE',
-    version = '1.1.1',
+    version = '1.1.2',
     description = 'deep learning tools for bulk RNA-seq deconvolution and gene expression analysis',
     author = 'Yanshuo Chen',
     author_email = 'poseidonchan@icloud.com',
     url = 'https://github.com/poseidonchan/TAPE',
     license = 'GPL-3.0 License',
     packages = find_packages(),
-    python_requires='==3.7',
+    python_requires='>=3.7',
     platforms = 'any',
     install_requires = [
         'torch>=1.8.0',
         'numpy>=1.21',
-        'pandas>=1.3.1',
+        'pandas>=1.0',
         'matplotlib>=3.4',
         'anndata>=0.7.6',
         'tqdm>=4.6',
         'scikit-learn>=0.23',
         'seaborn>=0.11'
     ],
 )
```


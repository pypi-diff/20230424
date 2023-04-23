# Comparing `tmp/pyseistr-0.0.4.2.tar.gz` & `tmp/pyseistr-0.0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyseistr-0.0.4.2.tar", last modified: Sat Oct 29 14:09:44 2022, max compression
+gzip compressed data, was "pyseistr-0.0.4.3.tar", last modified: Sun Apr 23 22:01:58 2023, max compression
```

## Comparing `pyseistr-0.0.4.2.tar` & `pyseistr-0.0.4.3.tar`

### file list

```diff
@@ -1,37 +1,40 @@
-drwxrwxr-x   0 chenyk    (1000) chenyk    (1000)        0 2022-10-29 14:09:44.959500 pyseistr-0.0.4.2/
--rw-rw-r--   0 chenyk    (1000) chenyk    (1000)     1173 2022-10-29 14:09:44.959500 pyseistr-0.0.4.2/PKG-INFO
--rw-rw-r--   0 chenyk    (1000) chenyk    (1000)     5038 2022-10-29 13:49:10.000000 pyseistr-0.0.4.2/README.md
-drwxrwxr-x   0 chenyk    (1000) chenyk    (1000)        0 2022-10-29 14:09:44.957500 pyseistr-0.0.4.2/pyseistr/
--rw-rw-r--   0 chenyk    (1000) chenyk    (1000)     1788 2022-10-29 13:49:10.000000 pyseistr-0.0.4.2/pyseistr/__init__.py
--rw-rw-r--   0 chenyk    (1000) chenyk    (1000)     5563 2022-10-29 13:49:10.000000 pyseistr-0.0.4.2/pyseistr/bp.py
--rw-rw-r--   0 chenyk    (1000) chenyk    (1000)     4551 2022-10-29 13:49:10.000000 pyseistr-0.0.4.2/pyseistr/dip2d.py
--rw-rw-r--   0 chenyk    (1000) chenyk    (1000)     6346 2022-10-29 13:49:10.000000 pyseistr-0.0.4.2/pyseistr/dip3d.py
--rw-rw-r--   0 chenyk    (1000) chenyk    (1000)     7494 2022-10-29 13:49:10.000000 pyseistr-0.0.4.2/pyseistr/divne.py
--rw-rw-r--   0 chenyk    (1000) chenyk    (1000)     1044 2022-10-29 13:49:10.000000 pyseistr-0.0.4.2/pyseistr/fk.py
--rw-rw-r--   0 chenyk    (1000) chenyk    (1000)     4464 2022-10-29 13:49:10.000000 pyseistr-0.0.4.2/pyseistr/mf.py
--rw-rw-r--   0 chenyk    (1000) chenyk    (1000)     4557 2022-10-29 13:49:10.000000 pyseistr-0.0.4.2/pyseistr/operators.py
--rw-rw-r--   0 chenyk    (1000) chenyk    (1000)      696 2022-10-29 13:49:10.000000 pyseistr-0.0.4.2/pyseistr/plot.py
--rw-rw-r--   0 chenyk    (1000) chenyk    (1000)     6801 2022-10-29 13:49:10.000000 pyseistr-0.0.4.2/pyseistr/pwspray2d.py
--rw-rw-r--   0 chenyk    (1000) chenyk    (1000)     9410 2022-10-29 13:49:10.000000 pyseistr-0.0.4.2/pyseistr/pwspray3d.py
--rw-rw-r--   0 chenyk    (1000) chenyk    (1000)      657 2022-10-29 13:49:10.000000 pyseistr-0.0.4.2/pyseistr/ricker.py
--rw-rw-r--   0 chenyk    (1000) chenyk    (1000)     2372 2022-10-29 13:49:10.000000 pyseistr-0.0.4.2/pyseistr/soint3d.py
--rw-rw-r--   0 chenyk    (1000) chenyk    (1000)     7771 2022-10-29 13:49:10.000000 pyseistr-0.0.4.2/pyseistr/solvers.py
--rw-rw-r--   0 chenyk    (1000) chenyk    (1000)     1263 2022-10-29 13:49:10.000000 pyseistr-0.0.4.2/pyseistr/somean2d.py
--rw-rw-r--   0 chenyk    (1000) chenyk    (1000)     1496 2022-10-29 13:49:10.000000 pyseistr-0.0.4.2/pyseistr/somean3d.py
--rw-rw-r--   0 chenyk    (1000) chenyk    (1000)     2823 2022-10-29 13:49:10.000000 pyseistr-0.0.4.2/pyseistr/somf2d.py
--rw-rw-r--   0 chenyk    (1000) chenyk    (1000)     2932 2022-10-29 13:49:10.000000 pyseistr-0.0.4.2/pyseistr/somf3d.py
-drwxrwxr-x   0 chenyk    (1000) chenyk    (1000)        0 2022-10-29 14:09:44.958500 pyseistr-0.0.4.2/pyseistr/src/
--rw-rw-r--   0 chenyk    (1000) chenyk    (1000)    14535 2022-10-29 13:49:10.000000 pyseistr-0.0.4.2/pyseistr/src/bp_cfuns.c
--rw-rw-r--   0 chenyk    (1000) chenyk    (1000)    42325 2022-10-29 14:05:17.000000 pyseistr-0.0.4.2/pyseistr/src/dip_cfuns.c
--rw-rw-r--   0 chenyk    (1000) chenyk    (1000)    35411 2022-10-29 13:49:10.000000 pyseistr-0.0.4.2/pyseistr/src/sof3d_cfuns.c
--rw-rw-r--   0 chenyk    (1000) chenyk    (1000)    34486 2022-10-29 13:49:10.000000 pyseistr-0.0.4.2/pyseistr/src/sof_cfuns.c
--rw-rw-r--   0 chenyk    (1000) chenyk    (1000)    31174 2022-10-29 13:49:10.000000 pyseistr-0.0.4.2/pyseistr/src/soint3d_cfuns.c
-drwxrwxr-x   0 chenyk    (1000) chenyk    (1000)        0 2022-10-29 14:09:44.958500 pyseistr-0.0.4.2/pyseistr.egg-info/
--rw-rw-r--   0 chenyk    (1000) chenyk    (1000)     1173 2022-10-29 14:09:44.000000 pyseistr-0.0.4.2/pyseistr.egg-info/PKG-INFO
--rw-rw-r--   0 chenyk    (1000) chenyk    (1000)      680 2022-10-29 14:09:44.000000 pyseistr-0.0.4.2/pyseistr.egg-info/SOURCES.txt
--rw-rw-r--   0 chenyk    (1000) chenyk    (1000)        1 2022-10-29 14:09:44.000000 pyseistr-0.0.4.2/pyseistr.egg-info/dependency_links.txt
--rw-rw-r--   0 chenyk    (1000) chenyk    (1000)        1 2022-10-29 14:00:19.000000 pyseistr-0.0.4.2/pyseistr.egg-info/not-zip-safe
--rw-rw-r--   0 chenyk    (1000) chenyk    (1000)       53 2022-10-29 14:09:44.000000 pyseistr-0.0.4.2/pyseistr.egg-info/requires.txt
--rw-rw-r--   0 chenyk    (1000) chenyk    (1000)       54 2022-10-29 14:09:44.000000 pyseistr-0.0.4.2/pyseistr.egg-info/top_level.txt
--rw-rw-r--   0 chenyk    (1000) chenyk    (1000)       38 2022-10-29 14:09:44.959500 pyseistr-0.0.4.2/setup.cfg
--rw-rw-r--   0 chenyk    (1000) chenyk    (1000)     2376 2022-10-29 14:09:39.000000 pyseistr-0.0.4.2/setup.py
+drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-04-23 22:01:58.872939 pyseistr-0.0.4.3/
+-rw-r--r--   0 chenyk     (501) staff       (20)    35149 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3/LICENSE
+-rw-r--r--   0 chenyk     (501) staff       (20)     1165 2023-04-23 22:01:58.872546 pyseistr-0.0.4.3/PKG-INFO
+-rw-r--r--   0 chenyk     (501) staff       (20)     5858 2023-04-23 22:01:30.000000 pyseistr-0.0.4.3/README.md
+drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-04-23 22:01:58.862369 pyseistr-0.0.4.3/pyseistr/
+-rw-r--r--   0 chenyk     (501) staff       (20)     1893 2023-04-22 20:38:05.000000 pyseistr-0.0.4.3/pyseistr/__init__.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     5563 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3/pyseistr/bp.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     4852 2023-04-23 20:41:03.000000 pyseistr-0.0.4.3/pyseistr/dip2d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     6636 2023-04-23 20:41:11.000000 pyseistr-0.0.4.3/pyseistr/dip3d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     7494 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3/pyseistr/divne.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     1044 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3/pyseistr/fk.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     4464 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3/pyseistr/mf.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     4557 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3/pyseistr/operators.py
+-rw-r--r--   0 chenyk     (501) staff       (20)      696 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3/pyseistr/plot.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     6801 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3/pyseistr/pwspray2d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     9410 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3/pyseistr/pwspray3d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)      657 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3/pyseistr/ricker.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     1990 2023-04-23 18:14:53.000000 pyseistr-0.0.4.3/pyseistr/soint2d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     2300 2023-04-22 20:42:00.000000 pyseistr-0.0.4.3/pyseistr/soint3d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     7771 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3/pyseistr/solvers.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     1263 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3/pyseistr/somean2d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     1496 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3/pyseistr/somean3d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     2823 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3/pyseistr/somf2d.py
+-rw-r--r--   0 chenyk     (501) staff       (20)     2932 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3/pyseistr/somf3d.py
+drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-04-23 22:01:58.871936 pyseistr-0.0.4.3/pyseistr/src/
+-rw-r--r--   0 chenyk     (501) staff       (20)    14513 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3/pyseistr/src/bp_cfuns.c
+-rw-r--r--   0 chenyk     (501) staff       (20)    42528 2023-04-23 21:14:48.000000 pyseistr-0.0.4.3/pyseistr/src/dip_cfuns.c
+-rw-r--r--   0 chenyk     (501) staff       (20)    35389 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3/pyseistr/src/sof3d_cfuns.c
+-rw-r--r--   0 chenyk     (501) staff       (20)    34464 2022-10-30 03:00:33.000000 pyseistr-0.0.4.3/pyseistr/src/sof_cfuns.c
+-rw-r--r--   0 chenyk     (501) staff       (20)    49126 2023-04-23 18:43:05.000000 pyseistr-0.0.4.3/pyseistr/src/soint2d_cfuns.c
+-rw-r--r--   0 chenyk     (501) staff       (20)    31152 2023-04-22 19:39:19.000000 pyseistr-0.0.4.3/pyseistr/src/soint3d_cfuns.c
+drwxr-xr-x   0 chenyk     (501) staff       (20)        0 2023-04-23 22:01:58.866471 pyseistr-0.0.4.3/pyseistr.egg-info/
+-rw-r--r--   0 chenyk     (501) staff       (20)     1165 2023-04-23 22:01:58.000000 pyseistr-0.0.4.3/pyseistr.egg-info/PKG-INFO
+-rw-r--r--   0 chenyk     (501) staff       (20)      737 2023-04-23 22:01:58.000000 pyseistr-0.0.4.3/pyseistr.egg-info/SOURCES.txt
+-rw-r--r--   0 chenyk     (501) staff       (20)        1 2023-04-23 22:01:58.000000 pyseistr-0.0.4.3/pyseistr.egg-info/dependency_links.txt
+-rw-r--r--   0 chenyk     (501) staff       (20)        1 2023-04-22 19:39:47.000000 pyseistr-0.0.4.3/pyseistr.egg-info/not-zip-safe
+-rw-r--r--   0 chenyk     (501) staff       (20)       53 2023-04-23 22:01:58.000000 pyseistr-0.0.4.3/pyseistr.egg-info/requires.txt
+-rw-r--r--   0 chenyk     (501) staff       (20)       66 2023-04-23 22:01:58.000000 pyseistr-0.0.4.3/pyseistr.egg-info/top_level.txt
+-rw-r--r--   0 chenyk     (501) staff       (20)       38 2023-04-23 22:01:58.873088 pyseistr-0.0.4.3/setup.cfg
+-rw-r--r--   0 chenyk     (501) staff       (20)     2666 2023-04-23 22:01:45.000000 pyseistr-0.0.4.3/setup.py
```

### Comparing `pyseistr-0.0.4.2/PKG-INFO` & `pyseistr-0.0.4.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pyseistr
-Version: 0.0.4.2
+Version: 0.0.4.3
 Summary: A python package for structural denoising and interpolation of multi-channel seismic data
 Home-page: https://github.com/aaspip/pyseistr
 Author: pyseistr developing team
 Author-email: chenyk2016@gmail.com
 License: GNU General Public License, Version 3 (GPLv3)
-Description: Source code: https://github.com/aaspip/pyseistr
 Keywords: seismology,earthquake seismology,exploration seismology,array seismology,denoising,science,engineering,structure,local slope,filtering
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Provides-Extra: docs
+License-File: LICENSE
+
+Source code: https://github.com/aaspip/pyseistr
```

### Comparing `pyseistr-0.0.4.2/README.md` & `pyseistr-0.0.4.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 ======
 
 ## Description
 
 **Pyseistr** is a python package for structural denoising and interpolation of multi-channel seismic data. The latest version has incorporated both Python and C (hundreds of times faster) implementations of the embedded functions. We keep both implementations for both educational and production purposes. This package has a variety of applications in both exploration and earthquake seismology.
 
 ## Reference
-Chen et al., 2022, Pyseistr: a python package for structural denoising and interpolation of multi-channel seismic data, under review. 
+Chen et al., 2023, Pyseistr: a python package for structural denoising and interpolation of multi-channel seismic data, Seismological Research Letters, 94(1), 457-472. 
 
 BibTeX:
 
 	@article{pyseistr,
 	  title={Pyseistr: a python package for structural denoising and interpolation of multi-channel seismic data},
 	  author={Yangkang Chen and Alexandros Savvaidis and Sergey Fomel and Yunfeng Chen and Omar M. Saad and Yapo Abol{\'e} Serge Innocent Obou{\'e} and Quan Zhang and Wei Chen},
-	  journal={TBD},
-	  volume={1},
+	  journal={Seismological Research Letters},
+	  volume={94},
 	  number={1},
-	  pages={1-10},
-	  year={2022}
+	  pages={457-472},
+	  year={2023}
 	}
 
 -----------
 ## Copyright
     The pyseistr developing team, 2021-present
 -----------
 
@@ -38,15 +38,15 @@
     cd pyseistr
     pip install -v -e .
 or using Pypi
 
     pip install pyseistr
 
 -----------
-## Examples
+## DEMO scripts
     The "demo" directory contains all runable scripts to demonstrate different applications of pyseistr. 
 
 -----------
 ## Gallery
 The gallery figures of the pyseistr package can be found at
     https://github.com/aaspip/gallery/tree/main/pyseistr
 Each figure in the gallery directory corresponds to a DEMO script in the "demo" directory with the exactly the same file name.
@@ -55,23 +55,23 @@
 ## Dependence Packages
 * scipy 
 * numpy 
 * matplotlib
 
 -----------
 ## Modules
-    dip2d.py  -> 2D local slope estimation (including both python and C implementations)
-    dip3d.py  -> 3D local slope estimation (including both python and C implementations)
-    divne.py  -> element-wise division constrained by shaping regularization (python implementation)
-    somean2d.py -> 2D structure-oriented mean filter  (including both python and C implementations)
-    somean3d.py -> 3D structure-oriented mean filter  (including both python and C implementations)
+    dip2d.py  	-> 2D local slope estimation (including both python and C implementations)
+    dip3d.py  	-> 3D local slope estimation (including both python and C implementations)
+    divne.py  	-> element-wise division constrained by shaping regularization (python implementation)
+    somean2d.py 	-> 2D structure-oriented mean filter  (including both python and C implementations)
+    somean3d.py 	-> 3D structure-oriented mean filter  (including both python and C implementations)
     somf2d.py 	-> 2D structure-oriented median filter  (including both python and C implementations)
     somf3d.py 	-> 3D structure-oriented median filter  (including both python and C implementations)
-    soint2d.py  -> 2D structural interpolation  (including both python and C implementations)
-    soint3d.py  -> 3D structural interpolation  (including both python and C implementations)
+    soint2d.py  	-> 2D structural interpolation  (including both python and C implementations)
+    soint3d.py  	-> 3D structural interpolation  (including both python and C implementations)
     ricker.py	-> Ricker wavelet
     bp.py		-> Butterworth bandpass filter (including both python and C implementations)
     fk.py		-> FK dip filter
     plot.py		-> seismic plotting functions
     
 -----------
 ## Development
@@ -122,7 +122,16 @@
 <img src='https://github.com/aaspip/gallery/blob/main/pyseistr/test_pyseistr_rf.png' alt='Slicing' width=960/>
 
 # Example 8 (structure-oriented distributed acoustic sensing (DAS) data processing) 
 Produced by demos/test_pyseistr_das.py
 
 <img src='https://github.com/aaspip/gallery/blob/main/pyseistr/test_pyseistr_das.png' alt='Slicing' width=960/>
 
+# Below are New Examples in addition to the results in the original paper
+
+# Below is a paper for 2D structure-oriented interpolation of a multi-channel synthetic seismic data
+Generated by [demos/test_pyseistr_soint2d.m](https://github.com/aaspip/pyseistr/tree/main/demos/test_pyseistr_soint2d.m)
+<img src='https://github.com/aaspip/gallery/blob/main/pyseistr/test_pyseistr_soint2d.png' alt='comp' width=960/>
+
+# Below is a paper for 2D structure-oriented interpolation of a seafloor dataset
+Generated by [demos/test_pyseistr_soint2d.m](https://github.com/aaspip/pyseistr/tree/main/demos/test_pyseistr_soint2d_seafloor.m)
+<img src='https://github.com/aaspip/gallery/blob/main/pyseistr/test_pyseistr_soint2d_seafloor.png' alt='comp' width=960/>
```

### Comparing `pyseistr-0.0.4.2/pyseistr/__init__.py` & `pyseistr-0.0.4.3/pyseistr/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 from .dip2d import dip2d
 from .dip3d import dip3d
 from .divne import divne
 from .somean2d import somean2d
 from .somean3d import somean3d
 from .somf2d import somf2d
 from .somf3d import somf3d
+from .soint2d import soint2d #structure-oriented interpolation for 2D data
 from .soint3d import soint3d #structure-oriented interpolation for 3D data
 from .ricker import ricker
 from .bp import bandpass
 from .fk import fkdip
 from .plot import cseis
 
 
@@ -61,14 +62,15 @@
 ## C versions
 from .dip2d import dip2dc
 from .dip3d import dip3dc
 from .somean2d import somean2dc
 from .somean3d import somean3dc
 from .somf2d import somf2dc
 from .somf3d import somf3dc
+from .soint2d import soint2dc
 from .soint3d import soint3dc
 from .bp import bandpassc
 
 from dipcfun import *
 from sofcfun import *
 from sof3dcfun import *
 from bpcfun import *
```

### Comparing `pyseistr-0.0.4.2/pyseistr/bp.py` & `pyseistr-0.0.4.3/pyseistr/bp.py`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.2/pyseistr/dip2d.py` & `pyseistr-0.0.4.3/pyseistr/dip2d.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 import numpy as np
 from dipcfun import *
 
 def dip2d(din,niter=5,liter=20,order=2,eps_dv=0.01, eps_cg=1, tol_cg=0.000001,rect=[10,10,1],verb=1):
-	# dip2d: dip estimation based on shaping regularized PWD algorithm 
-	# (independent implementation)
-	#
-	# INPUT
-	# din: input data (nt*nx)
-	# niter: number of nonlinear iterations
-	# liter: number of linear iterations (in divn)
-	# order: accuracy order
-	# eps_dv: eps for divn  (default: 0.01)
-	# eps_cg: eps for CG    (default: 1)
-	# tol_cg: tolerence for CG (default: 0.000001)
-	# rect:  smoothing radius (ndim*1)
-	# verb: verbosity flag
-	#
-	# OUTPUT
-	# dip:  2D slope
+	'''
+	dip2d: dip estimation based on shaping regularized PWD algorithm 
+	(independent implementation)
+	
+	INPUT
+	din: input data (nt*nx)
+	niter: number of nonlinear iterations
+	liter: number of linear iterations (in divn)
+	order: accuracy order
+	eps_dv: eps for divn  (default: 0.01)
+	eps_cg: eps for CG    (default: 1)
+	tol_cg: tolerence for CG (default: 0.000001)
+	rect:  smoothing radius (ndim*1)
+	verb: verbosity flag
+	
+	OUTPUT
+	dip:  2D slope
+	
+	NOTE: mask function is not enabled yet (will do in the future)
+	'''
+	
 	from .divne import divne
 	
 	p0 = 0.0;
 	nj1 = 1;
 	nj2 = 1;
 	dim = 3;
 	
@@ -41,68 +46,80 @@
 		"""corresponding to the eq.21 in the paper  (Wang et al., 2022)"""
 		[u1,u2] = conv_allpass(din,dip,order); 
 		ratio = divne(-u2, u1, liter, rect, n, eps_dv, eps_cg, tol_cg,verb);
 		dip=dip+ratio;
 
 	return dip
 
-def dip2dc(din,niter=5,liter=20,order=2,eps_dv=0.01, eps_cg=1, tol_cg=0.000001,rect=[10,10,1],verb=1):
-	# dip2d: dip estimation based on shaping regularized PWD algorithm 
-	# (independent implementation)
-	#
-	# INPUT
-	# din: input data (nt*nx)
-	# niter: number of nonlinear iterations
-	# liter: number of linear iterations (in divn)
-	# order: accuracy order
-	# eps_dv: eps for divn  (default: 0.01)
-	# eps_cg: eps for CG    (default: 1)
-	# tol_cg: tolerence for CG (default: 0.000001)
-	# rect:  smoothing radius (ndim*1)
-	# verb: verbosity flag
-	#
-	# OUTPUT
-	# dip:  2D slope
+def dip2dc(din,mask=None,niter=5,liter=20,order=2,eps_dv=0.01, eps_cg=1, tol_cg=0.000001,rect=[10,10,1],verb=1):
+	'''
+	dip2dc: dip estimation based on shaping regularized PWD algorithm 
+	(C implementation)
+	
+	INPUT
+	din: input data (nt*nx)
+	niter: number of nonlinear iterations
+	liter: number of linear iterations (in divn)
+	order: accuracy order
+	eps_dv: eps for divn  (default: 0.01)
+	eps_cg: eps for CG    (default: 1)
+	tol_cg: tolerence for CG (default: 0.000001)
+	rect:  smoothing radius (ndim*1)
+	verb: verbosity flag
+	
+	OUTPUT
+	dip:  2D slope
+	
 	from .divne import divne
+	'''
 	
 	p0 = 0.0;
 	nj1 = 1;
 	nj2 = 1;
 	dim = 3;
 	
 	n1 = din.shape[0];
 	n2 = din.shape[1];
 	n3 = 1;
 	
 	r1=rect[0]
 	r2=rect[1]
 	r3=rect[2]
-	
-	din=np.float32(din.flatten(order='F'));
-	dip=dipc(din,n1,n2,n3,niter,liter,order,eps_dv,eps_cg,tol_cg,r1,r2,r3,verb);
+
+	if mask is None:
+		din=np.float32(din.flatten(order='F'));
+		hasmask=0
+	else:
+		if din.size != mask.size:
+			Exception("Mask and Data should have the same dimension")
+		else:
+			din=np.float32(np.concatenate([din.flatten(order='F'),mask.flatten(order='F')],axis=0));
+			hasmask=1;
+	dip=dipc(din,n1,n2,n3,niter,liter,order,eps_dv,eps_cg,tol_cg,r1,r2,r3,hasmask,verb);
 	dip=dip.reshape(n1,n2,order='F');
 		
 	return dip
 	
 def conv_allpass(din,dip,order):
-	#conv_allpass: Convolutional operator implemented by an allpass filter
-	#
-	#Linearized inverse problem
-	#C'(\sigma)d\Delta \sigma =  C(\sigma)d
-	#
-	#IPNUT:
-	#din: input data
-	#dip: 3D dip
-	#order: accuracy order
-	#
-	#OUTPUT:
-	#u1: C'(\sigma)d (denominator)
-	#u2: C(\sigma)d  (numerator)
-	#
+	'''
+	conv_allpass: Convolutional operator implemented by an allpass filter
+	
+	Linearized inverse problem
+	C'(\sigma)d\Delta \sigma =  C(\sigma)d
 	
+	IPNUT:
+	din: input data
+	dip: 3D dip
+	order: accuracy order
+	
+	OUTPUT:
+	u1: C'(\sigma)d (denominator)
+	u2: C(\sigma)d  (numerator)
+	
+	'''
 	[n1,n2]=din.shape;
 	u1=np.zeros([n1,n2]);
 	u2=np.zeros([n1,n2]);
 
 	if order==1:
 		nw=1;
 	else:
@@ -127,52 +144,56 @@
 				u2[i1,i2]=u2[i1,i2]+(din[i1+iw,i2+1]-din[i1-iw,i2])*filt2[iw+nw];
 
 	return u1,u2
 
 #cprresponding to eqs.13-16
 #form the filters
 def B3(sigma):
-	#B3 coefficient
-	#sigma: slope
-
+	'''
+	B3 coefficient
+	sigma: slope
+	'''
 	b3=np.zeros[2];
 	b3[0]=(1-sigma)*(2-sigma)/12;
 	b3[1]=(2+sigma)*(2-sigma)/6;
 	b3[2]=(1+sigma)*(2+sigma)/12;
 	
 	return b3
 
 def B3d(sigma):
-	#B3 coefficient derivative
-	#sigma: slope
-
+	'''
+	B3 coefficient derivative
+	sigma: slope
+	'''
 	b3d=np.zeros[2];
 	b3d[0]=-(2-sigma)/12-(1-sigma)/12;
 	b3d[1]=(2-sigma)/6-(2+sigma)/6;
 	b3d[2]=(2+sigma)/12+(1+sigma)/12;
 
 	return b3d
 
 def B5(sigma):
-	#B5 coefficient
-	#sigma: slope
-
+	'''
+	B5 coefficient
+	sigma: slope
+	'''
 	b5=np.zeros(5);
 	b5[0]=(1-sigma)*(2-sigma)*(3-sigma)*(4-sigma)/1680;
 	b5[1]=(4-sigma)*(2-sigma)*(3-sigma)*(4+sigma)/420;
 	b5[2]=(4-sigma)*(3-sigma)*(3+sigma)*(4+sigma)/280;
 	b5[3]=(4-sigma)*(2+sigma)*(3+sigma)*(4+sigma)/420;
 	b5[4]=(1+sigma)*(2+sigma)*(3+sigma)*(4+sigma)/1680;
 
 	return b5
 
 def B5d(sigma):
-	#B5 coefficient derivative
-	#sigma: slope
-
+	'''
+	B5 coefficient derivative
+	sigma: slope
+	'''
 	b5d=np.zeros(5);
 	b5d[0]=-(2-sigma)*(3-sigma)*(4-sigma)/1680-\
 	(1-sigma)*(3-sigma)*(4-sigma)/1680-\
 	(1-sigma)*(2-sigma)*(4-sigma)/1680-\
 	(1-sigma)*(2-sigma)*(3-sigma)/1680;
 
 	b5d[1]=-(2-sigma)*(3-sigma)*(4+sigma)/420-\
```

### Comparing `pyseistr-0.0.4.2/pyseistr/dip3d.py` & `pyseistr-0.0.4.3/pyseistr/dip3d.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 import numpy as np
 from dipcfun import *
 
 def dip3d(din,niter=5,liter=10,order=2,eps_dv=0.01, eps_cg=1, tol_cg=0.000001,rect=[5,5,5],verb=1):
-	#dip3d: 3D dip estimation based on shaping regularized PWD algorithm
-	#(independent implementation)
-	#
-	#Ported to Python by Yangkang Chen, 2022, verified to be exactly the same as the Matlab version
-	#
-	#INPUT
-	#din: input data (nt*nx)
-	#niter: number of nonlinear iterations
-	#liter: number of linear iterations (in divn)
-	#order: accuracy order
-	#eps_dv: eps for divn  (default: 0.01)
-	#eps_cg: eps for CG	(default: 1)
-	#tol_cg: tolerence for CG (default: 0.000001)
-	#rect:  smoothing radius (ndim*1)
-	#verb: verbosity flag
-	#
-	#OUTPUT
-	#dipi:  inline 3D slope
-	#dipx:  xline 3D slope
+	'''
+	dip3d: 3D dip estimation based on shaping regularized PWD algorithm
+	(independent implementation)
+	
+	Ported to Python by Yangkang Chen, 2022, verified to be exactly the same as the Matlab version
+	
+	INPUT
+	din: input data (nt*nx)
+	niter: number of nonlinear iterations
+	liter: number of linear iterations (in divn)
+	order: accuracy order
+	eps_dv: eps for divn  (default: 0.01)
+	eps_cg: eps for CG	(default: 1)
+	tol_cg: tolerence for CG (default: 0.000001)
+	rect:  smoothing radius (ndim*1)
+	verb: verbosity flag
+	
+	OUTPUT
+	dipi:  inline 3D slope
+	dipx:  xline 3D slope
+	
+	NOTE: mask function is not enabled yet (will do in the future)
+	'''
 	from .divne import divne
 	
 	dim = 3;
 	n = np.zeros(dim,dtype='int');
 	n1 = din.shape[0];
 	n2 = din.shape[1];
 	n3 = din.shape[2];
@@ -48,35 +52,37 @@
 		ratio_x  = divne(-u2_x, u1_x, liter, rect, n, eps_dv, eps_cg, tol_cg,verb);
 	
 		dip_i=dip_i+ratio_i;
 		dip_x=dip_x+ratio_x;
 
 	return dip_i,dip_x
 
-def dip3dc(din,niter=5,liter=10,order=2,eps_dv=0.01, eps_cg=1, tol_cg=0.000001,rect=[5,5,5],verb=1,runc=1):
-	#dip3d: 3D dip estimation based on shaping regularized PWD algorithm
-	#(independent implementation)
-	#
-	#Ported to Python by Yangkang Chen, 2022, verified to be exactly the same as the Matlab version
-	#
-	#INPUT
-	#din: input data (nt*nx)
-	#niter: number of nonlinear iterations
-	#liter: number of linear iterations (in divn)
-	#order: accuracy order
-	#eps_dv: eps for divn  (default: 0.01)
-	#eps_cg: eps for CG	(default: 1)
-	#tol_cg: tolerence for CG (default: 0.000001)
-	#rect:  smoothing radius (ndim*1)
-	#verb: verbosity flag
-	#runc: if runc
-	# 
-	#OUTPUT
-	#dipi:  inline 3D slope
-	#dipx:  xline 3D slope
+def dip3dc(din,mask=None,niter=5,liter=10,order=2,eps_dv=0.01, eps_cg=1, tol_cg=0.000001,rect=[5,5,5],verb=1,runc=1):
+	'''
+	dip3dc: 3D dip estimation based on shaping regularized PWD algorithm
+	(C implementation)
+	
+	Ported to Python by Yangkang Chen, 2022, verified to be exactly the same as the Matlab version
+	
+	INPUT
+	din: input data (nt*nx)
+	niter: number of nonlinear iterations
+	liter: number of linear iterations (in divn)
+	order: accuracy order
+	eps_dv: eps for divn  (default: 0.01)
+	eps_cg: eps for CG	(default: 1)
+	tol_cg: tolerence for CG (default: 0.000001)
+	rect:  smoothing radius (ndim*1)
+	verb: verbosity flag
+	runc: if runc
+	 
+	OUTPUT
+	dipi:  inline 3D slope
+	dipx:  xline 3D slope
+	'''
 	from .divne import divne
 	
 	dim = 3;
 	n = np.zeros(dim,dtype='int');
 	n1 = din.shape[0];
 	n2 = din.shape[1];
 	n3 = din.shape[2];
@@ -85,43 +91,52 @@
 	n[2] = n3;
 
 	n123 = din.size;
 
 	r1=rect[0]
 	r2=rect[1]
 	r3=rect[2]
-
 	
-	din=np.float32(din.flatten(order='F'));
-	dip=dipc(din,n1,n2,n3,niter,liter,order,eps_dv,eps_cg,tol_cg,r1,r2,r3,verb);
+	if mask is None:
+		din=np.float32(din.flatten(order='F'));
+		hasmask=0
+	else:
+		if din.size != mask.size:
+			Exception("Mask and Data should have the same dimension")
+		else:
+			din=np.float32(np.concatenate([din.flatten(order='F'),mask.flatten(order='F')],axis=0));
+			hasmask=1;
+	
+	dip=dipc(din,n1,n2,n3,niter,liter,order,eps_dv,eps_cg,tol_cg,r1,r2,r3,hasmask,verb);
 	dip=dip.reshape(n1,n2,n3,2,order='F');
 	
 	dip_i=dip[:,:,:,0]
 	dip_x=dip[:,:,:,1]	
 	
 
 	return dip_i,dip_x
 
 
 def conv_allpass_i(din,dip,order):
-	# conv_allpass_i: Convolutional operator implemented by an allpass filter (iline direction)
-	# 
-	# Linearized inverse problem
-	# C'(\sigma)d\Delta \sigma =  C(\sigma)d
-	# 
-	# IPNUT:
-	# din: input data
-	# dip: 3D dip
-	# order: accuracy order
-	#
-	# OUTPUT:
-	# u1: C'(\sigma)d (denominator)
-	# u2: C(\sigma)d  (numerator)
-	# 
+	'''
+	conv_allpass_i: Convolutional operator implemented by an allpass filter (iline direction)
+	
+	Linearized inverse problem
+	C'(\sigma)d\Delta \sigma =  C(\sigma)d
 	
+	IPNUT:
+	din: input data
+	dip: 3D dip
+	order: accuracy order
+	
+	OUTPUT:
+	u1: C'(\sigma)d (denominator)
+	u2: C(\sigma)d  (numerator)
+	
+	'''
 	[n1,n2,n3]=din.shape;
 	u1=np.zeros([n1,n2,n3]);
 	u2=np.zeros([n1,n2,n3]);
 
 	if order==1:
 		nw=1;
 	else:
@@ -146,28 +161,30 @@
 				for iw in range(-nw,nw+1):
 					u1[i1,i2,i3]=u1[i1,i2,i3]+(din[i1+iw,i2+1,i3]-din[i1-iw,i2,i3])*filt1[iw+nw];
 					u2[i1,i2,i3]=u2[i1,i2,i3]+(din[i1+iw,i2+1,i3]-din[i1-iw,i2,i3])*filt2[iw+nw];
 
 	return u1,u2
 
 def conv_allpass_x(din,dip,order):
-	# conv_allpass_x: Convolutional operator implemented by an allpass filter (xline direction)
-	# 
-	# Linearized inverse problem
-	# C'(\sigma)d\Delta \sigma =  C(\sigma)d
-	# 
-	# IPNUT:
-	# din: input data
-	# dip: 3D dip
-	# order: accuracy order
-	#
-	# OUTPUT:
-	# u1: C'(\sigma)d (denominator)
-	# u2: C(\sigma)d  (numerator)
-	# 
+	'''
+	conv_allpass_x: Convolutional operator implemented by an allpass filter (xline direction)
+	
+	Linearized inverse problem
+	C'(\sigma)d\Delta \sigma =  C(\sigma)d
+	
+	IPNUT:
+	din: input data
+	dip: 3D dip
+	order: accuracy order
+	
+	OUTPUT:
+	u1: C'(\sigma)d (denominator)
+	u2: C(\sigma)d  (numerator)
+	
+	'''
 	
 	[n1,n2,n3]=din.shape;
 	u1=np.zeros([n1,n2,n3]);
 	u2=np.zeros([n1,n2,n3]);
 
 	if order==1:
 		nw=1;
@@ -194,52 +211,56 @@
 					u2[i1,i2,i3]=u2[i1,i2,i3]+(din[i1+iw,i2,i3+1]-din[i1-iw,i2,i3])*filt2[iw+nw];
 	return u1,u2
 
 
 #cprresponding to eqs.13-16
 #form the filters
 def B3(sigma):
-	#B3 coefficient
-	#sigma: slope
-
+	'''
+	B3 coefficient
+	sigma: slope
+	'''
 	b3=np.zeros[2];
 	b3[0]=(1-sigma)*(2-sigma)/12;
 	b3[1]=(2+sigma)*(2-sigma)/6;
 	b3[2]=(1+sigma)*(2+sigma)/12;
 	
 	return b3
 
 def B3d(sigma):
-	#B3 coefficient derivative
-	#sigma: slope
-
+	'''
+	B3 coefficient derivative
+	sigma: slope
+	'''
 	b3d=np.zeros[2];
 	b3d[0]=-(2-sigma)/12-(1-sigma)/12;
 	b3d[1]=(2-sigma)/6-(2+sigma)/6;
 	b3d[2]=(2+sigma)/12+(1+sigma)/12;
 
 	return b3d
 
 def B5(sigma):
-	#B5 coefficient
-	#sigma: slope
-
+	'''
+	B5 coefficient
+	sigma: slope
+	'''
 	b5=np.zeros(5);
 	b5[0]=(1-sigma)*(2-sigma)*(3-sigma)*(4-sigma)/1680;
 	b5[1]=(4-sigma)*(2-sigma)*(3-sigma)*(4+sigma)/420;
 	b5[2]=(4-sigma)*(3-sigma)*(3+sigma)*(4+sigma)/280;
 	b5[3]=(4-sigma)*(2+sigma)*(3+sigma)*(4+sigma)/420;
 	b5[4]=(1+sigma)*(2+sigma)*(3+sigma)*(4+sigma)/1680;
 
 	return b5
 
 def B5d(sigma):
-	#B5 coefficient derivative
-	#sigma: slope
-
+	'''
+	B5 coefficient derivative
+	sigma: slope
+	'''
 	b5d=np.zeros(5);
 	b5d[0]=-(2-sigma)*(3-sigma)*(4-sigma)/1680-\
 	(1-sigma)*(3-sigma)*(4-sigma)/1680-\
 	(1-sigma)*(2-sigma)*(4-sigma)/1680-\
 	(1-sigma)*(2-sigma)*(3-sigma)/1680;
 
 	b5d[1]=-(2-sigma)*(3-sigma)*(4+sigma)/420-\
```

### Comparing `pyseistr-0.0.4.2/pyseistr/divne.py` & `pyseistr-0.0.4.3/pyseistr/divne.py`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.2/pyseistr/fk.py` & `pyseistr-0.0.4.3/pyseistr/fk.py`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.2/pyseistr/mf.py` & `pyseistr-0.0.4.3/pyseistr/mf.py`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.2/pyseistr/operators.py` & `pyseistr-0.0.4.3/pyseistr/operators.py`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.2/pyseistr/plot.py` & `pyseistr-0.0.4.3/pyseistr/plot.py`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.2/pyseistr/pwspray2d.py` & `pyseistr-0.0.4.3/pyseistr/pwspray2d.py`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.2/pyseistr/pwspray3d.py` & `pyseistr-0.0.4.3/pyseistr/pwspray3d.py`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.2/pyseistr/ricker.py` & `pyseistr-0.0.4.3/pyseistr/ricker.py`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.2/pyseistr/soint3d.py` & `pyseistr-0.0.4.3/pyseistr/soint3d.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from soint3dcfun import *
 
 def soint3d(din,mask,dipi,dipx,order=1,niter=100,njs=[1,1],drift=0,verb=1):
-	# soint3d: 3D structure-oriented interpolation
-	# 
-	# by Yangkang Chen, 2022
-	#
-	# INPUT:
-	# dn: model  noisy data
-	# dipi: inline slope
-	# dipx: xline slope
-	# r1,r2:    spray radius
-	# order:    PWD order
-	# eps: regularization (default:0.01);
-	# 
-	# OUTPUT:
-	# ds: filtered data 
-	#
-	# Demo
-	# demos/test_xxx_soint3d.py
+	'''
+	soint3d: 3D structure-oriented interpolation
+	
+	by Yangkang Chen, 2022
 	
+	INPUT:
+	dn: model  noisy data
+	dipi: inline slope
+	dipx: xline slope
+	order:    PWD order
+	
+	OUTPUT:
+	dout: filtered data 
+
+	Demo
+	demos/test_xxx_soint3d.py
+	'''
 	from .solvers import solver
 	from .solvers import cgstep
 	from .operators import allpass3_lop
 	import numpy as np
 	
 	nw=order;
 	nj1=njs[0];
@@ -60,32 +59,34 @@
 	
 	dout=mm2.reshape(n1,n2,n3,order='F');
 
 	return dout
 	
 	
 def soint3dc(din,mask,dipi,dipx,order=1,niter=100,njs=[1,1],drift=0,seed=202223,hasmask=1,var=0,verb=1):
+	'''
 	# soint3d: 3D structure-oriented interpolation
 	# 
 	# by Yangkang Chen, 2022
 	#
 	# INPUT:
 	# dn: model  noisy data
 	# dipi: inline slope
 	# dipx: xline slope
 	# r1,r2:    spray radius
 	# order:    PWD order
 	# eps: regularization (default:0.01);
 	# hasmask: if 1, using the provided mask; if 0, using the data itself to determine
 	# 
 	# OUTPUT:
-	# ds: filtered data 
+	# dout: filtered data 
 	#
 	# Demo
 	# demos/test_xxx_soint3d.py
+	'''
 	
 	from .solvers import solver
 	from .solvers import cgstep
 	from .operators import allpass3_lop
 	import numpy as np
 	
 	nw=order;
```

### Comparing `pyseistr-0.0.4.2/pyseistr/solvers.py` & `pyseistr-0.0.4.3/pyseistr/solvers.py`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.2/pyseistr/somean2d.py` & `pyseistr-0.0.4.3/pyseistr/somean2d.py`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.2/pyseistr/somean3d.py` & `pyseistr-0.0.4.3/pyseistr/somean3d.py`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.2/pyseistr/somf2d.py` & `pyseistr-0.0.4.3/pyseistr/somf2d.py`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.2/pyseistr/somf3d.py` & `pyseistr-0.0.4.3/pyseistr/somf3d.py`

 * *Files identical despite different names*

### Comparing `pyseistr-0.0.4.2/pyseistr/src/bp_cfuns.c` & `pyseistr-0.0.4.3/pyseistr/src/bp_cfuns.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #include <Python.h>
 #include <math.h>
 #include <stdlib.h>
 #include <stdbool.h>
 #include <stdio.h>
 #include <numpy/arrayobject.h>
-// #include <float.h>
 
 /*NOTE: PS indicates PySeistr*/
 #define PS_NINT(x) ((int)((x)>0.0?(x)+0.5:(x)-0.5))
 #define PS_MAX_DIM 9
 #define PS_PI (3.14159265358979323846264338328)
 
 #define SF_MAX(a,b) ((a) < (b) ? (b) : (a))
```

### Comparing `pyseistr-0.0.4.2/pyseistr/src/dip_cfuns.c` & `pyseistr-0.0.4.3/pyseistr/src/dip_cfuns.c`

 * *Files 1% similar despite different names*

```diff
@@ -1692,31 +1692,31 @@
 
 
 static PyObject *dipc(PyObject *self, PyObject *args){
 	
     /*Below is the input part*/
     int f2,f3,f4,f5,f6,f7;
     float f8,f9,f10;
-    int f11,f12,f13,f14;
+    int f11,f12,f13,f14,f15;
     
 	/**initialize data input**/
     int nd, nd2;
     
     PyObject *f1=NULL;
     PyObject *arrf1=NULL;
 
     
-	PyArg_ParseTuple(args, "Oiiiiiifffiiii", &f1, &f2, &f3, &f4, &f5, &f6, &f7, &f8, &f9, &f10, &f11, &f12, &f13, &f14); 	
+	PyArg_ParseTuple(args, "Oiiiiiifffiiiii", &f1, &f2, &f3, &f4, &f5, &f6, &f7, &f8, &f9, &f10, &f11, &f12, &f13, &f14, &f15); 	
     
     int n123, niter, order, nj1,nj2, i,j, liter, dim;
     int n[PS_MAX_DIM], rect[3], n4, nr, ir; 
-    float p0, q0, *u, *p, *pi=NULL, *qi=NULL;
+    float p0, q0, *u, *um, *p, *pi=NULL, *qi=NULL;
     float pmin, pmax, qmin, qmax, eps;
     char key[4];
-    bool verb, both, **mm, drift;
+    bool verb, both, **mm, drift, hasmask;
 
     dim=4;
     if (dim < 2) n[1]=1;
     if (dim < 3) n[2]=1;
     n123 = n[0]*n[1]*n[2];
     nr = 1;
     for (j=3; j < dim; j++) {
@@ -1771,55 +1771,55 @@
     /* in-line antialiasing */
     nj2=1;
     /* cross-line antialiasing */
     drift=false;
     /* if shift filter */
     verb = false;
     /* verbosity flag */
-//    pmin = -FLT_MAX;
+    
     /* minimum inline dip */
-//     pmax = +FLT_MAX;
     /* maximum inline dip */
-//     qmin = -FLT_MAX;
     /* minimum cross-line dip */
-//     qmax = +FLT_MAX;
     /* maximum cross-line dip */
-
-pmin=-340282346638528859811704183484516925440.000000;
-pmax=340282346638528859811704183484516925440.000000;
-qmin=-340282346638528859811704183484516925440.000000;
-qmax=340282346638528859811704183484516925440.000000;
-/*printf("pmin pmax qmin qmax=%f,%f,%f,%f\n",pmin,pmax,qmin,qmax);*/
+	pmin=-340282346638528859811704183484516925440.000000;
+	pmax=340282346638528859811704183484516925440.000000;
+	qmin=-340282346638528859811704183484516925440.000000;
+	qmax=340282346638528859811704183484516925440.000000;
+	/*printf("pmin pmax qmin qmax=%f,%f,%f,%f\n",pmin,pmax,qmin,qmax);*/
 
 	n[0]=f2;
 	n[1]=f3;
 	n[2]=f4;
 	n123=n[0]*n[1]*n[2];
 	niter=f5;
 	liter=f6;
 	order=f7;
 	eps=f8;
 	
     rect[0]=f11;
     rect[1]=f12;
     rect[2]=f13;
-	verb=f14;
-	verb=true;
+	hasmask=f14;
+	verb=f15;
+// 	verb=true;
+	
     arrf1 = PyArray_FROM_OTF(f1, NPY_FLOAT, NPY_IN_ARRAY);
     
     nd2=PyArray_NDIM(arrf1);
     npy_intp *sp=PyArray_SHAPE(arrf1);
 
 	
-    if (*sp != n123)
-    {
-    	printf("Dimension mismatch, N_input = %d, N_data = %d\n", *sp, n123);
-    	return NULL;
-    }
-
+	if(hasmask==0)
+    	if (*sp != n123)
+    	{
+    		printf("Dimension mismatch, N_input = %d, N_data = %d\n", *sp, n123);
+    		return NULL;
+    	}
+    printf("rect1=%d,rect2=%d,rect3=%d\n",rect[0],rect[1],rect[2]);
+	printf("both=%d,hasmask=%d,verb=%d\n",both,hasmask,verb);
 	printf("n123=%d\n",n123);
 	printf("eps_dv=%f\n",eps);
 
 
 	if(n[2]==1)
 	{
 	n4=0;
@@ -1827,14 +1827,15 @@
 	}
 	else
 	{
 	n4=2; /*calculate both inline and crossline dips*/
 	p = ps_floatalloc(n123*2);
 	}
     u = ps_floatalloc(n123);
+    um = ps_floatalloc(n123); /*temporary array for mask*/
     
     
     /*reading data*/
     for (i=0; i<n123; i++)
     {
         u[i]=*((float*)PyArray_GETPTR1(arrf1,i));
         p[i]=0;
@@ -1843,22 +1844,22 @@
     }
 
     /* initialize dip estimation */
     dip3_init(n[0], n[1], n[2], rect, liter, eps, verb);
 
 
 
-//     if (NULL != sf_getstring("mask")) {
-// 	mm = ps_boolalloc2(n123,both? 4:2);
+    if (hasmask) {
+	mm = ps_boolalloc2(n123,both? 4:2);
 // 	mask = sf_input("mask");
-//     } else {
+    } else {
 	mm = (bool**) ps_alloc(4,sizeof(bool*));
 	mm[0] = mm[1] = mm[2] = mm[3] = NULL;
 // 	mask = NULL;
-//     }
+    }
 
 //     if (NULL != sf_getstring("idip")) {
 // 	/* initial in-line dip */
 // 	idip0 = sf_input("idip");
 // 	if (both) pi = ps_floatalloc(n123);
 //     } else {
 // 	idip0 = NULL;
@@ -1870,18 +1871,20 @@
 // 	if (both) qi = ps_floatalloc(n123);
 //     } else {
 // 	xdip0 = NULL;
 //     }
 
 	nr=1;
     for (ir=0; ir < nr; ir++) {
-//     	if (NULL != mask) {
+    	if (hasmask) {
 // 	    sf_floatread(u,n123,mask);
-// 	    mask32 (both, order, nj1, nj2, n[0], n[1], n[2], u, mm);
-// 	}
+    	for (i=0; i<n123; i++)
+        	um[i]=*((float*)PyArray_GETPTR1(arrf1,i+n123));
+	    mask32 (both, order, nj1, nj2, n[0], n[1], n[2], um, mm);
+	}
 	
 	if (1 != n4) {
 	    /* initialize t-x dip */
 // 	    if (NULL != idip0) {
 // 		if (both) {
 // // 		    sf_floatread(pi,n123,idip0);
 // 		    for(i=0; i < n123; i++) {
```

### Comparing `pyseistr-0.0.4.2/pyseistr/src/sof3d_cfuns.c` & `pyseistr-0.0.4.3/pyseistr/src/sof3d_cfuns.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #include <Python.h>
 #include <math.h>
 #include <stdlib.h>
 #include <stdbool.h>
 #include <stdio.h>
 #include <numpy/arrayobject.h>
-// #include <float.h>
 
 /*NOTE: PS indicates PySeistr*/
 #define PS_NINT(x) ((int)((x)>0.0?(x)+0.5:(x)-0.5))
 #define PS_MAX_DIM 9
 
 #define SF_MAX(a,b) ((a) < (b) ? (b) : (a))
 #define SF_MIN(a,b) ((a) < (b) ? (a) : (b))
```

### Comparing `pyseistr-0.0.4.2/pyseistr/src/sof_cfuns.c` & `pyseistr-0.0.4.3/pyseistr/src/sof_cfuns.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #include <Python.h>
 #include <math.h>
 #include <stdlib.h>
 #include <stdbool.h>
 #include <stdio.h>
 #include <numpy/arrayobject.h>
-// #include <float.h>
 
 /*NOTE: PS indicates PySeistr*/
 #define PS_NINT(x) ((int)((x)>0.0?(x)+0.5:(x)-0.5))
 #define PS_MAX_DIM 9
 
 #define SF_MAX(a,b) ((a) < (b) ? (b) : (a))
 #define SF_MIN(a,b) ((a) < (b) ? (a) : (b))
```

### Comparing `pyseistr-0.0.4.2/pyseistr/src/soint3d_cfuns.c` & `pyseistr-0.0.4.3/pyseistr/src/soint3d_cfuns.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 #include <Python.h>
 #include <math.h>
 #include <stdlib.h>
 #include <stdbool.h>
 #include <stdio.h>
 #include <numpy/arrayobject.h>
-// #include <float.h>
 
 
 /*NOTE: PS indicates PySeistr*/
 #define PS_NINT(x) ((int)((x)>0.0?(x)+0.5:(x)-0.5))
 #define PS_MAX_DIM 9
 #define PS_PI (3.14159265358979323846264338328)
 
 
-#define SF_MAX(a,b) ((a) < (b) ? (b) : (a))
-#define SF_MIN(a,b) ((a) < (b) ? (a) : (b))
-#define SF_ABS(a)   ((a) >= 0  ? (a) : (-(a)))
+#define PS_MAX(a,b) ((a) < (b) ? (b) : (a))
+#define PS_MIN(a,b) ((a) < (b) ? (a) : (b))
+#define PS_ABS(a)   ((a) >= 0  ? (a) : (-(a)))
 
 /*sf functions*/
 typedef void (*operator)(bool,bool,int,int,float*,float*);
 
 void ps_adjnull (bool adj /* adjoint flag */, 
 		 bool add /* addition flag */, 
 		 int nx   /* size of x */, 
@@ -865,19 +864,19 @@
 	free (S);
 	free (Ss);
 	Allocated = false;
     }
 }
 
 static const float TOLERANCE=1.e-12;
-typedef void (*sf_operator)(bool,bool,int,int,float*,float*);
+typedef void (*ps_operator)(bool,bool,int,int,float*,float*);
 typedef void (*ps_solverstep)(bool,int,int,float*,
 			   const float*,float*,const float*);
-typedef void (*sf_weight)(int,const float*,float*);
-void ps_solver (sf_operator oper   /* linear operator */, 
+typedef void (*ps_weight)(int,const float*,float*);
+void ps_solver (ps_operator oper   /* linear operator */, 
 		ps_solverstep solv /* stepping function */, 
 		int nx             /* size of x */, 
 		int ny             /* size of dat */, 
 		float* x           /* estimated model */, 
 		const float* dat   /* data */, 
 		int niter          /* number of iterations */, 
 		...                /* variable number of arguments */)
@@ -890,17 +889,17 @@
   Example: 
   ---
   ps_solver (oper_lop,ps_cgstep,nx,ny,x,y,100,"x0",x0,"end");
   ---
   Parameters in ...:
   ---
   "wt":     float*:         weight      
-  "wght":   sf_weight wght: weighting function
+  "wght":   ps_weight wght: weighting function
   "x0":     float*:         initial model
-  "nloper": sf_operator:    nonlinear operator
+  "nloper": ps_operator:    nonlinear operator
   "mwt":    float*:         model weight
   "verb":   bool:           verbosity flag
   "known":  bool*:          known model mask
   "nmem":   int:            iteration memory
   "nfreq":  int:            periodic restart
   "xmov":   float**:        model iteration
   "rmov":   float**:        residual iteration
@@ -908,17 +907,17 @@
   "res":    float*:         final residual
   >*/ 
 {
 
     va_list args;
     char* par;
     float* wt = NULL;
-    sf_weight wght = NULL;
+    ps_weight wght = NULL;
     float* x0 = NULL;
-    sf_operator nloper = NULL;
+    ps_operator nloper = NULL;
     float* mwt = NULL;
     bool verb = false;
     bool* known = NULL;
     int nmem = -1;
     int nfreq = 0;
     float** xmov = NULL;
     float** rmov = NULL;
@@ -933,19 +932,19 @@
     va_start (args, niter);
     for (;;) {
 	par = va_arg (args, char *);
 	if      (0 == strcmp (par,"end")) {break;}
 	else if (0 == strcmp (par,"wt"))      
 	{                    wt = va_arg (args, float*);}
 	else if (0 == strcmp (par,"wght"))      
-	{                    wght = va_arg (args, sf_weight);}
+	{                    wght = va_arg (args, ps_weight);}
 	else if (0 == strcmp (par,"x0"))      
 	{                    x0 = va_arg (args, float*);}
 	else if (0 == strcmp (par,"nloper"))      
-	{                    nloper = va_arg (args, sf_operator);}
+	{                    nloper = va_arg (args, ps_operator);}
 	else if (0 == strcmp (par,"mwt"))      
 	{                    mwt = va_arg (args, float*);}
 	else if (0 == strcmp (par,"verb"))      
 	{                    verb = (bool) va_arg (args, int);}    
 	else if (0 == strcmp (par,"known"))      
 	{                    known = va_arg (args, bool*);}  
 	else if (0 == strcmp (par,"nmem"))      
@@ -1227,15 +1226,15 @@
     return genrand_int32()*(1.0/4294967295.0); 
     /* divided by 2^32-1 */ 
 }
 
 static bool   iset = true;
 static float  vset = 0.0;
 
-float sf_randn_one_bm (void)
+float ps_randn_one_bm (void)
 /*< return a random number (normally distributed, Box-Muller method) >*/
 {
     double x1, x2, y1, y2, z1, z2;
     
     if (iset) {
 	do {
 	    x1 = genrand_real1 ();
@@ -1337,15 +1336,15 @@
 	} else {
 	    for (i=0; i < n123; i++) {
 		known[i] = (bool) (mm[i] != 0.);
 	    }
 	}
 	
 	for (i=0; i < 2*n123; i++) {
-	    dd[i] = a*sf_randn_one_bm();
+	    dd[i] = a*ps_randn_one_bm();
 	}
 	
 	ps_solver(allpass3_lop, ps_cgstep, n123, 2*n123, mm, dd, niter,
 		  "known", known, "x0", mm, "verb", verb, "end");
 	ps_cgstep_close();
```

### Comparing `pyseistr-0.0.4.2/pyseistr.egg-info/PKG-INFO` & `pyseistr-0.0.4.3/pyseistr.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pyseistr
-Version: 0.0.4.2
+Version: 0.0.4.3
 Summary: A python package for structural denoising and interpolation of multi-channel seismic data
 Home-page: https://github.com/aaspip/pyseistr
 Author: pyseistr developing team
 Author-email: chenyk2016@gmail.com
 License: GNU General Public License, Version 3 (GPLv3)
-Description: Source code: https://github.com/aaspip/pyseistr
 Keywords: seismology,earthquake seismology,exploration seismology,array seismology,denoising,science,engineering,structure,local slope,filtering
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Provides-Extra: docs
+License-File: LICENSE
+
+Source code: https://github.com/aaspip/pyseistr
```

### Comparing `pyseistr-0.0.4.2/pyseistr.egg-info/SOURCES.txt` & `pyseistr-0.0.4.3/pyseistr.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+LICENSE
 README.md
 setup.py
 pyseistr/__init__.py
 pyseistr/bp.py
 pyseistr/dip2d.py
 pyseistr/dip3d.py
 pyseistr/divne.py
 pyseistr/fk.py
 pyseistr/mf.py
 pyseistr/operators.py
 pyseistr/plot.py
 pyseistr/pwspray2d.py
 pyseistr/pwspray3d.py
 pyseistr/ricker.py
+pyseistr/soint2d.py
 pyseistr/soint3d.py
 pyseistr/solvers.py
 pyseistr/somean2d.py
 pyseistr/somean3d.py
 pyseistr/somf2d.py
 pyseistr/somf3d.py
 pyseistr.egg-info/PKG-INFO
@@ -24,8 +26,9 @@
 pyseistr.egg-info/not-zip-safe
 pyseistr.egg-info/requires.txt
 pyseistr.egg-info/top_level.txt
 pyseistr/src/bp_cfuns.c
 pyseistr/src/dip_cfuns.c
 pyseistr/src/sof3d_cfuns.c
 pyseistr/src/sof_cfuns.c
+pyseistr/src/soint2d_cfuns.c
 pyseistr/src/soint3d_cfuns.c
```

### Comparing `pyseistr-0.0.4.2/setup.py` & `pyseistr-0.0.4.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 #!/usr/bin/env python
 # -*- encoding: utf8 -*-
-import glob
-import inspect
 import io
 import os
 
-from setuptools import find_packages
 from setuptools import setup
+from distutils.core import Extension
+import numpy
 
 
 long_description = """
 Source code: https://github.com/aaspip/pyseistr""".strip() 
 
 
 def read(*names, **kwargs):
     return io.open(
         os.path.join(os.path.dirname(__file__), *names),
         encoding=kwargs.get("encoding", "utf8")).read()
 
-from distutils.core import Extension
-
-dipc_module = Extension('dipcfun', sources=['pyseistr/src/dip_cfuns.c'])
-sofc_module = Extension('sofcfun', sources=['pyseistr/src/sof_cfuns.c'])
-sofc3d_module = Extension('sof3dcfun', sources=['pyseistr/src/sof3d_cfuns.c'])
-sointc3d_module = Extension('soint3dcfun', sources=['pyseistr/src/soint3d_cfuns.c'])
-bpc_module = Extension('bpcfun', sources=['pyseistr/src/bp_cfuns.c'])
-
-from numpy.distutils.core import setup 
+dipc_module = Extension('dipcfun', sources=['pyseistr/src/dip_cfuns.c'], 
+										include_dirs=[numpy.get_include()])
+sofc_module = Extension('sofcfun', sources=['pyseistr/src/sof_cfuns.c'], 
+										include_dirs=[numpy.get_include()])
+sofc3d_module = Extension('sof3dcfun', sources=['pyseistr/src/sof3d_cfuns.c'], 
+										include_dirs=[numpy.get_include()])
+sointc3d_module = Extension('soint3dcfun', sources=['pyseistr/src/soint3d_cfuns.c'], 
+										include_dirs=[numpy.get_include()])
+sointc2d_module = Extension('soint2dcfun', sources=['pyseistr/src/soint2d_cfuns.c'], 
+										include_dirs=[numpy.get_include()])
+bpc_module = Extension('bpcfun', sources=['pyseistr/src/bp_cfuns.c'], 
+										include_dirs=[numpy.get_include()])
 
 setup(
     name="pyseistr",
-    version="0.0.4.2",
+    version="0.0.4.3",
     license='GNU General Public License, Version 3 (GPLv3)',
     description="A python package for structural denoising and interpolation of multi-channel seismic data",
     long_description=long_description,
     author="pyseistr developing team",
     author_email="chenyk2016@gmail.com",
     url="https://github.com/aaspip/pyseistr",
-    ext_modules=[dipc_module,sofc_module,sofc3d_module,sointc3d_module,bpc_module],
+    ext_modules=[dipc_module,sofc_module,sofc3d_module,sointc2d_module,sointc3d_module,bpc_module],
     packages=['pyseistr'],
     include_package_data=True,
     zip_safe=False,
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
```


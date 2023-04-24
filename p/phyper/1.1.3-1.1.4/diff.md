# Comparing `tmp/phyper-1.1.3-py3-none-any.whl.zip` & `tmp/phyper-1.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 29225 bytes, number of entries: 15
--rw-r--r--  2.0 unx      685 b- defN 23-Apr-20 10:38 phyper/__init__.py
--rw-r--r--  2.0 unx      292 b- defN 23-Apr-20 12:42 phyper/chemometrics/__init__.py
--rw-r--r--  2.0 unx     9505 b- defN 23-Apr-20 13:00 phyper/chemometrics/_gui.py
--rw-r--r--  2.0 unx    13252 b- defN 23-Apr-20 10:38 phyper/chemometrics/analysis.py
--rw-r--r--  2.0 unx    50208 b- defN 23-Apr-20 14:26 phyper/chemometrics/dataset.py
--rw-r--r--  2.0 unx     2713 b- defN 23-Apr-20 10:38 phyper/chemometrics/preprocessing.py
--rw-r--r--  2.0 unx     2298 b- defN 23-Apr-20 10:38 phyper/chemometrics/sampling.py
--rw-r--r--  2.0 unx      121 b- defN 23-Apr-20 10:38 phyper/lab/__init__.py
--rw-r--r--  2.0 unx      802 b- defN 23-Apr-20 10:38 phyper/lab/_misc.py
--rw-r--r--  2.0 unx    15275 b- defN 23-Apr-20 13:35 phyper/lab/measurement.py
--rwxrwxrwx  2.0 unx     1075 b- defN 23-Apr-20 14:30 phyper-1.1.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     2231 b- defN 23-Apr-20 14:30 phyper-1.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-20 14:30 phyper-1.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Apr-20 14:30 phyper-1.1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1219 b- defN 23-Apr-20 14:30 phyper-1.1.3.dist-info/RECORD
-15 files, 99775 bytes uncompressed, 27215 bytes compressed:  72.7%
+Zip file size: 29358 bytes, number of entries: 15
+-rw-r--r--  2.0 unx      685 b- defN 23-Apr-24 07:40 phyper/__init__.py
+-rw-r--r--  2.0 unx      292 b- defN 23-Apr-24 07:40 phyper/chemometrics/__init__.py
+-rw-r--r--  2.0 unx     9505 b- defN 23-Apr-24 07:40 phyper/chemometrics/_gui.py
+-rw-r--r--  2.0 unx    13252 b- defN 23-Apr-24 07:40 phyper/chemometrics/analysis.py
+-rw-r--r--  2.0 unx    50472 b- defN 23-Apr-24 08:50 phyper/chemometrics/dataset.py
+-rw-r--r--  2.0 unx     2713 b- defN 23-Apr-24 07:40 phyper/chemometrics/preprocessing.py
+-rw-r--r--  2.0 unx     2298 b- defN 23-Apr-24 07:40 phyper/chemometrics/sampling.py
+-rw-r--r--  2.0 unx      121 b- defN 23-Apr-24 07:40 phyper/lab/__init__.py
+-rw-r--r--  2.0 unx      802 b- defN 23-Apr-24 07:40 phyper/lab/_misc.py
+-rw-r--r--  2.0 unx    15275 b- defN 23-Apr-24 07:40 phyper/lab/measurement.py
+-rwxr-xr-x  2.0 unx     1075 b- defN 23-Apr-24 08:53 phyper-1.1.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2268 b- defN 23-Apr-24 08:53 phyper-1.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 08:53 phyper-1.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-24 08:53 phyper-1.1.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1219 b- defN 23-Apr-24 08:53 phyper-1.1.4.dist-info/RECORD
+15 files, 100076 bytes uncompressed, 27348 bytes compressed:  72.7%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: phyper/lab/_misc.py
 Comment: 
 
 Filename: phyper/lab/measurement.py
 Comment: 
 
-Filename: phyper-1.1.3.dist-info/LICENSE
+Filename: phyper-1.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: phyper-1.1.3.dist-info/METADATA
+Filename: phyper-1.1.4.dist-info/METADATA
 Comment: 
 
-Filename: phyper-1.1.3.dist-info/WHEEL
+Filename: phyper-1.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: phyper-1.1.3.dist-info/top_level.txt
+Filename: phyper-1.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: phyper-1.1.3.dist-info/RECORD
+Filename: phyper-1.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## phyper/chemometrics/dataset.py

```diff
@@ -1017,32 +1017,35 @@
             roiHSD = deepcopy(self)
             roiHSD.set_HC(self.get_HC()[round(min_row):round(max_row),round(min_col):round(max_col),:])
             return roiHSD
         else:
             print('ROI does not agree with hypercube dimensions ({0},{1})'.format(self.get_dimY(),self.get_dimX()))
             return None
 
-    def get_rgb(self, preprocessed=False, labeloverlay=True, raw=False, channels=[]):
+    def get_rgb(self, preprocessed=False, labeloverlay=True, channels=[]):
         
         if not channels:
             try:
+                # see if possible to reconstructon 'real' RGB image
                 red_idx = self.get_wl_idx(570)
                 green_idx = self.get_wl_idx(540)
                 blue_idx = self.get_wl_idx(500)
             except:
-                red_idx = self.get_wl_idx(1100)
-                green_idx = self.get_wl_idx(1300)
-                blue_idx = self.get_wl_idx(1600)
+                # if you can not find these wavelengths, take central and left and right of central. Also works for dimL == 1 or dimL == 2 (not so nice for dimL == 3)
+                dimL = self.get_dimL()
+                green_idx = dimL//2
+                red_idx = green_idx//2
+                blue_idx = red_idx + green_idx
         else:
             red_idx, green_idx, blue_idx = [self.get_wl_idx(wl) for wl in channels]
 
         reflectance_im = self.get_HC(preprocessed=preprocessed)[:, :, [red_idx, green_idx, blue_idx]]
 
         #scale raw images to max bit value
-        if raw:
+        if np.amax(reflectance_im) > 100:
             #TODO: make valid for all kinds of bit depth images. Mabye store type
             reflectance_im = reflectance_im/(2**12-1)
         
         #convert to 8bit RGB
         reflectance_im = np.clip(reflectance_im, 0, 1)
 
         im = np.multiply(reflectance_im, 255).astype(np.uint8)
```

## Comparing `phyper-1.1.3.dist-info/LICENSE` & `phyper-1.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `phyper-1.1.3.dist-info/METADATA` & `phyper-1.1.4.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: phyper
-Version: 1.1.3
+Version: 1.1.4
 Summary: Package for managing (hyper)spectral datasets
 Home-page: https://gitlab.kuleuven.be/u0123403/pyper
 Author: Remi Van Belleghem
 Author-email: remi.vanbelleghem@kuleuven.be
 Maintainer: MeBios - KULeuven
 Maintainer-email: wouter.saeys@kuleuven.be
+License: UNKNOWN
 Keywords: hyperspectral,chemometrics
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6,<4.0
 Description-Content-Type: text/markdown
@@ -63,7 +65,9 @@
 2. Use pip to install the package in editable format  
 `pip install -e .`
 
 
 ## Acknowledgements
 
 Written by Remi Van Belleghem. Based on Matlab toolbox from Niels Wouters.
+
+
```

## Comparing `phyper-1.1.3.dist-info/RECORD` & `phyper-1.1.4.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 phyper/__init__.py,sha256=4hYB58cealu01B6FLn3lhRnI0JAPY6Va107e65WXTcs,685
 phyper/chemometrics/__init__.py,sha256=5y7WaXHDvt1RbplvdekletkldO9cMdvYHRFzJkE1ziE,292
 phyper/chemometrics/_gui.py,sha256=3h4jW2pVt-14QTx3g-wFnMzaQTq8SZC2BBabRBZ9bpA,9505
 phyper/chemometrics/analysis.py,sha256=903ZGNPjkmJL_z0CeeorcQkoiCMZLeOYK3_q18CmBnc,13252
-phyper/chemometrics/dataset.py,sha256=usVvonWQZXK6gdy0jNdjdiTRRJ_tgM2u3IaQbocnjKM,50208
+phyper/chemometrics/dataset.py,sha256=2CEeXG647iTQ2mJ2Nm7CmMX_Mfskv1zd1_TRiemc6k8,50472
 phyper/chemometrics/preprocessing.py,sha256=lKoB64-a4IdM82pC1OAh9cCy-LXKLOcFbygVYnQCBcM,2713
 phyper/chemometrics/sampling.py,sha256=H-xl0PrAwRoaxwah8DqVSlRJ1gPl9Qm806Zh7MPuu2U,2298
 phyper/lab/__init__.py,sha256=p1f53MLglxawnDhRGT4O1NI5CpL2Rvski2XEyg9ErM8,121
 phyper/lab/_misc.py,sha256=irgAaObHkaIBESTdw-o0e0Eb-z2pUm9Kdc9ujZq8pg8,802
 phyper/lab/measurement.py,sha256=YCQX5YkgWDmwesoELt14JgdWcVYc2vq8cqnjIbxHfSM,15275
-phyper-1.1.3.dist-info/LICENSE,sha256=i-l_fDhG098wzA_kHlskLIwp3UKEjHzNP1PVuIu2wuQ,1075
-phyper-1.1.3.dist-info/METADATA,sha256=wtwBal0wXrDPj4jr4I6gUC453-KX9aA2Ss0K6_wHX8E,2231
-phyper-1.1.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-phyper-1.1.3.dist-info/top_level.txt,sha256=1CRpBqxQW0H4uxZ6GzjiIKUq4FJksW5pai8komowTII,7
-phyper-1.1.3.dist-info/RECORD,,
+phyper-1.1.4.dist-info/LICENSE,sha256=i-l_fDhG098wzA_kHlskLIwp3UKEjHzNP1PVuIu2wuQ,1075
+phyper-1.1.4.dist-info/METADATA,sha256=wvHjdJbz2V34HioyH1uUCpwAjPu9S4K2Hzerhf-HKSc,2268
+phyper-1.1.4.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+phyper-1.1.4.dist-info/top_level.txt,sha256=1CRpBqxQW0H4uxZ6GzjiIKUq4FJksW5pai8komowTII,7
+phyper-1.1.4.dist-info/RECORD,,
```


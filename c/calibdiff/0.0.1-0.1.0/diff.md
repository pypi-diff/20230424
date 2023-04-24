# Comparing `tmp/calibdiff-0.0.1.tar.gz` & `tmp/calibdiff-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/calibdiff-0.0.1.tar", last modified: Sun Apr 16 15:49:46 2023, max compression
+gzip compressed data, was "dist/calibdiff-0.1.0.tar", last modified: Mon Apr 24 11:07:33 2023, max compression
```

## Comparing `calibdiff-0.0.1.tar` & `calibdiff-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-04-16 15:49:46.000000 calibdiff-0.0.1/
--rw-rw-r--   0 dl        (1000) dl        (1000)       35 2023-04-10 08:40:35.000000 calibdiff-0.0.1/MANIFEST.in
--rw-rw-r--   0 dl        (1000) dl        (1000)      687 2023-04-16 15:49:46.000000 calibdiff-0.0.1/PKG-INFO
--rw-rw-r--   0 dl        (1000) dl        (1000)      861 2023-04-16 14:40:41.000000 calibdiff-0.0.1/README.md
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-04-16 15:49:46.000000 calibdiff-0.0.1/calibdiff/
--rw-rw-r--   0 dl        (1000) dl        (1000)      661 2023-04-16 14:36:21.000000 calibdiff-0.0.1/calibdiff/__info__.py
--rw-rw-r--   0 dl        (1000) dl        (1000)      170 2023-04-13 11:48:03.000000 calibdiff-0.0.1/calibdiff/__init__.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     1476 2023-04-14 08:01:00.000000 calibdiff-0.0.1/calibdiff/apply_rectify_on_uv.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     6628 2023-04-14 08:53:03.000000 calibdiff-0.0.1/calibdiff/calibdiff_utils.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     5812 2023-04-14 08:22:04.000000 calibdiff-0.0.1/calibdiff/feature_matching.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     2689 2023-04-14 05:14:41.000000 calibdiff-0.0.1/calibdiff/rt_to_rectify.py
--rw-rw-r--   0 dl        (1000) dl        (1000)     6080 2023-04-16 15:47:32.000000 calibdiff-0.0.1/calibdiff/stereo_optimize.py
-drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-04-16 15:49:46.000000 calibdiff-0.0.1/calibdiff.egg-info/
--rw-rw-r--   0 dl        (1000) dl        (1000)      687 2023-04-16 15:49:45.000000 calibdiff-0.0.1/calibdiff.egg-info/PKG-INFO
--rw-rw-r--   0 dl        (1000) dl        (1000)      403 2023-04-16 15:49:45.000000 calibdiff-0.0.1/calibdiff.egg-info/SOURCES.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)        1 2023-04-16 15:49:45.000000 calibdiff-0.0.1/calibdiff.egg-info/dependency_links.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       26 2023-04-16 15:49:45.000000 calibdiff-0.0.1/calibdiff.egg-info/requires.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       10 2023-04-16 15:49:45.000000 calibdiff-0.0.1/calibdiff.egg-info/top_level.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       26 2023-04-16 15:30:04.000000 calibdiff-0.0.1/requirements.txt
--rw-rw-r--   0 dl        (1000) dl        (1000)       38 2023-04-16 15:49:46.000000 calibdiff-0.0.1/setup.cfg
--rw-rw-r--   0 dl        (1000) dl        (1000)      957 2023-04-10 08:42:07.000000 calibdiff-0.0.1/setup.py
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-04-24 11:07:33.000000 calibdiff-0.1.0/
+-rw-rw-r--   0 dl        (1000) dl        (1000)       35 2023-04-10 08:40:35.000000 calibdiff-0.1.0/MANIFEST.in
+-rw-rw-r--   0 dl        (1000) dl        (1000)      687 2023-04-24 11:07:33.000000 calibdiff-0.1.0/PKG-INFO
+-rw-rw-r--   0 dl        (1000) dl        (1000)      861 2023-04-16 14:40:41.000000 calibdiff-0.1.0/README.md
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-04-24 11:07:33.000000 calibdiff-0.1.0/calibdiff/
+-rw-rw-r--   0 dl        (1000) dl        (1000)      661 2023-04-24 11:01:05.000000 calibdiff-0.1.0/calibdiff/__info__.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)      170 2023-04-13 11:48:03.000000 calibdiff-0.1.0/calibdiff/__init__.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     1476 2023-04-14 08:01:00.000000 calibdiff-0.1.0/calibdiff/apply_rectify_on_uv.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     8456 2023-04-24 11:00:47.000000 calibdiff-0.1.0/calibdiff/calibdiff_utils.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     8241 2023-04-24 11:00:47.000000 calibdiff-0.1.0/calibdiff/feature_matching.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     2689 2023-04-14 05:14:41.000000 calibdiff-0.1.0/calibdiff/rt_to_rectify.py
+-rw-rw-r--   0 dl        (1000) dl        (1000)     7325 2023-04-24 11:05:04.000000 calibdiff-0.1.0/calibdiff/stereo_optimize.py
+drwxrwxr-x   0 dl        (1000) dl        (1000)        0 2023-04-24 11:07:33.000000 calibdiff-0.1.0/calibdiff.egg-info/
+-rw-rw-r--   0 dl        (1000) dl        (1000)      687 2023-04-24 11:07:33.000000 calibdiff-0.1.0/calibdiff.egg-info/PKG-INFO
+-rw-rw-r--   0 dl        (1000) dl        (1000)      403 2023-04-24 11:07:33.000000 calibdiff-0.1.0/calibdiff.egg-info/SOURCES.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)        1 2023-04-24 11:07:33.000000 calibdiff-0.1.0/calibdiff.egg-info/dependency_links.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       26 2023-04-24 11:07:33.000000 calibdiff-0.1.0/calibdiff.egg-info/requires.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       10 2023-04-24 11:07:33.000000 calibdiff-0.1.0/calibdiff.egg-info/top_level.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       26 2023-04-16 15:30:04.000000 calibdiff-0.1.0/requirements.txt
+-rw-rw-r--   0 dl        (1000) dl        (1000)       38 2023-04-24 11:07:33.000000 calibdiff-0.1.0/setup.cfg
+-rw-rw-r--   0 dl        (1000) dl        (1000)      957 2023-04-10 08:42:07.000000 calibdiff-0.1.0/setup.py
```

### Comparing `calibdiff-0.0.1/PKG-INFO` & `calibdiff-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calibdiff
-Version: 0.0.1
+Version: 0.1.0
 Summary: A PyTorch-based differential camera calibration library for intrinsic, extrinsic, and stereo camera calibration.
 Home-page: https://github.com/DIYer22/calibdiff
 Author: DIYer22
 Author-email: ylxx@live.com
 License: UNKNOWN
 Description: A PyTorch-based differential camera calibration library for intrinsic, extrinsic, and stereo camera calibration.
 Platform: UNKNOWN
```

### Comparing `calibdiff-0.0.1/README.md` & `calibdiff-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `calibdiff-0.0.1/calibdiff/__info__.py` & `calibdiff-0.1.0/calibdiff/__info__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.1"
+__version__ = "0.1.0"
 __description__ = "A PyTorch-based differential camera calibration library for intrinsic, extrinsic, and stereo camera calibration."
 __license__ = "MIT"
 __author__ = "DIYer22"
 __author_email__ = "ylxx@live.com"
 __maintainer__ = "DIYer22"
 __maintainer_email__ = "ylxx@live.com"
 __github_username__ = "DIYer22"
```

### Comparing `calibdiff-0.0.1/calibdiff/apply_rectify_on_uv.py` & `calibdiff-0.1.0/calibdiff/apply_rectify_on_uv.py`

 * *Files identical despite different names*

### Comparing `calibdiff-0.0.1/calibdiff/calibdiff_utils.py` & `calibdiff-0.1.0/calibdiff/calibdiff_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,16 +20,28 @@
 
 def rodrigues_pytorch(rvec):
     theta = torch.norm(rvec) + eps
     # if theta == 0:
     #     return torch.eye(3).type_as(rvec)
 
     k = rvec / theta
-    K = torch_tensor([[0, -k[2], k[1]], [k[2], 0, -k[0]], [-k[1], k[0], 0]])
-    # TODO 有梯度吗?
+    K = torch.stack(
+        [
+            torch_tensor(0.0),
+            -k[2],
+            k[1],
+            k[2],
+            torch_tensor(0.0),
+            -k[0],
+            -k[1],
+            k[0],
+            torch_tensor(0.0),
+        ]
+    ).view(3, 3)
+    # K = torch_tensor([[0, -k[2], k[1]], [k[2], 0, -k[0]], [-k[1], k[0], 0]])
 
     R = (
         torch.eye(3).to(device)
         + torch.sin(theta) * K
         + (1 - torch.cos(theta)) * torch.matmul(K, K)
     )
     return R
@@ -164,33 +176,57 @@
     #     d[f'K{i}'] = torch_tensor([[d[f'fx{i}'], 0, d[f'cx{i}']],[0, d[f'fy{i}'], d[f'cy{i}']],[0,0,1]], requires_grad=True)
 
     for i in range(1, 3):
         d[f"K{i}"] = generate_K(d[f"fx{i}"], d[f"cx{i}"], d[f"fy{i}"], d[f"cy{i}"])
     return d
 
 
+def set_rotate_imread_for_test(rotate_substr="stereo_r.jpg", angle=30):
+    def _imread(fname, *l, **kv):
+        import skimage.io
+
+        img = skimage.io.imread(fname, *l, **kv)
+        if rotate_substr in fname:
+            print(fname)
+            img = np.uint8(
+                __import__("skimage.transform").transform.rotate(img, angle=angle)
+                * 255.5
+            )
+        return img
+
+    boxx.imread = _imread
+
+
+def try_load_img(arr_or_path):
+    if isinstance(arr_or_path, str):
+        return boxx.imread(arr_or_path)
+    return arr_or_path
+
+
 """
 pormpt: Write a function to vis points matched in two images
 - uvs1 are normalizd xy(0~1) of points in img1
 - img are RGB format(h,w,3). if img is None, just replace by a 512*512 black img
 - line color between uv1 and uv2 are random Highly saturated colors.
 - if has confidence shape(n,), less confidence more tranparent
 - support img1 and img2 have different shape
 - line thickness are adaptive to img size 
 """
 
 
 def vis_matched_uvs(uvs1, uvs2, img1=None, img2=None, confidence=None):
-    from random import randint
-
+    if uvs1.max() > 1 and uvs2.max() > 1:
+        maxx = max(uvs1.max(), uvs2.max())
+        uvs1 = uvs1 / ([maxx, maxx] if img1 is None else img1.shape[:2][::-1])
+        uvs2 = uvs2 / ([maxx, maxx] if img2 is None else img2.shape[:2][::-1])
     if img1 is None:
-        img1 = np.zeros((512, 512, 3), dtype=np.uint8)
+        img1 = np.zeros((1024, 1024, 3), dtype=np.uint8) + 192
     if img2 is None:
-        img2 = np.zeros((512, 512, 3), dtype=np.uint8)
-
+        img2 = np.zeros((1024, 1024, 3), dtype=np.uint8) + 64
+    img1, img2 = try_load_img(img1), try_load_img(img2)
     h1, w1, _ = img1.shape
     h2, w2, _ = img2.shape
 
     # Resize images to have the same height
     if h1 != h2:
         new_w1 = int(w1 * h2 / h1)
         img1 = cv2.resize(img1, (new_w1, h2))
@@ -203,28 +239,44 @@
 
     if confidence is not None:
         if confidence.ndim == 1:
             confidence = np.expand_dims(confidence, axis=1)
         assert (
             uvs1.shape[0] == confidence.shape[0]
         ), "Confidence values must match the number of points in uvs1"
-    if uvs1.max() > 1 and uvs2.max() > 1:
-        uvs1 = uvs1 / [w1, h1]
-        uvs2 = uvs2 / [w2, h2]
+    # First, draw all lines
+    line_colors = boxx.getDefaultColorList(12, uint8=True) * (len(uvs1) // 10 + 1)
     for i, (uv1, uv2) in enumerate(zip(uvs1, uvs2)):
         x1, y1 = int(uv1[0] * w1), int(uv1[1] * h1)
         x2, y2 = int(uv2[0] * w2) + w1, int(uv2[1] * h2)
 
-        line_color = (randint(0, 255), randint(0, 255), randint(0, 255))
-        line_thickness = max(1, int(min(w1, w2) * 0.0015))
+        line_color = line_colors[i]
+        line_thickness = max(1, int(min(w1, w2) * 0.001))
 
         if confidence is not None:
             alpha = max(0.2, min(1, confidence[i]))
             line_color = tuple(int(c * alpha) for c in line_color)
 
         cv2.line(canvas, (x1, y1), (x2, y2), line_color, thickness=line_thickness)
 
+    # Then, draw all points
+    for i, (uv1, uv2) in enumerate(zip(uvs1, uvs2)):
+        x1, y1 = int(uv1[0] * w1), int(uv1[1] * h1)
+        x2, y2 = int(uv2[0] * w2) + w1, int(uv2[1] * h2)
+
+        line_color = line_colors[i]
+        point_radius = max(1, int(min(w1, w2) * 0.0015))
+
+        if confidence is not None:
+            alpha = max(0.2, min(1, confidence[i]))
+            line_color = tuple(int(c * alpha) for c in line_color)
+
+        cv2.circle(canvas, (x1, y1), point_radius * 2, (255, 255, 255), thickness=-1)
+        cv2.circle(canvas, (x2, y2), point_radius * 2, (255, 255, 255), thickness=-1)
+        cv2.circle(canvas, (x1, y1), point_radius, line_color, thickness=-1)
+        cv2.circle(canvas, (x2, y2), point_radius, line_color, thickness=-1)
+
     return canvas
 
 
 if __name__ == "__main__":
     from boxx import *
```

### Comparing `calibdiff-0.0.1/calibdiff/rt_to_rectify.py` & `calibdiff-0.1.0/calibdiff/rt_to_rectify.py`

 * *Files identical despite different names*

### Comparing `calibdiff-0.0.1/calibdiff/stereo_optimize.py` & `calibdiff-0.1.0/calibdiff/stereo_optimize.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 #!/usr/bin/env python3
 
 import boxx
 import torch
-import torch.optim as optim
-from boxx import npa, np
 import calibrating
+import torch.optim as optim
+from boxx import npa, np, strnum, glob, os
 
 with boxx.inpkg():
     from . import calibdiff_utils
     from . import rt_to_rectify
+    from .calibdiff_utils import eps, device
 
-device = calibdiff_utils.device
+# calibdiff_utils.set_rotate_imread_for_test()
 
 
 class StereoOptimize:
     def __init__(self, stereo, uvs1, uvs2):
         self.stereo = stereo
+        if not all(stereo.t):
+            import warnings
+
+            warnings.warn(
+                f"stereo.t({stereo.t}) has zeros, try to add eps as {self.stereo.t + eps}",
+                UserWarning,
+            )
+            self.stereo.t = self.stereo.t + eps
         self.uv_pairs = torch.from_numpy(np.concatenate([uvs1, uvs2], 1)).to(device)
         self.context = self.stereo_to_context()
 
     def stereo_to_context(self):
         context = {}
         cam1 = self.stereo.cam1
         cam2 = self.stereo.cam2
@@ -64,30 +73,44 @@
             re = rt_to_rectify.stereo_recitfy(R, param["t"])
             uv1_rectifys = calibdiff_utils.apply_rectify_on_uv(
                 self.uv_pairs[:, :2], d["K1"], re["R1"]
             )
             uv2_rectifys = calibdiff_utils.apply_rectify_on_uv(
                 self.uv_pairs[:, 2:], d["K2"], re["R2"]
             )
-            loss_polar_alignment = torch.abs(
-                uv1_rectifys[:, 1] - uv2_rectifys[:, 1]
-            ).mean()
-            loss = loss_polar_alignment / self.stereo.cam1.xy[1]
-            # loss = loss**2
+
+            l1s = torch.abs(uv1_rectifys[:, 1] - uv2_rectifys[:, 1])
+            _, loss_idx = l1s.topk(int(len(l1s) * 0.95), largest=False)
+            retval = l1s.mean()
+
+            lossd = {}
+            lossd["polar_alignment"] = l1s[loss_idx].mean() / self.stereo.cam1.xy[1]
+
+            # lossd['l2'] = (((
+            #     uv1_rectifys[:, 1] - uv2_rectifys[:, 1]
+            # )/(18))**2)[loss_idx].mean()
+
+            target_baseline = self.stereo.baseline
+            lossd["distance"] = (
+                (target_baseline - (param["t"] ** 2 + eps).sum() ** 0.5)
+                / (target_baseline * 1 + eps)
+            ) ** 2
+
+            loss = sum(lossd.values())
             loss.backward()
-            if idx % 100 == 0 and boxx.mg():
+            if idx % 100 == 0 and 1:  # boxx.mg():
                 # print({k: v.grad for k, v in param.items()})
                 print(
-                    f"Iteration {idx}: loss_polar_alignment = {loss_polar_alignment.item()}"
+                    f"Iteration {idx}: retval={strnum(retval.item())}, {', '.join([f'{k}={strnum(lossd[k])}' for k in lossd])}"
                 )
             optimizer.step()
 
         return calibrating.Stereo.load(
             dict(
-                retval=loss_polar_alignment,
+                retval=retval,
                 R=npa - R,
                 t=npa - param["t"],
                 cam1=dict(
                     fx=param["fx1"],
                     cx=param["cx1"],
                     fy=param["fy1"],
                     cy=param["cy1"],
@@ -154,24 +177,24 @@
 """
     )
     # stereo.R = cv2.Rodrigues(boxx.npa-[0.17]*3)[0]
     return caml, camr, stereo
 
 
 if __name__ == "__main__":
-    from boxx import glob, os
-
     with boxx.inpkg():
         from .feature_matching import (
             LoftrFeatureMatching,
             get_uv_pairs_from_stereo_boards,
         )
         from boxx import *
 
-    caml, camr, camd = calibrating.get_test_cams().values()
+    example_type = "checkboard"
+    example_type = "aruco"
+    caml, camr, camd = calibrating.get_test_cams(example_type).values()
 
     stereo = calibrating.Stereo.load(
         """
 R: [[1,0,0.],[0,1,0,],[0.,0,1.]]
 _calibrating_version: 0.6.2
 cam1:
   cx: 1368
@@ -187,46 +210,53 @@
   fx: 1316
   fy: 1316
   xy:
   - 2736
   - 1824
 t:
 - - -0.3
-- - -0.0
+- - 0.0
 - - 0.0
 """
     )
+    if example_type == "checkboard":
+        for cam in [stereo.cam1, stereo.cam2]:
+            cam.K = np.array([[2545, 0, 1250.0], [0, 2545, 900], [0, 0, 1]])
+            cam.xy = (2500, 1800)
 
     # caml, camr, stereo = get_jx_stereo()
 
     stereo_gt = calibrating.Stereo(caml, camr)
     # stereo = stereo_gt.copy()
     # TODO 为什么在不设置畸变的情况下, 从 gt 继承初始值效果差好多?
+    # DONE: test L2 loss, little different, L1 sigtly better than L2
+    img_path_pairs = [
+        (
+            caml[k]["path"],
+            camr[k]["path"],
+        )
+        for k in caml
+        if k in camr
+    ]
 
     mode = "LoFTR_feature"
     # mode = "boards_feature"
     if mode == "LoFTR_feature":
-        feature_matching = LoftrFeatureMatching(dict(topk=0.5))
-        img_path_pairs = [
-            (
-                caml[k]["path"],
-                camr[k]["path"],
-            )
-            for k in caml
-            if k in camr
-        ]
-        matched = feature_matching.process_img_path_pairs(img_path_pairs[:3])
+        feature_matching = LoftrFeatureMatching(dict(topk=0.995))
+        matched = feature_matching.process_img_path_pairs(img_path_pairs[:1])
         uvs1, uvs2 = matched["uvs1"], matched["uvs2"]
     elif mode == "boards_feature":
         uvs1, uvs2 = get_uv_pairs_from_stereo_boards(stereo_gt)
 
     stereo_optimize = StereoOptimize(stereo, uvs1, uvs2)
 
     stereo_re = stereo_optimize.optimize()
     print("stereo_gt:")
     print(stereo_gt)
     print("stereo_re:")
     print(stereo_re)
-    caml.vis_stereo(camr, stereo_gt)
+    # caml.vis_stereo(camr, stereo_gt)
     caml.vis_stereo(camr, stereo_re)
-    caml.vis_stereo(camr, stereo)
-    # showb - feature_matching.vis(matched)
+    # caml.vis_stereo(camr, stereo)
+    img1, img2 = boxx.imread(img_path_pairs[0][0]), boxx.imread(img_path_pairs[0][1])
+    matched_vis = feature_matching.vis(matched, img1, img2)
+    boxx.shows(matched_vis)
```

### Comparing `calibdiff-0.0.1/calibdiff.egg-info/PKG-INFO` & `calibdiff-0.1.0/calibdiff.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calibdiff
-Version: 0.0.1
+Version: 0.1.0
 Summary: A PyTorch-based differential camera calibration library for intrinsic, extrinsic, and stereo camera calibration.
 Home-page: https://github.com/DIYer22/calibdiff
 Author: DIYer22
 Author-email: ylxx@live.com
 License: UNKNOWN
 Description: A PyTorch-based differential camera calibration library for intrinsic, extrinsic, and stereo camera calibration.
 Platform: UNKNOWN
```

### Comparing `calibdiff-0.0.1/setup.py` & `calibdiff-0.1.0/setup.py`

 * *Files identical despite different names*


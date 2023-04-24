# Comparing `tmp/focal_loss_torch-0.1.1.tar.gz` & `tmp/focal_loss_torch-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "focal_loss_torch-0.1.1.tar", last modified: Mon Jan 23 19:51:29 2023, max compression
+gzip compressed data, was "focal_loss_torch-0.1.2.tar", last modified: Mon Apr 24 14:13:09 2023, max compression
```

## Comparing `focal_loss_torch-0.1.1.tar` & `focal_loss_torch-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mathias   (1000) mathias   (1000)        0 2023-01-23 19:51:29.378218 focal_loss_torch-0.1.1/
--rw-r--r--   0 mathias   (1000) mathias   (1000)     1070 2021-09-03 11:13:37.000000 focal_loss_torch-0.1.1/LICENSE
--rw-r--r--   0 mathias   (1000) mathias   (1000)     2120 2023-01-23 19:51:29.378218 focal_loss_torch-0.1.1/PKG-INFO
--rw-r--r--   0 mathias   (1000) mathias   (1000)     1659 2023-01-23 19:44:40.000000 focal_loss_torch-0.1.1/README.md
-drwxr-xr-x   0 mathias   (1000) mathias   (1000)        0 2023-01-23 19:51:29.374884 focal_loss_torch-0.1.1/focal_loss/
--rw-r--r--   0 mathias   (1000) mathias   (1000)       57 2023-01-23 19:46:45.000000 focal_loss_torch-0.1.1/focal_loss/__init__.py
--rw-r--r--   0 mathias   (1000) mathias   (1000)     3510 2023-01-23 19:44:40.000000 focal_loss_torch-0.1.1/focal_loss/focal_loss.py
-drwxr-xr-x   0 mathias   (1000) mathias   (1000)        0 2023-01-23 19:51:29.378218 focal_loss_torch-0.1.1/focal_loss_torch.egg-info/
--rw-r--r--   0 mathias   (1000) mathias   (1000)     2120 2023-01-23 19:51:29.000000 focal_loss_torch-0.1.1/focal_loss_torch.egg-info/PKG-INFO
--rw-r--r--   0 mathias   (1000) mathias   (1000)      283 2023-01-23 19:51:29.000000 focal_loss_torch-0.1.1/focal_loss_torch.egg-info/SOURCES.txt
--rw-r--r--   0 mathias   (1000) mathias   (1000)        1 2023-01-23 19:51:29.000000 focal_loss_torch-0.1.1/focal_loss_torch.egg-info/dependency_links.txt
--rw-r--r--   0 mathias   (1000) mathias   (1000)       12 2023-01-23 19:51:29.000000 focal_loss_torch-0.1.1/focal_loss_torch.egg-info/requires.txt
--rw-r--r--   0 mathias   (1000) mathias   (1000)       11 2023-01-23 19:51:29.000000 focal_loss_torch-0.1.1/focal_loss_torch.egg-info/top_level.txt
--rw-r--r--   0 mathias   (1000) mathias   (1000)       87 2023-01-23 19:51:29.378218 focal_loss_torch-0.1.1/setup.cfg
--rw-r--r--   0 mathias   (1000) mathias   (1000)      753 2023-01-23 19:51:11.000000 focal_loss_torch-0.1.1/setup.py
+drwxr-xr-x   0 mathias   (1000) mathias   (1000)        0 2023-04-24 14:13:09.833530 focal_loss_torch-0.1.2/
+-rw-r--r--   0 mathias   (1000) mathias   (1000)     1070 2023-04-24 14:02:01.000000 focal_loss_torch-0.1.2/LICENSE
+-rw-r--r--   0 mathias   (1000) mathias   (1000)     2120 2023-04-24 14:13:09.833530 focal_loss_torch-0.1.2/PKG-INFO
+-rw-r--r--   0 mathias   (1000) mathias   (1000)     1659 2023-04-24 14:02:01.000000 focal_loss_torch-0.1.2/README.md
+drwxr-xr-x   0 mathias   (1000) mathias   (1000)        0 2023-04-24 14:13:09.830197 focal_loss_torch-0.1.2/focal_loss/
+-rw-r--r--   0 mathias   (1000) mathias   (1000)       57 2023-04-24 14:11:21.000000 focal_loss_torch-0.1.2/focal_loss/__init__.py
+-rw-r--r--   0 mathias   (1000) mathias   (1000)     3806 2023-04-24 14:02:01.000000 focal_loss_torch-0.1.2/focal_loss/focal_loss.py
+drwxr-xr-x   0 mathias   (1000) mathias   (1000)        0 2023-04-24 14:13:09.833530 focal_loss_torch-0.1.2/focal_loss_torch.egg-info/
+-rw-r--r--   0 mathias   (1000) mathias   (1000)     2120 2023-04-24 14:13:09.000000 focal_loss_torch-0.1.2/focal_loss_torch.egg-info/PKG-INFO
+-rw-r--r--   0 mathias   (1000) mathias   (1000)      283 2023-04-24 14:13:09.000000 focal_loss_torch-0.1.2/focal_loss_torch.egg-info/SOURCES.txt
+-rw-r--r--   0 mathias   (1000) mathias   (1000)        1 2023-04-24 14:13:09.000000 focal_loss_torch-0.1.2/focal_loss_torch.egg-info/dependency_links.txt
+-rw-r--r--   0 mathias   (1000) mathias   (1000)       12 2023-04-24 14:13:09.000000 focal_loss_torch-0.1.2/focal_loss_torch.egg-info/requires.txt
+-rw-r--r--   0 mathias   (1000) mathias   (1000)       11 2023-04-24 14:13:09.000000 focal_loss_torch-0.1.2/focal_loss_torch.egg-info/top_level.txt
+-rw-r--r--   0 mathias   (1000) mathias   (1000)       87 2023-04-24 14:13:09.833530 focal_loss_torch-0.1.2/setup.cfg
+-rw-r--r--   0 mathias   (1000) mathias   (1000)      753 2023-04-24 14:11:09.000000 focal_loss_torch-0.1.2/setup.py
```

### Comparing `focal_loss_torch-0.1.1/LICENSE` & `focal_loss_torch-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `focal_loss_torch-0.1.1/PKG-INFO` & `focal_loss_torch-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: focal_loss_torch
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simple pytorch implementation of focal loss
 Home-page: https://github.com/mathiaszinnen/focal_loss_torch
 Author: Mathias Zinnen
 Author-email: mathias.zinnen@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `focal_loss_torch-0.1.1/README.md` & `focal_loss_torch-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `focal_loss_torch-0.1.1/focal_loss/focal_loss.py` & `focal_loss_torch-0.1.2/focal_loss/focal_loss.py`

 * *Files 17% similar despite different names*

```diff
@@ -45,16 +45,20 @@
     def _get_weights(self, target: Tensor) -> Tensor:
         if self.weights is None:
             return torch.ones(target.shape[0])
         weights = target * self.weights
         return weights.sum(dim=-1)
 
     def _process_target(
-            self, target: Tensor, num_classes: int
+            self, target: Tensor, num_classes: int, mask: Tensor
             ) -> Tensor:
+        
+        #convert all ignore_index elements to zero to avoid error in one_hot
+        #note - the choice of value 0 is arbitrary, but it should not matter as these elements will be ignored in the loss calculation
+        target = target * (target!=self.ignore_index) 
         target = target.view(-1)
         return one_hot(target, num_classes=num_classes)
 
     def _process_preds(self, x: Tensor) -> Tensor:
         if x.dim() == 1:
             x = torch.vstack([1 - x, x])
             x = x.permute(1, 0)
@@ -75,15 +79,15 @@
                 make sure to pass the values to sigmoid for binary \
                 classification or softmax for multi-class classification'
         )
         mask = target == self.ignore_index
         mask = mask.view(-1)
         x = self._process_preds(x)
         num_classes = x.shape[-1]
-        target = self._process_target(target, num_classes)
+        target = self._process_target(target, num_classes, mask)
         weights = self._get_weights(target).to(x.device)
         pt = self._calc_pt(target, x, mask)
         focal = 1 - pt
         nll = -torch.log(self.eps + pt)
         nll = nll.masked_fill(mask, 0)
         loss = weights * (focal ** self.gamma) * nll
         return self._reduce(loss, mask, weights)
```

### Comparing `focal_loss_torch-0.1.1/focal_loss_torch.egg-info/PKG-INFO` & `focal_loss_torch-0.1.2/focal_loss_torch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: focal-loss-torch
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simple pytorch implementation of focal loss
 Home-page: https://github.com/mathiaszinnen/focal_loss_torch
 Author: Mathias Zinnen
 Author-email: mathias.zinnen@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `focal_loss_torch-0.1.1/setup.py` & `focal_loss_torch-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(
     setup_requires=['wheel'],
     name="focal_loss_torch",
-    version="0.1.1",
+    version="0.1.2",
     description="Simple pytorch implementation of focal loss",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/mathiaszinnen/focal_loss_torch",
     author="Mathias Zinnen",
     author_email="mathias.zinnen@gmail.com",
     license="MIT",
```


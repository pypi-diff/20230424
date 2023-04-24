# Comparing `tmp/searchlogit-0.3.7.tar.gz` & `tmp/searchlogit-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchlogit-0.3.7.tar", last modified: Fri Apr 21 05:01:11 2023, max compression
+gzip compressed data, was "searchlogit-0.3.8.tar", last modified: Mon Apr 24 09:14:28 2023, max compression
```

## Comparing `searchlogit-0.3.7.tar` & `searchlogit-0.3.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 05:01:11.583451 searchlogit-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-21 05:01:02.000000 searchlogit-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-04-21 05:01:11.583451 searchlogit-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-04-21 05:01:02.000000 searchlogit-0.3.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 05:01:11.583451 searchlogit-0.3.7/searchlogit/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-21 05:01:02.000000 searchlogit-0.3.7/searchlogit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29646 2023-04-21 05:01:02.000000 searchlogit-0.3.7/searchlogit/_choice_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-21 05:01:02.000000 searchlogit-0.3.7/searchlogit/_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-04-21 05:01:02.000000 searchlogit-0.3.7/searchlogit/boxcox_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    50811 2023-04-21 05:01:02.000000 searchlogit-0.3.7/searchlogit/latent_class_mixed_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    35762 2023-04-21 05:01:02.000000 searchlogit-0.3.7/searchlogit/latent_class_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    60055 2023-04-21 05:01:02.000000 searchlogit-0.3.7/searchlogit/mixed_logit.py
--rw-r--r--   0 runner    (1001) docker     (123)    14368 2023-04-21 05:01:02.000000 searchlogit-0.3.7/searchlogit/multinomial_logit.py
--rw-r--r--   0 runner    (1001) docker     (123)   169595 2023-04-21 05:01:02.000000 searchlogit-0.3.7/searchlogit/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 05:01:11.583451 searchlogit-0.3.7/searchlogit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-04-21 05:01:11.000000 searchlogit-0.3.7/searchlogit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-21 05:01:11.000000 searchlogit-0.3.7/searchlogit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 05:01:11.000000 searchlogit-0.3.7/searchlogit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 05:01:11.000000 searchlogit-0.3.7/searchlogit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-21 05:01:11.000000 searchlogit-0.3.7/searchlogit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-21 05:01:11.000000 searchlogit-0.3.7/searchlogit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-21 05:01:11.583451 searchlogit-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-21 05:01:02.000000 searchlogit-0.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 05:01:11.583451 searchlogit-0.3.7/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2391 2023-04-21 05:01:02.000000 searchlogit-0.3.7/tests/test__choice_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-04-21 05:01:02.000000 searchlogit-0.3.7/tests/test__device.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-21 05:01:02.000000 searchlogit-0.3.7/tests/test_latent_class_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-21 05:01:02.000000 searchlogit-0.3.7/tests/test_mixed_logit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2862 2023-04-21 05:01:02.000000 searchlogit-0.3.7/tests/test_multinomial_logit.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 05:01:02.000000 searchlogit-0.3.7/tests/test_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:28.718192 searchlogit-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-24 09:14:15.000000 searchlogit-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-04-24 09:14:28.718192 searchlogit-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-04-24 09:14:15.000000 searchlogit-0.3.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:28.714192 searchlogit-0.3.8/searchlogit/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-24 09:14:15.000000 searchlogit-0.3.8/searchlogit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29646 2023-04-24 09:14:15.000000 searchlogit-0.3.8/searchlogit/_choice_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-24 09:14:15.000000 searchlogit-0.3.8/searchlogit/_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-04-24 09:14:15.000000 searchlogit-0.3.8/searchlogit/boxcox_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50811 2023-04-24 09:14:15.000000 searchlogit-0.3.8/searchlogit/latent_class_mixed_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35762 2023-04-24 09:14:15.000000 searchlogit-0.3.8/searchlogit/latent_class_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60055 2023-04-24 09:14:15.000000 searchlogit-0.3.8/searchlogit/mixed_logit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14342 2023-04-24 09:14:15.000000 searchlogit-0.3.8/searchlogit/multinomial_logit.py
+-rw-r--r--   0 runner    (1001) docker     (123)   169595 2023-04-24 09:14:15.000000 searchlogit-0.3.8/searchlogit/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:28.718192 searchlogit-0.3.8/searchlogit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-04-24 09:14:28.000000 searchlogit-0.3.8/searchlogit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-24 09:14:28.000000 searchlogit-0.3.8/searchlogit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 09:14:28.000000 searchlogit-0.3.8/searchlogit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 09:14:28.000000 searchlogit-0.3.8/searchlogit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-24 09:14:28.000000 searchlogit-0.3.8/searchlogit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 09:14:28.000000 searchlogit-0.3.8/searchlogit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-24 09:14:28.718192 searchlogit-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-24 09:14:15.000000 searchlogit-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:28.718192 searchlogit-0.3.8/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2391 2023-04-24 09:14:15.000000 searchlogit-0.3.8/tests/test__choice_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-04-24 09:14:15.000000 searchlogit-0.3.8/tests/test__device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-24 09:14:15.000000 searchlogit-0.3.8/tests/test_latent_class_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-24 09:14:15.000000 searchlogit-0.3.8/tests/test_mixed_logit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2862 2023-04-24 09:14:15.000000 searchlogit-0.3.8/tests/test_multinomial_logit.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 09:14:15.000000 searchlogit-0.3.8/tests/test_search.py
```

### Comparing `searchlogit-0.3.7/LICENSE` & `searchlogit-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.7/PKG-INFO` & `searchlogit-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchlogit
-Version: 0.3.7
+Version: 0.3.8
 Summary: Extensions for a Python package for                               GPU-accelerated estimation of mixed logit models.
 Home-page: https://github.com/RyanJafefKelly/searchlogit
 Author: Ryan Kelly, Prithvi Beeramoole and Alexander Paz
 Author-email: ryan@kiiii.com
 License: MIT
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
```

### Comparing `searchlogit-0.3.7/README.rst` & `searchlogit-0.3.8/README.rst`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.7/searchlogit/_choice_model.py` & `searchlogit-0.3.8/searchlogit/_choice_model.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.7/searchlogit/_device.py` & `searchlogit-0.3.8/searchlogit/_device.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.7/searchlogit/boxcox_functions.py` & `searchlogit-0.3.8/searchlogit/boxcox_functions.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.7/searchlogit/latent_class_mixed_model.py` & `searchlogit-0.3.8/searchlogit/latent_class_mixed_model.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.7/searchlogit/latent_class_model.py` & `searchlogit-0.3.8/searchlogit/latent_class_model.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.7/searchlogit/mixed_logit.py` & `searchlogit-0.3.8/searchlogit/mixed_logit.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.7/searchlogit/multinomial_logit.py` & `searchlogit-0.3.8/searchlogit/multinomial_logit.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,20 +225,21 @@
             XB += XB_trans
 
         XB[XB > max_exp_val] = max_exp_val  # avoiding infs
         XB[XB < -max_exp_val] = -max_exp_val  # avoiding infs
 
         XB = XB.reshape(self.N, self.J)
 
+        eXB = np.exp(XB)
         if avail is not None:
-            XB = XB*avail
+            eXB = eXB*avail
 
-        XB_logsumexp = np.logaddexp.reduce(XB, axis=1, keepdims=True)
-        p = np.exp(XB - np.vstack(XB_logsumexp))
+        p = eXB / np.sum(eXB, axis=1, keepdims=True)
 
+        # TODO
         self.ind_pred_prob = p
         self.choice_pred_prob = p
         self.pred_prob = np.mean(p, axis=0)
 
         return p, Xtrans_lmda
 
     def _loglik_and_gradient(self, betas, X, y, weights, avail):
@@ -299,15 +300,15 @@
             self.Hinv = Hinv
 
         grad = np.sum(grad, axis=0, dtype=np.float64)
         self.gtol_res = np.linalg.norm(grad, ord=np.inf)
 
         result = (loglik)
         logger.debug('Norm: {}'.format(np.linalg.norm(grad, ord=np.inf)))
-        # print('norm', np.linalg.norm(grad, ord=np.inf)) #  this is useful debug gtol
+        print('norm', np.linalg.norm(grad, ord=np.inf)) #  this is useful debug gtol
 
         if self.grad:
             result = (-loglik, -grad)
             if self.hess:
                 result = (-loglik, -grad, Hinv)
 
         return result
```

### Comparing `searchlogit-0.3.7/searchlogit/search.py` & `searchlogit-0.3.8/searchlogit/search.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.7/searchlogit.egg-info/PKG-INFO` & `searchlogit-0.3.8/searchlogit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchlogit
-Version: 0.3.7
+Version: 0.3.8
 Summary: Extensions for a Python package for                               GPU-accelerated estimation of mixed logit models.
 Home-page: https://github.com/RyanJafefKelly/searchlogit
 Author: Ryan Kelly, Prithvi Beeramoole and Alexander Paz
 Author-email: ryan@kiiii.com
 License: MIT
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
```

### Comparing `searchlogit-0.3.7/searchlogit.egg-info/SOURCES.txt` & `searchlogit-0.3.8/searchlogit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.7/setup.py` & `searchlogit-0.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import setuptools
 
 with codecs.open("README.rst", encoding='utf8') as fh:
     long_description = fh.read()
 
 setuptools.setup(name='searchlogit',
-                 version='0.3.7',
+                 version='0.3.8',
                  description='Extensions for a Python package for \
                               GPU-accelerated estimation of mixed logit models.',
                  long_description=long_description,
                  long_description_content_type="text/x-rst",
                  url='https://github.com/RyanJafefKelly/searchlogit',
                  author='Ryan Kelly, Prithvi Beeramoole and Alexander Paz',
                  author_email='ryan@kiiii.com',
```

### Comparing `searchlogit-0.3.7/tests/test__choice_model.py` & `searchlogit-0.3.8/tests/test__choice_model.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.7/tests/test__device.py` & `searchlogit-0.3.8/tests/test__device.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.7/tests/test_latent_class_model.py` & `searchlogit-0.3.8/tests/test_latent_class_model.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.7/tests/test_mixed_logit.py` & `searchlogit-0.3.8/tests/test_mixed_logit.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.7/tests/test_multinomial_logit.py` & `searchlogit-0.3.8/tests/test_multinomial_logit.py`

 * *Files identical despite different names*


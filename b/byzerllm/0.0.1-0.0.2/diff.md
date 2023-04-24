# Comparing `tmp/byzerllm-0.0.1.tar.gz` & `tmp/byzerllm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byzerllm-0.0.1.tar", last modified: Thu Apr 20 03:56:53 2023, max compression
+gzip compressed data, was "byzerllm-0.0.2.tar", last modified: Mon Apr 24 12:10:10 2023, max compression
```

## Comparing `byzerllm-0.0.1.tar` & `byzerllm-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,29 @@
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-20 03:56:53.886438 byzerllm-0.0.1/
--rw-r--r--   0 allwefantasy   (501) staff       (20)      314 2023-04-20 03:56:53.886057 byzerllm-0.0.1/PKG-INFO
--rw-r--r--   0 allwefantasy   (501) staff       (20)       38 2023-04-20 03:56:53.886529 byzerllm-0.0.1/setup.cfg
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1194 2023-04-20 03:56:51.000000 byzerllm-0.0.1/setup.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-20 03:56:53.881294 byzerllm-0.0.1/src/
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-20 03:56:53.882383 byzerllm-0.0.1/src/byzerllm/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-04-04 03:26:20.000000 byzerllm-0.0.1/src/byzerllm/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-20 03:56:53.885553 byzerllm-0.0.1/src/byzerllm/chatglm6b/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-04-04 03:28:57.000000 byzerllm-0.0.1/src/byzerllm/chatglm6b/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     8182 2023-04-04 03:41:37.000000 byzerllm-0.0.1/src/byzerllm/chatglm6b/arguments.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    21286 2023-04-20 03:53:12.000000 byzerllm-0.0.1/src/byzerllm/chatglm6b/finetune.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    11575 2023-04-04 03:39:19.000000 byzerllm-0.0.1/src/byzerllm/chatglm6b/trainer_seq2seq.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)       22 2023-04-04 03:25:39.000000 byzerllm-0.0.1/src/byzerllm/version.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-20 03:56:53.883709 byzerllm-0.0.1/src/byzerllm.egg-info/
--rw-r--r--   0 allwefantasy   (501) staff       (20)      314 2023-04-20 03:56:53.000000 byzerllm-0.0.1/src/byzerllm.egg-info/PKG-INFO
--rw-r--r--   0 allwefantasy   (501) staff       (20)      349 2023-04-20 03:56:53.000000 byzerllm-0.0.1/src/byzerllm.egg-info/SOURCES.txt
--rw-r--r--   0 allwefantasy   (501) staff       (20)        1 2023-04-20 03:56:53.000000 byzerllm-0.0.1/src/byzerllm.egg-info/dependency_links.txt
--rw-r--r--   0 allwefantasy   (501) staff       (20)        9 2023-04-20 03:56:53.000000 byzerllm-0.0.1/src/byzerllm.egg-info/top_level.txt
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-24 12:10:10.881198 byzerllm-0.0.2/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      314 2023-04-24 12:10:10.880917 byzerllm-0.0.2/PKG-INFO
+-rw-r--r--   0 allwefantasy   (501) staff       (20)       38 2023-04-24 12:10:10.881274 byzerllm-0.0.2/setup.cfg
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1205 2023-04-24 12:09:56.000000 byzerllm-0.0.2/setup.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-24 12:10:10.872729 byzerllm-0.0.2/src/
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-24 12:10:10.873929 byzerllm-0.0.2/src/byzerllm/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-04-04 03:26:20.000000 byzerllm-0.0.2/src/byzerllm/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-24 12:10:10.877472 byzerllm-0.0.2/src/byzerllm/chatglm6b/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-04-04 03:28:57.000000 byzerllm-0.0.2/src/byzerllm/chatglm6b/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     8182 2023-04-04 03:41:37.000000 byzerllm-0.0.2/src/byzerllm/chatglm6b/arguments.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    21286 2023-04-20 03:53:12.000000 byzerllm-0.0.2/src/byzerllm/chatglm6b/finetune.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    11575 2023-04-04 03:39:19.000000 byzerllm-0.0.2/src/byzerllm/chatglm6b/trainer_seq2seq.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-24 12:10:10.878806 byzerllm-0.0.2/src/byzerllm/moss/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-04-24 12:08:52.000000 byzerllm-0.0.2/src/byzerllm/moss/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    12657 2023-04-24 12:08:52.000000 byzerllm-0.0.2/src/byzerllm/moss/finetune_moss.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-24 12:10:10.880586 byzerllm-0.0.2/src/byzerllm/moss/models/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-04-24 12:08:52.000000 byzerllm-0.0.2/src/byzerllm/moss/models/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5097 2023-04-24 12:08:52.000000 byzerllm-0.0.2/src/byzerllm/moss/models/configuration_moss.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6735 2023-04-24 12:08:52.000000 byzerllm-0.0.2/src/byzerllm/moss/models/custom_autotune.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    31351 2023-04-24 12:08:52.000000 byzerllm-0.0.2/src/byzerllm/moss/models/modeling_moss.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    18866 2023-04-24 12:08:52.000000 byzerllm-0.0.2/src/byzerllm/moss/models/quantization.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    15952 2023-04-24 12:08:52.000000 byzerllm-0.0.2/src/byzerllm/moss/models/tokenization_moss.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    17212 2023-04-24 12:08:52.000000 byzerllm-0.0.2/src/byzerllm/moss/moss_inference.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)       22 2023-04-24 12:08:52.000000 byzerllm-0.0.2/src/byzerllm/version.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2023-04-24 12:10:10.875360 byzerllm-0.0.2/src/byzerllm.egg-info/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      314 2023-04-24 12:10:10.000000 byzerllm-0.0.2/src/byzerllm.egg-info/PKG-INFO
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      707 2023-04-24 12:10:10.000000 byzerllm-0.0.2/src/byzerllm.egg-info/SOURCES.txt
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        1 2023-04-24 12:10:10.000000 byzerllm-0.0.2/src/byzerllm.egg-info/dependency_links.txt
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        9 2023-04-24 12:10:10.000000 byzerllm-0.0.2/src/byzerllm.egg-info/top_level.txt
```

### Comparing `byzerllm-0.0.1/setup.py` & `byzerllm-0.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 __version__ = None
 with open(version_path) as f:
     exec(f.read(), globals())
 
 req_path = os.path.join(folder, "requirements.txt")
 install_requires = []
-#if os.path.exists(req_path):
-#    with open(req_path) as fp:
-#        install_requires = [line.strip() for line in fp]
+# if os.path.exists(req_path):
+#     with open(req_path) as fp:
+#         install_requires = [line.strip() for line in fp]
 
 readme_path = os.path.join(folder, "README.md")
 readme_contents = ""
 if os.path.exists(readme_path):
     with open(readme_path) as fp:
         readme_contents = fp.read().strip()
 
@@ -28,14 +28,14 @@
     author="allwefantasy",
     long_description=readme_contents,
     long_description_content_type="text/markdown",
     package_dir={"": "src"},
     packages=find_packages("src"),
     package_data={},
     install_requires=install_requires,
-    classifiers=[
+    classifiers=[        
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     requires_python=">=3.9",
 )
```

### Comparing `byzerllm-0.0.1/src/byzerllm/chatglm6b/arguments.py` & `byzerllm-0.0.2/src/byzerllm/chatglm6b/arguments.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.1/src/byzerllm/chatglm6b/finetune.py` & `byzerllm-0.0.2/src/byzerllm/chatglm6b/finetune.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.0.1/src/byzerllm/chatglm6b/trainer_seq2seq.py` & `byzerllm-0.0.2/src/byzerllm/chatglm6b/trainer_seq2seq.py`

 * *Files identical despite different names*


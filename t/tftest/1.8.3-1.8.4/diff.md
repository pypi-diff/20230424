# Comparing `tmp/tftest-1.8.3.tar.gz` & `tmp/tftest-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tftest-1.8.3.tar", last modified: Sun Apr 16 10:11:46 2023, max compression
+gzip compressed data, was "tftest-1.8.4.tar", last modified: Mon Apr 24 14:43:21 2023, max compression
```

## Comparing `tftest-1.8.3.tar` & `tftest-1.8.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 ludomagno  (1000) ludomagno  (1000)        0 2023-04-16 10:11:46.448596 tftest-1.8.3/
--rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)    11358 2019-03-22 10:16:40.000000 tftest-1.8.3/LICENSE
--rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)     6345 2023-04-16 10:11:46.448596 tftest-1.8.3/PKG-INFO
--rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)     5888 2022-11-02 06:43:54.000000 tftest-1.8.3/README.md
--rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)       38 2023-04-16 10:11:46.448596 tftest-1.8.3/setup.cfg
--rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     1331 2022-10-02 16:38:55.000000 tftest-1.8.3/setup.py
-drwxr-xr-x   0 ludomagno  (1000) ludomagno  (1000)        0 2023-04-16 10:11:46.447596 tftest-1.8.3/test/
--rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)     5036 2023-01-26 11:01:12.000000 tftest-1.8.3/test/test_args.py
--rw-r-----   0 ludomagno  (1000) ludomagno  (1000)      989 2022-05-03 17:38:56.000000 tftest-1.8.3/test/test_backend_config.py
--rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)     6280 2022-11-09 06:41:18.000000 tftest-1.8.3/test/test_cache.py
--rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     1150 2022-05-03 17:45:33.000000 tftest-1.8.3/test/test_files.py
--rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     1322 2022-05-03 17:38:59.000000 tftest-1.8.3/test/test_no_outputs.py
--rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     1505 2022-09-15 05:23:54.000000 tftest-1.8.3/test/test_pickle.py
--rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     2663 2022-08-04 06:30:41.000000 tftest-1.8.3/test/test_plan.py
--rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     2246 2022-05-03 17:45:33.000000 tftest-1.8.3/test/test_prevent_destroy.py
--rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     1002 2022-05-03 17:39:03.000000 tftest-1.8.3/test/test_sample_apply.py
--rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     1344 2022-05-03 17:39:05.000000 tftest-1.8.3/test/test_sample_plan.py
--rw-r-----   0 ludomagno  (1000) ludomagno  (1000)      993 2022-08-04 10:45:46.000000 tftest-1.8.3/test/test_sample_plan_error.py
--rw-r-----   0 ludomagno  (1000) ludomagno  (1000)      925 2022-05-03 17:39:04.000000 tftest-1.8.3/test/test_sample_plan_no_variables.py
--rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     1181 2022-05-03 17:39:06.000000 tftest-1.8.3/test/test_state.py
--rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     2784 2022-05-03 17:45:33.000000 tftest-1.8.3/test/test_tg_all.py
--rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     1005 2022-05-03 17:39:09.000000 tftest-1.8.3/test/test_value_dict.py
--rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     1543 2022-07-11 12:25:59.000000 tftest-1.8.3/test/test_workspace.py
-drwxr-xr-x   0 ludomagno  (1000) ludomagno  (1000)        0 2023-04-16 10:11:46.448596 tftest-1.8.3/tftest.egg-info/
--rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)     6345 2023-04-16 10:11:46.000000 tftest-1.8.3/tftest.egg-info/PKG-INFO
--rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)      537 2023-04-16 10:11:46.000000 tftest-1.8.3/tftest.egg-info/SOURCES.txt
--rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)        1 2023-04-16 10:11:46.000000 tftest-1.8.3/tftest.egg-info/dependency_links.txt
--rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)        7 2023-04-16 10:11:46.000000 tftest-1.8.3/tftest.egg-info/top_level.txt
--rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)    28712 2023-04-16 10:07:35.000000 tftest-1.8.3/tftest.py
+drwxr-xr-x   0 ludomagno  (1000) ludomagno  (1000)        0 2023-04-24 14:43:21.407570 tftest-1.8.4/
+-rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)    11358 2019-03-22 10:16:40.000000 tftest-1.8.4/LICENSE
+-rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)     6345 2023-04-24 14:43:21.407570 tftest-1.8.4/PKG-INFO
+-rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)     5888 2022-11-02 06:43:54.000000 tftest-1.8.4/README.md
+-rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)       38 2023-04-24 14:43:21.407570 tftest-1.8.4/setup.cfg
+-rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     1331 2022-10-02 16:38:55.000000 tftest-1.8.4/setup.py
+drwxr-xr-x   0 ludomagno  (1000) ludomagno  (1000)        0 2023-04-24 14:43:21.407570 tftest-1.8.4/test/
+-rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)     5036 2023-01-26 11:01:12.000000 tftest-1.8.4/test/test_args.py
+-rw-r-----   0 ludomagno  (1000) ludomagno  (1000)      989 2022-05-03 17:38:56.000000 tftest-1.8.4/test/test_backend_config.py
+-rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)     6280 2022-11-09 06:41:18.000000 tftest-1.8.4/test/test_cache.py
+-rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     1150 2022-05-03 17:45:33.000000 tftest-1.8.4/test/test_files.py
+-rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     1322 2022-05-03 17:38:59.000000 tftest-1.8.4/test/test_no_outputs.py
+-rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     1505 2022-09-15 05:23:54.000000 tftest-1.8.4/test/test_pickle.py
+-rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     2663 2022-08-04 06:30:41.000000 tftest-1.8.4/test/test_plan.py
+-rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     2246 2022-05-03 17:45:33.000000 tftest-1.8.4/test/test_prevent_destroy.py
+-rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     1002 2022-05-03 17:39:03.000000 tftest-1.8.4/test/test_sample_apply.py
+-rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     1344 2022-05-03 17:39:05.000000 tftest-1.8.4/test/test_sample_plan.py
+-rw-r-----   0 ludomagno  (1000) ludomagno  (1000)      993 2022-08-04 10:45:46.000000 tftest-1.8.4/test/test_sample_plan_error.py
+-rw-r-----   0 ludomagno  (1000) ludomagno  (1000)      925 2022-05-03 17:39:04.000000 tftest-1.8.4/test/test_sample_plan_no_variables.py
+-rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     1181 2022-05-03 17:39:06.000000 tftest-1.8.4/test/test_state.py
+-rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     2784 2022-05-03 17:45:33.000000 tftest-1.8.4/test/test_tg_all.py
+-rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     1005 2022-05-03 17:39:09.000000 tftest-1.8.4/test/test_value_dict.py
+-rw-r-----   0 ludomagno  (1000) ludomagno  (1000)     1543 2022-07-11 12:25:59.000000 tftest-1.8.4/test/test_workspace.py
+drwxr-xr-x   0 ludomagno  (1000) ludomagno  (1000)        0 2023-04-24 14:43:21.407570 tftest-1.8.4/tftest.egg-info/
+-rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)     6345 2023-04-24 14:43:21.000000 tftest-1.8.4/tftest.egg-info/PKG-INFO
+-rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)      537 2023-04-24 14:43:21.000000 tftest-1.8.4/tftest.egg-info/SOURCES.txt
+-rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)        1 2023-04-24 14:43:21.000000 tftest-1.8.4/tftest.egg-info/dependency_links.txt
+-rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)        7 2023-04-24 14:43:21.000000 tftest-1.8.4/tftest.egg-info/top_level.txt
+-rw-r--r--   0 ludomagno  (1000) ludomagno  (1000)    28834 2023-04-24 14:40:08.000000 tftest-1.8.4/tftest.py
```

### Comparing `tftest-1.8.3/LICENSE` & `tftest-1.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tftest-1.8.3/PKG-INFO` & `tftest-1.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tftest
-Version: 1.8.3
+Version: 1.8.4
 Summary: Simple Terraform test helper
 Home-page: https://github.com/GoogleCloudPlatform/terraform-python-testing-helper
 Author: Ludovico Magnocavallo
 Author-email: ludomagno@google.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `tftest-1.8.3/README.md` & `tftest-1.8.4/README.md`

 * *Files identical despite different names*

### Comparing `tftest-1.8.3/setup.py` & `tftest-1.8.4/setup.py`

 * *Files identical despite different names*

### Comparing `tftest-1.8.3/test/test_args.py` & `tftest-1.8.4/test/test_args.py`

 * *Files identical despite different names*

### Comparing `tftest-1.8.3/test/test_backend_config.py` & `tftest-1.8.4/test/test_backend_config.py`

 * *Files identical despite different names*

### Comparing `tftest-1.8.3/test/test_cache.py` & `tftest-1.8.4/test/test_cache.py`

 * *Files identical despite different names*

### Comparing `tftest-1.8.3/test/test_files.py` & `tftest-1.8.4/test/test_files.py`

 * *Files identical despite different names*

### Comparing `tftest-1.8.3/test/test_no_outputs.py` & `tftest-1.8.4/test/test_no_outputs.py`

 * *Files identical despite different names*

### Comparing `tftest-1.8.3/test/test_pickle.py` & `tftest-1.8.4/test/test_pickle.py`

 * *Files identical despite different names*

### Comparing `tftest-1.8.3/test/test_plan.py` & `tftest-1.8.4/test/test_plan.py`

 * *Files identical despite different names*

### Comparing `tftest-1.8.3/test/test_prevent_destroy.py` & `tftest-1.8.4/test/test_prevent_destroy.py`

 * *Files identical despite different names*

### Comparing `tftest-1.8.3/test/test_sample_apply.py` & `tftest-1.8.4/test/test_sample_apply.py`

 * *Files identical despite different names*

### Comparing `tftest-1.8.3/test/test_sample_plan.py` & `tftest-1.8.4/test/test_sample_plan.py`

 * *Files identical despite different names*

### Comparing `tftest-1.8.3/test/test_sample_plan_error.py` & `tftest-1.8.4/test/test_sample_plan_error.py`

 * *Files identical despite different names*

### Comparing `tftest-1.8.3/test/test_sample_plan_no_variables.py` & `tftest-1.8.4/test/test_sample_plan_no_variables.py`

 * *Files identical despite different names*

### Comparing `tftest-1.8.3/test/test_state.py` & `tftest-1.8.4/test/test_state.py`

 * *Files identical despite different names*

### Comparing `tftest-1.8.3/test/test_tg_all.py` & `tftest-1.8.4/test/test_tg_all.py`

 * *Files identical despite different names*

### Comparing `tftest-1.8.3/test/test_value_dict.py` & `tftest-1.8.4/test/test_value_dict.py`

 * *Files identical despite different names*

### Comparing `tftest-1.8.3/test/test_workspace.py` & `tftest-1.8.4/test/test_workspace.py`

 * *Files identical despite different names*

### Comparing `tftest-1.8.3/tftest.egg-info/PKG-INFO` & `tftest-1.8.4/tftest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tftest
-Version: 1.8.3
+Version: 1.8.4
 Summary: Simple Terraform test helper
 Home-page: https://github.com/GoogleCloudPlatform/terraform-python-testing-helper
 Author: Ludovico Magnocavallo
 Author-email: ludomagno@google.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `tftest-1.8.3/tftest.egg-info/SOURCES.txt` & `tftest-1.8.4/tftest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tftest-1.8.3/tftest.py` & `tftest-1.8.4/tftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 import weakref
 
 from functools import partial
 from hashlib import sha1
 from pathlib import Path
 from typing import List
 
-__version__ = '1.8.3'
+__version__ = '1.8.4'
 
 _LOGGER = logging.getLogger('tftest')
 
 TerraformCommandOutput = collections.namedtuple('TerraformCommandOutput',
                                                 'retcode out err')
 
 TerraformStateResource = collections.namedtuple(
@@ -382,15 +382,16 @@
     return path if os.path.isabs(path) else os.path.join(self._basedir, path)
 
   def _dirhash(self, directory, hash, ignore_hidden=False,
                exclude_directories=[], excluded_extensions=[]):
     """Returns hash of directory's file contents"""
     assert Path(directory).is_dir()
     try:
-      dir_iter = sorted(Path(directory).iterdir(), key=lambda p: str(p).lower())
+      dir_iter = sorted(Path(directory).iterdir(),
+                        key=lambda p: str(p).lower())
     except FileNotFoundError:
       return hash
     for path in dir_iter:
       if path.is_file():
         if ignore_hidden and path.name.startswith("."):
           continue
         if path.suffix in excluded_extensions:
@@ -429,15 +430,15 @@
               open(method_kwargs[path_param], 'rb').read()).hexdigest()
 
     # creates hash of all file content within tfdir
     # excludes .terraform/, hidden files, tfstate files from being used for hash
     params["tfdir"] = self._dirhash(self.tfdir, sha1(), ignore_hidden=True,
                                     exclude_directories=[".terraform"],
                                     excluded_extensions=['.backup', '.tfstate'
-                                                        ]).hexdigest()
+                                                         ]).hexdigest()
 
     return sha1(
         json.dumps(params, sort_keys=True,
                    default=str).encode("cp037")).hexdigest() + ".pickle"
 
   def _cache(func):
 
@@ -454,15 +455,15 @@
 
       if not self.enable_cache:
         return func(self, **kwargs)
       elif not kwargs.get("use_cache", False):
         return func(self, **kwargs)
 
       cache_dir = self.cache_dir / \
-          Path(self.tfdir.strip("/")) / Path(func.__name__)
+          Path(sha1(self.tfdir.encode("cp037")).hexdigest()) / Path(func.__name__)
       cache_dir.mkdir(parents=True, exist_ok=True)
 
       hash_filename = self.generate_cache_hash(kwargs)
       cache_key = cache_dir / hash_filename
       _LOGGER.debug("Cache key: %s", cache_key)
 
       try:
@@ -701,16 +702,17 @@
     _LOGGER.debug([cmd, cmd_args])
     cmdline = [self.binary, *self._tg_ra(), cmd]
     cmdline += cmd_args
     _LOGGER.info(cmdline)
     retcode = None
     full_output_lines = []
     try:
+      stderr_mode = subprocess.STDOUT if os.name == 'nt' else subprocess.PIPE
       p = subprocess.Popen(cmdline, stdout=subprocess.PIPE,
-                           stderr=subprocess.PIPE, cwd=self.tfdir, env=self.env,
+                           stderr=stderr_mode, cwd=self.tfdir, env=self.env,
                            universal_newlines=True, encoding='utf-8',
                            errors='ignore')
       while True:
         output = p.stdout.readline()
         if output == '' and p.poll() is not None:
           break
         if output:
```


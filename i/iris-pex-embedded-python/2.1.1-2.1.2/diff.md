# Comparing `tmp/iris_pex_embedded_python-2.1.1.tar.gz` & `tmp/iris_pex_embedded_python-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iris_pex_embedded_python-2.1.1.tar", last modified: Fri Apr 21 15:02:40 2023, max compression
+gzip compressed data, was "iris_pex_embedded_python-2.1.2.tar", last modified: Mon Apr 24 18:55:23 2023, max compression
```

## Comparing `iris_pex_embedded_python-2.1.1.tar` & `iris_pex_embedded_python-2.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-04-21 15:02:40.426096 iris_pex_embedded_python-2.1.1/
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1089 2021-08-27 09:20:59.000000 iris_pex_embedded_python-2.1.1/LICENSE
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    35813 2023-04-21 15:02:40.418997 iris_pex_embedded_python-2.1.1/PKG-INFO
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    34904 2022-12-16 16:40:23.000000 iris_pex_embedded_python-2.1.1/README.md
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2022-12-16 16:40:23.000000 iris_pex_embedded_python-2.1.1/pyproject.toml
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)       38 2023-04-21 15:02:40.426471 iris_pex_embedded_python-2.1.1/setup.cfg
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     2016 2023-04-21 15:01:45.000000 iris_pex_embedded_python-2.1.1/setup.py
-drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-04-21 15:02:40.326360 iris_pex_embedded_python-2.1.1/src/
-drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-04-21 15:02:40.325209 iris_pex_embedded_python-2.1.1/src/grongier/
-drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-04-21 15:02:40.342478 iris_pex_embedded_python-2.1.1/src/grongier/iris/
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.1/src/grongier/iris/__init__.py
-drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-04-21 15:02:40.384415 iris_pex_embedded_python-2.1.1/src/grongier/pex/
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1166 2023-04-18 10:17:07.000000 iris_pex_embedded_python-2.1.1/src/grongier/pex/__init__.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    20152 2023-04-21 15:01:34.000000 iris_pex_embedded_python-2.1.1/src/grongier/pex/_business_host.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     3509 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.1/src/grongier/pex/_business_operation.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    11838 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.1/src/grongier/pex/_business_process.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     3735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.1/src/grongier/pex/_business_service.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    15107 2023-04-21 08:43:30.000000 iris_pex_embedded_python-2.1.1/src/grongier/pex/_common.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     3840 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.1/src/grongier/pex/_director.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1661 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.1/src/grongier/pex/_inbound_adapter.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      325 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.1/src/grongier/pex/_message.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.1/src/grongier/pex/_outbound_adapter.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      331 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.1/src/grongier/pex/_pickle_message.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     5033 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.1/src/grongier/pex/_private_session_duplex.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1722 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.1/src/grongier/pex/_private_session_process.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     7063 2023-04-21 08:18:02.000000 iris_pex_embedded_python-2.1.1/src/grongier/pex/_utils.py
-drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-04-21 15:02:40.413571 iris_pex_embedded_python-2.1.1/src/iris_pex_embedded_python.egg-info/
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    35813 2023-04-21 15:02:40.000000 iris_pex_embedded_python-2.1.1/src/iris_pex_embedded_python.egg-info/PKG-INFO
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      824 2023-04-21 15:02:40.000000 iris_pex_embedded_python-2.1.1/src/iris_pex_embedded_python.egg-info/SOURCES.txt
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        1 2023-04-21 15:02:40.000000 iris_pex_embedded_python-2.1.1/src/iris_pex_embedded_python.egg-info/dependency_links.txt
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)       14 2023-04-21 15:02:40.000000 iris_pex_embedded_python-2.1.1/src/iris_pex_embedded_python.egg-info/requires.txt
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        9 2023-04-21 15:02:40.000000 iris_pex_embedded_python-2.1.1/src/iris_pex_embedded_python.egg-info/top_level.txt
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-24 18:55:23.773568 iris_pex_embedded_python-2.1.2/
+-rw-r--r--   0 grongier (902446405) 1252422112     1089 2021-08-27 09:20:59.000000 iris_pex_embedded_python-2.1.2/LICENSE
+-rw-r--r--   0 grongier (902446405) 1252422112    35813 2023-04-24 18:55:23.771821 iris_pex_embedded_python-2.1.2/PKG-INFO
+-rw-r--r--   0 grongier (902446405) 1252422112    34904 2022-12-16 16:40:23.000000 iris_pex_embedded_python-2.1.2/README.md
+-rw-r--r--   0 grongier (902446405) 1252422112        0 2022-12-16 16:40:23.000000 iris_pex_embedded_python-2.1.2/pyproject.toml
+-rw-r--r--   0 grongier (902446405) 1252422112       38 2023-04-24 18:55:23.773883 iris_pex_embedded_python-2.1.2/setup.cfg
+-rw-r--r--   0 grongier (902446405) 1252422112     2016 2023-04-24 18:54:36.000000 iris_pex_embedded_python-2.1.2/setup.py
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-24 18:55:23.692658 iris_pex_embedded_python-2.1.2/src/
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-24 18:55:23.690857 iris_pex_embedded_python-2.1.2/src/grongier/
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-24 18:55:23.707815 iris_pex_embedded_python-2.1.2/src/grongier/iris/
+-rw-r--r--   0 grongier (902446405) 1252422112        0 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.2/src/grongier/iris/__init__.py
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-24 18:55:23.757154 iris_pex_embedded_python-2.1.2/src/grongier/pex/
+-rw-r--r--   0 grongier (902446405) 1252422112     1166 2023-04-18 10:17:07.000000 iris_pex_embedded_python-2.1.2/src/grongier/pex/__init__.py
+-rw-r--r--   0 grongier (902446405) 1252422112    20152 2023-04-21 15:01:34.000000 iris_pex_embedded_python-2.1.2/src/grongier/pex/_business_host.py
+-rw-r--r--   0 grongier (902446405) 1252422112     3509 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.2/src/grongier/pex/_business_operation.py
+-rw-r--r--   0 grongier (902446405) 1252422112    11838 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.2/src/grongier/pex/_business_process.py
+-rw-r--r--   0 grongier (902446405) 1252422112     3735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.2/src/grongier/pex/_business_service.py
+-rw-r--r--   0 grongier (902446405) 1252422112    15107 2023-04-21 08:43:30.000000 iris_pex_embedded_python-2.1.2/src/grongier/pex/_common.py
+-rw-r--r--   0 grongier (902446405) 1252422112     3840 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.2/src/grongier/pex/_director.py
+-rw-r--r--   0 grongier (902446405) 1252422112     1661 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.2/src/grongier/pex/_inbound_adapter.py
+-rw-r--r--   0 grongier (902446405) 1252422112      325 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.2/src/grongier/pex/_message.py
+-rw-r--r--   0 grongier (902446405) 1252422112      735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.2/src/grongier/pex/_outbound_adapter.py
+-rw-r--r--   0 grongier (902446405) 1252422112      331 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.2/src/grongier/pex/_pickle_message.py
+-rw-r--r--   0 grongier (902446405) 1252422112     5033 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.2/src/grongier/pex/_private_session_duplex.py
+-rw-r--r--   0 grongier (902446405) 1252422112     1722 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.1.2/src/grongier/pex/_private_session_process.py
+-rw-r--r--   0 grongier (902446405) 1252422112     7063 2023-04-21 08:18:02.000000 iris_pex_embedded_python-2.1.2/src/grongier/pex/_utils.py
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-04-24 18:55:23.768385 iris_pex_embedded_python-2.1.2/src/iris_pex_embedded_python.egg-info/
+-rw-r--r--   0 grongier (902446405) 1252422112    35813 2023-04-24 18:55:23.000000 iris_pex_embedded_python-2.1.2/src/iris_pex_embedded_python.egg-info/PKG-INFO
+-rw-r--r--   0 grongier (902446405) 1252422112      824 2023-04-24 18:55:23.000000 iris_pex_embedded_python-2.1.2/src/iris_pex_embedded_python.egg-info/SOURCES.txt
+-rw-r--r--   0 grongier (902446405) 1252422112        1 2023-04-24 18:55:23.000000 iris_pex_embedded_python-2.1.2/src/iris_pex_embedded_python.egg-info/dependency_links.txt
+-rw-r--r--   0 grongier (902446405) 1252422112       14 2023-04-24 18:55:23.000000 iris_pex_embedded_python-2.1.2/src/iris_pex_embedded_python.egg-info/requires.txt
+-rw-r--r--   0 grongier (902446405) 1252422112        9 2023-04-24 18:55:23.000000 iris_pex_embedded_python-2.1.2/src/iris_pex_embedded_python.egg-info/top_level.txt
```

### Comparing `iris_pex_embedded_python-2.1.1/LICENSE` & `iris_pex_embedded_python-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.1.1/PKG-INFO` & `iris_pex_embedded_python-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iris_pex_embedded_python
-Version: 2.1.1
+Version: 2.1.2
 Summary: iris_pex_embedded_python
 Home-page: https://github.com/grongierisc/interoperability-embedded-python
 Author: grongier
 Author-email: guillaume.rongier@intersystems.com
 License: MIT
 Keywords: iris_pex_embedded_python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `iris_pex_embedded_python-2.1.1/README.md` & `iris_pex_embedded_python-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.1.1/setup.py` & `iris_pex_embedded_python-2.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     # Do the setup
     setup(
         name='iris_pex_embedded_python',
         description='iris_pex_embedded_python',
         long_description=long_description,
         long_description_content_type='text/markdown',
-        version='2.1.1',
+        version='2.1.2',
         author='grongier',
         author_email='guillaume.rongier@intersystems.com',
         keywords='iris_pex_embedded_python',
         url='https://github.com/grongierisc/interoperability-embedded-python',
         license='MIT',
         classifiers=[
             'Development Status :: 5 - Production/Stable',
```

### Comparing `iris_pex_embedded_python-2.1.1/src/grongier/pex/__init__.py` & `iris_pex_embedded_python-2.1.2/src/grongier/pex/__init__.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.1.1/src/grongier/pex/_business_host.py` & `iris_pex_embedded_python-2.1.2/src/grongier/pex/_business_host.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.1.1/src/grongier/pex/_business_operation.py` & `iris_pex_embedded_python-2.1.2/src/grongier/pex/_business_operation.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.1.1/src/grongier/pex/_business_process.py` & `iris_pex_embedded_python-2.1.2/src/grongier/pex/_business_process.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.1.1/src/grongier/pex/_business_service.py` & `iris_pex_embedded_python-2.1.2/src/grongier/pex/_business_service.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.1.1/src/grongier/pex/_common.py` & `iris_pex_embedded_python-2.1.2/src/grongier/pex/_common.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.1.1/src/grongier/pex/_director.py` & `iris_pex_embedded_python-2.1.2/src/grongier/pex/_director.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.1.1/src/grongier/pex/_inbound_adapter.py` & `iris_pex_embedded_python-2.1.2/src/grongier/pex/_inbound_adapter.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.1.1/src/grongier/pex/_outbound_adapter.py` & `iris_pex_embedded_python-2.1.2/src/grongier/pex/_outbound_adapter.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.1.1/src/grongier/pex/_private_session_duplex.py` & `iris_pex_embedded_python-2.1.2/src/grongier/pex/_private_session_duplex.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.1.1/src/grongier/pex/_private_session_process.py` & `iris_pex_embedded_python-2.1.2/src/grongier/pex/_private_session_process.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.1.1/src/grongier/pex/_utils.py` & `iris_pex_embedded_python-2.1.2/src/grongier/pex/_utils.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.1.1/src/iris_pex_embedded_python.egg-info/PKG-INFO` & `iris_pex_embedded_python-2.1.2/src/iris_pex_embedded_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iris-pex-embedded-python
-Version: 2.1.1
+Version: 2.1.2
 Summary: iris_pex_embedded_python
 Home-page: https://github.com/grongierisc/interoperability-embedded-python
 Author: grongier
 Author-email: guillaume.rongier@intersystems.com
 License: MIT
 Keywords: iris_pex_embedded_python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `iris_pex_embedded_python-2.1.1/src/iris_pex_embedded_python.egg-info/SOURCES.txt` & `iris_pex_embedded_python-2.1.2/src/iris_pex_embedded_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*


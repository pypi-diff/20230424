# Comparing `tmp/openziti-0.7.6.tar.gz` & `tmp/openziti-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openziti-0.7.6.tar", last modified: Thu Mar 23 14:05:54 2023, max compression
+gzip compressed data, was "openziti-0.7.7.tar", last modified: Mon Apr 24 17:37:04 2023, max compression
```

## Comparing `openziti-0.7.6.tar` & `openziti-0.7.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 14:05:54.381090 openziti-0.7.6/
--rw-r--r--   0 runner    (1001) docker     (122)    11340 2023-03-23 14:05:46.000000 openziti-0.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-03-23 14:05:46.000000 openziti-0.7.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2062 2023-03-23 14:05:54.381090 openziti-0.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1176 2023-03-23 14:05:46.000000 openziti-0.7.6/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-03-23 14:05:54.381090 openziti-0.7.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3214 2023-03-23 14:05:46.000000 openziti-0.7.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 14:05:54.377090 openziti-0.7.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 14:05:54.381090 openziti-0.7.6/src/openziti/
--rw-r--r--   0 runner    (1001) docker     (122)     1178 2023-03-23 14:05:46.000000 openziti-0.7.6/src/openziti/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1617 2023-03-23 14:05:46.000000 openziti-0.7.6/src/openziti/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-03-23 14:05:54.381090 openziti-0.7.6/src/openziti/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     3231 2023-03-23 14:05:46.000000 openziti-0.7.6/src/openziti/context.py
--rw-r--r--   0 runner    (1001) docker     (122)     2599 2023-03-23 14:05:46.000000 openziti-0.7.6/src/openziti/decor.py
--rw-r--r--   0 runner    (1001) docker     (122)     9279 2023-03-23 14:05:46.000000 openziti-0.7.6/src/openziti/zitilib.py
--rw-r--r--   0 runner    (1001) docker     (122)     3860 2023-03-23 14:05:46.000000 openziti-0.7.6/src/openziti/zitisock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-23 14:05:54.381090 openziti-0.7.6/src/openziti.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2062 2023-03-23 14:05:54.000000 openziti-0.7.6/src/openziti.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      376 2023-03-23 14:05:54.000000 openziti-0.7.6/src/openziti.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-23 14:05:54.000000 openziti-0.7.6/src/openziti.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-03-23 14:05:54.000000 openziti-0.7.6/src/openziti.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    81180 2023-03-23 14:05:46.000000 openziti-0.7.6/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 17:37:04.670298 openziti-0.7.7/
+-rw-r--r--   0 runner    (1001) docker     (122)    11340 2023-04-24 17:36:48.000000 openziti-0.7.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-04-24 17:36:48.000000 openziti-0.7.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6885 2023-04-24 17:37:04.670298 openziti-0.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5999 2023-04-24 17:36:48.000000 openziti-0.7.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-04-24 17:37:04.674298 openziti-0.7.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3214 2023-04-24 17:36:48.000000 openziti-0.7.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 17:37:04.666298 openziti-0.7.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 17:37:04.674298 openziti-0.7.7/src/openziti/
+-rw-r--r--   0 runner    (1001) docker     (122)     1178 2023-04-24 17:36:48.000000 openziti-0.7.7/src/openziti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2234 2023-04-24 17:36:48.000000 openziti-0.7.7/src/openziti/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-04-24 17:37:04.674298 openziti-0.7.7/src/openziti/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3231 2023-04-24 17:36:48.000000 openziti-0.7.7/src/openziti/context.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2599 2023-04-24 17:36:48.000000 openziti-0.7.7/src/openziti/decor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-04-24 17:36:48.000000 openziti-0.7.7/src/openziti/zitilib.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3860 2023-04-24 17:36:48.000000 openziti-0.7.7/src/openziti/zitisock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-24 17:37:04.670298 openziti-0.7.7/src/openziti.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6885 2023-04-24 17:37:04.000000 openziti-0.7.7/src/openziti.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      376 2023-04-24 17:37:04.000000 openziti-0.7.7/src/openziti.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-24 17:37:04.000000 openziti-0.7.7/src/openziti.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-04-24 17:37:04.000000 openziti-0.7.7/src/openziti.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    81180 2023-04-24 17:36:48.000000 openziti-0.7.7/versioneer.py
```

### Comparing `openziti-0.7.6/LICENSE` & `openziti-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `openziti-0.7.6/setup.cfg` & `openziti-0.7.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -34,13 +34,13 @@
 style = pep440-pre
 versionfile_source = src/openziti/_version.py
 versionfile_build = openziti/_version.py
 tag_prefix = v
 parentdir_prefix = openziti-
 
 [openziti]
-ziti_sdk_version = 0.31.5
+ziti_sdk_version = 0.32.2
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `openziti-0.7.6/setup.py` & `openziti-0.7.7/setup.py`

 * *Files identical despite different names*

### Comparing `openziti-0.7.6/src/openziti/__init__.py` & `openziti-0.7.7/src/openziti/__init__.py`

 * *Files identical despite different names*

### Comparing `openziti-0.7.6/src/openziti/context.py` & `openziti-0.7.7/src/openziti/context.py`

 * *Files identical despite different names*

### Comparing `openziti-0.7.6/src/openziti/decor.py` & `openziti-0.7.7/src/openziti/decor.py`

 * *Files identical despite different names*

### Comparing `openziti-0.7.6/src/openziti/zitilib.py` & `openziti-0.7.7/src/openziti/zitilib.py`

 * *Files 4% similar despite different names*

```diff
@@ -225,15 +225,16 @@
 
 def ziti_socket(type):
     fd = _ziti_socket(type)
     return fd
 
 
 def ziti_close(fd):
-    _ziti_close(fd)
+    if fd:
+        _ziti_close(fd)
 
 
 def shutdown():
     ziti.Ziti_lib_shutdown()
 
 
 def load(path):
@@ -293,15 +294,19 @@
         with open(jwt, 'rb') as jwt_f:
             jwtc = bytes(jwt_f.read())
     except:
         jwtc = bytes(jwt, 'utf-8')
 
     id_json = ctypes.c_char_p()
     id_json_len = ctypes.c_size_t()
-    retcode = _ziti_enroll(jwtc, key, cert,
+
+    keyb = None if key is None else bytes(key, 'utf-8')
+    certb = None if cert is None else bytes(cert, 'utf-8')
+
+    retcode = _ziti_enroll(jwtc, keyb, certb,
                            ctypes.byref(id_json),
                            ctypes.byref(id_json_len))
     if retcode != 0:
         raise RuntimeError(errorstr(retcode))
     try:
         return id_json.value.decode()
     finally:
```

### Comparing `openziti-0.7.6/src/openziti/zitisock.py` & `openziti-0.7.7/src/openziti/zitisock.py`

 * *Files identical despite different names*

### Comparing `openziti-0.7.6/versioneer.py` & `openziti-0.7.7/versioneer.py`

 * *Files identical despite different names*


# Comparing `tmp/pmserializer-2.0.3.tar.gz` & `tmp/pmserializer-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmserializer-2.0.3.tar", last modified: Sat Apr 22 07:30:12 2023, max compression
+gzip compressed data, was "pmserializer-2.0.4.tar", last modified: Mon Apr 24 16:04:14 2023, max compression
```

## Comparing `pmserializer-2.0.3.tar` & `pmserializer-2.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 07:30:12.589366 pmserializer-2.0.3/
--rw-rw-rw-   0        0        0      221 2023-04-22 07:30:12.588367 pmserializer-2.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-22 07:30:12.557282 pmserializer-2.0.3/lab3/
--rw-rw-rw-   0        0        0     4534 2023-04-21 14:44:58.000000 pmserializer-2.0.3/lab3/DeserializerJson.py
--rw-rw-rw-   0        0        0     3857 2023-04-21 14:39:00.000000 pmserializer-2.0.3/lab3/DeserializerYaml.py
--rw-rw-rw-   0        0        0      641 2023-04-21 14:44:58.000000 pmserializer-2.0.3/lab3/Json.py
--rw-rw-rw-   0        0        0      367 2023-04-21 14:44:58.000000 pmserializer-2.0.3/lab3/SerializerFactory.py
--rw-rw-rw-   0        0        0     7068 2023-04-21 14:44:58.000000 pmserializer-2.0.3/lab3/SerializerJson.py
--rw-rw-rw-   0        0        0     5514 2023-04-21 14:44:58.000000 pmserializer-2.0.3/lab3/SerializerYaml.py
--rw-rw-rw-   0        0        0      689 2023-04-21 14:44:58.000000 pmserializer-2.0.3/lab3/Toml.py
--rw-rw-rw-   0        0        0      676 2023-04-21 14:44:58.000000 pmserializer-2.0.3/lab3/Yaml.py
--rw-rw-rw-   0        0        0      113 2023-04-22 07:25:28.000000 pmserializer-2.0.3/lab3/__init__.py
--rw-rw-rw-   0        0        0      279 2023-04-21 14:39:00.000000 pmserializer-2.0.3/lab3/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-22 07:30:12.587369 pmserializer-2.0.3/pmserializer.egg-info/
--rw-rw-rw-   0        0        0      221 2023-04-22 07:30:12.000000 pmserializer-2.0.3/pmserializer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-04-22 07:30:12.000000 pmserializer-2.0.3/pmserializer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 07:30:12.000000 pmserializer-2.0.3/pmserializer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-22 07:30:12.000000 pmserializer-2.0.3/pmserializer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-22 07:30:12.000000 pmserializer-2.0.3/pmserializer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 07:30:12.590361 pmserializer-2.0.3/setup.cfg
--rw-rw-rw-   0        0        0      289 2023-04-22 07:30:06.000000 pmserializer-2.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 16:04:14.098863 pmserializer-2.0.4/
+-rw-rw-rw-   0        0        0      253 2023-04-24 16:04:14.098863 pmserializer-2.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-24 16:04:14.086716 pmserializer-2.0.4/lab3/
+-rw-rw-rw-   0        0        0     4534 2023-04-21 14:44:58.000000 pmserializer-2.0.4/lab3/DeserializerJson.py
+-rw-rw-rw-   0        0        0     3857 2023-04-21 14:39:00.000000 pmserializer-2.0.4/lab3/DeserializerYaml.py
+-rw-rw-rw-   0        0        0      641 2023-04-21 14:44:58.000000 pmserializer-2.0.4/lab3/Json.py
+-rw-rw-rw-   0        0        0      367 2023-04-21 14:44:58.000000 pmserializer-2.0.4/lab3/SerializerFactory.py
+-rw-rw-rw-   0        0        0     7068 2023-04-21 14:44:58.000000 pmserializer-2.0.4/lab3/SerializerJson.py
+-rw-rw-rw-   0        0        0     5514 2023-04-21 14:44:58.000000 pmserializer-2.0.4/lab3/SerializerYaml.py
+-rw-rw-rw-   0        0        0      689 2023-04-21 14:44:58.000000 pmserializer-2.0.4/lab3/Toml.py
+-rw-rw-rw-   0        0        0      676 2023-04-21 14:44:58.000000 pmserializer-2.0.4/lab3/Yaml.py
+-rw-rw-rw-   0        0        0      113 2023-04-22 07:25:28.000000 pmserializer-2.0.4/lab3/__init__.py
+-rw-rw-rw-   0        0        0      279 2023-04-21 14:39:00.000000 pmserializer-2.0.4/lab3/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-24 16:04:14.098863 pmserializer-2.0.4/pmserializer.egg-info/
+-rw-rw-rw-   0        0        0      253 2023-04-24 16:04:13.000000 pmserializer-2.0.4/pmserializer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-04-24 16:04:13.000000 pmserializer-2.0.4/pmserializer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 16:04:13.000000 pmserializer-2.0.4/pmserializer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-24 16:04:13.000000 pmserializer-2.0.4/pmserializer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-24 16:04:13.000000 pmserializer-2.0.4/pmserializer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 16:04:14.098863 pmserializer-2.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      340 2023-04-24 16:04:02.000000 pmserializer-2.0.4/setup.py
```

### Comparing `pmserializer-2.0.3/lab3/DeserializerJson.py` & `pmserializer-2.0.4/lab3/DeserializerJson.py`

 * *Files identical despite different names*

### Comparing `pmserializer-2.0.3/lab3/DeserializerYaml.py` & `pmserializer-2.0.4/lab3/DeserializerYaml.py`

 * *Files identical despite different names*

### Comparing `pmserializer-2.0.3/lab3/Json.py` & `pmserializer-2.0.4/lab3/Json.py`

 * *Files identical despite different names*

### Comparing `pmserializer-2.0.3/lab3/SerializerJson.py` & `pmserializer-2.0.4/lab3/SerializerJson.py`

 * *Files identical despite different names*

### Comparing `pmserializer-2.0.3/lab3/SerializerYaml.py` & `pmserializer-2.0.4/lab3/SerializerYaml.py`

 * *Files identical despite different names*

### Comparing `pmserializer-2.0.3/lab3/Toml.py` & `pmserializer-2.0.4/lab3/Toml.py`

 * *Files identical despite different names*

### Comparing `pmserializer-2.0.3/lab3/Yaml.py` & `pmserializer-2.0.4/lab3/Yaml.py`

 * *Files identical despite different names*


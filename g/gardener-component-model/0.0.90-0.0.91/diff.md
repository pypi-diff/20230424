# Comparing `tmp/gardener-component-model-0.0.90.tar.gz` & `tmp/gardener-component-model-0.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener-component-model-0.0.90.tar", last modified: Tue Apr 11 13:53:52 2023, max compression
+gzip compressed data, was "gardener-component-model-0.0.91.tar", last modified: Mon Apr 24 12:16:36 2023, max compression
```

## Comparing `gardener-component-model-0.0.90.tar` & `gardener-component-model-0.0.91.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:53:52.321206 gardener-component-model-0.0.90/
--rw-r--r--   0 root         (0) root         (0)      126 2023-04-11 13:53:52.321206 gardener-component-model-0.0.90/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:53:52.321206 gardener-component-model-0.0.90/gardener_component_model.egg-info/
--rw-r--r--   0 root         (0) root         (0)      126 2023-04-11 13:53:52.000000 gardener-component-model-0.0.90/gardener_component_model.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      338 2023-04-11 13:53:52.000000 gardener-component-model-0.0.90/gardener_component_model.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 13:53:52.000000 gardener-component-model-0.0.90/gardener_component_model.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       41 2023-04-11 13:53:52.000000 gardener-component-model-0.0.90/gardener_component_model.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-04-11 13:53:52.000000 gardener-component-model-0.0.90/gardener_component_model.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:53:52.321206 gardener-component-model-0.0.90/gci/
--rw-r--r--   0 root         (0) root         (0)      165 2023-04-11 13:53:18.000000 gardener-component-model-0.0.90/gci/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10026 2023-04-11 13:53:19.000000 gardener-component-model-0.0.90/gci/component-descriptor.json-schema.yaml
--rw-r--r--   0 root         (0) root         (0)    17809 2023-04-11 13:53:18.000000 gardener-component-model-0.0.90/gci/componentmodel.py
--rw-r--r--   0 root         (0) root         (0)     3021 2023-04-11 13:53:18.000000 gardener-component-model-0.0.90/gci/oci.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 13:53:52.321206 gardener-component-model-0.0.90/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      942 2023-04-11 13:53:18.000000 gardener-component-model-0.0.90/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:16:36.413985 gardener-component-model-0.0.91/
+-rw-r--r--   0 root         (0) root         (0)      126 2023-04-24 12:16:36.413985 gardener-component-model-0.0.91/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:16:36.413985 gardener-component-model-0.0.91/gardener_component_model.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      126 2023-04-24 12:16:36.000000 gardener-component-model-0.0.91/gardener_component_model.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      338 2023-04-24 12:16:36.000000 gardener-component-model-0.0.91/gardener_component_model.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 12:16:36.000000 gardener-component-model-0.0.91/gardener_component_model.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-04-24 12:16:36.000000 gardener-component-model-0.0.91/gardener_component_model.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-24 12:16:36.000000 gardener-component-model-0.0.91/gardener_component_model.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 12:16:36.413985 gardener-component-model-0.0.91/gci/
+-rw-r--r--   0 root         (0) root         (0)      165 2023-04-24 12:16:00.000000 gardener-component-model-0.0.91/gci/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10026 2023-04-24 12:16:01.000000 gardener-component-model-0.0.91/gci/component-descriptor.json-schema.yaml
+-rw-r--r--   0 root         (0) root         (0)    17820 2023-04-24 12:16:00.000000 gardener-component-model-0.0.91/gci/componentmodel.py
+-rw-r--r--   0 root         (0) root         (0)     3021 2023-04-24 12:16:00.000000 gardener-component-model-0.0.91/gci/oci.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 12:16:36.413985 gardener-component-model-0.0.91/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      942 2023-04-24 12:16:00.000000 gardener-component-model-0.0.91/setup.py
```

### Comparing `gardener-component-model-0.0.90/gci/component-descriptor.json-schema.yaml` & `gardener-component-model-0.0.91/gci/component-descriptor.json-schema.yaml`

 * *Files identical despite different names*

### Comparing `gardener-component-model-0.0.90/gci/componentmodel.py` & `gardener-component-model-0.0.91/gci/componentmodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -448,15 +448,19 @@
     def component_version_oci_ref(
         self,
         name: typing.Union[str, 'Component', 'ComponentIdentity'],
         version: str=None,
     ):
         if isinstance(name, Component):
             name = name.name
+            if not version:
+                version = name.version
         elif isinstance(name, ComponentIdentity):
+            if not version:
+                version = name.version
             name = name.name
 
         if not version:
             name, version = name.rsplit(':', 1)
 
         return f'{self.component_oci_ref(name)}:{version}'
 
@@ -597,10 +601,8 @@
 class EnumValueYamlDumper(yaml.SafeDumper):
     '''
     a yaml.SafeDumper that will dump enum objects using their values
     '''
     def represent_data(self, data):
         if isinstance(data, enum.Enum):
             return self.represent_data(data.value)
-        if isinstance(data, datetime.datetime):
-            return self.represent_data(data.isoformat(timespec='seconds'))
         return super().represent_data(data)
```

### Comparing `gardener-component-model-0.0.90/gci/oci.py` & `gardener-component-model-0.0.91/gci/oci.py`

 * *Files identical despite different names*

### Comparing `gardener-component-model-0.0.90/setup.py` & `gardener-component-model-0.0.91/setup.py`

 * *Files identical despite different names*


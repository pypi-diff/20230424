# Comparing `tmp/apf_base-2.1.4.tar.gz` & `tmp/apf_base-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/APF/APF/dist/.tmp-x7lhr3tt/apf_base-2.1.4.tar", last modified: Thu Mar  2 20:47:21 2023, max compression
+gzip compressed data, was "/home/runner/work/APF/APF/dist/.tmp-8suq76lh/apf_base-2.1.5.tar", last modified: Mon Mar  6 19:34:43 2023, max compression
```

## Comparing `apf_base-2.1.4.tar` & `apf_base-2.1.5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:47:21.000000 apf_base-2.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-03-02 20:46:50.000000 apf_base-2.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-03-02 20:47:21.000000 apf_base-2.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-03-02 20:46:50.000000 apf_base-2.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:47:21.000000 apf_base-2.1.4/apf/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:47:21.000000 apf_base-2.1.4/apf/consumers/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-02 20:46:50.000000 apf_base-2.1.4/apf/consumers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-03-02 20:46:50.000000 apf_base-2.1.4/apf/consumers/avro_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-03-02 20:46:50.000000 apf_base-2.1.4/apf/consumers/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-03-02 20:46:50.000000 apf_base-2.1.4/apf/consumers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-03-02 20:46:50.000000 apf_base-2.1.4/apf/consumers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-03-02 20:46:50.000000 apf_base-2.1.4/apf/consumers/kafka.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:47:21.000000 apf_base-2.1.4/apf/core/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-03-02 20:46:50.000000 apf_base-2.1.4/apf/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:47:21.000000 apf_base-2.1.4/apf/core/management/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-02 20:46:50.000000 apf_base-2.1.4/apf/core/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-03-02 20:46:50.000000 apf_base-2.1.4/apf/core/management/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-02 20:46:50.000000 apf_base-2.1.4/apf/core/secret_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    13635 2023-03-02 20:46:50.000000 apf_base-2.1.4/apf/core/step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:47:21.000000 apf_base-2.1.4/apf/core/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:47:21.000000 apf_base-2.1.4/apf/core/templates/step/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-02 20:46:50.000000 apf_base-2.1.4/apf/core/templates/step/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:47:21.000000 apf_base-2.1.4/apf/core/templates/step/package/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-02 20:46:50.000000 apf_base-2.1.4/apf/core/templates/step/package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-03-02 20:46:50.000000 apf_base-2.1.4/apf/core/templates/step/package/step.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-02 20:46:50.000000 apf_base-2.1.4/apf/core/templates/step/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:47:21.000000 apf_base-2.1.4/apf/core/templates/step/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-02 20:46:50.000000 apf_base-2.1.4/apf/core/templates/step/scripts/run_step.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-03-02 20:46:50.000000 apf_base-2.1.4/apf/core/templates/step/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 20:46:50.000000 apf_base-2.1.4/apf/core/templates/step/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-03-02 20:46:50.000000 apf_base-2.1.4/apf/core/topic_management.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:47:21.000000 apf_base-2.1.4/apf/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-02 20:46:50.000000 apf_base-2.1.4/apf/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-03-02 20:46:50.000000 apf_base-2.1.4/apf/metrics/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-03-02 20:46:50.000000 apf_base-2.1.4/apf/metrics/kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-03-02 20:46:50.000000 apf_base-2.1.4/apf/metrics/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:47:21.000000 apf_base-2.1.4/apf/metrics/prometheus/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-02 20:46:50.000000 apf_base-2.1.4/apf/metrics/prometheus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-02 20:46:50.000000 apf_base-2.1.4/apf/metrics/prometheus/prometheus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:47:21.000000 apf_base-2.1.4/apf/producers/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-02 20:46:50.000000 apf_base-2.1.4/apf/producers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-03-02 20:46:50.000000 apf_base-2.1.4/apf/producers/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-03-02 20:46:50.000000 apf_base-2.1.4/apf/producers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-03-02 20:46:50.000000 apf_base-2.1.4/apf/producers/json_prod.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-03-02 20:46:50.000000 apf_base-2.1.4/apf/producers/kafka.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:47:21.000000 apf_base-2.1.4/apf_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-03-02 20:47:21.000000 apf_base-2.1.4/apf_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-03-02 20:47:21.000000 apf_base-2.1.4/apf_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 20:47:21.000000 apf_base-2.1.4/apf_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-03-02 20:47:21.000000 apf_base-2.1.4/apf_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-02 20:47:21.000000 apf_base-2.1.4/apf_base.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:47:21.000000 apf_base-2.1.4/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-03-02 20:46:50.000000 apf_base-2.1.4/scripts/apf
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-02 20:47:21.000000 apf_base-2.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-03-02 20:46:50.000000 apf_base-2.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:34:43.000000 apf_base-2.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-03-06 19:34:17.000000 apf_base-2.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-03-06 19:34:43.000000 apf_base-2.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-03-06 19:34:17.000000 apf_base-2.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:34:43.000000 apf_base-2.1.5/apf/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:34:43.000000 apf_base-2.1.5/apf/consumers/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/consumers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/consumers/avro_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/consumers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/consumers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/consumers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/consumers/kafka.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:34:43.000000 apf_base-2.1.5/apf/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:34:43.000000 apf_base-2.1.5/apf/core/management/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/core/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/core/management/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/core/secret_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13635 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/core/step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:34:43.000000 apf_base-2.1.5/apf/core/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:34:43.000000 apf_base-2.1.5/apf/core/templates/step/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/core/templates/step/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:34:43.000000 apf_base-2.1.5/apf/core/templates/step/package/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/core/templates/step/package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/core/templates/step/package/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/core/templates/step/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:34:43.000000 apf_base-2.1.5/apf/core/templates/step/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/core/templates/step/scripts/run_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/core/templates/step/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/core/templates/step/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/core/topic_management.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:34:43.000000 apf_base-2.1.5/apf/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/metrics/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/metrics/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/metrics/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:34:43.000000 apf_base-2.1.5/apf/metrics/prometheus/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/metrics/prometheus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/metrics/prometheus/prometheus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:34:43.000000 apf_base-2.1.5/apf/producers/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/producers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/producers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/producers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/producers/json_prod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-03-06 19:34:17.000000 apf_base-2.1.5/apf/producers/kafka.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:34:43.000000 apf_base-2.1.5/apf_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-03-06 19:34:43.000000 apf_base-2.1.5/apf_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-03-06 19:34:43.000000 apf_base-2.1.5/apf_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 19:34:43.000000 apf_base-2.1.5/apf_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-03-06 19:34:43.000000 apf_base-2.1.5/apf_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-06 19:34:43.000000 apf_base-2.1.5/apf_base.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 19:34:43.000000 apf_base-2.1.5/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-03-06 19:34:17.000000 apf_base-2.1.5/scripts/apf
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 19:34:43.000000 apf_base-2.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-03-06 19:34:17.000000 apf_base-2.1.5/setup.py
```

### Comparing `apf_base-2.1.4/LICENSE` & `apf_base-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.4/PKG-INFO` & `apf_base-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apf_base
-Version: 2.1.4
+Version: 2.1.5
 Summary: ALeRCE Alert Processing Framework.
 Author: ALeRCE Team
 Author-email: contact@alerce.online
 Project-URL: Github, https://github.com/alercebroker/APF
 Project-URL: Documentation, https://apf.readthedocs.io/en/latest/index.html
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `apf_base-2.1.4/README.md` & `apf_base-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.4/apf/consumers/avro_file.py` & `apf_base-2.1.5/apf/consumers/avro_file.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.4/apf/consumers/csv.py` & `apf_base-2.1.5/apf/consumers/csv.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.4/apf/consumers/generic.py` & `apf_base-2.1.5/apf/consumers/generic.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.4/apf/consumers/json.py` & `apf_base-2.1.5/apf/consumers/json.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.4/apf/consumers/kafka.py` & `apf_base-2.1.5/apf/consumers/kafka.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.4/apf/core/__init__.py` & `apf_base-2.1.5/apf/core/__init__.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.4/apf/core/management/helpers.py` & `apf_base-2.1.5/apf/core/management/helpers.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.4/apf/core/secret_manager.py` & `apf_base-2.1.5/apf/core/secret_manager.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.4/apf/core/step.py` & `apf_base-2.1.5/apf/core/step.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -203,18 +203,18 @@
         ----------
         message : dict, list
             Dict-like message to be processed or list of dict-like messages
         """
         pass
 
     def _post_execute(self, result: Union[Iterable[Dict[str, Any]], Dict[str, Any]]):
-        if self.commit:
-            self.consumer.commit()
         self.logger.info("Processed message. Begin post processing")
         final_result = self.post_execute(result)
+        if self.commit:
+            self.consumer.commit()
         self.metrics["timestamp_sent"] = datetime.datetime.now(datetime.timezone.utc)
         time_difference = (
             self.metrics["timestamp_sent"] - self.metrics["timestamp_received"]
         )
         self.metrics["execution_time"] = time_difference.total_seconds()
         if self.extra_metrics:
             extra_metrics = self.get_extra_metrics(self.message)
```

### Comparing `apf_base-2.1.4/apf/core/templates/step/package/step.py` & `apf_base-2.1.5/apf/core/templates/step/package/step.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.4/apf/core/templates/step/scripts/run_step.py` & `apf_base-2.1.5/apf/core/templates/step/scripts/run_step.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.4/apf/core/topic_management.py` & `apf_base-2.1.5/apf/core/topic_management.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.4/apf/metrics/generic.py` & `apf_base-2.1.5/apf/metrics/generic.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.4/apf/metrics/kafka.py` & `apf_base-2.1.5/apf/metrics/kafka.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.4/apf/metrics/log.py` & `apf_base-2.1.5/apf/metrics/log.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.4/apf/metrics/prometheus/prometheus.py` & `apf_base-2.1.5/apf/metrics/prometheus/prometheus.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.4/apf/producers/csv.py` & `apf_base-2.1.5/apf/producers/csv.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.4/apf/producers/generic.py` & `apf_base-2.1.5/apf/producers/generic.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.4/apf/producers/json_prod.py` & `apf_base-2.1.5/apf/producers/json_prod.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.4/apf/producers/kafka.py` & `apf_base-2.1.5/apf/producers/kafka.py`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.4/apf_base.egg-info/PKG-INFO` & `apf_base-2.1.5/apf_base.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apf-base
-Version: 2.1.4
+Version: 2.1.5
 Summary: ALeRCE Alert Processing Framework.
 Author: ALeRCE Team
 Author-email: contact@alerce.online
 Project-URL: Github, https://github.com/alercebroker/APF
 Project-URL: Documentation, https://apf.readthedocs.io/en/latest/index.html
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `apf_base-2.1.4/apf_base.egg-info/SOURCES.txt` & `apf_base-2.1.5/apf_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apf_base-2.1.4/setup.py` & `apf_base-2.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="apf_base",
-    version="2.1.4",
+    version="2.1.5",
     description="ALeRCE Alert Processing Framework.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ALeRCE Team",
     author_email="contact@alerce.online",
     packages=find_namespace_packages(include=["apf.*"]),
     scripts=["scripts/apf"],
```


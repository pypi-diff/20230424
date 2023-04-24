# Comparing `tmp/eppo-server-sdk-1.0.4.tar.gz` & `tmp/eppo-server-sdk-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eppo-server-sdk-1.0.4.tar", last modified: Mon Aug  8 15:41:38 2022, max compression
+gzip compressed data, was "eppo-server-sdk-1.1.1.tar", last modified: Fri Sep 16 23:06:22 2022, max compression
```

## Comparing `eppo-server-sdk-1.0.4.tar` & `eppo-server-sdk-1.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 ploomis    (501) staff       (20)        0 2022-08-08 15:41:38.705644 eppo-server-sdk-1.0.4/
--rw-r--r--   0 ploomis    (501) staff       (20)     1071 2022-05-04 03:03:00.000000 eppo-server-sdk-1.0.4/LICENSE
--rw-r--r--   0 ploomis    (501) staff       (20)       88 2022-05-06 16:40:59.000000 eppo-server-sdk-1.0.4/MANIFEST.in
--rw-r--r--   0 ploomis    (501) staff       (20)      760 2022-08-08 15:41:38.705726 eppo-server-sdk-1.0.4/PKG-INFO
--rw-r--r--   0 ploomis    (501) staff       (20)      269 2022-06-15 17:53:51.000000 eppo-server-sdk-1.0.4/README.md
-drwxr-xr-x   0 ploomis    (501) staff       (20)        0 2022-08-08 15:41:38.704421 eppo-server-sdk-1.0.4/eppo_client/
--rw-r--r--   0 ploomis    (501) staff       (20)     2507 2022-08-08 15:34:49.000000 eppo-server-sdk-1.0.4/eppo_client/__init__.py
--rw-r--r--   0 ploomis    (501) staff       (20)      117 2022-06-27 14:59:22.000000 eppo-server-sdk-1.0.4/eppo_client/assignment_logger.py
--rw-r--r--   0 ploomis    (501) staff       (20)      326 2022-05-04 03:03:00.000000 eppo-server-sdk-1.0.4/eppo_client/base_model.py
--rw-r--r--   0 ploomis    (501) staff       (20)     4643 2022-07-11 20:58:37.000000 eppo-server-sdk-1.0.4/eppo_client/client.py
--rw-r--r--   0 ploomis    (501) staff       (20)      512 2022-07-11 20:58:37.000000 eppo-server-sdk-1.0.4/eppo_client/config.py
--rw-r--r--   0 ploomis    (501) staff       (20)     2019 2022-06-15 17:53:51.000000 eppo-server-sdk-1.0.4/eppo_client/configuration_requestor.py
--rw-r--r--   0 ploomis    (501) staff       (20)      868 2022-05-06 17:32:51.000000 eppo-server-sdk-1.0.4/eppo_client/configuration_store.py
--rw-r--r--   0 ploomis    (501) staff       (20)      249 2022-05-06 17:33:05.000000 eppo-server-sdk-1.0.4/eppo_client/constants.py
--rw-r--r--   0 ploomis    (501) staff       (20)     2395 2022-05-06 17:31:04.000000 eppo-server-sdk-1.0.4/eppo_client/http_client.py
--rw-r--r--   0 ploomis    (501) staff       (20)     1130 2022-05-06 17:31:04.000000 eppo-server-sdk-1.0.4/eppo_client/poller.py
--rw-r--r--   0 ploomis    (501) staff       (20)     1222 2022-05-06 16:40:59.000000 eppo-server-sdk-1.0.4/eppo_client/read_write_lock.py
--rw-r--r--   0 ploomis    (501) staff       (20)     2175 2022-08-08 15:34:49.000000 eppo-server-sdk-1.0.4/eppo_client/rules.py
--rw-r--r--   0 ploomis    (501) staff       (20)      618 2022-05-04 03:03:00.000000 eppo-server-sdk-1.0.4/eppo_client/shard.py
--rw-r--r--   0 ploomis    (501) staff       (20)      193 2022-05-04 03:03:00.000000 eppo-server-sdk-1.0.4/eppo_client/validation.py
-drwxr-xr-x   0 ploomis    (501) staff       (20)        0 2022-08-08 15:41:38.705523 eppo-server-sdk-1.0.4/eppo_server_sdk.egg-info/
--rw-r--r--   0 ploomis    (501) staff       (20)      760 2022-08-08 15:41:38.000000 eppo-server-sdk-1.0.4/eppo_server_sdk.egg-info/PKG-INFO
--rw-r--r--   0 ploomis    (501) staff       (20)      661 2022-08-08 15:41:38.000000 eppo-server-sdk-1.0.4/eppo_server_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 ploomis    (501) staff       (20)        1 2022-08-08 15:41:38.000000 eppo-server-sdk-1.0.4/eppo_server_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 ploomis    (501) staff       (20)       29 2022-08-08 15:41:38.000000 eppo-server-sdk-1.0.4/eppo_server_sdk.egg-info/requires.txt
--rw-r--r--   0 ploomis    (501) staff       (20)       12 2022-08-08 15:41:38.000000 eppo-server-sdk-1.0.4/eppo_server_sdk.egg-info/top_level.txt
--rw-r--r--   0 ploomis    (501) staff       (20)       84 2022-04-28 02:07:07.000000 eppo-server-sdk-1.0.4/pyproject.toml
--rw-r--r--   0 ploomis    (501) staff       (20)       46 2022-06-20 22:49:01.000000 eppo-server-sdk-1.0.4/requirements-test.txt
--rw-r--r--   0 ploomis    (501) staff       (20)       61 2022-06-20 22:49:01.000000 eppo-server-sdk-1.0.4/requirements.txt
--rw-r--r--   0 ploomis    (501) staff       (20)      667 2022-08-08 15:41:38.706025 eppo-server-sdk-1.0.4/setup.cfg
+drwxr-xr-x   0 ploomis    (501) staff       (20)        0 2022-09-16 23:06:22.370704 eppo-server-sdk-1.1.1/
+-rw-r--r--   0 ploomis    (501) staff       (20)     1071 2022-05-04 03:03:00.000000 eppo-server-sdk-1.1.1/LICENSE
+-rw-r--r--   0 ploomis    (501) staff       (20)       88 2022-05-06 16:40:59.000000 eppo-server-sdk-1.1.1/MANIFEST.in
+-rw-r--r--   0 ploomis    (501) staff       (20)      760 2022-09-16 23:06:22.370790 eppo-server-sdk-1.1.1/PKG-INFO
+-rw-r--r--   0 ploomis    (501) staff       (20)      269 2022-06-15 17:53:51.000000 eppo-server-sdk-1.1.1/README.md
+drwxr-xr-x   0 ploomis    (501) staff       (20)        0 2022-09-16 23:06:22.364459 eppo-server-sdk-1.1.1/eppo_client/
+-rw-r--r--   0 ploomis    (501) staff       (20)     2507 2022-09-16 22:24:12.000000 eppo-server-sdk-1.1.1/eppo_client/__init__.py
+-rw-r--r--   0 ploomis    (501) staff       (20)      117 2022-06-27 14:59:22.000000 eppo-server-sdk-1.1.1/eppo_client/assignment_logger.py
+-rw-r--r--   0 ploomis    (501) staff       (20)      326 2022-05-04 03:03:00.000000 eppo-server-sdk-1.1.1/eppo_client/base_model.py
+-rw-r--r--   0 ploomis    (501) staff       (20)     4946 2022-09-16 20:27:28.000000 eppo-server-sdk-1.1.1/eppo_client/client.py
+-rw-r--r--   0 ploomis    (501) staff       (20)      512 2022-07-11 20:58:37.000000 eppo-server-sdk-1.1.1/eppo_client/config.py
+-rw-r--r--   0 ploomis    (501) staff       (20)     1914 2022-09-16 22:24:12.000000 eppo-server-sdk-1.1.1/eppo_client/configuration_requestor.py
+-rw-r--r--   0 ploomis    (501) staff       (20)      868 2022-05-06 17:32:51.000000 eppo-server-sdk-1.1.1/eppo_client/configuration_store.py
+-rw-r--r--   0 ploomis    (501) staff       (20)      249 2022-05-06 17:33:05.000000 eppo-server-sdk-1.1.1/eppo_client/constants.py
+-rw-r--r--   0 ploomis    (501) staff       (20)     2107 2022-09-16 22:24:12.000000 eppo-server-sdk-1.1.1/eppo_client/http_client.py
+-rw-r--r--   0 ploomis    (501) staff       (20)     1130 2022-05-06 17:31:04.000000 eppo-server-sdk-1.1.1/eppo_client/poller.py
+-rw-r--r--   0 ploomis    (501) staff       (20)     1222 2022-05-06 16:40:59.000000 eppo-server-sdk-1.1.1/eppo_client/read_write_lock.py
+-rw-r--r--   0 ploomis    (501) staff       (20)     2200 2022-09-16 20:27:28.000000 eppo-server-sdk-1.1.1/eppo_client/rules.py
+-rw-r--r--   0 ploomis    (501) staff       (20)      618 2022-05-04 03:03:00.000000 eppo-server-sdk-1.1.1/eppo_client/shard.py
+-rw-r--r--   0 ploomis    (501) staff       (20)      193 2022-05-04 03:03:00.000000 eppo-server-sdk-1.1.1/eppo_client/validation.py
+drwxr-xr-x   0 ploomis    (501) staff       (20)        0 2022-09-16 23:06:22.370590 eppo-server-sdk-1.1.1/eppo_server_sdk.egg-info/
+-rw-r--r--   0 ploomis    (501) staff       (20)      760 2022-09-16 23:06:22.000000 eppo-server-sdk-1.1.1/eppo_server_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 ploomis    (501) staff       (20)      661 2022-09-16 23:06:22.000000 eppo-server-sdk-1.1.1/eppo_server_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 ploomis    (501) staff       (20)        1 2022-09-16 23:06:22.000000 eppo-server-sdk-1.1.1/eppo_server_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 ploomis    (501) staff       (20)       29 2022-09-16 23:06:22.000000 eppo-server-sdk-1.1.1/eppo_server_sdk.egg-info/requires.txt
+-rw-r--r--   0 ploomis    (501) staff       (20)       12 2022-09-16 23:06:22.000000 eppo-server-sdk-1.1.1/eppo_server_sdk.egg-info/top_level.txt
+-rw-r--r--   0 ploomis    (501) staff       (20)       84 2022-04-28 02:07:07.000000 eppo-server-sdk-1.1.1/pyproject.toml
+-rw-r--r--   0 ploomis    (501) staff       (20)       25 2022-09-16 20:27:28.000000 eppo-server-sdk-1.1.1/requirements-test.txt
+-rw-r--r--   0 ploomis    (501) staff       (20)       61 2022-06-20 22:49:01.000000 eppo-server-sdk-1.1.1/requirements.txt
+-rw-r--r--   0 ploomis    (501) staff       (20)      667 2022-09-16 23:06:22.371104 eppo-server-sdk-1.1.1/setup.cfg
```

### Comparing `eppo-server-sdk-1.0.4/LICENSE` & `eppo-server-sdk-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eppo-server-sdk-1.0.4/PKG-INFO` & `eppo-server-sdk-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eppo-server-sdk
-Version: 1.0.4
+Version: 1.1.1
 Summary: Eppo SDK for Python
 Home-page: https://github.com/Eppo-exp/python-sdk
 Author: Eppo
 Author-email: eppo-team@geteppo.com
 Project-URL: Bug Tracker, https://github.com/Eppo-exp/python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eppo-server-sdk-1.0.4/eppo_client/__init__.py` & `eppo-server-sdk-1.1.1/eppo_client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     ExperimentConfigurationRequestor,
 )
 from eppo_client.configuration_store import ConfigurationStore
 from eppo_client.constants import MAX_CACHE_ENTRIES
 from eppo_client.http_client import HttpClient, SdkParams
 from eppo_client.read_write_lock import ReadWriteLock
 
-__version__ = "1.0.4"
+__version__ = "1.1.1"
 
 __client: Optional[EppoClient] = None
 __lock = ReadWriteLock()
 
 
 def init(config: Config) -> EppoClient:
     """Initializes a global Eppo client instance
```

### Comparing `eppo-server-sdk-1.0.4/eppo_client/client.py` & `eppo-server-sdk-1.1.1/eppo_client/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import hashlib
 import datetime
 import logging
-from typing import List, Optional
+from typing import Optional
 from eppo_client.assignment_logger import AssignmentLogger
 from eppo_client.configuration_requestor import (
     ExperimentConfigurationDto,
     ExperimentConfigurationRequestor,
 )
 from eppo_client.constants import POLL_INTERVAL_MILLIS, POLL_JITTER_MILLIS
 from eppo_client.poller import Poller
-from eppo_client.rules import Rule, matches_any_rule
+from eppo_client.rules import find_matching_rule
 from eppo_client.shard import get_shard, is_in_shard_range
 from eppo_client.validation import validate_not_blank
 
 logger = logging.getLogger(__name__)
 
 
 class EppoClient:
@@ -28,73 +28,84 @@
             interval_millis=POLL_INTERVAL_MILLIS,
             jitter_millis=POLL_JITTER_MILLIS,
             callback=config_requestor.fetch_and_store_configurations,
         )
         self.__poller.start()
 
     def get_assignment(
-        self, subject_key: str, experiment_key: str, subject_attributes=dict()
+        self, subject_key: str, flag_key: str, subject_attributes=dict()
     ) -> Optional[str]:
         """Maps a subject to a variation for a given experiment
         Returns None if the subject is not part of the experiment sample.
 
         :param subject_key: an identifier of the experiment subject, for example a user ID.
-        :param experiment_key: an experiment identifier
+        :param flag_key: an experiment or feature flag identifier
         :param subject_attributes: optional attributes associated with the subject, for example name and email.
         The subject attributes are used for evaluating any targeting rules tied to the experiment.
         """
         validate_not_blank("subject_key", subject_key)
-        validate_not_blank("experiment_key", experiment_key)
-        experiment_config = self.__config_requestor.get_configuration(experiment_key)
+        validate_not_blank("flag_key", flag_key)
+        experiment_config = self.__config_requestor.get_configuration(flag_key)
         override = self._get_subject_variation_override(experiment_config, subject_key)
         if override:
             return override
-        if (
-            experiment_config is None
-            or not experiment_config.enabled
-            or not self._subject_attributes_satisfy_rules(
-                subject_attributes, experiment_config.rules
+
+        if experiment_config is None or not experiment_config.enabled:
+            logger.info(
+                "[Eppo SDK] No assigned variation. No active experiment or flag for key: "
+                + flag_key
             )
-            or not self._is_in_experiment_sample(
-                subject_key, experiment_key, experiment_config
+            return None
+
+        matched_rule = find_matching_rule(subject_attributes, experiment_config.rules)
+        if matched_rule is None:
+            logger.info(
+                "[Eppo SDK] No assigned variation. Subject attributes do not match targeting rules: {0}".format(
+                    subject_attributes
+                )
             )
+            return None
+
+        allocation = experiment_config.allocations[matched_rule.allocation_key]
+        if not self._is_in_experiment_sample(
+            subject_key,
+            flag_key,
+            experiment_config.subject_shards,
+            allocation.percent_exposure,
         ):
+            logger.info(
+                "[Eppo SDK] No assigned variation. Subject is not part of experiment sample population"
+            )
             return None
+
         shard = get_shard(
-            "assignment-{}-{}".format(subject_key, experiment_key),
+            "assignment-{}-{}".format(subject_key, flag_key),
             experiment_config.subject_shards,
         )
         assigned_variation = next(
             (
-                variation.name
-                for variation in experiment_config.variations
+                variation.value
+                for variation in allocation.variations
                 if is_in_shard_range(shard, variation.shard_range)
             ),
             None,
         )
         assignment_event = {
-            "experiment": experiment_key,
+            "experiment": flag_key,
             "variation": assigned_variation,
             "subject": subject_key,
             "timestamp": datetime.datetime.utcnow().isoformat(),
             "subjectAttributes": subject_attributes,
         }
         try:
             self.__assignment_logger.log_assignment(assignment_event)
         except Exception as e:
             logger.error("[Eppo SDK] Error logging assignment event: " + str(e))
         return assigned_variation
 
-    def _subject_attributes_satisfy_rules(
-        self, subject_attributes: dict, rules: List[Rule]
-    ) -> bool:
-        if len(rules) == 0:
-            return True
-        return matches_any_rule(subject_attributes, rules)
-
     def _shutdown(self):
         """Stops all background processes used by the client
         Do not use the client after calling this method.
         """
         self.__poller.stop()
 
     def _get_subject_variation_override(
@@ -108,17 +119,15 @@
             return experiment_config.overrides[subject_hash]
         return None
 
     def _is_in_experiment_sample(
         self,
         subject: str,
         experiment_key: str,
-        experiment_config: ExperimentConfigurationDto,
+        subject_shards: int,
+        percent_exposure: float,
     ):
         shard = get_shard(
             "exposure-{}-{}".format(subject, experiment_key),
-            experiment_config.subject_shards,
-        )
-        return (
-            shard
-            <= experiment_config.percent_exposure * experiment_config.subject_shards
+            subject_shards,
         )
+        return shard <= percent_exposure * subject_shards
```

### Comparing `eppo-server-sdk-1.0.4/eppo_client/config.py` & `eppo-server-sdk-1.1.1/eppo_client/config.py`

 * *Files identical despite different names*

### Comparing `eppo-server-sdk-1.0.4/eppo_client/configuration_requestor.py` & `eppo-server-sdk-1.1.1/eppo_client/configuration_requestor.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 import logging
-from typing import Dict, List, Optional, cast
+from typing import Any, Dict, List, Optional, cast
 from eppo_client.base_model import SdkBaseModel
 from eppo_client.configuration_store import ConfigurationStore
-from eppo_client.http_client import HttpClient, HttpRequestError
+from eppo_client.http_client import HttpClient
 from eppo_client.rules import Rule
 
 from eppo_client.shard import ShardRange
 
 logger = logging.getLogger(__name__)
 
 
 class VariationDto(SdkBaseModel):
     name: str
+    value: Any
     shard_range: ShardRange
 
 
+class AllocationDto(SdkBaseModel):
+    percent_exposure: float
+    variations: List[VariationDto]
+
+
 class ExperimentConfigurationDto(SdkBaseModel):
     subject_shards: int
-    percent_exposure: float
     enabled: bool
-    variations: List[VariationDto]
     name: Optional[str]
     overrides: Dict[str, str] = {}
     rules: List[Rule] = []
+    allocations: Dict[str, AllocationDto]
 
 
-RAC_ENDPOINT = "/randomized_assignment/config"
+RAC_ENDPOINT = "/randomized_assignment/v2/config"
 
 
 class ExperimentConfigurationRequestor:
     def __init__(
         self,
         http_client: HttpClient,
         config_store: ConfigurationStore[ExperimentConfigurationDto],
@@ -42,20 +47,15 @@
     ) -> Optional[ExperimentConfigurationDto]:
         if self.__http_client.is_unauthorized():
             raise ValueError("Unauthorized: please check your API key")
         return self.__config_store.get_configuration(experiment_key)
 
     def fetch_and_store_configurations(self) -> Dict[str, ExperimentConfigurationDto]:
         try:
-            configs = cast(
-                dict, self.__http_client.get(RAC_ENDPOINT).get("experiments", {})
-            )
+            configs = cast(dict, self.__http_client.get(RAC_ENDPOINT).get("flags", {}))
             for exp_key, exp_config in configs.items():
                 configs[exp_key] = ExperimentConfigurationDto(**exp_config)
             self.__config_store.set_configurations(configs)
             return configs
-        except HttpRequestError as e:
+        except Exception as e:
             logger.error("Error retrieving assignment configurations: " + str(e))
-            if e.is_recoverable():
-                return {}
-            else:
-                raise e  # caught by the polling task; causes assignment polling to stop
+            return {}
```

### Comparing `eppo-server-sdk-1.0.4/eppo_client/configuration_store.py` & `eppo-server-sdk-1.1.1/eppo_client/configuration_store.py`

 * *Files identical despite different names*

### Comparing `eppo-server-sdk-1.0.4/eppo_client/http_client.py` & `eppo-server-sdk-1.1.1/eppo_client/http_client.py`

 * *Files 27% similar despite different names*

```diff
@@ -16,22 +16,14 @@
 
 
 class HttpRequestError(Exception):
     def __init__(self, message: str, status_code: int):
         self.status_code = status_code
         super().__init__(message)
 
-    def is_recoverable(self) -> bool:
-        if self.status_code >= 400 and self.status_code < 500:
-            return (
-                self.status_code == HTTPStatus.TOO_MANY_REQUESTS
-                or self.status_code == HTTPStatus.REQUEST_TIMEOUT
-            )
-        return True
-
 
 REQUEST_TIMEOUT_SECONDS = 2
 # Retry reference: https://urllib3.readthedocs.io/en/latest/reference/urllib3.util.html#module-urllib3.util.retry
 # This applies only to failed DNS lookups and connection timeouts,
 # never to requests where data has made it to the server.
 MAX_RETRIES = Retry(total=3, backoff_factor=1)
```

### Comparing `eppo-server-sdk-1.0.4/eppo_client/poller.py` & `eppo-server-sdk-1.1.1/eppo_client/poller.py`

 * *Files identical despite different names*

### Comparing `eppo-server-sdk-1.0.4/eppo_client/read_write_lock.py` & `eppo-server-sdk-1.1.1/eppo_client/read_write_lock.py`

 * *Files identical despite different names*

### Comparing `eppo-server-sdk-1.0.4/eppo_client/rules.py` & `eppo-server-sdk-1.1.1/eppo_client/rules.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,22 +19,23 @@
 class Condition(SdkBaseModel):
     operator: OperatorType
     attribute: str
     value: Any
 
 
 class Rule(SdkBaseModel):
+    allocation_key: str
     conditions: List[Condition]
 
 
-def matches_any_rule(subject_attributes: dict, rules: List[Rule]):
+def find_matching_rule(subject_attributes: dict, rules: List[Rule]):
     for rule in rules:
         if matches_rule(subject_attributes, rule):
-            return True
-    return False
+            return rule
+    return None
 
 
 def matches_rule(subject_attributes: dict, rule: Rule):
     for condition in rule.conditions:
         if not evaluate_condition(subject_attributes, condition):
             return False
     return True
```

### Comparing `eppo-server-sdk-1.0.4/eppo_client/shard.py` & `eppo-server-sdk-1.1.1/eppo_client/shard.py`

 * *Files identical despite different names*

### Comparing `eppo-server-sdk-1.0.4/eppo_server_sdk.egg-info/PKG-INFO` & `eppo-server-sdk-1.1.1/eppo_server_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eppo-server-sdk
-Version: 1.0.4
+Version: 1.1.1
 Summary: Eppo SDK for Python
 Home-page: https://github.com/Eppo-exp/python-sdk
 Author: Eppo
 Author-email: eppo-team@geteppo.com
 Project-URL: Bug Tracker, https://github.com/Eppo-exp/python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eppo-server-sdk-1.0.4/eppo_server_sdk.egg-info/SOURCES.txt` & `eppo-server-sdk-1.1.1/eppo_server_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eppo-server-sdk-1.0.4/setup.cfg` & `eppo-server-sdk-1.1.1/setup.cfg`

 * *Files identical despite different names*


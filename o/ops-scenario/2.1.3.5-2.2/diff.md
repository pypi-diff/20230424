# Comparing `tmp/ops-scenario-2.1.3.5.tar.gz` & `tmp/ops-scenario-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ops-scenario-2.1.3.5.tar", last modified: Fri Apr 21 13:19:18 2023, max compression
+gzip compressed data, was "ops-scenario-2.2.tar", last modified: Mon Apr 24 08:20:26 2023, max compression
```

## Comparing `ops-scenario-2.1.3.5.tar` & `ops-scenario-2.2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:19:18.320035 ops-scenario-2.1.3.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:19:18.312034 ops-scenario-2.1.3.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:19:18.316035 ops-scenario-2.1.3.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/.github/workflows/build_wheels.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/.github/workflows/quality_checks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    29581 2023-04-21 13:19:18.320035 ops-scenario-2.1.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28953 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:19:18.316035 ops-scenario-2.1.3.5/ops_scenario.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29581 2023-04-21 13:19:18.000000 ops-scenario-2.1.3.5/ops_scenario.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-21 13:19:18.000000 ops-scenario-2.1.3.5/ops_scenario.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 13:19:18.000000 ops-scenario-2.1.3.5/ops_scenario.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-21 13:19:18.000000 ops-scenario-2.1.3.5/ops_scenario.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-21 13:19:18.000000 ops-scenario-2.1.3.5/ops_scenario.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-21 13:19:18.000000 ops-scenario-2.1.3.5/ops_scenario.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:19:18.316035 ops-scenario-2.1.3.5/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    19480 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/resources/state-transition-model.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:19:18.316035 ops-scenario-2.1.3.5/scenario/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/scenario/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/scenario/capture_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    10466 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/scenario/consistency_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/scenario/fs_mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/scenario/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/scenario/mocking.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/scenario/ops_main_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)    18076 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/scenario/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:19:18.316035 ops-scenario-2.1.3.5/scenario/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/scenario/scripts/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/scenario/scripts/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/scenario/scripts/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    29386 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/scenario/scripts/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/scenario/scripts/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/scenario/sequences.py
--rw-r--r--   0 runner    (1001) docker     (123)    38623 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/scenario/state.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 13:19:18.320035 ops-scenario-2.1.3.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:19:18.316035 ops-scenario-2.1.3.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:19:18.316035 ops-scenario-2.1.3.5/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/resources/demo_decorate_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_consistency_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:19:18.320035 ops-scenario-2.1.3.5/tests/test_e2e/
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_e2e/test_builtin_scenes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_e2e/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_e2e/test_custom_event_triggers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_e2e/test_deferred.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_e2e/test_juju_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_e2e/test_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_e2e/test_observers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8429 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_e2e/test_pebble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_e2e/test_play_assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_e2e/test_relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_e2e/test_rubbish_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_e2e/test_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_e2e/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_e2e/test_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_e2e/test_stored_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_e2e/test_vroot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_emitted_events_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tests/test_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-21 13:19:05.000000 ops-scenario-2.1.3.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:20:26.261593 ops-scenario-2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:20:26.249593 ops-scenario-2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:20:26.253593 ops-scenario-2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-24 08:20:14.000000 ops-scenario-2.2/.github/workflows/build_wheels.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-24 08:20:14.000000 ops-scenario-2.2/.github/workflows/quality_checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-24 08:20:14.000000 ops-scenario-2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-24 08:20:14.000000 ops-scenario-2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    29577 2023-04-24 08:20:26.261593 ops-scenario-2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28953 2023-04-24 08:20:14.000000 ops-scenario-2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:20:26.253593 ops-scenario-2.2/ops_scenario.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29577 2023-04-24 08:20:26.000000 ops-scenario-2.2/ops_scenario.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-24 08:20:26.000000 ops-scenario-2.2/ops_scenario.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 08:20:26.000000 ops-scenario-2.2/ops_scenario.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-24 08:20:26.000000 ops-scenario-2.2/ops_scenario.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-24 08:20:26.000000 ops-scenario-2.2/ops_scenario.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-24 08:20:26.000000 ops-scenario-2.2/ops_scenario.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-24 08:20:14.000000 ops-scenario-2.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:20:26.253593 ops-scenario-2.2/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    19480 2023-04-24 08:20:14.000000 ops-scenario-2.2/resources/state-transition-model.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:20:26.257593 ops-scenario-2.2/scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-24 08:20:14.000000 ops-scenario-2.2/scenario/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-24 08:20:14.000000 ops-scenario-2.2/scenario/capture_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10466 2023-04-24 08:20:14.000000 ops-scenario-2.2/scenario/consistency_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-24 08:20:14.000000 ops-scenario-2.2/scenario/fs_mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-24 08:20:14.000000 ops-scenario-2.2/scenario/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12809 2023-04-24 08:20:14.000000 ops-scenario-2.2/scenario/mocking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-24 08:20:14.000000 ops-scenario-2.2/scenario/ops_main_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18076 2023-04-24 08:20:14.000000 ops-scenario-2.2/scenario/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:20:26.257593 ops-scenario-2.2/scenario/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-24 08:20:14.000000 ops-scenario-2.2/scenario/scripts/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-24 08:20:14.000000 ops-scenario-2.2/scenario/scripts/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-24 08:20:14.000000 ops-scenario-2.2/scenario/scripts/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29386 2023-04-24 08:20:14.000000 ops-scenario-2.2/scenario/scripts/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-24 08:20:14.000000 ops-scenario-2.2/scenario/scripts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-04-24 08:20:14.000000 ops-scenario-2.2/scenario/sequences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39970 2023-04-24 08:20:14.000000 ops-scenario-2.2/scenario/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 08:20:26.261593 ops-scenario-2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:20:26.257593 ops-scenario-2.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:20:26.257593 ops-scenario-2.2/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/resources/demo_decorate_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_consistency_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 08:20:26.261593 ops-scenario-2.2/tests/test_e2e/
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_e2e/test_builtin_scenes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_e2e/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_e2e/test_custom_event_triggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_e2e/test_deferred.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_e2e/test_juju_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_e2e/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_e2e/test_observers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_e2e/test_pebble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_e2e/test_play_assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_e2e/test_relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_e2e/test_rubbish_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_e2e/test_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_e2e/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_e2e/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_e2e/test_stored_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_e2e/test_vroot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_emitted_events_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-04-24 08:20:14.000000 ops-scenario-2.2/tests/test_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-24 08:20:14.000000 ops-scenario-2.2/tox.ini
```

### Comparing `ops-scenario-2.1.3.5/.github/workflows/build_wheels.yaml` & `ops-scenario-2.2/.github/workflows/build_wheels.yaml`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.5/.github/workflows/quality_checks.yaml` & `ops-scenario-2.2/.github/workflows/quality_checks.yaml`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.5/LICENSE.txt` & `ops-scenario-2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.5/PKG-INFO` & `ops-scenario-2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-scenario
-Version: 2.1.3.5
+Version: 2.2
 Summary: Python library providing a Scenario-based testing API for Operator Framework charms.
 Author-email: Pietro Pasotti <pietro.pasotti@canonical.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/PietroPasotti/ops-scenario
 Project-URL: Bug Tracker, https://github.com/PietroPasotti/ops-scenario/issues
 Keywords: juju,test
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ops-scenario-2.1.3.5/README.md` & `ops-scenario-2.2/README.md`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.5/ops_scenario.egg-info/PKG-INFO` & `ops-scenario-2.2/ops_scenario.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-scenario
-Version: 2.1.3.5
+Version: 2.2
 Summary: Python library providing a Scenario-based testing API for Operator Framework charms.
 Author-email: Pietro Pasotti <pietro.pasotti@canonical.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/PietroPasotti/ops-scenario
 Project-URL: Bug Tracker, https://github.com/PietroPasotti/ops-scenario/issues
 Keywords: juju,test
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ops-scenario-2.1.3.5/ops_scenario.egg-info/SOURCES.txt` & `ops-scenario-2.2/ops_scenario.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.5/pyproject.toml` & `ops-scenario-2.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "setuptools_scm >= 2.0.0, <3"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ops-scenario"
 
-version = "2.1.3.5"
+version = "2.2"
 authors = [
     { name = "Pietro Pasotti", email = "pietro.pasotti@canonical.com" }
 ]
 description = "Python library providing a Scenario-based testing API for Operator Framework charms."
 license.text = "Apache-2.0"
 keywords = ["juju", "test"]
```

### Comparing `ops-scenario-2.1.3.5/resources/state-transition-model.png` & `ops-scenario-2.2/resources/state-transition-model.png`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.5/scenario/capture_events.py` & `ops-scenario-2.2/scenario/capture_events.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.5/scenario/consistency_checker.py` & `ops-scenario-2.2/scenario/consistency_checker.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.5/scenario/fs_mocks.py` & `ops-scenario-2.2/scenario/fs_mocks.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.5/scenario/mocking.py` & `ops-scenario-2.2/scenario/mocking.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,15 +216,15 @@
         peek: bool = False,
     ) -> Dict[str, str]:
         secret = self._get_secret(id, label)
         revision = secret.revision
         if peek or refresh:
             revision = max(secret.contents.keys())
             if refresh:
-                secret.revision = revision
+                secret._set_revision(revision)
 
         return secret.contents[revision]
 
     def secret_info_get(
         self, *, id: Optional[str] = None, label: Optional[str] = None
     ) -> SecretInfo:
         secret = self._get_secret(id, label)
@@ -294,14 +294,18 @@
             raise RuntimeError(f"not the owner of {secret}")
 
         if revision:
             del secret.contents[revision]
         else:
             secret.contents.clear()
 
+    def relation_remote_app_name(self, relation_id: int):
+        relation = self._get_relation_by_id(relation_id)
+        return relation.remote_app_name
+
     # TODO:
     def action_set(self, *args, **kwargs):
         raise NotImplementedError("action_set")
 
     def action_fail(self, *args, **kwargs):
         raise NotImplementedError("action_fail")
 
@@ -310,17 +314,14 @@
 
     def storage_add(self, *args, **kwargs):
         raise NotImplementedError("storage_add")
 
     def action_get(self):
         raise NotImplementedError("action_get")
 
-    def relation_remote_app_name(self, *args, **kwargs):
-        raise NotImplementedError("relation_remote_app_name")
-
     def resource_get(self, *args, **kwargs):
         raise NotImplementedError("resource_get")
 
     def storage_list(self, *args, **kwargs):
         raise NotImplementedError("storage_list")
 
     def storage_get(self, *args, **kwargs):
```

### Comparing `ops-scenario-2.1.3.5/scenario/ops_main_mock.py` & `ops-scenario-2.2/scenario/ops_main_mock.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.5/scenario/runtime.py` & `ops-scenario-2.2/scenario/runtime.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.5/scenario/scripts/main.py` & `ops-scenario-2.2/scenario/scripts/main.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.5/scenario/scripts/snapshot.py` & `ops-scenario-2.2/scenario/scripts/snapshot.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.5/scenario/scripts/utils.py` & `ops-scenario-2.2/scenario/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.5/scenario/sequences.py` & `ops-scenario-2.2/scenario/sequences.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.5/scenario/state.py` & `ops-scenario-2.2/scenario/state.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,24 +66,24 @@
 class StateValidationError(RuntimeError):
     """Raised when individual parts of the State are inconsistent."""
 
     # as opposed to InconsistentScenario error where the
     # **combination** of several parts of the State are.
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class _DCBase:
     def replace(self, *args, **kwargs):
         return dataclasses.replace(self, *args, **kwargs)
 
     def copy(self) -> "Self":
         return copy.deepcopy(self)
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class Secret(_DCBase):
     id: str
 
     # mapping from revision IDs to each revision's contents
     contents: Dict[int, Dict[str, str]]
 
     # indicates if the secret is owned by THIS unit, THIS app or some other app/unit.
@@ -138,14 +138,19 @@
         """Sugar to generate a secret-remove event."""
         if not self.owner:
             raise ValueError(
                 "This unit will never receive secret-removed for a secret it does not own."
             )
         return Event(name="secret_removed", secret=self)
 
+    def _set_revision(self, revision: int):
+        """Set a new tracked revision."""
+        # bypass frozen dataclass
+        object.__setattr__(self, "revision", revision)
+
 
 _RELATION_IDS_CTR = 0
 
 
 def normalize_name(s: str):
     """Event names need underscores instead of dashes."""
     return s.replace("-", "_")
@@ -168,23 +173,33 @@
 
         return Event(*self._args, *self._kwargs, relation_remote_unit_id=remote_unit)
 
     def deferred(self, handler: Callable, event_id: int = 1) -> "DeferredEvent":
         return self().deferred(handler=handler, event_id=event_id)
 
 
-@dataclasses.dataclass
+def _generate_new_relation_id():
+    global _RELATION_IDS_CTR
+    _RELATION_IDS_CTR += 1
+    logger.info(
+        f"relation ID unset; automatically assigning {_RELATION_IDS_CTR}. "
+        f"If there are problems, pass one manually."
+    )
+    return _RELATION_IDS_CTR
+
+
+@dataclasses.dataclass(frozen=True)
 class RelationBase(_DCBase):
     endpoint: str
 
     # we can derive this from the charm's metadata
     interface: str = None
 
     # Every new Relation instance gets a new one, if there's trouble, override.
-    relation_id: int = -1
+    relation_id: int = dataclasses.field(default_factory=_generate_new_relation_id)
 
     local_app_data: Dict[str, str] = dataclasses.field(default_factory=dict)
     local_unit_data: Dict[str, str] = dataclasses.field(default_factory=dict)
 
     @property
     def _databags(self):
         """Yield all databags in this relation."""
@@ -208,23 +223,14 @@
     def __post_init__(self):
         if type(self) is RelationBase:
             raise RuntimeError(
                 "RelationBase cannot be instantiated directly; "
                 "please use Relation, PeerRelation, or SubordinateRelation"
             )
 
-        global _RELATION_IDS_CTR
-        if self.relation_id == -1:
-            _RELATION_IDS_CTR += 1
-            logger.info(
-                f"relation ID unset; automatically assigning {_RELATION_IDS_CTR}. "
-                f"If there are problems, pass one manually."
-            )
-            self.relation_id = _RELATION_IDS_CTR
-
         for databag in self._databags:
             self._validate_databag(databag)
 
     def _validate_databag(self, databag: dict):
         if not isinstance(databag, dict):
             raise StateValidationError(
                 f"all databags should be dicts, not {type(databag)}"
@@ -310,27 +316,39 @@
         ids = [x for x in data]
     else:
         ids = [0]
         data = {0: {}}
     return ids, data
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class Relation(RelationBase):
     remote_app_name: str = "remote"
+
+    # fixme: simplify API by deriving remote_unit_ids from remote_units_data.
     remote_unit_ids: List[int] = dataclasses.field(default_factory=list)
 
     # local limit
     limit: int = 1
 
     remote_app_data: Dict[str, str] = dataclasses.field(default_factory=dict)
     remote_units_data: Dict[int, Dict[str, str]] = dataclasses.field(
         default_factory=dict
     )
 
+    def __post_init__(self):
+        super().__post_init__()
+
+        remote_unit_ids, remote_units_data = unify_ids_and_remote_units_data(
+            self.remote_unit_ids, self.remote_units_data
+        )
+        # bypass frozen dataclass
+        object.__setattr__(self, "remote_unit_ids", remote_unit_ids)
+        object.__setattr__(self, "remote_units_data", remote_units_data)
+
     @property
     def _remote_app_name(self) -> str:
         """Who is on the other end of this relation?"""
         return self.remote_app_name
 
     @property
     def _remote_unit_ids(self) -> Tuple[int]:
@@ -345,22 +363,16 @@
     def _databags(self):
         """Yield all databags in this relation."""
         yield self.local_app_data
         yield self.local_unit_data
         yield self.remote_app_data
         yield from self.remote_units_data.values()
 
-    def __post_init__(self):
-        super().__post_init__()
-        self.remote_unit_ids, self.remote_units_data = unify_ids_and_remote_units_data(
-            self.remote_unit_ids, self.remote_units_data
-        )
-
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class SubordinateRelation(RelationBase):
     # todo: consider renaming them to primary_*_data
     remote_app_data: Dict[str, str] = dataclasses.field(default_factory=dict)
     remote_unit_data: Dict[str, str] = dataclasses.field(default_factory=dict)
 
     # app name and ID of the primary that *this unit* is attached to.
     primary_app_name: str = "remote"
@@ -389,15 +401,15 @@
         yield self.remote_unit_data
 
     @property
     def primary_name(self) -> str:
         return f"{self.primary_app_name}/{self.primary_id}"
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class PeerRelation(RelationBase):
     peers_data: Dict[int, Dict[str, str]] = dataclasses.field(default_factory=dict)
 
     # IDs of the peers. Consistency checks will validate that *this unit*'s ID is not in here.
     peers_ids: List[int] = dataclasses.field(default_factory=list)
 
     @property
@@ -419,28 +431,31 @@
         return tuple(self.peers_ids)
 
     def _get_databag_for_remote(self, unit_id: int) -> Dict[str, str]:
         """Return the databag for some remote unit ID."""
         return self.peers_data[unit_id]
 
     def __post_init__(self):
-        self.peers_ids, self.peers_data = unify_ids_and_remote_units_data(
+        peers_ids, peers_data = unify_ids_and_remote_units_data(
             self.peers_ids, self.peers_data
         )
+        # bypass frozen dataclass guards
+        object.__setattr__(self, "peers_ids", peers_ids)
+        object.__setattr__(self, "peers_data", peers_data)
 
 
 def _random_model_name():
     import random
     import string
 
     space = string.ascii_letters + string.digits
     return "".join(random.choice(space) for _ in range(20))
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class Model(_DCBase):
     name: str = _random_model_name()
     uuid: str = str(uuid4())
 
     # whatever juju models --format=json | jq '.models[<current-model-index>].type' gives back.
     # TODO: make this exhaustive.
     type: Literal["kubernetes", "lxd"] = "kubernetes"
@@ -449,39 +464,47 @@
 # for now, proc mock allows you to map one command to one mocked output.
 # todo extend: one input -> multiple outputs, at different times
 
 
 _CHANGE_IDS = 0
 
 
-@dataclasses.dataclass
+def _generate_new_change_id():
+    global _CHANGE_IDS
+    _CHANGE_IDS += 1
+    logger.info(
+        f"change ID unset; automatically assigning {_CHANGE_IDS}. "
+        f"If there are problems, pass one manually."
+    )
+    return _CHANGE_IDS
+
+
+@dataclasses.dataclass(frozen=True)
 class ExecOutput:
     return_code: int = 0
     stdout: str = ""
     stderr: str = ""
 
     # change ID: used internally to keep track of mocked processes
-    _change_id: int = -1
+    _change_id: int = dataclasses.field(default_factory=_generate_new_change_id)
 
     def _run(self) -> int:
-        global _CHANGE_IDS
-        _CHANGE_IDS = self._change_id = _CHANGE_IDS + 1
-        return _CHANGE_IDS
+        return self._change_id
 
 
 _ExecMock = Dict[Tuple[str, ...], ExecOutput]
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class Mount(_DCBase):
     location: Union[str, PurePosixPath]
     src: Union[str, Path]
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class Container(_DCBase):
     name: str
     can_connect: bool = False
 
     # This is the base plan. On top of it, one can add layers.
     # We need to model pebble in this way because it's impossible to retrieve the layers from pebble
     # or derive them from the resulting plan (which one CAN get from pebble).
@@ -579,23 +602,23 @@
             logger.warning(
                 "you **can** fire pebble-ready while the container cannot connect, "
                 "but that's most likely not what you want."
             )
         return Event(name=normalize_name(self.name + "-pebble-ready"), container=self)
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class Address(_DCBase):
     hostname: str
     value: str
     cidr: str
     address: str = ""  # legacy
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class BindAddress(_DCBase):
     interface_name: str
     addresses: List[Address]
     mac_address: Optional[str] = None
 
     def hook_tool_output_fmt(self):
         # dumps itself to dict in the same format the hook tool would
@@ -605,15 +628,15 @@
             "addresses": [dataclasses.asdict(addr) for addr in self.addresses],
         }
         if self.mac_address:
             dct["mac-address"] = self.mac_address
         return dct
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class Network(_DCBase):
     name: str
 
     bind_addresses: List[BindAddress]
     ingress_addresses: List[str]
     egress_subnets: List[str]
 
@@ -650,15 +673,15 @@
                 )
             ],
             egress_subnets=list(egress_subnets),
             ingress_addresses=list(ingress_addresses),
         )
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class _EntityStatus(_DCBase):
     """This class represents StatusBase and should not be interacted with directly."""
 
     # Why not use StatusBase directly? Because that's not json-serializable.
 
     name: Literal["waiting", "blocked", "active", "unknown", "error", "maintenance"]
     message: str = ""
@@ -686,15 +709,15 @@
 
 
 def _status_to_entitystatus(obj: StatusBase) -> _EntityStatus:
     """Convert StatusBase to _EntityStatus."""
     return _EntityStatus(obj.name, obj.message)
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class Status(_DCBase):
     """Represents the 'juju statuses' of the application/unit being tested."""
 
     # the current statuses. Will be cast to _EntitiyStatus in __post_init__
     app: Union[StatusBase, _EntityStatus] = _EntityStatus("unknown")
     unit: Union[StatusBase, _EntityStatus] = _EntityStatus("unknown")
     app_version: str = ""
@@ -706,45 +729,49 @@
 
     def __post_init__(self):
         for name in ["app", "unit"]:
             val = getattr(self, name)
             if isinstance(val, _EntityStatus):
                 pass
             elif isinstance(val, StatusBase):
-                setattr(self, name, _status_to_entitystatus(val))
+                object.__setattr__(self, name, _status_to_entitystatus(val))
             elif isinstance(val, tuple):
                 logger.warning(
                     "Initializing Status.[app/unit] with Tuple[str, str] is deprecated "
                     "and will be removed soon. \n"
                     f"Please pass a StatusBase instance: `StatusBase(*{val})`"
                 )
-                setattr(self, name, _EntityStatus(*val))
+                object.__setattr__(self, name, _EntityStatus(*val))
             else:
                 raise TypeError(f"Invalid status.{name}: {val!r}")
 
     def _update_app_version(self, new_app_version: str):
         """Update the current app version and record the previous one."""
         # We don't keep a full history because we don't expect the app version to change more
         # than once per hook.
-        self.previous_app_version = self.app_version
-        self.app_version = new_app_version
+
+        # bypass frozen dataclass
+        object.__setattr__(self, "previous_app_version", self.app_version)
+        object.__setattr__(self, "app_version", new_app_version)
 
     def _update_status(
         self, new_status: str, new_message: str = "", is_app: bool = False
     ):
         """Update the current app/unit status and add the previous one to the history."""
         if is_app:
             self.app_history.append(self.app)
-            self.app = _EntityStatus(new_status, new_message)
+            # bypass frozen dataclass
+            object.__setattr__(self, "app", _EntityStatus(new_status, new_message))
         else:
             self.unit_history.append(self.unit)
-            self.unit = _EntityStatus(new_status, new_message)
+            # bypass frozen dataclass
+            object.__setattr__(self, "unit", _EntityStatus(new_status, new_message))
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class StoredState(_DCBase):
     # /-separated Object names. E.g. MyCharm/MyCharmLib.
     # if None, this StoredState instance is owned by the Framework.
     owner_path: Optional[str]
 
     name: str = "_stored"
     content: Dict[str, Any] = dataclasses.field(default_factory=dict)
@@ -752,15 +779,15 @@
     data_type_name: str = "StoredStateData"
 
     @property
     def handle_path(self):
         return f"{self.owner_path or ''}/{self.data_type_name}[{self.name}]"
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class State(_DCBase):
     """Represents the juju-owned portion of a unit's state.
 
     Roughly speaking, it wraps all hook-tool- and pebble-mediated data a charm can access in its lifecycle.
     For example, status-get will return data from `State.status`, is-leader will return data from
     `State.leader`, and so on.
     """
@@ -866,15 +893,15 @@
             config=config,
             charm_root=charm_root,
             juju_version=juju_version,
             unit_id=unit_id,
         )
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class _CharmSpec(_DCBase):
     """Charm spec."""
 
     charm_type: Type["CharmType"]
     meta: Optional[Dict[str, Any]]
     actions: Optional[Dict[str, Any]] = None
     config: Optional[Dict[str, Any]] = None
@@ -910,29 +937,29 @@
         )
 
 
 def sort_patch(patch: List[Dict], key=lambda obj: obj["path"] + obj["op"]):
     return sorted(patch, key=key)
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class DeferredEvent(_DCBase):
     handle_path: str
     owner: str
     observer: str
 
     # needs to be marshal.dumps-able.
     snapshot_data: Dict = dataclasses.field(default_factory=dict)
 
     @property
     def name(self):
         return self.handle_path.split("/")[-1].split("[")[0]
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class Event(_DCBase):
     name: str
     args: Tuple[Any] = ()
     kwargs: Dict[str, Any] = dataclasses.field(default_factory=dict)
 
     # if this is a relation event, the relation it refers to
     relation: Optional["AnyRelation"] = None
@@ -957,15 +984,17 @@
                 "non-relation event constructor."
             )
         return self.replace(relation_remote_unit_id=remote_unit_id)
 
     def __post_init__(self):
         if "-" in self.name:
             logger.warning(f"Only use underscores in event names. {self.name!r}")
-        self.name = normalize_name(self.name)
+
+        # bypass frozen dataclass
+        object.__setattr__(self, "name", normalize_name(self.name))
 
     @property
     def _is_relation_event(self) -> bool:
         """Whether the event name indicates that this is a relation event."""
         return any(self.name.endswith(suffix) for suffix in RELATION_EVENTS_SUFFIX)
 
     @property
@@ -1081,22 +1110,22 @@
 ):
     """Construct a DeferredEvent from an Event or an event name."""
     if isinstance(event, str):
         event = Event(event, relation=relation, container=container)
     return event.deferred(handler=handler, event_id=event_id)
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class Inject(_DCBase):
     """Base class for injectors: special placeholders used to tell harness_ctx
     to inject instances that can't be retrieved in advance in event args or kwargs.
     """
 
 
-@dataclasses.dataclass
+@dataclasses.dataclass(frozen=True)
 class InjectRelation(Inject):
     relation_name: str
     relation_id: Optional[int] = None
 
 
 def _derive_args(event_name: str):
     args = []
```

### Comparing `ops-scenario-2.1.3.5/tests/test_consistency_checker.py` & `ops-scenario-2.2/tests/test_consistency_checker.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.5/tests/test_e2e/test_builtin_scenes.py` & `ops-scenario-2.2/tests/test_e2e/test_builtin_scenes.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.5/tests/test_e2e/test_config.py` & `ops-scenario-2.2/tests/test_e2e/test_config.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.5/tests/test_e2e/test_custom_event_triggers.py` & `ops-scenario-2.2/tests/test_e2e/test_custom_event_triggers.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.5/tests/test_e2e/test_deferred.py` & `ops-scenario-2.2/tests/test_e2e/test_deferred.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.5/tests/test_e2e/test_juju_log.py` & `ops-scenario-2.2/tests/test_e2e/test_juju_log.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.5/tests/test_e2e/test_network.py` & `ops-scenario-2.2/tests/test_e2e/test_network.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.5/tests/test_e2e/test_observers.py` & `ops-scenario-2.2/tests/test_e2e/test_observers.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.5/tests/test_e2e/test_pebble.py` & `ops-scenario-2.2/tests/test_e2e/test_pebble.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,17 +124,16 @@
     )
 
     if make_dirs:
         file = out.get_container("foo").filesystem.open("/foo/bar/baz.txt")
         assert file.read() == text
     else:
         # nothing has changed
-        out.juju_log = []
-        out.stored_state = state.stored_state  # ignore stored state in delta.
-        assert not out.jsonpatch_delta(state)
+        out_purged = out.replace(juju_log=[], stored_state=state.stored_state)
+        assert not out_purged.jsonpatch_delta(state)
 
 
 LS = """
 .rw-rw-r--  228 ubuntu ubuntu 18 jan 12:05 -- charmcraft.yaml    
 .rw-rw-r--  497 ubuntu ubuntu 18 jan 12:05 -- config.yaml        
 .rw-rw-r--  900 ubuntu ubuntu 18 jan 12:05 -- CONTRIBUTING.md    
 drwxrwxr-x    - ubuntu ubuntu 18 jan 12:06 -- lib
```

### Comparing `ops-scenario-2.1.3.5/tests/test_e2e/test_play_assertions.py` & `ops-scenario-2.2/tests/test_e2e/test_play_assertions.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,17 +54,16 @@
         event="start",
         post_event=post_event,
         pre_event=pre_event,
     )
 
     assert out.status.unit == ActiveStatus("yabadoodle")
 
-    out.juju_log = []  # exclude juju log from delta
-    out.stored_state = initial_state.stored_state  # ignore stored state in delta.
-    assert out.jsonpatch_delta(initial_state) == [
+    out_purged = out.replace(juju_log=[], stored_state=initial_state.stored_state)
+    assert out_purged.jsonpatch_delta(initial_state) == [
         {
             "op": "replace",
             "path": "/status/unit/message",
             "value": "yabadoodle",
         },
         {
             "op": "replace",
```

### Comparing `ops-scenario-2.1.3.5/tests/test_e2e/test_relations.py` & `ops-scenario-2.2/tests/test_e2e/test_relations.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.5/tests/test_e2e/test_rubbish_events.py` & `ops-scenario-2.2/tests/test_e2e/test_rubbish_events.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.5/tests/test_e2e/test_secrets.py` & `ops-scenario-2.2/tests/test_e2e/test_secrets.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.5/tests/test_e2e/test_state.py` & `ops-scenario-2.2/tests/test_e2e/test_state.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,17 +56,16 @@
 @pytest.fixture
 def state():
     return State(config={"foo": "bar"}, leader=True)
 
 
 def test_bare_event(state, mycharm):
     out = state.trigger("start", mycharm, meta={"name": "foo"})
-    out.juju_log = []  # ignore logging output in the delta
-    out.stored_state = state.stored_state  # ignore stored state in delta.
-    assert state.jsonpatch_delta(out) == []
+    out_purged = out.replace(juju_log=[], stored_state=state.stored_state)
+    assert state.jsonpatch_delta(out_purged) == []
 
 
 def test_leader_get(state, mycharm):
     def pre_event(charm):
         assert charm.unit.is_leader()
 
     state.trigger(
@@ -84,22 +83,23 @@
         charm.app.status = WaitingStatus("foo barz")
 
     mycharm._call = call
     out = state.trigger(
         "start",
         mycharm,
         meta={"name": "foo"},
+        config={"options": {"foo": {"type": "string"}}},
     )
     assert out.status.unit == ActiveStatus("foo test")
     assert out.status.app == WaitingStatus("foo barz")
     assert out.status.app_version == ""
 
-    out.juju_log = []  # ignore logging output in the delta
-    out.stored_state = state.stored_state  # ignore stored state in delta.
-    assert out.jsonpatch_delta(state) == sort_patch(
+    # ignore logging output and stored state in the delta
+    out_purged = out.replace(juju_log=[], stored_state=state.stored_state)
+    assert out_purged.jsonpatch_delta(state) == sort_patch(
         [
             {"op": "replace", "path": "/status/app/message", "value": "foo barz"},
             {"op": "replace", "path": "/status/app/name", "value": "waiting"},
             {
                 "op": "add",
                 "path": "/status/app_history/0",
                 "value": {"message": "", "name": "unknown"},
@@ -119,15 +119,15 @@
 def test_container(connect, mycharm):
     def pre_event(charm: CharmBase):
         container = charm.unit.get_container("foo")
         assert container is not None
         assert container.name == "foo"
         assert container.can_connect() is connect
 
-    State(containers=(Container(name="foo", can_connect=connect),)).trigger(
+    State(containers=[Container(name="foo", can_connect=connect)]).trigger(
         "start",
         mycharm,
         meta={
             "name": "foo",
             "containers": {"foo": {"resource": "bar"}},
         },
         pre_event=pre_event,
```

### Comparing `ops-scenario-2.1.3.5/tests/test_e2e/test_status.py` & `ops-scenario-2.2/tests/test_e2e/test_status.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.5/tests/test_e2e/test_stored_state.py` & `ops-scenario-2.2/tests/test_e2e/test_stored_state.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.5/tests/test_e2e/test_vroot.py` & `ops-scenario-2.2/tests/test_e2e/test_vroot.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.5/tests/test_emitted_events_util.py` & `ops-scenario-2.2/tests/test_emitted_events_util.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.5/tests/test_runtime.py` & `ops-scenario-2.2/tests/test_runtime.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-2.1.3.5/tox.ini` & `ops-scenario-2.2/tox.ini`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2022 Canonical
 # See LICENSE file for licensing details.
 
 [tox]
 envlist =
-    {py36,py37,py38}
+    {py36,py37,py38,py311}
     unit, lint
 isolated_build = True
 skip_missing_interpreters = True
 
 
 [vars]
 src_path = {toxinidir}/scenario
```


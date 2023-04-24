# Comparing `tmp/david-test-datadog-sma-0.0.1.tar.gz` & `tmp/david-test-datadog-sma-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "david-test-datadog-sma-0.0.1.tar", last modified: Mon Apr 24 16:56:20 2023, max compression
+gzip compressed data, was "david-test-datadog-sma-0.0.2.tar", last modified: Mon Apr 24 19:24:23 2023, max compression
```

## Comparing `david-test-datadog-sma-0.0.1.tar` & `david-test-datadog-sma-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-04-24 16:56:20.681625 david-test-datadog-sma-0.0.1/
--rw-r--r--   0 david.lee   (503) staff       (20)       66 2023-04-24 16:56:20.681461 david-test-datadog-sma-0.0.1/PKG-INFO
--rw-r--r--   0 david.lee   (503) staff       (20)      107 2023-04-24 16:56:16.000000 david-test-datadog-sma-0.0.1/pyproject.toml
--rw-r--r--   0 david.lee   (503) staff       (20)       38 2023-04-24 16:56:20.681673 david-test-datadog-sma-0.0.1/setup.cfg
-drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-04-24 16:56:20.679246 david-test-datadog-sma-0.0.1/src/
--rw-r--r--   0 david.lee   (503) staff       (20)        0 2023-04-18 15:20:38.000000 david-test-datadog-sma-0.0.1/src/__init__.py
-drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-04-24 16:56:20.679408 david-test-datadog-sma-0.0.1/src/datadog-serverless-agent-linux-amd64/
--rw-r--r--   0 david.lee   (503) staff       (20)   863300 2023-04-24 16:56:16.000000 david-test-datadog-sma-0.0.1/src/datadog-serverless-agent-linux-amd64/datadog-serverless-trace-mini-agent
-drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-04-24 16:56:20.680134 david-test-datadog-sma-0.0.1/src/datadog-serverless-agent-windows-amd64/
--rw-r--r--   0 david.lee   (503) staff       (20)   824832 2023-04-24 16:56:16.000000 david-test-datadog-sma-0.0.1/src/datadog-serverless-agent-windows-amd64/datadog-serverless-trace-mini-agent.exe
-drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-04-24 16:56:20.681285 david-test-datadog-sma-0.0.1/src/david_test_datadog_sma.egg-info/
--rw-r--r--   0 david.lee   (503) staff       (20)       66 2023-04-24 16:56:20.000000 david-test-datadog-sma-0.0.1/src/david_test_datadog_sma.egg-info/PKG-INFO
--rw-r--r--   0 david.lee   (503) staff       (20)      390 2023-04-24 16:56:20.000000 david-test-datadog-sma-0.0.1/src/david_test_datadog_sma.egg-info/SOURCES.txt
--rw-r--r--   0 david.lee   (503) staff       (20)        1 2023-04-24 16:56:20.000000 david-test-datadog-sma-0.0.1/src/david_test_datadog_sma.egg-info/dependency_links.txt
--rw-r--r--   0 david.lee   (503) staff       (20)       85 2023-04-24 16:56:20.000000 david-test-datadog-sma-0.0.1/src/david_test_datadog_sma.egg-info/top_level.txt
+drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-04-24 19:24:23.469530 david-test-datadog-sma-0.0.2/
+-rw-r--r--   0 david.lee   (503) staff       (20)       66 2023-04-24 19:24:23.469355 david-test-datadog-sma-0.0.2/PKG-INFO
+-rw-r--r--   0 david.lee   (503) staff       (20)      107 2023-04-24 19:24:19.000000 david-test-datadog-sma-0.0.2/pyproject.toml
+-rw-r--r--   0 david.lee   (503) staff       (20)       38 2023-04-24 19:24:23.469576 david-test-datadog-sma-0.0.2/setup.cfg
+drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-04-24 19:24:23.464781 david-test-datadog-sma-0.0.2/src/
+-rw-r--r--   0 david.lee   (503) staff       (20)        0 2023-04-18 15:20:38.000000 david-test-datadog-sma-0.0.2/src/__init__.py
+drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-04-24 19:24:23.464908 david-test-datadog-sma-0.0.2/src/datadog-serverless-agent-linux-amd64/
+-rw-r--r--   0 david.lee   (503) staff       (20)  2061544 2023-04-24 19:24:19.000000 david-test-datadog-sma-0.0.2/src/datadog-serverless-agent-linux-amd64/datadog-serverless-trace-mini-agent
+drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-04-24 19:24:23.466506 david-test-datadog-sma-0.0.2/src/datadog-serverless-agent-windows-amd64/
+-rw-r--r--   0 david.lee   (503) staff       (20)   824832 2023-04-24 16:56:16.000000 david-test-datadog-sma-0.0.2/src/datadog-serverless-agent-windows-amd64/datadog-serverless-trace-mini-agent.exe
+drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-04-24 19:24:23.469163 david-test-datadog-sma-0.0.2/src/david_test_datadog_sma.egg-info/
+-rw-r--r--   0 david.lee   (503) staff       (20)       66 2023-04-24 19:24:23.000000 david-test-datadog-sma-0.0.2/src/david_test_datadog_sma.egg-info/PKG-INFO
+-rw-r--r--   0 david.lee   (503) staff       (20)      390 2023-04-24 19:24:23.000000 david-test-datadog-sma-0.0.2/src/david_test_datadog_sma.egg-info/SOURCES.txt
+-rw-r--r--   0 david.lee   (503) staff       (20)        1 2023-04-24 19:24:23.000000 david-test-datadog-sma-0.0.2/src/david_test_datadog_sma.egg-info/dependency_links.txt
+-rw-r--r--   0 david.lee   (503) staff       (20)       85 2023-04-24 19:24:23.000000 david-test-datadog-sma-0.0.2/src/david_test_datadog_sma.egg-info/top_level.txt
```

### Comparing `david-test-datadog-sma-0.0.1/src/datadog-serverless-agent-windows-amd64/datadog-serverless-trace-mini-agent.exe` & `david-test-datadog-sma-0.0.2/src/datadog-serverless-agent-windows-amd64/datadog-serverless-trace-mini-agent.exe`

 * *Files identical despite different names*


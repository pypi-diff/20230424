# Comparing `tmp/daktari-0.0.92.tar.gz` & `tmp/daktari-0.0.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daktari-0.0.92.tar", last modified: Mon Apr 24 06:11:43 2023, max compression
+gzip compressed data, was "daktari-0.0.93.tar", last modified: Mon Apr 24 06:14:38 2023, max compression
```

## Comparing `daktari-0.0.92.tar` & `daktari-0.0.93.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:11:43.312399 daktari-0.0.92/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-24 06:11:32.000000 daktari-0.0.92/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-24 06:11:32.000000 daktari-0.0.92/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-04-24 06:11:43.312399 daktari-0.0.92/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-24 06:11:34.000000 daktari-0.0.92/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:11:43.308399 daktari-0.0.92/daktari/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-24 06:11:34.000000 daktari-0.0.92/daktari/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1389 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/check_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/check_sorter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/check_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:11:43.312399 daktari-0.0.92/daktari/checks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/checks/certs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/checks/direnv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/checks/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/checks/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/checks/flutter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/checks/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/checks/google.py
--rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/checks/intellij_idea.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/checks/java.py
--rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/checks/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/checks/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/checks/nodejs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/checks/onepassword.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/checks/python.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/checks/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/checks/terraform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/checks/test_certs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/checks/test_java.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/checks/test_ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/checks/test_yarn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/checks/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/checks/yarn.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/collection_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/command_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/os.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/resource_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:11:43.312399 daktari-0.0.92/daktari/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/resources/daktari-local-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/resources/mock_cert.pem
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/result_printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/test_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/test_check_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/test_check_sorter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/test_check_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/test_collection_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/test_version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-24 06:11:32.000000 daktari-0.0.92/daktari/version_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:11:43.308399 daktari-0.0.92/daktari.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-04-24 06:11:43.000000 daktari-0.0.92/daktari.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-24 06:11:43.000000 daktari-0.0.92/daktari.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 06:11:43.000000 daktari-0.0.92/daktari.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-24 06:11:43.000000 daktari-0.0.92/daktari.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-24 06:11:43.000000 daktari-0.0.92/daktari.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 06:11:43.000000 daktari-0.0.92/daktari.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-24 06:11:32.000000 daktari-0.0.92/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-24 06:11:32.000000 daktari-0.0.92/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 06:11:43.312399 daktari-0.0.92/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-24 06:11:34.000000 daktari-0.0.92/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:14:38.481343 daktari-0.0.93/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-24 06:14:25.000000 daktari-0.0.93/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-24 06:14:25.000000 daktari-0.0.93/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-04-24 06:14:38.481343 daktari-0.0.93/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-24 06:14:27.000000 daktari-0.0.93/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:14:38.477343 daktari-0.0.93/daktari/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-24 06:14:27.000000 daktari-0.0.93/daktari/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1389 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/check_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/check_sorter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/check_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:14:38.481343 daktari-0.0.93/daktari/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/checks/certs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/checks/direnv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/checks/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/checks/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/checks/flutter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/checks/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/checks/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/checks/intellij_idea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/checks/java.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/checks/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/checks/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/checks/nodejs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/checks/onepassword.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/checks/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/checks/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/checks/terraform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/checks/test_certs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/checks/test_java.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/checks/test_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/checks/test_yarn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/checks/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/checks/yarn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/collection_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/command_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/os.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/resource_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:14:38.481343 daktari-0.0.93/daktari/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/resources/daktari-local-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/resources/mock_cert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/result_printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/test_check_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/test_check_sorter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/test_check_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/test_collection_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/test_version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-24 06:14:25.000000 daktari-0.0.93/daktari/version_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 06:14:38.477343 daktari-0.0.93/daktari.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-04-24 06:14:38.000000 daktari-0.0.93/daktari.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-24 06:14:38.000000 daktari-0.0.93/daktari.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 06:14:38.000000 daktari-0.0.93/daktari.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-24 06:14:38.000000 daktari-0.0.93/daktari.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-24 06:14:38.000000 daktari-0.0.93/daktari.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 06:14:38.000000 daktari-0.0.93/daktari.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-24 06:14:25.000000 daktari-0.0.93/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-24 06:14:25.000000 daktari-0.0.93/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 06:14:38.481343 daktari-0.0.93/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-24 06:14:27.000000 daktari-0.0.93/setup.py
```

### Comparing `daktari-0.0.92/LICENSE.txt` & `daktari-0.0.93/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/PKG-INFO` & `daktari-0.0.93/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daktari
-Version: 0.0.92
+Version: 0.0.93
 Summary: Assist in setting up and maintaining developer environments
 Home-page: https://github.com/sonocent/daktari
 Author: Matt Russell
 Author-email: matthew.russell@sonocent.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,15 @@
 ## Configuration
 
 In the root of the project repository, create a `.daktari.py` configuration file listing the checks you want run. For example,
 
 ```python
 from daktari.checks.git import *
 
-version = "0.0.92"
+version = "0.0.93"
 title = "My Project"
 
 checks = [
     GitInstalled(),
     GitLfsInstalled(),
     GitLfsSetUpForUser(),
     GitLfsFilesDownloaded(),
```

### Comparing `daktari-0.0.92/README.md` & `daktari-0.0.93/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ## Configuration
 
 In the root of the project repository, create a `.daktari.py` configuration file listing the checks you want run. For example,
 
 ```python
 from daktari.checks.git import *
 
-version = "0.0.92"
+version = "0.0.93"
 title = "My Project"
 
 checks = [
     GitInstalled(),
     GitLfsInstalled(),
     GitLfsSetUpForUser(),
     GitLfsFilesDownloaded(),
```

### Comparing `daktari-0.0.92/daktari/__main__.py` & `daktari-0.0.93/daktari/__main__.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/check.py` & `daktari-0.0.93/daktari/check.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/check_runner.py` & `daktari-0.0.93/daktari/check_runner.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/check_sorter.py` & `daktari-0.0.93/daktari/check_sorter.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/check_utils.py` & `daktari-0.0.93/daktari/check_utils.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/checks/certs.py` & `daktari-0.0.93/daktari/checks/certs.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/checks/direnv.py` & `daktari-0.0.93/daktari/checks/direnv.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/checks/docker.py` & `daktari-0.0.93/daktari/checks/docker.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/checks/files.py` & `daktari-0.0.93/daktari/checks/files.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/checks/flutter.py` & `daktari-0.0.93/daktari/checks/flutter.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/checks/git.py` & `daktari-0.0.93/daktari/checks/git.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/checks/google.py` & `daktari-0.0.93/daktari/checks/google.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/checks/intellij_idea.py` & `daktari-0.0.93/daktari/checks/intellij_idea.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/checks/java.py` & `daktari-0.0.93/daktari/checks/java.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/checks/kubernetes.py` & `daktari-0.0.93/daktari/checks/kubernetes.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/checks/misc.py` & `daktari-0.0.93/daktari/checks/misc.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/checks/nodejs.py` & `daktari-0.0.93/daktari/checks/nodejs.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/checks/onepassword.py` & `daktari-0.0.93/daktari/checks/onepassword.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/checks/python.py` & `daktari-0.0.93/daktari/checks/python.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/checks/ssh.py` & `daktari-0.0.93/daktari/checks/ssh.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/checks/terraform.py` & `daktari-0.0.93/daktari/checks/terraform.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/checks/test_certs.py` & `daktari-0.0.93/daktari/checks/test_certs.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/checks/test_java.py` & `daktari-0.0.93/daktari/checks/test_java.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/checks/test_ssh.py` & `daktari-0.0.93/daktari/checks/test_ssh.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/checks/test_yarn.py` & `daktari-0.0.93/daktari/checks/test_yarn.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/checks/xml.py` & `daktari-0.0.93/daktari/checks/xml.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/checks/yarn.py` & `daktari-0.0.93/daktari/checks/yarn.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/command_utils.py` & `daktari-0.0.93/daktari/command_utils.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/config.py` & `daktari-0.0.93/daktari/config.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/file_utils.py` & `daktari-0.0.93/daktari/file_utils.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/options.py` & `daktari-0.0.93/daktari/options.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/os.py` & `daktari-0.0.93/daktari/os.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/result_printer.py` & `daktari-0.0.93/daktari/result_printer.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/test_check.py` & `daktari-0.0.93/daktari/test_check.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/test_check_factory.py` & `daktari-0.0.93/daktari/test_check_factory.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/test_check_sorter.py` & `daktari-0.0.93/daktari/test_check_sorter.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/test_check_utils.py` & `daktari-0.0.93/daktari/test_check_utils.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/test_config.py` & `daktari-0.0.93/daktari/test_config.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/test_version_utils.py` & `daktari-0.0.93/daktari/test_version_utils.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari/version_utils.py` & `daktari-0.0.93/daktari/version_utils.py`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/daktari.egg-info/PKG-INFO` & `daktari-0.0.93/daktari.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daktari
-Version: 0.0.92
+Version: 0.0.93
 Summary: Assist in setting up and maintaining developer environments
 Home-page: https://github.com/sonocent/daktari
 Author: Matt Russell
 Author-email: matthew.russell@sonocent.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,15 @@
 ## Configuration
 
 In the root of the project repository, create a `.daktari.py` configuration file listing the checks you want run. For example,
 
 ```python
 from daktari.checks.git import *
 
-version = "0.0.92"
+version = "0.0.93"
 title = "My Project"
 
 checks = [
     GitInstalled(),
     GitLfsInstalled(),
     GitLfsSetUpForUser(),
     GitLfsFilesDownloaded(),
```

### Comparing `daktari-0.0.92/daktari.egg-info/SOURCES.txt` & `daktari-0.0.93/daktari.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `daktari-0.0.92/requirements.txt` & `daktari-0.0.93/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 semver==3.0.0
 python-hosts==1.0.3
 tabulate==0.9.0
 types-tabulate==0.9.0.2
 PyYAML==6.0
 types-PyYAML==6.0.12.9
 pyobjc-core==9.1.1; sys_platform == 'darwin'
-pyobjc-framework-Cocoa==9.1; sys_platform == 'darwin'
+pyobjc-framework-Cocoa==9.1.1; sys_platform == 'darwin'
 requests-unixsocket==0.3.0
 dpath==2.1.5
 pyOpenSSL==23.1.1
 types-pyOpenSSL==23.1.0.2
```

### Comparing `daktari-0.0.92/setup.py` & `daktari-0.0.93/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setuptools.setup(
     name="daktari",
-    version="0.0.92",
+    version="0.0.93",
     description="Assist in setting up and maintaining developer environments",
     long_description=README,
     long_description_content_type="text/markdown",
     license="MIT",
     author="Matt Russell",
     author_email="matthew.russell@sonocent.com",
     url="https://github.com/sonocent/daktari",
```


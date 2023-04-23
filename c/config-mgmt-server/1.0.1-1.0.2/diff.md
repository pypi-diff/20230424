# Comparing `tmp/config-mgmt-server-1.0.1.tar.gz` & `tmp/config-mgmt-server-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "config-mgmt-server-1.0.1.tar", last modified: Fri Apr 21 21:35:02 2023, max compression
+gzip compressed data, was "config-mgmt-server-1.0.2.tar", last modified: Sun Apr 23 22:12:00 2023, max compression
```

## Comparing `config-mgmt-server-1.0.1.tar` & `config-mgmt-server-1.0.2.tar`

### file list

```diff
@@ -1,27 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:35:02.099201 config-mgmt-server-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-21 21:34:49.000000 config-mgmt-server-1.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-21 21:34:49.000000 config-mgmt-server-1.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-21 21:34:49.000000 config-mgmt-server-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-21 21:35:02.099201 config-mgmt-server-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-21 21:34:49.000000 config-mgmt-server-1.0.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     1918 2023-04-21 21:34:49.000000 config-mgmt-server-1.0.1/_initial_setup.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      725 2023-04-21 21:34:49.000000 config-mgmt-server-1.0.1/_pip_install.sh
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-21 21:34:49.000000 config-mgmt-server-1.0.1/mypy.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)      317 2023-04-21 21:34:49.000000 config-mgmt-server-1.0.1/precommit_hook.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-04-21 21:34:49.000000 config-mgmt-server-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-21 21:34:49.000000 config-mgmt-server-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 21:35:02.099201 config-mgmt-server-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:35:02.095201 config-mgmt-server-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:35:02.095201 config-mgmt-server-1.0.1/src/config_mgmt_server/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-21 21:34:49.000000 config-mgmt-server-1.0.1/src/config_mgmt_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:35:02.099201 config-mgmt-server-1.0.1/src/config_mgmt_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-21 21:35:02.000000 config-mgmt-server-1.0.1/src/config_mgmt_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-21 21:35:02.000000 config-mgmt-server-1.0.1/src/config_mgmt_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 21:35:02.000000 config-mgmt-server-1.0.1/src/config_mgmt_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-21 21:35:02.000000 config-mgmt-server-1.0.1/src/config_mgmt_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-21 21:35:02.000000 config-mgmt-server-1.0.1/src/config_mgmt_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-21 21:35:02.000000 config-mgmt-server-1.0.1/src/config_mgmt_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:35:02.099201 config-mgmt-server-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-21 21:34:49.000000 config-mgmt-server-1.0.1/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-21 21:34:49.000000 config-mgmt-server-1.0.1/tests/test_my_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-21 21:34:49.000000 config-mgmt-server-1.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:12:00.489437 config-mgmt-server-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-23 22:11:44.000000 config-mgmt-server-1.0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-23 22:11:44.000000 config-mgmt-server-1.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-23 22:11:44.000000 config-mgmt-server-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-23 22:12:00.489437 config-mgmt-server-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-23 22:11:44.000000 config-mgmt-server-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-04-23 22:11:44.000000 config-mgmt-server-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-23 22:11:44.000000 config-mgmt-server-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 22:12:00.489437 config-mgmt-server-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:12:00.485437 config-mgmt-server-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:12:00.489437 config-mgmt-server-1.0.2/src/config_mgmt_server/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-23 22:11:44.000000 config-mgmt-server-1.0.2/src/config_mgmt_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-23 22:11:44.000000 config-mgmt-server-1.0.2/src/config_mgmt_server/testService.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:12:00.489437 config-mgmt-server-1.0.2/src/config_mgmt_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-23 22:12:00.000000 config-mgmt-server-1.0.2/src/config_mgmt_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-23 22:12:00.000000 config-mgmt-server-1.0.2/src/config_mgmt_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 22:12:00.000000 config-mgmt-server-1.0.2/src/config_mgmt_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-23 22:12:00.000000 config-mgmt-server-1.0.2/src/config_mgmt_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-23 22:12:00.000000 config-mgmt-server-1.0.2/src/config_mgmt_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-23 22:12:00.000000 config-mgmt-server-1.0.2/src/config_mgmt_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 22:12:00.489437 config-mgmt-server-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-23 22:11:44.000000 config-mgmt-server-1.0.2/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-23 22:11:44.000000 config-mgmt-server-1.0.2/tests/test_my_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-23 22:11:44.000000 config-mgmt-server-1.0.2/tox.ini
```

### Comparing `config-mgmt-server-1.0.1/PKG-INFO` & `config-mgmt-server-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: config-mgmt-server
-Version: 1.0.1
+Version: 1.0.2
 Summary: Suncoast Systems Core Router Config Mgmt Server
 Author-email: Suncoast Systems <administrator@suncoast.systems>
 Maintainer-email: Dotcom Row <dotcom.row@gmail.com>
 License: This project is only for Dotcom Row services, no other use is allowed or even possible!
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Reports, https://github.com/pypa/sampleproject/issues
 Project-URL: Funding, https://donate.pypi.org
```

### Comparing `config-mgmt-server-1.0.1/README.md` & `config-mgmt-server-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `config-mgmt-server-1.0.1/pyproject.toml` & `config-mgmt-server-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "config-mgmt-server"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.1"  # Required
+version = "1.0.2"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "Suncoast Systems Core Router Config Mgmt Server"  # Optional
 
 # This is an optional longer description of your project that represents
@@ -93,15 +93,16 @@
 # This field lists other packages that your project depends on to run.
 # Any package you put here will be installed by pip when your project is
 # installed, so they must be valid existing projects.
 #
 # For an analysis of this field vs pip's requirements files see:
 # https://packaging.python.org/discussions/install-requires-vs-requirements/
 dependencies = [ # Optional
-  "peppercorn"
+  "python-daemon",
+  "flask"
 ]
 
 # List additional groups of dependencies here (e.g. development
 # dependencies). Users will be able to install these using the "extras"
 # syntax, for example:
 #
 #   $ pip install sampleproject[dev]
```

### Comparing `config-mgmt-server-1.0.1/requirements.txt` & `config-mgmt-server-1.0.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `config-mgmt-server-1.0.1/src/config_mgmt_server.egg-info/PKG-INFO` & `config-mgmt-server-1.0.2/src/config_mgmt_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: config-mgmt-server
-Version: 1.0.1
+Version: 1.0.2
 Summary: Suncoast Systems Core Router Config Mgmt Server
 Author-email: Suncoast Systems <administrator@suncoast.systems>
 Maintainer-email: Dotcom Row <dotcom.row@gmail.com>
 License: This project is only for Dotcom Row services, no other use is allowed or even possible!
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Reports, https://github.com/pypa/sampleproject/issues
 Project-URL: Funding, https://donate.pypi.org
```

### Comparing `config-mgmt-server-1.0.1/tests/requirements.txt` & `config-mgmt-server-1.0.2/tests/requirements.txt`

 * *Files identical despite different names*

### Comparing `config-mgmt-server-1.0.1/tox.ini` & `config-mgmt-server-1.0.2/tox.ini`

 * *Files identical despite different names*


# Comparing `tmp/cornflow-core-0.1.8.tar.gz` & `tmp/cornflow-core-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cornflow-core-0.1.8.tar", last modified: Mon Feb 13 19:50:38 2023, max compression
+gzip compressed data, was "dist/cornflow-core-0.1.9.tar", last modified: Mon Mar  6 09:54:47 2023, max compression
```

## Comparing `cornflow-core-0.1.8.tar` & `cornflow-core-0.1.9.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-13 19:50:38.000000 cornflow-core-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (116)    10766 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       72 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     8974 2023-02-13 19:50:38.000000 cornflow-core-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     6877 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-13 19:50:38.000000 cornflow-core-0.1.8/cornflow_core/
--rw-r--r--   0 runner    (1001) docker     (116)       16 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-13 19:50:38.000000 cornflow-core-0.1.8/cornflow_core/authentication/
--rw-r--r--   0 runner    (1001) docker     (116)      141 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    13745 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/authentication/auth.py
--rw-r--r--   0 runner    (1001) docker     (116)     1282 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/authentication/decorators.py
--rw-r--r--   0 runner    (1001) docker     (116)     4853 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/authentication/ldap.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-13 19:50:38.000000 cornflow-core-0.1.8/cornflow_core/cli/
--rw-r--r--   0 runner    (1001) docker     (116)       37 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2505 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/cli/generate_from_schema.py
--rw-r--r--   0 runner    (1001) docker     (116)     1852 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/cli/schema_from_models.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-13 19:50:38.000000 cornflow-core-0.1.8/cornflow_core/cli/tools/
--rw-r--r--   0 runner    (1001) docker     (116)       19 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/cli/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    16935 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/cli/tools/api_generator.py
--rw-r--r--   0 runner    (1001) docker     (116)    10747 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/cli/tools/endpoint_tools.py
--rw-r--r--   0 runner    (1001) docker     (116)     5520 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/cli/tools/models_tools.py
--rw-r--r--   0 runner    (1001) docker     (116)     7540 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/cli/tools/schema_generator.py
--rw-r--r--   0 runner    (1001) docker     (116)     2298 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/cli/tools/schemas_tools.py
--rw-r--r--   0 runner    (1001) docker     (116)      122 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/cli/tools/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-13 19:50:38.000000 cornflow-core-0.1.8/cornflow_core/compress/
--rw-r--r--   0 runner    (1001) docker     (116)      100 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/compress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1347 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/compress/compress.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-13 19:50:38.000000 cornflow-core-0.1.8/cornflow_core/constants/
--rw-r--r--   0 runner    (1001) docker     (116)       80 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      604 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/constants/authentication.py
--rw-r--r--   0 runner    (1001) docker     (116)      346 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/constants/roles.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-13 19:50:38.000000 cornflow-core-0.1.8/cornflow_core/exceptions/
--rw-r--r--   0 runner    (1001) docker     (116)       89 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4487 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-13 19:50:38.000000 cornflow-core-0.1.8/cornflow_core/messages/
--rw-r--r--   0 runner    (1001) docker     (116)       95 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3435 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/messages/email.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-13 19:50:38.000000 cornflow-core-0.1.8/cornflow_core/models/
--rw-r--r--   0 runner    (1001) docker     (116)      407 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1218 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/models/action.py
--rw-r--r--   0 runner    (1001) docker     (116)    11975 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/models/meta_models.py
--rw-r--r--   0 runner    (1001) docker     (116)     2795 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/models/permissions.py
--rw-r--r--   0 runner    (1001) docker     (116)     2063 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/models/role.py
--rw-r--r--   0 runner    (1001) docker     (116)     8063 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/models/user.py
--rw-r--r--   0 runner    (1001) docker     (116)     4941 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/models/user_role.py
--rw-r--r--   0 runner    (1001) docker     (116)     2036 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/models/view.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-13 19:50:38.000000 cornflow-core-0.1.8/cornflow_core/resources/
--rw-r--r--   0 runner    (1001) docker     (116)      255 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6242 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/resources/log_in.py
--rw-r--r--   0 runner    (1001) docker     (116)     8478 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/resources/meta_resource.py
--rw-r--r--   0 runner    (1001) docker     (116)     2165 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/resources/recover_password.py
--rw-r--r--   0 runner    (1001) docker     (116)     2721 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/resources/sign_up.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-13 19:50:38.000000 cornflow-core-0.1.8/cornflow_core/schemas/
--rw-r--r--   0 runner    (1001) docker     (116)      541 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      340 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/schemas/action.py
--rw-r--r--   0 runner    (1001) docker     (116)      260 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/schemas/patch.py
--rw-r--r--   0 runner    (1001) docker     (116)     1282 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/schemas/permissions.py
--rw-r--r--   0 runner    (1001) docker     (116)      984 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/schemas/query.py
--rw-r--r--   0 runner    (1001) docker     (116)      469 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/schemas/role.py
--rw-r--r--   0 runner    (1001) docker     (116)     1218 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/schemas/user.py
--rw-r--r--   0 runner    (1001) docker     (116)      615 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/schemas/user_role.py
--rw-r--r--   0 runner    (1001) docker     (116)      429 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/schemas/view.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-13 19:50:38.000000 cornflow-core-0.1.8/cornflow_core/shared/
--rw-r--r--   0 runner    (1001) docker     (116)      295 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      681 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/shared/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     3441 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/shared/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-13 19:50:38.000000 cornflow-core-0.1.8/cornflow_core/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    12262 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/tests/test_generate_from_schema.py
--rw-r--r--   0 runner    (1001) docker     (116)     3640 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/cornflow_core/tests/test_schema_from_models.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-13 19:50:38.000000 cornflow-core-0.1.8/cornflow_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     8974 2023-02-13 19:50:38.000000 cornflow-core-0.1.8/cornflow_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2123 2023-02-13 19:50:38.000000 cornflow-core-0.1.8/cornflow_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-02-13 19:50:38.000000 cornflow-core-0.1.8/cornflow_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      179 2023-02-13 19:50:38.000000 cornflow-core-0.1.8/cornflow_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      229 2023-02-13 19:50:38.000000 cornflow-core-0.1.8/cornflow_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       14 2023-02-13 19:50:38.000000 cornflow-core-0.1.8/cornflow_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-02-13 19:50:38.000000 cornflow-core-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1164 2023-02-13 19:50:36.000000 cornflow-core-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:47.000000 cornflow-core-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (116)    10766 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)       72 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     8974 2023-03-06 09:54:47.000000 cornflow-core-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     6877 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:47.000000 cornflow-core-0.1.9/cornflow_core/
+-rw-r--r--   0 runner    (1001) docker     (116)       16 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:47.000000 cornflow-core-0.1.9/cornflow_core/authentication/
+-rw-r--r--   0 runner    (1001) docker     (116)      141 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13745 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/authentication/auth.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1282 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/authentication/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4853 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/authentication/ldap.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:47.000000 cornflow-core-0.1.9/cornflow_core/cli/
+-rw-r--r--   0 runner    (1001) docker     (116)       37 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2505 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/cli/generate_from_schema.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1852 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/cli/schema_from_models.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:47.000000 cornflow-core-0.1.9/cornflow_core/cli/tools/
+-rw-r--r--   0 runner    (1001) docker     (116)       19 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/cli/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16935 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/cli/tools/api_generator.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10747 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/cli/tools/endpoint_tools.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5520 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/cli/tools/models_tools.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7540 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/cli/tools/schema_generator.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2298 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/cli/tools/schemas_tools.py
+-rw-r--r--   0 runner    (1001) docker     (116)      122 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/cli/tools/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:47.000000 cornflow-core-0.1.9/cornflow_core/compress/
+-rw-r--r--   0 runner    (1001) docker     (116)      100 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/compress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1347 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/compress/compress.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:47.000000 cornflow-core-0.1.9/cornflow_core/constants/
+-rw-r--r--   0 runner    (1001) docker     (116)       80 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      604 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/constants/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (116)      346 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/constants/roles.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:47.000000 cornflow-core-0.1.9/cornflow_core/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (116)       89 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4487 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:47.000000 cornflow-core-0.1.9/cornflow_core/messages/
+-rw-r--r--   0 runner    (1001) docker     (116)       95 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3435 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/messages/email.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:47.000000 cornflow-core-0.1.9/cornflow_core/models/
+-rw-r--r--   0 runner    (1001) docker     (116)      407 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1218 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/models/action.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11975 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/models/meta_models.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2795 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/models/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2063 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/models/role.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8063 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4941 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/models/user_role.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2036 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/models/view.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:47.000000 cornflow-core-0.1.9/cornflow_core/resources/
+-rw-r--r--   0 runner    (1001) docker     (116)      255 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6242 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/resources/log_in.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8478 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/resources/meta_resource.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2165 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/resources/recover_password.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2721 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/resources/sign_up.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:47.000000 cornflow-core-0.1.9/cornflow_core/schemas/
+-rw-r--r--   0 runner    (1001) docker     (116)      541 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      340 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/schemas/action.py
+-rw-r--r--   0 runner    (1001) docker     (116)      260 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/schemas/patch.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1282 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/schemas/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (116)      984 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/schemas/query.py
+-rw-r--r--   0 runner    (1001) docker     (116)      469 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/schemas/role.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1218 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/schemas/user.py
+-rw-r--r--   0 runner    (1001) docker     (116)      615 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/schemas/user_role.py
+-rw-r--r--   0 runner    (1001) docker     (116)      429 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/schemas/view.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:47.000000 cornflow-core-0.1.9/cornflow_core/shared/
+-rw-r--r--   0 runner    (1001) docker     (116)      229 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      681 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/shared/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2921 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/shared/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:47.000000 cornflow-core-0.1.9/cornflow_core/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12262 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/tests/test_generate_from_schema.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3640 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/cornflow_core/tests/test_schema_from_models.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:47.000000 cornflow-core-0.1.9/cornflow_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     8974 2023-03-06 09:54:47.000000 cornflow-core-0.1.9/cornflow_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2123 2023-03-06 09:54:47.000000 cornflow-core-0.1.9/cornflow_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-06 09:54:47.000000 cornflow-core-0.1.9/cornflow_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      179 2023-03-06 09:54:47.000000 cornflow-core-0.1.9/cornflow_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      229 2023-03-06 09:54:47.000000 cornflow-core-0.1.9/cornflow_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       14 2023-03-06 09:54:47.000000 cornflow-core-0.1.9/cornflow_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2023-03-06 09:54:47.000000 cornflow-core-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1164 2023-03-06 09:54:45.000000 cornflow-core-0.1.9/setup.py
```

### Comparing `cornflow-core-0.1.8/LICENSE` & `cornflow-core-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cornflow-core-0.1.8/PKG-INFO` & `cornflow-core-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cornflow-core
-Version: 0.1.8
+Version: 0.1.9
 Summary: REST API flask backend components used by cornflow and other REST APIs
 Home-page: https://github.com/baobabsoluciones/cornflow
 Author: baobab soluciones
 Author-email: sistemas@baobabsoluciones.es
 License: UNKNOWN
 Description: ==============
         Cornflow-tools
```

### Comparing `cornflow-core-0.1.8/README.rst` & `cornflow-core-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `cornflow-core-0.1.8/cornflow_core/authentication/auth.py` & `cornflow-core-0.1.9/cornflow_core/authentication/auth.py`

 * *Files identical despite different names*

### Comparing `cornflow-core-0.1.8/cornflow_core/authentication/decorators.py` & `cornflow-core-0.1.9/cornflow_core/authentication/decorators.py`

 * *Files identical despite different names*

### Comparing `cornflow-core-0.1.8/cornflow_core/authentication/ldap.py` & `cornflow-core-0.1.9/cornflow_core/authentication/ldap.py`

 * *Files identical despite different names*

### Comparing `cornflow-core-0.1.8/cornflow_core/cli/generate_from_schema.py` & `cornflow-core-0.1.9/cornflow_core/cli/generate_from_schema.py`

 * *Files identical despite different names*

### Comparing `cornflow-core-0.1.8/cornflow_core/cli/schema_from_models.py` & `cornflow-core-0.1.9/cornflow_core/cli/schema_from_models.py`

 * *Files identical despite different names*

### Comparing `cornflow-core-0.1.8/cornflow_core/cli/tools/api_generator.py` & `cornflow-core-0.1.9/cornflow_core/cli/tools/api_generator.py`

 * *Files identical despite different names*

### Comparing `cornflow-core-0.1.8/cornflow_core/cli/tools/endpoint_tools.py` & `cornflow-core-0.1.9/cornflow_core/cli/tools/endpoint_tools.py`

 * *Files identical despite different names*

### Comparing `cornflow-core-0.1.8/cornflow_core/cli/tools/models_tools.py` & `cornflow-core-0.1.9/cornflow_core/cli/tools/models_tools.py`

 * *Files identical despite different names*

### Comparing `cornflow-core-0.1.8/cornflow_core/cli/tools/schema_generator.py` & `cornflow-core-0.1.9/cornflow_core/cli/tools/schema_generator.py`

 * *Files identical despite different names*

### Comparing `cornflow-core-0.1.8/cornflow_core/cli/tools/schemas_tools.py` & `cornflow-core-0.1.9/cornflow_core/cli/tools/schemas_tools.py`

 * *Files identical despite different names*

### Comparing `cornflow-core-0.1.8/cornflow_core/compress/compress.py` & `cornflow-core-0.1.9/cornflow_core/compress/compress.py`

 * *Files identical despite different names*

### Comparing `cornflow-core-0.1.8/cornflow_core/constants/authentication.py` & `cornflow-core-0.1.9/cornflow_core/constants/authentication.py`

 * *Files identical despite different names*

### Comparing `cornflow-core-0.1.8/cornflow_core/exceptions/exceptions.py` & `cornflow-core-0.1.9/cornflow_core/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `cornflow-core-0.1.8/cornflow_core/messages/email.py` & `cornflow-core-0.1.9/cornflow_core/messages/email.py`

 * *Files identical despite different names*

### Comparing `cornflow-core-0.1.8/cornflow_core/models/action.py` & `cornflow-core-0.1.9/cornflow_core/models/action.py`

 * *Files identical despite different names*

### Comparing `cornflow-core-0.1.8/cornflow_core/models/meta_models.py` & `cornflow-core-0.1.9/cornflow_core/models/meta_models.py`

 * *Files identical despite different names*

### Comparing `cornflow-core-0.1.8/cornflow_core/models/permissions.py` & `cornflow-core-0.1.9/cornflow_core/models/permissions.py`

 * *Files identical despite different names*

### Comparing `cornflow-core-0.1.8/cornflow_core/models/role.py` & `cornflow-core-0.1.9/cornflow_core/models/role.py`

 * *Files identical despite different names*

### Comparing `cornflow-core-0.1.8/cornflow_core/models/user.py` & `cornflow-core-0.1.9/cornflow_core/models/user.py`

 * *Files identical despite different names*

### Comparing `cornflow-core-0.1.8/cornflow_core/models/user_role.py` & `cornflow-core-0.1.9/cornflow_core/models/user_role.py`

 * *Files identical despite different names*

### Comparing `cornflow-core-0.1.8/cornflow_core/models/view.py` & `cornflow-core-0.1.9/cornflow_core/models/view.py`

 * *Files identical despite different names*

### Comparing `cornflow-core-0.1.8/cornflow_core/resources/log_in.py` & `cornflow-core-0.1.9/cornflow_core/resources/log_in.py`

 * *Files identical despite different names*

### Comparing `cornflow-core-0.1.8/cornflow_core/resources/meta_resource.py` & `cornflow-core-0.1.9/cornflow_core/resources/meta_resource.py`

 * *Files identical despite different names*

### Comparing `cornflow-core-0.1.8/cornflow_core/resources/recover_password.py` & `cornflow-core-0.1.9/cornflow_core/resources/recover_password.py`

 * *Files identical despite different names*

### Comparing `cornflow-core-0.1.8/cornflow_core/resources/sign_up.py` & `cornflow-core-0.1.9/cornflow_core/resources/sign_up.py`

 * *Files identical despite different names*

### Comparing `cornflow-core-0.1.8/cornflow_core/schemas/__init__.py` & `cornflow-core-0.1.9/cornflow_core/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `cornflow-core-0.1.8/cornflow_core/schemas/permissions.py` & `cornflow-core-0.1.9/cornflow_core/schemas/permissions.py`

 * *Files identical despite different names*

### Comparing `cornflow-core-0.1.8/cornflow_core/schemas/query.py` & `cornflow-core-0.1.9/cornflow_core/schemas/query.py`

 * *Files identical despite different names*

### Comparing `cornflow-core-0.1.8/cornflow_core/schemas/user.py` & `cornflow-core-0.1.9/cornflow_core/schemas/user.py`

 * *Files identical despite different names*

### Comparing `cornflow-core-0.1.8/cornflow_core/schemas/user_role.py` & `cornflow-core-0.1.9/cornflow_core/schemas/user_role.py`

 * *Files identical despite different names*

### Comparing `cornflow-core-0.1.8/cornflow_core/shared/utils.py` & `cornflow-core-0.1.9/cornflow_core/shared/utils.py`

 * *Files identical despite different names*

### Comparing `cornflow-core-0.1.8/cornflow_core/shared/validators.py` & `cornflow-core-0.1.9/cornflow_core/shared/validators.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """
 This file has several validators used on cornflow core
 """
 import re
 from typing import Tuple, Union
 
 from jsonschema import Draft7Validator
-from marshmallow import ValidationError
-from cornflow_core.exceptions import InvalidUsage
 from disposable_email_domains import blocklist
 
 
 def is_special_character(character):
     """
     Method to return if a character is a special character
 
@@ -64,28 +62,14 @@
         return False, "Invalid email address."
     domain = email.split("@")[1]
     if domain in blocklist:
         return False, "Invalid email address"
     return True, None
 
 
-def validate_and_continue(obj, data):
-    """
-    Method to validate data against an object
-    """
-    try:
-        validate = obj.load(data)
-    except ValidationError as e:
-        raise InvalidUsage(error=f"Bad data format: {e}")
-    err = ""
-    if validate is None:
-        raise InvalidUsage(error=f"Bad data format: {err}")
-    return validate
-
-
 def json_schema_validate(schema: dict, data: dict) -> list:
     """
     Method to validate some data against a json schema
 
     :param dict schema:the json schema in dict format.
     :param dict data: the data to validate in dict format
     :return: a list with the errors found
@@ -103,13 +87,7 @@
 
     :param dict schema:the json schema in dict format.
     :param dict data: the data to validate in dict format
     :return: a list with the errors found
     :rtype: list
     """
     return [str(e) for e in json_schema_validate(schema, data)]
-
-
-"""
-Aliases
-"""
-marshmallow_validate_and_continue = validate_and_continue
```

### Comparing `cornflow-core-0.1.8/cornflow_core/tests/test_generate_from_schema.py` & `cornflow-core-0.1.9/cornflow_core/tests/test_generate_from_schema.py`

 * *Files identical despite different names*

### Comparing `cornflow-core-0.1.8/cornflow_core/tests/test_schema_from_models.py` & `cornflow-core-0.1.9/cornflow_core/tests/test_schema_from_models.py`

 * *Files identical despite different names*

### Comparing `cornflow-core-0.1.8/cornflow_core.egg-info/PKG-INFO` & `cornflow-core-0.1.9/cornflow_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cornflow-core
-Version: 0.1.8
+Version: 0.1.9
 Summary: REST API flask backend components used by cornflow and other REST APIs
 Home-page: https://github.com/baobabsoluciones/cornflow
 Author: baobab soluciones
 Author-email: sistemas@baobabsoluciones.es
 License: UNKNOWN
 Description: ==============
         Cornflow-tools
```

### Comparing `cornflow-core-0.1.8/cornflow_core.egg-info/SOURCES.txt` & `cornflow-core-0.1.9/cornflow_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cornflow-core-0.1.8/setup.py` & `cornflow-core-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 required = []
 with open("requirements.txt", "r") as fh:
     required.append(fh.read().splitlines())
 
 setuptools.setup(
     name="cornflow-core",
-    version="0.1.8",
+    version="0.1.9",
     author="baobab soluciones",
     author_email="sistemas@baobabsoluciones.es",
     description="REST API flask backend components used by cornflow and other REST APIs",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/baobabsoluciones/cornflow",
     packages=setuptools.find_packages(),
```


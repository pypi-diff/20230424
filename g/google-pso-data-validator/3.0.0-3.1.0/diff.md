# Comparing `tmp/google-pso-data-validator-3.0.0.tar.gz` & `tmp/google-pso-data-validator-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-pso-data-validator-3.0.0.tar", last modified: Thu Mar 30 17:29:48 2023, max compression
+gzip compressed data, was "google-pso-data-validator-3.1.0.tar", last modified: Mon Apr 24 05:22:28 2023, max compression
```

## Comparing `google-pso-data-validator-3.0.0.tar` & `google-pso-data-validator-3.1.0.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 17:29:48.448330 google-pso-data-validator-3.0.0/
--rw-r--r--   0 root         (0) root         (0)    11358 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    35955 2023-03-30 17:29:48.448330 google-pso-data-validator-3.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    35243 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 17:29:48.420328 google-pso-data-validator-3.0.0/data_validation/
--rw-r--r--   0 root         (0) root         (0)      715 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/data_validation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20441 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/data_validation/__main__.py
--rw-r--r--   0 root         (0) root         (0)     1986 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/data_validation/app.py
--rw-r--r--   0 root         (0) root         (0)    43663 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/data_validation/cli_tools.py
--rw-r--r--   0 root         (0) root         (0)      881 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/data_validation/client_info.py
--rw-r--r--   0 root         (0) root         (0)    10258 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/data_validation/clients.py
--rw-r--r--   0 root         (0) root         (0)    13911 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/data_validation/combiner.py
--rw-r--r--   0 root         (0) root         (0)    34285 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/data_validation/config_manager.py
--rw-r--r--   0 root         (0) root         (0)     5052 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/data_validation/consts.py
--rw-r--r--   0 root         (0) root         (0)    16222 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/data_validation/data_validation.py
--rw-r--r--   0 root         (0) root         (0)      632 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/data_validation/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1269 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/data_validation/jellyfish_distance.py
--rw-r--r--   0 root         (0) root         (0)     2497 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/data_validation/metadata.py
--rw-r--r--   0 root         (0) root         (0)    10638 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/data_validation/partition_builder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 17:29:48.424329 google-pso-data-validator-3.0.0/data_validation/query_builder/
--rw-r--r--   0 root         (0) root         (0)      575 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/data_validation/query_builder/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2880 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/data_validation/query_builder/partition_row_builder.py
--rw-r--r--   0 root         (0) root         (0)    18741 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/data_validation/query_builder/query_builder.py
--rw-r--r--   0 root         (0) root         (0)     7409 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/data_validation/query_builder/random_row_builder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 17:29:48.424329 google-pso-data-validator-3.0.0/data_validation/result_handlers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/data_validation/result_handlers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3970 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/data_validation/result_handlers/bigquery.py
--rw-r--r--   0 root         (0) root         (0)     2440 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/data_validation/result_handlers/text.py
--rw-r--r--   0 root         (0) root         (0)    11146 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/data_validation/schema_validation.py
--rw-r--r--   0 root         (0) root         (0)     1773 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/data_validation/secret_manager.py
--rw-r--r--   0 root         (0) root         (0)     9477 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/data_validation/state_manager.py
--rw-r--r--   0 root         (0) root         (0)    16109 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/data_validation/validation_builder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 17:29:48.428329 google-pso-data-validator-3.0.0/google_pso_data_validator.egg-info/
--rw-r--r--   0 root         (0) root         (0)    35955 2023-03-30 17:29:48.000000 google-pso-data-validator-3.0.0/google_pso_data_validator.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3483 2023-03-30 17:29:48.000000 google-pso-data-validator-3.0.0/google_pso_data_validator.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-30 17:29:48.000000 google-pso-data-validator-3.0.0/google_pso_data_validator.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-03-30 17:29:48.000000 google-pso-data-validator-3.0.0/google_pso_data_validator.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      587 2023-03-30 17:29:48.000000 google-pso-data-validator-3.0.0/google_pso_data_validator.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2023-03-30 17:29:48.000000 google-pso-data-validator-3.0.0/google_pso_data_validator.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       67 2023-03-30 17:29:48.452330 google-pso-data-validator-3.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2877 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 17:29:48.404327 google-pso-data-validator-3.0.0/third_party/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 17:29:48.408327 google-pso-data-validator-3.0.0/third_party/ibis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 17:29:48.428329 google-pso-data-validator-3.0.0/third_party/ibis/ibis_DB2/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_DB2/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3365 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_DB2/alchemy.py
--rw-r--r--   0 root         (0) root         (0)     1198 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_DB2/api.py
--rw-r--r--   0 root         (0) root         (0)     6460 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_DB2/client.py
--rw-r--r--   0 root         (0) root         (0)    18605 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_DB2/compiler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 17:29:48.432329 google-pso-data-validator-3.0.0/third_party/ibis/ibis_DB2/expr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_DB2/expr/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4952 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_DB2/expr/datatypes.py
--rw-r--r--   0 root         (0) root         (0)     2373 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_DB2/expr/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 17:29:48.432329 google-pso-data-validator-3.0.0/third_party/ibis/ibis_addon/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_addon/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1524 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_addon/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 17:29:48.432329 google-pso-data-validator-3.0.0/third_party/ibis/ibis_addon/base_sqlalchemy/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_addon/base_sqlalchemy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2519 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_addon/base_sqlalchemy/alchemy.py
--rw-r--r--   0 root         (0) root         (0)     3551 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_addon/datatypes.py
--rw-r--r--   0 root         (0) root         (0)    11436 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_addon/operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 17:29:48.436329 google-pso-data-validator-3.0.0/third_party/ibis/ibis_cloud_spanner/
--rw-r--r--   0 root         (0) root         (0)        2 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_cloud_spanner/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2069 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_cloud_spanner/api.py
--rw-r--r--   0 root         (0) root         (0)    14574 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_cloud_spanner/client.py
--rw-r--r--   0 root         (0) root         (0)     1898 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_cloud_spanner/compiler.py
--rw-r--r--   0 root         (0) root         (0)     2750 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_cloud_spanner/datatypes.py
--rw-r--r--   0 root         (0) root         (0)     3789 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_cloud_spanner/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 17:29:48.436329 google-pso-data-validator-3.0.0/third_party/ibis/ibis_cloud_spanner/tests/
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_cloud_spanner/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4944 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_cloud_spanner/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)    14058 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_cloud_spanner/tests/test_client.py
--rw-r--r--   0 root         (0) root         (0)    14908 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_cloud_spanner/tests/test_compiler.py
--rw-r--r--   0 root         (0) root         (0)     1916 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_cloud_spanner/tests/test_datatypes.py
--rw-r--r--   0 root         (0) root         (0)     1494 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_cloud_spanner/to_pandas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 17:29:48.440330 google-pso-data-validator-3.0.0/third_party/ibis/ibis_impala/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_impala/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6555 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_impala/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 17:29:48.440330 google-pso-data-validator-3.0.0/third_party/ibis/ibis_mssql/
--rw-r--r--   0 root         (0) root         (0)       69 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_mssql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4042 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_mssql/api.py
--rw-r--r--   0 root         (0) root         (0)     8284 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_mssql/client.py
--rw-r--r--   0 root         (0) root         (0)    14803 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_mssql/compiler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 17:29:48.440330 google-pso-data-validator-3.0.0/third_party/ibis/ibis_mssql/expr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_mssql/expr/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4032 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_mssql/expr/api.py
--rw-r--r--   0 root         (0) root         (0)     1867 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_mssql/expr/operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 17:29:48.444330 google-pso-data-validator-3.0.0/third_party/ibis/ibis_oracle/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_oracle/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2135 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_oracle/alchemy.py
--rw-r--r--   0 root         (0) root         (0)     1215 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_oracle/api.py
--rw-r--r--   0 root         (0) root         (0)     9748 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_oracle/client.py
--rw-r--r--   0 root         (0) root         (0)    17172 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_oracle/compiler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 17:29:48.444330 google-pso-data-validator-3.0.0/third_party/ibis/ibis_oracle/expr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_oracle/expr/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6010 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_oracle/expr/datatypes.py
--rw-r--r--   0 root         (0) root         (0)     2449 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_oracle/expr/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 17:29:48.444330 google-pso-data-validator-3.0.0/third_party/ibis/ibis_oracle/udf/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_oracle/udf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6995 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_oracle/udf/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 17:29:48.448330 google-pso-data-validator-3.0.0/third_party/ibis/ibis_postgres/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_postgres/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4788 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_postgres/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 17:29:48.448330 google-pso-data-validator-3.0.0/third_party/ibis/ibis_teradata/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_teradata/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1494 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_teradata/api.py
--rw-r--r--   0 root         (0) root         (0)     9302 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_teradata/client.py
--rw-r--r--   0 root         (0) root         (0)    26138 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_teradata/compiler.py
--rw-r--r--   0 root         (0) root         (0)     4738 2023-03-30 17:28:14.000000 google-pso-data-validator-3.0.0/third_party/ibis/ibis_teradata/datatypes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.948369 google-pso-data-validator-3.1.0/
+-rw-r--r--   0 root         (0) root         (0)    11358 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    35942 2023-04-24 05:22:28.948369 google-pso-data-validator-3.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    35230 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.912366 google-pso-data-validator-3.1.0/data_validation/
+-rw-r--r--   0 root         (0) root         (0)      715 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20439 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     1986 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/app.py
+-rw-r--r--   0 root         (0) root         (0)    44528 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/cli_tools.py
+-rw-r--r--   0 root         (0) root         (0)      881 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/client_info.py
+-rw-r--r--   0 root         (0) root         (0)    10258 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/clients.py
+-rw-r--r--   0 root         (0) root         (0)    13911 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/combiner.py
+-rw-r--r--   0 root         (0) root         (0)    34285 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/config_manager.py
+-rw-r--r--   0 root         (0) root         (0)     5052 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/consts.py
+-rw-r--r--   0 root         (0) root         (0)    16222 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/data_validation.py
+-rw-r--r--   0 root         (0) root         (0)      632 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1269 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/jellyfish_distance.py
+-rw-r--r--   0 root         (0) root         (0)     2497 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/metadata.py
+-rw-r--r--   0 root         (0) root         (0)    10638 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/partition_builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.916366 google-pso-data-validator-3.1.0/data_validation/query_builder/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/query_builder/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2880 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/query_builder/partition_row_builder.py
+-rw-r--r--   0 root         (0) root         (0)    18741 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/query_builder/query_builder.py
+-rw-r--r--   0 root         (0) root         (0)     7520 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/query_builder/random_row_builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.916366 google-pso-data-validator-3.1.0/data_validation/result_handlers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/result_handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3970 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/result_handlers/bigquery.py
+-rw-r--r--   0 root         (0) root         (0)     2548 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/result_handlers/text.py
+-rw-r--r--   0 root         (0) root         (0)    11146 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/schema_validation.py
+-rw-r--r--   0 root         (0) root         (0)     1773 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/secret_manager.py
+-rw-r--r--   0 root         (0) root         (0)     9477 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/state_manager.py
+-rw-r--r--   0 root         (0) root         (0)    16109 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/data_validation/validation_builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.920367 google-pso-data-validator-3.1.0/google_pso_data_validator.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    35942 2023-04-24 05:22:28.000000 google-pso-data-validator-3.1.0/google_pso_data_validator.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3483 2023-04-24 05:22:28.000000 google-pso-data-validator-3.1.0/google_pso_data_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 05:22:28.000000 google-pso-data-validator-3.1.0/google_pso_data_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-04-24 05:22:28.000000 google-pso-data-validator-3.1.0/google_pso_data_validator.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      587 2023-04-24 05:22:28.000000 google-pso-data-validator-3.1.0/google_pso_data_validator.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-24 05:22:28.000000 google-pso-data-validator-3.1.0/google_pso_data_validator.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2023-04-24 05:22:28.948369 google-pso-data-validator-3.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2877 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.892365 google-pso-data-validator-3.1.0/third_party/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.900365 google-pso-data-validator-3.1.0/third_party/ibis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.924367 google-pso-data-validator-3.1.0/third_party/ibis/ibis_DB2/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_DB2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3434 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_DB2/alchemy.py
+-rw-r--r--   0 root         (0) root         (0)     1198 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_DB2/api.py
+-rw-r--r--   0 root         (0) root         (0)     7727 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_DB2/client.py
+-rw-r--r--   0 root         (0) root         (0)    18668 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_DB2/compiler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.924367 google-pso-data-validator-3.1.0/third_party/ibis/ibis_DB2/expr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_DB2/expr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4949 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_DB2/expr/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)     2373 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_DB2/expr/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.928367 google-pso-data-validator-3.1.0/third_party/ibis/ibis_addon/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_addon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1524 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_addon/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.928367 google-pso-data-validator-3.1.0/third_party/ibis/ibis_addon/base_sqlalchemy/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_addon/base_sqlalchemy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7579 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_addon/base_sqlalchemy/alchemy.py
+-rw-r--r--   0 root         (0) root         (0)     3551 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_addon/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)    12820 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_addon/operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.932368 google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/
+-rw-r--r--   0 root         (0) root         (0)        2 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2069 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/api.py
+-rw-r--r--   0 root         (0) root         (0)    14574 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/client.py
+-rw-r--r--   0 root         (0) root         (0)     1898 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/compiler.py
+-rw-r--r--   0 root         (0) root         (0)     2750 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)     3789 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.932368 google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/tests/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4944 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)    14058 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/tests/test_client.py
+-rw-r--r--   0 root         (0) root         (0)    14908 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/tests/test_compiler.py
+-rw-r--r--   0 root         (0) root         (0)     1916 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/tests/test_datatypes.py
+-rw-r--r--   0 root         (0) root         (0)     1494 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/to_pandas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.936368 google-pso-data-validator-3.1.0/third_party/ibis/ibis_impala/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_impala/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7010 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_impala/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.936368 google-pso-data-validator-3.1.0/third_party/ibis/ibis_mssql/
+-rw-r--r--   0 root         (0) root         (0)       69 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_mssql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4042 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_mssql/api.py
+-rw-r--r--   0 root         (0) root         (0)     8514 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_mssql/client.py
+-rw-r--r--   0 root         (0) root         (0)    14803 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_mssql/compiler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.940368 google-pso-data-validator-3.1.0/third_party/ibis/ibis_mssql/expr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_mssql/expr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4032 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_mssql/expr/api.py
+-rw-r--r--   0 root         (0) root         (0)     1867 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_mssql/expr/operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.940368 google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2135 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/alchemy.py
+-rw-r--r--   0 root         (0) root         (0)     1215 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/api.py
+-rw-r--r--   0 root         (0) root         (0)     9908 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/client.py
+-rw-r--r--   0 root         (0) root         (0)    17172 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/compiler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.944369 google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/expr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/expr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6010 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/expr/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)     2449 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/expr/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.944369 google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/udf/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/udf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6995 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/udf/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.944369 google-pso-data-validator-3.1.0/third_party/ibis/ibis_postgres/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_postgres/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4788 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_postgres/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 05:22:28.948369 google-pso-data-validator-3.1.0/third_party/ibis/ibis_teradata/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_teradata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1494 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_teradata/api.py
+-rw-r--r--   0 root         (0) root         (0)     9302 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_teradata/client.py
+-rw-r--r--   0 root         (0) root         (0)    26138 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_teradata/compiler.py
+-rw-r--r--   0 root         (0) root         (0)     4738 2023-04-24 05:20:49.000000 google-pso-data-validator-3.1.0/third_party/ibis/ibis_teradata/datatypes.py
```

### Comparing `google-pso-data-validator-3.0.0/LICENSE` & `google-pso-data-validator-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/PKG-INFO` & `google-pso-data-validator-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-pso-data-validator
-Version: 3.0.0
+Version: 3.1.0
 Summary: A package to enable easy data validation
 Home-page: https://github.com/pypa/sampleproject
 Author: Dylan Hercher
 Author-email: dhercher@google.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -30,15 +30,15 @@
 compared to ensure they are matched and correct after each migration step
 (e.g. data and schema migration, SQL script translation, ETL migration, etc.).
 The Data Validation Tool (DVT) provides an automated and repeatable solution to
 perform this task.
 
 DVT supports the following validations:
 * Column validation (count, sum, avg, min, max, group by)
-* Row validation (BQ, Hive, Teradata, Oracle, SQL Server, Postgres only)
+* Row validation (BQ, Hive, Teradata, Oracle, SQL Server, Postgres, Mysql only)
 * Schema validation 
 * Custom Query validation
 * Ad hoc SQL exploration
 
 DVT supports the following connection types:
 
 *   [BigQuery](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#google-bigquery)
@@ -152,15 +152,15 @@
 The default aggregation type is a 'COUNT *'. If no aggregation flag (i.e count,
 sum , min, etc.) is provided, the default aggregation will run.
 
 The [Examples](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/examples.md) page provides many examples of how a tool can be used to run powerful validations without writing any queries.
 
 #### Row Validations
 
-(Note: Row hash validation is currently supported for BigQuery, Teradata, Impala/Hive, Oracle, SQL Server, Postgres, and Alloy DB. Struct and array data types are not currently supported.
+(Note: Row hash validation is currently supported for BigQuery, Teradata, Impala/Hive, Oracle, SQL Server, Postgres, Mysql, Db2 and Alloy DB. Struct and array data types are not currently supported.
 In addition, please note that SHA256 is not a supported function on Teradata systems. 
 If you wish to perform this comparison on Teradata you will need to 
 [deploy a UDF to perform the conversion](https://github.com/akuroda/teradata-udf-sha2/blob/master/src/sha256.c).)
 
 Below is the command syntax for row validations. In order to run row level
 validations you need to pass a `--primary-key` flag which defines what field(s)
 the validation will be compared on, as well as either the `--comparison-fields` flag
@@ -249,15 +249,15 @@
   --concat COLUMNS      Comma separated list of columns to concatenate or * for all columns (use if a common hash function is not available between databases)
   --config-dir CONFIG_DIR, -cdir CONFIG_DIR
                         Directory Path to store YAML Config Files
                         GCS: Provide a full gs:// path of the target directory. Eg: `gs://<BUCKET>/partitions_dir`
                         Local: Provide a relative path of the target directory. Eg: `partitions_dir`
   --partition-num [1-1000], -pn [1-1000]
                         Number of partitions/config files to generate
-                        In case this value exceeds the row count of the source/target table, its will be decreased to max(source_row_count, target_row_count)
+                        In case this value exceeds the row count of the source/target table, it will be decreased to max(source_row_count, target_row_count)
   [--partition-key PARTITION_KEY, -partkey PARTITION_KEY]
                         Column on which the partitions would be generated. Column type must be integer. Defaults to Primary key
   [--filters SOURCE_FILTER:TARGET_FILTER]
                         Colon spearated string values of source and target filters.
                         If target filter is not provided, the source filter will run on source and target tables.
                         See: *Filters* section
 ```
@@ -472,21 +472,20 @@
 
 -   Pulls all tables in the source (applying a supplied allowed-schemas filter)
 -   Pulls all tables from the target
 -   Uses Levenshtein distance to match tables
 -   Finally, it prints a JSON list of tables which can be a reference for the
     validation run config.
 
-Note that our score cutoff default is a 0.8, which was manually tested to be an
-accurate value. If no matches occur, reduce this value.
+Note that our score cutoff default is 1. If no matches occur, reduce this value as deemed necessary.
 
 ```
 data-validation find-tables --source-conn source --target-conn target \
     --allowed-schemas pso_data_validator \
-    --score-cutoff 0.8
+    --score-cutoff 1
 ```
 
 ### Using Beta CLI Features
 
 There may be occasions we want to release a new CLI feature under a Beta flag.
 Any features under Beta may or may not make their way to production. However, if
 there is a Beta feature you wish to use than it can be accessed using the
@@ -508,15 +507,15 @@
 ### Aggregated Fields
 
 Aggregate fields contain the SQL fields that you want to produce an aggregate
 for. Currently the functions `COUNT()`, `AVG()`, `SUM()`, `MIN()`, and `MAX()`
 are supported.
 
 Here is a sample aggregate config:
-```
+```yaml
 validations:
 - aggregates:
     - field_alias: count
     source_column: null
     target_column: null
     type: count
     - field_alias: count__tripduration
@@ -601,15 +600,15 @@
       target_calculated_columns: ['rtrim_col_a', 'ltrim_col_b']
       type: concat
       depth: 1 # calculated one query above
 ```
 
 is equivalent to the following SQL query...
 
-```
+```sql
 SELECT
   CONCAT(rtrim_col_a, rtrim_col_b) AS concat_col_a_col_b
 FROM (
   SELECT
       RTRIM(col_a) AS rtrim_col_a
     , LTRIM(col_b) AS ltrim_col_b
   FROM my.table
```

### Comparing `google-pso-data-validator-3.0.0/README.md` & `google-pso-data-validator-3.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 compared to ensure they are matched and correct after each migration step
 (e.g. data and schema migration, SQL script translation, ETL migration, etc.).
 The Data Validation Tool (DVT) provides an automated and repeatable solution to
 perform this task.
 
 DVT supports the following validations:
 * Column validation (count, sum, avg, min, max, group by)
-* Row validation (BQ, Hive, Teradata, Oracle, SQL Server, Postgres only)
+* Row validation (BQ, Hive, Teradata, Oracle, SQL Server, Postgres, Mysql only)
 * Schema validation 
 * Custom Query validation
 * Ad hoc SQL exploration
 
 DVT supports the following connection types:
 
 *   [BigQuery](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#google-bigquery)
@@ -132,15 +132,15 @@
 The default aggregation type is a 'COUNT *'. If no aggregation flag (i.e count,
 sum , min, etc.) is provided, the default aggregation will run.
 
 The [Examples](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/examples.md) page provides many examples of how a tool can be used to run powerful validations without writing any queries.
 
 #### Row Validations
 
-(Note: Row hash validation is currently supported for BigQuery, Teradata, Impala/Hive, Oracle, SQL Server, Postgres, and Alloy DB. Struct and array data types are not currently supported.
+(Note: Row hash validation is currently supported for BigQuery, Teradata, Impala/Hive, Oracle, SQL Server, Postgres, Mysql, Db2 and Alloy DB. Struct and array data types are not currently supported.
 In addition, please note that SHA256 is not a supported function on Teradata systems. 
 If you wish to perform this comparison on Teradata you will need to 
 [deploy a UDF to perform the conversion](https://github.com/akuroda/teradata-udf-sha2/blob/master/src/sha256.c).)
 
 Below is the command syntax for row validations. In order to run row level
 validations you need to pass a `--primary-key` flag which defines what field(s)
 the validation will be compared on, as well as either the `--comparison-fields` flag
@@ -229,15 +229,15 @@
   --concat COLUMNS      Comma separated list of columns to concatenate or * for all columns (use if a common hash function is not available between databases)
   --config-dir CONFIG_DIR, -cdir CONFIG_DIR
                         Directory Path to store YAML Config Files
                         GCS: Provide a full gs:// path of the target directory. Eg: `gs://<BUCKET>/partitions_dir`
                         Local: Provide a relative path of the target directory. Eg: `partitions_dir`
   --partition-num [1-1000], -pn [1-1000]
                         Number of partitions/config files to generate
-                        In case this value exceeds the row count of the source/target table, its will be decreased to max(source_row_count, target_row_count)
+                        In case this value exceeds the row count of the source/target table, it will be decreased to max(source_row_count, target_row_count)
   [--partition-key PARTITION_KEY, -partkey PARTITION_KEY]
                         Column on which the partitions would be generated. Column type must be integer. Defaults to Primary key
   [--filters SOURCE_FILTER:TARGET_FILTER]
                         Colon spearated string values of source and target filters.
                         If target filter is not provided, the source filter will run on source and target tables.
                         See: *Filters* section
 ```
@@ -452,21 +452,20 @@
 
 -   Pulls all tables in the source (applying a supplied allowed-schemas filter)
 -   Pulls all tables from the target
 -   Uses Levenshtein distance to match tables
 -   Finally, it prints a JSON list of tables which can be a reference for the
     validation run config.
 
-Note that our score cutoff default is a 0.8, which was manually tested to be an
-accurate value. If no matches occur, reduce this value.
+Note that our score cutoff default is 1. If no matches occur, reduce this value as deemed necessary.
 
 ```
 data-validation find-tables --source-conn source --target-conn target \
     --allowed-schemas pso_data_validator \
-    --score-cutoff 0.8
+    --score-cutoff 1
 ```
 
 ### Using Beta CLI Features
 
 There may be occasions we want to release a new CLI feature under a Beta flag.
 Any features under Beta may or may not make their way to production. However, if
 there is a Beta feature you wish to use than it can be accessed using the
@@ -488,15 +487,15 @@
 ### Aggregated Fields
 
 Aggregate fields contain the SQL fields that you want to produce an aggregate
 for. Currently the functions `COUNT()`, `AVG()`, `SUM()`, `MIN()`, and `MAX()`
 are supported.
 
 Here is a sample aggregate config:
-```
+```yaml
 validations:
 - aggregates:
     - field_alias: count
     source_column: null
     target_column: null
     type: count
     - field_alias: count__tripduration
@@ -581,15 +580,15 @@
       target_calculated_columns: ['rtrim_col_a', 'ltrim_col_b']
       type: concat
       depth: 1 # calculated one query above
 ```
 
 is equivalent to the following SQL query...
 
-```
+```sql
 SELECT
   CONCAT(rtrim_col_a, rtrim_col_b) AS concat_col_a_col_b
 FROM (
   SELECT
       RTRIM(col_a) AS rtrim_col_a
     , LTRIM(col_b) AS ltrim_col_b
   FROM my.table
```

### Comparing `google-pso-data-validator-3.0.0/data_validation/__init__.py` & `google-pso-data-validator-3.1.0/data_validation/__init__.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/data_validation/__main__.py` & `google-pso-data-validator-3.1.0/data_validation/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -370,15 +370,15 @@
         }
 
     return table_map
 
 
 def find_tables_using_string_matching(args):
     """Return JSON String with matched tables for use in validations."""
-    score_cutoff = args.score_cutoff or 0.8
+    score_cutoff = args.score_cutoff or 1
 
     mgr = state_manager.StateManager()
     source_client = clients.get_data_client(mgr.get_connection_config(args.source_conn))
     target_client = clients.get_data_client(mgr.get_connection_config(args.target_conn))
 
     allowed_schemas = cli_tools.get_arg_list(args.allowed_schemas)
     source_table_map = get_table_map(source_client, allowed_schemas=allowed_schemas)
```

### Comparing `google-pso-data-validator-3.0.0/data_validation/app.py` & `google-pso-data-validator-3.1.0/data_validation/app.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/data_validation/cli_tools.py` & `google-pso-data-validator-3.1.0/data_validation/cli_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,14 +124,30 @@
         ["port", "Desired Imapala port (10000 if not provided)"],
         ["database", "Desired Impala database (default if not provided)"],
         ["auth_mechanism", "Desired Impala auth mechanism (PLAIN if not provided)"],
         [
             "kerberos_service_name",
             "Desired Kerberos service name ('impala' if not provided)",
         ],
+        ["use_ssl", "Use SSL when connecting to HiveServer2 (default is False)"],
+        [
+            "timeout",
+            "Connection timeout in seconds when communicating with HiveServer2 (default is 45)",
+        ],
+        [
+            "ca_cert",
+            "Local path to 3rd party CA certificate or copy of server certificate for self-signed certificates. If SSL is enabled, but this argument is None, then certificate validation is skipped.",
+        ],
+        ["user", "LDAP user to authenticate"],
+        ["password", "LDAP password to authenticate"],
+        [
+            "pool_size",
+            "Size of the connection pool. Typically this is not necessary to configure. (default is 8)",
+        ],
+        ["hdfs_client", "An existing HDFS client"],
     ],
     "DB2": [
         ["host", "Desired DB2 host"],
         ["port", "Desired DB2 port (50000 if not provided)"],
         ["user", "Username to connect to"],
         ["password", "Password for authentication of user"],
         ["database", "Database in DB2 to connect to"],
@@ -968,17 +984,17 @@
     mgr.create_connection(connection_name, conn)
 
 
 def list_connections():
     """List all saved connections."""
     mgr = state_manager.StateManager()
     connections = mgr.list_connections()
-
     for conn_name in connections:
-        logging.info(f"Connection Name: {conn_name}")
+        source_type = mgr.get_connection_config(conn_name).get("source_type")
+        logging.info(f"Connection Name: {conn_name} : {source_type}")
 
 
 def get_connection(connection_name):
     """Return dict connection details for a specific connection."""
     mgr = state_manager.StateManager()
     return mgr.get_connection_config(connection_name)
```

### Comparing `google-pso-data-validator-3.0.0/data_validation/client_info.py` & `google-pso-data-validator-3.1.0/data_validation/client_info.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/data_validation/clients.py` & `google-pso-data-validator-3.1.0/data_validation/clients.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/data_validation/combiner.py` & `google-pso-data-validator-3.1.0/data_validation/combiner.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/data_validation/config_manager.py` & `google-pso-data-validator-3.1.0/data_validation/config_manager.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/data_validation/consts.py` & `google-pso-data-validator-3.1.0/data_validation/consts.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/data_validation/data_validation.py` & `google-pso-data-validator-3.1.0/data_validation/data_validation.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/data_validation/exceptions.py` & `google-pso-data-validator-3.1.0/data_validation/exceptions.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/data_validation/jellyfish_distance.py` & `google-pso-data-validator-3.1.0/data_validation/jellyfish_distance.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/data_validation/metadata.py` & `google-pso-data-validator-3.1.0/data_validation/metadata.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/data_validation/partition_builder.py` & `google-pso-data-validator-3.1.0/data_validation/partition_builder.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/data_validation/query_builder/__init__.py` & `google-pso-data-validator-3.1.0/data_validation/query_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/data_validation/query_builder/partition_row_builder.py` & `google-pso-data-validator-3.1.0/data_validation/query_builder/partition_row_builder.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/data_validation/query_builder/query_builder.py` & `google-pso-data-validator-3.1.0/data_validation/query_builder/query_builder.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/data_validation/query_builder/random_row_builder.py` & `google-pso-data-validator-3.1.0/data_validation/query_builder/random_row_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 import ibis.backends.base_sqlalchemy.alchemy as sqla
 import ibis.backends.pandas.execution.util as pandas_util
 
 from ibis_bigquery import BigQueryClient
 from ibis.backends.impala.client import ImpalaClient
 from ibis.backends.pandas.client import PandasClient
 from ibis.backends.postgres.client import PostgreSQLClient
+from ibis.backends.mysql.client import MySQLClient
 from ibis.expr.signature import Argument as Arg
 from data_validation import clients
 from data_validation.query_builder.query_builder import QueryBuilder
 
 
 """ The QueryBuilder for retreiving random row values to filter against."""
 
@@ -48,14 +49,16 @@
     PandasClient: "NA",
     BigQueryClient: "RAND()",
     clients.TeradataClient: None,
     ImpalaClient: "RAND()",
     clients.OracleClient: "DBMS_RANDOM.VALUE",
     PostgreSQLClient: "RANDOM()",
     clients.MSSQLClient: "NEWID()",
+    clients.DB2Client: "RAND()",
+    MySQLClient: "RAND()",
 }
 
 
 class RandomSortExpr(tz.AnyValue, tz.SortExpr):
     _dtype = rlz.string
     _name = "RandomSortExpr"
```

### Comparing `google-pso-data-validator-3.0.0/data_validation/result_handlers/bigquery.py` & `google-pso-data-validator-3.1.0/data_validation/result_handlers/bigquery.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/data_validation/result_handlers/text.py` & `google-pso-data-validator-3.1.0/data_validation/result_handlers/text.py`

 * *Files 18% similar despite different names*

```diff
@@ -41,19 +41,19 @@
         Utility for printing formatted results
         :param result_df
         """
         if self.status_list is not None:
             result_df = filter_validation_status(self.status_list, result_df)
 
         if self.format == "text":
-            print(result_df.to_string(index=False))
+            print(result_df.drop(self.cols_filter_list, axis=1).to_string(index=False))
         elif self.format == "csv":
-            print(result_df.to_csv(index=False))
+            print(result_df.drop(self.cols_filter_list, axis=1).to_csv(index=False))
         elif self.format == "json":
-            print(result_df.to_json(orient="index"))
+            print(result_df.drop(self.cols_filter_list, axis=1).to_json(orient="index"))
         else:
             print(
                 result_df.drop(self.cols_filter_list, axis=1).to_markdown(
                     tablefmt="fancy_grid", index=False
                 )
             )
```

### Comparing `google-pso-data-validator-3.0.0/data_validation/schema_validation.py` & `google-pso-data-validator-3.1.0/data_validation/schema_validation.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/data_validation/secret_manager.py` & `google-pso-data-validator-3.1.0/data_validation/secret_manager.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/data_validation/state_manager.py` & `google-pso-data-validator-3.1.0/data_validation/state_manager.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/data_validation/validation_builder.py` & `google-pso-data-validator-3.1.0/data_validation/validation_builder.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/google_pso_data_validator.egg-info/PKG-INFO` & `google-pso-data-validator-3.1.0/google_pso_data_validator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-pso-data-validator
-Version: 3.0.0
+Version: 3.1.0
 Summary: A package to enable easy data validation
 Home-page: https://github.com/pypa/sampleproject
 Author: Dylan Hercher
 Author-email: dhercher@google.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -30,15 +30,15 @@
 compared to ensure they are matched and correct after each migration step
 (e.g. data and schema migration, SQL script translation, ETL migration, etc.).
 The Data Validation Tool (DVT) provides an automated and repeatable solution to
 perform this task.
 
 DVT supports the following validations:
 * Column validation (count, sum, avg, min, max, group by)
-* Row validation (BQ, Hive, Teradata, Oracle, SQL Server, Postgres only)
+* Row validation (BQ, Hive, Teradata, Oracle, SQL Server, Postgres, Mysql only)
 * Schema validation 
 * Custom Query validation
 * Ad hoc SQL exploration
 
 DVT supports the following connection types:
 
 *   [BigQuery](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/connections.md#google-bigquery)
@@ -152,15 +152,15 @@
 The default aggregation type is a 'COUNT *'. If no aggregation flag (i.e count,
 sum , min, etc.) is provided, the default aggregation will run.
 
 The [Examples](https://github.com/GoogleCloudPlatform/professional-services-data-validator/blob/develop/docs/examples.md) page provides many examples of how a tool can be used to run powerful validations without writing any queries.
 
 #### Row Validations
 
-(Note: Row hash validation is currently supported for BigQuery, Teradata, Impala/Hive, Oracle, SQL Server, Postgres, and Alloy DB. Struct and array data types are not currently supported.
+(Note: Row hash validation is currently supported for BigQuery, Teradata, Impala/Hive, Oracle, SQL Server, Postgres, Mysql, Db2 and Alloy DB. Struct and array data types are not currently supported.
 In addition, please note that SHA256 is not a supported function on Teradata systems. 
 If you wish to perform this comparison on Teradata you will need to 
 [deploy a UDF to perform the conversion](https://github.com/akuroda/teradata-udf-sha2/blob/master/src/sha256.c).)
 
 Below is the command syntax for row validations. In order to run row level
 validations you need to pass a `--primary-key` flag which defines what field(s)
 the validation will be compared on, as well as either the `--comparison-fields` flag
@@ -249,15 +249,15 @@
   --concat COLUMNS      Comma separated list of columns to concatenate or * for all columns (use if a common hash function is not available between databases)
   --config-dir CONFIG_DIR, -cdir CONFIG_DIR
                         Directory Path to store YAML Config Files
                         GCS: Provide a full gs:// path of the target directory. Eg: `gs://<BUCKET>/partitions_dir`
                         Local: Provide a relative path of the target directory. Eg: `partitions_dir`
   --partition-num [1-1000], -pn [1-1000]
                         Number of partitions/config files to generate
-                        In case this value exceeds the row count of the source/target table, its will be decreased to max(source_row_count, target_row_count)
+                        In case this value exceeds the row count of the source/target table, it will be decreased to max(source_row_count, target_row_count)
   [--partition-key PARTITION_KEY, -partkey PARTITION_KEY]
                         Column on which the partitions would be generated. Column type must be integer. Defaults to Primary key
   [--filters SOURCE_FILTER:TARGET_FILTER]
                         Colon spearated string values of source and target filters.
                         If target filter is not provided, the source filter will run on source and target tables.
                         See: *Filters* section
 ```
@@ -472,21 +472,20 @@
 
 -   Pulls all tables in the source (applying a supplied allowed-schemas filter)
 -   Pulls all tables from the target
 -   Uses Levenshtein distance to match tables
 -   Finally, it prints a JSON list of tables which can be a reference for the
     validation run config.
 
-Note that our score cutoff default is a 0.8, which was manually tested to be an
-accurate value. If no matches occur, reduce this value.
+Note that our score cutoff default is 1. If no matches occur, reduce this value as deemed necessary.
 
 ```
 data-validation find-tables --source-conn source --target-conn target \
     --allowed-schemas pso_data_validator \
-    --score-cutoff 0.8
+    --score-cutoff 1
 ```
 
 ### Using Beta CLI Features
 
 There may be occasions we want to release a new CLI feature under a Beta flag.
 Any features under Beta may or may not make their way to production. However, if
 there is a Beta feature you wish to use than it can be accessed using the
@@ -508,15 +507,15 @@
 ### Aggregated Fields
 
 Aggregate fields contain the SQL fields that you want to produce an aggregate
 for. Currently the functions `COUNT()`, `AVG()`, `SUM()`, `MIN()`, and `MAX()`
 are supported.
 
 Here is a sample aggregate config:
-```
+```yaml
 validations:
 - aggregates:
     - field_alias: count
     source_column: null
     target_column: null
     type: count
     - field_alias: count__tripduration
@@ -601,15 +600,15 @@
       target_calculated_columns: ['rtrim_col_a', 'ltrim_col_b']
       type: concat
       depth: 1 # calculated one query above
 ```
 
 is equivalent to the following SQL query...
 
-```
+```sql
 SELECT
   CONCAT(rtrim_col_a, rtrim_col_b) AS concat_col_a_col_b
 FROM (
   SELECT
       RTRIM(col_a) AS rtrim_col_a
     , LTRIM(col_b) AS ltrim_col_b
   FROM my.table
```

### Comparing `google-pso-data-validator-3.0.0/google_pso_data_validator.egg-info/SOURCES.txt` & `google-pso-data-validator-3.1.0/google_pso_data_validator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/google_pso_data_validator.egg-info/requires.txt` & `google-pso-data-validator-3.1.0/google_pso_data_validator.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/setup.py` & `google-pso-data-validator-3.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import os
 
 import setuptools
 
 name = "google-pso-data-validator"
 description = "A package to enable easy data validation"
-version = "3.0.0"
+version = "3.1.0"
 release_status = "Development Status :: 3 - Alpha"
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 dependencies = [
     # Dependency corrections from our requirements
```

### Comparing `google-pso-data-validator-3.0.0/third_party/ibis/ibis_DB2/alchemy.py` & `google-pso-data-validator-3.1.0/third_party/ibis/ibis_DB2/alchemy.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     dt.CLOB: sa.CLOB,
     dt.BLOB: sa.BLOB,
     dt.SMALLINT: sa.SMALLINT,
     dt.INTEGER: sa.INTEGER,
     dt.BIGINT: sa.BIGINT,
 }
 _ibis_type_to_sqla.update(s_al._ibis_type_to_sqla)
+_ibis_type_to_sqla[dts.String] = sa.sql.sqltypes.String(length=3000)
 
 
 def _to_sqla_type(itype, type_map=None):
     if type_map is None:
         type_map = _ibis_type_to_sqla
     if isinstance(itype, dt11.Decimal):
         return sa.types.NUMERIC(itype.precision, itype.scale)
```

### Comparing `google-pso-data-validator-3.0.0/third_party/ibis/ibis_DB2/api.py` & `google-pso-data-validator-3.1.0/third_party/ibis/ibis_DB2/api.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/third_party/ibis/ibis_DB2/client.py` & `google-pso-data-validator-3.1.0/third_party/ibis/ibis_DB2/client.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,17 +13,18 @@
 # limitations under the License.
 
 import contextlib
 import getpass
 from typing import Optional
 
 import sqlalchemy as sa
-
+import ibis.expr.operations as ops
 import third_party.ibis.ibis_DB2.alchemy as alch
 from third_party.ibis.ibis_DB2.compiler import DB2Dialect
+import ibis.expr.schema as sch
 
 
 class DB2Table(alch.AlchemyTable):
     pass
 
 
 class DB2Schema(alch.AlchemyDatabaseSchema):
@@ -194,8 +195,46 @@
                 like=like, schema=schema
             )
         else:
             parent = super(DB2Client, self)
             return parent.list_tables(like=like, schema=schema)
 
     def get_schema(self, name, schema=None):
-        return self.table(name, schema=schema).schema()
+        return self.table(name, schema=schema).schema()
+
+    def sql(self, query):
+        """
+        Convert a DB2 query to an Ibis table expression
+
+        Parameters
+        ----------
+        query: string
+           SQL query to execute on connection
+
+        Returns
+        -------
+        table : TableExpr
+        """
+        limited_query = 'SELECT * FROM ({}) t0 LIMIT 1'.format(query)
+        schema = self._get_schema_using_query(limited_query)
+        return ops.SQLQueryResult(query, schema, self).to_expr()
+
+    def _get_schema_using_query(self, limited_query):
+        type_map = {
+            'INTEGER': 'int64',
+            'BOOLEAN': 'boolean',
+            'FLOAT': 'float64',
+            'VARCHAR': 'string',
+            'DOUBLE': 'float64'
+        }
+
+        with self._execute(limited_query, results=True) as cur:
+            names = []
+            ibis_types = []
+            for row in cur.proxy._cursor_description():
+                names.append(row[0].lower())
+                datatypes = list(row[1])
+                for datatype in datatypes: 
+                    if datatype in type_map:
+                        ibis_types.append(type_map[datatype])
+                        break
+        return sch.Schema(names, ibis_types)
```

### Comparing `google-pso-data-validator-3.0.0/third_party/ibis/ibis_DB2/compiler.py` & `google-pso-data-validator-3.1.0/third_party/ibis/ibis_DB2/compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -489,15 +489,16 @@
         return sa.cast(result, ibm_db_sa.double)
     else:
         return result
 
 
 def _string_join(t, expr):
     sep, elements = expr.op().args
-    return sa.func.concat(*map(t.translate, elements))
+    columns = [col.name for col in map(t.translate, elements)]
+    return sa.sql.literal_column(" || ".join(columns))
 
 
 def _literal(t, expr):
     dtype = expr.type()
     op = expr.op()
     value = op.value
```

### Comparing `google-pso-data-validator-3.0.0/third_party/ibis/ibis_DB2/expr/datatypes.py` & `google-pso-data-validator-3.1.0/third_party/ibis/ibis_DB2/expr/datatypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         )
     ]
 )
 _TYPE_RULES.update(dt._TYPE_RULES)
 _TYPE_KEYS = tuple(_TYPE_RULES.keys())
 
 
-class TypeParser_Oracle(dt.TypeParser):
+class TypeParser_DB2(dt.TypeParser):
     def type(self) -> dt.DataType:
         if self._accept(Token_DB2.CLOB):
             return CLOB()
         elif self._accept(Token_DB2.BLOB):
             return BLOB()
         elif self._accept(Token_DB2.DBCLOB):
             return DBCLOB()
```

### Comparing `google-pso-data-validator-3.0.0/third_party/ibis/ibis_DB2/expr/types.py` & `google-pso-data-validator-3.1.0/third_party/ibis/ibis_DB2/expr/types.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/third_party/ibis/ibis_addon/api.py` & `google-pso-data-validator-3.1.0/third_party/ibis/ibis_addon/api.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/third_party/ibis/ibis_addon/datatypes.py` & `google-pso-data-validator-3.1.0/third_party/ibis/ibis_addon/datatypes.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/third_party/ibis/ibis_addon/operations.py` & `google-pso-data-validator-3.1.0/third_party/ibis/ibis_addon/operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,32 +25,42 @@
 
 import ibis
 import sqlalchemy as sa
 
 import ibis.expr.api
 import ibis.expr.datatypes as dt
 import ibis.expr.rules as rlz
+import ibis.expr.operations as ops
 
 from data_validation.clients import _raise_missing_client_error
 from ibis_bigquery.compiler import (
     reduction as bq_reduction,
     BigQueryExprTranslator,
     STRFTIME_FORMAT_FUNCTIONS as BQ_STRFTIME_FORMAT_FUNCTIONS
 )
+from ibis.backends.base_sqlalchemy.alchemy import fixed_arity
 from ibis.expr.operations import Arg, Cast, Comparison, Reduction, Strftime, ValueOp
 from ibis.expr.types import BinaryValue, IntegerColumn, StringValue, NumericValue, TemporalValue
 from ibis.backends.impala.compiler import ImpalaExprTranslator
 from ibis.backends.pandas import client as _pandas_client
 from ibis.backends.base_sqlalchemy.alchemy import AlchemyExprTranslator
 from ibis.backends.base_sqlalchemy.compiler import ExprTranslator
 from ibis.backends.base_sql.compiler import BaseExprTranslator
 from third_party.ibis.ibis_oracle.compiler import OracleExprTranslator
 from third_party.ibis.ibis_teradata.compiler import TeradataExprTranslator
 from third_party.ibis.ibis_mssql.compiler import MSSQLExprTranslator
 from ibis.backends.postgres.compiler import PostgreSQLExprTranslator
+from ibis.backends.mysql.compiler import MySQLExprTranslator
+
+# avoid errors if Db2 is not installed and not needed
+try:
+    from third_party.ibis.ibis_DB2.compiler import DB2ExprTranslator
+except Exception:
+    DB2ExprTranslator = None
+
 
 # from third_party.ibis.ibis_snowflake.compiler import SnowflakeExprTranslator
 # from third_party.ibis.ibis_oracle.compiler import OracleExprTranslator <<<<<< DB2
 
 class BitXor(Reduction):
     """Aggregate bitwise XOR operation."""
 
@@ -209,27 +219,44 @@
 
 def sa_format_hashbytes_oracle(translator, expr):
     arg, how = expr.op().args
     compiled_arg = translator.translate(arg)
     hash_func = sa.func.standard_hash(compiled_arg, sa.sql.literal_column("'SHA256'"))
     return sa.func.lower(hash_func)
 
+def sa_format_hashbytes_mysql(translator, expr):
+    arg, how = expr.op().args
+    compiled_arg = translator.translate(arg)
+    hash_func = sa.func.sha2(compiled_arg, sa.sql.literal_column("'256'"))
+    return hash_func
+
+def sa_format_hashbytes_db2(translator, expr):
+    arg, how = expr.op().args
+    compiled_arg = translator.translate(arg)
+    hashfunc = sa.func.hash(compiled_arg,sa.sql.literal_column("2"))
+    hex = sa.func.hex(hashfunc)
+    return sa.func.lower(hex)
+
 def sa_format_hashbytes_postgres(translator, expr):
     arg, how = expr.op().args
     compiled_arg = translator.translate(arg)
     convert = sa.func.convert_to(compiled_arg, sa.sql.literal_column("'UTF8'"))
     hash_func = sa.func.sha256(convert)
     return sa.func.encode(hash_func, sa.sql.literal_column("'hex'"))
 
 def sa_format_to_char(translator, expr):
     arg, fmt = expr.op().args
     compiled_arg = translator.translate(arg)
     compiled_fmt = translator.translate(fmt)
     return sa.func.to_char(compiled_arg, compiled_fmt)
 
+def sa_format_to_stringjoin(translator, expr):
+    sep, elements = expr.op().args
+    return sa.func.concat_ws(translator.translate(sep), *map(translator.translate, elements))
+
 
 def sa_cast_postgres(t, expr):
     arg, typ = expr.op().args
 
     sa_arg = t.translate(arg)
     sa_type = t.get_sqla_type(typ)
 
@@ -288,7 +315,14 @@
 OracleExprTranslator._registry[ToChar] = sa_format_to_char
 TeradataExprTranslator._registry[RawSQL] = format_raw_sql
 TeradataExprTranslator._registry[HashBytes] = format_hashbytes_teradata
 PostgreSQLExprTranslator._registry[HashBytes] = sa_format_hashbytes_postgres
 PostgreSQLExprTranslator._registry[RawSQL] = sa_format_raw_sql
 PostgreSQLExprTranslator._registry[ToChar] = sa_format_to_char
 PostgreSQLExprTranslator._registry[Cast] = sa_cast_postgres
+MySQLExprTranslator._registry[RawSQL] = sa_format_raw_sql
+MySQLExprTranslator._registry[HashBytes] = sa_format_hashbytes_mysql
+MySQLExprTranslator._registry[ops.IfNull] = fixed_arity(sa.func.ifnull, 2)
+MySQLExprTranslator._registry[ops.StringJoin] = sa_format_to_stringjoin
+
+if DB2ExprTranslator: #check if Db2 driver is loaded
+    DB2ExprTranslator._registry[HashBytes] = sa_format_hashbytes_db2
```

### Comparing `google-pso-data-validator-3.0.0/third_party/ibis/ibis_cloud_spanner/api.py` & `google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/api.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/third_party/ibis/ibis_cloud_spanner/client.py` & `google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/client.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/third_party/ibis/ibis_cloud_spanner/compiler.py` & `google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/compiler.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/third_party/ibis/ibis_cloud_spanner/datatypes.py` & `google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/datatypes.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/third_party/ibis/ibis_cloud_spanner/table.py` & `google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/table.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/third_party/ibis/ibis_cloud_spanner/tests/conftest.py` & `google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/third_party/ibis/ibis_cloud_spanner/tests/test_client.py` & `google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/third_party/ibis/ibis_cloud_spanner/tests/test_compiler.py` & `google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/third_party/ibis/ibis_cloud_spanner/tests/test_datatypes.py` & `google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/third_party/ibis/ibis_cloud_spanner/to_pandas.py` & `google-pso-data-validator-3.1.0/third_party/ibis/ibis_cloud_spanner/to_pandas.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/third_party/ibis/ibis_impala/api.py` & `google-pso-data-validator-3.1.0/third_party/ibis/ibis_impala/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,27 +29,45 @@
 
 def impala_connect(
     host=None,
     port=10000,
     database="default",
     auth_mechanism="PLAIN",
     kerberos_service_name="impala",
+    use_ssl=False,
+    timeout=45,
+    ca_cert=None,
+    user=None,
+    password=None,
+    pool_size=8,
+    hdfs_client=None
 ):
     auth_mechanism = (auth_mechanism, "PLAIN")[auth_mechanism is None]
     database = (database, "default")[database is None]
     port = (port, 10000)[port is None]
     kerberos_service_name = (kerberos_service_name, "impala")[
         kerberos_service_name is None
     ]
+    use_ssl = (use_ssl, False)[use_ssl is None]
+    timeout = (timeout, 45)[timeout is None]
+    pool_size = (pool_size, 8)[pool_size is None]
+    
     return connect(
         host=host,
         port=int(port),
         database=database,
         auth_mechanism=auth_mechanism,
         kerberos_service_name=kerberos_service_name,
+        use_ssl=use_ssl,
+        timeout=timeout,
+        ca_cert=ca_cert,
+        user=user,
+        password=password,
+        pool_size=pool_size,
+        hdfs_client=hdfs_client
     )
 
 
 def parse_type(t):
     """Returns the Ibis datatype from source type."""
     t = t.lower()
     if t in _impala_to_ibis_type:
```

### Comparing `google-pso-data-validator-3.0.0/third_party/ibis/ibis_mssql/api.py` & `google-pso-data-validator-3.1.0/third_party/ibis/ibis_mssql/api.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/third_party/ibis/ibis_mssql/client.py` & `google-pso-data-validator-3.1.0/third_party/ibis/ibis_mssql/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,24 +25,35 @@
 import ibis.expr.datatypes as dt
 import ibis.expr.operations as ops
 import ibis.expr.schema as sch
 from third_party.ibis.ibis_mssql.compiler import MSSQLDialect
 
 import pyodbc  # NOQA fail early if the driver is missing
 
+
 @dt.dtype.register(MSDialect_pyodbc, sa.dialects.mssql.UNIQUEIDENTIFIER)
 def sa_string(_, satype, nullable=True):
     return dt.String(nullable=nullable)
 
 
 @dt.dtype.register(MSDialect_pyodbc, sa.dialects.mssql.BIT)
 def sa_boolean(_, satype, nullable=True):
     return dt.Boolean(nullable=nullable)
 
 
+@dt.dtype.register(MSDialect_pyodbc, sa.dialects.mssql.DATETIMEOFFSET)
+def sa_timestamp_tz(_, satype, nullable=True):
+    return dt.Timestamp("UTC", nullable=nullable)
+
+
+@dt.dtype.register(MSDialect_pyodbc, sa.dialects.mssql.FLOAT)
+def sa_float64(_, satype, nullable=True):
+    return dt.Float64(nullable=nullable)
+
+
 class MSSQLTable(alch.AlchemyTable):
     pass
 
 
 class MSSQLSchema(alch.AlchemyDatabaseSchema):
     pass
 
@@ -61,37 +72,37 @@
 
     dialect = MSSQLDialect
     database_class = MSSQLDatabase
     table_class = MSSQLTable
 
     def __init__(
         self,
-        host='localhost',
+        host="localhost",
         user=None,
         password=None,
         port=1433,
-        database='master',
+        database="master",
         url=None,
-        driver='pyodbc',
-        odbc_driver='ODBC Driver 17 for SQL Server',
+        driver="pyodbc",
+        odbc_driver="ODBC Driver 17 for SQL Server",
     ):
         if url is None:
-            if driver != 'pyodbc':
+            if driver != "pyodbc":
                 raise NotImplementedError(
-                    'pyodbc is currently the only supported driver'
+                    "pyodbc is currently the only supported driver"
                 )
             user = user or getpass.getuser()
             url = sa.engine.url.URL(
-                'mssql+pyodbc',
+                "mssql+pyodbc",
                 host=host,
                 port=port,
                 username=user,
                 password=password,
                 database=database,
-                query={'driver': odbc_driver},
+                query={"driver": odbc_driver},
             )
         else:
             url = sa.engine.url.make_url(url)
         super().__init__(sa.create_engine(url))
         self.database_name = url.database
 
     @contextlib.contextmanager
@@ -157,28 +168,26 @@
         """Database client is currently connected to."""
         return self.database_name
 
     def list_databases(self):
         """List all databases for client to connect to."""
         return [
             row.name
-            for row in self.con.execute(
-                'SELECT name FROM master.dbo.sysdatabases'
-            )
+            for row in self.con.execute("SELECT name FROM master.dbo.sysdatabases")
         ]
 
     def list_schemas(self):
         """List all the schemas in the current database."""
         return self.inspector.get_schema_names()
 
     def set_database(self, name):
         """Set current database that client is connected to."""
         raise NotImplementedError(
-            'Cannot set database with MSSQL client. To use a different'
-            ' database, use client.database({!r})'.format(name)
+            "Cannot set database with MSSQL client. To use a different"
+            " database, use client.database({!r})".format(name)
         )
 
     @property
     def client(self):
         return self
 
     def table(self, name, database=None, schema=None):
@@ -222,17 +231,15 @@
 
         Returns
         -------
         list
             A list with all tables available for the current database.
         """
         if database is not None and database != self.current_database:
-            return self.database(name=database).list_tables(
-                like=like, schema=schema
-            )
+            return self.database(name=database).list_tables(like=like, schema=schema)
         else:
             parent = super(MSSQLClient, self)
             return parent.list_tables(like=like, schema=schema)
 
     def sql(self, query):
         """
         Convert a MSSQL query to an Ibis table expression
@@ -242,30 +249,28 @@
         query: string
            SQL query to execute on connection
 
         Returns
         -------
         table : TableExpr
         """
-        limited_query = 'SELECT TOP 0 * FROM ({}) t0'.format(query)
+        limited_query = "SELECT TOP 0 * FROM ({}) t0".format(query)
         schema = self._get_schema_using_query(limited_query)
         return ops.SQLQueryResult(query, schema, self).to_expr()
 
     def _get_schema_using_query(self, limited_query):
         type_map = {
-            int: 'int64',
-            bool: 'boolean',
-            float: 'float64',
-            str: 'string',
-            datetime.datetime: 'timestamp',
-            decimal.Decimal: 'Decimal'
+            int: "int64",
+            bool: "boolean",
+            float: "float64",
+            str: "string",
+            datetime.datetime: "timestamp",
+            decimal.Decimal: "Decimal",
         }
 
         with self._execute(limited_query, results=True) as cur:
             names = [row[0] for row in cur.proxy._cursor_description()]
-            ibis_types = [
-                type_map[row[1]] for row in cur.proxy._cursor_description()
-            ]
+            ibis_types = [type_map[row[1]] for row in cur.proxy._cursor_description()]
         return sch.Schema(names, ibis_types)
 
     def get_schema(self, name, schema=None):
-        return self.table(name, schema=schema).schema()
+        return self.table(name, schema=schema).schema()
```

### Comparing `google-pso-data-validator-3.0.0/third_party/ibis/ibis_mssql/compiler.py` & `google-pso-data-validator-3.1.0/third_party/ibis/ibis_mssql/compiler.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/third_party/ibis/ibis_mssql/expr/api.py` & `google-pso-data-validator-3.1.0/third_party/ibis/ibis_mssql/expr/api.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/third_party/ibis/ibis_mssql/expr/operations.py` & `google-pso-data-validator-3.1.0/third_party/ibis/ibis_mssql/expr/operations.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/third_party/ibis/ibis_oracle/alchemy.py` & `google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/alchemy.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/third_party/ibis/ibis_oracle/api.py` & `google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/api.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/third_party/ibis/ibis_oracle/client.py` & `google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,14 +46,19 @@
 @dt.dtype.register(OracleDialect_cx_oracle, sa.dialects.oracle.NUMBER)
 def sa_oracle_NUMBER(_, satype, nullable=True):
     if not satype.precision and not satype.scale:
         return dt.Decimal(38, 0, nullable=nullable)
     return dt.Decimal(satype.precision, satype.scale, nullable=nullable)
 
 
+@dt.dtype.register(OracleDialect_cx_oracle, sa.dialects.oracle.BINARY_DOUBLE)
+def sa_oracle_BINARY_DOUBLE(_, satype, nullable=True):
+    return dt.Float64(nullable=nullable)
+
+
 @dt.dtype.register(OracleDialect_cx_oracle, sa.dialects.oracle.BFILE)
 def sa_oracle_BFILE(_, satype, nullable=True):
     return dt.Binary(nullable=nullable)
 
 
 @dt.dtype.register(OracleDialect_cx_oracle, sa.dialects.oracle.RAW)
 def sa_oracle_RAW(_, satype, nullable=True):
@@ -65,22 +70,25 @@
     return dt.Date(nullable=nullable)
 
 
 @dt.dtype.register(OracleDialect_cx_oracle, sa.dialects.oracle.VARCHAR)
 def sa_oracle_VARCHAR(_, satype, nullable=True):
     return dt.String(nullable=nullable)
 
+
 @dt.dtype.register(OracleDialect_cx_oracle, sa.dialects.oracle.VARCHAR2)
 def sa_oracle_VARCHAR2(_, satype, nullable=True):
     return dt.String(nullable=nullable)
 
+
 @dt.dtype.register(OracleDialect_cx_oracle, sa.dialects.oracle.TIMESTAMP)
 def sa_oracle_TIMESTAMP(_, satype, nullable=True):
     return dt.Timestamp(nullable=nullable)
 
+
 class OracleTable(alch.AlchemyTable):
     pass
 
 
 class OracleSchema(alch.AlchemyDatabaseSchema):
     pass
 
@@ -240,15 +248,15 @@
             return self.database(name=database).list_tables(like=like, schema=schema)
         else:
             parent = super(OracleClient, self)
             return parent.list_tables(like=like, schema=schema)
 
     def get_schema(self, name, schema=None):
         return self.table(name, schema=schema).schema()
-    
+
     def sql(self, query):
         """
         Convert a Oracle query to an Ibis table expression
 
         Parameters
         ----------
         query: string
@@ -263,15 +271,15 @@
         return ops.SQLQueryResult(query, schema, self).to_expr()
 
     def _get_schema_using_query(self, limited_query):
         type_map = {
             "DB_TYPE_NVARCHAR": "string",
             "DB_TYPE_VARCHAR": "string",
             "DB_TYPE_TIMESTAMP": "timestamp",
-            "DB_TYPE_DATE": "timestamp"
+            "DB_TYPE_DATE": "timestamp",
         }
 
         with self._execute(limited_query, results=True) as cur:
             names = [row[0].lower() for row in cur.proxy._cursor_description()]
             ibis_types = []
             for row in cur.proxy._cursor_description():
                 if row[1].name == "DB_TYPE_NUMBER":
@@ -279,9 +287,9 @@
                     if scale > 0:
                         ibis_datatype = "float64"
                     else:
                         ibis_datatype = "int64"
                 else:
                     ibis_datatype = type_map[row[1].name]
                 ibis_types.append(ibis_datatype)
-                
+
         return sch.Schema(names, ibis_types)
```

### Comparing `google-pso-data-validator-3.0.0/third_party/ibis/ibis_oracle/compiler.py` & `google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/compiler.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/third_party/ibis/ibis_oracle/expr/datatypes.py` & `google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/expr/datatypes.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/third_party/ibis/ibis_oracle/expr/types.py` & `google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/expr/types.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/third_party/ibis/ibis_oracle/udf/api.py` & `google-pso-data-validator-3.1.0/third_party/ibis/ibis_oracle/udf/api.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/third_party/ibis/ibis_postgres/client.py` & `google-pso-data-validator-3.1.0/third_party/ibis/ibis_postgres/client.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/third_party/ibis/ibis_teradata/api.py` & `google-pso-data-validator-3.1.0/third_party/ibis/ibis_teradata/api.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/third_party/ibis/ibis_teradata/client.py` & `google-pso-data-validator-3.1.0/third_party/ibis/ibis_teradata/client.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/third_party/ibis/ibis_teradata/compiler.py` & `google-pso-data-validator-3.1.0/third_party/ibis/ibis_teradata/compiler.py`

 * *Files identical despite different names*

### Comparing `google-pso-data-validator-3.0.0/third_party/ibis/ibis_teradata/datatypes.py` & `google-pso-data-validator-3.1.0/third_party/ibis/ibis_teradata/datatypes.py`

 * *Files identical despite different names*


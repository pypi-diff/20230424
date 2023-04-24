# Comparing `tmp/okdata-cli-1.6.0.tar.gz` & `tmp/okdata-cli-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "okdata-cli-1.6.0.tar", last modified: Tue Mar 21 09:48:41 2023, max compression
+gzip compressed data, was "okdata-cli-2.0.0.tar", last modified: Mon Apr 24 11:07:40 2023, max compression
```

## Comparing `okdata-cli-1.6.0.tar` & `okdata-cli-2.0.0.tar`

### file list

```diff
@@ -1,76 +1,66 @@
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-03-21 09:48:41.520621 okdata-cli-1.6.0/
--rw-r--r--   0 simen     (1000) simen     (1000)     1077 2020-04-30 07:54:22.000000 okdata-cli-1.6.0/LICENSE
--rw-r--r--   0 simen     (1000) simen     (1000)     1077 2023-03-21 09:48:41.520621 okdata-cli-1.6.0/PKG-INFO
--rw-r--r--   0 simen     (1000) simen     (1000)      352 2022-08-25 09:06:50.000000 okdata-cli-1.6.0/README.md
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-03-21 09:48:41.516621 okdata-cli-1.6.0/okdata/
--rw-r--r--   0 simen     (1000) simen     (1000)       56 2020-12-09 11:27:37.000000 okdata-cli-1.6.0/okdata/__init__.py
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-03-21 09:48:41.516621 okdata-cli-1.6.0/okdata/cli/
--rw-r--r--   0 simen     (1000) simen     (1000)        0 2020-12-09 11:27:37.000000 okdata-cli-1.6.0/okdata/cli/__init__.py
--rw-r--r--   0 simen     (1000) simen     (1000)     2584 2023-03-08 09:01:18.000000 okdata-cli-1.6.0/okdata/cli/__main__.py
--rw-r--r--   0 simen     (1000) simen     (1000)     4199 2023-03-21 09:47:26.000000 okdata-cli-1.6.0/okdata/cli/command.py
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-03-21 09:48:41.516621 okdata-cli-1.6.0/okdata/cli/commands/
--rw-r--r--   0 simen     (1000) simen     (1000)        0 2020-12-09 11:27:37.000000 okdata-cli-1.6.0/okdata/cli/commands/__init__.py
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-03-21 09:48:41.516621 okdata-cli-1.6.0/okdata/cli/commands/datasets/
--rw-r--r--   0 simen     (1000) simen     (1000)       69 2023-03-21 06:17:16.000000 okdata-cli-1.6.0/okdata/cli/commands/datasets/__init__.py
--rw-r--r--   0 simen     (1000) simen     (1000)    14629 2023-03-21 06:17:16.000000 okdata-cli-1.6.0/okdata/cli/commands/datasets/datasets.py
--rw-r--r--   0 simen     (1000) simen     (1000)     5669 2023-03-21 06:17:16.000000 okdata-cli-1.6.0/okdata/cli/commands/datasets/questions.py
--rw-r--r--   0 simen     (1000) simen     (1000)     4461 2023-03-21 06:17:16.000000 okdata-cli-1.6.0/okdata/cli/commands/datasets/validators.py
--rw-r--r--   0 simen     (1000) simen     (1000)     3699 2023-03-21 06:17:16.000000 okdata-cli-1.6.0/okdata/cli/commands/datasets/wizards.py
--rw-r--r--   0 simen     (1000) simen     (1000)     4568 2022-04-27 09:26:47.000000 okdata-cli-1.6.0/okdata/cli/commands/permissions.py
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-03-21 09:48:41.516621 okdata-cli-1.6.0/okdata/cli/commands/pipelines/
--rw-r--r--   0 simen     (1000) simen     (1000)       58 2020-12-09 11:27:37.000000 okdata-cli-1.6.0/okdata/cli/commands/pipelines/__init__.py
--rw-r--r--   0 simen     (1000) simen     (1000)     1706 2022-04-27 09:26:47.000000 okdata-cli-1.6.0/okdata/cli/commands/pipelines/inputs.py
--rw-r--r--   0 simen     (1000) simen     (1000)     3193 2022-04-28 08:30:13.000000 okdata-cli-1.6.0/okdata/cli/commands/pipelines/instances.py
--rw-r--r--   0 simen     (1000) simen     (1000)     3109 2022-04-28 08:30:13.000000 okdata-cli-1.6.0/okdata/cli/commands/pipelines/pipelines.py
--rw-r--r--   0 simen     (1000) simen     (1000)     1724 2022-04-27 09:26:47.000000 okdata-cli-1.6.0/okdata/cli/commands/pipelines/schemas.py
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-03-21 09:48:41.516621 okdata-cli-1.6.0/okdata/cli/commands/pubreg/
--rw-r--r--   0 simen     (1000) simen     (1000)       89 2021-09-24 07:58:38.000000 okdata-cli-1.6.0/okdata/cli/commands/pubreg/__init__.py
--rw-r--r--   0 simen     (1000) simen     (1000)     2392 2023-03-21 06:10:29.000000 okdata-cli-1.6.0/okdata/cli/commands/pubreg/client.py
--rw-r--r--   0 simen     (1000) simen     (1000)    12114 2023-03-13 08:50:41.000000 okdata-cli-1.6.0/okdata/cli/commands/pubreg/pubreg.py
--rw-r--r--   0 simen     (1000) simen     (1000)     5459 2023-03-13 08:50:41.000000 okdata-cli-1.6.0/okdata/cli/commands/pubreg/questions.py
--rw-r--r--   0 simen     (1000) simen     (1000)     3121 2023-03-13 08:50:41.000000 okdata-cli-1.6.0/okdata/cli/commands/pubreg/wizards.py
--rw-r--r--   0 simen     (1000) simen     (1000)     3067 2022-04-27 09:26:47.000000 okdata-cli-1.6.0/okdata/cli/commands/status.py
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-03-21 09:48:41.516621 okdata-cli-1.6.0/okdata/cli/commands/teams/
--rw-r--r--   0 simen     (1000) simen     (1000)     2997 2023-02-17 13:22:37.000000 okdata-cli-1.6.0/okdata/cli/commands/teams/questions.py
--rw-r--r--   0 simen     (1000) simen     (1000)     7027 2022-12-09 07:24:37.000000 okdata-cli-1.6.0/okdata/cli/commands/teams/teams.py
--rw-r--r--   0 simen     (1000) simen     (1000)      456 2022-12-09 07:24:37.000000 okdata-cli-1.6.0/okdata/cli/commands/teams/util.py
--rw-r--r--   0 simen     (1000) simen     (1000)     1223 2022-12-09 07:24:37.000000 okdata-cli-1.6.0/okdata/cli/commands/teams/wizards.py
--rw-r--r--   0 simen     (1000) simen     (1000)      341 2023-02-17 13:22:37.000000 okdata-cli-1.6.0/okdata/cli/commands/wizard.py
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-03-21 09:48:41.516621 okdata-cli-1.6.0/okdata/cli/data/
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-03-21 09:48:41.520621 okdata-cli-1.6.0/okdata/cli/data/output-format/
--rw-r--r--   0 simen     (1000) simen     (1000)      180 2020-12-09 11:27:37.000000 okdata-cli-1.6.0/okdata/cli/data/output-format/datasets_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)      266 2020-12-09 11:27:37.000000 okdata-cli-1.6.0/okdata/cli/data/output-format/datasets_copy_file_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)      206 2020-12-09 11:27:37.000000 okdata-cli-1.6.0/okdata/cli/data/output-format/datasets_copy_file_config_2.json
--rw-r--r--   0 simen     (1000) simen     (1000)      359 2020-12-09 11:27:37.000000 okdata-cli-1.6.0/okdata/cli/data/output-format/datasets_dataset_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)      345 2020-12-09 11:27:37.000000 okdata-cli-1.6.0/okdata/cli/data/output-format/datasets_dataset_version_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)      328 2020-12-09 11:27:37.000000 okdata-cli-1.6.0/okdata/cli/data/output-format/datasets_dataset_version_edition_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)      119 2020-12-09 11:27:37.000000 okdata-cli-1.6.0/okdata/cli/data/output-format/datasets_dataset_version_edition_distributions_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)      209 2020-12-09 11:27:37.000000 okdata-cli-1.6.0/okdata/cli/data/output-format/datasets_dataset_versions_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)      146 2021-05-19 10:09:25.000000 okdata-cli-1.6.0/okdata/cli/data/output-format/my_permissions_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)      204 2021-05-19 10:09:25.000000 okdata-cli-1.6.0/okdata/cli/data/output-format/permissions_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)       55 2020-12-09 11:27:37.000000 okdata-cli-1.6.0/okdata/cli/data/output-format/pipelines_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)      203 2020-12-09 11:27:37.000000 okdata-cli-1.6.0/okdata/cli/data/output-format/pipelines_instances_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)      231 2020-12-09 11:27:37.000000 okdata-cli-1.6.0/okdata/cli/data/output-format/pipelines_instances_inputs_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)       52 2020-12-09 11:27:37.000000 okdata-cli-1.6.0/okdata/cli/data/output-format/pipelines_instances_schemas_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)      301 2022-08-25 09:15:43.000000 okdata-cli-1.6.0/okdata/cli/data/output-format/pubreg_audit_log_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)      246 2022-04-27 09:26:47.000000 okdata-cli-1.6.0/okdata/cli/data/output-format/pubreg_clients_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)      201 2023-03-13 08:50:41.000000 okdata-cli-1.6.0/okdata/cli/data/output-format/pubreg_multiple_client_keys_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)      125 2023-03-13 08:50:41.000000 okdata-cli-1.6.0/okdata/cli/data/output-format/pubreg_single_client_keys_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)      354 2021-07-06 12:28:25.000000 okdata-cli-1.6.0/okdata/cli/data/output-format/status_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)      721 2021-07-06 12:28:25.000000 okdata-cli-1.6.0/okdata/cli/data/output-format/status_history_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)      183 2022-08-25 13:30:17.000000 okdata-cli-1.6.0/okdata/cli/data/output-format/team_members_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)      124 2022-08-25 09:06:50.000000 okdata-cli-1.6.0/okdata/cli/data/output-format/teams_config.json
--rw-r--r--   0 simen     (1000) simen     (1000)      163 2020-12-09 11:27:37.000000 okdata-cli-1.6.0/okdata/cli/date.py
--rw-r--r--   0 simen     (1000) simen     (1000)      730 2020-12-09 11:27:37.000000 okdata-cli-1.6.0/okdata/cli/io.py
--rw-r--r--   0 simen     (1000) simen     (1000)     5538 2022-08-25 09:06:50.000000 okdata-cli-1.6.0/okdata/cli/output.py
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-03-21 09:48:41.520621 okdata-cli-1.6.0/okdata_cli.egg-info/
--rw-r--r--   0 simen     (1000) simen     (1000)     1077 2023-03-21 09:48:41.000000 okdata-cli-1.6.0/okdata_cli.egg-info/PKG-INFO
--rw-r--r--   0 simen     (1000) simen     (1000)     2673 2023-03-21 09:48:41.000000 okdata-cli-1.6.0/okdata_cli.egg-info/SOURCES.txt
--rw-r--r--   0 simen     (1000) simen     (1000)        1 2023-03-21 09:48:41.000000 okdata-cli-1.6.0/okdata_cli.egg-info/dependency_links.txt
--rw-r--r--   0 simen     (1000) simen     (1000)       52 2023-03-21 09:48:41.000000 okdata-cli-1.6.0/okdata_cli.egg-info/entry_points.txt
--rw-r--r--   0 simen     (1000) simen     (1000)        7 2023-03-21 09:48:41.000000 okdata-cli-1.6.0/okdata_cli.egg-info/namespace_packages.txt
--rw-r--r--   0 simen     (1000) simen     (1000)       80 2023-03-21 09:48:41.000000 okdata-cli-1.6.0/okdata_cli.egg-info/requires.txt
--rw-r--r--   0 simen     (1000) simen     (1000)       11 2023-03-21 09:48:41.000000 okdata-cli-1.6.0/okdata_cli.egg-info/top_level.txt
--rw-r--r--   0 simen     (1000) simen     (1000)      276 2020-04-30 07:54:22.000000 okdata-cli-1.6.0/pyproject.toml
--rw-r--r--   0 simen     (1000) simen     (1000)       38 2023-03-21 09:48:41.520621 okdata-cli-1.6.0/setup.cfg
--rw-r--r--   0 simen     (1000) simen     (1000)     1380 2023-03-21 09:47:26.000000 okdata-cli-1.6.0/setup.py
+drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-04-24 11:07:40.861759 okdata-cli-2.0.0/
+-rw-r--r--   0 simen     (1000) simen     (1000)     1077 2020-04-30 07:54:22.000000 okdata-cli-2.0.0/LICENSE
+-rw-r--r--   0 simen     (1000) simen     (1000)     1045 2023-04-24 11:07:40.861759 okdata-cli-2.0.0/PKG-INFO
+-rw-r--r--   0 simen     (1000) simen     (1000)      320 2023-04-21 08:20:57.000000 okdata-cli-2.0.0/README.md
+drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-04-24 11:07:40.857759 okdata-cli-2.0.0/okdata/
+-rw-r--r--   0 simen     (1000) simen     (1000)       56 2020-12-09 11:27:37.000000 okdata-cli-2.0.0/okdata/__init__.py
+drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-04-24 11:07:40.857759 okdata-cli-2.0.0/okdata/cli/
+-rw-r--r--   0 simen     (1000) simen     (1000)       27 2023-04-21 09:45:40.000000 okdata-cli-2.0.0/okdata/cli/__init__.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     2534 2023-04-21 10:35:45.000000 okdata-cli-2.0.0/okdata/cli/__main__.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     4400 2023-04-24 11:06:10.000000 okdata-cli-2.0.0/okdata/cli/command.py
+drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-04-24 11:07:40.857759 okdata-cli-2.0.0/okdata/cli/commands/
+-rw-r--r--   0 simen     (1000) simen     (1000)        0 2020-12-09 11:27:37.000000 okdata-cli-2.0.0/okdata/cli/commands/__init__.py
+drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-04-24 11:07:40.857759 okdata-cli-2.0.0/okdata/cli/commands/datasets/
+-rw-r--r--   0 simen     (1000) simen     (1000)       69 2023-03-21 06:17:16.000000 okdata-cli-2.0.0/okdata/cli/commands/datasets/__init__.py
+-rw-r--r--   0 simen     (1000) simen     (1000)    14604 2023-04-24 08:36:09.000000 okdata-cli-2.0.0/okdata/cli/commands/datasets/datasets.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     5669 2023-03-21 06:17:16.000000 okdata-cli-2.0.0/okdata/cli/commands/datasets/questions.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     4461 2023-03-21 06:17:16.000000 okdata-cli-2.0.0/okdata/cli/commands/datasets/validators.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     3699 2023-03-21 06:17:16.000000 okdata-cli-2.0.0/okdata/cli/commands/datasets/wizards.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     4568 2022-04-27 09:26:47.000000 okdata-cli-2.0.0/okdata/cli/commands/permissions.py
+drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-04-24 11:07:40.857759 okdata-cli-2.0.0/okdata/cli/commands/pubreg/
+-rw-r--r--   0 simen     (1000) simen     (1000)       89 2021-09-24 07:58:38.000000 okdata-cli-2.0.0/okdata/cli/commands/pubreg/__init__.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     2392 2023-03-21 06:10:29.000000 okdata-cli-2.0.0/okdata/cli/commands/pubreg/client.py
+-rw-r--r--   0 simen     (1000) simen     (1000)    11255 2023-04-24 08:36:09.000000 okdata-cli-2.0.0/okdata/cli/commands/pubreg/pubreg.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     5459 2023-03-13 08:50:41.000000 okdata-cli-2.0.0/okdata/cli/commands/pubreg/questions.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     3121 2023-03-13 08:50:41.000000 okdata-cli-2.0.0/okdata/cli/commands/pubreg/wizards.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     3067 2022-04-27 09:26:47.000000 okdata-cli-2.0.0/okdata/cli/commands/status.py
+drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-04-24 11:07:40.857759 okdata-cli-2.0.0/okdata/cli/commands/teams/
+-rw-r--r--   0 simen     (1000) simen     (1000)     2997 2023-02-17 13:22:37.000000 okdata-cli-2.0.0/okdata/cli/commands/teams/questions.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     5633 2023-04-24 08:36:09.000000 okdata-cli-2.0.0/okdata/cli/commands/teams/teams.py
+-rw-r--r--   0 simen     (1000) simen     (1000)      456 2022-12-09 07:24:37.000000 okdata-cli-2.0.0/okdata/cli/commands/teams/util.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     1223 2022-12-09 07:24:37.000000 okdata-cli-2.0.0/okdata/cli/commands/teams/wizards.py
+-rw-r--r--   0 simen     (1000) simen     (1000)      341 2023-02-17 13:22:37.000000 okdata-cli-2.0.0/okdata/cli/commands/wizard.py
+drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-04-24 11:07:40.857759 okdata-cli-2.0.0/okdata/cli/data/
+drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-04-24 11:07:40.861759 okdata-cli-2.0.0/okdata/cli/data/output-format/
+-rw-r--r--   0 simen     (1000) simen     (1000)      180 2020-12-09 11:27:37.000000 okdata-cli-2.0.0/okdata/cli/data/output-format/datasets_config.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      266 2020-12-09 11:27:37.000000 okdata-cli-2.0.0/okdata/cli/data/output-format/datasets_copy_file_config.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      206 2020-12-09 11:27:37.000000 okdata-cli-2.0.0/okdata/cli/data/output-format/datasets_copy_file_config_2.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      359 2020-12-09 11:27:37.000000 okdata-cli-2.0.0/okdata/cli/data/output-format/datasets_dataset_config.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      345 2020-12-09 11:27:37.000000 okdata-cli-2.0.0/okdata/cli/data/output-format/datasets_dataset_version_config.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      328 2020-12-09 11:27:37.000000 okdata-cli-2.0.0/okdata/cli/data/output-format/datasets_dataset_version_edition_config.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      119 2020-12-09 11:27:37.000000 okdata-cli-2.0.0/okdata/cli/data/output-format/datasets_dataset_version_edition_distributions_config.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      209 2020-12-09 11:27:37.000000 okdata-cli-2.0.0/okdata/cli/data/output-format/datasets_dataset_versions_config.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      146 2021-05-19 10:09:25.000000 okdata-cli-2.0.0/okdata/cli/data/output-format/my_permissions_config.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      204 2021-05-19 10:09:25.000000 okdata-cli-2.0.0/okdata/cli/data/output-format/permissions_config.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      301 2022-08-25 09:15:43.000000 okdata-cli-2.0.0/okdata/cli/data/output-format/pubreg_audit_log_config.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      246 2022-04-27 09:26:47.000000 okdata-cli-2.0.0/okdata/cli/data/output-format/pubreg_clients_config.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      201 2023-03-13 08:50:41.000000 okdata-cli-2.0.0/okdata/cli/data/output-format/pubreg_multiple_client_keys_config.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      125 2023-03-13 08:50:41.000000 okdata-cli-2.0.0/okdata/cli/data/output-format/pubreg_single_client_keys_config.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      354 2021-07-06 12:28:25.000000 okdata-cli-2.0.0/okdata/cli/data/output-format/status_config.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      721 2021-07-06 12:28:25.000000 okdata-cli-2.0.0/okdata/cli/data/output-format/status_history_config.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      183 2022-08-25 13:30:17.000000 okdata-cli-2.0.0/okdata/cli/data/output-format/team_members_config.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      124 2022-08-25 09:06:50.000000 okdata-cli-2.0.0/okdata/cli/data/output-format/teams_config.json
+-rw-r--r--   0 simen     (1000) simen     (1000)      163 2020-12-09 11:27:37.000000 okdata-cli-2.0.0/okdata/cli/date.py
+-rw-r--r--   0 simen     (1000) simen     (1000)      730 2020-12-09 11:27:37.000000 okdata-cli-2.0.0/okdata/cli/io.py
+-rw-r--r--   0 simen     (1000) simen     (1000)     4802 2023-04-21 08:20:57.000000 okdata-cli-2.0.0/okdata/cli/output.py
+drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2023-04-24 11:07:40.861759 okdata-cli-2.0.0/okdata_cli.egg-info/
+-rw-r--r--   0 simen     (1000) simen     (1000)     1045 2023-04-24 11:07:40.000000 okdata-cli-2.0.0/okdata_cli.egg-info/PKG-INFO
+-rw-r--r--   0 simen     (1000) simen     (1000)     2211 2023-04-24 11:07:40.000000 okdata-cli-2.0.0/okdata_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 simen     (1000) simen     (1000)        1 2023-04-24 11:07:40.000000 okdata-cli-2.0.0/okdata_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 simen     (1000) simen     (1000)       52 2023-04-24 11:07:40.000000 okdata-cli-2.0.0/okdata_cli.egg-info/entry_points.txt
+-rw-r--r--   0 simen     (1000) simen     (1000)        7 2023-04-24 11:07:40.000000 okdata-cli-2.0.0/okdata_cli.egg-info/namespace_packages.txt
+-rw-r--r--   0 simen     (1000) simen     (1000)       80 2023-04-24 11:07:40.000000 okdata-cli-2.0.0/okdata_cli.egg-info/requires.txt
+-rw-r--r--   0 simen     (1000) simen     (1000)       11 2023-04-24 11:07:40.000000 okdata-cli-2.0.0/okdata_cli.egg-info/top_level.txt
+-rw-r--r--   0 simen     (1000) simen     (1000)      276 2020-04-30 07:54:22.000000 okdata-cli-2.0.0/pyproject.toml
+-rw-r--r--   0 simen     (1000) simen     (1000)       38 2023-04-24 11:07:40.861759 okdata-cli-2.0.0/setup.cfg
+-rw-r--r--   0 simen     (1000) simen     (1000)     1380 2023-04-24 11:06:10.000000 okdata-cli-2.0.0/setup.py
```

### Comparing `okdata-cli-1.6.0/LICENSE` & `okdata-cli-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `okdata-cli-1.6.0/PKG-INFO` & `okdata-cli-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okdata-cli
-Version: 1.6.0
+Version: 2.0.0
 Summary: CLI for services provided by Oslo Origo
 Home-page: https://github.com/oslokommune/okdata-cli/
 Author: Oslo Origo
 Author-email: dataplattform@oslo.kommune.no
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
@@ -20,12 +20,11 @@
 
 # `okdata-cli`: Oslo Origo data services CLI
 
 Okdata CLI provides a unified interface to data services for Oslo Origo teams.
 
 * [Install](doc/install.md)
 * [Configuration](doc/configuration.md)
-* [Datasets](doc/datasets.md)
-* [Permissions](doc/permissions.md)
-* [Pipelines](doc/pipelines.md)
 * [Public registers](doc/pubreg.md)
 * [Teams](doc/teams.md)
+* [Datasets](doc/datasets.md)
+* [Permissions](doc/permissions.md)
```

### Comparing `okdata-cli-1.6.0/okdata/cli/__main__.py` & `okdata-cli-2.0.0/okdata/cli/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import json
 import sys
 
 from keycloak.exceptions import KeycloakGetError
 from okdata.sdk.exceptions import ApiAuthenticateError
 from requests.exceptions import RequestException
 
+from okdata.cli import MAINTAINER
 from okdata.cli.command import BaseCommand
 from okdata.cli.commands.datasets import DatasetsCommand
 from okdata.cli.commands.permissions import PermissionsCommand
-from okdata.cli.commands.pipelines import Pipelines
 from okdata.cli.commands.pubreg import PubregCommand
 from okdata.cli.commands.status import StatusCommand
 from okdata.cli.commands.teams.teams import TeamsCommand
 
 
 def main():
     argv = sys.argv
@@ -29,15 +29,15 @@
             instance.handle()
         except RequestException as e:
             if hasattr(e.response, "json"):
                 instance.print_error_response(e.response.json())
             else:
                 instance.print(
                     "A server error occurred. Please try again, or contact "
-                    "Datapatruljen if the problem persists.",
+                    f"{MAINTAINER} if the problem persists.",
                 )
         except ApiAuthenticateError:
             instance.print(
                 "An error occurred (ApiAuthenticateError): Invalid credentials",
                 {"error": 1, "message": "Invalid credentials"},
             )
         except KeycloakGetError as e:
@@ -65,15 +65,14 @@
         BaseCommand().help()
 
 
 def get_command_class(argv):
     commands = {
         "datasets": DatasetsCommand,
         "permissions": PermissionsCommand,
-        "pipelines": Pipelines,
         "pubreg": PubregCommand,
         "status": StatusCommand,
         "teams": TeamsCommand,
     }
     return commands.get(argv[1], False)
```

### Comparing `okdata-cli-1.6.0/okdata/cli/command.py` & `okdata-cli-2.0.0/okdata/cli/command.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,35 +9,33 @@
   -h, --help                # Print this help
   -d, --debug               # Output debug information while executing task
   --format=<value>          # Output format: table OR json
   --env=<value>             # Environment to run command in: prod OR dev"""
 
 
 class BaseCommand:
-    version = "1.6.0"
+    version = "2.0.0"
     # TODO: Can use `importlib` in Python 3.8 and up instead of hard coding the
     #       version here:
     #
     # version = importlib.metadata.version("okdata-cli")
 
     __doc__ = f"""okdata-cli {version}
 
 usage:
   okdata datasets [options]
   okdata permissions [options]
-  okdata pipelines [options]
   okdata pubreg [options]
   okdata status [options]
   okdata teams [options]
   okdata -h | --help
 
 Commands available:
   datasets
   permissions
-  pipelines
   pubreg
   status
   teams
 
 Options:{BASE_COMMAND_OPTIONS}
 """
     log = logging.getLogger(__name__)
@@ -121,33 +119,43 @@
         if self.opt("format") == "json":
             print(f"{str}")
 
     def help(self):
         print(self.__doc__, end="")
 
     def print_error_response(self, response_body):
-        if type(response_body) != dict:
+        if not isinstance(response_body, dict):
             print(response_body)
             return
 
         response_body.update({"error": 1})
 
         if self.opt("format") == "json":
             print(json.dumps(response_body))
         else:
             try:
-                feedback = generate_error_feedback(
-                    message=response_body["message"],
-                    errors=response_body.get("errors", None),
+                print(
+                    _format_error_message(
+                        response_body["message"], response_body.get("errors")
+                    )
                 )
-                print(feedback)
             except KeyError:
                 self.log.debug("Got unexpected response body from api.")
                 print(response_body)
 
 
-def generate_error_feedback(message, errors=None):
-    feedback = f"An error occurred: {message}"
-    if errors:
-        feedback += f"\nCause:\n\t{errors}"
+def _format_error_message(message, errors=None):
+    msg = f"An error occurred: {message}"
+    sep = "\n - "
+
+    if isinstance(errors, list):
+        msg += "\nCause{}:{}{}".format(
+            "s" if len(errors) > 1 else "",
+            sep,
+            sep.join(
+                err.get("msg", "") if isinstance(err, dict) else err for err in errors
+            ),
+        )
+    elif errors:
+        msg += f"\nCause:{sep}{errors}"
 
-    return f"{feedback}"
+    return msg
```

### Comparing `okdata-cli-1.6.0/okdata/cli/commands/datasets/datasets.py` & `okdata-cli-2.0.0/okdata/cli/commands/datasets/datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,16 +242,15 @@
     def get_latest_or_create_edition(self, dataset_id, version):
         self.log.info(f"Resolving edition for dataset-uri: {dataset_id}/{version}")
         try:
             return self.sdk.get_latest_edition(dataset_id, version)["Id"].split("/")[-1]
         except HTTPError as he:
             if he.response.status_code == 404:
                 return self._auto_create_edition(dataset_id, version)
-            else:
-                raise he
+            raise
 
     # #################################### #
     # Distribution
     # #################################### #
     def create_distribution(self):
         payload = read_json(self.opt("file"))
         dataset_id = self.arg("datasetid")
```

### Comparing `okdata-cli-1.6.0/okdata/cli/commands/datasets/questions.py` & `okdata-cli-2.0.0/okdata/cli/commands/datasets/questions.py`

 * *Files identical despite different names*

### Comparing `okdata-cli-1.6.0/okdata/cli/commands/datasets/validators.py` & `okdata-cli-2.0.0/okdata/cli/commands/datasets/validators.py`

 * *Files identical despite different names*

### Comparing `okdata-cli-1.6.0/okdata/cli/commands/datasets/wizards.py` & `okdata-cli-2.0.0/okdata/cli/commands/datasets/wizards.py`

 * *Files identical despite different names*

### Comparing `okdata-cli-1.6.0/okdata/cli/commands/permissions.py` & `okdata-cli-2.0.0/okdata/cli/commands/permissions.py`

 * *Files identical despite different names*

### Comparing `okdata-cli-1.6.0/okdata/cli/commands/pubreg/client.py` & `okdata-cli-2.0.0/okdata/cli/commands/pubreg/client.py`

 * *Files identical despite different names*

### Comparing `okdata-cli-1.6.0/okdata/cli/commands/pubreg/pubreg.py` & `okdata-cli-2.0.0/okdata/cli/commands/pubreg/pubreg.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import base64
 from datetime import datetime
 from operator import itemgetter
 
 from okdata.sdk.team.client import TeamClient
-from requests.exceptions import HTTPError
 
+from okdata.cli import MAINTAINER
 from okdata.cli.command import BASE_COMMAND_OPTIONS, BaseCommand
 from okdata.cli.commands.pubreg.client import PubregClient
 from okdata.cli.commands.pubreg.questions import NoClientsError, NoKeysError
 from okdata.cli.commands.pubreg.wizards import (
     audit_log_wizard,
     create_client_wizard,
     create_key_wizard,
@@ -68,15 +68,15 @@
 
     def create_client(self):
         try:
             config = create_client_wizard(self.team_client)
         except NoTeamError:
             self.print(
                 "We haven't yet registered you as member of any Origo team. "
-                "Please contact Datapatruljen to get it done."
+                f"Please contact {MAINTAINER} to get it done."
             )
             return
 
         team_id = config["team_id"]
         provider_id = config["provider_id"]
         provider_name = config["provider_name"]
         integration = config["integration"]
@@ -84,30 +84,26 @@
         env = config["env"]
 
         self.confirm_to_continue(
             f"Will create a new client for {provider_name} in {env} with "
             f"scopes {scopes}."
         )
 
-        try:
-            self.print("Creating client...")
-            response = self.pubreg_client.create_client(
-                team_id, provider_id, integration, scopes, env
-            )
-            client_name = response["client_name"]
-            self.print(
-                f"""
+        self.print("Creating client...")
+        response = self.pubreg_client.create_client(
+            team_id, provider_id, integration, scopes, env
+        )
+        client_name = response["client_name"]
+        self.print(
+            f"""
 Done! Created a new client '{client_name}'.
 You may now go ahead and create a key for it by running:
 
   okdata pubreg create-key"""
-            )
-        except HTTPError as e:
-            message = e.response.json()["message"]
-            self.print(f"Something went wrong: {message}")
+        )
 
     def list_clients(self):
         config = list_clients_wizard()
         env = config["env"]
         clients = self.pubreg_client.get_clients(env)
         out = create_output(self.opt("format"), "pubreg_clients_config.json")
         out.add_rows(sorted(clients, key=itemgetter("client_name")))
@@ -131,42 +127,36 @@
                     f"({aws_region})"
                 )
                 if delete_from_aws
                 else "",
             ),
         )
 
-        try:
-            self.print(f"Deleting client '{client_name}' [{env}]...")
-            res = self.pubreg_client.delete_client(
-                env, client_id, aws_account, aws_region
-            )
-            deleted_ssm_params = res["deleted_ssm_params"]
-            self.print("\nDone! The client is deleted and will no longer work.")
+        self.print(f"Deleting client '{client_name}' [{env}]...")
+        res = self.pubreg_client.delete_client(env, client_id, aws_account, aws_region)
+        deleted_ssm_params = res["deleted_ssm_params"]
 
-            if delete_from_aws:
-                if deleted_ssm_params:
-                    self.print(
-                        "\nThe following {} deleted from SSM:".format(
-                            "parameter was"
-                            if len(deleted_ssm_params) == 1
-                            else "parameters were"
-                        )
-                    )
-                    for param in deleted_ssm_params:
-                        self.print(f"- {param}")
-                else:
-                    self.print(
-                        "However the key secrets couldn't be deleted from SSM "
-                        "as requested."
-                    )
+        self.print("\nDone! The client is deleted and will no longer work.")
 
-        except HTTPError as e:
-            message = e.response.json()["message"]
-            self.print(f"Something went wrong: {message}")
+        if delete_from_aws:
+            if deleted_ssm_params:
+                self.print(
+                    "\nThe following {} deleted from SSM:".format(
+                        "parameter was"
+                        if len(deleted_ssm_params) == 1
+                        else "parameters were"
+                    )
+                )
+                for param in deleted_ssm_params:
+                    self.print(f"- {param}")
+            else:
+                self.print(
+                    "However the key secrets couldn't be deleted from SSM as "
+                    "requested."
+                )
 
     def _handle_new_key_aws(self, key, enabled_auto_rotate):
         params = key.get("ssm_params")
 
         if params:
             self.print(
                 (
@@ -182,15 +172,15 @@
                 self.print(
                     "\nThe key has been scheduled for automatic rotation.",
                 )
         else:
             self.print(
                 "The key was created, but it appears that the relevant "
                 "parameters weren't added to SSM. This should not happen, "
-                "please contact Datapatruljen!"
+                f"please contact {MAINTAINER}!"
             )
 
     def _handle_new_key_local(self, key, client_name, env):
         outfile = f"{client_name}-{env}-{key['kid']}.p12"
 
         with open(outfile, "wb") as f:
             f.write(base64.b64decode(key["keystore"]))
@@ -247,32 +237,26 @@
                     else "The key will NOT be rotated automatically.\n",
                 ]
             )
         )
 
         self.print("Creating key for '{}' [{}]...".format(client_name, env))
 
-        try:
-            key = self.pubreg_client.create_key(
-                env, client_id, aws_account, aws_region, enable_auto_rotate
-            )
-        except HTTPError as e:
-            message = e.response.json()["message"]
-            self.print(f"Something went wrong: {message}")
-            return
+        key = self.pubreg_client.create_key(
+            env, client_id, aws_account, aws_region, enable_auto_rotate
+        )
 
         if key.get("ssm_params") is not None:
             self._handle_new_key_aws(key, enable_auto_rotate)
         elif key.get("keystore") and key.get("key_password"):
             self._handle_new_key_local(key, client_name, env)
         else:
             self.print(
                 "The key was neither added to AWS nor returned to the "
-                "client. This should not happen, please contact "
-                "Datapatruljen!"
+                f"client. This should not happen, please contact {MAINTAINER}!"
             )
 
     def _list_client_keys_single(self, client_id, client_name, env):
         keys = self.pubreg_client.get_keys(env, client_id)
         out = create_output(
             self.opt("format"),
             "pubreg_single_client_keys_config.json",
@@ -317,23 +301,17 @@
         client_name = choices["client_name"]
         key_id = choices["key_id"]
 
         self.confirm_to_continue(
             f"Will delete key '{key_id}' from '{client_name}' [{env}]."
         )
 
-        try:
-            self.print(
-                f"Deleting key '{key_id}' from '{client_name}' [{env}]...",
-            )
-            self.pubreg_client.delete_key(env, client_id, key_id)
-            self.print("Done! The key is deleted and will no longer work.")
-        except HTTPError as e:
-            message = e.response.json()["message"]
-            self.print(f"Something went wrong: {message}")
+        self.print(f"Deleting key '{key_id}' from '{client_name}' [{env}]...")
+        self.pubreg_client.delete_key(env, client_id, key_id)
+        self.print("Done! The key is deleted and will no longer work.")
 
     def audit_log(self):
         choices = audit_log_wizard(self.pubreg_client)
         env = choices["env"]
         client_id = choices["client_id"]
         client_name = choices["client_name"]
```

### Comparing `okdata-cli-1.6.0/okdata/cli/commands/pubreg/questions.py` & `okdata-cli-2.0.0/okdata/cli/commands/pubreg/questions.py`

 * *Files identical despite different names*

### Comparing `okdata-cli-1.6.0/okdata/cli/commands/pubreg/wizards.py` & `okdata-cli-2.0.0/okdata/cli/commands/pubreg/wizards.py`

 * *Files identical despite different names*

### Comparing `okdata-cli-1.6.0/okdata/cli/commands/status.py` & `okdata-cli-2.0.0/okdata/cli/commands/status.py`

 * *Files identical despite different names*

### Comparing `okdata-cli-1.6.0/okdata/cli/commands/teams/questions.py` & `okdata-cli-2.0.0/okdata/cli/commands/teams/questions.py`

 * *Files identical despite different names*

### Comparing `okdata-cli-1.6.0/okdata/cli/commands/teams/teams.py` & `okdata-cli-2.0.0/okdata/cli/commands/teams/teams.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from operator import itemgetter
 
 from okdata.sdk.team.client import TeamClient
-from requests.exceptions import HTTPError
 
+from okdata.cli import MAINTAINER
 from okdata.cli.command import BASE_COMMAND_OPTIONS, BaseCommand
 from okdata.cli.commands.teams.questions import NoTeamError
 from okdata.cli.commands.teams.util import (
     member_representation,
     sorted_member_list,
 )
 from okdata.cli.commands.teams.wizards import (
@@ -52,159 +52,123 @@
             self.list_members(self.opt("my"))
         if self.cmd("add-member"):
             self.add_member()
         if self.cmd("remove-member"):
             self.remove_member()
 
     def ls(self, my):
-        try:
-            teams = self.client.get_teams(
-                include=None if my else "all", has_role="origo-team"
-            )
-        except HTTPError as e:
-            message = e.response.json()["message"]
-            self.print(f"Something went wrong: {message}")
-            return
-
+        teams = self.client.get_teams(
+            include=None if my else "all", has_role="origo-team"
+        )
         out = create_output(self.opt("format"), "teams_config.json")
         out.add_rows(sorted(teams, key=itemgetter("name")))
         self.print("{} teams:".format("My" if my else "All"), out)
 
     def edit(self):
         try:
             config = edit_team_wizard(self.client)
         except NoTeamError:
             self.print(
                 "We haven't yet registered you as member of any Origo team. "
-                "Please contact Datapatruljen to get it done."
+                f"Please contact {MAINTAINER} to get it done."
             )
             return
 
-        try:
-            if config["attribute"] == "name":
-                self.client.update_team_name(
-                    config["team_id"],
-                    config["team_name"],
-                )
-            else:
-                self.client.update_team_attribute(
-                    config["team_id"],
-                    config["attribute"],
-                    config["attribute_value"],
-                )
-            self.print("Done!")
-        except HTTPError as e:
-            data = e.response.json()
-
-            if e.response.status_code == 400:
-                errors = data.get("errors", [])
-                message = "\n".join(err.get("msg", "") for err in errors).strip()
-            else:
-                message = data["message"]
-
-            self.print(f"Something went wrong: {message}")
+        if config["attribute"] == "name":
+            self.client.update_team_name(config["team_id"], config["team_name"])
+        else:
+            self.client.update_team_attribute(
+                config["team_id"], config["attribute"], config["attribute_value"]
+            )
+        self.print("Done!")
 
     def list_members(self, my):
         try:
             config = list_members_wizard(self.client, my)
             members = self.client.get_team_members(config["team_id"])
         except NoTeamError:
             self.print(
                 "We haven't yet registered you as member of any Origo team. "
-                "Please contact Datapatruljen to get it done."
+                f"Please contact {MAINTAINER} to get it done."
                 if my
                 else "No teams exist yet."
             )
             return
-        except HTTPError as e:
-            message = e.response.json()["message"]
-            self.print(f"Something went wrong: {message}")
-            return
 
         out = create_output(self.opt("format"), "team_members_config.json")
 
         out.add_rows(sorted_member_list(members))
         self.print("Team members", out)
 
     def add_member(self):
         try:
             config = add_member_wizard(self.client)
         except NoTeamError:
             self.print(
                 "We haven't yet registered you as member of any Origo team. "
-                "Please contact Datapatruljen to get it done."
+                f"Please contact {MAINTAINER} to get it done."
             )
             return
 
-        try:
-            user = self.client.get_user_by_username(config["username"])
-            team_members = [
-                m["username"] for m in self.client.get_team_members(config["team_id"])
-            ]
-
-            if user["username"] in team_members:
-                self.print(
-                    "User {} is already a member of this team.".format(
-                        member_representation(user)
-                    )
-                )
-                return
+        user = self.client.get_user_by_username(config["username"])
+        team_members = [
+            m["username"] for m in self.client.get_team_members(config["team_id"])
+        ]
 
-            self.confirm_to_continue(
-                "Add {} to the team?".format(member_representation(user))
-            )
-
-            self.client.update_team_members(
-                config["team_id"], team_members + [user["username"]]
+        if user["username"] in team_members:
+            self.print(
+                "User {} is already a member of this team.".format(
+                    member_representation(user)
+                )
             )
-            self.print("Done!")
-        except HTTPError as e:
-            message = e.response.json()["message"]
-            self.print(f"Something went wrong: {message}")
             return
 
+        self.confirm_to_continue(
+            "Add {} to the team?".format(member_representation(user))
+        )
+
+        self.client.update_team_members(
+            config["team_id"], team_members + [user["username"]]
+        )
+        self.print("Done!")
+
     def remove_member(self):
         try:
             config = remove_member_wizard(self.client)
         except NoTeamError:
             self.print(
                 "We haven't yet registered you as member of any Origo team. "
-                "Please contact Datapatruljen to get it done."
+                f"Please contact {MAINTAINER} to get it done."
             )
             return
 
-        try:
-            team_members = self.client.get_team_members(config["team_id"])
-            members_to_remove, members_to_keep = [], []
-            for member in team_members:
-                if member["username"] in config["usernames"]:
-                    members_to_remove.append(member)
-                else:
-                    members_to_keep.append(member)
-
-            if len(members_to_keep) == 0:
-                self.confirm_to_continue(
-                    "You are about to delete all members from the team, including "
-                    "yourself. It will not be possible to edit this team any further "
-                    "without being re-added by a systems administrator."
-                )
+        team_members = self.client.get_team_members(config["team_id"])
+        members_to_remove, members_to_keep = [], []
+        for member in team_members:
+            if member["username"] in config["usernames"]:
+                members_to_remove.append(member)
             else:
-                self.confirm_to_continue(
-                    "Remove the following member{} from the team?\n - {}".format(
-                        "s" if len(members_to_remove) > 1 else "",
-                        "\n - ".join(
-                            [
-                                member_representation(m)
-                                for m in sorted_member_list(members_to_remove)
-                            ]
-                        ),
-                    )
-                )
+                members_to_keep.append(member)
 
-            self.client.update_team_members(
-                config["team_id"], [m["username"] for m in members_to_keep]
+        if len(members_to_keep) == 0:
+            self.confirm_to_continue(
+                "You are about to delete all members from the team, including "
+                "yourself. It will not be possible to edit this team any "
+                "further without being re-added by a systems administrator."
             )
-            self.print("Done!")
-        except HTTPError as e:
-            message = e.response.json()["message"]
-            self.print(f"Something went wrong: {message}")
-            return
+        else:
+            self.confirm_to_continue(
+                "Remove the following member{} from the team?\n - {}".format(
+                    "s" if len(members_to_remove) > 1 else "",
+                    "\n - ".join(
+                        [
+                            member_representation(m)
+                            for m in sorted_member_list(members_to_remove)
+                        ]
+                    ),
+                )
+            )
+
+        self.client.update_team_members(
+            config["team_id"], [m["username"] for m in members_to_keep]
+        )
+        self.print("Done!")
```

### Comparing `okdata-cli-1.6.0/okdata/cli/commands/teams/wizards.py` & `okdata-cli-2.0.0/okdata/cli/commands/teams/wizards.py`

 * *Files identical despite different names*

### Comparing `okdata-cli-1.6.0/okdata/cli/data/output-format/status_history_config.json` & `okdata-cli-2.0.0/okdata/cli/data/output-format/status_history_config.json`

 * *Files identical despite different names*

### Comparing `okdata-cli-1.6.0/okdata/cli/io.py` & `okdata-cli-2.0.0/okdata/cli/io.py`

 * *Files identical despite different names*

### Comparing `okdata-cli-1.6.0/okdata/cli/output.py` & `okdata-cli-2.0.0/okdata/cli/output.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import inspect
 import json
 import logging
 import os
 from datetime import datetime
 from textwrap import wrap, fill
 
 from prettytable import PrettyTable
@@ -27,38 +26,14 @@
         config = json.load(config_file)
 
     if format == "json":
         return JsonOutput(config)
     return TableOutput(config)
 
 
-def table_config_from_schema(resource, exclude=None):
-    if exclude is None:
-        exclude = []
-
-    def _for(properties):
-        for property in properties:
-            body = properties[property]
-            if "properties" not in body:
-                yield body["title"], {"name": body["title"], "key": property}
-            else:
-                _for(body["properties"])
-
-    with open(
-        os.path.dirname(inspect.getfile(resource))
-        + f"/schemas/{resource.__resource_name__}.json",
-        "r",
-    ) as f:
-        schema = json.loads(f.read())
-        config = {
-            key: body for key, body in _for(schema["properties"]) if key not in exclude
-        }
-        return TableOutput(config)
-
-
 class TableOutput(PrettyTable):
     def __init__(self, config):
         self.config = config
         self.output_singular_object = False
         column_headers = []
         for key in self.config:
             name = self.config[key]["name"]
```

### Comparing `okdata-cli-1.6.0/okdata_cli.egg-info/PKG-INFO` & `okdata-cli-2.0.0/okdata_cli.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okdata-cli
-Version: 1.6.0
+Version: 2.0.0
 Summary: CLI for services provided by Oslo Origo
 Home-page: https://github.com/oslokommune/okdata-cli/
 Author: Oslo Origo
 Author-email: dataplattform@oslo.kommune.no
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
@@ -20,12 +20,11 @@
 
 # `okdata-cli`: Oslo Origo data services CLI
 
 Okdata CLI provides a unified interface to data services for Oslo Origo teams.
 
 * [Install](doc/install.md)
 * [Configuration](doc/configuration.md)
-* [Datasets](doc/datasets.md)
-* [Permissions](doc/permissions.md)
-* [Pipelines](doc/pipelines.md)
 * [Public registers](doc/pubreg.md)
 * [Teams](doc/teams.md)
+* [Datasets](doc/datasets.md)
+* [Permissions](doc/permissions.md)
```

### Comparing `okdata-cli-1.6.0/okdata_cli.egg-info/SOURCES.txt` & `okdata-cli-2.0.0/okdata_cli.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -14,19 +14,14 @@
 okdata/cli/commands/status.py
 okdata/cli/commands/wizard.py
 okdata/cli/commands/datasets/__init__.py
 okdata/cli/commands/datasets/datasets.py
 okdata/cli/commands/datasets/questions.py
 okdata/cli/commands/datasets/validators.py
 okdata/cli/commands/datasets/wizards.py
-okdata/cli/commands/pipelines/__init__.py
-okdata/cli/commands/pipelines/inputs.py
-okdata/cli/commands/pipelines/instances.py
-okdata/cli/commands/pipelines/pipelines.py
-okdata/cli/commands/pipelines/schemas.py
 okdata/cli/commands/pubreg/__init__.py
 okdata/cli/commands/pubreg/client.py
 okdata/cli/commands/pubreg/pubreg.py
 okdata/cli/commands/pubreg/questions.py
 okdata/cli/commands/pubreg/wizards.py
 okdata/cli/commands/teams/questions.py
 okdata/cli/commands/teams/teams.py
@@ -38,18 +33,14 @@
 okdata/cli/data/output-format/datasets_dataset_config.json
 okdata/cli/data/output-format/datasets_dataset_version_config.json
 okdata/cli/data/output-format/datasets_dataset_version_edition_config.json
 okdata/cli/data/output-format/datasets_dataset_version_edition_distributions_config.json
 okdata/cli/data/output-format/datasets_dataset_versions_config.json
 okdata/cli/data/output-format/my_permissions_config.json
 okdata/cli/data/output-format/permissions_config.json
-okdata/cli/data/output-format/pipelines_config.json
-okdata/cli/data/output-format/pipelines_instances_config.json
-okdata/cli/data/output-format/pipelines_instances_inputs_config.json
-okdata/cli/data/output-format/pipelines_instances_schemas_config.json
 okdata/cli/data/output-format/pubreg_audit_log_config.json
 okdata/cli/data/output-format/pubreg_clients_config.json
 okdata/cli/data/output-format/pubreg_multiple_client_keys_config.json
 okdata/cli/data/output-format/pubreg_single_client_keys_config.json
 okdata/cli/data/output-format/status_config.json
 okdata/cli/data/output-format/status_history_config.json
 okdata/cli/data/output-format/team_members_config.json
```

### Comparing `okdata-cli-1.6.0/setup.py` & `okdata-cli-2.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="okdata-cli",
-    version="1.6.0",
+    version="2.0.0",
     author="Oslo Origo",
     author_email="dataplattform@oslo.kommune.no",
     description="CLI for services provided by Oslo Origo",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/oslokommune/okdata-cli/",
```


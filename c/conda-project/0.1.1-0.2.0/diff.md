# Comparing `tmp/conda-project-0.1.1.tar.gz` & `tmp/conda-project-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conda-project-0.1.1.tar", last modified: Thu Apr  6 01:04:09 2023, max compression
+gzip compressed data, was "conda-project-0.2.0.tar", last modified: Mon Apr 24 21:41:53 2023, max compression
```

## Comparing `conda-project-0.1.1.tar` & `conda-project-0.2.0.tar`

### file list

```diff
@@ -1,85 +1,95 @@
-drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-06 01:04:09.032415 conda-project-0.1.1/
--rw-r--r--   0 adefusco   (502) staff       (20)      136 2023-04-05 14:24:50.000000 conda-project-0.1.1/.flake8
--rw-r--r--   0 adefusco   (502) staff       (20)       58 2022-04-01 15:52:07.000000 conda-project-0.1.1/.gitattributes
-drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-06 01:04:09.016528 conda-project-0.1.1/.github/
--rw-r--r--   0 adefusco   (502) staff       (20)       71 2022-04-14 22:10:46.000000 conda-project-0.1.1/.github/disclaimer.txt
-drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-06 01:04:09.017362 conda-project-0.1.1/.github/workflows/
--rw-r--r--   0 adefusco   (502) staff       (20)     1163 2022-12-06 15:55:00.000000 conda-project-0.1.1/.github/workflows/docs.yml
--rw-r--r--   0 adefusco   (502) staff       (20)     5597 2023-04-06 01:03:58.000000 conda-project-0.1.1/.github/workflows/main.yaml
--rw-r--r--   0 adefusco   (502) staff       (20)     1913 2023-04-06 01:03:58.000000 conda-project-0.1.1/.gitignore
--rw-r--r--   0 adefusco   (502) staff       (20)      999 2023-04-05 20:34:59.000000 conda-project-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 adefusco   (502) staff       (20)      340 2023-04-01 01:55:09.000000 conda-project-0.1.1/CHANGELOG.md
--rw-r--r--   0 adefusco   (502) staff       (20)     1544 2022-04-01 15:50:48.000000 conda-project-0.1.1/LICENSE
--rw-r--r--   0 adefusco   (502) staff       (20)     5543 2023-04-06 01:04:09.032248 conda-project-0.1.1/PKG-INFO
--rw-r--r--   0 adefusco   (502) staff       (20)     4114 2023-04-01 01:55:09.000000 conda-project-0.1.1/README.md
-drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-06 01:04:09.017576 conda-project-0.1.1/conda.recipe/
--rw-r--r--   0 adefusco   (502) staff       (20)     1078 2023-04-06 01:03:58.000000 conda-project-0.1.1/conda.recipe/meta.yaml
-drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-06 01:04:09.017937 conda-project-0.1.1/docs/
--rw-r--r--   0 adefusco   (502) staff       (20)     1759 2023-04-06 01:03:58.000000 conda-project-0.1.1/docs/Makefile
--rw-r--r--   0 adefusco   (502) staff       (20)      112 2022-12-06 15:55:00.000000 conda-project-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-06 01:04:09.019636 conda-project-0.1.1/docs/source/
--rw-r--r--   0 adefusco   (502) staff       (20)     1771 2023-04-06 01:03:58.000000 conda-project-0.1.1/docs/source/conf.py
--rw-r--r--   0 adefusco   (502) staff       (20)      138 2023-03-28 16:19:13.000000 conda-project-0.1.1/docs/source/index.md
--rw-r--r--   0 adefusco   (502) staff       (20)     1636 2023-03-28 16:19:13.000000 conda-project-0.1.1/docs/source/setup_for_development.md
--rw-r--r--   0 adefusco   (502) staff       (20)     5873 2023-03-30 21:40:52.000000 conda-project-0.1.1/docs/source/tutorial.md
--rw-r--r--   0 adefusco   (502) staff       (20)    12563 2023-03-30 21:40:52.000000 conda-project-0.1.1/docs/source/user_guide.md
--rw-r--r--   0 adefusco   (502) staff       (20)      224 2023-04-05 14:24:50.000000 conda-project-0.1.1/environment.yml
-drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-06 01:04:09.020214 conda-project-0.1.1/etc/
--rw-r--r--   0 adefusco   (502) staff       (20)      102 2023-04-05 14:24:50.000000 conda-project-0.1.1/etc/build-environment.yml
--rw-r--r--   0 adefusco   (502) staff       (20)      228 2023-04-04 03:44:13.000000 conda-project-0.1.1/etc/test-environment.yml
-drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-06 01:04:09.020756 conda-project-0.1.1/examples/
--rw-r--r--   0 adefusco   (502) staff       (20)       95 2023-04-01 01:55:09.000000 conda-project-0.1.1/examples/.gitignore
--rw-r--r--   0 adefusco   (502) staff       (20)      621 2023-04-01 01:55:09.000000 conda-project-0.1.1/examples/README.md
-drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-06 01:04:09.022096 conda-project-0.1.1/examples/cmds-and-vars/
--rw-r--r--   0 adefusco   (502) staff       (20)     1959 2023-04-01 01:55:09.000000 conda-project-0.1.1/examples/cmds-and-vars/README.md
--rw-r--r--   0 adefusco   (502) staff       (20)    22470 2023-04-01 01:55:09.000000 conda-project-0.1.1/examples/cmds-and-vars/conda-lock.default.yml
--rw-r--r--   0 adefusco   (502) staff       (20)      317 2023-04-01 01:55:09.000000 conda-project-0.1.1/examples/cmds-and-vars/conda-project.yml
--rw-r--r--   0 adefusco   (502) staff       (20)       54 2023-04-01 01:55:09.000000 conda-project-0.1.1/examples/cmds-and-vars/environment.yml
-drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-06 01:04:09.022739 conda-project-0.1.1/examples/condarc-settings/
--rw-r--r--   0 adefusco   (502) staff       (20)       16 2023-04-01 01:55:09.000000 conda-project-0.1.1/examples/condarc-settings/.condarc
--rw-r--r--   0 adefusco   (502) staff       (20)      389 2023-04-01 01:55:09.000000 conda-project-0.1.1/examples/condarc-settings/README.md
--rw-r--r--   0 adefusco   (502) staff       (20)       92 2023-04-01 01:55:09.000000 conda-project-0.1.1/examples/condarc-settings/environment.yml
-drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-06 01:04:09.023208 conda-project-0.1.1/examples/env-file-only/
--rw-r--r--   0 adefusco   (502) staff       (20)     1434 2023-04-01 01:55:09.000000 conda-project-0.1.1/examples/env-file-only/README.md
--rw-r--r--   0 adefusco   (502) staff       (20)       40 2023-04-01 01:55:09.000000 conda-project-0.1.1/examples/env-file-only/environment.yml
-drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-06 01:04:09.025173 conda-project-0.1.1/examples/multi-env-files/
--rw-r--r--   0 adefusco   (502) staff       (20)     2971 2023-04-01 01:55:09.000000 conda-project-0.1.1/examples/multi-env-files/README.md
--rw-r--r--   0 adefusco   (502) staff       (20)    22470 2023-04-01 01:55:09.000000 conda-project-0.1.1/examples/multi-env-files/conda-lock.default.yml
--rw-r--r--   0 adefusco   (502) staff       (20)    33992 2023-04-01 01:55:09.000000 conda-project-0.1.1/examples/multi-env-files/conda-lock.test.yml
--rw-r--r--   0 adefusco   (502) staff       (20)      117 2023-04-01 01:55:09.000000 conda-project-0.1.1/examples/multi-env-files/conda-project.yml
--rw-r--r--   0 adefusco   (502) staff       (20)       54 2023-04-01 01:55:09.000000 conda-project-0.1.1/examples/multi-env-files/environment.yml
--rw-r--r--   0 adefusco   (502) staff       (20)       49 2023-04-01 01:55:09.000000 conda-project-0.1.1/examples/multi-env-files/extras.yml
--rw-r--r--   0 adefusco   (502) staff       (20)      299 2023-04-01 01:55:09.000000 conda-project-0.1.1/examples/multi-env-files/print_version.py
--rw-r--r--   0 adefusco   (502) staff       (20)      195 2023-04-01 01:55:09.000000 conda-project-0.1.1/examples/multi-env-files/test_get_version.py
--rw-r--r--   0 adefusco   (502) staff       (20)     3060 2023-04-06 01:03:58.000000 conda-project-0.1.1/pyproject.toml
--rw-r--r--   0 adefusco   (502) staff       (20)       38 2023-04-06 01:04:09.032476 conda-project-0.1.1/setup.cfg
-drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-06 01:04:09.013192 conda-project-0.1.1/src/
-drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-06 01:04:09.027241 conda-project-0.1.1/src/conda_project/
--rw-r--r--   0 adefusco   (502) staff       (20)      303 2023-04-06 01:03:58.000000 conda-project-0.1.1/src/conda_project/__init__.py
--rw-r--r--   0 adefusco   (502) staff       (20)      134 2023-04-05 14:24:50.000000 conda-project-0.1.1/src/conda_project/__main__.py
--rw-r--r--   0 adefusco   (502) staff       (20)      160 2023-04-06 01:04:08.000000 conda-project-0.1.1/src/conda_project/_version.py
-drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-06 01:04:09.029485 conda-project-0.1.1/src/conda_project/cli/
--rw-r--r--   0 adefusco   (502) staff       (20)       99 2023-04-05 14:24:50.000000 conda-project-0.1.1/src/conda_project/cli/__init__.py
--rw-r--r--   0 adefusco   (502) staff       (20)     4004 2023-04-05 14:24:50.000000 conda-project-0.1.1/src/conda_project/cli/commands.py
--rw-r--r--   0 adefusco   (502) staff       (20)    11990 2023-04-05 14:24:50.000000 conda-project-0.1.1/src/conda_project/cli/main.py
--rw-r--r--   0 adefusco   (502) staff       (20)     4775 2023-04-05 14:24:50.000000 conda-project-0.1.1/src/conda_project/conda.py
--rw-r--r--   0 adefusco   (502) staff       (20)      264 2023-04-05 14:24:50.000000 conda-project-0.1.1/src/conda_project/exceptions.py
--rw-r--r--   0 adefusco   (502) staff       (20)    27189 2023-04-05 14:24:50.000000 conda-project-0.1.1/src/conda_project/project.py
--rw-r--r--   0 adefusco   (502) staff       (20)     2619 2023-04-05 14:24:50.000000 conda-project-0.1.1/src/conda_project/project_file.py
--rw-r--r--   0 adefusco   (502) staff       (20)     4466 2023-04-05 14:24:50.000000 conda-project-0.1.1/src/conda_project/utils.py
-drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-06 01:04:09.028738 conda-project-0.1.1/src/conda_project.egg-info/
--rw-r--r--   0 adefusco   (502) staff       (20)     5543 2023-04-06 01:04:08.000000 conda-project-0.1.1/src/conda_project.egg-info/PKG-INFO
--rw-r--r--   0 adefusco   (502) staff       (20)     1904 2023-04-06 01:04:09.000000 conda-project-0.1.1/src/conda_project.egg-info/SOURCES.txt
--rw-r--r--   0 adefusco   (502) staff       (20)        1 2023-04-06 01:04:08.000000 conda-project-0.1.1/src/conda_project.egg-info/dependency_links.txt
--rw-r--r--   0 adefusco   (502) staff       (20)       62 2023-04-06 01:04:08.000000 conda-project-0.1.1/src/conda_project.egg-info/entry_points.txt
--rw-r--r--   0 adefusco   (502) staff       (20)      210 2023-04-06 01:04:08.000000 conda-project-0.1.1/src/conda_project.egg-info/requires.txt
--rw-r--r--   0 adefusco   (502) staff       (20)       14 2023-04-06 01:04:08.000000 conda-project-0.1.1/src/conda_project.egg-info/top_level.txt
-drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-06 01:04:09.031921 conda-project-0.1.1/tests/
--rw-r--r--   0 adefusco   (502) staff       (20)       99 2022-04-14 22:10:46.000000 conda-project-0.1.1/tests/__init__.py
--rw-r--r--   0 adefusco   (502) staff       (20)     2509 2023-03-28 15:38:12.000000 conda-project-0.1.1/tests/conftest.py
--rw-r--r--   0 adefusco   (502) staff       (20)    10104 2023-03-30 21:40:52.000000 conda-project-0.1.1/tests/test_cli.py
--rw-r--r--   0 adefusco   (502) staff       (20)    10585 2023-03-30 21:40:52.000000 conda-project-0.1.1/tests/test_commands.py
--rw-r--r--   0 adefusco   (502) staff       (20)     4925 2023-03-28 15:38:12.000000 conda-project-0.1.1/tests/test_conda.py
--rw-r--r--   0 adefusco   (502) staff       (20)    35061 2023-03-30 21:40:52.000000 conda-project-0.1.1/tests/test_project.py
--rw-r--r--   0 adefusco   (502) staff       (20)     4922 2023-04-01 01:55:09.000000 conda-project-0.1.1/tests/test_project_file.py
--rw-r--r--   0 adefusco   (502) staff       (20)     6869 2023-03-28 15:38:12.000000 conda-project-0.1.1/tests/test_utils.py
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.586355 conda-project-0.2.0/
+-rw-r--r--   0 adefusco   (502) staff       (20)      136 2023-04-05 14:24:50.000000 conda-project-0.2.0/.flake8
+-rw-r--r--   0 adefusco   (502) staff       (20)       58 2022-04-01 15:52:07.000000 conda-project-0.2.0/.gitattributes
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.567293 conda-project-0.2.0/.github/
+-rw-r--r--   0 adefusco   (502) staff       (20)       71 2022-04-14 22:10:46.000000 conda-project-0.2.0/.github/disclaimer.txt
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.567885 conda-project-0.2.0/.github/workflows/
+-rw-r--r--   0 adefusco   (502) staff       (20)     1163 2022-12-06 15:55:00.000000 conda-project-0.2.0/.github/workflows/docs.yml
+-rw-r--r--   0 adefusco   (502) staff       (20)     5597 2023-04-24 21:40:33.000000 conda-project-0.2.0/.github/workflows/main.yaml
+-rw-r--r--   0 adefusco   (502) staff       (20)     1913 2023-04-06 01:03:58.000000 conda-project-0.2.0/.gitignore
+-rw-r--r--   0 adefusco   (502) staff       (20)      999 2023-04-05 20:34:59.000000 conda-project-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 adefusco   (502) staff       (20)     1111 2023-04-24 21:40:33.000000 conda-project-0.2.0/CHANGELOG.md
+-rw-r--r--   0 adefusco   (502) staff       (20)     1544 2022-04-01 15:50:48.000000 conda-project-0.2.0/LICENSE
+-rw-r--r--   0 adefusco   (502) staff       (20)     6180 2023-04-24 21:41:53.586156 conda-project-0.2.0/PKG-INFO
+-rw-r--r--   0 adefusco   (502) staff       (20)     4751 2023-04-24 21:40:33.000000 conda-project-0.2.0/README.md
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.568056 conda-project-0.2.0/conda.recipe/
+-rw-r--r--   0 adefusco   (502) staff       (20)     1154 2023-04-24 21:40:33.000000 conda-project-0.2.0/conda.recipe/meta.yaml
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.568518 conda-project-0.2.0/docs/
+-rw-r--r--   0 adefusco   (502) staff       (20)     1759 2023-04-06 01:03:58.000000 conda-project-0.2.0/docs/Makefile
+-rw-r--r--   0 adefusco   (502) staff       (20)      112 2022-12-06 15:55:00.000000 conda-project-0.2.0/docs/requirements.txt
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.570545 conda-project-0.2.0/docs/source/
+-rw-r--r--   0 adefusco   (502) staff       (20)     1771 2023-04-06 01:03:58.000000 conda-project-0.2.0/docs/source/conf.py
+-rw-r--r--   0 adefusco   (502) staff       (20)     4022 2023-04-24 21:40:33.000000 conda-project-0.2.0/docs/source/experimental.md
+-rw-r--r--   0 adefusco   (502) staff       (20)      151 2023-04-24 21:40:33.000000 conda-project-0.2.0/docs/source/index.md
+-rw-r--r--   0 adefusco   (502) staff       (20)     1636 2023-03-28 16:19:13.000000 conda-project-0.2.0/docs/source/setup_for_development.md
+-rw-r--r--   0 adefusco   (502) staff       (20)     5873 2023-03-30 21:40:52.000000 conda-project-0.2.0/docs/source/tutorial.md
+-rw-r--r--   0 adefusco   (502) staff       (20)    12563 2023-03-30 21:40:52.000000 conda-project-0.2.0/docs/source/user_guide.md
+-rw-r--r--   0 adefusco   (502) staff       (20)      259 2023-04-24 21:40:33.000000 conda-project-0.2.0/environment.yml
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.571349 conda-project-0.2.0/etc/
+-rw-r--r--   0 adefusco   (502) staff       (20)      102 2023-04-05 14:24:50.000000 conda-project-0.2.0/etc/build-environment.yml
+-rw-r--r--   0 adefusco   (502) staff       (20)      263 2023-04-24 21:40:33.000000 conda-project-0.2.0/etc/test-environment.yml
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.571753 conda-project-0.2.0/examples/
+-rw-r--r--   0 adefusco   (502) staff       (20)       95 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/.gitignore
+-rw-r--r--   0 adefusco   (502) staff       (20)      621 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/README.md
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.573179 conda-project-0.2.0/examples/cmds-and-vars/
+-rw-r--r--   0 adefusco   (502) staff       (20)     1959 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/cmds-and-vars/README.md
+-rw-r--r--   0 adefusco   (502) staff       (20)    22470 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/cmds-and-vars/conda-lock.default.yml
+-rw-r--r--   0 adefusco   (502) staff       (20)      317 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/cmds-and-vars/conda-project.yml
+-rw-r--r--   0 adefusco   (502) staff       (20)       54 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/cmds-and-vars/environment.yml
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.573787 conda-project-0.2.0/examples/condarc-settings/
+-rw-r--r--   0 adefusco   (502) staff       (20)       16 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/condarc-settings/.condarc
+-rw-r--r--   0 adefusco   (502) staff       (20)      389 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/condarc-settings/README.md
+-rw-r--r--   0 adefusco   (502) staff       (20)       92 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/condarc-settings/environment.yml
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.574322 conda-project-0.2.0/examples/env-file-only/
+-rw-r--r--   0 adefusco   (502) staff       (20)     1434 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/env-file-only/README.md
+-rw-r--r--   0 adefusco   (502) staff       (20)       40 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/env-file-only/environment.yml
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.576299 conda-project-0.2.0/examples/multi-env-files/
+-rw-r--r--   0 adefusco   (502) staff       (20)     2971 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/multi-env-files/README.md
+-rw-r--r--   0 adefusco   (502) staff       (20)    22470 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/multi-env-files/conda-lock.default.yml
+-rw-r--r--   0 adefusco   (502) staff       (20)    33992 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/multi-env-files/conda-lock.test.yml
+-rw-r--r--   0 adefusco   (502) staff       (20)      117 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/multi-env-files/conda-project.yml
+-rw-r--r--   0 adefusco   (502) staff       (20)       54 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/multi-env-files/environment.yml
+-rw-r--r--   0 adefusco   (502) staff       (20)       49 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/multi-env-files/extras.yml
+-rw-r--r--   0 adefusco   (502) staff       (20)      299 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/multi-env-files/print_version.py
+-rw-r--r--   0 adefusco   (502) staff       (20)      195 2023-04-01 01:55:09.000000 conda-project-0.2.0/examples/multi-env-files/test_get_version.py
+-rw-r--r--   0 adefusco   (502) staff       (20)     3120 2023-04-24 21:40:33.000000 conda-project-0.2.0/pyproject.toml
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.576520 conda-project-0.2.0/scripts/
+-rw-r--r--   0 adefusco   (502) staff       (20)     6189 2023-04-24 21:40:33.000000 conda-project-0.2.0/scripts/ap-to-cp.py
+-rw-r--r--   0 adefusco   (502) staff       (20)       38 2023-04-24 21:41:53.586422 conda-project-0.2.0/setup.cfg
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.564498 conda-project-0.2.0/src/
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.579357 conda-project-0.2.0/src/conda_project/
+-rw-r--r--   0 adefusco   (502) staff       (20)      303 2023-04-06 01:03:58.000000 conda-project-0.2.0/src/conda_project/__init__.py
+-rw-r--r--   0 adefusco   (502) staff       (20)      134 2023-04-05 14:24:50.000000 conda-project-0.2.0/src/conda_project/__main__.py
+-rw-r--r--   0 adefusco   (502) staff       (20)      160 2023-04-24 21:41:53.000000 conda-project-0.2.0/src/conda_project/_version.py
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.581736 conda-project-0.2.0/src/conda_project/cli/
+-rw-r--r--   0 adefusco   (502) staff       (20)       99 2023-04-05 14:24:50.000000 conda-project-0.2.0/src/conda_project/cli/__init__.py
+-rw-r--r--   0 adefusco   (502) staff       (20)     4687 2023-04-24 21:40:33.000000 conda-project-0.2.0/src/conda_project/cli/commands.py
+-rw-r--r--   0 adefusco   (502) staff       (20)    13155 2023-04-24 21:40:33.000000 conda-project-0.2.0/src/conda_project/cli/main.py
+-rw-r--r--   0 adefusco   (502) staff       (20)     5094 2023-04-24 21:40:33.000000 conda-project-0.2.0/src/conda_project/conda.py
+-rw-r--r--   0 adefusco   (502) staff       (20)     6798 2023-04-21 15:52:22.000000 conda-project-0.2.0/src/conda_project/conda_transfer.py
+-rw-r--r--   0 adefusco   (502) staff       (20)      264 2023-04-11 15:51:33.000000 conda-project-0.2.0/src/conda_project/exceptions.py
+-rw-r--r--   0 adefusco   (502) staff       (20)    30045 2023-04-24 21:40:33.000000 conda-project-0.2.0/src/conda_project/project.py
+-rw-r--r--   0 adefusco   (502) staff       (20)     2619 2023-04-24 00:49:12.000000 conda-project-0.2.0/src/conda_project/project_file.py
+-rw-r--r--   0 adefusco   (502) staff       (20)     5010 2023-04-24 21:40:33.000000 conda-project-0.2.0/src/conda_project/utils.py
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.580713 conda-project-0.2.0/src/conda_project.egg-info/
+-rw-r--r--   0 adefusco   (502) staff       (20)     6180 2023-04-24 21:41:53.000000 conda-project-0.2.0/src/conda_project.egg-info/PKG-INFO
+-rw-r--r--   0 adefusco   (502) staff       (20)     2158 2023-04-24 21:41:53.000000 conda-project-0.2.0/src/conda_project.egg-info/SOURCES.txt
+-rw-r--r--   0 adefusco   (502) staff       (20)        1 2023-04-24 21:41:53.000000 conda-project-0.2.0/src/conda_project.egg-info/dependency_links.txt
+-rw-r--r--   0 adefusco   (502) staff       (20)       62 2023-04-24 21:41:53.000000 conda-project-0.2.0/src/conda_project.egg-info/entry_points.txt
+-rw-r--r--   0 adefusco   (502) staff       (20)      230 2023-04-24 21:41:53.000000 conda-project-0.2.0/src/conda_project.egg-info/requires.txt
+-rw-r--r--   0 adefusco   (502) staff       (20)       14 2023-04-24 21:41:53.000000 conda-project-0.2.0/src/conda_project.egg-info/top_level.txt
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.585073 conda-project-0.2.0/tests/
+-rw-r--r--   0 adefusco   (502) staff       (20)       99 2022-04-14 22:10:46.000000 conda-project-0.2.0/tests/__init__.py
+drwxr-xr-x   0 adefusco   (502) staff       (20)        0 2023-04-24 21:41:53.585824 conda-project-0.2.0/tests/assets/
+-rw-r--r--   0 adefusco   (502) staff       (20)     6798 2023-04-24 21:40:33.000000 conda-project-0.2.0/tests/assets/no-top-level-dir.tar.gz
+-rw-r--r--   0 adefusco   (502) staff       (20)     6850 2023-04-24 21:40:33.000000 conda-project-0.2.0/tests/assets/relative-paths.tar.gz
+-rw-r--r--   0 adefusco   (502) staff       (20)     6855 2023-04-24 21:40:33.000000 conda-project-0.2.0/tests/assets/top-level-dir.tar.gz
+-rw-r--r--   0 adefusco   (502) staff       (20)     6848 2023-04-24 21:40:33.000000 conda-project-0.2.0/tests/assets/unnamed-top-level-dir.tar.gz
+-rw-r--r--   0 adefusco   (502) staff       (20)     2509 2023-04-18 17:50:49.000000 conda-project-0.2.0/tests/conftest.py
+-rw-r--r--   0 adefusco   (502) staff       (20)     3665 2023-04-24 21:40:33.000000 conda-project-0.2.0/tests/test_archive.py
+-rw-r--r--   0 adefusco   (502) staff       (20)    11521 2023-04-24 21:40:33.000000 conda-project-0.2.0/tests/test_cli.py
+-rw-r--r--   0 adefusco   (502) staff       (20)    12269 2023-04-24 21:40:33.000000 conda-project-0.2.0/tests/test_commands.py
+-rw-r--r--   0 adefusco   (502) staff       (20)     6297 2023-04-24 21:40:33.000000 conda-project-0.2.0/tests/test_conda.py
+-rw-r--r--   0 adefusco   (502) staff       (20)    35061 2023-04-19 03:34:42.000000 conda-project-0.2.0/tests/test_project.py
+-rw-r--r--   0 adefusco   (502) staff       (20)     4922 2023-04-01 01:55:09.000000 conda-project-0.2.0/tests/test_project_file.py
+-rw-r--r--   0 adefusco   (502) staff       (20)     7628 2023-04-24 21:40:33.000000 conda-project-0.2.0/tests/test_utils.py
```

### Comparing `conda-project-0.1.1/.github/workflows/docs.yml` & `conda-project-0.2.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `conda-project-0.1.1/.github/workflows/main.yaml` & `conda-project-0.2.0/.github/workflows/main.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             python-version: "3.10"
           - conda-version: "4.11"
             python-version: "3.10"
     env:
       OS: ${{ matrix.os }}
       PYTHON: ${{ matrix.python-version }}
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Download conda standalone
         shell: bash
         run: |
           if [ $RUNNER_OS == 'Linux' ]; then
             curl https://repo.anaconda.com/pkgs/misc/conda-execs/conda-latest-linux-64.exe -o conda.exe
           elif [ $RUNNER_OS == 'Windows' ]; then
             curl https://repo.anaconda.com/pkgs/misc/conda-execs/conda-4.10.3-win-64.exe -o conda.exe
@@ -122,15 +122,15 @@
           env_vars: OS,PYTHON
   upload:
     needs: test
     runs-on: ubuntu-latest
     if: github.event_name == 'push'
     steps:
     - name: Retrieve the source code
-      uses: actions/checkout@v2
+      uses: actions/checkout@v3
       with:
         fetch-depth: 0
     - name: Download the build artifacts
       uses: actions/download-artifact@v2
       with:
         name: package-${{ github.sha }}
         path: conda-bld
```

### Comparing `conda-project-0.1.1/.gitignore` & `conda-project-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `conda-project-0.1.1/.pre-commit-config.yaml` & `conda-project-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `conda-project-0.1.1/LICENSE` & `conda-project-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `conda-project-0.1.1/PKG-INFO` & `conda-project-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conda-project
-Version: 0.1.1
+Version: 0.2.0
 Summary: Tool for encapsulating, running, and reproducing projects with conda environments
 Author-email: Albert DeFusco <adefusco@anaconda.com>, Matt Kramer <mkramer@anaconda.com>
 License: BSD-3-Clause
 Project-URL: repository, https://github.com/conda-incubator/conda-project
 Project-URL: homepage, https://github.com/conda-incubator/conda-project
 Project-URL: documentation, https://conda-incubator.github.io/conda-project/user_guide.html
 Project-URL: Issue Tracker, https://github.com/conda-incubator/conda-project/issues
@@ -31,26 +31,38 @@
 # conda-project
 
 [![codecov](https://codecov.io/gh/conda-incubator/conda-project/branch/main/graph/badge.svg?token=XNRS8JKT75)](https://codecov.io/gh/conda-incubator/conda-project)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/conda-incubator/conda-project/main.svg)](https://results.pre-commit.ci/latest/github/conda-incubator/conda-project/main)
 
 Tool for encapsulating, running, and reproducing projects with conda environments.
 
-This package is intended as a successor to [Anaconda Project](https://github.com/Anaconda-Platform/anaconda-project).
 
 ## Why?
 
 Sharing your work is more than sharing your code in a script file or notebook. To make your work properly reproducible, it is necessary to include the list of required third-party dependencies, specifications for how to run your code, and
 any other files that it may need.
 
 See [8 Levels of Reproduciblity](https://www.anaconda.com/blog/8-levels-of-reproducibility) for an in-depth
 discussion of the differences between "It works for me." to "I've made sure that anyone can reliably execute my work."
 Conda Project is a framework that aims to help you to ensure a high degree of reproducibility in the projects you
 create.
 
+### How is this different from Anaconda Project?
+
+This package is intended as a successor to [Anaconda Project](https://github.com/Anaconda-Platform/anaconda-project).
+We chose to create Conda Project to foster community involvement, adopt newer standards like conda-lock, and provide
+a conda-native workflow. A standalone conversion script is provided in this repo at `scripts/ap-to-cp.py`. You can run
+it as follows. By default it will write Conda Project files into your current working directory. You can read anaconda-project.yml file from any other directory or output Conda Project files to any other directory.
+
+You'll need `pydantic` and `ruamel.yaml` installed.
+
+```text
+python ap-to-cp.py /path/to/anaconda-project.yml [/output/directory]
+```
+
 ## Installation
 
 You can install conda-project using the conda package manager:
 
 ```text
 conda install -c conda-forge conda-project
 ```
```

### Comparing `conda-project-0.1.1/README.md` & `conda-project-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,38 @@
 # conda-project
 
 [![codecov](https://codecov.io/gh/conda-incubator/conda-project/branch/main/graph/badge.svg?token=XNRS8JKT75)](https://codecov.io/gh/conda-incubator/conda-project)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/conda-incubator/conda-project/main.svg)](https://results.pre-commit.ci/latest/github/conda-incubator/conda-project/main)
 
 Tool for encapsulating, running, and reproducing projects with conda environments.
 
-This package is intended as a successor to [Anaconda Project](https://github.com/Anaconda-Platform/anaconda-project).
 
 ## Why?
 
 Sharing your work is more than sharing your code in a script file or notebook. To make your work properly reproducible, it is necessary to include the list of required third-party dependencies, specifications for how to run your code, and
 any other files that it may need.
 
 See [8 Levels of Reproduciblity](https://www.anaconda.com/blog/8-levels-of-reproducibility) for an in-depth
 discussion of the differences between "It works for me." to "I've made sure that anyone can reliably execute my work."
 Conda Project is a framework that aims to help you to ensure a high degree of reproducibility in the projects you
 create.
 
+### How is this different from Anaconda Project?
+
+This package is intended as a successor to [Anaconda Project](https://github.com/Anaconda-Platform/anaconda-project).
+We chose to create Conda Project to foster community involvement, adopt newer standards like conda-lock, and provide
+a conda-native workflow. A standalone conversion script is provided in this repo at `scripts/ap-to-cp.py`. You can run
+it as follows. By default it will write Conda Project files into your current working directory. You can read anaconda-project.yml file from any other directory or output Conda Project files to any other directory.
+
+You'll need `pydantic` and `ruamel.yaml` installed.
+
+```text
+python ap-to-cp.py /path/to/anaconda-project.yml [/output/directory]
+```
+
 ## Installation
 
 You can install conda-project using the conda package manager:
 
 ```text
 conda install -c conda-forge conda-project
 ```
```

### Comparing `conda-project-0.1.1/conda.recipe/meta.yaml` & `conda-project-0.2.0/conda.recipe/meta.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -22,17 +22,23 @@
 requirements:
   host:
     - python {{ project['requires-python'] }}
     - pip
     - setuptools
   run:
     - python {{ project['requires-python'] }}
-    {% for dep in project['dependencies'] %}
-    - {{ dep.lower() }}
-    {% endfor %}
+    - conda-lock >=1.2
+    - lockfile
+    - pexpect
+    - ruamel.yaml
+    - pydantic
+    - shellingham
+    - python-dotenv
+    - fsspec
+    - python-libarchive-c
 
 test:
   imports:
     - conda_project
   commands:
     - conda-project --help
     - conda-project --version
```

### Comparing `conda-project-0.1.1/docs/Makefile` & `conda-project-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `conda-project-0.1.1/docs/source/conf.py` & `conda-project-0.2.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `conda-project-0.1.1/docs/source/setup_for_development.md` & `conda-project-0.2.0/docs/source/setup_for_development.md`

 * *Files identical despite different names*

### Comparing `conda-project-0.1.1/docs/source/tutorial.md` & `conda-project-0.2.0/docs/source/tutorial.md`

 * *Files identical despite different names*

### Comparing `conda-project-0.1.1/docs/source/user_guide.md` & `conda-project-0.2.0/docs/source/user_guide.md`

 * *Files identical despite different names*

### Comparing `conda-project-0.1.1/examples/README.md` & `conda-project-0.2.0/examples/README.md`

 * *Files identical despite different names*

### Comparing `conda-project-0.1.1/examples/cmds-and-vars/README.md` & `conda-project-0.2.0/examples/cmds-and-vars/README.md`

 * *Files identical despite different names*

### Comparing `conda-project-0.1.1/examples/cmds-and-vars/conda-lock.default.yml` & `conda-project-0.2.0/examples/cmds-and-vars/conda-lock.default.yml`

 * *Files identical despite different names*

### Comparing `conda-project-0.1.1/examples/env-file-only/README.md` & `conda-project-0.2.0/examples/env-file-only/README.md`

 * *Files identical despite different names*

### Comparing `conda-project-0.1.1/examples/multi-env-files/README.md` & `conda-project-0.2.0/examples/multi-env-files/README.md`

 * *Files identical despite different names*

### Comparing `conda-project-0.1.1/examples/multi-env-files/conda-lock.default.yml` & `conda-project-0.2.0/examples/multi-env-files/conda-lock.default.yml`

 * *Files identical despite different names*

### Comparing `conda-project-0.1.1/examples/multi-env-files/conda-lock.test.yml` & `conda-project-0.2.0/examples/multi-env-files/conda-lock.test.yml`

 * *Files identical despite different names*

### Comparing `conda-project-0.1.1/pyproject.toml` & `conda-project-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,16 @@
     "conda-lock >=1.2",
     "lockfile",
     "pexpect",
     "ruamel.yaml",
     "pydantic",
     "shellingham",
     "python-dotenv",
+    "fsspec",
+    "libarchive-c"
 ]
 
 [tool.setuptools_scm]
 version_scheme = "post-release"
 write_to = "src/conda_project/_version.py"
 
 [project.optional-dependencies]
@@ -64,14 +66,15 @@
 #"Conda-Forge Feedstock" = "https://github.com/conda-forge/conda-project-feedstock"
 #"AnacondaRecipes Feedstock" = "https://github.com/AnacondaRecipes/conda-project-feedstock"
 
 [tool.coverage.report]
 omit = [
     "conda_project/__main__.py",
     "tests/*",
+    "scripts/*"
 ]
 exclude_lines = [
     "pragma: no cover",
     # This covers both typing.TYPE_CHECKING and plain TYPE_CHECKING, with any amount of whitespace
     "if\\s+(typing\\.)?TYPE_CHECKING:",
     'if __name__ == "__main__":'
 ]
@@ -85,13 +88,13 @@
 [tool.mypy]
 files = [ "src/conda_project/**/*.py" ]
 python_version = "3.8"
 disallow_untyped_defs = true
 warn_no_return = true
 
 [tool.pytest.ini_options]
-norecursedirs = [".*", "*.egg*", "build", "dist", "conda.recipe", "examples", "env"]
+norecursedirs = [".*", "*.egg*", "build", "dist", "conda.recipe", "examples", "env", "scripts"]
 addopts = "-vv --cov-report term-missing --cov conda_project --tb native --strict-markers --durations=20"
 markers = [
     "serial: execute test serially (to avoid race conditions)",
     "slow: tests can take a long time (deselect with '-m \"not slow\"')",
 ]
```

### Comparing `conda-project-0.1.1/src/conda_project/cli/commands.py` & `conda-project-0.2.0/src/conda_project/cli/commands.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,38 @@
 
 from ..exceptions import CommandNotFoundError, CondaProjectError
 from ..project import Command, CondaProject
 
 logger = logging.getLogger(__name__)
 
 
+def _load_project(args: Namespace):
+    if args.project_archive is not None:
+        _storage_options = (
+            []
+            if args.archive_storage_options is None
+            else args.archive_storage_options.split(",")
+        )
+
+        storage_options = {}
+        for option in _storage_options:
+            k, v = option.split("=")
+            storage_options[k] = v
+
+        project = CondaProject.from_archive(
+            args.project_archive,
+            storage_options=storage_options,
+            output_directory=args.directory,
+        )
+    else:
+        project = CondaProject(args.directory)
+
+    return project
+
+
 def handle_errors(func: Callable[[Namespace], Any]) -> Callable[[Namespace], int]:
     """Wrap a subcommand function to catch exceptions and return an appropriate error code."""
 
     @wraps(func)
     def wrapper(args: Namespace) -> int:
         try:
             ret = func(args)
@@ -57,36 +81,36 @@
         "The 'create' subcommand is an alias for 'init' and may be removed in a future version."
     )
     return init(args)
 
 
 @handle_errors
 def lock(args: Namespace) -> bool:
-    project = CondaProject(args.directory)
+    project = _load_project(args)
 
     if args.environment:
         to_lock = [project.environments[args.environment]]
     else:
         to_lock = project.environments.values()
 
     for env in to_lock:
         env.lock(force=args.force, verbose=True)
 
     return True
 
 
 @handle_errors
 def check(args: Namespace) -> bool:
-    project = CondaProject(args.directory)
+    project = _load_project(args)
     return project.check(verbose=True)
 
 
 @handle_errors
 def install(args: Namespace) -> bool:
-    project = CondaProject(args.directory)
+    project = _load_project(args)
 
     if args.all:
         for _, env in project.environments:
             env.install(force=args.force, verbose=True)
     else:
         env = (
             project.environments[args.environment]
@@ -121,35 +145,40 @@
         env.clean(verbose=True)
 
     return True
 
 
 @handle_errors
 def run(args: Namespace) -> NoReturn:
-    project = CondaProject(args.directory)
+    project = _load_project(args)
 
     if args.command:
         try:
             to_run = project.commands[args.command]
         except CommandNotFoundError:
             to_run = Command(
                 name=str(args.command),
                 cmd=args.command,
                 environment=project.default_environment,
                 project=project,
             )
     else:
         to_run = project.default_command
 
-    to_run.run(environment=args.environment, extra_args=args.extra_args, verbose=True)
+    to_run.run(
+        environment=args.environment,
+        external_environment=args.external_environment,
+        extra_args=args.extra_args,
+        verbose=True,
+    )
 
 
 @handle_errors
 def activate(args: Namespace) -> bool:
-    project = CondaProject(args.directory)
+    project = _load_project(args)
 
     if args.environment:
         env = project.environments[args.environment]
     else:
         env = project.default_environment
 
     env.activate(verbose=True)
```

### Comparing `conda-project-0.1.1/src/conda_project/cli/main.py` & `conda-project-0.2.0/src/conda_project/cli/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,14 +23,35 @@
     common.add_argument(
         "--directory",
         metavar="PROJECT_DIR",
         default=".",
         help="Project directory (defaults to current directory)",
     )
 
+    extras = ArgumentParser(add_help=False)
+    extras.add_argument(
+        "--project-archive",
+        metavar="PROJECT_ARCHIVE_FILE_OR_URL",
+        help=(
+            "EXPERIMENTAL: Extract and run directly from a project archive. The archive can be a local file "
+            "or a fsspec compatible URL. You may need to install appropriate driver packages to work with "
+            "remote archives. Optionally, use --directory to set the destination directory of the extracted "
+            "project."
+        ),
+    )
+    extras.add_argument(
+        "--archive-storage-options",
+        help=(
+            "EXPERIMENTAL: Comma separated list of fsspec storage_options for accessing a remote archive "
+            "For example --archive-storage-options username=<user>,password=<pass>"
+        ),
+        action="store",
+        default=None,
+    )
+
     p = ArgumentParser(
         description="Tool for encapsulating, running, and reproducing projects with conda environments",
         conflict_handler="resolve",
     )
     p.add_argument(
         "-V",
         "--version",
@@ -38,40 +59,40 @@
         help="Show the conda-prefix-replacement version number and exit.",
         version="conda_project %s" % __version__,
     )
 
     subparsers = p.add_subparsers(metavar="command", required=True)
 
     _create_init_parser(subparsers, common)
-    _create_lock_parser(subparsers, common)
-    _create_check_parser(subparsers, common)
-    _create_install_parser(subparsers, common)
-    _create_activate_parser(subparsers, common)
+    _create_lock_parser(subparsers, common, extras)
+    _create_check_parser(subparsers, common, extras)
+    _create_install_parser(subparsers, common, extras)
+    _create_activate_parser(subparsers, common, extras)
     _create_clean_parser(subparsers, common)
-    _create_run_parser(subparsers, common)
+    _create_run_parser(subparsers, common, extras)
 
     return p
 
 
 def _create_init_parser(
-    subparsers: "_SubParsersAction", parent_parser: ArgumentParser
+    subparsers: "_SubParsersAction", *parent_parsers: ArgumentParser
 ) -> None:
     """Add a subparser for the "init" and "create" subcommands.
 
     Args:
         subparsers: The existing subparsers corresponding to the "command" meta-variable.
-        parent_parser: The parent parser, which is used to pass common arguments into the subcommands.
+        parent_parsers: The parent parsers, which are used to pass common arguments into the subcommands.
 
     """
     desc = "Initialize a new project"
 
     # TODO: If we deprecate "create", this loop can go away.
     for subcommand_name in ["init", "create"]:
         p = subparsers.add_parser(
-            subcommand_name, description=desc, help=desc, parents=[parent_parser]
+            subcommand_name, description=desc, help=desc, parents=parent_parsers
         )
         p.add_argument(
             "-n", "--name", help="Name for the project.", action="store", default=None
         )
         p.add_argument(
             "-c",
             "--channel",
@@ -121,27 +142,27 @@
             metavar="PACKAGE_SPECIFICATION",
         )
 
         p.set_defaults(func=getattr(commands, subcommand_name))
 
 
 def _create_lock_parser(
-    subparsers: "_SubParsersAction", parent_parser: ArgumentParser
+    subparsers: "_SubParsersAction", *parent_parsers: ArgumentParser
 ) -> None:
     """Add a subparser for the "lock" subcommand.
 
     Args:
         subparsers: The existing subparsers corresponding to the "command" meta-variable.
-        parent_parser: The parent parser, which is used to pass common arguments into the subcommands.
+        parent_parsers: The parent parsers, which are used to pass common arguments into the subcommands.
 
     """
     desc = "Lock all conda environments or a specific one by creating conda-lock.<env>.yml file(s)."
 
     p = subparsers.add_parser(
-        "lock", description=desc, help=desc, parents=[parent_parser]
+        "lock", description=desc, help=desc, parents=parent_parsers
     )
     p.add_argument(
         "environment",
         help="Optional: Lock the selected environment. If no environment name is selected "
         "all environments are locked.",
         nargs="?",
     )
@@ -151,52 +172,52 @@
         action="store_true",
     )
 
     p.set_defaults(func=commands.lock)
 
 
 def _create_check_parser(
-    subparsers: "_SubParsersAction", parent_parser: ArgumentParser
+    subparsers: "_SubParsersAction", *parent_parsers: ArgumentParser
 ) -> None:
     """Add a subparser for the "lock" subcommand.
 
     Args:
         subparsers: The existing subparsers corresponding to the "command" meta-variable.
-        parent_parser: The parent parser, which is used to pass common arguments into the subcommands.
+        parent_parsers: The parent parsers, which are used to pass common arguments into the subcommands.
 
     """
     desc = (
         "Check the project for inconsistencies or errors. This will check that conda-lock.<env>.yml file(s) "
         "have been created for each environment and are up-to-date with the source environment specifications. "
         "If the project is fully locked this command will not print anything and return status code 0. If any "
         "environment is not fully locked details are printed to stderr and the command returns status code 1."
     )
 
     p = subparsers.add_parser(
-        "check", description=desc, help=desc, parents=[parent_parser]
+        "check", description=desc, help=desc, parents=parent_parsers
     )
 
     p.set_defaults(func=commands.check)
 
 
 def _create_install_parser(
-    subparsers: "_SubParsersAction", parent_parser: ArgumentParser
+    subparsers: "_SubParsersAction", *parent_parsers: ArgumentParser
 ) -> None:
     """Add a subparser for the "install" and "prepare" subcommands.
 
     Args:
         subparsers: The existing subparsers corresponding to the "command" meta-variable.
-        parent_parser: The parent parser, which is used to pass common arguments into the subcommands.
+        parent_parsers: The parent parsers, which are used to pass common arguments into the subcommands.
 
     """
     desc = "Install the packages into the conda environments"
 
     for subcommand_name in ["install", "prepare"]:
         p = subparsers.add_parser(
-            subcommand_name, description=desc, help=desc, parents=[parent_parser]
+            subcommand_name, description=desc, help=desc, parents=parent_parsers
         )
         group = p.add_mutually_exclusive_group(required=False)
         group.add_argument(
             "environment",
             help="Prepare the selected environment. If no environment name is selected "
             "the first environment defined in the conda-project.yml file is prepared.",
             nargs="?",
@@ -226,27 +247,27 @@
             action="store_true",
         )
 
         p.set_defaults(func=getattr(commands, subcommand_name))
 
 
 def _create_clean_parser(
-    subparsers: "_SubParsersAction", parent_parser: ArgumentParser
+    subparsers: "_SubParsersAction", *parent_parsers: ArgumentParser
 ) -> None:
     """Add a subparser for the "clean" subcommand.
 
     Args:
         subparsers: The existing subparsers corresponding to the "command" meta-variable.
-        parent_parser: The parent parser, which is used to pass common arguments into the subcommands.
+        parent_parsers: The parent parsers, which are used to pass common arguments into the subcommands.
 
     """
     desc = "Clean the conda environments"
 
     p = subparsers.add_parser(
-        "clean", description=desc, help=desc, parents=[parent_parser]
+        "clean", description=desc, help=desc, parents=parent_parsers
     )
     p.add_argument(
         "environment",
         help="Remove environment prefix for selected environment. If no environment name is selected "
         "the first environment defined in the conda-project.yml file is removed.",
         nargs="?",
     )
@@ -254,36 +275,43 @@
         "--all", help="Prepare all defined environments.", action="store_true"
     )
 
     p.set_defaults(func=commands.clean)
 
 
 def _create_run_parser(
-    subparsers: "_SubParsersAction", parent_parser: ArgumentParser
+    subparsers: "_SubParsersAction", *parent_parsers: ArgumentParser
 ) -> None:
     """Add a subparser for the "run" subcommand.
 
     Args:
         subparsers: The existing subparsers corresponding to the "command" meta-variable.
-        parent_parser: The parent parser, which is used to pass common arguments into the subcommands.
+        parent_parsers: The parent parsers, which are used to pass common arguments into the subcommands.
 
     """
     desc = "Run commands in project environments."
 
     p = subparsers.add_parser(
-        "run", description=desc, help=desc, parents=[parent_parser]
+        "run", description=desc, help=desc, parents=parent_parsers
     )
     p.add_argument(
         "--environment",
         help=(
             "Specify the environment in which to run the command. The default environment for the command is either "
             "what was specified in the command definition or the first environment defined in the project."
         ),
     )
     p.add_argument(
+        "--external-environment",
+        metavar="ENV_NAME_OR_PREFIX",
+        help=(
+            "EXPERIMENTAL: Specify the name or prefix path to a conda environment not declared in this project."
+        ),
+    )
+    p.add_argument(
         "command",
         help="Optional: Run a command in the conda environment. The full command can be provided on the CLI "
         "or the name of a command defined in the conda-project.yml file. If no command is provided "
         "the first command in the conda-project.yml file is run if there is one.",
         nargs="?",
     )
     p.add_argument(
@@ -293,27 +321,27 @@
         default=None,
     )
 
     p.set_defaults(func=commands.run)
 
 
 def _create_activate_parser(
-    subparsers: "_SubParsersAction", parent_parser: ArgumentParser
+    subparsers: "_SubParsersAction", *parent_parsers: ArgumentParser
 ) -> None:
     """Add a subparser for the "run" subcommand.
 
     Args:
         subparsers: The existing subparsers corresponding to the "command" meta-variable.
-        parent_parser: The parent parser, which is used to pass common arguments into the subcommands.
+        parent_parsers: The parent parsers, which are used to pass common arguments into the subcommands.
 
     """
     desc = "Activate a conda environment defined in the environment.yml or conda-project.yml files."
 
     p = subparsers.add_parser(
-        "activate", description=desc, help=desc, parents=[parent_parser]
+        "activate", description=desc, help=desc, parents=parent_parsers
     )
     p.add_argument(
         "environment",
         help="Activate selected environment in a new shell. If no environment name is selected "
         "the first environment defined in the conda-project.yml file is activated.",
         nargs="?",
     )
```

### Comparing `conda-project-0.1.1/src/conda_project/conda.py` & `conda-project-0.2.0/src/conda_project/conda.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,22 +7,21 @@
 import os
 import shlex
 import signal
 import subprocess
 from functools import lru_cache
 from logging import Logger
 from pathlib import Path
-from typing import Dict, List, NoReturn, Optional
+from typing import Dict, List, NoReturn, Optional, Union
 
 import pexpect
-import shellingham
 from conda_lock._vendor.conda.utils import wrap_subprocess_call
 
 from .exceptions import CondaProjectError
-from .utils import execvped, is_windows
+from .utils import detect_shell, execvped, is_windows
 
 CONDA_EXE = os.environ.get("CONDA_EXE", "conda")
 CONDA_ROOT = os.environ.get("CONDA_ROOT")
 CONDA_PREFIX = os.environ.get("CONDA_PREFIX")
 
 
 def call_conda(
@@ -61,14 +60,40 @@
     if proc.returncode != 0:
         print_cmd = " ".join(cmd)
         raise CondaProjectError(f"Failed to run:\n  {print_cmd}\n{proc.stderr.strip()}")
 
     return proc
 
 
+def is_conda_env(path: Path) -> bool:
+    return (path / "conda-meta" / "history").exists()
+
+
+def conda_prefix(env: Optional[Union[str, Path]] = None) -> Path:
+    """Return the path to a conda environment"""
+
+    if env is None:
+        return Path(os.environ["CONDA_PREFIX"]).resolve()
+
+    elif env in ("base", "root"):
+        return Path(os.environ["CONDA_ROOT"]).resolve()
+
+    else:
+        env = Path(env) if isinstance(env, str) else env
+
+        if is_conda_env(env):
+            return env.resolve()
+
+        else:
+            for d in conda_info()["envs_dirs"]:
+                p = Path(d) / env
+                if is_conda_env(p):
+                    return p.resolve()
+
+
 def conda_info():
     proc = call_conda(["info", "--json"])
     parsed = json.loads(proc.stdout)
     return parsed
 
 
 @lru_cache()
@@ -101,15 +126,15 @@
 
     if not is_windows():
         args = ["-c", *args]
 
     execvped(file=shell, args=args, env=env, cwd=working_dir)
 
 
-def _send_activation(child_shell, prefix):
+def _send_activation(child_shell: pexpect.spawn, prefix):
     def sigwinch_passthrough(sig, data):
         if not child_shell.closed:
             t = os.get_terminal_size()
             child_shell.setwinsize(t.lines, t.columns)
 
     t = os.get_terminal_size()
     child_shell.setwinsize(t.lines, t.columns)
@@ -118,23 +143,15 @@
     child_shell.interact()
     child_shell.close()
 
 
 def conda_activate(prefix: Path, working_dir: Path, env: Optional[Dict] = None):
     env = {} if env is None else env
 
-    try:
-        shell_name, shell_path = shellingham.detect_shell()
-    except shellingham.ShellDetectionFailure:
-        if os.name == "posix":
-            shell_name = shell_path = os.environ.get("SHELL", "/bin/sh")
-        elif os.name == "nt":
-            shell_name = shell_path = os.environ.get("COMSPEC", "cmd.exe")
-        else:
-            raise RuntimeError("Could not determine an appropriate shell to activate.")
+    shell_path, shell_name = detect_shell()
 
     args = []
     if is_windows():
         if shell_name in ["powershell", "pwsh"]:
             conda_hook = str(Path(CONDA_ROOT) / "shell" / "condabin" / "conda-hook.ps1")
             args = [
                 "-ExecutionPolicy",
@@ -158,11 +175,11 @@
     )
     print(activate_message)
 
     if is_windows():
         subprocess.run([shell_path, *args], cwd=working_dir, env=env)
     else:
         child_shell = pexpect.spawn(
-            command=shell_path, args=args, cwd=working_dir, env=env, echo=False
+            command=shell_path, args=args, cwd=working_dir, env=env, echo=True
         )
 
         _send_activation(child_shell, prefix)
```

### Comparing `conda-project-0.1.1/src/conda_project/project.py` & `conda-project-0.2.0/src/conda_project/project.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,26 +15,35 @@
 from collections import OrderedDict
 from contextlib import nullcontext, redirect_stderr
 from io import StringIO
 from pathlib import Path
 from subprocess import SubprocessError
 from typing import Dict, List, NoReturn, Optional, Tuple, Union
 
+import fsspec
 from conda_lock._vendor.conda.core.prefix_data import PrefixData
 from conda_lock._vendor.conda.models.records import PackageType
 from conda_lock.conda_lock import (
     default_virtual_package_repodata,
     make_lock_files,
     make_lock_spec,
     parse_conda_lock_file,
     render_lockfile_for_platform,
 )
+from fsspec.core import split_protocol
 from pydantic import BaseModel, create_model
 
-from .conda import CONDA_EXE, call_conda, conda_activate, conda_run, current_platform
+from .conda import (
+    CONDA_EXE,
+    call_conda,
+    conda_activate,
+    conda_prefix,
+    conda_run,
+    current_platform,
+)
 from .exceptions import CommandNotFoundError, CondaProjectError, CondaProjectLockFailed
 from .project_file import (
     ENVIRONMENT_YAML_FILENAMES,
     PROJECT_YAML_FILENAMES,
     CondaProjectYaml,
     EnvironmentYaml,
     yaml,
@@ -127,14 +136,77 @@
                     [("default", [environment_yaml_path.relative_to(self.directory)])]
                 ),
             )
 
         self.condarc = self.directory / ".condarc"
 
     @classmethod
+    def from_archive(
+        cls,
+        fn: Union[Path, str],
+        storage_options: Optional[Dict[str, str]] = None,
+        output_directory: Union[Path, str] = ".",
+    ):
+        """Extra a conda-project archive and load the project"""
+
+        if isinstance(output_directory, str):
+            output_directory = Path(output_directory)
+
+        storage_options = {} if storage_options is None else storage_options
+        protocol, _ = split_protocol(fn)
+        if protocol is not None:
+            options = {protocol: storage_options}
+        else:
+            options = {}
+
+        files = fsspec.open_files(f"libarchive://**::{fn}", **options)
+        archive_name = Path(Path(fn).name.split(".", maxsplit=1)[0])
+
+        first_parts = set(Path(p.path).parts[0] for p in files)
+        if ".." in first_parts:
+            raise CondaProjectError(
+                f"The archive {fn} contains relative paths, which are not allowed."
+            )
+
+        if len(first_parts) == 1:
+            # This looks like a project archive with a directory
+            # at the top level
+            if not output_directory.name:
+                project_directory = Path(list(first_parts)[0])
+            else:
+                project_directory = output_directory
+        else:
+            # This looks like a project archive without a directory
+            # at the top level
+            if not output_directory.name:
+                project_directory = archive_name
+            else:
+                project_directory = output_directory
+
+        for afile in files:
+            with afile as f:
+                if len(first_parts) == 1:
+                    if not output_directory.name:
+                        dest = Path(afile.path)
+                    else:
+                        dest = output_directory / Path(*Path(afile.path).parts[1:])
+                else:
+                    if not output_directory.name:
+                        dest = archive_name / afile.path
+                    else:
+                        dest = output_directory / afile.path
+
+                dest.parents[0].mkdir(parents=True, exist_ok=True)
+                dest.write_bytes(f.read())
+                print(dest, file=sys.stderr)
+
+        project = CondaProject(project_directory)
+        return project
+
+    @classmethod
     def init(
         cls,
         directory: Union[Path, str] = ".",
         name: Optional[str] = None,
         dependencies: Optional[List[str]] = None,
         channels: Optional[List[str]] = None,
         platforms: Optional[List[str]] = None,
@@ -234,16 +306,19 @@
             **{k: (Environment, ...) for k in envs},
             __base__=BaseEnvironments,
         )
         return Environments(**envs)
 
     @property
     def default_environment(self) -> Environment:
-        name = next(iter(self._project_file.environments))
-        return self.environments[name]
+        try:
+            name = next(iter(self._project_file.environments))
+            return self.environments[name]
+        except StopIteration:
+            return None
 
     @property
     def commands(self) -> BaseCommands:
         cmds = OrderedDict()
         for name, cmd in self._project_file.commands.items():
             if isinstance(cmd, str):
                 cmd_args = cmd
@@ -705,37 +780,50 @@
     class Config:
         allow_mutation = False
 
 
 class Command(BaseModel):
     name: str
     cmd: str
-    environment: Environment
+    environment: Optional[Environment] = None
     command_variables: Optional[Dict[str, Optional[str]]] = None
     project: CondaProject
 
-    def run(self, environment=None, extra_args=None, verbose=False) -> NoReturn:
-        if environment is None:
-            environment = self.environment
+    def run(
+        self,
+        environment=None,
+        external_environment=None,
+        extra_args=None,
+        verbose=False,
+    ) -> NoReturn:
+        if external_environment is None and self.environment is None:
+            prefix = conda_prefix()
+        elif external_environment is not None:
+            prefix = conda_prefix(external_environment)
         else:
-            if isinstance(environment, str):
-                environment = self.project.environments[environment]
+            if environment is None:
+                environment = self.environment
+            else:
+                if isinstance(environment, str):
+                    environment = self.project.environments[environment]
+
+            if not environment.is_consistent:
+                environment.install(verbose=verbose)
 
-        if not environment.is_consistent:
-            environment.install(verbose=verbose)
+            prefix = environment.prefix
 
         env = prepare_variables(
             self.project.directory,
             self.project._project_file.variables,
             self.command_variables,
         )
 
         conda_run(
             cmd=self.cmd,
-            prefix=environment.prefix,
+            prefix=prefix,
             working_dir=self.project.directory,
             env=env,
             extra_args=extra_args,
         )
 
     class Config:
         arbitrary_types_allowed = True
```

### Comparing `conda-project-0.1.1/src/conda_project/project_file.py` & `conda-project-0.2.0/src/conda_project/project_file.py`

 * *Files identical despite different names*

### Comparing `conda-project-0.1.1/src/conda_project/utils.py` & `conda-project-0.2.0/src/conda_project/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from collections.abc import Generator
 from contextlib import contextmanager
 from inspect import Traceback
 from pathlib import Path
 from subprocess import Popen
 from typing import Dict, List, NoReturn, Optional, Type, Union
 
+import shellingham
 from dotenv import dotenv_values
 
 from .exceptions import CondaProjectError
 
 
 @contextmanager
 def env_variable(key: str, value: str) -> Generator:
@@ -161,7 +162,23 @@
     else:
         old_dir = Path.cwd()
         try:
             os.chdir(cwd)
             os.execvpe(file, args, env)
         finally:
             os.chdir(old_dir)
+
+
+def detect_shell():
+    try:
+        shell_name, shell_path = shellingham.detect_shell()
+    except shellingham.ShellDetectionFailure:
+        if os.name == "posix":
+            shell_name = shell_path = os.environ.get("SHELL", "/bin/sh")
+        elif os.name == "nt":
+            shell_name = shell_path = os.environ.get("COMSPEC", "cmd.exe")
+        else:
+            raise RuntimeError(
+                "Could not determine an appropriate shell to activate for your OS."
+            )
+
+    return shell_name, shell_path
```

### Comparing `conda-project-0.1.1/src/conda_project.egg-info/PKG-INFO` & `conda-project-0.2.0/src/conda_project.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conda-project
-Version: 0.1.1
+Version: 0.2.0
 Summary: Tool for encapsulating, running, and reproducing projects with conda environments
 Author-email: Albert DeFusco <adefusco@anaconda.com>, Matt Kramer <mkramer@anaconda.com>
 License: BSD-3-Clause
 Project-URL: repository, https://github.com/conda-incubator/conda-project
 Project-URL: homepage, https://github.com/conda-incubator/conda-project
 Project-URL: documentation, https://conda-incubator.github.io/conda-project/user_guide.html
 Project-URL: Issue Tracker, https://github.com/conda-incubator/conda-project/issues
@@ -31,26 +31,38 @@
 # conda-project
 
 [![codecov](https://codecov.io/gh/conda-incubator/conda-project/branch/main/graph/badge.svg?token=XNRS8JKT75)](https://codecov.io/gh/conda-incubator/conda-project)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/conda-incubator/conda-project/main.svg)](https://results.pre-commit.ci/latest/github/conda-incubator/conda-project/main)
 
 Tool for encapsulating, running, and reproducing projects with conda environments.
 
-This package is intended as a successor to [Anaconda Project](https://github.com/Anaconda-Platform/anaconda-project).
 
 ## Why?
 
 Sharing your work is more than sharing your code in a script file or notebook. To make your work properly reproducible, it is necessary to include the list of required third-party dependencies, specifications for how to run your code, and
 any other files that it may need.
 
 See [8 Levels of Reproduciblity](https://www.anaconda.com/blog/8-levels-of-reproducibility) for an in-depth
 discussion of the differences between "It works for me." to "I've made sure that anyone can reliably execute my work."
 Conda Project is a framework that aims to help you to ensure a high degree of reproducibility in the projects you
 create.
 
+### How is this different from Anaconda Project?
+
+This package is intended as a successor to [Anaconda Project](https://github.com/Anaconda-Platform/anaconda-project).
+We chose to create Conda Project to foster community involvement, adopt newer standards like conda-lock, and provide
+a conda-native workflow. A standalone conversion script is provided in this repo at `scripts/ap-to-cp.py`. You can run
+it as follows. By default it will write Conda Project files into your current working directory. You can read anaconda-project.yml file from any other directory or output Conda Project files to any other directory.
+
+You'll need `pydantic` and `ruamel.yaml` installed.
+
+```text
+python ap-to-cp.py /path/to/anaconda-project.yml [/output/directory]
+```
+
 ## Installation
 
 You can install conda-project using the conda package manager:
 
 ```text
 conda install -c conda-forge conda-project
 ```
```

### Comparing `conda-project-0.1.1/src/conda_project.egg-info/SOURCES.txt` & `conda-project-0.2.0/src/conda_project.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 .github/disclaimer.txt
 .github/workflows/docs.yml
 .github/workflows/main.yaml
 conda.recipe/meta.yaml
 docs/Makefile
 docs/requirements.txt
 docs/source/conf.py
+docs/source/experimental.md
 docs/source/index.md
 docs/source/setup_for_development.md
 docs/source/tutorial.md
 docs/source/user_guide.md
 etc/build-environment.yml
 etc/test-environment.yml
 examples/.gitignore
@@ -35,18 +36,20 @@
 examples/multi-env-files/conda-lock.default.yml
 examples/multi-env-files/conda-lock.test.yml
 examples/multi-env-files/conda-project.yml
 examples/multi-env-files/environment.yml
 examples/multi-env-files/extras.yml
 examples/multi-env-files/print_version.py
 examples/multi-env-files/test_get_version.py
+scripts/ap-to-cp.py
 src/conda_project/__init__.py
 src/conda_project/__main__.py
 src/conda_project/_version.py
 src/conda_project/conda.py
+src/conda_project/conda_transfer.py
 src/conda_project/exceptions.py
 src/conda_project/project.py
 src/conda_project/project_file.py
 src/conda_project/utils.py
 src/conda_project.egg-info/PKG-INFO
 src/conda_project.egg-info/SOURCES.txt
 src/conda_project.egg-info/dependency_links.txt
@@ -54,13 +57,18 @@
 src/conda_project.egg-info/requires.txt
 src/conda_project.egg-info/top_level.txt
 src/conda_project/cli/__init__.py
 src/conda_project/cli/commands.py
 src/conda_project/cli/main.py
 tests/__init__.py
 tests/conftest.py
+tests/test_archive.py
 tests/test_cli.py
 tests/test_commands.py
 tests/test_conda.py
 tests/test_project.py
 tests/test_project_file.py
-tests/test_utils.py
+tests/test_utils.py
+tests/assets/no-top-level-dir.tar.gz
+tests/assets/relative-paths.tar.gz
+tests/assets/top-level-dir.tar.gz
+tests/assets/unnamed-top-level-dir.tar.gz
```

### Comparing `conda-project-0.1.1/tests/conftest.py` & `conda-project-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `conda-project-0.1.1/tests/test_cli.py` & `conda-project-0.2.0/tests/test_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) 2022 Anaconda, Inc
 # SPDX-License-Identifier: BSD-3-Clause
+from argparse import Namespace
 from textwrap import dedent
 
 import pytest
 
+from conda_project.cli.commands import _load_project
 from conda_project.cli.main import cli, main, parse_and_run
 from conda_project.project import CondaProject
 
 PROJECT_ACTIONS = ("init", "create", "check")
 ENVIRONMENT_ACTIONS = ("clean", "install", "prepare", "lock", "activate")
 COMMAND_ACTIONS = ("run",)
 ALL_ACTIONS = PROJECT_ACTIONS + ENVIRONMENT_ACTIONS + COMMAND_ACTIONS
@@ -220,27 +222,27 @@
 
 def test_run_default_command(mocker, multi_env_multi_command):
     default_command = mocker.spy(CondaProject, "default_command")
 
     _ = parse_and_run(["run", "--directory", str(multi_env_multi_command)])
 
     assert default_command.run.call_args == mocker.call(
-        environment=None, extra_args=[], verbose=True
+        environment=None, extra_args=[], external_environment=None, verbose=True
     )
 
 
 def test_run_default_command_with_env(mocker, multi_env_multi_command):
     default_command = mocker.spy(CondaProject, "default_command")
 
     _ = parse_and_run(
         ["run", "--directory", str(multi_env_multi_command), "--environment", "env2"]
     )
 
     assert default_command.run.call_args == mocker.call(
-        environment="env2", extra_args=[], verbose=True
+        environment="env2", extra_args=[], external_environment=None, verbose=True
     )
 
 
 def test_run_named_command(mocker, multi_env_multi_command):
     default_command = mocker.spy(CondaProject, "default_command")
     commands = mocker.spy(CondaProject, "commands")
 
@@ -265,15 +267,15 @@
     assert command.call_args == mocker.call(
         name="cmd3",
         cmd="cmd3",
         environment=project.spy_return.default_environment,
         project=project.spy_return,
     )
     assert mocked_run.call_args == mocker.call(
-        environment=None, extra_args=[], verbose=True
+        environment=None, extra_args=[], external_environment=None, verbose=True
     )
 
 
 def test_run_unnamed_command_with_env(mocker, multi_env_multi_command):
     from conda_project.cli import commands as commands_module
 
     command = mocker.spy(commands_module, "Command")
@@ -295,15 +297,15 @@
     assert command.call_args == mocker.call(
         name="cmd3",
         cmd="cmd3",
         environment=project.spy_return.default_environment,
         project=project.spy_return,
     )
     assert mocked_run.call_args == mocker.call(
-        environment="env2", extra_args=[], verbose=True
+        environment="env2", extra_args=[], external_environment=None, verbose=True
     )
 
 
 def test_run_unnamed_command_with_extra_args(mocker, multi_env_multi_command):
     from conda_project.cli import commands as commands_module
 
     command = mocker.spy(commands_module, "Command")
@@ -328,9 +330,51 @@
     assert command.call_args == mocker.call(
         name="cmd3",
         cmd="cmd3",
         environment=project.spy_return.default_environment,
         project=project.spy_return,
     )
     assert mocked_run.call_args == mocker.call(
-        environment="env2", extra_args=["--flag", "value", "arg1"], verbose=True
+        environment="env2",
+        extra_args=["--flag", "value", "arg1"],
+        external_environment=None,
+        verbose=True,
     )
+
+
+@pytest.mark.parametrize("action", ("lock", "check", "install", "activate", "run"))
+def test_cli_archive_arguments(action, mocker, capsys):
+    mocked_action = mocker.patch(
+        f"conda_project.cli.commands.{action}",
+        return_value=42,
+        side_effect=print(f"I am {action}"),
+    )
+
+    ret = parse_and_run(
+        [action, "--project-archive", "project.tar.gz", "--directory", "project-dir"]
+    )
+    assert ret == 42
+
+    assert mocked_action.call_count == 1
+    assert "project_archive" in mocked_action.call_args.args[0]
+    assert "archive_storage_options" in mocked_action.call_args.args[0]
+
+    out, err = capsys.readouterr()
+    assert f"I am {action}\n" == out
+    assert "" == err
+
+
+def test_archive_storage_options_remote(mocker):
+    mocked_project = mocker.patch("conda_project.cli.commands.CondaProject")
+
+    args = Namespace(
+        project_archive="protocol://bucket/file.zip",
+        archive_storage_options="key1=valueA,key2=valueB",
+        directory=None,
+    )
+
+    _ = _load_project(args)
+
+    assert mocked_project.from_archive.call_args.kwargs["storage_options"] == {
+        "key1": "valueA",
+        "key2": "valueB",
+    }
```

### Comparing `conda-project-0.1.1/tests/test_commands.py` & `conda-project-0.2.0/tests/test_commands.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,40 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) 2022 Anaconda, Inc
 # SPDX-License-Identifier: BSD-3-Clause
 import os
+from pathlib import Path
 from textwrap import dedent
 
 import pytest
 
+from conda_project.conda import conda_prefix
 from conda_project.exceptions import CommandNotFoundError
 from conda_project.project import CondaProject
 
 
 @pytest.fixture
+def no_env_one_command(project_directory_factory) -> CondaProject:
+    project_yaml = dedent(
+        """\
+        name: test
+        environments: {}
+        commands:
+          the-command: run-me
+        """
+    )
+
+    project_path = project_directory_factory(
+        project_yaml=project_yaml,
+    )
+    project = CondaProject(project_path)
+    return project
+
+
+@pytest.fixture
 def one_env_no_commands(project_directory_factory) -> CondaProject:
     env_yaml = "dependencies: []\n"
 
     project_yaml = dedent(
         f"""\
         name: test
         environments:
@@ -362,14 +382,62 @@
         prefix=project.default_environment.prefix,
         working_dir=project.directory,
         env=os.environ,
         extra_args=["--flag", "a", "b"],
     )
 
 
+def test_run_with_external_environment(
+    one_env_one_command: CondaProject, mocked_execvped, mocker
+):
+    from conda_project import project as project_module
+
+    conda_run = mocker.spy(project_module, "conda_run")
+
+    project = one_env_one_command
+
+    project.default_command.run(
+        extra_args=["--flag", "a", "b"], external_environment="base"
+    )
+
+    assert mocked_execvped.call_count == 1
+
+    assert conda_run.call_args == mocker.call(
+        cmd="run-me",
+        prefix=conda_prefix("base"),
+        working_dir=project.directory,
+        env=os.environ,
+        extra_args=["--flag", "a", "b"],
+    )
+
+
+def test_run_no_project_environment(
+    no_env_one_command: CondaProject, mocked_execvped, mocker
+):
+    from conda_project import project as project_module
+
+    conda_run = mocker.spy(project_module, "conda_run")
+
+    project = no_env_one_command
+
+    project.default_command.run(
+        extra_args=["--flag", "a", "b"],
+    )
+
+    assert mocked_execvped.call_count == 1
+
+    assert conda_run.call_args == mocker.call(
+        cmd="run-me",
+        prefix=Path(os.environ["CONDA_PREFIX"]),
+        working_dir=project.directory,
+        env=os.environ,
+        extra_args=["--flag", "a", "b"],
+    )
+
+
 def test_activate_prepares_env(one_env_no_commands: CondaProject, mocker):
     mocker.patch("conda_project.project.conda_activate")
 
     project = one_env_no_commands
 
     assert not project.default_environment.is_consistent
```

### Comparing `conda-project-0.1.1/tests/test_conda.py` & `conda-project-0.2.0/tests/test_conda.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 # -*- coding: utf-8 -*-
 # Copyright (C) 2022 Anaconda, Inc
 # SPDX-License-Identifier: BSD-3-Clause
 
+import os
+from pathlib import Path
+
 import pytest
 
 from conda_project.conda import (
     call_conda,
     conda_activate,
     conda_info,
+    conda_prefix,
     conda_run,
     current_platform,
     is_windows,
 )
 from conda_project.exceptions import CondaProjectError
 
 
@@ -122,35 +126,35 @@
     assert mocked_execvped.call_count == 1
 
 
 @pytest.mark.skipif(is_windows(), reason="On Windows we call subprocess")
 def test_conda_activate_pexpect(mocker, empty_conda_environment, capsys):
     mocked_spawn = mocker.patch("conda_project.conda.pexpect.spawn")
     mocker.patch(
-        "conda_project.conda.shellingham.detect_shell",
+        "conda_project.conda.detect_shell",
         return_value=("/bin/sh", "/bin/sh"),
     )
     mocker.patch("conda_project.conda._send_activation")
 
     conda_activate(
         prefix=empty_conda_environment, working_dir=empty_conda_environment, env=None
     )
 
     assert "activated in a new shell" in capsys.readouterr().out
 
     assert mocked_spawn.call_args == mocker.call(
-        command="/bin/sh", args=["-i"], cwd=empty_conda_environment, env={}, echo=False
+        command="/bin/sh", args=["-i"], cwd=empty_conda_environment, env={}, echo=True
     )
 
 
 @pytest.mark.skipif(is_windows(), reason="On Windows we call subprocess")
 def test_conda_activate_pexpect_with_variables(mocker, empty_conda_environment, capsys):
     mocked_spawn = mocker.patch("conda_project.conda.pexpect.spawn")
     mocker.patch(
-        "conda_project.conda.shellingham.detect_shell",
+        "conda_project.conda.detect_shell",
         return_value=("/bin/sh", "/bin/sh"),
     )
     mocker.patch("conda_project.conda._send_activation")
 
     conda_activate(
         prefix=empty_conda_environment,
         working_dir=empty_conda_environment,
@@ -160,9 +164,53 @@
     assert "activated in a new shell" in capsys.readouterr().out
 
     assert mocked_spawn.call_args == mocker.call(
         command="/bin/sh",
         args=["-i"],
         cwd=empty_conda_environment,
         env={"FOO": "set-in-project"},
-        echo=False,
+        echo=True,
     )
+
+
+def test_conda_prefix_with_name(empty_conda_environment: Path, monkeypatch):
+    monkeypatch.setenv("CONDA_ENVS_DIRS", str(empty_conda_environment.parent))
+
+    prefix = conda_prefix(empty_conda_environment.name)
+    assert prefix == empty_conda_environment
+
+
+def test_conda_prefix_root():
+    for env in "root", "base":
+        prefix = conda_prefix(env)
+        assert str(prefix) == os.environ["CONDA_ROOT"]
+
+
+def test_conda_prefix_current_env():
+    prefix = conda_prefix()
+    assert str(prefix) == os.environ["CONDA_PREFIX"]
+
+
+def test_conda_prefix_with_path(empty_conda_environment):
+    prefix = conda_prefix(empty_conda_environment)
+    assert prefix == empty_conda_environment
+
+
+def test_conda_prefix_prefers_path(tmp_path, monkeypatch):
+    monkeypatch.chdir(tmp_path)
+    monkeypatch.setenv("CONDA_ENVS_DIRS", str(tmp_path / "global-envs"))
+
+    create = ["create", "-n", "my-env", "--yes"]
+    _ = call_conda(create)
+    envs = conda_info()["envs"]
+    assert str(tmp_path / "global-envs" / "my-env") in envs
+
+    prefix = conda_prefix("my-env")
+    assert prefix == tmp_path / "global-envs" / "my-env"
+
+    create = ["create", "-p", str(tmp_path / "my-env"), "--yes"]
+    _ = call_conda(create)
+
+    prefix = conda_prefix("my-env")
+    assert prefix == tmp_path / "my-env"
+
+    _ = call_conda(["env", "remove", "-n", "my-env"])
```

### Comparing `conda-project-0.1.1/tests/test_project.py` & `conda-project-0.2.0/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `conda-project-0.1.1/tests/test_project_file.py` & `conda-project-0.2.0/tests/test_project_file.py`

 * *Files identical despite different names*

### Comparing `conda-project-0.1.1/tests/test_utils.py` & `conda-project-0.2.0/tests/test_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # Copyright (C) 2022 Anaconda, Inc
 # SPDX-License-Identifier: BSD-3-Clause
 
 import os
 from pathlib import Path
 
 import pytest
+from shellingham import ShellDetectionFailure
 
 from conda_project.exceptions import CondaProjectError
 from conda_project.utils import (
+    detect_shell,
     env_variable,
     execvped,
     find_file,
     is_windows,
     prepare_variables,
 )
 
@@ -240,7 +242,34 @@
     with pytest.raises(SystemExit) as exinfo:
         execvped(
             file="invalid-cmd", args=["arg1", "arg2"], env={"FOO": "bar"}, cwd=tmp_path
         )
 
     assert exinfo.value.code == 1
     assert mocked_popen.call_args.kwargs["args"] == ["invalid-cmd", "arg1", "arg2"]
+
+
+def test_detect_shell_from_env(mocker, monkeypatch):
+    if is_windows():
+        monkeypatch.setenv("COMSPEC", "/fake/shell")
+    else:
+        monkeypatch.setenv("SHELL", "/fake/shell")
+
+    mocker.patch(
+        "conda_project.utils.shellingham.detect_shell",
+        side_effect=ShellDetectionFailure(),
+    )
+
+    shell_name, shell_path = detect_shell()
+
+    assert shell_name == shell_path == "/fake/shell"
+
+
+def test_detect_shell_failed(mocker):
+    mocker.patch(
+        "conda_project.utils.shellingham.detect_shell",
+        side_effect=ShellDetectionFailure(),
+    )
+    mocker.patch("os.name", return_value="nope")
+
+    with pytest.raises(RuntimeError):
+        _ = detect_shell()
```


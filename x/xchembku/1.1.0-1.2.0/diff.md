# Comparing `tmp/xchembku-1.1.0.tar.gz` & `tmp/xchembku-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xchembku-1.1.0.tar", last modified: Thu Apr 13 08:38:26 2023, max compression
+gzip compressed data, was "xchembku-1.2.0.tar", last modified: Mon Apr 24 09:51:29 2023, max compression
```

## Comparing `xchembku-1.1.0.tar` & `xchembku-1.2.0.tar`

### file list

```diff
@@ -1,146 +1,148 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.715559 xchembku-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.703559 xchembku-1.1.0/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-13 08:38:18.000000 xchembku-1.1.0/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.703559 xchembku-1.1.0/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-13 08:38:18.000000 xchembku-1.1.0/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-13 08:38:18.000000 xchembku-1.1.0/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-13 08:38:18.000000 xchembku-1.1.0/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-13 08:38:18.000000 xchembku-1.1.0/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-13 08:38:18.000000 xchembku-1.1.0/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-13 08:38:18.000000 xchembku-1.1.0/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-13 08:38:18.000000 xchembku-1.1.0/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-13 08:38:18.000000 xchembku-1.1.0/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.707559 xchembku-1.1.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-13 08:38:18.000000 xchembku-1.1.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-04-13 08:38:18.000000 xchembku-1.1.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.707559 xchembku-1.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-13 08:38:18.000000 xchembku-1.1.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.703559 xchembku-1.1.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.707559 xchembku-1.1.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-13 08:38:18.000000 xchembku-1.1.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-13 08:38:18.000000 xchembku-1.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.707559 xchembku-1.1.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-13 08:38:18.000000 xchembku-1.1.0/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-13 08:38:18.000000 xchembku-1.1.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.707559 xchembku-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-04-13 08:38:18.000000 xchembku-1.1.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-13 08:38:18.000000 xchembku-1.1.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-13 08:38:18.000000 xchembku-1.1.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-13 08:38:18.000000 xchembku-1.1.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-13 08:38:18.000000 xchembku-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-13 08:38:18.000000 xchembku-1.1.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-13 08:38:18.000000 xchembku-1.1.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.707559 xchembku-1.1.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-13 08:38:18.000000 xchembku-1.1.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-13 08:38:18.000000 xchembku-1.1.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-13 08:38:18.000000 xchembku-1.1.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-13 08:38:18.000000 xchembku-1.1.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-13 08:38:18.000000 xchembku-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-04-13 08:38:26.715559 xchembku-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-13 08:38:18.000000 xchembku-1.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.707559 xchembku-1.1.0/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-13 08:38:18.000000 xchembku-1.1.0/configurations/development.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.707559 xchembku-1.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.703559 xchembku-1.1.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.707559 xchembku-1.1.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-13 08:38:18.000000 xchembku-1.1.0/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-04-13 08:38:18.000000 xchembku-1.1.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.707559 xchembku-1.1.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-04-13 08:38:18.000000 xchembku-1.1.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-13 08:38:18.000000 xchembku-1.1.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-13 08:38:18.000000 xchembku-1.1.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.707559 xchembku-1.1.0/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.707559 xchembku-1.1.0/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-13 08:38:18.000000 xchembku-1.1.0/docs/user/explanations/22-developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-13 08:38:18.000000 xchembku-1.1.0/docs/user/explanations/23-testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-13 08:38:18.000000 xchembku-1.1.0/docs/user/explanations/24-devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-13 08:38:18.000000 xchembku-1.1.0/docs/user/explanations/25-docs-structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.707559 xchembku-1.1.0/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-13 08:38:18.000000 xchembku-1.1.0/docs/user/how-to/01-installing_development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-13 08:38:18.000000 xchembku-1.1.0/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.707559 xchembku-1.1.0/docs/user/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.707559 xchembku-1.1.0/docs/user/reference/api/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-13 08:38:18.000000 xchembku-1.1.0/docs/user/reference/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-13 08:38:18.000000 xchembku-1.1.0/docs/user/reference/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-13 08:38:18.000000 xchembku-1.1.0/docs/user/reference/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-13 08:38:18.000000 xchembku-1.1.0/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.707559 xchembku-1.1.0/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-13 08:38:18.000000 xchembku-1.1.0/docs/user/tutorials/tbd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-04-13 08:38:18.000000 xchembku-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 08:38:26.715559 xchembku-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.703559 xchembku-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.711559 xchembku-1.1.0/src/xchembku.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-04-13 08:38:26.000000 xchembku-1.1.0/src/xchembku.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-13 08:38:26.000000 xchembku-1.1.0/src/xchembku.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:38:26.000000 xchembku-1.1.0/src/xchembku.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 08:38:26.000000 xchembku-1.1.0/src/xchembku.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-13 08:38:26.000000 xchembku-1.1.0/src/xchembku.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-13 08:38:26.000000 xchembku-1.1.0/src/xchembku.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.711559 xchembku-1.1.0/src/xchembku_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_api/aiohttp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_api/context_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.711559 xchembku-1.1.0/src/xchembku_api/databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_api/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_api/databases/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.711559 xchembku-1.1.0/src/xchembku_api/datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_api/datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10461 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_api/datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_api/datafaces/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_api/datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_api/datafaces/datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.711559 xchembku-1.1.0/src/xchembku_api/models/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_api/models/crystal_plate_filter_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_api/models/crystal_plate_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_api/models/crystal_well_autolocation_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_api/models/crystal_well_droplocation_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_api/models/crystal_well_filter_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_api/models/crystal_well_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_api/models/crystal_well_needing_droplocation_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.711559 xchembku-1.1.0/src/xchembku_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.711559 xchembku-1.1.0/src/xchembku_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_cli/subcommands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.711559 xchembku-1.1.0/src/xchembku_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 08:38:26.000000 xchembku-1.1.0/src/xchembku_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.715559 xchembku-1.1.0/src/xchembku_lib/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/contexts/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.715559 xchembku-1.1.0/src/xchembku_lib/databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/databases/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/databases/database_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/databases/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/databases/normsql.py
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/databases/table_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.715559 xchembku-1.1.0/src/xchembku_lib/datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/datafaces/datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/datafaces/direct.py
--rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/datafaces/direct_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/datafaces/direct_crystal_plates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/datafaces/direct_crystal_well_autolocations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/datafaces/direct_crystal_well_droplocations.py
--rw-r--r--   0 runner    (1001) docker     (123)    11637 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/datafaces/direct_crystal_wells.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/envvar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-13 08:38:18.000000 xchembku-1.1.0/src/xchembku_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.715559 xchembku-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:18.000000 xchembku-1.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-13 08:38:18.000000 xchembku-1.1.0/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:38:26.715559 xchembku-1.1.0/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-13 08:38:18.000000 xchembku-1.1.0/tests/configurations/direct.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-13 08:38:18.000000 xchembku-1.1.0/tests/configurations/service.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-04-13 08:38:18.000000 xchembku-1.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-04-13 08:38:18.000000 xchembku-1.1.0/tests/test_crystal_plate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-04-13 08:38:18.000000 xchembku-1.1.0/tests/test_crystal_well_autolocation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12133 2023-04-13 08:38:18.000000 xchembku-1.1.0/tests/test_crystal_well_droplocation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.750962 xchembku-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.734961 xchembku-1.2.0/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-24 09:51:15.000000 xchembku-1.2.0/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.738961 xchembku-1.2.0/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-24 09:51:15.000000 xchembku-1.2.0/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-24 09:51:15.000000 xchembku-1.2.0/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-24 09:51:15.000000 xchembku-1.2.0/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-24 09:51:15.000000 xchembku-1.2.0/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-24 09:51:15.000000 xchembku-1.2.0/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-24 09:51:15.000000 xchembku-1.2.0/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-24 09:51:15.000000 xchembku-1.2.0/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-24 09:51:15.000000 xchembku-1.2.0/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.738961 xchembku-1.2.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-24 09:51:15.000000 xchembku-1.2.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-04-24 09:51:15.000000 xchembku-1.2.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.738961 xchembku-1.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-24 09:51:15.000000 xchembku-1.2.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.730960 xchembku-1.2.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.738961 xchembku-1.2.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-24 09:51:15.000000 xchembku-1.2.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-24 09:51:15.000000 xchembku-1.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.738961 xchembku-1.2.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-24 09:51:15.000000 xchembku-1.2.0/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-24 09:51:15.000000 xchembku-1.2.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.738961 xchembku-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-04-24 09:51:15.000000 xchembku-1.2.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-24 09:51:15.000000 xchembku-1.2.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-24 09:51:15.000000 xchembku-1.2.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-24 09:51:15.000000 xchembku-1.2.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-24 09:51:15.000000 xchembku-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-24 09:51:15.000000 xchembku-1.2.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-24 09:51:15.000000 xchembku-1.2.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.738961 xchembku-1.2.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-24 09:51:15.000000 xchembku-1.2.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-24 09:51:15.000000 xchembku-1.2.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-24 09:51:15.000000 xchembku-1.2.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-24 09:51:15.000000 xchembku-1.2.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-24 09:51:15.000000 xchembku-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-04-24 09:51:29.750962 xchembku-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-24 09:51:15.000000 xchembku-1.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.738961 xchembku-1.2.0/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-24 09:51:15.000000 xchembku-1.2.0/configurations/development.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.738961 xchembku-1.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.730960 xchembku-1.2.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.738961 xchembku-1.2.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-24 09:51:15.000000 xchembku-1.2.0/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-04-24 09:51:15.000000 xchembku-1.2.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.738961 xchembku-1.2.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-04-24 09:51:15.000000 xchembku-1.2.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-24 09:51:15.000000 xchembku-1.2.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-24 09:51:15.000000 xchembku-1.2.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.738961 xchembku-1.2.0/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.742961 xchembku-1.2.0/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-24 09:51:15.000000 xchembku-1.2.0/docs/user/explanations/22-developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-24 09:51:15.000000 xchembku-1.2.0/docs/user/explanations/23-testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-24 09:51:15.000000 xchembku-1.2.0/docs/user/explanations/24-devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-24 09:51:15.000000 xchembku-1.2.0/docs/user/explanations/25-docs-structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.742961 xchembku-1.2.0/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-24 09:51:15.000000 xchembku-1.2.0/docs/user/how-to/01-installing_development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-24 09:51:15.000000 xchembku-1.2.0/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.742961 xchembku-1.2.0/docs/user/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.742961 xchembku-1.2.0/docs/user/reference/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-24 09:51:15.000000 xchembku-1.2.0/docs/user/reference/api/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-24 09:51:15.000000 xchembku-1.2.0/docs/user/reference/api/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-24 09:51:15.000000 xchembku-1.2.0/docs/user/reference/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-24 09:51:15.000000 xchembku-1.2.0/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.742961 xchembku-1.2.0/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-24 09:51:15.000000 xchembku-1.2.0/docs/user/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-24 09:51:15.000000 xchembku-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 09:51:29.750962 xchembku-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.734961 xchembku-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.742961 xchembku-1.2.0/src/xchembku.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-04-24 09:51:29.000000 xchembku-1.2.0/src/xchembku.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-04-24 09:51:29.000000 xchembku-1.2.0/src/xchembku.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 09:51:29.000000 xchembku-1.2.0/src/xchembku.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-24 09:51:29.000000 xchembku-1.2.0/src/xchembku.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-24 09:51:29.000000 xchembku-1.2.0/src/xchembku.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-24 09:51:29.000000 xchembku-1.2.0/src/xchembku.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.742961 xchembku-1.2.0/src/xchembku_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_api/aiohttp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_api/context_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.742961 xchembku-1.2.0/src/xchembku_api/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_api/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_api/databases/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.742961 xchembku-1.2.0/src/xchembku_api/datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_api/datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11768 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_api/datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_api/datafaces/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_api/datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_api/datafaces/datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.746961 xchembku-1.2.0/src/xchembku_api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_api/models/crystal_plate_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_api/models/crystal_plate_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_api/models/crystal_well_autolocation_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_api/models/crystal_well_droplocation_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_api/models/crystal_well_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_api/models/crystal_well_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_api/models/crystal_well_needing_droplocation_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.746961 xchembku-1.2.0/src/xchembku_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.746961 xchembku-1.2.0/src/xchembku_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_cli/subcommands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.746961 xchembku-1.2.0/src/xchembku_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 09:51:29.000000 xchembku-1.2.0/src/xchembku_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.746961 xchembku-1.2.0/src/xchembku_lib/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/contexts/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.746961 xchembku-1.2.0/src/xchembku_lib/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/databases/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/databases/database_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/databases/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/databases/normsql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/databases/table_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.750962 xchembku-1.2.0/src/xchembku_lib/datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/datafaces/datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/datafaces/direct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/datafaces/direct_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/datafaces/direct_crystal_plates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/datafaces/direct_crystal_well_autolocations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/datafaces/direct_crystal_well_droplocations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11445 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/datafaces/direct_crystal_wells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/datafaces/direct_soakdb3_crystal_wells.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/envvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-24 09:51:15.000000 xchembku-1.2.0/src/xchembku_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.750962 xchembku-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:15.000000 xchembku-1.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-24 09:51:15.000000 xchembku-1.2.0/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:51:29.750962 xchembku-1.2.0/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-24 09:51:15.000000 xchembku-1.2.0/tests/configurations/direct.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-04-24 09:51:15.000000 xchembku-1.2.0/tests/configurations/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-04-24 09:51:15.000000 xchembku-1.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-04-24 09:51:15.000000 xchembku-1.2.0/tests/test_crystal_plate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-04-24 09:51:15.000000 xchembku-1.2.0/tests/test_crystal_well_autolocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-04-24 09:51:15.000000 xchembku-1.2.0/tests/test_crystal_well_droplocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10145 2023-04-24 09:51:15.000000 xchembku-1.2.0/tests/test_soakdb3_crystal_well.py
```

### Comparing `xchembku-1.1.0/.dae-devops/Makefile` & `xchembku-1.2.0/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/.dae-devops/docs/conventions.rst` & `xchembku-1.2.0/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/.dae-devops/docs/developing.rst` & `xchembku-1.2.0/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/.dae-devops/docs/devops.rst` & `xchembku-1.2.0/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/.dae-devops/docs/docs_structure.rst` & `xchembku-1.2.0/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/.dae-devops/docs/installing.rst` & `xchembku-1.2.0/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/.dae-devops/docs/testing.rst` & `xchembku-1.2.0/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/.dae-devops/project.yaml` & `xchembku-1.2.0/.dae-devops/project.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -14,8 +14,9 @@
     dependencies:
         - type: pypi
           list:
               - dls_servbase
               - dls_mainiac
               - dls_multiconf
               - dls_utilpack
+              - soakdb3
               - pydantic
```

### Comparing `xchembku-1.1.0/.devcontainer/Dockerfile` & `xchembku-1.2.0/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/.devcontainer/devcontainer.json` & `xchembku-1.2.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/.github/CONTRIBUTING.rst` & `xchembku-1.2.0/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/.github/actions/install_requirements/action.yml` & `xchembku-1.2.0/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/.github/dependabot.yml` & `xchembku-1.2.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/.github/pages/make_switcher.py` & `xchembku-1.2.0/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/.github/workflows/code.yml` & `xchembku-1.2.0/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/.github/workflows/docs.yml` & `xchembku-1.2.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/.github/workflows/docs_clean.yml` & `xchembku-1.2.0/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/.github/workflows/linkcheck.yml` & `xchembku-1.2.0/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/.gitignore` & `xchembku-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/.gitlab-ci.yml` & `xchembku-1.2.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/.vscode/launch.json` & `xchembku-1.2.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/LICENSE` & `xchembku-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/PKG-INFO` & `xchembku-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchembku
-Version: 1.1.0
+Version: 1.2.0
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `xchembku-1.1.0/README.rst` & `xchembku-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/configurations/development.yaml` & `xchembku-1.2.0/configurations/development.yaml`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/docs/conf.py` & `xchembku-1.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/docs/images/dls-favicon.ico` & `xchembku-1.2.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/docs/images/dls-logo.svg` & `xchembku-1.2.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/docs/index.rst` & `xchembku-1.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/docs/user/explanations/25-docs-structure.rst` & `xchembku-1.2.0/docs/user/explanations/25-docs-structure.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/docs/user/index.rst` & `xchembku-1.2.0/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/pyproject.toml` & `xchembku-1.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 description = "XChem Business Knowledge Unit. Service, Client, API, persistent store."
-dependencies = ["dls_servbase", "dls_mainiac", "dls_multiconf", "dls_utilpack", "pydantic"]
+dependencies = ["dls_servbase", "dls_mainiac", "dls_multiconf", "dls_utilpack", "soakdb3", "pydantic"]
 dynamic = ["version"]
 license.file = "LICENSE"
 readme = "README.rst"
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = [
@@ -99,8 +99,8 @@
 source = ["src", "**/site-packages/"]
 
 # tox must currently be configured via an embedded ini string
 # See: https://github.com/tox-dev/tox/issues/999
 [tool.tox]
 legacy_tox_ini = "[tox]\nskipsdist=True\n\n[testenv:{pre-commit,mypy,pytest,docs}]\n# Don't create a virtualenv for the command, requires tox-direct plugin\ndirect = True\npassenv = *\nallowlist_externals = \n    pytest \n    pre-commit\n    mypy\n    sphinx-build\n    sphinx-autobuild\ncommands =\n    pytest: pytest {posargs}\n    mypy: mypy src tests {posargs}\n    pre-commit: pre-commit run --all-files {posargs}\n    docs: sphinx-{posargs:build -EW --keep-going} -T docs build/html\n"
 
-# dae_devops_fingerprint 2a6e4e14bc8b0cf0ba4ae9fe98e89ae9
+# dae_devops_fingerprint 18b9ab431706150f1fba1a06f8fdb1c4
```

### Comparing `xchembku-1.1.0/src/xchembku.egg-info/PKG-INFO` & `xchembku-1.2.0/src/xchembku.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchembku
-Version: 1.1.0
+Version: 1.2.0
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `xchembku-1.1.0/src/xchembku.egg-info/SOURCES.txt` & `xchembku-1.2.0/src/xchembku.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -95,15 +95,17 @@
 src/xchembku_lib/datafaces/datafaces.py
 src/xchembku_lib/datafaces/direct.py
 src/xchembku_lib/datafaces/direct_base.py
 src/xchembku_lib/datafaces/direct_crystal_plates.py
 src/xchembku_lib/datafaces/direct_crystal_well_autolocations.py
 src/xchembku_lib/datafaces/direct_crystal_well_droplocations.py
 src/xchembku_lib/datafaces/direct_crystal_wells.py
+src/xchembku_lib/datafaces/direct_soakdb3_crystal_wells.py
 tests/__init__.py
 tests/base.py
 tests/conftest.py
 tests/test_crystal_plate.py
 tests/test_crystal_well_autolocation.py
 tests/test_crystal_well_droplocation.py
+tests/test_soakdb3_crystal_well.py
 tests/configurations/direct.yaml
 tests/configurations/service.yaml
```

### Comparing `xchembku-1.1.0/src/xchembku_api/context_base.py` & `xchembku-1.2.0/src/xchembku_api/context_base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/src/xchembku_api/datafaces/aiohttp.py` & `xchembku-1.2.0/src/xchembku_api/datafaces/aiohttp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import logging
 from typing import Dict, List, Optional
 
 from dls_utilpack.callsign import callsign
+from soakdb3_api.models.crystal_well_model import (
+    CrystalWellModel as Soakdb3CrystalWellModel,
+)
 
 # Class for an aiohttp client.
 from xchembku_api.aiohttp_client import AiohttpClient
 
 # Dataface protocolj things.
 from xchembku_api.datafaces.constants import Commands, Keywords
 from xchembku_api.models.crystal_plate_filter_model import CrystalPlateFilterModel
@@ -78,15 +81,15 @@
             why=why,
         )
 
     # ----------------------------------------------------------------------------------------
     async def upsert_crystal_plates(
         self,
         models: List[CrystalPlateModel],
-        why=None,
+        why: Optional[str] = None,
     ) -> None:
         """"""
 
         records: List[Dict] = [model.dict() for model in models]
         await self.__send_protocolj(
             "upsert_crystal_plates_serialized",
             records,
@@ -228,27 +231,62 @@
 
         return None
 
     # ----------------------------------------------------------------------------------------
     async def upsert_crystal_well_droplocations(
         self,
         models: List[CrystalWellDroplocationModel],
-        why=None,
+        only_fields: Optional[List[str]] = None,
+        why: Optional[str] = None,
     ) -> None:
         """"""
 
         records: List[Dict] = [model.dict() for model in models]
         await self.__send_protocolj(
             "upsert_crystal_well_droplocations_serialized",
             records,
+            only_fields=only_fields,
+            why=why,
         )
 
         return None
 
     # ----------------------------------------------------------------------------------------
+    async def inject_soakdb3_crystal_wells(
+        self,
+        visitid: str,
+        models: List[Soakdb3CrystalWellModel],
+        why: Optional[str] = None,
+    ) -> Dict:
+        """"""
+
+        records: List[Dict] = [model.dict() for model in models]
+        result = await self.__send_protocolj(
+            "inject_soakdb3_crystal_wells_serialized", visitid, records, why=why
+        )
+        return result
+
+    # ----------------------------------------------------------------------------------------
+    async def fetch_soakdb3_crystal_wells(
+        self,
+        visitid: str,
+        why: Optional[str] = None,
+    ) -> List[Soakdb3CrystalWellModel]:
+        """"""
+
+        records = await self.__send_protocolj(
+            "fetch_soakdb3_crystal_wells_serialized", visitid, why=why
+        )
+
+        # Dicts are returned, so parse them into models.
+        models = [Soakdb3CrystalWellModel(**record) for record in records]
+
+        return models
+
+    # ----------------------------------------------------------------------------------------
     async def report_health(self):
         """"""
         return await self.__send_protocolj("report_health")
 
     # ----------------------------------------------------------------------------------------
     async def set_cookie(self, cookie_dict):
         """ """
```

### Comparing `xchembku-1.1.0/src/xchembku_api/datafaces/context.py` & `xchembku-1.2.0/src/xchembku_api/datafaces/context.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/src/xchembku_api/datafaces/datafaces.py` & `xchembku-1.2.0/src/xchembku_api/datafaces/datafaces.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/src/xchembku_api/exceptions.py` & `xchembku-1.2.0/src/xchembku_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/src/xchembku_api/models/crystal_plate_model.py` & `xchembku-1.2.0/src/xchembku_api/models/crystal_plate_model.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/src/xchembku_api/models/crystal_well_autolocation_model.py` & `xchembku-1.2.0/src/xchembku_api/models/crystal_well_autolocation_model.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/src/xchembku_api/models/crystal_well_droplocation_model.py` & `xchembku-1.2.0/src/xchembku_api/models/crystal_well_droplocation_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     Typically this structure is populated and transmitted by the chimpflow.
     """
 
     uuid: str
     crystal_well_uuid: Optional[str] = None
     confirmed_target_x: Optional[int] = None
     confirmed_target_y: Optional[int] = None
+    is_usable: Optional[bool] = None
 
     # TODO: Add proper pydantic date parsing/valiation to CREATED_ON fields.
     created_on: Optional[str] = None
 
     def __init__(self, **kwargs):
         # Automatically cook up a uuid if it's not provided to the constructor.
         if "uuid" not in kwargs:
```

### Comparing `xchembku-1.1.0/src/xchembku_api/models/crystal_well_model.py` & `xchembku-1.2.0/src/xchembku_api/models/crystal_well_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,20 @@
     # This is the well's position on the plate, such as A01_1, A01_2, etc.
     # TODO: Enforce crystal_well.position unique among wells in plate.
     position: str
 
     # This is the filename containing the well's image.
     filename: str
 
+    # This is the size of the well's image.
+    # Optional for now to avoid having to refactor all tests to include it on the constructur.
+    # TODO: Make crystal_well_model width and height not optional.
+    width: Optional[int] = None
+    height: Optional[int] = None
+
     # This is the error reading and parsing the image file, if any.
     error: Optional[str]
 
     # TODO: Add proper pydantic date parsing/valiation to CREATED_ON fields.
     created_on: Optional[str] = None
 
     def __init__(self, **kwargs):
```

### Comparing `xchembku-1.1.0/src/xchembku_cli/main.py` & `xchembku-1.2.0/src/xchembku_cli/main.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/src/xchembku_cli/subcommands/base.py` & `xchembku-1.2.0/src/xchembku_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/src/xchembku_cli/subcommands/service.py` & `xchembku-1.2.0/src/xchembku_cli/subcommands/service.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/src/xchembku_cli/version.py` & `xchembku-1.2.0/src/xchembku_cli/version.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/src/xchembku_lib/__main__.py` & `xchembku-1.2.0/src/xchembku_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/src/xchembku_lib/contexts/base.py` & `xchembku-1.2.0/src/xchembku_lib/contexts/base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/src/xchembku_lib/databases/database_definition.py` & `xchembku-1.2.0/src/xchembku_lib/databases/database_definition.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/src/xchembku_lib/databases/databases.py` & `xchembku-1.2.0/src/xchembku_lib/databases/databases.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/src/xchembku_lib/databases/normsql.py` & `xchembku-1.2.0/src/xchembku_lib/databases/normsql.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/src/xchembku_lib/databases/table_definitions.py` & `xchembku-1.2.0/src/xchembku_lib/databases/table_definitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,8 +166,9 @@
                 elif field_type == bool:
                     sql_type = "BOOLEAN"
 
                 self.fields[field_name] = {"type": sql_type}
 
         # Add indexes.
         self.fields["crystal_well_uuid"]["index"] = True
+        self.fields["is_usable"]["index"] = True
         self.fields[CommonFieldnames.CREATED_ON]["index"] = True
```

### Comparing `xchembku-1.1.0/src/xchembku_lib/datafaces/aiohttp.py` & `xchembku-1.2.0/src/xchembku_lib/datafaces/aiohttp.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/src/xchembku_lib/datafaces/context.py` & `xchembku-1.2.0/src/xchembku_lib/datafaces/context.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/src/xchembku_lib/datafaces/datafaces.py` & `xchembku-1.2.0/src/xchembku_lib/datafaces/datafaces.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/src/xchembku_lib/datafaces/direct.py` & `xchembku-1.2.0/src/xchembku_lib/datafaces/direct.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,23 +5,27 @@
 from xchembku_lib.datafaces.direct_crystal_well_autolocations import (
     DirectCrystalWellAutolocations,
 )
 from xchembku_lib.datafaces.direct_crystal_well_droplocations import (
     DirectCrystalWellDroplocations,
 )
 from xchembku_lib.datafaces.direct_crystal_wells import DirectCrystalWells
+from xchembku_lib.datafaces.direct_soakdb3_crystal_wells import (
+    DirectSoakdb3CrystalWells,
+)
 
 logger = logging.getLogger(__name__)
 
 
 class Direct(
     DirectCrystalPlates,
     DirectCrystalWells,
     DirectCrystalWellAutolocations,
     DirectCrystalWellDroplocations,
+    DirectSoakdb3CrystalWells,
     DirectBase,
 ):
     """ """
 
     # ----------------------------------------------------------------------------------------
     def __init__(self, specification=None):
         DirectBase.__init__(self, specification)
```

### Comparing `xchembku-1.1.0/src/xchembku_lib/datafaces/direct_base.py` & `xchembku-1.2.0/src/xchembku_lib/datafaces/direct_base.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,14 +33,17 @@
     async def disconnect(self):
         if self.__database is not None:
             logger.debug(f"{callsign(self)} disconnecting")
             await self.__database.disconnect()
             logger.debug(f"{callsign(self)} disconnected")
             self.__database = None
 
+        # TODO: Figure out a better way to disconnect the dataface mixins.
+        await self.disconnect_soakdb3_crystal_wells_mixin()
+
     # ----------------------------------------------------------------------------------------
     async def establish_database_connection(self):
         if self.__database is None:
             self.__database = Databases().build_object(self.specification()["database"])
             await self.__database.connect()
 
     # ----------------------------------------------------------------------------------------
```

### Comparing `xchembku-1.1.0/src/xchembku_lib/datafaces/direct_crystal_plates.py` & `xchembku-1.2.0/src/xchembku_lib/datafaces/direct_crystal_plates.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/src/xchembku_lib/datafaces/direct_crystal_well_autolocations.py` & `xchembku-1.2.0/src/xchembku_lib/datafaces/direct_crystal_well_autolocations.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/src/xchembku_lib/datafaces/direct_crystal_wells.py` & `xchembku-1.2.0/src/xchembku_lib/datafaces/direct_crystal_wells.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import copy
 import logging
-from typing import Dict, List
+from typing import Any, Dict, List
 
 from dls_normsql.constants import CommonFieldnames
 from dls_utilpack.describe import describe
 
 from xchembku_api.models.crystal_well_filter_model import CrystalWellFilterModel
 from xchembku_api.models.crystal_well_model import CrystalWellModel
 from xchembku_api.models.crystal_well_needing_droplocation_model import (
@@ -177,15 +177,15 @@
     async def fetch_crystal_wells_needing_droplocation(
         self, filter: CrystalWellFilterModel, why=None
     ) -> List[CrystalWellNeedingDroplocationModel]:
         """
         Wells need a droplocation if they have an autolocation but no droplocation.
         """
 
-        subs = []
+        subs: List[Any] = []
 
         created_on = CommonFieldnames.CREATED_ON
 
         where = "WHERE"
 
         if why is None:
             why = "API fetch_crystal_wells_needing_droplocation"
@@ -196,14 +196,17 @@
             "\n  crystal_well_autolocations.auto_target_y,"
             "\n  crystal_well_autolocations.well_centroid_x,"
             "\n  crystal_well_autolocations.well_centroid_y,"
             "\n  crystal_well_autolocations.drop_detected,"
             "\n  crystal_well_autolocations.number_of_crystals,"
             "\n  crystal_well_droplocations.confirmed_target_x,"
             "\n  crystal_well_droplocations.confirmed_target_y,"
+            "\n  (crystal_well_droplocations.confirmed_target_x - crystal_well_autolocations.well_centroid_x) AS echo_coordinate_x,"
+            "\n  (crystal_well_droplocations.confirmed_target_y - crystal_well_autolocations.well_centroid_y) AS echo_coordinate_y,"
+            "\n  crystal_well_droplocations.is_usable,"
             "\n  crystal_plates.visit"
             "\nFROM crystal_wells"
             "\nJOIN crystal_well_autolocations ON crystal_well_autolocations.crystal_well_uuid = crystal_wells.uuid"
             "\nLEFT JOIN crystal_well_droplocations ON crystal_well_droplocations.crystal_well_uuid = crystal_wells.uuid"
             "\nLEFT JOIN crystal_plates ON crystal_plates.uuid = crystal_wells.crystal_plate_uuid"
         )
 
@@ -215,61 +218,53 @@
             )
             subs.append(filter.filename_pattern)
             where = "AND"
 
         # Caller wants specific barcode?
         if filter.barcode is not None:
             query += (
-                "\n/* Just a wells on plates with a certain barcode. */"
+                f"\n/* Just a wells on plates with barcode '{filter.barcode}'. */"
                 f"\n{where} crystal_plates.barcode = ?"
             )
             subs.append(filter.barcode)
             where = "AND"
 
         # Caller wants specific visit?
         if filter.visit is not None:
             query += (
-                "\n/* Just a wells on plates with a certain visit. */"
+                f"\n/* Just a wells on plates with visit '{filter.visit}'. */"
                 f"\n{where} crystal_plates.visit = ?"
             )
             subs.append(filter.visit)
             where = "AND"
 
-        # Caller wants only those not yet confirmed?
-        if filter.is_confirmed is False:
+        # Caller wants only those not yet decided?
+        if filter.is_decided is False:
             query += (
-                "\n/* Exclude crystal wells which already have confirmed drop locations. */"
-                f"\n{where} crystal_wells.uuid NOT IN (SELECT crystal_well_uuid FROM crystal_well_droplocations)"
+                "\n/* Include only crystal wells which have not had a decision made. */"
+                f"\n{where} crystal_well_droplocations.is_usable IS NULL"
             )
             where = "AND"
 
-        # Caller wants only those which are confirmed?
+        # Caller wants only those which are decided?
         # Confirmed means a droplocation record has been created at all (though might not have usable coordinates).
-        if filter.is_confirmed is True:
+        if filter.is_decided is True:
             query += (
-                "\n/* Include only crystal wells which already have confirmed drop locations. */"
-                f"\n{where} crystal_wells.uuid IN (SELECT crystal_well_uuid FROM crystal_well_droplocations)"
+                "\n/* Include only crystal wells which have a decision made. */"
+                f"\n{where} crystal_well_droplocations.is_usable IS NOT NULL"
             )
             where = "AND"
 
-        # Caller wants only those which are confirmed but do not have usable coordinates?
-        usable_sql = "SELECT crystal_well_uuid FROM crystal_well_droplocations WHERE confirmed_target_x IS NOT NULL AND confirmed_target_y IS NOT NULL"
-        if filter.is_usable is False:
+        # Caller wants only those which are decided but do or don't have usable coordinates?
+        if filter.is_usable is not None:
             query += (
-                "\n/* Include only crystal wells which DO NOT have drop locations with usable coordinates. */"
-                f"\n{where} crystal_wells.uuid NOT IN ({usable_sql})"
-            )
-            where = "AND"
-
-        # Caller wants only those which are confirmed to have usable coordinates?
-        if filter.is_usable is True:
-            query += (
-                "\n/* Include only crystal wells which have drop locations with usable coordinates. */"
-                f"\n{where} crystal_wells.uuid IN ({usable_sql})"
+                f"\n/* Include only crystal wells which have filter.is_usable = {filter.is_usable}. */"
+                f"\n{where} crystal_well_droplocations.is_usable = ?"
             )
+            subs.append(filter.is_usable)
             where = "AND"
 
         # Caller wants results relative to anchor?
         if filter.anchor is not None:
             # Caller wants the anchor itself?
             if filter.direction is None:
                 query += (
@@ -278,15 +273,15 @@
                 )
             # Not the anchor itself, but either side of the anchor?
             else:
                 op = ">"
                 if filter.direction == -1:
                     op = "<"
                 query += (
-                    "\n/* Get the crystal well(s) starting from the anchor. */"
+                    f"\n/* Get the crystal well(s) starting from the anchor {filter.anchor}. */"
                     f"\n{where} crystal_wells.created_on {op} (SELECT {created_on} FROM crystal_wells WHERE uuid = ?)"
                 )
             subs.append(filter.anchor)
 
         sql_direction = "ASC"
         if filter.direction == -1:
             sql_direction = "DESC"
```

### Comparing `xchembku-1.1.0/src/xchembku_lib/version.py` & `xchembku-1.2.0/src/xchembku_lib/version.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/tests/base.py` & `xchembku-1.2.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/tests/configurations/service.yaml` & `xchembku-1.2.0/tests/configurations/service.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -20,18 +20,53 @@
         host: 172.23.7.128
         port: 12201
         protocol: UDP
 
 # The external access bits.
 external_access_bits:
     dataface_port: &DATAFACE_PORT 27821
+    soakdb3_dataface_server: &SOAKDB3_DATAFACE_SERVER http://*:27824
+    soakdb3_dataface_client: &SOAKDB3_DATAFACE_CLIENT http://localhost:27824
 
+# -----------------------------------------------------------------------------
+# The soakdb3 dataface via direct.
+soakdb3_dataface_specification_direct: &SOAKDB3_DATAFACE_SPECIFICATION_DIRECT
+    type: "soakdb3_lib.datafaces.aiosqlite"
+    type_specific_tbd:
+        visitid_mappings:
+            - action: "regex_replace"
+              pattern: "^[Cc][:]"
+              replace: ""
+            - action: "regex_replace"
+              pattern: "^[Yy][:]"
+              replace: "/dls/labxchem/"
+        database:
+            type: "soakdb3_lib.databases.aiosqlite"
+            filename: "set by code"
+            backup_directory: "set by code"
+            log_level: "WARNING"
+
+# The soakdb3 dataface via networked service.
+soakdb3_dataface_specification: &SOAKDB3_DATAFACE_SPECIFICATION
+    type: "soakdb3_lib.datafaces.aiohttp"
+    type_specific_tbd:
+        # The remote dataface server access.
+        aiohttp_specification:
+            server: *SOAKDB3_DATAFACE_SERVER
+            client: *SOAKDB3_DATAFACE_CLIENT
+        # The local implementation of the dataface.
+        actual_dataface_specification: *SOAKDB3_DATAFACE_SPECIFICATION_DIRECT
+    context:
+        start_as: process
+
+# -----------------------------------------------------------------------------
 # The xchembku_dataface direct access.
 xchembku_dataface_specification_direct: &XCHEMBKU_DATAFACE_SPECIFICATION_DIRECT
     type: "xchembku_lib.xchembku_datafaces.direct"
+    soakdb3_dataface_specification: *SOAKDB3_DATAFACE_SPECIFICATION
     database:
         type: "xchembku_lib.xchembku_databases.normsql"
         filename: "${output_directory}/xchembku_dataface.sqlite"
         log_level: "WARNING"
 
 # The xchembku_dataface client/server composite.
 xchembku_dataface_specification: &XCHEMBKU_DATAFACE_SPECIFICATION
```

### Comparing `xchembku-1.1.0/tests/conftest.py` & `xchembku-1.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/tests/test_crystal_plate.py` & `xchembku-1.2.0/tests/test_crystal_plate.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/tests/test_crystal_well_autolocation.py` & `xchembku-1.2.0/tests/test_crystal_well_autolocation.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.1.0/tests/test_crystal_well_droplocation.py` & `xchembku-1.2.0/tests/test_crystal_well_droplocation.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,30 +145,30 @@
         await self.__check(
             dataface, CrystalWellFilterModel(), 5, "no limit, all after upsert"
         )
 
         await self.__check(dataface, CrystalWellFilterModel(limit=1), 1, "limit 1")
         await self.__check(dataface, CrystalWellFilterModel(limit=2), 2, "limit 2")
         await self.__check(
-            dataface, CrystalWellFilterModel(is_confirmed=True), 3, "confirmed only"
+            dataface, CrystalWellFilterModel(is_decided=True), 3, "confirmed only"
         )
         await self.__check(
             dataface,
-            CrystalWellFilterModel(barcode=self.__barcode, is_confirmed=True),
+            CrystalWellFilterModel(barcode=self.__barcode, is_decided=True),
             3,
             "confirmed only, barcode",
         )
         await self.__check(
             dataface,
-            CrystalWellFilterModel(barcode="abcd", is_confirmed=True),
+            CrystalWellFilterModel(barcode="abcd", is_decided=True),
             0,
             "confirmed only, other barcode",
         )
         await self.__check(
-            dataface, CrystalWellFilterModel(is_confirmed=False), 2, "unconfirmed only"
+            dataface, CrystalWellFilterModel(is_decided=False), 2, "unconfirmed only"
         )
 
         # Check the anchor query forward.
         await self.__check(
             dataface,
             CrystalWellFilterModel(anchor=models[3].uuid, direction=1, limit=1),
             1,
@@ -201,25 +201,25 @@
             "anchored at the start of the list",
         )
 
         # Check the anchor query backward at the start of the list of those unconfirmed.
         await self.__check(
             dataface,
             CrystalWellFilterModel(
-                is_confirmed=False, anchor=models[1].uuid, direction=-1
+                is_decided=False, anchor=models[1].uuid, direction=-1
             ),
             0,
             "anchored at the start of the list, backward, unconfirmed",
         )
 
         # Check the anchor query backward at the start of the list of those unconfirmed.
         await self.__check(
             dataface,
             CrystalWellFilterModel(
-                is_confirmed=False, anchor=models[2].uuid, direction=-1
+                is_decided=False, anchor=models[2].uuid, direction=-1
             ),
             0,
             "anchored at the start of the list, forward unconfirmed",
         )
 
         # Query for list from filename glob.
         crystal_well_models = await self.__check(
@@ -233,17 +233,17 @@
         assert crystal_well_models[1].filename == "002a.jpg"
         assert crystal_well_models[2].filename == "003a.jpg"
 
         # --------------------------------------------------------------------------
         # Check the usable queries.
         await self.__check(
             dataface,
-            CrystalWellFilterModel(is_confirmed=True, is_usable=False),
+            CrystalWellFilterModel(is_decided=True, is_usable=False),
             0,
-            "confirmed but unusable only",
+            "confirmed but unusable only (1)",
         )
         crystal_well_models = await self.__check(
             dataface,
             CrystalWellFilterModel(
                 visit=self.__visit,
                 is_usable=True,
             ),
@@ -260,30 +260,29 @@
             3,
             "usable only, barcode",
         )
 
         # Change one of the usable to unusable.
         t = CrystalWellDroplocationModel(
             crystal_well_uuid=crystal_well_models[0].uuid,
-            confirmed_target_x=None,
-            confirmed_target_y=None,
+            is_usable=False,
         )
 
         await dataface.upsert_crystal_well_droplocations([t])
 
         # Check the usable queries again.
         await self.__check(
             dataface,
             CrystalWellFilterModel(
                 visit=self.__visit,
-                is_confirmed=True,
+                is_decided=True,
                 is_usable=False,
             ),
             1,
-            "confirmed but unusable only",
+            "confirmed but unusable only (2)",
         )
         crystal_well_models = await self.__check(
             dataface,
             CrystalWellFilterModel(is_usable=True),
             2,
             "usable only after upsert",
         )
@@ -321,14 +320,15 @@
 
         if droplocation:
             # Add a crystal well droplocation.
             td = CrystalWellDroplocationModel(
                 crystal_well_uuid=m.uuid,
                 confirmed_target_x=10,
                 confirmed_target_y=11,
+                is_usable=True,
             )
 
             await dataface.upsert_crystal_well_droplocations([td])
 
         return m
 
     # ----------------------------------------------------------------------------------------
```


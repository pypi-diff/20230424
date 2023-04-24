# Comparing `tmp/lightning-app-2.0.1.post0.tar.gz` & `tmp/lightning-app-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-app-2.0.1.post0.tar", last modified: Tue Apr 11 18:44:10 2023, max compression
+gzip compressed data, was "lightning-app-2.0.2.tar", last modified: Mon Apr 24 13:57:18 2023, max compression
```

## Comparing `lightning-app-2.0.1.post0.tar` & `lightning-app-2.0.2.tar`

### file list

```diff
@@ -1,366 +1,366 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.575530 lightning-app-2.0.1.post0/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.547529 lightning-app-2.0.1.post0/.actions/
--rw-r--r--   0 runner    (1001) docker     (122)    17395 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/.actions/assistant.py
--rw-r--r--   0 runner    (1001) docker     (122)    11349 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    11142 2023-04-11 18:44:10.575530 lightning-app-2.0.1.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    22128 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     7219 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.539529 lightning-app-2.0.1.post0/requirements/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.547529 lightning-app-2.0.1.post0/requirements/app/
--rw-r--r--   0 runner    (1001) docker     (122)      652 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/requirements/app/base.txt
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/requirements/app/cloud.txt
--rw-r--r--   0 runner    (1001) docker     (122)      244 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/requirements/app/components.txt
--rw-r--r--   0 runner    (1001) docker     (122)      307 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/requirements/app/devel.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/requirements/app/docs.txt
--rw-r--r--   0 runner    (1001) docker     (122)      228 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/requirements/app/test.txt
--rw-r--r--   0 runner    (1001) docker     (122)       51 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/requirements/app/ui.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 18:44:10.575530 lightning-app-2.0.1.post0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     7917 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.547529 lightning-app-2.0.1.post0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.547529 lightning-app-2.0.1.post0/src/lightning_app/
--rw-r--r--   0 runner    (1001) docker     (122)    32714 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)      431 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/src/lightning_app/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9717 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/src/lightning_app/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/src/lightning_app/__about__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       88 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/src/lightning_app/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4826 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/src/lightning_app/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (122)      355 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/src/lightning_app/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.547529 lightning-app-2.0.1.post0/src/lightning_app/api/
--rw-r--r--   0 runner    (1001) docker     (122)      129 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8700 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/api/http_methods.py
--rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/api/request_types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.551529 lightning-app-2.0.1.post0/src/lightning_app/cli/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.551529 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/
--rw-r--r--   0 runner    (1001) docker     (122)     2087 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      802 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      365 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.551529 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/placeholdername/
--rw-r--r--   0 runner    (1001) docker     (122)      164 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/placeholdername/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.543529 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/placeholdername/components/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.551529 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/placeholdername/components/component_a/
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/placeholdername/components/component_a/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      122 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/placeholdername/components/component_a/component_a.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.551529 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/placeholdername/components/component_b/
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/placeholdername/components/component_b/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      122 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/placeholdername/components/component_b/component_a.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      415 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.551529 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      196 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       96 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/tests/test_placeholdername_app.py
--rw-r--r--   0 runner    (1001) docker     (122)     6148 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/cmd_apps.py
--rw-r--r--   0 runner    (1001) docker     (122)    16500 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/cmd_clusters.py
--rw-r--r--   0 runner    (1001) docker     (122)     5298 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/cmd_init.py
--rw-r--r--   0 runner    (1001) docker     (122)    21746 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/cmd_install.py
--rw-r--r--   0 runner    (1001) docker     (122)     6723 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/cmd_pl_init.py
--rw-r--r--   0 runner    (1001) docker     (122)     4382 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/cmd_react_ui_init.py
--rw-r--r--   0 runner    (1001) docker     (122)     2560 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/cmd_ssh_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.551529 lightning-app-2.0.1.post0/src/lightning_app/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5043 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/commands/app_commands.py
--rw-r--r--   0 runner    (1001) docker     (122)     3972 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/commands/cd.py
--rw-r--r--   0 runner    (1001) docker     (122)    12620 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/commands/cp.py
--rw-r--r--   0 runner    (1001) docker     (122)     4327 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/commands/logs.py
--rw-r--r--   0 runner    (1001) docker     (122)     9547 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/commands/ls.py
--rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/commands/pwd.py
--rw-r--r--   0 runner    (1001) docker     (122)     3738 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/commands/rm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.551529 lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.543529 lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.551529 lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2327 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/.github/workflows/ci-testing.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2087 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      863 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.551529 lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/placeholdername/
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/placeholdername/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      291 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/placeholdername/component.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      433 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.551529 lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      202 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       96 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      258 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/tests/test_placeholdername_component.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.551529 lightning-app-2.0.1.post0/src/lightning_app/cli/connect/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14456 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/connect/app.py
--rw-r--r--   0 runner    (1001) docker     (122)     3922 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/connect/data.py
--rw-r--r--   0 runner    (1001) docker     (122)    10662 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/connect/maverick.py
--rw-r--r--   0 runner    (1001) docker     (122)      790 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/core.py
--rw-r--r--   0 runner    (1001) docker     (122)    20545 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/lightning_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     4221 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/lightning_cli_create.py
--rw-r--r--   0 runner    (1001) docker     (122)     8947 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/lightning_cli_delete.py
--rw-r--r--   0 runner    (1001) docker     (122)     1662 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/lightning_cli_list.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.551529 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/.lightningignore
--rw-r--r--   0 runner    (1001) docker     (122)     4262 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.555529 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/core/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13108 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/core/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.555529 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/core/components/
--rw-r--r--   0 runner    (1001) docker     (122)      158 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/core/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.555529 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/core/components/logger/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/core/components/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/core/components/logger/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (122)      972 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/core/components/logger/weights_and_biases.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.555529 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/core/components/script_runner/
--rw-r--r--   0 runner    (1001) docker     (122)       83 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/core/components/script_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3193 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/core/components/script_runner/script_runner.py
--rw-r--r--   0 runner    (1001) docker     (122)     1183 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/core/state.py
--rw-r--r--   0 runner    (1001) docker     (122)      959 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.555529 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.555529 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/tests/core/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2519 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/tests/core/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (122)      331 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/tests/test_app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.555529 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/
--rw-r--r--   0 runner    (1001) docker     (122)      309 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (122)      529 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/.prettierrc
--rw-r--r--   0 runner    (1001) docker     (122)      696 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/craco.config.js
--rw-r--r--   0 runner    (1001) docker     (122)     2549 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/package.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.555529 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/public/
--rw-r--r--   0 runner    (1001) docker     (122)     2112 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/public/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (122)     2705 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/public/index.html
--rw-r--r--   0 runner    (1001) docker     (122)      318 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/public/manifest.json
--rw-r--r--   0 runner    (1001) docker     (122)       67 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/public/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.555529 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/
--rw-r--r--   0 runner    (1001) docker     (122)     4364 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/App.tsx
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.555529 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/components/
--rw-r--r--   0 runner    (1001) docker     (122)     1717 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/components/EnvironmentConfigurator.tsx
--rw-r--r--   0 runner    (1001) docker     (122)      809 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/components/ErrorPanel.tsx
--rw-r--r--   0 runner    (1001) docker     (122)     2829 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/components/ExecutionSummary.tsx
--rw-r--r--   0 runner    (1001) docker     (122)     3205 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/components/HyperparameterSummary.tsx
--rw-r--r--   0 runner    (1001) docker     (122)     5647 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/components/Launcher.tsx
--rw-r--r--   0 runner    (1001) docker     (122)     1275 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBar.tsx
--rw-r--r--   0 runner    (1001) docker     (122)     1528 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBarGroup.tsx
--rw-r--r--   0 runner    (1001) docker     (122)      823 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/components/Timer.tsx
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.555529 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/hooks/
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/hooks/useLightningState.ts
--rw-r--r--   0 runner    (1001) docker     (122)      452 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/index.css
--rw-r--r--   0 runner    (1001) docker     (122)      865 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/index.tsx
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/lightning-colors.ts
--rw-r--r--   0 runner    (1001) docker     (122)       40 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/react-app-env.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      425 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/reportWebVitals.ts
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.555529 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/types/
--rw-r--r--   0 runner    (1001) docker     (122)      988 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/types/lightning.ts
--rw-r--r--   0 runner    (1001) docker     (122)      547 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/tsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.555529 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/
--rw-r--r--   0 runner    (1001) docker     (122)     2453 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      840 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/example_app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.559529 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/
--rw-r--r--   0 runner    (1001) docker     (122)      475 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/index.html
--rw-r--r--   0 runner    (1001) docker     (122)      713 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/package.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.559529 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/src/
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/src/App.css
--rw-r--r--   0 runner    (1001) docker     (122)     2032 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/src/App.tsx
--rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/src/favicon.svg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.559529 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/src/hooks/
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/src/hooks/useLightningState.ts
--rw-r--r--   0 runner    (1001) docker     (122)      366 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/src/index.css
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/src/main.tsx
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.559529 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/src/types/
--rw-r--r--   0 runner    (1001) docker     (122)      988 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/src/types/lightning.ts
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/src/vite-env.d.ts
--rw-r--r--   0 runner    (1001) docker     (122)      560 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (122)      142 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/tsconfig.node.json
--rw-r--r--   0 runner    (1001) docker     (122)      310 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/vite.config.ts
--rw-r--r--   0 runner    (1001) docker     (122)    55270 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/yarn.lock
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.559529 lightning-app-2.0.1.post0/src/lightning_app/components/
--rw-r--r--   0 runner    (1001) docker     (122)     1430 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.559529 lightning-app-2.0.1.post0/src/lightning_app/components/database/
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3169 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/database/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     8480 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/database/server.py
--rw-r--r--   0 runner    (1001) docker     (122)     9225 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/database/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.559529 lightning-app-2.0.1.post0/src/lightning_app/components/multi_node/
--rw-r--r--   0 runner    (1001) docker     (122)      398 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/multi_node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3928 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/multi_node/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     4657 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/multi_node/fabric.py
--rw-r--r--   0 runner    (1001) docker     (122)     4160 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/multi_node/pytorch_spawn.py
--rw-r--r--   0 runner    (1001) docker     (122)     4741 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/multi_node/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.559529 lightning-app-2.0.1.post0/src/lightning_app/components/python/
--rw-r--r--   0 runner    (1001) docker     (122)      193 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3944 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/python/popen.py
--rw-r--r--   0 runner    (1001) docker     (122)     7397 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/python/tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.559529 lightning-app-2.0.1.post0/src/lightning_app/components/serve/
--rw-r--r--   0 runner    (1001) docker     (122)      550 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    30252 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/serve/auto_scaler.py
--rw-r--r--   0 runner    (1001) docker     (122)    20105 2023-04-11 18:44:07.000000 lightning-app-2.0.1.post0/src/lightning_app/components/serve/catimage.png
--rw-r--r--   0 runner    (1001) docker     (122)     2853 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/serve/cold_start_proxy.py
--rw-r--r--   0 runner    (1001) docker     (122)     2927 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/serve/gradio_server.py
--rw-r--r--   0 runner    (1001) docker     (122)    11367 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/serve/python_server.py
--rw-r--r--   0 runner    (1001) docker     (122)     5939 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/serve/serve.py
--rw-r--r--   0 runner    (1001) docker     (122)     5609 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/serve/streamlit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.559529 lightning-app-2.0.1.post0/src/lightning_app/components/serve/types/
--rw-r--r--   0 runner    (1001) docker     (122)      148 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/serve/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1514 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/serve/types/image.py
--rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/serve/types/type.py
--rw-r--r--   0 runner    (1001) docker     (122)     7244 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/components/training.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.559529 lightning-app-2.0.1.post0/src/lightning_app/core/
--rw-r--r--   0 runner    (1001) docker     (122)      210 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18413 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/core/api.py
--rw-r--r--   0 runner    (1001) docker     (122)    30187 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/core/app.py
--rw-r--r--   0 runner    (1001) docker     (122)     5538 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    32850 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/core/flow.py
--rw-r--r--   0 runner    (1001) docker     (122)    18071 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/core/queues.py
--rw-r--r--   0 runner    (1001) docker     (122)    30759 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/core/work.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.563529 lightning-app-2.0.1.post0/src/lightning_app/frontend/
--rw-r--r--   0 runner    (1001) docker     (122)      432 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2309 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/frontend/frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.563529 lightning-app-2.0.1.post0/src/lightning_app/frontend/just_py/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/frontend/just_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3951 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/frontend/just_py/just_py.py
--rw-r--r--   0 runner    (1001) docker     (122)     2075 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/frontend/just_py/just_py_base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.563529 lightning-app-2.0.1.post0/src/lightning_app/frontend/panel/
--rw-r--r--   0 runner    (1001) docker     (122)      310 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/frontend/panel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3288 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/frontend/panel/app_state_comm.py
--rw-r--r--   0 runner    (1001) docker     (122)     3965 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/frontend/panel/app_state_watcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     6300 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/frontend/panel/panel_frontend.py
--rw-r--r--   0 runner    (1001) docker     (122)     2156 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/frontend/panel/panel_serve_render_fn.py
--rw-r--r--   0 runner    (1001) docker     (122)     4161 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/frontend/stream_lit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1774 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/frontend/streamlit_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2528 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/frontend/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5127 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/frontend/web.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.563529 lightning-app-2.0.1.post0/src/lightning_app/perf/
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/perf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1488 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/perf/pdb.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.563529 lightning-app-2.0.1.post0/src/lightning_app/plugin/
--rw-r--r--   0 runner    (1001) docker     (122)      259 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2149 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/plugin/actions.py
--rw-r--r--   0 runner    (1001) docker     (122)     6605 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/plugin/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.563529 lightning-app-2.0.1.post0/src/lightning_app/runners/
--rw-r--r--   0 runner    (1001) docker     (122)      453 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/runners/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.563529 lightning-app-2.0.1.post0/src/lightning_app/runners/backends/
--rw-r--r--   0 runner    (1001) docker     (122)     1004 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/runners/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5218 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/runners/backends/backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     1754 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/runners/backends/cloud.py
--rw-r--r--   0 runner    (1001) docker     (122)     1380 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/runners/backends/docker.py
--rw-r--r--   0 runner    (1001) docker     (122)     5290 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/runners/backends/mp_process.py
--rw-r--r--   0 runner    (1001) docker     (122)    45888 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/runners/cloud.py
--rw-r--r--   0 runner    (1001) docker     (122)     6431 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/runners/multiprocess.py
--rw-r--r--   0 runner    (1001) docker     (122)     7239 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/runners/runtime.py
--rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/runners/runtime_type.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.563529 lightning-app-2.0.1.post0/src/lightning_app/source_code/
--rw-r--r--   0 runner    (1001) docker     (122)      184 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/source_code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6861 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/source_code/copytree.py
--rw-r--r--   0 runner    (1001) docker     (122)     1774 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/source_code/hashing.py
--rw-r--r--   0 runner    (1001) docker     (122)     5530 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/source_code/local.py
--rw-r--r--   0 runner    (1001) docker     (122)     6044 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/source_code/tar.py
--rw-r--r--   0 runner    (1001) docker     (122)     3889 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/source_code/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.563529 lightning-app-2.0.1.post0/src/lightning_app/storage/
--rw-r--r--   0 runner    (1001) docker     (122)      393 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6124 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/storage/copier.py
--rw-r--r--   0 runner    (1001) docker     (122)    13153 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/storage/drive.py
--rw-r--r--   0 runner    (1001) docker     (122)     6071 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/storage/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (122)     2938 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/storage/mount.py
--rw-r--r--   0 runner    (1001) docker     (122)     9419 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/storage/orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (122)    18598 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/storage/path.py
--rw-r--r--   0 runner    (1001) docker     (122)    10959 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/storage/payload.py
--rw-r--r--   0 runner    (1001) docker     (122)     1286 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/storage/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.567530 lightning-app-2.0.1.post0/src/lightning_app/structures/
--rw-r--r--   0 runner    (1001) docker     (122)      122 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6132 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/structures/dict.py
--rw-r--r--   0 runner    (1001) docker     (122)     6680 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/structures/list.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.567530 lightning-app-2.0.1.post0/src/lightning_app/testing/
--rw-r--r--   0 runner    (1001) docker     (122)      448 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/testing/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     5222 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/testing/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)    18595 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/testing/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.567530 lightning-app-2.0.1.post0/src/lightning_app/ui/
--rw-r--r--   0 runner    (1001) docker     (122)     1501 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (122)      747 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/index.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.567530 lightning-app-2.0.1.post0/src/lightning_app/ui/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.567530 lightning-app-2.0.1.post0/src/lightning_app/ui/static/css/
--rw-r--r--   0 runner    (1001) docker     (122)     1326 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/css/main.bb0f092c.css
--rw-r--r--   0 runner    (1001) docker     (122)     2015 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/css/main.bb0f092c.css.map
--rw-r--r--   0 runner    (1001) docker     (122)    15086 2022-12-09 18:23:41.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.567530 lightning-app-2.0.1.post0/src/lightning_app/ui/static/js/
--rw-r--r--   0 runner    (1001) docker     (122)     4605 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/js/787.418637a8.chunk.js
--rw-r--r--   0 runner    (1001) docker     (122)    10281 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/js/787.418637a8.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (122)   349883 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/js/main.2b242b99.js
--rw-r--r--   0 runner    (1001) docker     (122)     2144 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/js/main.2b242b99.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)  1343802 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/js/main.2b242b99.js.map
--rw-r--r--   0 runner    (1001) docker     (122)      571 2022-12-09 18:23:41.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/lightningState.js
--rw-r--r--   0 runner    (1001) docker     (122)      299 2022-12-09 18:23:41.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/manifest.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.571529 lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/
--rw-r--r--   0 runner    (1001) docker     (122)    21692 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/UCity-Light.30446c15a21bf8a994e8.woff2
--rw-r--r--   0 runner    (1001) docker     (122)    29124 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/UCity-Light.47cf3e33cb6bb1496c95.woff
--rw-r--r--   0 runner    (1001) docker     (122)    29800 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/UCity-Regular.7a3b475525ed92dc7816.woff
--rw-r--r--   0 runner    (1001) docker     (122)    22408 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/UCity-Regular.8afa44ac39706d62b62b.woff2
--rw-r--r--   0 runner    (1001) docker     (122)    21108 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/UCity-Semibold.80655a0e8b4bb5f30545.woff2
--rw-r--r--   0 runner    (1001) docker     (122)    28356 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/UCity-Semibold.bb7aab96e378ebd6a651.woff
--rw-r--r--   0 runner    (1001) docker     (122)      498 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/error.11892047d0183a4723b91dc0fb98cb95.svg
--rw-r--r--   0 runner    (1001) docker     (122)     7931 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/lightning-logo-with-text.b964c8fbf221c97eb8ce52bb6e3a30d6.svg
--rw-r--r--   0 runner    (1001) docker     (122)      390 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/success.5edae4c5b171e2c1c5a3c54273c47ba8.svg
--rw-r--r--   0 runner    (1001) docker     (122)     1066 2022-12-09 18:23:58.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/warning.5c542673e84e77ceb6a230bfea7f7263.svg
--rw-r--r--   0 runner    (1001) docker     (122)       67 2022-12-09 18:23:41.000000 lightning-app-2.0.1.post0/src/lightning_app/ui/static/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.575530 lightning-app-2.0.1.post0/src/lightning_app/utilities/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4615 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/app_commands.py
--rw-r--r--   0 runner    (1001) docker     (122)    20581 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/app_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     4455 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/app_logs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1433 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/app_status.py
--rw-r--r--   0 runner    (1001) docker     (122)     2044 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)    13389 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/cli_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2182 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/cloud.py
--rw-r--r--   0 runner    (1001) docker     (122)     4752 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/cluster_logs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1915 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/clusters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.575530 lightning-app-2.0.1.post0/src/lightning_app/utilities/commands/
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11147 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/commands/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     5398 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/component.py
--rw-r--r--   0 runner    (1001) docker     (122)     1572 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (122)     1009 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/dependency_caching.py
--rw-r--r--   0 runner    (1001) docker     (122)     2355 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/enum.py
--rw-r--r--   0 runner    (1001) docker     (122)     3391 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3310 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/frontend.py
--rw-r--r--   0 runner    (1001) docker     (122)     3227 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/git.py
--rw-r--r--   0 runner    (1001) docker     (122)     3980 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/imports.py
--rw-r--r--   0 runner    (1001) docker     (122)    11533 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/introspection.py
--rw-r--r--   0 runner    (1001) docker     (122)     8994 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/layout.py
--rw-r--r--   0 runner    (1001) docker     (122)    10765 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/load_app.py
--rw-r--r--   0 runner    (1001) docker     (122)      873 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (122)     1692 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/log_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     7924 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/login.py
--rw-r--r--   0 runner    (1001) docker     (122)     6202 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/logs_socket_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    60241 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/name_generator.py
--rw-r--r--   0 runner    (1001) docker     (122)    10409 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/network.py
--rw-r--r--   0 runner    (1001) docker     (122)     2707 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/openapi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.575530 lightning-app-2.0.1.post0/src/lightning_app/utilities/packaging/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/packaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2675 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/packaging/app_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     7851 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/packaging/build_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     6691 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/packaging/cloud_compute.py
--rw-r--r--   0 runner    (1001) docker     (122)     4667 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/packaging/docker.py
--rw-r--r--   0 runner    (1001) docker     (122)     7826 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/packaging/lightning_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1809 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/packaging/tarfile.py
--rw-r--r--   0 runner    (1001) docker     (122)     5960 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/port.py
--rw-r--r--   0 runner    (1001) docker     (122)    30463 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/proxies.py
--rw-r--r--   0 runner    (1001) docker     (122)     1222 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/redis.py
--rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/safe_pickle.py
--rw-r--r--   0 runner    (1001) docker     (122)     2413 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (122)     1501 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/secrets.py
--rw-r--r--   0 runner    (1001) docker     (122)    11877 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/state.py
--rw-r--r--   0 runner    (1001) docker     (122)     6667 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/tracer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3094 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/tree.py
--rw-r--r--   0 runner    (1001) docker     (122)      979 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/types.py
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-04-11 18:44:09.000000 lightning-app-2.0.1.post0/src/lightning_app/utilities/warnings.py
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/src/lightning_app/version.info
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 18:44:10.547529 lightning-app-2.0.1.post0/src/lightning_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    11142 2023-04-11 18:44:10.000000 lightning-app-2.0.1.post0/src/lightning_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    14208 2023-04-11 18:44:10.000000 lightning-app-2.0.1.post0/src/lightning_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 18:44:10.000000 lightning-app-2.0.1.post0/src/lightning_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-04-11 18:44:10.000000 lightning-app-2.0.1.post0/src/lightning_app.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 18:44:10.000000 lightning-app-2.0.1.post0/src/lightning_app.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)     1773 2023-04-11 18:44:10.000000 lightning-app-2.0.1.post0/src/lightning_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-04-11 18:44:10.000000 lightning-app-2.0.1.post0/src/lightning_app.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-11 18:43:57.000000 lightning-app-2.0.1.post0/src/version.info
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.955029 lightning-app-2.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.883029 lightning-app-2.0.2/.actions/
+-rw-r--r--   0 runner    (1001) docker     (123)    17395 2023-04-24 13:57:07.000000 lightning-app-2.0.2/.actions/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-04-24 13:57:07.000000 lightning-app-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-04-24 13:57:18.955029 lightning-app-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22128 2023-04-24 13:57:07.000000 lightning-app-2.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-04-24 13:57:07.000000 lightning-app-2.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.875028 lightning-app-2.0.2/requirements/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.887029 lightning-app-2.0.2/requirements/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-24 13:57:07.000000 lightning-app-2.0.2/requirements/app/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-24 13:57:07.000000 lightning-app-2.0.2/requirements/app/cloud.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-24 13:57:07.000000 lightning-app-2.0.2/requirements/app/components.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-24 13:57:07.000000 lightning-app-2.0.2/requirements/app/devel.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-24 13:57:07.000000 lightning-app-2.0.2/requirements/app/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-24 13:57:07.000000 lightning-app-2.0.2/requirements/app/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-24 13:57:07.000000 lightning-app-2.0.2/requirements/app/ui.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 13:57:18.955029 lightning-app-2.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7917 2023-04-24 13:57:07.000000 lightning-app-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.887029 lightning-app-2.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.887029 lightning-app-2.0.2/src/lightning_app/
+-rw-r--r--   0 runner    (1001) docker     (123)    32912 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-24 13:57:07.000000 lightning-app-2.0.2/src/lightning_app/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-04-24 13:57:07.000000 lightning-app-2.0.2/src/lightning_app/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-24 13:57:07.000000 lightning-app-2.0.2/src/lightning_app/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-24 13:57:07.000000 lightning-app-2.0.2/src/lightning_app/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-04-24 13:57:07.000000 lightning-app-2.0.2/src/lightning_app/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-24 13:57:07.000000 lightning-app-2.0.2/src/lightning_app/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.891029 lightning-app-2.0.2/src/lightning_app/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/api/http_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/api/request_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.895029 lightning-app-2.0.2/src/lightning_app/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.895029 lightning-app-2.0.2/src/lightning_app/cli/app-template/
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/app-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/app-template/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/app-template/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/app-template/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.895029 lightning-app-2.0.2/src/lightning_app/cli/app-template/placeholdername/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/app-template/placeholdername/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.875028 lightning-app-2.0.2/src/lightning_app/cli/app-template/placeholdername/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.895029 lightning-app-2.0.2/src/lightning_app/cli/app-template/placeholdername/components/component_a/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/app-template/placeholdername/components/component_a/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/app-template/placeholdername/components/component_a/component_a.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.895029 lightning-app-2.0.2/src/lightning_app/cli/app-template/placeholdername/components/component_b/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/app-template/placeholdername/components/component_b/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/app-template/placeholdername/components/component_b/component_a.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/app-template/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/app-template/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.899029 lightning-app-2.0.2/src/lightning_app/cli/app-template/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/app-template/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/app-template/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/app-template/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/app-template/tests/test_placeholdername_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/cmd_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16500 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/cmd_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/cmd_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21746 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/cmd_install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/cmd_pl_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/cmd_react_ui_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/cmd_ssh_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.899029 lightning-app-2.0.2/src/lightning_app/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/commands/app_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/commands/cd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12620 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/commands/cp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/commands/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/commands/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/commands/pwd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/commands/rm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.899029 lightning-app-2.0.2/src/lightning_app/cli/component-template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.875028 lightning-app-2.0.2/src/lightning_app/cli/component-template/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.899029 lightning-app-2.0.2/src/lightning_app/cli/component-template/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/component-template/.github/workflows/ci-testing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/component-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/component-template/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/component-template/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/component-template/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.903029 lightning-app-2.0.2/src/lightning_app/cli/component-template/placeholdername/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/component-template/placeholdername/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/component-template/placeholdername/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/component-template/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/component-template/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.903029 lightning-app-2.0.2/src/lightning_app/cli/component-template/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/component-template/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/component-template/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/component-template/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/component-template/tests/test_placeholdername_component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.903029 lightning-app-2.0.2/src/lightning_app/cli/connect/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14401 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/connect/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/connect/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10662 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/connect/maverick.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20545 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/lightning_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/lightning_cli_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/lightning_cli_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/lightning_cli_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.903029 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/.lightningignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.903029 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/core/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.907029 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/core/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/core/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.907029 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/core/components/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/core/components/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/core/components/logger/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/core/components/logger/weights_and_biases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.907029 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/core/components/script_runner/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/core/components/script_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/core/components/script_runner/script_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/core/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.907029 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.907029 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/tests/core/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/tests/test_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.907029 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/.prettierrc
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/craco.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.911029 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/public/
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/public/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/public/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/public/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/public/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.911029 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/App.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.915029 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/components/EnvironmentConfigurator.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/components/ErrorPanel.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/components/ExecutionSummary.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/components/HyperparameterSummary.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/components/Launcher.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBar.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBarGroup.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/components/Timer.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.915029 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/hooks/useLightningState.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/index.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/lightning-colors.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/react-app-env.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/reportWebVitals.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.915029 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/types/lightning.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.915029 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/example_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.915029 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.919029 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/src/App.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/src/App.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/src/favicon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.919029 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/src/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/src/hooks/useLightningState.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/src/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/src/main.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.919029 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/src/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/src/types/lightning.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/src/vite-env.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/tsconfig.node.json
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/vite.config.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    55270 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.919029 lightning-app-2.0.2/src/lightning_app/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.919029 lightning-app-2.0.2/src/lightning_app/components/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/database/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/database/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9225 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/database/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.919029 lightning-app-2.0.2/src/lightning_app/components/multi_node/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/multi_node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/multi_node/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/multi_node/fabric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/multi_node/pytorch_spawn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/multi_node/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.923029 lightning-app-2.0.2/src/lightning_app/components/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/python/popen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/python/tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.923029 lightning-app-2.0.2/src/lightning_app/components/serve/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30254 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/serve/auto_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20105 2023-04-24 13:57:16.000000 lightning-app-2.0.2/src/lightning_app/components/serve/catimage.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/serve/cold_start_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/serve/gradio_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/serve/python_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/serve/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/serve/streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.923029 lightning-app-2.0.2/src/lightning_app/components/serve/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/serve/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/serve/types/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/serve/types/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/components/training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.927029 lightning-app-2.0.2/src/lightning_app/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18413 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/core/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29740 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/core/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32847 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/core/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18582 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/core/queues.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30754 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/core/work.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.927029 lightning-app-2.0.2/src/lightning_app/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/frontend/frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.927029 lightning-app-2.0.2/src/lightning_app/frontend/just_py/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/frontend/just_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/frontend/just_py/just_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/frontend/just_py/just_py_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.927029 lightning-app-2.0.2/src/lightning_app/frontend/panel/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/frontend/panel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/frontend/panel/app_state_comm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/frontend/panel/app_state_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/frontend/panel/panel_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/frontend/panel/panel_serve_render_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/frontend/stream_lit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/frontend/streamlit_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/frontend/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/frontend/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.931029 lightning-app-2.0.2/src/lightning_app/perf/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/perf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/perf/pdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.931029 lightning-app-2.0.2/src/lightning_app/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/plugin/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/plugin/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.931029 lightning-app-2.0.2/src/lightning_app/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/runners/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.931029 lightning-app-2.0.2/src/lightning_app/runners/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/runners/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/runners/backends/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/runners/backends/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/runners/backends/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/runners/backends/mp_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45581 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/runners/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/runners/multiprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/runners/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/runners/runtime_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.935029 lightning-app-2.0.2/src/lightning_app/source_code/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/source_code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/source_code/copytree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/source_code/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/source_code/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/source_code/tar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/source_code/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.935029 lightning-app-2.0.2/src/lightning_app/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/storage/copier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13153 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/storage/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/storage/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/storage/mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/storage/orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18312 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/storage/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10967 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/storage/payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/storage/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.935029 lightning-app-2.0.2/src/lightning_app/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/structures/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/structures/list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.939029 lightning-app-2.0.2/src/lightning_app/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/testing/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/testing/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19376 2023-04-24 13:57:17.000000 lightning-app-2.0.2/src/lightning_app/testing/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.939029 lightning-app-2.0.2/src/lightning_app/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.939029 lightning-app-2.0.2/src/lightning_app/ui/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.939029 lightning-app-2.0.2/src/lightning_app/ui/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/static/css/main.bb0f092c.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/static/css/main.bb0f092c.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2022-12-09 18:23:41.000000 lightning-app-2.0.2/src/lightning_app/ui/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.939029 lightning-app-2.0.2/src/lightning_app/ui/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/static/js/787.418637a8.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10281 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/static/js/787.418637a8.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   349883 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/static/js/main.2b242b99.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/static/js/main.2b242b99.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  1343802 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/static/js/main.2b242b99.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2022-12-09 18:23:41.000000 lightning-app-2.0.2/src/lightning_app/ui/static/lightningState.js
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2022-12-09 18:23:41.000000 lightning-app-2.0.2/src/lightning_app/ui/static/manifest.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.943029 lightning-app-2.0.2/src/lightning_app/ui/static/media/
+-rw-r--r--   0 runner    (1001) docker     (123)    21692 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/static/media/UCity-Light.30446c15a21bf8a994e8.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    29124 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/static/media/UCity-Light.47cf3e33cb6bb1496c95.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    29800 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/static/media/UCity-Regular.7a3b475525ed92dc7816.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    22408 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/static/media/UCity-Regular.8afa44ac39706d62b62b.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    21108 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/static/media/UCity-Semibold.80655a0e8b4bb5f30545.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    28356 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/static/media/UCity-Semibold.bb7aab96e378ebd6a651.woff
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/static/media/error.11892047d0183a4723b91dc0fb98cb95.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7931 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/static/media/lightning-logo-with-text.b964c8fbf221c97eb8ce52bb6e3a30d6.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/static/media/success.5edae4c5b171e2c1c5a3c54273c47ba8.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2022-12-09 18:23:58.000000 lightning-app-2.0.2/src/lightning_app/ui/static/media/warning.5c542673e84e77ceb6a230bfea7f7263.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2022-12-09 18:23:41.000000 lightning-app-2.0.2/src/lightning_app/ui/static/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.955029 lightning-app-2.0.2/src/lightning_app/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/app_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20581 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/app_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/app_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/app_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13352 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/cli_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/cluster_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/clusters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.955029 lightning-app-2.0.2/src/lightning_app/utilities/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11147 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/dependency_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/load_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/log_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/logs_socket_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60241 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/name_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10409 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/openapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.955029 lightning-app-2.0.2/src/lightning_app/utilities/packaging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/packaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/packaging/app_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/packaging/build_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/packaging/cloud_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/packaging/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/packaging/lightning_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/packaging/tarfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30463 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/safe_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12643 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app/utilities/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 13:57:07.000000 lightning-app-2.0.2/src/lightning_app/version.info
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:57:18.891029 lightning-app-2.0.2/src/lightning_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14208 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-24 13:57:18.000000 lightning-app-2.0.2/src/lightning_app.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 13:57:07.000000 lightning-app-2.0.2/src/version.info
```

### Comparing `lightning-app-2.0.1.post0/.actions/assistant.py` & `lightning-app-2.0.2/.actions/assistant.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/LICENSE` & `lightning-app-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/PKG-INFO` & `lightning-app-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-app
-Version: 2.0.1.post0
+Version: 2.0.2
 Summary: Use Lightning Apps to build everything from production-ready, multi-cloud ML systems to simple research demos.
 Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning-AI et al.
 Author-email: name@pytorchlightning.ai
 License: Apache-2.0
 Download-URL: https://github.com/Lightning-AI/lightning
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
@@ -21,18 +21,18 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: cloud
 Provides-Extra: components
 Provides-Extra: test
 Provides-Extra: ui
+Provides-Extra: cloud
 Provides-Extra: extra
 Provides-Extra: all
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: lightning-app Version: 2.0.1.post0 Summary: Use
-Lightning Apps to build everything from production-ready, multi-cloud ML
-systems to simple research demos. Home-page: https://github.com/Lightning-AI/
-lightning Author: Lightning-AI et al. Author-email: name@pytorchlightning.ai
-License: Apache-2.0 Download-URL: https://github.com/Lightning-AI/lightning
-Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
-Project-URL: Documentation, https://lightning.ai/lightning-docs Project-URL:
-Source Code, https://github.com/Lightning-AI/lightning Keywords: deep
-learning,pytorch,AI Platform: UNKNOWN Classifier: Environment :: Console
-Classifier: Natural Language :: English Classifier: Development Status :: 4 -
-Beta Classifier: Intended Audience :: Developers Classifier: Topic ::
-Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
-Scientific/Engineering :: Information Analysis Classifier: Operating System ::
-OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Requires-
-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra: cloud
-Provides-Extra: components Provides-Extra: test Provides-Extra: ui Provides-
-Extra: extra Provides-Extra: all Provides-Extra: dev License-File: LICENSE
+Metadata-Version: 2.1 Name: lightning-app Version: 2.0.2 Summary: Use Lightning
+Apps to build everything from production-ready, multi-cloud ML systems to
+simple research demos. Home-page: https://github.com/Lightning-AI/lightning
+Author: Lightning-AI et al. Author-email: name@pytorchlightning.ai License:
+Apache-2.0 Download-URL: https://github.com/Lightning-AI/lightning Project-URL:
+Bug Tracker, https://github.com/Lightning-AI/lightning/issues Project-URL:
+Documentation, https://lightning.ai/lightning-docs Project-URL: Source Code,
+https://github.com/Lightning-AI/lightning Keywords: deep learning,pytorch,AI
+Platform: UNKNOWN Classifier: Environment :: Console Classifier: Natural
+Language :: English Classifier: Development Status :: 4 - Beta Classifier:
+Intended Audience :: Developers Classifier: Topic :: Scientific/Engineering ::
+Artificial Intelligence Classifier: Topic :: Scientific/Engineering ::
+Information Analysis Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Requires-Python: >=3.8 Description-
+Content-Type: text/markdown Provides-Extra: components Provides-Extra: test
+Provides-Extra: ui Provides-Extra: cloud Provides-Extra: extra Provides-Extra:
+all Provides-Extra: dev License-File: LICENSE
  [https://pl-flash-data.s3.amazonaws.com/brandmark.png] **With Lightning Apps,
 you build exactly what you need: from production-ready, multi-cloud ML systems
                           to simple research demos.**
     ______________________________________________________________________
             Website â¢ Docs â¢ Getting_started â¢ Help â¢ Slack
        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
 lightning_app)](https://pypi.org/project/lightning_app/) [![PyPI Status](https:
```

### Comparing `lightning-app-2.0.1.post0/README.md` & `lightning-app-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/pyproject.toml` & `lightning-app-2.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,17 @@
 [tool.ruff]
 line-length = 120
 # Enable Pyflakes `E` and `F` codes by default.
 select = [
     "E", "W",  # see: https://pypi.org/project/pycodestyle
     "F",  # see: https://pypi.org/project/pyflakes
 ]
+extend-select = [
+    "C4",  # see: https://pypi.org/project/flake8-comprehensions
+]
 ignore = [
     "E731",  # Do not assign a lambda expression, use a def
 ]
 # Exclude a variety of commonly ignored directories.
 exclude = [
     ".git",
     "docs",
```

### Comparing `lightning-app-2.0.1.post0/setup.py` & `lightning-app-2.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/CHANGELOG.md` & `lightning-app-2.0.2/src/lightning_app/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/).
 
-## [2.0.1post] - 2023-04-12
+
+## [2.0.2] - 2023-04-24
 
 ### Fixed
 
-- Fix frontend hosts when running with multi-process in the cloud ([#17324](https://github.com/Lightning-AI/lightning/pull/17324))
+- Resolved Lightning App with remote storage ([#17426](https://github.com/Lightning-AI/lightning/pull/17426))
+- Fixed `AppState`, streamlit example ([#17452](https://github.com/Lightning-AI/lightning/pull/17452))
 
 
 
 ## [2.0.1] - 2023-03-30
 
-No changes.
+- Fix frontend hosts when running with multi-process in the cloud ([#17324](https://github.com/Lightning-AI/lightning/pull/17324))
 
 
 ## [2.0.0] - 2023-03-15
 
 ### Added
 
 - Added `--zip` option to the `lightning cp` command to copy content from the Cloud Platform Filesystem as a zipfile
```

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/README.md` & `lightning-app-2.0.2/src/lightning_app/README.md`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/__about__.py` & `lightning-app-2.0.2/src/lightning_app/__about__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/__init__.py` & `lightning-app-2.0.2/src/lightning_app/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/__setup__.py` & `lightning-app-2.0.2/src/lightning_app/__setup__.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 def _prepare_extras() -> Dict[str, Any]:
     assistant = _load_assistant()
     # https://setuptools.readthedocs.io/en/latest/setuptools.html#declaring-extras
     # Define package extras. These are only installed if you specify them.
     # From remote, use like `pip install pytorch-lightning[dev, docs]`
     # From local copy of repo, use like `pip install ".[dev, docs]"`
     req_files = [Path(p) for p in glob.glob(os.path.join(_PATH_REQUIREMENTS, "*.txt"))]
-    common_args = dict(path_dir=_PATH_REQUIREMENTS, unfreeze="none" if _FREEZE_REQUIREMENTS else "major")
+    common_args = {"path_dir": _PATH_REQUIREMENTS, "unfreeze": "none" if _FREEZE_REQUIREMENTS else "major"}
     extras = {
         p.stem: assistant.load_requirements(file_name=p.name, **common_args)
         for p in req_files
         if p.name not in ("docs.txt", "devel.txt", "base.txt")
     }
     extras["extra"] = extras["cloud"] + extras["ui"] + extras["components"]
     extras["all"] = extras["extra"]
@@ -54,47 +54,47 @@
     long_description = assistant.load_readme_description(
         _PACKAGE_ROOT, homepage=about.__homepage__, version=version.version
     )
 
     # TODO: remove this once lightning-ui package is ready as a dependency
     assistant._download_frontend(_PACKAGE_ROOT)
 
-    return dict(
-        name="lightning-app",
-        version=version.version,
-        description=about.__docs__,
-        author=about.__author__,
-        author_email=about.__author_email__,
-        url=about.__homepage__,
-        download_url="https://github.com/Lightning-AI/lightning",
-        license=about.__license__,
-        packages=find_packages(where="src", include=["lightning_app", "lightning_app.*"]),
-        package_dir={"": "src"},
-        long_description=long_description,
-        long_description_content_type="text/markdown",
-        include_package_data=True,
-        zip_safe=False,
-        keywords=["deep learning", "pytorch", "AI"],
-        python_requires=">=3.8",
-        entry_points={
+    return {
+        "name": "lightning-app",
+        "version": version.version,
+        "description": about.__docs__,
+        "author": about.__author__,
+        "author_email": about.__author_email__,
+        "url": about.__homepage__,
+        "download_url": "https://github.com/Lightning-AI/lightning",
+        "license": about.__license__,
+        "packages": find_packages(where="src", include=["lightning_app", "lightning_app.*"]),
+        "package_dir": {"": "src"},
+        "long_description": long_description,
+        "long_description_content_type": "text/markdown",
+        "include_package_data": True,
+        "zip_safe": False,
+        "keywords": ["deep learning", "pytorch", "AI"],
+        "python_requires": ">=3.8",
+        "entry_points": {
             "console_scripts": [
                 "lightning = lightning_app.cli.lightning_cli:main",
             ],
         },
-        setup_requires=[],
-        install_requires=assistant.load_requirements(
+        "setup_requires": [],
+        "install_requires": assistant.load_requirements(
             _PATH_REQUIREMENTS, unfreeze="none" if _FREEZE_REQUIREMENTS else "major"
         ),
-        extras_require=_prepare_extras(),
-        project_urls={
+        "extras_require": _prepare_extras(),
+        "project_urls": {
             "Bug Tracker": "https://github.com/Lightning-AI/lightning/issues",
             "Documentation": "https://lightning.ai/lightning-docs",
             "Source Code": "https://github.com/Lightning-AI/lightning",
         },
-        classifiers=[
+        "classifiers": [
             "Environment :: Console",
             "Natural Language :: English",
             # How mature is this project? Common values are
             #   3 - Alpha, 4 - Beta, 5 - Production/Stable
             "Development Status :: 4 - Beta",
             # Indicate who your project is intended for
             "Intended Audience :: Developers",
@@ -106,8 +106,8 @@
             # Specify the Python versions you support here. In particular, ensure
             # that you indicate whether you support Python 2, Python 3 or both.
             "Programming Language :: Python :: 3",
             "Programming Language :: Python :: 3.8",
             "Programming Language :: Python :: 3.9",
             "Programming Language :: Python :: 3.10",
         ],
-    )
+    }
```

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/api/http_methods.py` & `lightning-app-2.0.2/src/lightning_app/api/http_methods.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/api/request_types.py` & `lightning-app-2.0.2/src/lightning_app/api/request_types.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/.gitignore` & `lightning-app-2.0.2/src/lightning_app/cli/app-template/.gitignore`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/LICENSE` & `lightning-app-2.0.2/src/lightning_app/cli/app-template/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/README.md` & `lightning-app-2.0.2/src/lightning_app/cli/app-template/README.md`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/app-template/tests/test_placeholdername_app.py` & `lightning-app-2.0.2/src/lightning_app/cli/app-template/tests/test_placeholdername_app.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/cmd_apps.py` & `lightning-app-2.0.2/src/lightning_app/cli/cmd_apps.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/cmd_clusters.py` & `lightning-app-2.0.2/src/lightning_app/cli/cmd_clusters.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/cmd_init.py` & `lightning-app-2.0.2/src/lightning_app/cli/cmd_init.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/cmd_install.py` & `lightning-app-2.0.2/src/lightning_app/cli/cmd_install.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/cmd_pl_init.py` & `lightning-app-2.0.2/src/lightning_app/cli/cmd_pl_init.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/cmd_react_ui_init.py` & `lightning-app-2.0.2/src/lightning_app/cli/cmd_react_ui_init.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/cmd_ssh_keys.py` & `lightning-app-2.0.2/src/lightning_app/cli/cmd_ssh_keys.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/commands/app_commands.py` & `lightning-app-2.0.2/src/lightning_app/cli/commands/app_commands.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/commands/cd.py` & `lightning-app-2.0.2/src/lightning_app/cli/commands/cd.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/commands/cp.py` & `lightning-app-2.0.2/src/lightning_app/cli/commands/cp.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/commands/logs.py` & `lightning-app-2.0.2/src/lightning_app/cli/commands/logs.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/commands/ls.py` & `lightning-app-2.0.2/src/lightning_app/cli/commands/ls.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/commands/pwd.py` & `lightning-app-2.0.2/src/lightning_app/cli/commands/pwd.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/commands/rm.py` & `lightning-app-2.0.2/src/lightning_app/cli/commands/rm.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/.github/workflows/ci-testing.yml` & `lightning-app-2.0.2/src/lightning_app/cli/component-template/.github/workflows/ci-testing.yml`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/.gitignore` & `lightning-app-2.0.2/src/lightning_app/cli/component-template/.gitignore`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/LICENSE` & `lightning-app-2.0.2/src/lightning_app/cli/component-template/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/component-template/README.md` & `lightning-app-2.0.2/src/lightning_app/cli/component-template/README.md`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/connect/app.py` & `lightning-app-2.0.2/src/lightning_app/cli/connect/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,15 +259,15 @@
 
 
 def _get_commands_folder() -> str:
     return os.path.join(_LIGHTNING_CONNECTION_FOLDER, "commands")
 
 
 def _write_commands_metadata(api_commands):
-    metadata = {command_name: metadata for command_name, metadata in api_commands.items()}
+    metadata = dict(api_commands.items())
     metadata_path = os.path.join(_get_commands_folder(), ".meta.json")
     with open(metadata_path, "w") as f:
         json.dump(metadata, f)
 
 
 def _get_commands_metadata():
     metadata_path = os.path.join(_get_commands_folder(), ".meta.json")
@@ -279,15 +279,15 @@
     return os.path.join(_get_commands_folder(), f"{command}.py")
 
 
 def _list_app_commands(echo: bool = True) -> List[str]:
     metadata = _get_commands_metadata()
     metadata = {key.replace("_", " "): value for key, value in metadata.items()}
 
-    command_names = list(sorted(metadata.keys()))
+    command_names = sorted(metadata.keys())
     if not command_names:
         click.echo("The current Lightning App doesn't have commands.")
         return []
 
     app_info = metadata[command_names[0]].get("app_info", None)
 
     title, description, on_connect_end = "Lightning", None, None
```

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/connect/data.py` & `lightning-app-2.0.2/src/lightning_app/cli/connect/data.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/connect/maverick.py` & `lightning-app-2.0.2/src/lightning_app/cli/connect/maverick.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/core.py` & `lightning-app-2.0.2/src/lightning_app/cli/core.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/lightning_cli.py` & `lightning-app-2.0.2/src/lightning_app/cli/lightning_cli.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/lightning_cli_create.py` & `lightning-app-2.0.2/src/lightning_app/cli/lightning_cli_create.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/lightning_cli_delete.py` & `lightning-app-2.0.2/src/lightning_app/cli/lightning_cli_delete.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/lightning_cli_list.py` & `lightning-app-2.0.2/src/lightning_app/cli/lightning_cli_list.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/app.py` & `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/app.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/core/callbacks.py` & `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/core/callbacks.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/core/components/logger/tensorboard.py` & `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/core/components/logger/tensorboard.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/core/components/logger/weights_and_biases.py` & `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/core/components/logger/weights_and_biases.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/core/components/script_runner/script_runner.py` & `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/core/components/script_runner/script_runner.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/core/state.py` & `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/core/state.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/setup.py` & `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/setup.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/tests/core/test_callbacks.py` & `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/tests/core/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/.prettierrc` & `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/.prettierrc`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/craco.config.js` & `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/craco.config.js`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/package.json` & `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/package.json`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/public/favicon.svg` & `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/public/favicon.svg`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/public/index.html` & `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/public/index.html`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/App.tsx` & `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/App.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/components/EnvironmentConfigurator.tsx` & `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/components/EnvironmentConfigurator.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/components/ErrorPanel.tsx` & `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/components/ErrorPanel.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/components/ExecutionSummary.tsx` & `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/components/ExecutionSummary.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/components/HyperparameterSummary.tsx` & `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/components/HyperparameterSummary.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/components/Launcher.tsx` & `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/components/Launcher.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBar.tsx` & `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBar.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBarGroup.tsx` & `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBarGroup.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/components/Timer.tsx` & `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/components/Timer.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/hooks/useLightningState.ts` & `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/hooks/useLightningState.ts`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/index.tsx` & `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/index.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/src/types/lightning.ts` & `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/src/types/lightning.ts`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/pl-app-template/ui/tsconfig.json` & `lightning-app-2.0.2/src/lightning_app/cli/pl-app-template/ui/tsconfig.json`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/README.md` & `lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/README.md`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/example_app.py` & `lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/example_app.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/package.json` & `lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/package.json`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/src/App.tsx` & `lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/src/App.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/src/favicon.svg` & `lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/src/favicon.svg`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/src/hooks/useLightningState.ts` & `lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/src/hooks/useLightningState.ts`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/src/types/lightning.ts` & `lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/src/types/lightning.ts`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/tsconfig.json` & `lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/tsconfig.json`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/cli/react-ui-template/ui/yarn.lock` & `lightning-app-2.0.2/src/lightning_app/cli/react-ui-template/ui/yarn.lock`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/components/__init__.py` & `lightning-app-2.0.2/src/lightning_app/components/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/components/database/client.py` & `lightning-app-2.0.2/src/lightning_app/components/database/client.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/components/database/server.py` & `lightning-app-2.0.2/src/lightning_app/components/database/server.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/components/database/utilities.py` & `lightning-app-2.0.2/src/lightning_app/components/database/utilities.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/components/multi_node/base.py` & `lightning-app-2.0.2/src/lightning_app/components/multi_node/base.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/components/multi_node/fabric.py` & `lightning-app-2.0.2/src/lightning_app/components/multi_node/fabric.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/components/multi_node/pytorch_spawn.py` & `lightning-app-2.0.2/src/lightning_app/components/multi_node/pytorch_spawn.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/components/multi_node/trainer.py` & `lightning-app-2.0.2/src/lightning_app/components/multi_node/trainer.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/components/python/popen.py` & `lightning-app-2.0.2/src/lightning_app/components/python/popen.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/components/python/tracer.py` & `lightning-app-2.0.2/src/lightning_app/components/python/tracer.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/components/serve/__init__.py` & `lightning-app-2.0.2/src/lightning_app/components/serve/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/components/serve/auto_scaler.py` & `lightning-app-2.0.2/src/lightning_app/components/serve/auto_scaler.py`

 * *Files 0% similar despite different names*

```diff
@@ -605,18 +605,18 @@
     def workers(self) -> List[LightningWork]:
         return [self.get_work(i) for i in range(self.num_replicas)]
 
     def create_work(self) -> LightningWork:
         """Replicates a LightningWork instance with args and kwargs provided via ``__init__``."""
         cloud_compute = self._work_kwargs.get("cloud_compute", None)
         self._work_kwargs.update(
-            dict(
-                start_with_flow=False,
-                cloud_compute=cloud_compute.clone() if cloud_compute else None,
-            )
+            {
+                "start_with_flow": False,
+                "cloud_compute": cloud_compute.clone() if cloud_compute else None,
+            }
         )
         return self._work_cls(*self._work_args, **self._work_kwargs)
 
     def add_work(self, work) -> str:
         """Adds a new LightningWork instance.
 
         Returns:
```

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/components/serve/catimage.png` & `lightning-app-2.0.2/src/lightning_app/components/serve/catimage.png`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/components/serve/cold_start_proxy.py` & `lightning-app-2.0.2/src/lightning_app/components/serve/cold_start_proxy.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/components/serve/gradio_server.py` & `lightning-app-2.0.2/src/lightning_app/components/serve/gradio_server.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/components/serve/python_server.py` & `lightning-app-2.0.2/src/lightning_app/components/serve/python_server.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/components/serve/serve.py` & `lightning-app-2.0.2/src/lightning_app/components/serve/serve.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/components/serve/streamlit.py` & `lightning-app-2.0.2/src/lightning_app/components/serve/streamlit.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/components/serve/types/image.py` & `lightning-app-2.0.2/src/lightning_app/components/serve/types/image.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/components/serve/types/type.py` & `lightning-app-2.0.2/src/lightning_app/components/serve/types/type.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/components/training.py` & `lightning-app-2.0.2/src/lightning_app/components/training.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/core/api.py` & `lightning-app-2.0.2/src/lightning_app/core/api.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/core/app.py` & `lightning-app-2.0.2/src/lightning_app/core/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,26 +97,14 @@
                 This can be helpful when reporting bugs on Lightning repo.
             info: Provide additional info about the app which will be used to update html title,
                 description and image meta tags and specify any additional tags as list of html strings.
             root_path: Set this to `/path` if you want to run your app behind a proxy at `/path` leave empty for "/".
                 For instance, if you want to run your app at `https://customdomain.com/myapp`,
                 set `root_path` to `/myapp`.
                 You can learn more about proxy `here <https://www.fortinet.com/resources/cyberglossary/proxy-server>`_.
-
-
-        Example:
-
-            >>> from lightning_app import LightningFlow, LightningApp
-            >>> from lightning_app.runners import MultiProcessRuntime
-            >>> class RootFlow(LightningFlow):
-            ...     def run(self):
-            ...         self.stop()
-            ...
-            >>> app = LightningApp(RootFlow())  # application can be dispatched using the `runners`.
-            >>> MultiProcessRuntime(app).dispatch()
         """
 
         self.root_path = root_path  # when running behind a proxy
         self.info = info
 
         from lightning_app.core.flow import _RootFlow
```

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/core/constants.py` & `lightning-app-2.0.2/src/lightning_app/core/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 from pathlib import Path
 from typing import Optional
 
 import lightning_cloud.env
 
 
 def get_lightning_cloud_url() -> str:
+    # detect local development
+    if os.getenv("VSCODE_PROXY_URI", "").startswith("http://localhost:9800"):
+        return "http://localhost:9800"
     # DO NOT CHANGE!
     return os.getenv("LIGHTNING_CLOUD_URL", "https://lightning.ai")
 
 
 SUPPORTED_PRIMITIVE_TYPES = (type(None), str, int, float, bool)
 STATE_UPDATE_TIMEOUT = 0.001
 STATE_ACCUMULATE_WAIT = 0.15
@@ -111,21 +114,9 @@
 
 
 # interruptible support
 def enable_interruptible_works() -> bool:
     return bool(int(os.getenv("LIGHTNING_INTERRUPTIBLE_WORKS", "0")))
 
 
-# Get Cluster Driver
-_CLUSTER_DRIVERS = [None, "k8s", "direct"]
-
-
 def get_cluster_driver() -> Optional[str]:
-    value = os.getenv("LIGHTNING_CLUSTER_DRIVER", None)
-    if value is None:
-        if enable_interruptible_works():
-            value = "direct"
-        else:
-            value = None
-    if value not in _CLUSTER_DRIVERS:
-        raise ValueError(f"Found {value} cluster driver. The value needs to be in {_CLUSTER_DRIVERS}.")
-    return value
+    return "direct"
```

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/core/flow.py` & `lightning-app-2.0.2/src/lightning_app/core/flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         self._structures: set = set()
         self._calls: dict = {}
         self._changes: dict = {}
         self._layout: Union[List[Dict], Dict] = {}
         self._paths: dict = {}
         self._backend: Optional["Backend"] = None
         # tuple instead of a list so that it cannot be modified without using the setter
-        self._lightningignore: Tuple[str, ...] = tuple()
+        self._lightningignore: Tuple[str, ...] = ()
 
     @property
     def name(self) -> str:
         """Return the current LightningFlow name."""
         return self._name or "root"
 
     def __setattr__(self, name: str, value: Any) -> None:
@@ -625,15 +625,15 @@
 
         .. raw:: html
 
                 </div>
             </div>
             <br />
         """
-        return [dict(name=name, content=component) for (name, component) in self.flows.items()]
+        return [{"name": name, "content": component} for (name, component) in self.flows.items()]
 
     def experimental_iterate(self, iterable: Iterable, run_once: bool = True, user_key: str = "") -> Generator:
         """This method should always be used with any kind of iterable to ensure its fault tolerant.
 
         If you want your iterable to always be consumed from scratch, you shouldn't use this method.
 
         Arguments:
```

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/core/queues.py` & `lightning-app-2.0.2/src/lightning_app/core/queues.py`

 * *Files 2% similar despite different names*

```diff
@@ -384,27 +384,38 @@
         if not self.app_id:
             raise ValueError(f"App ID couldn't be extracted from the queue name: {self.name}")
 
         # it's a blocking call, we need to loop and call the backend to mimic this behavior
         if timeout is None:
             while True:
                 try:
-                    return self._get()
+                    try:
+                        return self._get()
+                    except requests.exceptions.HTTPError:
+                        pass
                 except queue.Empty:
                     time.sleep(HTTP_QUEUE_REFRESH_INTERVAL)
 
         # make one request and return the result
         if timeout == 0:
-            return self._get()
+            try:
+                return self._get()
+            except requests.exceptions.HTTPError:
+                return None
 
         # timeout is some value - loop until the timeout is reached
         start_time = time.time()
         while (time.time() - start_time) < timeout:
             try:
-                return self._get()
+                try:
+                    return self._get()
+                except requests.exceptions.HTTPError:
+                    if timeout > self.default_timeout:
+                        return None
+                    raise queue.Empty
             except queue.Empty:
                 # Note: In theory, there isn't a need for a sleep as the queue shouldn't
                 # block the flow if the queue is empty.
                 # However, as the Http Server can saturate,
                 # let's add a sleep here if a higher timeout is provided
                 # than the default timeout
                 if timeout > self.default_timeout:
@@ -437,16 +448,19 @@
         if resp.status_code != 201:
             raise RuntimeError(f"Failed to push to queue: {self._name_suffix}")
 
     def length(self) -> int:
         if not self.app_id:
             raise ValueError(f"App ID couldn't be extracted from the queue name: {self.name}")
 
-        val = self.client.get(f"/v1/{self.app_id}/{self._name_suffix}/length")
-        return int(val.text)
+        try:
+            val = self.client.get(f"/v1/{self.app_id}/{self._name_suffix}/length")
+            return int(val.text)
+        except requests.exceptions.HTTPError:
+            return 0
 
     @staticmethod
     def _split_app_id_and_queue_name(queue_name: str) -> Tuple[str, str]:
         """This splits the app id and the queue name into two parts.
 
         This can be brittle, as if the queue name creation logic changes, the response values from here wouldn't be
         accurate. Remove this eventually and let the Queue class take app id and name of the queue as arguments
```

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/core/work.py` & `lightning-app-2.0.2/src/lightning_app/core/work.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,15 +174,15 @@
         self._response_queue: Optional[BaseQueue] = None
         self._restarting: bool = False
         self._start_with_flow = start_with_flow
         self._local_build_config = local_build_config or BuildConfig()
         self._cloud_build_config = cloud_build_config or BuildConfig()
         self._cloud_compute = cloud_compute or CloudCompute()
         # tuple instead of a list so that it cannot be modified without using the setter
-        self._lightningignore: Tuple[str, ...] = tuple()
+        self._lightningignore: Tuple[str, ...] = ()
         self._backend: Optional[Backend] = None
         self._check_run_is_implemented()
         self._on_init_end()
 
     @property
     def url(self) -> str:
         """Returns the current url of the work."""
```

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/frontend/frontend.py` & `lightning-app-2.0.2/src/lightning_app/frontend/frontend.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/frontend/just_py/just_py.py` & `lightning-app-2.0.2/src/lightning_app/frontend/just_py/just_py.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/frontend/just_py/just_py_base.py` & `lightning-app-2.0.2/src/lightning_app/frontend/just_py/just_py_base.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/frontend/panel/app_state_comm.py` & `lightning-app-2.0.2/src/lightning_app/frontend/panel/app_state_comm.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/frontend/panel/app_state_watcher.py` & `lightning-app-2.0.2/src/lightning_app/frontend/panel/app_state_watcher.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/frontend/panel/panel_frontend.py` & `lightning-app-2.0.2/src/lightning_app/frontend/panel/panel_frontend.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/frontend/panel/panel_serve_render_fn.py` & `lightning-app-2.0.2/src/lightning_app/frontend/panel/panel_serve_render_fn.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/frontend/stream_lit.py` & `lightning-app-2.0.2/src/lightning_app/frontend/stream_lit.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/frontend/streamlit_base.py` & `lightning-app-2.0.2/src/lightning_app/frontend/streamlit_base.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/frontend/utils.py` & `lightning-app-2.0.2/src/lightning_app/frontend/utils.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/frontend/web.py` & `lightning-app-2.0.2/src/lightning_app/frontend/web.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,22 +51,22 @@
         self.serve_dir = serve_dir
         self._process: Optional[mp.Process] = None
 
     def start_server(self, host: str, port: int, root_path: str = "") -> None:
         log_file = str(get_logfile())
         self._process = mp.Process(
             target=_start_server,
-            kwargs=dict(
-                host=host,
-                port=port,
-                serve_dir=self.serve_dir,
-                path=f"/{self.flow.name}",
-                log_file=log_file,
-                root_path=root_path,
-            ),
+            kwargs={
+                "host": host,
+                "port": port,
+                "serve_dir": self.serve_dir,
+                "path": f"/{self.flow.name}",
+                "log_file": log_file,
+                "root_path": root_path,
+            },
         )
         self._process.start()
 
     def stop_server(self) -> None:
         if self._process is None:
             raise RuntimeError("Server is not running. Call `StaticWebFrontend.start_server()` first.")
         self._process.kill()
```

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/perf/pdb.py` & `lightning-app-2.0.2/src/lightning_app/perf/pdb.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/plugin/actions.py` & `lightning-app-2.0.2/src/lightning_app/plugin/actions.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/plugin/plugin.py` & `lightning-app-2.0.2/src/lightning_app/plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/runners/backends/__init__.py` & `lightning-app-2.0.2/src/lightning_app/runners/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/runners/backends/backend.py` & `lightning-app-2.0.2/src/lightning_app/runners/backends/backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     def _wrap_run_method(self, app: "lightning_app.LightningApp", work: "lightning_app.LightningWork"):
         if work.run.__name__ == "_dynamic_run_wrapper":
             return
 
         work.run = partial(self._dynamic_run_wrapper, app=app, work=work, work_run=unwrap(work.run))
 
     def _prepare_queues(self, app: "lightning_app.LightningApp"):
-        kw = dict(queue_id=self.queue_id)
+        kw = {"queue_id": self.queue_id}
         app.delta_queue = self.queues.get_delta_queue(**kw)
         app.readiness_queue = self.queues.get_readiness_queue(**kw)
         app.api_response_queue = self.queues.get_api_response_queue(**kw)
         app.error_queue = self.queues.get_error_queue(**kw)
         app.api_publish_state_queue = self.queues.get_api_state_publish_queue(**kw)
         app.api_delta_queue = app.delta_queue
         app.request_queues = {}
@@ -107,15 +107,15 @@
         app.copy_request_queues = {}
         app.copy_response_queues = {}
         app.caller_queues = {}
         app.work_queues = {}
         app.flow_to_work_delta_queues = {}
 
     def _register_queues(self, app, work):
-        kw = dict(queue_id=self.queue_id, work_name=work.name)
+        kw = {"queue_id": self.queue_id, "work_name": work.name}
         app.request_queues.update({work.name: self.queues.get_orchestrator_request_queue(**kw)})
         app.response_queues.update({work.name: self.queues.get_orchestrator_response_queue(**kw)})
         app.copy_request_queues.update({work.name: self.queues.get_orchestrator_copy_request_queue(**kw)})
         app.copy_response_queues.update({work.name: self.queues.get_orchestrator_copy_response_queue(**kw)})
         app.caller_queues.update({work.name: self.queues.get_caller_queue(**kw)})
         app.flow_to_work_delta_queues.update({work.name: self.queues.get_flow_to_work_delta_queue(**kw)})
```

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/runners/backends/cloud.py` & `lightning-app-2.0.2/src/lightning_app/runners/backends/cloud.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/runners/backends/docker.py` & `lightning-app-2.0.2/src/lightning_app/runners/backends/docker.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/runners/backends/mp_process.py` & `lightning-app-2.0.2/src/lightning_app/runners/backends/mp_process.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/runners/cloud.py` & `lightning-app-2.0.2/src/lightning_app/runners/cloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,14 @@
     ENABLE_APP_COMMENT_COMMAND_EXECUTION,
     enable_interruptible_works,
     enable_multiple_works_in_default_container,
     ENABLE_MULTIPLE_WORKS_IN_NON_DEFAULT_CONTAINER,
     ENABLE_PULLING_STATE_ENDPOINT,
     ENABLE_PUSHING_STATE_ENDPOINT,
     get_cloud_queue_type,
-    get_cluster_driver,
     get_lightning_cloud_url,
     LIGHTNING_CLOUD_PRINT_SPECS,
     SYS_CUSTOMIZATIONS_SYNC_ROOT,
 )
 from lightning_app.core.work import LightningWork
 from lightning_app.runners.backends.cloud import CloudBackend
 from lightning_app.runners.runtime import Runtime
@@ -462,15 +461,15 @@
             ignore_functions = []
 
         if self.app is not None:
             flow_lightningignores = [flow.lightningignore for flow in self.app.flows]
             work_lightningignores = [work.lightningignore for work in self.app.works]
             lightningignores = flow_lightningignores + work_lightningignores
             if lightningignores:
-                merged = sum(lightningignores, tuple())
+                merged = sum(lightningignores, ())
                 logger.debug(f"Found the following lightningignores: {merged}")
                 patterns = _parse_lightningignore(merged)
                 ignore_functions = [*ignore_functions, partial(_filter_ignored, root, patterns)]
 
         return LocalSourceCodeDir(path=root, ignore_functions=ignore_functions)
 
     def _resolve_project(self, project_id: Optional[str] = None) -> V1Membership:
@@ -870,20 +869,14 @@
 
         if not ENABLE_PULLING_STATE_ENDPOINT:
             v1_env_vars.append(V1EnvVar(name="ENABLE_PULLING_STATE_ENDPOINT", value="0"))
 
         if not ENABLE_PUSHING_STATE_ENDPOINT:
             v1_env_vars.append(V1EnvVar(name="ENABLE_PUSHING_STATE_ENDPOINT", value="0"))
 
-        if get_cloud_queue_type():
-            v1_env_vars.append(V1EnvVar(name="LIGHTNING_CLOUD_QUEUE_TYPE", value=get_cloud_queue_type()))
-
-        if get_cluster_driver():
-            v1_env_vars.append(V1EnvVar(name="LIGHTNING_CLUSTER_DRIVER", value=get_cluster_driver()))
-
         if enable_interruptible_works():
             v1_env_vars.append(
                 V1EnvVar(
                     name="LIGHTNING_INTERRUPTIBLE_WORKS",
                     value=os.getenv("LIGHTNING_INTERRUPTIBLE_WORKS", "0"),
                 )
             )
```

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/runners/multiprocess.py` & `lightning-app-2.0.2/src/lightning_app/runners/multiprocess.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,25 +101,25 @@
                     _validate_api(apis)
                     _add_tags_to_api(apis, ["app_api"])
 
                 if is_overridden("configure_commands", self.app.root):
                     commands = _prepare_commands(self.app)
                     apis += _commands_to_api(commands, info=self.app.info)
 
-                kwargs = dict(
-                    apis=apis,
-                    host=self.host,
-                    port=self.port,
-                    api_response_queue=self.app.api_response_queue,
-                    api_publish_state_queue=self.app.api_publish_state_queue,
-                    api_delta_queue=self.app.api_delta_queue,
-                    has_started_queue=has_started_queue,
-                    spec=extract_metadata_from_app(self.app),
-                    root_path=self.app.root_path,
-                )
+                kwargs = {
+                    "apis": apis,
+                    "host": self.host,
+                    "port": self.port,
+                    "api_response_queue": self.app.api_response_queue,
+                    "api_publish_state_queue": self.app.api_publish_state_queue,
+                    "api_delta_queue": self.app.api_delta_queue,
+                    "has_started_queue": has_started_queue,
+                    "spec": extract_metadata_from_app(self.app),
+                    "root_path": self.app.root_path,
+                }
                 server_proc = multiprocessing.Process(target=start_server, kwargs=kwargs)
                 self.processes["server"] = server_proc
                 server_proc.start()
                 # requires to wait for the UI to be clicked on.
 
                 # wait for server to be ready
                 has_started_queue.get()
```

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/runners/runtime.py` & `lightning-app-2.0.2/src/lightning_app/runners/runtime.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/runners/runtime_type.py` & `lightning-app-2.0.2/src/lightning_app/runners/runtime_type.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/source_code/copytree.py` & `lightning-app-2.0.2/src/lightning_app/source_code/copytree.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         ignore_functions = [*ignore_functions, ignore_fn]
 
     if not dry_run:
         os.makedirs(dst, exist_ok=dirs_exist_ok)
 
     errors = []
 
-    entries = [dr for dr in src.iterdir()]
+    entries = list(src.iterdir())
     for fn in ignore_functions:
         # ignore function return only the entries that are not ignored
         entries = fn(src, entries)
 
     for srcentry in entries:
         dstpath = dst / srcentry.name
         try:
```

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/source_code/hashing.py` & `lightning-app-2.0.2/src/lightning_app/source_code/hashing.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/source_code/local.py` & `lightning-app-2.0.2/src/lightning_app/source_code/local.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/source_code/tar.py` & `lightning-app-2.0.2/src/lightning_app/source_code/tar.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/source_code/uploader.py` & `lightning-app-2.0.2/src/lightning_app/source_code/uploader.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/storage/copier.py` & `lightning-app-2.0.2/src/lightning_app/storage/copier.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/storage/drive.py` & `lightning-app-2.0.2/src/lightning_app/storage/drive.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/storage/filesystem.py` & `lightning-app-2.0.2/src/lightning_app/storage/filesystem.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/storage/mount.py` & `lightning-app-2.0.2/src/lightning_app/storage/mount.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/storage/orchestrator.py` & `lightning-app-2.0.2/src/lightning_app/storage/orchestrator.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/storage/path.py` & `lightning-app-2.0.2/src/lightning_app/storage/path.py`

 * *Files 6% similar despite different names*

```diff
@@ -230,20 +230,20 @@
                 fs.get(glob, str(self.absolute()), recursive=False)
         else:
             _logger.debug(f"Attempting to copy {str(response.path)} -> {str(self.absolute())}")
             fs.get(str(response.path), str(self.absolute()), recursive=False)
 
     def to_dict(self) -> dict:
         """Serialize this Path to a dictionary."""
-        return dict(
-            path=str(self),
-            origin_name=self.origin_name,
-            consumer_name=self.consumer_name,
-            metadata=self._metadata,
-        )
+        return {
+            "path": str(self),
+            "origin_name": self.origin_name,
+            "consumer_name": self.consumer_name,
+            "metadata": self._metadata,
+        }
 
     @classmethod
     def from_dict(cls, content: dict) -> "Path":
         """Instantiate a Path from a dictionary."""
         path = cls(content["path"])
         path._origin = content["origin_name"]
         path._consumer = content["consumer_name"]
@@ -423,24 +423,20 @@
 
 def _filesystem() -> AbstractFileSystem:
     fs = LocalFileSystem()
 
     endpoint_url = os.getenv("LIGHTNING_BUCKET_ENDPOINT_URL", "")
     bucket_name = os.getenv("LIGHTNING_BUCKET_NAME", "")
     if endpoint_url != "" and bucket_name != "":
-        key = os.getenv("LIGHTNING_AWS_ACCESS_KEY_ID", "")
-        secret = os.getenv("LIGHTNING_AWS_SECRET_ACCESS_KEY", "")
-        # TODO: Remove when updated on the platform side.
-        if key == "" or secret == "":
-            key = os.getenv("AWS_ACCESS_KEY_ID", "")
-            secret = os.getenv("AWS_SECRET_ACCESS_KEY", "")
-        if key == "" or secret == "":
-            raise RuntimeError("missing S3 bucket credentials")
+        # FIXME: Temporary fix until we remove the injection from the platform
+        if "AWS_ACCESS_KEY_ID" in os.environ:
+            del os.environ["AWS_ACCESS_KEY_ID"]
+            del os.environ["AWS_SECRET_ACCESS_KEY"]
 
-        fs = S3FileSystem(key=key, secret=secret, use_ssl=False, client_kwargs={"endpoint_url": endpoint_url})
+        fs = S3FileSystem()
 
         app_id = os.getenv("LIGHTNING_CLOUD_APP_ID", "")
         if app_id == "":
             raise RuntimeError("missing LIGHTNING_CLOUD_APP_ID")
 
         if not fs.exists(_shared_storage_path()):
             raise RuntimeError(f"shared filesystem {_shared_storage_path()} does not exist")
```

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/storage/payload.py` & `lightning-app-2.0.2/src/lightning_app/storage/payload.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,20 +199,20 @@
             raise RuntimeError(
                 f"An exception was raised while trying to transfer the contents at {response.path}"
                 f" from Work {response.source} to {response.destination}. See the full stacktrace above."
             ) from response.exception
 
     def to_dict(self) -> dict:
         """Serialize this Path to a dictionary."""
-        return dict(
-            name=self.name,
-            origin_name=self.origin_name,
-            consumer_name=self.consumer_name,
-            metadata=self._metadata,
-        )
+        return {
+            "name": self.name,
+            "origin_name": self.origin_name,
+            "consumer_name": self.consumer_name,
+            "metadata": self._metadata,
+        }
 
     @classmethod
     def from_dict(cls, content: dict) -> "_BasePayload":
         """Instantiate a Payload from a dictionary."""
         payload = cls(None)
         payload._name = content["name"]
         payload._origin = content["origin_name"]
```

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/storage/requests.py` & `lightning-app-2.0.2/src/lightning_app/storage/requests.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/structures/dict.py` & `lightning-app-2.0.2/src/lightning_app/structures/dict.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/structures/list.py` & `lightning-app-2.0.2/src/lightning_app/structures/list.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,8 +169,8 @@
         for child_key, child_state in state["flows"].items():
             for child in children:
                 if _prepare_name(child) == child_key:
                     child.set_state(child_state)
 
     def __len__(self):
         """Returns the number of elements within this List."""
-        return len([v for v in self])
+        return sum(1 for _ in self)
```

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/testing/config.py` & `lightning-app-2.0.2/src/lightning_app/testing/config.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/testing/helpers.py` & `lightning-app-2.0.2/src/lightning_app/testing/helpers.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/testing/testing.py` & `lightning-app-2.0.2/src/lightning_app/testing/testing.py`

 * *Files 7% similar despite different names*

```diff
@@ -373,26 +373,28 @@
                 """data => {
                 window.localStorage.setItem('gridDefaultProjectIdOverride', JSON.stringify(data[0]));
             }
             """,
                 [constants.LIGHTNING_CLOUD_PROJECT_ID],
             )
 
+        admin_page.reload()
+
         view_page = context.new_page()
         i = 1
         while True:
             app = _fetch_app_by_name(client, project_id, name)
             msg = f"Still in phase {app.status.phase}"
 
             # wait until the app is running and openapi.json is ready
             if app.status.phase == V1LightningappInstanceState.RUNNING:
-                view_page.goto(f"{app.status.url}/view")
                 status_code = requests.get(f"{app.status.url}/openapi.json").status_code
                 if status_code == 200:
                     print("App is running, continuing with testing...")
+                    view_page.goto(f"{app.status.url}/view")
                     break
                 msg = f"Received status code {status_code} at {app.status.url!r}"
             elif app.status.phase not in (V1LightningappInstanceState.PENDING, V1LightningappInstanceState.NOT_STARTED):
                 # there's a race condition if the app goes from pending to running to something else before we evaluate
                 # the condition above. avoid it by checking stopped explicitly
                 print(f"App finished with phase {app.status.phase}, finished testing...")
                 break
@@ -474,14 +476,27 @@
             id=app_id,
         )
         assert res == {}
     except ApiException as ex:
         print(f"Failed to delete {app_name}. Exception {ex}")
 
 
+def _delete_cloud_space(client, project_id, cloud_space_id, app_name):
+    """Used to delete the parent cloudspace."""
+    print(f"Deleting {app_name} id: {cloud_space_id}")
+    try:
+        res = client.cloud_space_service_delete_cloud_space(
+            project_id=project_id,
+            id=cloud_space_id,
+        )
+        assert res == {}
+    except ApiException as ex:
+        print(f"Failed to delete {app_name}. Exception {ex}")
+
+
 def delete_cloud_lightning_apps():
     """Cleanup cloud apps that start with the name test-{PR_NUMBER}-{TEST_APP_NAME}.
 
     PR_NUMBER and TEST_APP_NAME are environment variables.
     """
 
     client = LightningClient()
@@ -498,14 +513,20 @@
     project_id = _get_project(client).project_id
     list_apps = client.lightningapp_instance_service_list_lightningapp_instances(project_id=project_id)
 
     for lit_app in list_apps.lightningapps:
         if pr_number and app_name and not lit_app.name.startswith(f"test-{pr_number}-{app_name}-"):
             continue
         _delete_lightning_app(client, project_id=project_id, app_id=lit_app.id, app_name=lit_app.name)
+        _delete_cloud_space(
+            client, project_id=project_id, cloud_space_id=lit_app.spec.cloud_space_id, app_name=lit_app.name
+        )
 
     print("deleting apps that were created more than 1 hour ago.")
 
     for lit_app in list_apps.lightningapps:
 
         if lit_app.created_at < datetime.datetime.now(lit_app.created_at.tzinfo) - datetime.timedelta(hours=1):
             _delete_lightning_app(client, project_id=project_id, app_id=lit_app.id, app_name=lit_app.name)
+            _delete_cloud_space(
+                client, project_id=project_id, cloud_space_id=lit_app.spec.cloud_space_id, app_name=lit_app.name
+            )
```

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/ui/asset-manifest.json` & `lightning-app-2.0.2/src/lightning_app/ui/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/ui/index.html` & `lightning-app-2.0.2/src/lightning_app/ui/index.html`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/ui/static/css/main.bb0f092c.css` & `lightning-app-2.0.2/src/lightning_app/ui/static/css/main.bb0f092c.css`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/ui/static/css/main.bb0f092c.css.map` & `lightning-app-2.0.2/src/lightning_app/ui/static/css/main.bb0f092c.css.map`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/ui/static/favicon.ico` & `lightning-app-2.0.2/src/lightning_app/ui/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/ui/static/js/787.418637a8.chunk.js` & `lightning-app-2.0.2/src/lightning_app/ui/static/js/787.418637a8.chunk.js`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/ui/static/js/787.418637a8.chunk.js.map` & `lightning-app-2.0.2/src/lightning_app/ui/static/js/787.418637a8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/ui/static/js/main.2b242b99.js` & `lightning-app-2.0.2/src/lightning_app/ui/static/js/main.2b242b99.js`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/ui/static/js/main.2b242b99.js.LICENSE.txt` & `lightning-app-2.0.2/src/lightning_app/ui/static/js/main.2b242b99.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/ui/static/js/main.2b242b99.js.map` & `lightning-app-2.0.2/src/lightning_app/ui/static/js/main.2b242b99.js.map`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/ui/static/lightningState.js` & `lightning-app-2.0.2/src/lightning_app/ui/static/lightningState.js`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/UCity-Light.30446c15a21bf8a994e8.woff2` & `lightning-app-2.0.2/src/lightning_app/ui/static/media/UCity-Light.30446c15a21bf8a994e8.woff2`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/UCity-Light.47cf3e33cb6bb1496c95.woff` & `lightning-app-2.0.2/src/lightning_app/ui/static/media/UCity-Light.47cf3e33cb6bb1496c95.woff`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/UCity-Regular.7a3b475525ed92dc7816.woff` & `lightning-app-2.0.2/src/lightning_app/ui/static/media/UCity-Regular.7a3b475525ed92dc7816.woff`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/UCity-Regular.8afa44ac39706d62b62b.woff2` & `lightning-app-2.0.2/src/lightning_app/ui/static/media/UCity-Regular.8afa44ac39706d62b62b.woff2`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/UCity-Semibold.80655a0e8b4bb5f30545.woff2` & `lightning-app-2.0.2/src/lightning_app/ui/static/media/UCity-Semibold.80655a0e8b4bb5f30545.woff2`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/UCity-Semibold.bb7aab96e378ebd6a651.woff` & `lightning-app-2.0.2/src/lightning_app/ui/static/media/UCity-Semibold.bb7aab96e378ebd6a651.woff`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/lightning-logo-with-text.b964c8fbf221c97eb8ce52bb6e3a30d6.svg` & `lightning-app-2.0.2/src/lightning_app/ui/static/media/lightning-logo-with-text.b964c8fbf221c97eb8ce52bb6e3a30d6.svg`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/ui/static/media/warning.5c542673e84e77ceb6a230bfea7f7263.svg` & `lightning-app-2.0.2/src/lightning_app/ui/static/media/warning.5c542673e84e77ceb6a230bfea7f7263.svg`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/app_commands.py` & `lightning-app-2.0.2/src/lightning_app/utilities/app_commands.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/app_helpers.py` & `lightning-app-2.0.2/src/lightning_app/utilities/app_helpers.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/app_logs.py` & `lightning-app-2.0.2/src/lightning_app/utilities/app_logs.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,21 +23,24 @@
 
 from lightning_app.utilities.log_helpers import _error_callback, _OrderedLogEntry
 from lightning_app.utilities.logs_socket_api import _LightningLogsSocketAPI
 
 
 @dataclass
 class _LogEventLabels:
-    app: str
-    container: str
-    filename: str
-    job: str
-    namespace: str
-    node_name: str
-    pod: str
+    app: Optional[str] = None
+    container: Optional[str] = None
+    filename: Optional[str] = None
+    job: Optional[str] = None
+    namespace: Optional[str] = None
+    node_name: Optional[str] = None
+    pod: Optional[str] = None
+    clusterID: Optional[str] = None
+    component: Optional[str] = None
+    projectID: Optional[str] = None
     stream: Optional[str] = None
 
 
 @dataclass
 class _LogEvent(_OrderedLogEntry):
     component_name: str
     labels: _LogEventLabels
```

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/app_status.py` & `lightning-app-2.0.2/src/lightning_app/utilities/app_status.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/auth.py` & `lightning-app-2.0.2/src/lightning_app/utilities/auth.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/cli_helpers.py` & `lightning-app-2.0.2/src/lightning_app/utilities/cli_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,15 +265,15 @@
         return None
     try:
         response = requests.get(f"https://pypi.org/pypi/{__package_name__}/json")
         releases = response.json()["releases"]
         if __version__ not in releases:
             # Always return None if not installed from PyPI (e.g. dev versions)
             return None
-        releases = {version: release for version, release in filter(_is_valid_release, releases.items())}
+        releases = dict(filter(_is_valid_release, releases.items()))
         sorted_releases = sorted(
             releases.items(), key=lambda release: release[1][0]["upload_time_iso_8601"], reverse=True
         )
         latest_version = sorted_releases[0][0]
         return None if __version__ == latest_version else latest_version
     except Exception:
         # Return None if any exception occurs
```

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/cloud.py` & `lightning-app-2.0.2/src/lightning_app/utilities/cloud.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/cluster_logs.py` & `lightning-app-2.0.2/src/lightning_app/utilities/cluster_logs.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/clusters.py` & `lightning-app-2.0.2/src/lightning_app/utilities/clusters.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/commands/base.py` & `lightning-app-2.0.2/src/lightning_app/utilities/commands/base.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/component.py` & `lightning-app-2.0.2/src/lightning_app/utilities/component.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/data_structures.py` & `lightning-app-2.0.2/src/lightning_app/utilities/data_structures.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/dependency_caching.py` & `lightning-app-2.0.2/src/lightning_app/utilities/dependency_caching.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/enum.py` & `lightning-app-2.0.2/src/lightning_app/utilities/enum.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/exceptions.py` & `lightning-app-2.0.2/src/lightning_app/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/frontend.py` & `lightning-app-2.0.2/src/lightning_app/utilities/frontend.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/git.py` & `lightning-app-2.0.2/src/lightning_app/utilities/git.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/imports.py` & `lightning-app-2.0.2/src/lightning_app/utilities/imports.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/introspection.py` & `lightning-app-2.0.2/src/lightning_app/utilities/introspection.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/layout.py` & `lightning-app-2.0.2/src/lightning_app/utilities/layout.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/load_app.py` & `lightning-app-2.0.2/src/lightning_app/utilities/load_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,26 +280,26 @@
 
 def component_to_metadata(obj: Union["LightningWork", "LightningFlow"]) -> Dict:
     from lightning_app import LightningWork
 
     extras = {}
 
     if isinstance(obj, LightningWork):
-        extras = dict(
-            local_build_config=obj.local_build_config.to_dict(),
-            cloud_build_config=obj.cloud_build_config.to_dict(),
-            cloud_compute=obj.cloud_compute.to_dict(),
-        )
+        extras = {
+            "local_build_config": obj.local_build_config.to_dict(),
+            "cloud_build_config": obj.cloud_build_config.to_dict(),
+            "cloud_compute": obj.cloud_compute.to_dict(),
+        }
 
     return dict(
         affiliation=obj.name.split("."),
         cls_name=obj.__class__.__name__,
         module=obj.__module__,
         docstring=inspect.getdoc(obj.__init__),
         **extras,
     )
 
 
 def extract_metadata_from_app(app: "LightningApp") -> List:
     metadata = {flow.name: component_to_metadata(flow) for flow in app.flows}
     metadata.update({work.name: component_to_metadata(work) for work in app.works})
-    return list(metadata[key] for key in sorted(metadata.keys()))
+    return [metadata[key] for key in sorted(metadata.keys())]
```

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/log.py` & `lightning-app-2.0.2/src/lightning_app/utilities/log.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/log_helpers.py` & `lightning-app-2.0.2/src/lightning_app/utilities/log_helpers.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/login.py` & `lightning-app-2.0.2/src/lightning_app/utilities/login.py`

 * *Files 3% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         )
 
 
 class AuthServer:
     @staticmethod
     def get_auth_url(port: int) -> str:
         redirect_uri = f"http://localhost:{port}/login-complete"
-        params = urlencode(dict(redirectTo=redirect_uri))
+        params = urlencode({"redirectTo": redirect_uri})
         return f"{get_lightning_cloud_url()}/sign-in?{params}"
 
     def login_with_browser(self, auth: Auth) -> None:
         app = FastAPI()
         port = find_free_network_port()
         url = self.get_auth_url(port)
 
@@ -196,15 +196,15 @@
                     background=BackgroundTask(stop_server_once_request_is_done),
                 )
 
             auth.save(token=token, username=user_id, user_id=user_id, api_key=key)
             logger.info("Login Successful")
 
             # Include the credentials in the redirect so that UI will also be logged in
-            params = urlencode(dict(token=token, key=key, userID=user_id))
+            params = urlencode({"token": token, "key": key, "userID": user_id})
 
             return RedirectResponse(
                 url=f"{get_lightning_cloud_url()}/cli-login-successful?{params}",
                 background=BackgroundTask(stop_server_once_request_is_done),
             )
 
         server = uvicorn.Server(config=uvicorn.Config(app, port=port, log_level="error"))
```

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/logs_socket_api.py` & `lightning-app-2.0.2/src/lightning_app/utilities/logs_socket_api.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/name_generator.py` & `lightning-app-2.0.2/src/lightning_app/utilities/name_generator.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/network.py` & `lightning-app-2.0.2/src/lightning_app/utilities/network.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/openapi.py` & `lightning-app-2.0.2/src/lightning_app/utilities/openapi.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/packaging/app_config.py` & `lightning-app-2.0.2/src/lightning_app/utilities/packaging/app_config.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/packaging/build_config.py` & `lightning-app-2.0.2/src/lightning_app/utilities/packaging/build_config.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/packaging/cloud_compute.py` & `lightning-app-2.0.2/src/lightning_app/utilities/packaging/cloud_compute.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,14 +107,19 @@
 
         if self.interruptible:
             if not enable_interruptible_works():
                 raise ValueError("CloudCompute with `interruptible=True` isn't supported yet.")
             if "gpu" not in self.name:
                 raise ValueError("CloudCompute `interruptible=True` is supported only with GPU.")
 
+        # FIXME: Clean the mess on the platform side
+        if self.name == "default" or self.name == "cpu":
+            self.name = "cpu-small"
+            self._internal_id = "default"
+
         # TODO: Remove from the platform first.
         self.preemptible = self.interruptible
 
         # All `default` CloudCompute are identified in the same way.
         if self._internal_id is None:
             self._internal_id = self._generate_id()
 
@@ -143,15 +148,15 @@
         return cls(**d)
 
     @property
     def id(self) -> Optional[str]:
         return self._internal_id
 
     def is_default(self) -> bool:
-        return self.name == "default"
+        return self.name in ("default", "cpu-small")
 
     def _generate_id(self):
         return "default" if self.name == "default" else uuid4().hex[:7]
 
     def clone(self):
         new_dict = self.to_dict()
         new_dict["_internal_id"] = self._generate_id()
```

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/packaging/docker.py` & `lightning-app-2.0.2/src/lightning_app/utilities/packaging/docker.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/packaging/lightning_utils.py` & `lightning-app-2.0.2/src/lightning_app/utilities/packaging/lightning_utils.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/packaging/tarfile.py` & `lightning-app-2.0.2/src/lightning_app/utilities/packaging/tarfile.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/port.py` & `lightning-app-2.0.2/src/lightning_app/utilities/port.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/proxies.py` & `lightning-app-2.0.2/src/lightning_app/utilities/proxies.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/redis.py` & `lightning-app-2.0.2/src/lightning_app/utilities/redis.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/safe_pickle.py` & `lightning-app-2.0.2/src/lightning_app/utilities/safe_pickle.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/scheduler.py` & `lightning-app-2.0.2/src/lightning_app/utilities/scheduler.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/secrets.py` & `lightning-app-2.0.2/src/lightning_app/utilities/secrets.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/state.py` & `lightning-app-2.0.2/src/lightning_app/utilities/state.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from deepdiff import DeepDiff
 from requests import Session
 from requests.exceptions import ConnectionError
 
 from lightning_app.core.constants import APP_SERVER_HOST, APP_SERVER_PORT
 from lightning_app.storage.drive import _maybe_create_drive
 from lightning_app.utilities.app_helpers import AppStatePlugin, BaseStatePlugin, Logger
-from lightning_app.utilities.network import _configure_session
+from lightning_app.utilities.network import _configure_session, LightningClient
 
 logger = Logger(__name__)
 
 # GLOBAL APP STATE
 _LAST_STATE = None
 _STATE = None
 
@@ -46,14 +46,15 @@
         "X-Lightning-Session-ID": context.get("session_id", ""),
         "X-Lightning-Type": context.get("type", ""),
     }
 
 
 class AppState:
     _APP_PRIVATE_KEYS: Tuple[str, ...] = (
+        "_use_localhost",
         "_host",
         "_session_id",
         "_state",
         "_last_state",
         "_url",
         "_port",
         "_request_state",
@@ -89,26 +90,42 @@
             port: Rest API Server current port
             last_state: The state pulled on first access.
             state: The state modified by the user.
             my_affiliation: A tuple describing the affiliation this app state represents. When storing a state dict
                 on this AppState, this affiliation will be used to reduce the scope of the given state.
             plugin: A plugin to handle authorization.
         """
-        use_localhost = "LIGHTNING_APP_STATE_URL" not in os.environ
-        self._host = host or APP_SERVER_HOST
-        self._port = port or (APP_SERVER_PORT if use_localhost else None)
-        self._url = f"{self._host}:{self._port}" if use_localhost else self._host
+        self._use_localhost = "LIGHTNING_APP_STATE_URL" not in os.environ
+        self._host = host or ("http://127.0.0.1" if self._use_localhost else None)
+        self._port = port or (APP_SERVER_PORT if self._use_localhost else None)
         self._last_state = last_state
         self._state = state
         self._session_id = "1234"
         self._my_affiliation = my_affiliation if my_affiliation is not None else AppState._MY_AFFILIATION
         self._authorized = None
         self._attach_plugin(plugin)
         self._session = self._configure_session()
 
+    @property
+    def _url(self) -> str:
+        if self._host is None:
+            app_ip = ""
+
+            if "LIGHTNING_CLOUD_PROJECT_ID" in os.environ and "LIGHTNING_CLOUD_APP_ID" in os.environ:
+                client = LightningClient()
+                app_instance = client.lightningapp_instance_service_get_lightningapp_instance(
+                    os.environ.get("LIGHTNING_CLOUD_PROJECT_ID"),
+                    os.environ.get("LIGHTNING_CLOUD_APP_ID"),
+                )
+                app_ip = app_instance.status.ip_address
+
+            # TODO: Don't hard code port 8080 here
+            self._host = f"http://{app_ip}:8080" if app_ip else APP_SERVER_HOST
+        return f"{self._host}:{self._port}" if self._use_localhost else self._host
+
     def _attach_plugin(self, plugin: Optional[BaseStatePlugin]) -> None:
         if plugin is not None:
             plugin = plugin
         else:
             plugin = AppStatePlugin()
         self._plugin = plugin
```

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/tracer.py` & `lightning-app-2.0.2/src/lightning_app/utilities/tracer.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/tree.py` & `lightning-app-2.0.2/src/lightning_app/utilities/tree.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/types.py` & `lightning-app-2.0.2/src/lightning_app/utilities/types.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app/utilities/warnings.py` & `lightning-app-2.0.2/src/lightning_app/utilities/warnings.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app.egg-info/PKG-INFO` & `lightning-app-2.0.2/src/lightning_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-app
-Version: 2.0.1.post0
+Version: 2.0.2
 Summary: Use Lightning Apps to build everything from production-ready, multi-cloud ML systems to simple research demos.
 Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning-AI et al.
 Author-email: name@pytorchlightning.ai
 License: Apache-2.0
 Download-URL: https://github.com/Lightning-AI/lightning
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
@@ -21,18 +21,18 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: cloud
 Provides-Extra: components
 Provides-Extra: test
 Provides-Extra: ui
+Provides-Extra: cloud
 Provides-Extra: extra
 Provides-Extra: all
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: lightning-app Version: 2.0.1.post0 Summary: Use
-Lightning Apps to build everything from production-ready, multi-cloud ML
-systems to simple research demos. Home-page: https://github.com/Lightning-AI/
-lightning Author: Lightning-AI et al. Author-email: name@pytorchlightning.ai
-License: Apache-2.0 Download-URL: https://github.com/Lightning-AI/lightning
-Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
-Project-URL: Documentation, https://lightning.ai/lightning-docs Project-URL:
-Source Code, https://github.com/Lightning-AI/lightning Keywords: deep
-learning,pytorch,AI Platform: UNKNOWN Classifier: Environment :: Console
-Classifier: Natural Language :: English Classifier: Development Status :: 4 -
-Beta Classifier: Intended Audience :: Developers Classifier: Topic ::
-Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
-Scientific/Engineering :: Information Analysis Classifier: Operating System ::
-OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Requires-
-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra: cloud
-Provides-Extra: components Provides-Extra: test Provides-Extra: ui Provides-
-Extra: extra Provides-Extra: all Provides-Extra: dev License-File: LICENSE
+Metadata-Version: 2.1 Name: lightning-app Version: 2.0.2 Summary: Use Lightning
+Apps to build everything from production-ready, multi-cloud ML systems to
+simple research demos. Home-page: https://github.com/Lightning-AI/lightning
+Author: Lightning-AI et al. Author-email: name@pytorchlightning.ai License:
+Apache-2.0 Download-URL: https://github.com/Lightning-AI/lightning Project-URL:
+Bug Tracker, https://github.com/Lightning-AI/lightning/issues Project-URL:
+Documentation, https://lightning.ai/lightning-docs Project-URL: Source Code,
+https://github.com/Lightning-AI/lightning Keywords: deep learning,pytorch,AI
+Platform: UNKNOWN Classifier: Environment :: Console Classifier: Natural
+Language :: English Classifier: Development Status :: 4 - Beta Classifier:
+Intended Audience :: Developers Classifier: Topic :: Scientific/Engineering ::
+Artificial Intelligence Classifier: Topic :: Scientific/Engineering ::
+Information Analysis Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Requires-Python: >=3.8 Description-
+Content-Type: text/markdown Provides-Extra: components Provides-Extra: test
+Provides-Extra: ui Provides-Extra: cloud Provides-Extra: extra Provides-Extra:
+all Provides-Extra: dev License-File: LICENSE
  [https://pl-flash-data.s3.amazonaws.com/brandmark.png] **With Lightning Apps,
 you build exactly what you need: from production-ready, multi-cloud ML systems
                           to simple research demos.**
     ______________________________________________________________________
             Website â¢ Docs â¢ Getting_started â¢ Help â¢ Slack
        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/
 lightning_app)](https://pypi.org/project/lightning_app/) [![PyPI Status](https:
```

### Comparing `lightning-app-2.0.1.post0/src/lightning_app.egg-info/SOURCES.txt` & `lightning-app-2.0.2/src/lightning_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.1.post0/src/lightning_app.egg-info/requires.txt` & `lightning-app-2.0.2/src/lightning_app.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-lightning-cloud>=0.5.31
+lightning-cloud>=0.5.34
 packaging
 typing-extensions<5.0,>=4.0.0
 deepdiff<7.0,>=5.7.0
 starsessions<2.0,>=1.2.1
 fsspec<2023.0,>=2022.5.0
 croniter<1.4.0,>=1.3.0
 traitlets<6.0,>=5.3.0
 arrow<2.0,>=1.2.0
 lightning-utilities<1.0,>=0.7.0
 beautifulsoup4<5.0,>=4.8.0
 inquirer<4.0,>=2.10.0
 psutil<6.0
 click<9.0
-fastapi<0.89.0
+fastapi<0.89.0,>=0.69.0
+starlette
+pydantic<3.0,>=1.7.4
 dateutils<1.0
 Jinja2<4.0
-pydantic<2.0
 PyYAML<7.0
 requests<3.0
 rich<14.0,>=12.3.0
-starlette<1.0
 urllib3<2.0
 uvicorn<1.0
 websocket-client<2.0
 websockets<11.0
 
 [all]
 redis<5.0,>=4.0.1
@@ -54,27 +54,25 @@
 streamlit<2.0,>=1.13.0
 panel<1.0,>=0.12.7
 lightning_api_access>=0.0.3
 aiohttp<4.0,>=3.8.0
 lightning-fabric>=1.9.0
 pytorch-lightning>=1.9.0
 coverage==6.5.0
-codecov==2.1.12
 pytest==7.2.0
 pytest-timeout==2.1.0
 pytest-cov==4.0.0
 pytest-doctestplus>=0.9.0
 pytest-asyncio==0.20.3
 playwright==1.30.0
 httpx
-trio<1.0
+trio<0.22.0
 pympler
 psutil
 setuptools<68.0
-sqlmodel
 requests-mock
 
 [extra]
 redis<5.0,>=4.0.1
 docker<7.0,>=5.0.0
 s3fs<2023.0,>=2022.5.0
 streamlit<2.0,>=1.13.0
@@ -82,25 +80,23 @@
 lightning_api_access>=0.0.3
 aiohttp<4.0,>=3.8.0
 lightning-fabric>=1.9.0
 pytorch-lightning>=1.9.0
 
 [test]
 coverage==6.5.0
-codecov==2.1.12
 pytest==7.2.0
 pytest-timeout==2.1.0
 pytest-cov==4.0.0
 pytest-doctestplus>=0.9.0
 pytest-asyncio==0.20.3
 playwright==1.30.0
 httpx
-trio<1.0
+trio<0.22.0
 pympler
 psutil
 setuptools<68.0
-sqlmodel
 requests-mock
 
 [ui]
 streamlit<2.0,>=1.13.0
 panel<1.0,>=0.12.7
```


# Comparing `tmp/mindflow-0.3.9.tar.gz` & `tmp/mindflow-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mindflow-0.3.9.tar", last modified: Mon Mar  6 22:02:46 2023, max compression
+gzip compressed data, was "mindflow-0.4.0.tar", last modified: Mon Apr 24 20:38:26 2023, max compression
```

## Comparing `mindflow-0.3.9.tar` & `mindflow-0.4.0.tar`

### file list

```diff
@@ -1,114 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:46.474168 mindflow-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-06 22:02:37.000000 mindflow-0.3.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-06 22:02:37.000000 mindflow-0.3.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-06 22:02:37.000000 mindflow-0.3.9/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-06 22:02:37.000000 mindflow-0.3.9/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 22:02:37.000000 mindflow-0.3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-03-06 22:02:46.474168 mindflow-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-03-06 22:02:37.000000 mindflow-0.3.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-06 22:02:37.000000 mindflow-0.3.9/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:46.466168 mindflow-0.3.9/mindflow/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:46.466168 mindflow-0.3.9/mindflow/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/app/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:46.466168 mindflow-0.3.9/mindflow/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:46.466168 mindflow-0.3.9/mindflow/cli/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/cli/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/cli/config/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/cli/config/menu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:46.466168 mindflow-0.3.9/mindflow/cli/config/questions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/cli/config/questions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:46.466168 mindflow-0.3.9/mindflow/cli/config/questions/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/cli/config/questions/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/cli/config/questions/common/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/cli/config/questions/common/questions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:46.466168 mindflow-0.3.9/mindflow/cli/config/questions/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/cli/config/questions/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/cli/config/questions/model/questions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:46.466168 mindflow-0.3.9/mindflow/cli/config/questions/service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/cli/config/questions/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/cli/config/questions/service/questions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:46.466168 mindflow-0.3.9/mindflow/cli/new_click_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/cli/new_click_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/cli/new_click_cli/cli_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:46.470168 mindflow-0.3.9/mindflow/cli/new_click_cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/cli/new_click_cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/cli/new_click_cli/commands/ask.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/cli/new_click_cli/commands/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/cli/new_click_cli/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/cli/new_click_cli/commands/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/cli/new_click_cli/commands/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/cli/new_click_cli/commands/index.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/cli/new_click_cli/commands/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/cli/new_click_cli/commands/login.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/cli/new_click_cli/commands/pr.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/cli/new_click_cli/commands/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:46.470168 mindflow-0.3.9/mindflow/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/core/ask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/core/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/core/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/core/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/core/index.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/core/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/core/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/core/pr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/core/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:46.470168 mindflow-0.3.9/mindflow/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/db/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:46.470168 mindflow-0.3.9/mindflow/db/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/db/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/db/db/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/db/db/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/db/db/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/db/db/static.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:46.470168 mindflow-0.3.9/mindflow/db/objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/db/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/db/objects/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/db/objects/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/db/objects/mindflow_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/db/objects/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/db/objects/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:46.470168 mindflow-0.3.9/mindflow/db/objects/static_definition/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/db/objects/static_definition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/db/objects/static_definition/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/db/objects/static_definition/mind_flow_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7791 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/db/objects/static_definition/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/db/objects/static_definition/model_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/db/objects/static_definition/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/db/objects/static_definition/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/db/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/main.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:46.474168 mindflow-0.3.9/mindflow/resolving/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/resolving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/resolving/resolve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:46.474168 mindflow-0.3.9/mindflow/resolving/resolvers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/resolving/resolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/resolving/resolvers/base_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/resolving/resolvers/file_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:46.474168 mindflow-0.3.9/mindflow/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/utils/enum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:46.474168 mindflow-0.3.9/mindflow/utils/files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/utils/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/utils/files/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/utils/files/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/utils/files/utf8.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/utils/prompt_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/utils/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-06 22:02:37.000000 mindflow-0.3.9/mindflow/utils/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 22:02:46.466168 mindflow-0.3.9/mindflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-03-06 22:02:46.000000 mindflow-0.3.9/mindflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-03-06 22:02:46.000000 mindflow-0.3.9/mindflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 22:02:46.000000 mindflow-0.3.9/mindflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-06 22:02:46.000000 mindflow-0.3.9/mindflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-06 22:02:46.000000 mindflow-0.3.9/mindflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-06 22:02:46.000000 mindflow-0.3.9/mindflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-06 22:02:37.000000 mindflow-0.3.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 22:02:46.474168 mindflow-0.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-03-06 22:02:37.000000 mindflow-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:26.774243 mindflow-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-24 20:38:15.000000 mindflow-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-24 20:38:15.000000 mindflow-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-24 20:38:15.000000 mindflow-0.4.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-24 20:38:15.000000 mindflow-0.4.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 20:38:15.000000 mindflow-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-24 20:38:15.000000 mindflow-0.4.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-04-24 20:38:26.774243 mindflow-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-04-24 20:38:15.000000 mindflow-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-24 20:38:15.000000 mindflow-0.4.0/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:26.754243 mindflow-0.4.0/mindflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:26.758243 mindflow-0.4.0/mindflow/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/cli/cli_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:26.758243 mindflow-0.4.0/mindflow/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/cli/commands/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/cli/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/cli/commands/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/cli/commands/gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:26.758243 mindflow-0.4.0/mindflow/cli/commands/git/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/cli/commands/git/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/cli/commands/git/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/cli/commands/git/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/cli/commands/git/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/cli/commands/git/mr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/cli/commands/git/pr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/cli/commands/git/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/cli/commands/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/cli/commands/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/cli/commands/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/cli/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:26.762243 mindflow-0.4.0/mindflow/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/core/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/core/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/core/gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:26.762243 mindflow-0.4.0/mindflow/core/git/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/core/git/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/core/git/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/core/git/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/core/git/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/core/git/mr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/core/git/pr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/core/git/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/core/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/core/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/core/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/core/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:26.762243 mindflow-0.4.0/mindflow/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:26.766243 mindflow-0.4.0/mindflow/db/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/db/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/db/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/db/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/db/static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:26.766243 mindflow-0.4.0/mindflow/db/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/objects/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/objects/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/objects/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/objects/mindflow_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/objects/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/objects/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:26.766243 mindflow-0.4.0/mindflow/db/objects/static_definition/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/objects/static_definition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/objects/static_definition/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/objects/static_definition/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/objects/static_definition/mind_flow_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14264 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/objects/static_definition/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/objects/static_definition/model_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/objects/static_definition/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/objects/static_definition/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/db/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:26.770243 mindflow-0.4.0/mindflow/resolving/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/resolving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/resolving/resolve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:26.770243 mindflow-0.4.0/mindflow/resolving/resolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/resolving/resolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/resolving/resolvers/base_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/resolving/resolvers/file_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:26.770243 mindflow-0.4.0/mindflow/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/unit_tests/dummy_diff.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/unit_tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12244 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/unit_tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:26.770243 mindflow-0.4.0/mindflow/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/utils/command_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/utils/diff_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/utils/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/utils/execute.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:26.774243 mindflow-0.4.0/mindflow/utils/files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/utils/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/utils/files/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/utils/files/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/utils/files/utf8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/utils/prompt_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/utils/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/utils/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-24 20:38:15.000000 mindflow-0.4.0/mindflow/utils/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:38:26.754243 mindflow-0.4.0/mindflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-04-24 20:38:26.000000 mindflow-0.4.0/mindflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-24 20:38:26.000000 mindflow-0.4.0/mindflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 20:38:26.000000 mindflow-0.4.0/mindflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-24 20:38:26.000000 mindflow-0.4.0/mindflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-24 20:38:26.000000 mindflow-0.4.0/mindflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-24 20:38:26.000000 mindflow-0.4.0/mindflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-24 20:38:15.000000 mindflow-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 20:38:26.774243 mindflow-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-24 20:38:15.000000 mindflow-0.4.0/setup.py
```

### Comparing `mindflow-0.3.9/.pre-commit-config.yaml` & `mindflow-0.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mindflow-0.3.9/mindflow/cli/config/main.py` & `mindflow-0.4.0/mindflow/db/objects/mindflow_model.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,130 +1,130 @@
-import getpass
 import sys
-
-from mindflow.cli.config.menu import menu
-from mindflow.db.objects.mindflow_model import MindFlowModelConfig
-from mindflow.db.objects.model import ModelConfig
-from mindflow.db.objects.service import ServiceConfig
-from mindflow.db.objects.static_definition.model import (
-    ModelConfigParameterKey,
-    ModelHardTokenLimit,
-    get_model_static,
-)
-from mindflow.db.objects.static_definition.mind_flow_model import (
-    MindFlowModelID,
-)
-
+from typing import Dict
+from typing import Optional
+from mindflow.db.db.json import JSON_DATABASE
+from mindflow.db.db.static import STATIC_DATABASE
+
+from mindflow.db.db.database import Collection
+from mindflow.db.objects.base import BaseObject
+from mindflow.db.objects.model import ConfiguredModel
+from mindflow.db.objects.service import ConfiguredServices
+from mindflow.db.objects.static_definition.mind_flow_model import MindFlowModelID
 from mindflow.db.objects.static_definition.service import (
     ServiceConfigParameterKey,
     ServiceID,
 )
-from mindflow.cli.config.questions.common.enums import (
-    MainOption,
-    YesNo,
-)
-from mindflow.cli.config.questions.common.questions import (
-    ask_another_config,
-)
-from mindflow.cli.config.questions.service.questions import (
-    ask_service,
-    ask_service_config,
-)
-from mindflow.cli.config.questions.model.questions import (
-    ask_mind_flow_model_type,
-    ask_model_by_service,
-    ask_model_config,
-    ask_model_text_completion_openai,
-    ask_model_text_embedding_openai,
-)
 
 
-def set_configuration():
-    option_choice = menu(
-        MainOption.values(), "Which options would you like to configure?"
-    )
-    if MainOption(option_choice) == MainOption.AUTHORIZE:
-        config_service()
-        # Model Config
-    elif MainOption(option_choice) == MainOption.MODEL:
-        config_model()
-    elif MainOption(option_choice) == MainOption.MIND_FLOW_MODEL:
-        config_mindflow_model()
-    else:
-        print("Unrecognized option")
-
-    if YesNo(ask_another_config()) == YesNo.YES:
-        set_configuration()
-
-
-def config_service():
-    service_key = ask_service()
-    service_config_param = ask_service_config()
-
-    if service_config_param == ServiceConfigParameterKey.API_KEY:
-        value = getpass.getpass("API Key: ")
-    elif service_config_param == ServiceConfigParameterKey.API_SECRET:
-        value = getpass.getpass("API Secret: ")
-    else:
-        print("Unrecognized model config parameter")
-        sys.exit(1)
-
-    service_config = ServiceConfig.load(f"{service_key.value}_config")
-    if not service_config:
-        service_config = ServiceConfig(id=f"{service_key.value}_config")
-
-    setattr(service_config, service_config_param.value, value)
-    service_config.save()
-
-
-def config_model():
-    service_key = ask_service()
-    model_key = ask_model_by_service(service_key)
-    model_config_param = ask_model_config()
-
-    if model_config_param == ModelConfigParameterKey.SOFT_TOKEN_LIMIT:
-        model_hard_token_limit = get_model_static(ModelHardTokenLimit, model_key).value
-        while True:
-            value = input("Soft Token Limit: ")
-            if not value.isdigit():
-                print("Soft token limit must be a number")
-                continue
-            value = int(value)
-            if value > model_hard_token_limit:
-                print("Soft token limit cannot be greater than hard token limit")
-            else:
-                break
-    else:
-        print("Unrecognized model config parameter")
-        sys.exit(1)
-
-    model_configs = ModelConfig.load(f"{model_key.value}_config")
-    if not model_configs:
-        model_configs = ModelConfig(id=f"{model_key.value}_config")
-
-    setattr(model_configs, model_config_param.value, value)
-    model_configs.save()
-
-
-def config_mindflow_model():
-    mindflow_model_key = ask_mind_flow_model_type()
-    if mindflow_model_key == MindFlowModelID.INDEX:
-        if mindflow_model_key == MindFlowModelID.INDEX:
-            if ask_service() == ServiceID.OPENAI:
-                value = ask_model_text_completion_openai().value
-        if mindflow_model_key == MindFlowModelID.QUERY:
-            if ask_service() == ServiceID.OPENAI:
-                value = ask_model_text_completion_openai().value
-        if mindflow_model_key == MindFlowModelID.EMBEDDING:
-            if ask_service() == ServiceID.OPENAI:
-                value = ask_model_text_embedding_openai().value
-
-    mindflow_model_config = MindFlowModelConfig.load(
-        f"{mindflow_model_key.value}_config"
-    )
-    if not mindflow_model_config:
-        mindflow_model_config = MindFlowModelConfig(
-            id=f"{mindflow_model_key.value}_config"
-        )
+class MindFlowModel(BaseObject):
+    """MindFlow model object."""
 
-    setattr(mindflow_model_config, "model", value)
-    mindflow_model_config.save()
+    id: str  # index, query, embedding
+    name: str
+    defaults: Dict[str, str]
+    model: str
+
+    _collection: Collection = Collection.MIND_FLOW_MODEL
+    _database = STATIC_DATABASE
+
+
+class MindFlowModelConfig(BaseObject):
+    """MindFlow model config object."""
+
+    id: str
+    model: str
+
+    _collection: Collection = Collection.CONFIGURATIONS
+    _database = JSON_DATABASE
+
+
+class ConfiguredMindFlowModel:
+    """MindFlow model object."""
+
+    id: str  # index, query, embedding
+    name: str
+    defaults: Dict[str, str]
+    model: ConfiguredModel
+
+    def __init__(self, mindflow_model_id: str, configured_services: ConfiguredServices):
+        self.id = mindflow_model_id
+
+        mind_flow_model = MindFlowModel.load(mindflow_model_id)
+        mind_flow_model_config = MindFlowModelConfig.load(f"{mindflow_model_id}_config")
+
+        if mind_flow_model:
+            for key, value in mind_flow_model.__dict__.items():
+                setattr(self, key, value)
+
+        model_id: Optional[str] = None
+        if mind_flow_model_config:
+            if hasattr(mind_flow_model_config, "model"):
+                model_id = mind_flow_model_config.model
+
+        if model_id is None:
+            model_id = self.get_default_model_id(mindflow_model_id, configured_services)
+
+        self.model = ConfiguredModel(model_id)
+
+    def get_default_model_id(
+        self, mindflow_model_id: str, configured_services: ConfiguredServices
+    ) -> str:
+        model_id: Optional[str] = None
+        if hasattr(configured_services.openai, ServiceConfigParameterKey.API_KEY.value):
+            service = configured_services.openai
+            model_id = self.defaults.get(ServiceID.OPENAI.value, None)
+        elif hasattr(
+            configured_services.anthropic, ServiceConfigParameterKey.API_KEY.value
+        ):
+            service = configured_services.anthropic
+            model_id = self.defaults.get(ServiceID.ANTHROPIC.value, None)
+        else:
+            print(
+                "No service API key configured. Please configure an API key for at least one service."
+            )
+            sys.exit(1)
+
+        if model_id is None:
+            raise Exception(
+                "No default model configured for mindflow model: "
+                + mindflow_model_id
+                + " and service: "
+                + service.id
+            )
+
+        return model_id
+
+
+class ConfiguredMindFlowModels:
+    def __init__(self, configured_services: ConfiguredServices):
+        self._configured_services = configured_services
+        self._mind_flow_models: Dict[str, ConfiguredMindFlowModel] = {}
+
+    @property
+    def index(self):
+        if MindFlowModelID.INDEX.value not in self._mind_flow_models:
+            self._mind_flow_models[
+                MindFlowModelID.INDEX.value
+            ] = ConfiguredMindFlowModel(
+                MindFlowModelID.INDEX.value, self._configured_services
+            )
+        return self._mind_flow_models[MindFlowModelID.INDEX.value]
+
+    @property
+    def query(self):
+        if MindFlowModelID.QUERY.value not in self._mind_flow_models:
+            self._mind_flow_models[
+                MindFlowModelID.QUERY.value
+            ] = ConfiguredMindFlowModel(
+                MindFlowModelID.QUERY.value, self._configured_services
+            )
+        return self._mind_flow_models[MindFlowModelID.QUERY.value]
+
+    @property
+    def embedding(self):
+        if MindFlowModelID.EMBEDDING.value not in self._mind_flow_models:
+            self._mind_flow_models[
+                MindFlowModelID.EMBEDDING.value
+            ] = ConfiguredMindFlowModel(
+                MindFlowModelID.EMBEDDING.value, self._configured_services
+            )
+        return self._mind_flow_models[MindFlowModelID.EMBEDDING.value]
```

### Comparing `mindflow-0.3.9/mindflow/cli/new_click_cli/cli_main.py` & `mindflow-0.4.0/mindflow/cli/cli_main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,50 @@
 import click
 
+from mindflow.cli.commands.git.add import add
+from mindflow.cli.commands.git.push import push
+from mindflow.cli.commands.git.commit import commit
+from mindflow.cli.commands.git.diff import diff
+from mindflow.cli.commands.git.mr import mr
+from mindflow.cli.commands.git.pr import pr
+
+from mindflow.cli.commands.chat import chat, history
+from mindflow.cli.commands.delete import delete
+from mindflow.cli.commands.index import index
+from mindflow.cli.commands.inspect import inspect
+from mindflow.cli.commands.login import login
+from mindflow.cli.commands.gen import gen
+from mindflow.cli.commands.config import config
+
 # from mindflow.cli.new_click_cli.commands.config import config
-from mindflow.cli.new_click_cli.commands.ask import ask
-from mindflow.cli.new_click_cli.commands.commit import commit
-from mindflow.cli.new_click_cli.commands.delete import delete
-from mindflow.cli.new_click_cli.commands.diff import diff
-from mindflow.cli.new_click_cli.commands.index import index
-from mindflow.cli.new_click_cli.commands.inspect import inspect
-from mindflow.cli.new_click_cli.commands.login import login
-from mindflow.cli.new_click_cli.commands.pr import pr
-from mindflow.cli.new_click_cli.commands.query import query
 
 
 @click.group()
 def mindflow_cli():
     pass
 
 
 @mindflow_cli.command()
 def version():
-    """Print the version of mindflow."""
+    """Get the currently installed version of mindflow."""
     from mindflow import __version__
 
     click.echo(__version__)
 
 
-mindflow_cli.add_command(ask)
+mindflow_cli.add_command(login)
+mindflow_cli.add_command(chat)
 mindflow_cli.add_command(commit)
-mindflow_cli.add_command(delete)
-mindflow_cli.add_command(diff)
+mindflow_cli.add_command(history)
+mindflow_cli.add_command(gen)
 mindflow_cli.add_command(index)
 mindflow_cli.add_command(inspect)
-mindflow_cli.add_command(login)
+mindflow_cli.add_command(add)
+mindflow_cli.add_command(push)
+mindflow_cli.add_command(delete)
+mindflow_cli.add_command(diff)
+mindflow_cli.add_command(mr)
 mindflow_cli.add_command(pr)
-mindflow_cli.add_command(query)
+mindflow_cli.add_command(config)
 
 if __name__ == "__main__":
     mindflow_cli()
```

### Comparing `mindflow-0.3.9/mindflow/db/controller.py` & `mindflow-0.4.0/mindflow/db/controller.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,38 @@
-from typing import Dict, Optional
+from typing import Dict
+from typing import Optional
 
 from mindflow.db.db.database import Store
 from mindflow.db.db.json import JsonDatabase
 from mindflow.db.db.static import Static
+from mindflow.db.db.pinecone import PineconeDatabase
 
 
 class Databases:
     def __init__(self):
-        self.databases = {}
+        self._databases = {}
 
     @property
     def static(self) -> Static:
-        if Store.STATIC not in self.databases:
-            self.databases[Store.STATIC] = Static()
-        return self.databases[Store.STATIC]
+        if Store.STATIC not in self._databases:
+            self._databases[Store.STATIC] = Static()
+        return self._databases[Store.STATIC]
 
     @property
     def json(self) -> JsonDatabase:
-        if Store.JSON not in self.databases:
-            self.databases[Store.JSON] = JsonDatabase()
-        return self.databases[Store.JSON]
+        if Store.JSON not in self._databases:
+            self._databases[Store.JSON] = JsonDatabase()
+        return self._databases[Store.JSON]
+
+    @property
+    def pinecone(self) -> JsonDatabase:
+        if Store.PINECONE not in self._databases:
+            self._databases[Store.PINECONE] = PineconeDatabase()
+
+        return self._databases[Store.PINECONE]
 
 
 class DatabaseController:
     def __init__(self, db_config: Optional[Dict] = None):
         self.databases = Databases()
```

### Comparing `mindflow-0.3.9/mindflow/db/db/database.py` & `mindflow-0.4.0/mindflow/db/db/database.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,40 @@
-from typing import List, Optional
+from typing import List
+from typing import Optional
+
 from mindflow.utils.enum import ExtendedEnum
 
 
 class Store(ExtendedEnum):
     STATIC = "static"
     JSON = "json"
-    NEO4J = "neo4j"
+    PINECONE = "pinecone"
 
 
 class Collection(ExtendedEnum):
     SERVICE = "service"
     MODEL = "model"
     MIND_FLOW_MODEL = "mind_flow_model"
     CONFIGURATIONS = "configurations"
     DOCUMENT = "document"
+    DOCUMENT_CHUNK = "document_chunk"
+    CONVERSATION = "conversation"
 
 
 class Database:
     def load(self, collection: str, object_id: str) -> Optional[dict]:
         raise NotImplementedError
 
-    def load_bulk(self, collection: str, object_ids: List[str]) -> Optional[List[dict]]:
+    def load_bulk(self, collection: str, object_ids: List[str]) -> List[Optional[dict]]:
         raise NotImplementedError
 
     def delete(self, collection: str, object_id: str):
         raise NotImplementedError
 
     def delete_bulk(self, collection: str, object_ids: List[str]):
         raise NotImplementedError
 
     def save(self, collection: str, value: dict):
         raise NotImplementedError
+
+    def save_bulk(self, collection: str, values: List[dict]):
+        raise NotImplementedError
```

### Comparing `mindflow-0.3.9/mindflow/db/db/static.py` & `mindflow-0.4.0/mindflow/db/db/static.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from typing import Union
+from mindflow.db.db.database import Collection, Database
 from mindflow.db.objects.static_definition.mind_flow_model import MINDFLOW_MODEL_STATIC
-
-from mindflow.db.objects.static_definition.service import SERVICE_STATIC
 from mindflow.db.objects.static_definition.model import MODEL_STATIC
-
-from mindflow.db.db.database import Database, Collection
+from mindflow.db.objects.static_definition.service import SERVICE_STATIC
 
 
 class Static(Database):
     @staticmethod
     def load(collection: str, object_key: str):
         if collection == Collection.SERVICE.value:
             return SERVICE_STATIC[object_key]
         elif collection == Collection.MODEL.value:
             return MODEL_STATIC[object_key]
         elif collection == Collection.MIND_FLOW_MODEL.value:
             return MINDFLOW_MODEL_STATIC[object_key]
         else:
             raise ValueError(f"Unknown object collection: {collection}")
+
+
+STATIC_DATABASE = Static()
```

### Comparing `mindflow-0.3.9/mindflow/db/objects/service.py` & `mindflow-0.4.0/mindflow/db/objects/service.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,45 @@
+from mindflow.db.db.json import JSON_DATABASE
+from mindflow.db.db.static import STATIC_DATABASE
 from mindflow.db.db.database import Collection
-from mindflow.db.objects.base import BaseObject, StaticObject
+from mindflow.db.objects.base import BaseObject
 from mindflow.db.objects.static_definition.service import ServiceID
 
 
-class Service(StaticObject):
+class Service(BaseObject):
     id: str
     name: str
     url: str
     api_url: str
 
     _collection: Collection = Collection.SERVICE
+    _database = STATIC_DATABASE
 
 
 class ServiceConfig(BaseObject):
     """Service config object."""
 
     id: str
     api_key: str
     api_secret: str
+    environment: str
 
     _collection: Collection = Collection.CONFIGURATIONS
+    _database = JSON_DATABASE
 
 
 class ConfiguredService:
     id: str
     name: str
     url: str
     api_url: str
 
     api_key: str
     api_secret: str
+    environment: str
 
     def __init__(self, service_id: str):
         service = Service.load(service_id)
         service_config = ServiceConfig.load(f"{service_id}_config")
 
         if service:
             for key, value in service.__dict__.items():
@@ -42,10 +48,33 @@
         if service_config:
             for key, value in service_config.__dict__.items():
                 if value not in [None, ""]:
                     setattr(self, key, value)
 
 
 class ConfiguredServices:
+    def __init__(self):
+        self._services = {}
+
     @property
     def openai(self) -> ConfiguredService:
-        return ConfiguredService(ServiceID.OPENAI.value)
+        if ServiceID.OPENAI.value not in self._services:
+            self._services[ServiceID.OPENAI.value] = ConfiguredService(
+                ServiceID.OPENAI.value
+            )
+        return self._services[ServiceID.OPENAI.value]
+
+    @property
+    def anthropic(self) -> ConfiguredService:
+        if ServiceID.ANTHROPIC.value not in self._services:
+            self._services[ServiceID.ANTHROPIC.value] = ConfiguredService(
+                ServiceID.ANTHROPIC.value
+            )
+        return self._services[ServiceID.ANTHROPIC.value]
+
+    @property
+    def pinecone(self) -> ConfiguredService:
+        if ServiceID.PINECONE.value not in self._services:
+            self._services[ServiceID.PINECONE.value] = ConfiguredService(
+                ServiceID.PINECONE.value
+            )
+        return self._services[ServiceID.PINECONE.value]
```

### Comparing `mindflow-0.3.9/mindflow/db/objects/static_definition/mind_flow_model.py` & `mindflow-0.4.0/mindflow/db/objects/static_definition/mind_flow_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from typing import Type, Union
-from mindflow.db.objects.static_definition.model_type import ModelType
 from mindflow.db.objects.static_definition.model import ModelID
+from mindflow.db.objects.static_definition.model_type import ModelType
 from mindflow.utils.enum import ExtendedEnum
 
 
 class MindFlowModelParameterKey(ExtendedEnum):
     ID = "id"
     NAME = "name"
     DEFAULTS = "defaults"
+    DESCRIPTION = "description"
 
 
 class MindFlowModelID(ExtendedEnum):
     QUERY = "query"
     INDEX = "index"
     EMBEDDING = "embedding"
 
@@ -37,33 +37,37 @@
 class MindFlowModelType(ExtendedEnum):
     QUERY = ModelType.TEXT_COMPLETION.value
     INDEX = ModelType.TEXT_COMPLETION.value
     EMBEDDING = ModelType.TEXT_EMBEDDING.value
 
 
 class MindFlowModelDescription(ExtendedEnum):
-    QUERY = f"{MindFlowModelName.QUERY}:    Used to generate final response from query."
-    INDEX = f"{MindFlowModelName.INDEX}:    Used to generate deep index from query. (Warning! Expensive and slow!)"
+    QUERY = f"{MindFlowModelName.QUERY}:    Used to respond to chat, queries, and git functionality."
+    INDEX = f"{MindFlowModelName.INDEX}:    Used to generate index summaries used for search."
+    EMBEDDING = f"{MindFlowModelName.EMBEDDING}:    Used to generate embeddings for text used in search."
 
 
 MINDFLOW_MODEL_STATIC = {
     MindFlowModelID.QUERY.value: {
         MindFlowModelParameterKey.ID.value: MindFlowModelID.QUERY.value,
         MindFlowModelParameterKey.NAME.value: MindFlowModelName.QUERY.value,
         MindFlowModelParameterKey.DEFAULTS.value: MindFlowModelDefaults.QUERY.value,
+        MindFlowModelParameterKey.DESCRIPTION.value: MindFlowModelDescription.QUERY.value,
     },
     MindFlowModelID.INDEX.value: {
         MindFlowModelParameterKey.ID.value: MindFlowModelID.INDEX.value,
         MindFlowModelParameterKey.NAME.value: MindFlowModelName.INDEX.value,
         MindFlowModelParameterKey.DEFAULTS.value: MindFlowModelDefaults.INDEX.value,
+        MindFlowModelParameterKey.DESCRIPTION.value: MindFlowModelDescription.INDEX.value,
     },
     MindFlowModelID.EMBEDDING.value: {
         MindFlowModelParameterKey.ID.value: MindFlowModelID.EMBEDDING.value,
         MindFlowModelParameterKey.NAME.value: MindFlowModelName.EMBEDDING.value,
         MindFlowModelParameterKey.DEFAULTS.value: MindFlowModelDefaults.EMBEDDING.value,
+        MindFlowModelParameterKey.DESCRIPTION.value: MindFlowModelDescription.EMBEDDING.value,
     },
 }
 
 # MindFlowModelUnion = Union[
 #     MindFlowModelID,
 #     MindFlowModelDefaults,
 #     MindFlowModelName,
```

### Comparing `mindflow-0.3.9/mindflow/db/objects/static_definition/model_type.py` & `mindflow-0.4.0/mindflow/db/objects/static_definition/model_type.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from typing import Union
 from mindflow.utils.enum import ExtendedEnum
 
 
 class ModelType(ExtendedEnum):
     TEXT_COMPLETION = "text_completion"
     TEXT_EMBEDDING = "text_embedding"
```

### Comparing `mindflow-0.3.9/mindflow/db/objects/static_definition/object.py` & `mindflow-0.4.0/mindflow/db/objects/static_definition/object.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from typing import Type, Union
-from mindflow.db.objects.service import Service, ServiceConfig
-from mindflow.db.objects.model import Model, ModelConfig
-from mindflow.db.objects.mindflow_model import MindFlowModel, MindFlowModelConfig
 from mindflow.db.objects.document import Document
+from mindflow.db.objects.mindflow_model import MindFlowModel
+from mindflow.db.objects.mindflow_model import MindFlowModelConfig
+from mindflow.db.objects.model import Model
+from mindflow.db.objects.model import ModelConfig
+from mindflow.db.objects.service import Service
+from mindflow.db.objects.service import ServiceConfig
 from mindflow.utils.enum import ExtendedEnum
 
 
 class ObjectID(ExtendedEnum):
     SERVICE = "service"
     SERVICE_CONFIG = "service_config"
     MODEL = "model"
```

### Comparing `mindflow-0.3.9/mindflow/utils/files/extract.py` & `mindflow-0.4.0/mindflow/utils/files/extract.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 Module for recursively extracting all files from a file path.
 """
-
 import logging
 import os
+from typing import List
+from typing import Union
 
-from typing import List, Union
-
-from mindflow.utils.files.git import is_within_git_repo, get_git_files
+from mindflow.utils.files.git import get_git_files
+from mindflow.utils.files.git import is_within_git_repo
 
 
-def extract_files(path: Union[str, os.PathLike]) -> List[str]:
+def extract_files(path) -> List[str]:
     """
     Extract all files from a directory.
     """
     file_paths = []
     if os.path.isfile(path):
         return [os.fspath(path)]
     if is_within_git_repo(path):
```

### Comparing `mindflow-0.3.9/mindflow/utils/files/git.py` & `mindflow-0.4.0/mindflow/utils/files/git.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Handles git related operations.
 """
 import logging
 import os
 import subprocess
-from typing import List, Union
+from typing import List
+from typing import Union
 
 
 class NotInGit(BaseException):
     """
     Raised when the given path is not within a git repository.
     """
```

### Comparing `mindflow-0.3.9/mindflow/utils/prompts.py` & `mindflow-0.4.0/mindflow/utils/prompts.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """
 This file contains the prompts that are used in the CLI.
 """
 
 GIT_DIFF_PROMPT_PREFIX = "The following is a git diff from my code repository. \
     Please thoroughly explain to me in bullet points the changes for each file. \
-        Only provide the file name with its bulleted summary and nothing else in the format: \
-            {\
-                - *file_name*,\
-                    - change1 \
-                    - change2 \
-                    - change3 \
-            }\
-        with a new line for each file and change."
+        In your response back to me, only provide the file name with its bulleted summary indented once and nothing else in the format:\n \
+            \
+            - *file_name*:\n \
+                - change1\n \
+                - change2\n \
+                - change3\n \
+            \
+        with a new line for each file and change. Your entire response should be bulleted like just mentioned with no additional text."
 INDEX_PROMPT_PREFIX = "Pretend you are a search engine trying to provide an information rich \
     yet condensed string that can serve as an index for the contents or the purpose \
     of a file. I want you to respond in as few words as possible while still conveying \
          the full content and purpose of this file."
-COMMIT_PROMPT_PREFIX = "Please provide a commit message for the following changes. Only respond with the commit message and nothing else."
+CHAT_PROMPT_PREFIX = "You are a helpful virtual assistant responding to a users query using your general knowledge and the text provided below."
+COMMIT_PROMPT_PREFIX = "Please provide a commit message for the following changes. Only respond with a single commit message and nothing else. Put the response within XML tage like <COMMIT></COMMIT>."
 PR_TITLE_PREFIX = "Please provide a title for the following pull request using this git diff summary. Only respond with the title and nothing else."
-PR_BODY_PREFIX = "Please provide a body for the following pull request using this git diff summary. I'd like it to include, bulleted summaries of \
-    changes and titles to give a coherent picture of what has changed. Only respond with the body and nothing else."
-QUERY = "Please answer the following query like a helpful virtual assistant using the context provided below: "
+PR_BODY_PREFIX = "Please provide a body for the following pull request using this git diff summary. I want you to keep it high level, and give core \
+      themes and reasons for changes. Try to include some titles and bullet points. Only respond with the body and nothing else."
+QUERY_PROMPT_PREFIX = "You are a helpful virtual assistant responding to a users query using your general knowledge and the text provided below."
+DEFAULT_CONVERSATION_SYSTEM_PROMPT = "You are a senior software engineer responding to another software engineer's chat messages regarding your codebase, make sure to be polite and helpful, and provide thorough answers with example code when necessary."
```

### Comparing `mindflow-0.3.9/mindflow.egg-info/SOURCES.txt` & `mindflow-0.4.0/mindflow.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,91 +1,100 @@
 .gitignore
 .pre-commit-config.yaml
 .pylintrc
 Dockerfile
 MANIFEST.in
+Makefile
 README.md
 docker-compose.yml
 requirements.txt
 setup.py
 mindflow/__init__.py
-mindflow/main.py
 mindflow/mypy.ini
 mindflow/settings.py
+mindflow/test.py
 mindflow.egg-info/PKG-INFO
 mindflow.egg-info/SOURCES.txt
 mindflow.egg-info/dependency_links.txt
 mindflow.egg-info/entry_points.txt
 mindflow.egg-info/requires.txt
 mindflow.egg-info/top_level.txt
-mindflow/app/__init__.py
-mindflow/app/app.py
 mindflow/cli/__init__.py
-mindflow/cli/config/__init__.py
-mindflow/cli/config/main.py
-mindflow/cli/config/menu.py
-mindflow/cli/config/questions/__init__.py
-mindflow/cli/config/questions/common/__init__.py
-mindflow/cli/config/questions/common/enums.py
-mindflow/cli/config/questions/common/questions.py
-mindflow/cli/config/questions/model/__init__.py
-mindflow/cli/config/questions/model/questions.py
-mindflow/cli/config/questions/service/__init__.py
-mindflow/cli/config/questions/service/questions.py
-mindflow/cli/new_click_cli/__init__.py
-mindflow/cli/new_click_cli/cli_main.py
-mindflow/cli/new_click_cli/commands/__init__.py
-mindflow/cli/new_click_cli/commands/ask.py
-mindflow/cli/new_click_cli/commands/commit.py
-mindflow/cli/new_click_cli/commands/config.py
-mindflow/cli/new_click_cli/commands/delete.py
-mindflow/cli/new_click_cli/commands/diff.py
-mindflow/cli/new_click_cli/commands/index.py
-mindflow/cli/new_click_cli/commands/inspect.py
-mindflow/cli/new_click_cli/commands/login.py
-mindflow/cli/new_click_cli/commands/pr.py
-mindflow/cli/new_click_cli/commands/query.py
+mindflow/cli/cli_main.py
+mindflow/cli/util.py
+mindflow/cli/commands/__init__.py
+mindflow/cli/commands/chat.py
+mindflow/cli/commands/config.py
+mindflow/cli/commands/delete.py
+mindflow/cli/commands/gen.py
+mindflow/cli/commands/index.py
+mindflow/cli/commands/inspect.py
+mindflow/cli/commands/login.py
+mindflow/cli/commands/git/__init__.py
+mindflow/cli/commands/git/add.py
+mindflow/cli/commands/git/commit.py
+mindflow/cli/commands/git/diff.py
+mindflow/cli/commands/git/mr.py
+mindflow/cli/commands/git/pr.py
+mindflow/cli/commands/git/push.py
 mindflow/core/__init__.py
-mindflow/core/ask.py
-mindflow/core/commit.py
+mindflow/core/chat.py
 mindflow/core/delete.py
-mindflow/core/diff.py
+mindflow/core/gen.py
 mindflow/core/index.py
 mindflow/core/inspect.py
 mindflow/core/login.py
-mindflow/core/pr.py
 mindflow/core/query.py
+mindflow/core/git/__init__.py
+mindflow/core/git/add.py
+mindflow/core/git/commit.py
+mindflow/core/git/diff.py
+mindflow/core/git/mr.py
+mindflow/core/git/pr.py
+mindflow/core/git/push.py
 mindflow/db/__init__.py
 mindflow/db/controller.py
 mindflow/db/utils.py
 mindflow/db/db/__init__.py
 mindflow/db/db/database.py
 mindflow/db/db/json.py
-mindflow/db/db/neo4j.py
+mindflow/db/db/pinecone.py
 mindflow/db/db/static.py
 mindflow/db/objects/__init__.py
 mindflow/db/objects/base.py
+mindflow/db/objects/conversation.py
 mindflow/db/objects/document.py
 mindflow/db/objects/mindflow_model.py
 mindflow/db/objects/model.py
 mindflow/db/objects/service.py
 mindflow/db/objects/static_definition/__init__.py
+mindflow/db/objects/static_definition/conversation.py
 mindflow/db/objects/static_definition/document.py
 mindflow/db/objects/static_definition/mind_flow_model.py
 mindflow/db/objects/static_definition/model.py
 mindflow/db/objects/static_definition/model_type.py
 mindflow/db/objects/static_definition/object.py
 mindflow/db/objects/static_definition/service.py
 mindflow/resolving/__init__.py
 mindflow/resolving/resolve.py
 mindflow/resolving/resolvers/__init__.py
 mindflow/resolving/resolvers/base_resolver.py
 mindflow/resolving/resolvers/file_resolver.py
+mindflow/unit_tests/dummy_diff.txt
+mindflow/unit_tests/test_cli.py
+mindflow/unit_tests/test_utils.py
 mindflow/utils/__init__.py
+mindflow/utils/command_parse.py
+mindflow/utils/constants.py
+mindflow/utils/diff_parser.py
 mindflow/utils/enum.py
+mindflow/utils/errors.py
+mindflow/utils/execute.py
+mindflow/utils/helpers.py
 mindflow/utils/prompt_builders.py
 mindflow/utils/prompts.py
 mindflow/utils/response.py
+mindflow/utils/token.py
 mindflow/utils/files/__init__.py
 mindflow/utils/files/extract.py
 mindflow/utils/files/git.py
 mindflow/utils/files/utf8.py
```

### Comparing `mindflow-0.3.9/setup.py` & `mindflow-0.4.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
 # get version from mindflow/__init__.py
 with open("mindflow/__init__.py", "r") as f:
     for line in f:
         if line.startswith("__version__"):
             version = line.split("=")[1].strip().strip('"')
             break
@@ -11,18 +11,23 @@
     install_requires = f.read().strip().split("\n")
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mindflow",
-    python_requires='>=3.7.1',
+    python_requires=">=3.8",
     version=version,
     py_modules=["mindflow"],
     # entry_points={"console_scripts": ["mf = mindflow.main:main"]},
-    entry_points={"console_scripts": ["mf = mindflow.cli.new_click_cli.cli_main:mindflow_cli"]},
+    entry_points={
+        "console_scripts": [
+            "mf = mindflow.cli.cli_main:mindflow_cli",
+            "mindflow = mindflow.cli.cli_main:mindflow_cli",
+        ],
+    },
     packages=find_packages(),
     install_requires=install_requires,
     description="AI-powered search engine for your code!",
     long_description=long_description,
     long_description_content_type="text/markdown",
 )
```


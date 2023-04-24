# Comparing `tmp/jupyter-lsp-2.0.1.tar.gz` & `tmp/jupyter-lsp-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter-lsp-2.0.1.tar", last modified: Tue Mar 21 15:50:17 2023, max compression
+gzip compressed data, was "jupyter-lsp-2.1.0.tar", last modified: Sun Apr 23 21:22:46 2023, max compression
```

## Comparing `jupyter-lsp-2.0.1.tar` & `jupyter-lsp-2.1.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:50:17.609524 jupyter-lsp-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-03-21 15:50:17.609524 jupyter-lsp-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:50:17.597524 jupyter-lsp-2.0.1/jupyter_lsp/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:50:17.601524 jupyter-lsp-2.0.1/jupyter_lsp/etc/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/etc/jupyter-lsp-jupyter-server.json
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/etc/jupyter-lsp-notebook.json
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10505 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/non_blocking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:50:17.601524 jupyter-lsp-2.0.1/jupyter_lsp/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/schema/schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/serverextension.py
--rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:50:17.605524 jupyter-lsp-2.0.1/jupyter_lsp/specs/
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/specs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/specs/bash_language_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:50:17.605524 jupyter-lsp-2.0.1/jupyter_lsp/specs/config/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/specs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/specs/config/bash-language-server.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    11154 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/specs/config/dockerfile-language-server-nodejs.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/specs/config/julia-language-server.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/specs/config/pyls.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    12070 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/specs/config/pylsp.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    23281 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/specs/config/pyright.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/specs/config/r-languageserver.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/specs/config/sql-language-server.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/specs/config/texlab.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/specs/config/typescript-language-server.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/specs/config/yaml-language-server.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/specs/dockerfile_language_server_nodejs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/specs/javascript_typescript_langserver.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/specs/jedi_language_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/specs/julia_language_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/specs/pyls.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/specs/pyright.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/specs/python_lsp_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/specs/r_languageserver.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/specs/sql_language_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/specs/texlab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/specs/typescript_language_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/specs/unified_language_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/specs/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/specs/vscode_css_languageserver.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/specs/vscode_html_languageserver.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/specs/vscode_json_languageserver.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/specs/yaml_language_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     7030 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/stdio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:50:17.609524 jupyter-lsp-2.0.1/jupyter_lsp/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/tests/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/tests/test_bad_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/tests/test_conf_d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/tests/test_detect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/tests/test_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/tests/test_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/tests/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/tests/test_stdio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/tests/test_virtual_documents_shadow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/trait_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/jupyter_lsp/virtual_documents_shadow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:50:17.601524 jupyter-lsp-2.0.1/jupyter_lsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-03-21 15:50:17.000000 jupyter-lsp-2.0.1/jupyter_lsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-03-21 15:50:17.000000 jupyter-lsp-2.0.1/jupyter_lsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 15:50:17.000000 jupyter-lsp-2.0.1/jupyter_lsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-03-21 15:50:17.000000 jupyter-lsp-2.0.1/jupyter_lsp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 15:50:17.000000 jupyter-lsp-2.0.1/jupyter_lsp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-21 15:50:17.000000 jupyter-lsp-2.0.1/jupyter_lsp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-21 15:50:17.000000 jupyter-lsp-2.0.1/jupyter_lsp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-03-21 15:50:17.609524 jupyter-lsp-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-03-21 15:47:08.000000 jupyter-lsp-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:22:46.203579 jupyter-lsp-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-23 21:22:46.203579 jupyter-lsp-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:22:46.195579 jupyter-lsp-2.1.0/jupyter_lsp/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/jupyter_lsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/jupyter_lsp/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/jupyter_lsp/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:22:46.199579 jupyter-lsp-2.1.0/jupyter_lsp/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/jupyter_lsp/etc/jupyter-lsp-jupyter-server.json
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/jupyter_lsp/etc/jupyter-lsp-notebook.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/jupyter_lsp/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10505 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/jupyter_lsp/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/jupyter_lsp/non_blocking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/jupyter_lsp/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:22:46.199579 jupyter-lsp-2.1.0/jupyter_lsp/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/jupyter_lsp/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8855 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/jupyter_lsp/schema/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/jupyter_lsp/serverextension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/jupyter_lsp/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:22:46.199579 jupyter-lsp-2.1.0/jupyter_lsp/specs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/bash_language_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:22:46.199579 jupyter-lsp-2.1.0/jupyter_lsp/specs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-23 21:20:14.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/config/bash-language-server.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11154 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/config/dockerfile-language-server-nodejs.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/config/julia-language-server.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/config/pyls.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12070 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/config/pylsp.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23281 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/config/pyright.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/config/r-languageserver.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/config/sql-language-server.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/config/texlab.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/config/typescript-language-server.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/config/yaml-language-server.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/dockerfile_language_server_nodejs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/javascript_typescript_langserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/jedi_language_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/julia_language_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/pyls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/pyright.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/python_lsp_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/r_languageserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/sql_language_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/texlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/typescript_language_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/unified_language_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/vscode_css_languageserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/vscode_html_languageserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/vscode_json_languageserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/specs/yaml_language_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7030 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/stdio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:22:46.203579 jupyter-lsp-2.1.0/jupyter_lsp/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/tests/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/tests/test_bad_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/tests/test_conf_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/tests/test_detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/tests/test_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/tests/test_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/tests/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/tests/test_stdio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/tests/test_virtual_documents_shadow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/trait_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/jupyter_lsp/virtual_documents_shadow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:22:46.199579 jupyter-lsp-2.1.0/jupyter_lsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-23 21:22:46.000000 jupyter-lsp-2.1.0/jupyter_lsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-04-23 21:22:46.000000 jupyter-lsp-2.1.0/jupyter_lsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 21:22:46.000000 jupyter-lsp-2.1.0/jupyter_lsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-23 21:22:46.000000 jupyter-lsp-2.1.0/jupyter_lsp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 21:22:46.000000 jupyter-lsp-2.1.0/jupyter_lsp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-23 21:22:46.000000 jupyter-lsp-2.1.0/jupyter_lsp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-23 21:22:46.000000 jupyter-lsp-2.1.0/jupyter_lsp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-23 21:22:46.203579 jupyter-lsp-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-23 21:20:15.000000 jupyter-lsp-2.1.0/setup.py
```

### Comparing `jupyter-lsp-2.0.1/LICENSE` & `jupyter-lsp-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/PKG-INFO` & `jupyter-lsp-2.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-lsp
-Version: 2.0.1
+Version: 2.1.0
 Summary: Multi-Language Server WebSocket proxy for Jupyter Notebook/Lab server
 Author: jupyter-lsp Contributors
 Author-email: project.jupyter@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/jupyter-lsp/jupyterlab-lsp/issues
 Project-URL: Documentation, https://jupyterlab-lsp.readthedocs.io/
 Project-URL: Source Code, https://github.com/jupyter-lsp/jupyterlab-lsp
```

### Comparing `jupyter-lsp-2.0.1/README.md` & `jupyter-lsp-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/handlers.py` & `jupyter-lsp-2.1.0/jupyter_lsp/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/manager.py` & `jupyter-lsp-2.1.0/jupyter_lsp/manager.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/non_blocking.py` & `jupyter-lsp-2.1.0/jupyter_lsp/non_blocking.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/paths.py` & `jupyter-lsp-2.1.0/jupyter_lsp/paths.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/schema/__init__.py` & `jupyter-lsp-2.1.0/jupyter_lsp/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/schema/schema.json` & `jupyter-lsp-2.1.0/jupyter_lsp/schema/schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999503968253969%*

 * *Differences: {"'definitions'": "{'partial-language-server-spec': {'properties': {'requires_documents_on_disk': "*

 * *                  "OrderedDict([('default', True), ('description', 'Whether to write un-saved "*

 * *                  'documents to disk in a transient `.virtual_documents` directory. Well-behaved '*

 * *                  'language servers that work against in-memory files should set this to `false`, '*

 * *                  "which will become the default in the future.'), ('type', 'boolean')])}}}"}*

```diff
@@ -154,14 +154,19 @@
                     "$ref": "#/definitions/language-list"
                 },
                 "mime_types": {
                     "$ref": "#/definitions/language-list",
                     "description": "list of MIME types supported by the language server",
                     "title": "MIME Types"
                 },
+                "requires_documents_on_disk": {
+                    "default": true,
+                    "description": "Whether to write un-saved documents to disk in a transient `.virtual_documents` directory. Well-behaved language servers that work against in-memory files should set this to `false`, which will become the default in the future.",
+                    "type": "boolean"
+                },
                 "troubleshoot": {
                     "description": "information on troubleshooting the installation or auto-detection of the language server",
                     "title": "Troubleshooting",
                     "type": "string"
                 },
                 "urls": {
                     "additionalProperties": {
```

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/serverextension.py` & `jupyter-lsp-2.1.0/jupyter_lsp/serverextension.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,20 +12,36 @@
 
 async def initialize(nbapp, virtual_documents_uri):  # pragma: no cover
     """Perform lazy initialization."""
     import concurrent.futures
 
     from .virtual_documents_shadow import setup_shadow_filesystem
 
-    manager = nbapp.language_server_manager
+    manager: LanguageServerManager = nbapp.language_server_manager
 
     with concurrent.futures.ThreadPoolExecutor() as pool:
         await nbapp.io_loop.run_in_executor(pool, manager.initialize)
 
-    setup_shadow_filesystem(virtual_documents_uri=virtual_documents_uri)
+    servers_requiring_disk_access = [
+        server_id
+        for server_id, server in manager.language_servers.items()
+        if server.get("requires_documents_on_disk", True)
+    ]
+
+    if any(servers_requiring_disk_access):
+        nbapp.log.debug(
+            "[lsp] Servers that requested virtual documents on disk: %s",
+            servers_requiring_disk_access,
+        )
+        setup_shadow_filesystem(virtual_documents_uri=virtual_documents_uri)
+    else:
+        nbapp.log.debug(
+            "[lsp] None of the installed servers require virtual documents"
+            " disabling shadow filesystem."
+        )
 
     nbapp.log.debug(
         "[lsp] The following Language Servers will be available: {}".format(
             json.dumps(manager.language_servers, indent=2, sort_keys=True)
         )
     )
```

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/session.py` & `jupyter-lsp-2.1.0/jupyter_lsp/session.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/specs/__init__.py` & `jupyter-lsp-2.1.0/jupyter_lsp/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/specs/bash_language_server.py` & `jupyter-lsp-2.1.0/jupyter_lsp/specs/bash_language_server.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/specs/config/bash-language-server.schema.json` & `jupyter-lsp-2.1.0/jupyter_lsp/specs/config/bash-language-server.schema.json`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/specs/config/dockerfile-language-server-nodejs.schema.json` & `jupyter-lsp-2.1.0/jupyter_lsp/specs/config/dockerfile-language-server-nodejs.schema.json`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/specs/config/julia-language-server.schema.json` & `jupyter-lsp-2.1.0/jupyter_lsp/specs/config/julia-language-server.schema.json`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/specs/config/pyls.schema.json` & `jupyter-lsp-2.1.0/jupyter_lsp/specs/config/pyls.schema.json`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/specs/config/pylsp.schema.json` & `jupyter-lsp-2.1.0/jupyter_lsp/specs/config/pylsp.schema.json`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/specs/config/pyright.schema.json` & `jupyter-lsp-2.1.0/jupyter_lsp/specs/config/pyright.schema.json`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/specs/config/r-languageserver.schema.json` & `jupyter-lsp-2.1.0/jupyter_lsp/specs/config/r-languageserver.schema.json`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/specs/config/sql-language-server.schema.json` & `jupyter-lsp-2.1.0/jupyter_lsp/specs/config/sql-language-server.schema.json`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/specs/config/texlab.schema.json` & `jupyter-lsp-2.1.0/jupyter_lsp/specs/config/texlab.schema.json`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/specs/config/typescript-language-server.schema.json` & `jupyter-lsp-2.1.0/jupyter_lsp/specs/config/typescript-language-server.schema.json`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/specs/config/yaml-language-server.schema.json` & `jupyter-lsp-2.1.0/jupyter_lsp/specs/config/yaml-language-server.schema.json`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/specs/dockerfile_language_server_nodejs.py` & `jupyter-lsp-2.1.0/jupyter_lsp/specs/dockerfile_language_server_nodejs.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/specs/javascript_typescript_langserver.py` & `jupyter-lsp-2.1.0/jupyter_lsp/specs/javascript_typescript_langserver.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/specs/jedi_language_server.py` & `jupyter-lsp-2.1.0/jupyter_lsp/specs/jedi_language_server.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/specs/julia_language_server.py` & `jupyter-lsp-2.1.0/jupyter_lsp/specs/julia_language_server.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/specs/pyls.py` & `jupyter-lsp-2.1.0/jupyter_lsp/specs/pyls.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/specs/pyright.py` & `jupyter-lsp-2.1.0/jupyter_lsp/specs/vscode_css_languageserver.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-from .config import load_config_schema
 from .utils import NodeModuleSpec
 
 
-class PyrightLanguageServer(NodeModuleSpec):
-    node_module = key = "pyright"
-    script = ["langserver.index.js"]
+class VSCodeCSSLanguageServer(NodeModuleSpec):
+    node_module = key = "vscode-css-languageserver-bin"
+    script = ["cssServerMain.js"]
     args = ["--stdio"]
-    languages = ["python"]
+    languages = ["css", "less", "scss"]
     spec = dict(
         display_name=key,
-        mime_types=["text/python", "text/x-ipython"],
+        mime_types=["text/x-scss", "text/css", "text/x-less"],
         urls=dict(
-            home="https://github.com/microsoft/pyright",
-            issues="https://github.com/microsoft/pyright/issues",
+            home="https://github.com/vscode-langservers/{}".format(key),
+            issues="https://github.com/vscode-langservers/{}/issues".format(key),
         ),
         install=dict(
             npm="npm install --save-dev {}".format(key),
             yarn="yarn add --dev {}".format(key),
             jlpm="jlpm add --dev {}".format(key),
         ),
-        config_schema=load_config_schema(key),
     )
```

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/specs/python_lsp_server.py` & `jupyter-lsp-2.1.0/jupyter_lsp/specs/python_lsp_server.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/specs/r_languageserver.py` & `jupyter-lsp-2.1.0/jupyter_lsp/specs/r_languageserver.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/specs/sql_language_server.py` & `jupyter-lsp-2.1.0/jupyter_lsp/specs/sql_language_server.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/specs/texlab.py` & `jupyter-lsp-2.1.0/jupyter_lsp/specs/texlab.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/specs/typescript_language_server.py` & `jupyter-lsp-2.1.0/jupyter_lsp/specs/typescript_language_server.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/specs/unified_language_server.py` & `jupyter-lsp-2.1.0/jupyter_lsp/specs/unified_language_server.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/specs/utils.py` & `jupyter-lsp-2.1.0/jupyter_lsp/specs/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/specs/vscode_css_languageserver.py` & `jupyter-lsp-2.1.0/jupyter_lsp/specs/yaml_language_server.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+from .config import load_config_schema
 from .utils import NodeModuleSpec
 
 
-class VSCodeCSSLanguageServer(NodeModuleSpec):
-    node_module = key = "vscode-css-languageserver-bin"
-    script = ["cssServerMain.js"]
+class YAMLLanguageServer(NodeModuleSpec):
+    node_module = key = "yaml-language-server"
+    script = ["bin", key]
     args = ["--stdio"]
-    languages = ["css", "less", "scss"]
+    languages = ["yaml"]
     spec = dict(
         display_name=key,
-        mime_types=["text/x-scss", "text/css", "text/x-less"],
+        mime_types=["text/x-yaml", "text/yaml"],
         urls=dict(
-            home="https://github.com/vscode-langservers/{}".format(key),
-            issues="https://github.com/vscode-langservers/{}/issues".format(key),
+            home="https://github.com/redhat-developer/{}".format(key),
+            issues="https://github.com/redhat-developer/{}/issues".format(key),
         ),
         install=dict(
             npm="npm install --save-dev {}".format(key),
             yarn="yarn add --dev {}".format(key),
             jlpm="jlpm add --dev {}".format(key),
         ),
+        config_schema=load_config_schema(key),
     )
```

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/specs/vscode_html_languageserver.py` & `jupyter-lsp-2.1.0/jupyter_lsp/specs/vscode_html_languageserver.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/specs/vscode_json_languageserver.py` & `jupyter-lsp-2.1.0/jupyter_lsp/specs/vscode_json_languageserver.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/specs/yaml_language_server.py` & `jupyter-lsp-2.1.0/jupyter_lsp/specs/pyright.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from .config import load_config_schema
 from .utils import NodeModuleSpec
 
 
-class YAMLLanguageServer(NodeModuleSpec):
-    node_module = key = "yaml-language-server"
-    script = ["bin", key]
+class PyrightLanguageServer(NodeModuleSpec):
+    node_module = key = "pyright"
+    script = ["langserver.index.js"]
     args = ["--stdio"]
-    languages = ["yaml"]
+    languages = ["python"]
     spec = dict(
         display_name=key,
-        mime_types=["text/x-yaml", "text/yaml"],
+        mime_types=["text/python", "text/x-ipython"],
         urls=dict(
-            home="https://github.com/redhat-developer/{}".format(key),
-            issues="https://github.com/redhat-developer/{}/issues".format(key),
+            home="https://github.com/microsoft/pyright",
+            issues="https://github.com/microsoft/pyright/issues",
         ),
         install=dict(
             npm="npm install --save-dev {}".format(key),
             yarn="yarn add --dev {}".format(key),
             jlpm="jlpm add --dev {}".format(key),
         ),
         config_schema=load_config_schema(key),
+        requires_documents_on_disk=False,
     )
```

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/stdio.py` & `jupyter-lsp-2.1.0/jupyter_lsp/stdio.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/tests/conftest.py` & `jupyter-lsp-2.1.0/jupyter_lsp/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/tests/test_detect.py` & `jupyter-lsp-2.1.0/jupyter_lsp/tests/test_detect.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/tests/test_extension.py` & `jupyter-lsp-2.1.0/jupyter_lsp/tests/test_extension.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/tests/test_listener.py` & `jupyter-lsp-2.1.0/jupyter_lsp/tests/test_listener.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/tests/test_paths.py` & `jupyter-lsp-2.1.0/jupyter_lsp/tests/test_paths.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/tests/test_session.py` & `jupyter-lsp-2.1.0/jupyter_lsp/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/tests/test_stdio.py` & `jupyter-lsp-2.1.0/jupyter_lsp/tests/test_stdio.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/tests/test_virtual_documents_shadow.py` & `jupyter-lsp-2.1.0/jupyter_lsp/tests/test_virtual_documents_shadow.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from pathlib import Path
+from types import SimpleNamespace
 from typing import List
 
 import pytest
 
 from ..virtual_documents_shadow import (
     EditableFile,
     ShadowFilesystemError,
@@ -86,43 +87,90 @@
 
 
 @pytest.fixture
 def shadow_path(tmpdir):
     return str(tmpdir.mkdir(".virtual_documents"))
 
 
+@pytest.fixture
+def manager():
+    return SimpleNamespace(
+        language_servers={"python-lsp-server": {"requires_documents_on_disk": True}}
+    )
+
+
 @pytest.mark.asyncio
 @pytest.mark.parametrize(
     "message_func, content, expected_content",
     [
         [did_open, "content\nof\nopened\nfile", "content\nof\nopened\nfile"],
         [did_change, [{"text": "content after change"}], "content after change"],
         [did_save_with_text, "content at save", "content at save"],
     ],
 )
-async def test_shadow(shadow_path, message_func, content, expected_content):
+async def test_shadow(shadow_path, message_func, content, expected_content, manager):
     shadow = setup_shadow_filesystem(Path(shadow_path).as_uri())
     ok_file_path = Path(shadow_path) / "test.py"
 
     message = message_func(ok_file_path.as_uri(), content)
-    result = await shadow("client", message, ["python"], None)
+    result = await shadow("client", message, "python-lsp-server", manager)
     assert isinstance(result, str)
 
-    with open(str(ok_file_path)) as f:  # str is a Python 3.5 relict
+    with open(ok_file_path) as f:
         assert f.read() == expected_content
 
 
 @pytest.mark.asyncio
-async def test_shadow_failures(shadow_path):
+async def test_no_shadow_for_well_behaved_server(
+    shadow_path,
+):
+    """We call server well behaved when it does not require a disk copy"""
+    shadow_path_for_well = Path(shadow_path) / "well"
+    shadow = setup_shadow_filesystem(Path(shadow_path_for_well).as_uri())
+    ok_file_path = Path(shadow_path_for_well) / "test.py"
+
+    manager = SimpleNamespace(
+        language_servers={"python-lsp-server": {"requires_documents_on_disk": False}}
+    )
+
+    message = did_open(ok_file_path.as_uri(), "content\nof\nopened\nfile")
+    result = await shadow("client", message, "python-lsp-server", manager)
+    # should short-circuit for well behaved server
+    assert result is None
+    # should not create the directory
+    assert not shadow_path_for_well.exists()
+
 
+@pytest.mark.asyncio
+async def test_shadow_created_for_ill_behaved_server(
+    shadow_path,
+):
+    shadow_path_for_ill = Path(shadow_path) / "ill"
+    shadow = setup_shadow_filesystem(shadow_path_for_ill.as_uri())
+    ok_file_path = Path(shadow_path_for_ill) / "test.py"
+
+    manager = SimpleNamespace(
+        language_servers={"python-lsp-server": {"requires_documents_on_disk": True}}
+    )
+
+    message = did_open(ok_file_path.as_uri(), "content\nof\nopened\nfile")
+    result = await shadow("client", message, "python-lsp-server", manager)
+    assert result is not None
+    # should create the directory at given path
+    assert shadow_path_for_ill.exists()
+    assert shadow_path_for_ill.is_dir()
+
+
+@pytest.mark.asyncio
+async def test_shadow_failures(shadow_path, manager):
     shadow = setup_shadow_filesystem(Path(shadow_path).as_uri())
     ok_file_uri = (Path(shadow_path) / "test.py").as_uri()
 
     def run_shadow(message):
-        return shadow("client", message, ["python"], None)
+        return shadow("client", message, "python-lsp-server", manager)
 
     # missing textDocument
     with pytest.raises(ShadowFilesystemError, match="Could not get textDocument from"):
         await run_shadow({"method": "textDocument/didChange"})
 
     # missing URI
     with pytest.raises(ShadowFilesystemError, match="Could not get URI from"):
```

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/trait_types.py` & `jupyter-lsp-2.1.0/jupyter_lsp/trait_types.py`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/types.py` & `jupyter-lsp-2.1.0/jupyter_lsp/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,22 @@
     Callable,
     Dict,
     List,
     Optional,
     Pattern,
     Text,
     Union,
+    cast,
 )
 
 try:
     from jupyter_server.transutils import _i18n as _
 except ImportError:  # pragma: no cover
     from jupyter_server.transutils import _
+
 from traitlets import Instance
 from traitlets import List as List_
 from traitlets import Unicode, default
 from traitlets.config import LoggingConfigurable
 
 LanguageServerSpec = Dict[Text, Any]
 LanguageServerMessage = Dict[Text, Any]
@@ -40,15 +42,15 @@
 
     class HandlerListenerCallback(Protocol):
         def __call__(
             self,
             scope: Text,
             message: LanguageServerMessage,
             language_server: Text,
-            manager: "HasListeners",
+            manager: "LanguageServerManagerAPI",
         ) -> Awaitable[None]:
             ...
 
 
 class SessionStatus(enum.Enum):
     """States in which a language server session can be"""
 
@@ -85,15 +87,15 @@
         self.method = re.compile(method) if method else None
 
     async def __call__(
         self,
         scope: Text,
         message: LanguageServerMessage,
         language_server: Text,
-        manager: "HasListeners",
+        manager: "LanguageServerManagerAPI",
     ) -> None:
         """actually dispatch the message to the listener and capture any errors"""
         try:
             await self.listener(
                 scope=scope,
                 message=message,
                 language_server=language_server,
@@ -178,27 +180,29 @@
             message = json.loads(message_str)
 
             futures = [
                 listener(
                     scope_val,
                     message=message,
                     language_server=language_server,
-                    manager=self,
+                    manager=cast("LanguageServerManagerAPI", self),
                 )
                 for listener in listeners
                 if listener.wants(message, language_server)
             ]
 
             if futures:
                 await asyncio.gather(*futures)
 
 
 class LanguageServerManagerAPI(LoggingConfigurable, HasListeners):
     """Public API that can be used for python-based spec finders and listeners"""
 
+    language_servers: KeyedLanguageServerSpecs
+
     nodejs = Unicode(help=_("path to nodejs executable")).tag(config=True)
 
     node_roots = List_([], help=_("absolute paths in which to seek node_modules")).tag(
         config=True
     )
 
     extra_node_roots = List_(
```

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp/virtual_documents_shadow.py` & `jupyter-lsp-2.1.0/jupyter_lsp/virtual_documents_shadow.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from shutil import rmtree
 
 from tornado.concurrent import run_on_executor
 from tornado.gen import convert_yielded
 
 from .manager import lsp_message_listener
 from .paths import file_uri_to_path
+from .types import LanguageServerManagerAPI
 
 # TODO: make configurable
 MAX_WORKERS = 4
 
 
 def extract_or_none(obj, path):
     for crumb in path:
@@ -97,37 +98,38 @@
 WRITE_ONE = ["textDocument/didOpen", "textDocument/didChange", "textDocument/didSave"]
 
 
 class ShadowFilesystemError(ValueError):
     """Error in the shadow file system."""
 
 
-def setup_shadow_filesystem(virtual_documents_uri):
+def setup_shadow_filesystem(virtual_documents_uri: str):
 
     if not virtual_documents_uri.startswith("file:/"):
         raise ShadowFilesystemError(  # pragma: no cover
             'Virtual documents URI has to start with "file:/", got '
             + virtual_documents_uri
         )
 
+    initialized = False
     shadow_filesystem = Path(file_uri_to_path(virtual_documents_uri))
-    # create if does no exist (so that removal does not raise)
-    shadow_filesystem.mkdir(parents=True, exist_ok=True)
-    # remove with contents
-    rmtree(str(shadow_filesystem))
-    # create again
-    shadow_filesystem.mkdir(parents=True, exist_ok=True)
 
     @lsp_message_listener("client")
     async def shadow_virtual_documents(scope, message, language_server, manager):
         """Intercept a message with document contents creating a shadow file for it.
 
         Only create the shadow file if the URI matches the virtual documents URI.
         Returns the path on filesystem where the content was stored.
         """
+        nonlocal initialized
+
+        # short-circut if language server does not require documents on disk
+        server_spec = manager.language_servers[language_server]
+        if not server_spec.get("requires_documents_on_disk", True):
+            return
 
         if not message.get("method") in WRITE_ONE:
             return
 
         document = extract_or_none(message, ["params", "textDocument"])
         if document is None:
             raise ShadowFilesystemError(
@@ -137,14 +139,24 @@
         uri = extract_or_none(document, ["uri"])
         if not uri:
             raise ShadowFilesystemError("Could not get URI from: {}".format(message))
 
         if not uri.startswith(virtual_documents_uri):
             return
 
+        # initialization (/any file system operations) delayed until needed
+        if not initialized:
+            # create if does no exist (so that removal does not raise)
+            shadow_filesystem.mkdir(parents=True, exist_ok=True)
+            # remove with contents
+            rmtree(str(shadow_filesystem))
+            # create again
+            shadow_filesystem.mkdir(parents=True, exist_ok=True)
+            initialized = True
+
         path = file_uri_to_path(uri)
         editable_file = EditableFile(path)
 
         await editable_file.read()
 
         text = extract_or_none(document, ["text"])
```

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp.egg-info/PKG-INFO` & `jupyter-lsp-2.1.0/jupyter_lsp.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-lsp
-Version: 2.0.1
+Version: 2.1.0
 Summary: Multi-Language Server WebSocket proxy for Jupyter Notebook/Lab server
 Author: jupyter-lsp Contributors
 Author-email: project.jupyter@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/jupyter-lsp/jupyterlab-lsp/issues
 Project-URL: Documentation, https://jupyterlab-lsp.readthedocs.io/
 Project-URL: Source Code, https://github.com/jupyter-lsp/jupyterlab-lsp
```

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp.egg-info/SOURCES.txt` & `jupyter-lsp-2.1.0/jupyter_lsp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/jupyter_lsp.egg-info/entry_points.txt` & `jupyter-lsp-2.1.0/jupyter_lsp.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/setup.cfg` & `jupyter-lsp-2.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `jupyter-lsp-2.0.1/setup.py` & `jupyter-lsp-2.1.0/setup.py`

 * *Files identical despite different names*


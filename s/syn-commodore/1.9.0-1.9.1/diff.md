# Comparing `tmp/syn-commodore-1.9.0.tar.gz` & `tmp/syn-commodore-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syn-commodore-1.9.0.tar", max compression
+gzip compressed data, was "syn-commodore-1.9.1.tar", max compression
```

## Comparing `syn-commodore-1.9.0.tar` & `syn-commodore-1.9.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     1504 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/LICENSE
--rw-r--r--   0        0        0     6352 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/README.md
--rw-r--r--   0        0        0      376 2022-08-30 09:18:15.319739 syn-commodore-1.9.0/commodore/__init__.py
--rw-r--r--   0        0        0      143 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/__main__.py
--rw-r--r--   0        0        0     8355 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/catalog.py
--rw-r--r--   0        0        0    34991 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/cli.py
--rw-r--r--   0        0        0     7461 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/cluster.py
--rw-r--r--   0        0        0     8779 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/compile.py
--rw-r--r--   0        0        0     6309 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/component/__init__.py
--rw-r--r--   0        0        0     9504 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/component/compile.py
--rw-r--r--   0        0        0     5738 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/component/template.py
--rw-r--r--   0        0        0    14738 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/config.py
--rw-r--r--   0        0        0      370 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/cruft/__init__.py
--rw-r--r--   0        0        0       48 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/cruft/__main__.py
--rw-r--r--   0        0        0     9466 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/cruft/_cli.py
--rw-r--r--   0        0        0      239 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/cruft/_commands/__init__.py
--rw-r--r--   0        0        0     1436 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/cruft/_commands/check.py
--rw-r--r--   0        0        0     2306 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/cruft/_commands/create.py
--rw-r--r--   0        0        0     3444 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/cruft/_commands/diff.py
--rw-r--r--   0        0        0     2271 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/cruft/_commands/link.py
--rw-r--r--   0        0        0    10378 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/cruft/_commands/update.py
--rw-r--r--   0        0        0      550 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/cruft/_commands/utils/__init__.py
--rw-r--r--   0        0        0     3699 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/cruft/_commands/utils/cookiecutter.py
--rw-r--r--   0        0        0     1335 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/cruft/_commands/utils/cruft.py
--rw-r--r--   0        0        0     2532 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/cruft/_commands/utils/diff.py
--rw-r--r--   0        0        0     5851 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/cruft/_commands/utils/generate.py
--rw-r--r--   0        0        0      576 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/cruft/_commands/utils/iohelper.py
--rw-r--r--   0        0        0      848 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/cruft/_logo.py
--rw-r--r--   0        0        0      400 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/cruft/_version.py
--rw-r--r--   0        0        0     2249 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/cruft/exceptions.py
--rw-r--r--   0        0        0     7161 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/dependency_mgmt/__init__.py
--rw-r--r--   0        0        0     2728 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/dependency_mgmt/component_library.py
--rw-r--r--   0        0        0     5033 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/dependency_mgmt/discovery.py
--rw-r--r--   0        0        0     3580 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/dependency_mgmt/jsonnet_bundler.py
--rw-r--r--   0        0        0      756 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/dependency_mgmt/tools.py
--rw-r--r--   0        0        0     3087 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/dependency_mgmt/version_parsing.py
--rw-r--r--   0        0        0     5597 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/dependency_syncer.py
--rw-r--r--   0        0        0    13400 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/dependency_templater.py
--rw-r--r--   0        0        0      643 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/filters/helm_namespace.jsonnet
--rw-r--r--   0        0        0    23594 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/gitrepo.py
--rw-r--r--   0        0        0     7321 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/helpers.py
--rw-r--r--   0        0        0     2928 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/inventory/__init__.py
--rw-r--r--   0        0        0     3765 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/inventory/lint.py
--rw-r--r--   0        0        0     1930 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/inventory/lint_dependency_specification.py
--rw-r--r--   0        0        0     1517 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/inventory/lint_deprecated_parameters.py
--rw-r--r--   0        0        0    11229 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/inventory/parameters.py
--rw-r--r--   0        0        0     2304 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/inventory/render.py
--rw-r--r--   0        0        0     1205 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/k8sobject.py
--rw-r--r--   0        0        0    12996 2022-08-30 09:17:53.383496 syn-commodore-1.9.0/commodore/lib/commodore.libjsonnet
--rw-r--r--   0        0        0     8858 2022-08-30 09:17:53.387496 syn-commodore-1.9.0/commodore/login.py
--rw-r--r--   0        0        0     3621 2022-08-30 09:17:53.387496 syn-commodore-1.9.0/commodore/multi_dependency.py
--rw-r--r--   0        0        0     2644 2022-08-30 09:17:53.387496 syn-commodore-1.9.0/commodore/package/__init__.py
--rw-r--r--   0        0        0     6977 2022-08-30 09:17:53.387496 syn-commodore-1.9.0/commodore/package/compile.py
--rw-r--r--   0        0        0     1193 2022-08-30 09:17:53.387496 syn-commodore-1.9.0/commodore/package/template.py
--rw-r--r--   0        0        0     5119 2022-08-30 09:17:53.387496 syn-commodore-1.9.0/commodore/postprocess/__init__.py
--rw-r--r--   0        0        0     2714 2022-08-30 09:17:53.387496 syn-commodore-1.9.0/commodore/postprocess/builtin_filters.py
--rw-r--r--   0        0        0     4490 2022-08-30 09:17:53.387496 syn-commodore-1.9.0/commodore/postprocess/jsonnet.py
--rw-r--r--   0        0        0     6795 2022-08-30 09:17:53.387496 syn-commodore-1.9.0/commodore/refs.py
--rw-r--r--   0        0        0     1088 2022-08-30 09:17:53.387496 syn-commodore-1.9.0/commodore/tokencache.py
--rw-r--r--   0        0        0     1918 2022-08-30 09:18:15.795745 syn-commodore-1.9.0/pyproject.toml
--rw-r--r--   0        0        0     8094 2022-08-30 09:18:16.437350 syn-commodore-1.9.0/setup.py
--rw-r--r--   0        0        0     7613 2022-08-30 09:18:16.438043 syn-commodore-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1504 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/LICENSE
+-rw-r--r--   0        0        0     6352 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/README.md
+-rw-r--r--   0        0        0      376 2022-09-30 07:26:09.103329 syn-commodore-1.9.1/commodore/__init__.py
+-rw-r--r--   0        0        0      143 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/__main__.py
+-rw-r--r--   0        0        0     8355 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/catalog.py
+-rw-r--r--   0        0        0    37004 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/cli.py
+-rw-r--r--   0        0        0     7461 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/cluster.py
+-rw-r--r--   0        0        0     8779 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/compile.py
+-rw-r--r--   0        0        0     6309 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/component/__init__.py
+-rw-r--r--   0        0        0     9504 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/component/compile.py
+-rw-r--r--   0        0        0     5738 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/component/template.py
+-rw-r--r--   0        0        0    14738 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/config.py
+-rw-r--r--   0        0        0      370 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/cruft/__init__.py
+-rw-r--r--   0        0        0       48 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/cruft/__main__.py
+-rw-r--r--   0        0        0     9466 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/cruft/_cli.py
+-rw-r--r--   0        0        0      239 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/cruft/_commands/__init__.py
+-rw-r--r--   0        0        0     1436 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/cruft/_commands/check.py
+-rw-r--r--   0        0        0     2306 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/cruft/_commands/create.py
+-rw-r--r--   0        0        0     3444 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/cruft/_commands/diff.py
+-rw-r--r--   0        0        0     2271 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/cruft/_commands/link.py
+-rw-r--r--   0        0        0    10378 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/cruft/_commands/update.py
+-rw-r--r--   0        0        0      550 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/cruft/_commands/utils/__init__.py
+-rw-r--r--   0        0        0     3699 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/cruft/_commands/utils/cookiecutter.py
+-rw-r--r--   0        0        0     1335 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/cruft/_commands/utils/cruft.py
+-rw-r--r--   0        0        0     2532 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/cruft/_commands/utils/diff.py
+-rw-r--r--   0        0        0     5851 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/cruft/_commands/utils/generate.py
+-rw-r--r--   0        0        0      576 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/cruft/_commands/utils/iohelper.py
+-rw-r--r--   0        0        0      848 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/cruft/_logo.py
+-rw-r--r--   0        0        0      400 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/cruft/_version.py
+-rw-r--r--   0        0        0     2249 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/cruft/exceptions.py
+-rw-r--r--   0        0        0     7161 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/dependency_mgmt/__init__.py
+-rw-r--r--   0        0        0     2728 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/dependency_mgmt/component_library.py
+-rw-r--r--   0        0        0     5033 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/dependency_mgmt/discovery.py
+-rw-r--r--   0        0        0     3580 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/dependency_mgmt/jsonnet_bundler.py
+-rw-r--r--   0        0        0      756 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/dependency_mgmt/tools.py
+-rw-r--r--   0        0        0     3087 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/dependency_mgmt/version_parsing.py
+-rw-r--r--   0        0        0     7269 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/dependency_syncer.py
+-rw-r--r--   0        0        0    16014 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/dependency_templater.py
+-rw-r--r--   0        0        0      643 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/filters/helm_namespace.jsonnet
+-rw-r--r--   0        0        0    24824 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/gitrepo.py
+-rw-r--r--   0        0        0     7321 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/helpers.py
+-rw-r--r--   0        0        0     2928 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/inventory/__init__.py
+-rw-r--r--   0        0        0     3765 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/inventory/lint.py
+-rw-r--r--   0        0        0     1930 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/inventory/lint_dependency_specification.py
+-rw-r--r--   0        0        0     1517 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/inventory/lint_deprecated_parameters.py
+-rw-r--r--   0        0        0    11229 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/inventory/parameters.py
+-rw-r--r--   0        0        0     2304 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/inventory/render.py
+-rw-r--r--   0        0        0     1205 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/k8sobject.py
+-rw-r--r--   0        0        0    12996 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/lib/commodore.libjsonnet
+-rw-r--r--   0        0        0     8858 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/login.py
+-rw-r--r--   0        0        0     3621 2022-09-30 07:25:47.639344 syn-commodore-1.9.1/commodore/multi_dependency.py
+-rw-r--r--   0        0        0     2644 2022-09-30 07:25:47.643344 syn-commodore-1.9.1/commodore/package/__init__.py
+-rw-r--r--   0        0        0     6977 2022-09-30 07:25:47.643344 syn-commodore-1.9.1/commodore/package/compile.py
+-rw-r--r--   0        0        0     1193 2022-09-30 07:25:47.643344 syn-commodore-1.9.1/commodore/package/template.py
+-rw-r--r--   0        0        0     5119 2022-09-30 07:25:47.643344 syn-commodore-1.9.1/commodore/postprocess/__init__.py
+-rw-r--r--   0        0        0     2714 2022-09-30 07:25:47.643344 syn-commodore-1.9.1/commodore/postprocess/builtin_filters.py
+-rw-r--r--   0        0        0     4490 2022-09-30 07:25:47.643344 syn-commodore-1.9.1/commodore/postprocess/jsonnet.py
+-rw-r--r--   0        0        0     6795 2022-09-30 07:25:47.643344 syn-commodore-1.9.1/commodore/refs.py
+-rw-r--r--   0        0        0     1088 2022-09-30 07:25:47.643344 syn-commodore-1.9.1/commodore/tokencache.py
+-rw-r--r--   0        0        0     1918 2022-09-30 07:26:09.503325 syn-commodore-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0     8098 1970-01-01 00:00:00.000000 syn-commodore-1.9.1/setup.py
+-rw-r--r--   0        0        0     7613 1970-01-01 00:00:00.000000 syn-commodore-1.9.1/PKG-INFO
```

### Comparing `syn-commodore-1.9.0/LICENSE` & `syn-commodore-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/README.md` & `syn-commodore-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/catalog.py` & `syn-commodore-1.9.1/commodore/catalog.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/cli.py` & `syn-commodore-1.9.1/commodore/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import json
 import sys
 from collections.abc import Iterable
+from datetime import timedelta
 from pathlib import Path
 from typing import Optional
 
 import click
 import yaml
 
 from dotenv import load_dotenv, find_dotenv
@@ -482,14 +483,17 @@
     remove_test_case: Iterable[str],
     commit: bool,
 ):
     """This command updates the component at COMPONENT_PATH to the latest version of the
     template which was originally used to create it, if the template version is given as
     a Git branch.
 
+    The command will never commit `.rej` or `.orig` files which result from template
+    updates which couldn't be applied cleanly.
+
     The command can also add or remove component features, based on the provided command
     line options.
     """
     config.update_verbosity(verbose)
 
     t = ComponentTemplater.from_existing(config, Path(component_path))
     if copyright_holder:
@@ -618,33 +622,55 @@
     default=False,
 )
 @click.option(
     "--pr-branch",
     "-b",
     metavar="BRANCH",
     default="template-sync",
+    show_default=True,
     type=str,
     help="Branch name to use for updates from template",
 )
 @click.option(
     "--pr-label",
     "-l",
     metavar="LABEL",
     default=[],
     multiple=True,
     help="Labels to set on the PR. Can be repeated",
 )
+@click.option(
+    "--pr-batch-size",
+    metavar="COUNT",
+    default=10,
+    type=int,
+    show_default=True,
+    help="Number of PRs to create before pausing"
+    + "Tune this parameter if your sync job hits the GitHub secondary rate limit.",
+)
+@click.option(
+    "--github-pause",
+    metavar="DURATION",
+    default=120,
+    type=int,
+    show_default=True,
+    help="Duration for which to pause (in seconds) after creating a number PRs "
+    + "(according to --pr-batch-size). "
+    + "Tune this parameter if your sync job hits the GitHub secondary rate limit.",
+)
 def component_sync(
     config: Config,
     verbose: int,
     component_list: str,
     github_token: str,
     dry_run: bool,
     pr_branch: str,
     pr_label: Iterable[str],
+    pr_batch_size: int,
+    github_pause: int,
 ):
     """This command processes all components listed in the provided `COMPONENT_LIST`
     YAML file.
 
     Currently, the command only supports updating components hosted on GitHub. The
     command expects that the YAML file contains a single document with a list of GitHub
     repositories in form `organization/repository-name`.
@@ -666,14 +692,16 @@
         config,
         Path(component_list),
         dry_run,
         pr_branch,
         pr_label,
         Component,
         ComponentTemplater,
+        pr_batch_size,
+        timedelta(seconds=github_pause),
     )
 
 
 @commodore.group(short_help="Interact with a Commodore config package")
 @verbosity
 @pass_config
 def package(config: Config, verbose: int):
@@ -827,14 +855,24 @@
     copyright_holder: Optional[str],
     golden_tests: Optional[bool],
     update_copyright_year: bool,
     additional_test_case: Iterable[str],
     remove_test_case: Iterable[str],
     commit: bool,
 ):
+    """This command updates the package at PACKAGE_PATH to the latest version of the
+    template which was originally used to create it, if the template version is given as
+    a Git branch.
+
+    The command will never commit `.rej` or `.orig` files which result from template
+    updates which couldn't be applied cleanly.
+
+    The command can also add or remove package features, based on the provided command
+    line options.
+    """
     config.update_verbosity(verbose)
     t = PackageTemplater.from_existing(config, Path(package_path))
 
     # Add provided values
     if copyright_holder:
         t.copyright_holder = copyright_holder
     if golden_tests is not None:
@@ -929,33 +967,55 @@
     default=False,
 )
 @click.option(
     "--pr-branch",
     "-b",
     metavar="BRANCH",
     default="template-sync",
+    show_default=True,
     type=str,
     help="Branch name to use for updates from template",
 )
 @click.option(
     "--pr-label",
     "-l",
     metavar="LABEL",
     default=[],
     multiple=True,
     help="Labels to set on the PR. Can be repeated",
 )
+@click.option(
+    "--pr-batch-size",
+    metavar="COUNT",
+    default=10,
+    type=int,
+    show_default=True,
+    help="Number of PRs to create before pausing"
+    + "Tune this parameter if your sync job hits the GitHub secondary rate limit.",
+)
+@click.option(
+    "--github-pause",
+    metavar="DURATION",
+    default=120,
+    type=int,
+    show_default=True,
+    help="Duration for which to pause (in seconds) after creating a number PRs "
+    + "(according to --pr-batch-size). "
+    + "Tune this parameter if your sync job hits the GitHub secondary rate limit.",
+)
 def package_sync(
     config: Config,
     verbose: int,
     package_list: str,
     github_token: str,
     dry_run: bool,
     pr_branch: str,
     pr_label: Iterable[str],
+    pr_batch_size: int,
+    github_pause: int,
 ):
     """This command processes all packages listed in the provided `PACKAGE_LIST` YAML file.
 
     Currently, the command only supports updating packages hosted on GitHub. The command
     expects that the YAML file contains a single document with a list of GitHub
     repositories in form `organization/repository-name`.
 
@@ -976,14 +1036,16 @@
         config,
         Path(package_list),
         dry_run,
         pr_branch,
         pr_label,
         Package,
         PackageTemplater,
+        pr_batch_size,
+        timedelta(seconds=github_pause),
     )
 
 
 @commodore.group(short_help="Interact with a Commodore inventory")
 @verbosity
 @pass_config
 def inventory(config: Config, verbose):
```

### Comparing `syn-commodore-1.9.0/commodore/cluster.py` & `syn-commodore-1.9.1/commodore/cluster.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/compile.py` & `syn-commodore-1.9.1/commodore/compile.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/component/__init__.py` & `syn-commodore-1.9.1/commodore/component/__init__.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/component/compile.py` & `syn-commodore-1.9.1/commodore/component/compile.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/component/template.py` & `syn-commodore-1.9.1/commodore/component/template.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/config.py` & `syn-commodore-1.9.1/commodore/config.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/cruft/_cli.py` & `syn-commodore-1.9.1/commodore/cruft/_cli.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/cruft/_commands/check.py` & `syn-commodore-1.9.1/commodore/cruft/_commands/check.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/cruft/_commands/create.py` & `syn-commodore-1.9.1/commodore/cruft/_commands/create.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/cruft/_commands/diff.py` & `syn-commodore-1.9.1/commodore/cruft/_commands/diff.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/cruft/_commands/link.py` & `syn-commodore-1.9.1/commodore/cruft/_commands/link.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/cruft/_commands/update.py` & `syn-commodore-1.9.1/commodore/cruft/_commands/update.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/cruft/_commands/utils/__init__.py` & `syn-commodore-1.9.1/commodore/cruft/_commands/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/cruft/_commands/utils/cookiecutter.py` & `syn-commodore-1.9.1/commodore/cruft/_commands/utils/cookiecutter.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/cruft/_commands/utils/cruft.py` & `syn-commodore-1.9.1/commodore/cruft/_commands/utils/cruft.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/cruft/_commands/utils/diff.py` & `syn-commodore-1.9.1/commodore/cruft/_commands/utils/diff.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/cruft/_commands/utils/generate.py` & `syn-commodore-1.9.1/commodore/cruft/_commands/utils/generate.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/cruft/_commands/utils/iohelper.py` & `syn-commodore-1.9.1/commodore/cruft/_commands/utils/iohelper.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/cruft/_logo.py` & `syn-commodore-1.9.1/commodore/cruft/_logo.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/cruft/exceptions.py` & `syn-commodore-1.9.1/commodore/cruft/exceptions.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/dependency_mgmt/__init__.py` & `syn-commodore-1.9.1/commodore/dependency_mgmt/__init__.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/dependency_mgmt/component_library.py` & `syn-commodore-1.9.1/commodore/dependency_mgmt/component_library.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/dependency_mgmt/discovery.py` & `syn-commodore-1.9.1/commodore/dependency_mgmt/discovery.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/dependency_mgmt/jsonnet_bundler.py` & `syn-commodore-1.9.1/commodore/dependency_mgmt/jsonnet_bundler.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/dependency_mgmt/tools.py` & `syn-commodore-1.9.1/commodore/dependency_mgmt/tools.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/dependency_mgmt/version_parsing.py` & `syn-commodore-1.9.1/commodore/dependency_mgmt/version_parsing.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/dependency_syncer.py` & `syn-commodore-1.9.1/commodore/dependency_syncer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
-import random
 import time
 
+from datetime import timedelta
 from pathlib import Path
 from typing import Iterable, Union, Type
 
 import click
 import git
 import github
 import yaml.parser
@@ -26,14 +26,16 @@
     config: Config,
     dependency_list: Path,
     dry_run: bool,
     pr_branch: str,
     pr_label: Iterable[str],
     deptype: Type[Union[Component, Package]],
     templater: Type[Templater],
+    pr_batch_size: int = 10,
+    pause: timedelta = timedelta(seconds=120),
 ) -> None:
     if not config.github_token:
         raise click.ClickException("Can't continue, missing GitHub API token.")
 
     deptype_str = deptype.__name__.lower()
 
     try:
@@ -45,14 +47,16 @@
             f"Expected a list in '{dependency_list}', but got {e}"
         )
     except (yaml.parser.ParserError, yaml.scanner.ScannerError):
         raise click.ClickException(f"Failed to parse YAML in '{dependency_list}'")
 
     gh = github.Github(config.github_token)
     dep_count = len(deps)
+    # Keep track of how many PRs we've created to better avoid running into rate limits
+    update_count = 0
     for i, dn in enumerate(deps, start=1):
         click.secho(f"Synchronizing {dn}", bold=True)
         _, dreponame = dn.split("/")
         dname = dreponame.replace(f"{deptype_str}-", "", 1)
 
         # Clone dependency
         try:
@@ -64,44 +68,85 @@
 
         if not (d.target_dir / ".cruft.json").is_file():
             click.echo(f" > Skipping repo {dn} which doesn't have `.cruft.json`")
             continue
 
         # Update the dependency
         t = templater.from_existing(config, d.target_dir)
-        changed = t.update(print_completion_message=False, commit=not dry_run)
+        changed = t.update(
+            print_completion_message=False,
+            commit=not dry_run,
+            ignore_template_commit=True,
+        )
 
         # Create or update PR if there were updates
-        create_or_update_pr(d, dn, gr, changed, pr_branch, pr_label, dry_run)
-        if changed and not dry_run and i < dep_count:
-            # except when processing the last dependency in the list, sleep for 1-2
-            # seconds to avoid hitting secondary rate-limits for PR creation. No
-            # need to sleep if we're not creating a PR.
-            # Without the #nosec annotations bandit warns (correctly) that
-            # `random.random()` generates weak random numbers, but since the quality
-            # of the randomness doesn't matter here, we don't need to use a more
-            # expensive RNG.
-            backoff = 1.0 + random.random()  # nosec
-            time.sleep(backoff)
+        comment = render_pr_comment(d)
+        create_or_update_pr(d, dn, gr, changed, pr_branch, pr_label, dry_run, comment)
+        if changed:
+            update_count += 1
+        if not dry_run and i < dep_count:
+            # Pause processing to avoid running into GitHub secondary rate limits, if
+            # we're not in dry run mode, and we've not yet processed the last
+            # dependency.
+            _maybe_pause(update_count, pr_batch_size, pause)
+
+
+def render_pr_comment(d: Union[Component, Package]):
+    """Render comment to add to PR if there's `.rej` files in the dependency repo after
+    applying the template update."""
+    deptype = type_name(d)
+
+    if not d.repo or not d.repo.working_tree_dir:
+        raise ValueError(f"{deptype} repo not initialized")
+
+    comment = ""
+    rej_files = [
+        fname for fname in d.repo.repo.untracked_files if fname.endswith(".rej")
+    ]
+    if len(rej_files) > 0:
+        comment = (
+            f"{deptype.capitalize()} update was only partially successful. "
+            + "Please check the PR carefully.\n\n"
+            + "Rejected patches:\n\n"
+        )
+        for fname in rej_files:
+            with open(d.repo.working_tree_dir / fname, "r", encoding="utf-8") as f:
+                comment += "```diff\n" + f.read() + "```\n"
+
+    return comment
+
+
+def _maybe_pause(update_count: int, pr_batch_size: int, pause: timedelta):
+    if update_count > 0 and update_count % pr_batch_size == 0:
+        # Pause for 2 minutes after we've created `pr_batch_size` (defaults to 10)
+        # PRs, to avoid hitting secondary rate limits for PR creation. No need to
+        # consider dependencies for which we're not creating a PR. Additionally,
+        # never sleep after processing the last dependency.
+        click.echo(
+            f" > Created or updated {pr_batch_size} PRs, "
+            + f"pausing for {pause.seconds}s to avoid secondary rate limits."
+        )
+        time.sleep(pause.seconds)
 
 
 def create_or_update_pr(
     d: Union[Component, Package],
     dn: str,
     gr: Repository,
     changed: bool,
     pr_branch: str,
     pr_label,
     dry_run: bool,
+    comment: str,
 ):
     if dry_run and changed:
         click.secho(f"Would create or update PR for {dn}", bold=True)
     elif changed:
         ensure_branch(d, pr_branch)
-        msg = ensure_pr(d, dn, gr, pr_branch, pr_label)
+        msg = ensure_pr(d, dn, gr, pr_branch, pr_label, comment)
         click.secho(msg, bold=True)
     else:
         dep_type = type_name(d)
         click.secho(f"{dep_type.capitalize()} {dn} already up-to-date", bold=True)
 
 
 def message_body(c: git.objects.commit.Commit) -> str:
@@ -133,14 +178,15 @@
 
 def ensure_pr(
     d: Union[Component, Package],
     dn: str,
     gr: Repository,
     branch_name: str,
     pr_labels: Iterable[str],
+    comment: str,
 ) -> str:
     """Create or update template sync PR."""
     deptype = type_name(d)
 
     if not d.repo:
         raise ValueError(f"{deptype} repo not initialized")
 
@@ -160,14 +206,16 @@
                 gr.default_branch,
                 branch_name,
             )
         else:
             sync_pr = [pr for pr in prs if pr.head.ref == branch_name][0]
             sync_pr.edit(body=pr_body)
         sync_pr.add_to_labels(*list(pr_labels))
+        if comment != "":
+            sync_pr.as_issue().create_comment(comment)
     except github.UnknownObjectException:
         return (
             f"Unable to {cu} PR for {dn}. "
             + "Please make sure your GitHub token has permission 'public_repo'"
         )
 
     return f"PR for {deptype} {dn} successfully {cu}d"
```

### Comparing `syn-commodore-1.9.0/commodore/dependency_templater.py` & `syn-commodore-1.9.1/commodore/dependency_templater.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,68 @@
 from __future__ import annotations
 
 import datetime
+import difflib
 import json
 import re
 import tempfile
 import shutil
 import textwrap
 
 from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import Optional, Sequence
+from typing import Optional
 
 import click
 
 from commodore.config import Config
 from commodore.cruft import create as cruft_create, update as cruft_update
-from commodore.gitrepo import GitRepo, MergeConflict
+from commodore.gitrepo import GitRepo, MergeConflict, default_difffunc
 from commodore.multi_dependency import MultiDependency
 
 SLUG_REGEX = re.compile("^[a-z][a-z0-9-]+[a-z0-9]$")
 
+REJ_IGNORE = re.compile(r"\.(orig|rej)$")
+
+
+def _ignore_cruft_json_commit_id(
+    before_text: str, after_text: str, fromfile: str = "", tofile: str = ""
+):
+    """Custom diff function which omits `.cruft.json` diffs which only differ in the
+    template commit id."""
+    before_lines = before_text.split("\n")
+    after_lines = after_text.split("\n")
+    diff_lines = difflib.unified_diff(
+        before_lines, after_lines, lineterm="", fromfile=fromfile, tofile=tofile
+    )
+    omit = False
+    if fromfile == ".cruft.json" and tofile == ".cruft.json":
+        # Compute diff without context lines for `.cruft.json` (n=0) and drop the
+        # unified diff header (first 3 lines).
+        minimal_diff = list(
+            difflib.unified_diff(
+                before_lines,
+                after_lines,
+                lineterm="",
+                fromfile=fromfile,
+                tofile=tofile,
+                n=0,
+            )
+        )[3:]
+        # If the context-less diff has exactly 2 lines and both of them start with
+        # '[-+] "commit":', we omit the diff
+        if (
+            len(minimal_diff) == 2
+            and minimal_diff[0].startswith('-  "commit":')
+            and minimal_diff[1].startswith('+  "commit":')
+        ):
+            omit = True
+    # never suppress diffs in default difffunc
+    return diff_lines, omit
+
 
 class Templater(ABC):
     config: Config
     _slug: str
     _name: Optional[str]
     github_owner: str
     copyright_holder: str
@@ -236,24 +275,14 @@
         return cases
 
     @test_cases.setter
     def test_cases(self, test_cases: list[str]):
         self._test_cases = test_cases
 
     @property
-    def additional_files(self) -> Sequence[str]:
-        return [
-            ".github",
-            ".gitignore",
-            ".*.yml",
-            ".editorconfig",
-            ".cruft.json",
-        ]
-
-    @property
     def template_commit(self) -> Optional[str]:
         cruft_json = self.target_dir / ".cruft.json"
         if not cruft_json.is_file():
             click.echo(
                 f" > {self.deptype.capitalize()} doesn't have a `.cruft.json`, "
                 + "can't determine template commit."
             )
@@ -293,48 +322,36 @@
 
         self.commit("Initial commit", amend=want_worktree)
         click.secho(
             f"{self.deptype.capitalize()} {self.name} successfully added 🎉", bold=True
         )
 
     def update(
-        self, print_completion_message: bool = True, commit: bool = True
+        self,
+        print_completion_message: bool = True,
+        commit: bool = True,
+        ignore_template_commit: bool = False,
     ) -> bool:
         if len(self.test_cases) == 0:
             raise click.ClickException(
                 f"{self.deptype.capitalize()} template doesn't support removing all test cases."
             )
         cruft_updated = cruft_update(
             self.target_dir,
             cookiecutter_input=False,
             checkout=self.template_version,
             extra_context=self.cookiecutter_args,
         )
         if not cruft_updated:
             raise click.ClickException("Update from template failed")
 
-        if not commit:
-            diff_text, updated = self.diff()
-            if updated:
-                indented = textwrap.indent(diff_text, "     ")
-                message = f" > Changes:\n{indented}"
-            else:
-                message = " > No changes."
-            click.echo(message)
-        else:
-            commit_msg = (
-                f"Update from template\n\nTemplate version: {self.template_version}"
-            )
-            if self.template_commit:
-                commit_msg += f" ({self.template_commit[:7]})"
-
-            updated = self.commit(commit_msg, init=False)
+        updated = self._commit_or_print_changes(commit, ignore_template_commit)
 
         if print_completion_message:
-            if not commit:
+            if not commit and updated:
                 click.secho(
                     " > User requested to skip committing the rendered changes."
                 )
 
             if updated:
                 click.secho(
                     f"{self.deptype.capitalize()} {self.name} successfully updated 🎉",
@@ -344,32 +361,86 @@
                 click.secho(
                     f"{self.deptype.capitalize()} {self.name} already up-to-date 🎉",
                     bold=True,
                 )
 
         return updated
 
-    def diff(self) -> tuple[str, bool]:
+    def _commit_or_print_changes(
+        self, commit: bool, ignore_template_commit: bool
+    ) -> bool:
+        """Helper for update() which either prints or commits the changes in the
+        dependency repo"""
+        if not commit:
+            diff_text, updated = self.diff(
+                ignore_template_commit=ignore_template_commit
+            )
+            if updated:
+                indented = textwrap.indent(diff_text, "     ")
+                message = f" > Changes:\n{indented}"
+            else:
+                message = " > No changes."
+            click.echo(message)
+        else:
+            commit_msg = (
+                f"Update from template\n\nTemplate version: {self.template_version}"
+            )
+            if self.template_commit:
+                commit_msg += f" ({self.template_commit[:7]})"
+
+            updated = self.commit(
+                commit_msg, init=False, ignore_template_commit=ignore_template_commit
+            )
+
+        return updated
+
+    def _stage_all(self, ignore_template_commit: bool = False) -> tuple[str, bool]:
+        """Wrapper for GitRepo.stage_all() which stages all changes for a dependency."""
         repo = GitRepo(self.repo_url, self.target_dir, force_init=False)
-        repo.stage_files(self.additional_files)
-        diff_text, changed = repo.stage_all()
+
+        diff_func = default_difffunc
+        if ignore_template_commit:
+            diff_func = _ignore_cruft_json_commit_id
+        diff_text, changed = repo.stage_all(
+            diff_func=diff_func, ignore_pattern=REJ_IGNORE
+        )
+
+        if ignore_template_commit:
+            # If we want to ignore updates which only modify the template commit id, we
+            # don't use the returned `changed` but instead singal whether there was a
+            # change by checking if the diff_text has any contents.
+            changed = len(diff_text) > 0
+
+        return diff_text, changed
+
+    def diff(self, ignore_template_commit: bool = False) -> tuple[str, bool]:
+        repo = GitRepo(self.repo_url, self.target_dir, force_init=False)
+        diff_text, changed = self._stage_all(
+            ignore_template_commit=ignore_template_commit
+        )
+
+        # When only computing the diff, we reset all staged changes
         repo.reset(working_tree=False)
         return diff_text, changed
 
-    def commit(self, msg: str, amend=False, init=True) -> bool:
+    def commit(
+        self,
+        msg: str,
+        amend: bool = False,
+        init: bool = True,
+        ignore_template_commit: bool = False,
+    ) -> bool:
         # If we're amending an existing commit, we don't want to force initialize the
         # repo.
         repo = GitRepo(self.repo_url, self.target_dir, force_init=not amend and init)
 
-        # stage_all() returns the full diff compared to the last commit. Therefore, we
-        # do stage_files() first and then stage_all(), to ensure we get the complete
-        # diff.
         try:
-            repo.stage_files(self.additional_files)
-            diff_text, changed = repo.stage_all()
+            diff_text, changed = self._stage_all(
+                ignore_template_commit=ignore_template_commit
+            )
         except MergeConflict as e:
             raise click.ClickException(
                 f"Can't commit template changes: merge error in '{e}'. "
                 + "Please resolve conflicts and commit manually."
             ) from e
 
         if changed:
```

### Comparing `syn-commodore-1.9.0/commodore/filters/helm_namespace.jsonnet` & `syn-commodore-1.9.1/commodore/filters/helm_namespace.jsonnet`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/gitrepo.py` & `syn-commodore-1.9.1/commodore/gitrepo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import difflib
 import hashlib
+import re
 import shutil
 
 from collections import namedtuple
 from collections.abc import Iterable, Sequence
 from pathlib import Path
 from typing import Optional, Protocol
 
@@ -91,15 +92,15 @@
     similarity_diff = []
     similarity_diff.append(click.style(f"--- {change.b_path}", fg="yellow"))
     similarity_diff.append(click.style(f"+++ {change.a_path}", fg="yellow"))
     similarity_diff.append(f"Renamed file, similarity index {r * 100:.2f}%")
     return similarity_diff
 
 
-def _default_difffunc(
+def default_difffunc(
     before_text: str, after_text: str, fromfile: str = "", tofile: str = ""
 ) -> tuple[Iterable[str], bool]:
     before_lines = before_text.split("\n")
     after_lines = after_text.split("\n")
     diff_lines = difflib.unified_diff(
         before_lines, after_lines, lineterm="", fromfile=fromfile, tofile=tofile
     )
@@ -535,36 +536,64 @@
         """Check for conflicts in index. Raise `MergeConflict` for the first conflict
         found."""
         for (path, blobs) in self.repo.index.unmerged_blobs().items():
             for stage, b in blobs:
                 if stage != 0:
                     raise MergeConflict(path)
 
-    def stage_all(self, diff_func: DiffFunc = _default_difffunc) -> tuple[str, bool]:
+    def _compute_changed_files(
+        self, ignore_pattern: Optional[re.Pattern]
+    ) -> tuple[list[str], list[str]]:
+        """Return a list of files to add to the index and a list of files to remove from
+        the index.
+
+        New or modified files matching `ignore_pattern` are not considered for staging.
+        The `ignore_pattern` is never applied to files to be removed."""
+        # We always want to stage untracked files. The implementation for
+        # `untracked_files` respects the repo's `.gitignore`.
+        to_add = self._repo.untracked_files
+        # We don't want to remove anything by default.
+        to_remove = []
+
+        # Determine changes to stage, separated into removals and other changes
+        changes = self._repo.index.diff(None)
+        if changes:
+            for c in changes:
+                if c.change_type == "D" or c.deleted_file:
+                    # Track removed files for `index.remove()`
+                    to_remove.append(c.b_path)
+                else:
+                    # Track changes which aren't deletions for `index.add()`
+                    to_add.append(c.a_path)
+
+        if ignore_pattern:
+            to_add = [f for f in to_add if not ignore_pattern.search(f)]
+
+        return to_add, to_remove
+
+    def stage_all(
+        self,
+        diff_func: DiffFunc = default_difffunc,
+        ignore_pattern: Optional[re.Pattern] = None,
+    ) -> tuple[str, bool]:
         """Stage all changes.
         This method currently doesn't handle hidden files correctly.
 
         This method returns a tuple containing the colorized diff of the staged changes
         and a boolean indicating whether any changes were staged.
 
         The method can raise `MergeConflict` if staged changes contain merge conflicts.
         """
-        index = self._repo.index
+        to_add, to_remove = self._compute_changed_files(ignore_pattern)
 
-        # Stage deletions
-        dels = index.diff(None)
-        if dels:
-            to_remove = []
-            for c in dels.iter_change_type("D"):
-                to_remove.append(c.b_path)
-            if len(to_remove) > 0:
-                index.remove(items=to_remove)
-
-        # Stage all remaining changes
-        index.add("*")
+        index = self._repo.index
+        if len(to_add) > 0:
+            index.add(items=to_add)
+        if len(to_remove) > 0:
+            index.remove(items=to_remove)
 
         self._check_conflicts()
 
         # Compute diff of all changes
         try:
             diff = index.diff(self._repo.head.commit)
         except ValueError:
```

### Comparing `syn-commodore-1.9.0/commodore/helpers.py` & `syn-commodore-1.9.1/commodore/helpers.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/inventory/__init__.py` & `syn-commodore-1.9.1/commodore/inventory/__init__.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/inventory/lint.py` & `syn-commodore-1.9.1/commodore/inventory/lint.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/inventory/lint_dependency_specification.py` & `syn-commodore-1.9.1/commodore/inventory/lint_dependency_specification.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/inventory/lint_deprecated_parameters.py` & `syn-commodore-1.9.1/commodore/inventory/lint_deprecated_parameters.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/inventory/parameters.py` & `syn-commodore-1.9.1/commodore/inventory/parameters.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/inventory/render.py` & `syn-commodore-1.9.1/commodore/inventory/render.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/k8sobject.py` & `syn-commodore-1.9.1/commodore/k8sobject.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/lib/commodore.libjsonnet` & `syn-commodore-1.9.1/commodore/lib/commodore.libjsonnet`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/login.py` & `syn-commodore-1.9.1/commodore/login.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/multi_dependency.py` & `syn-commodore-1.9.1/commodore/multi_dependency.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/package/__init__.py` & `syn-commodore-1.9.1/commodore/package/__init__.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/package/compile.py` & `syn-commodore-1.9.1/commodore/package/compile.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/package/template.py` & `syn-commodore-1.9.1/commodore/package/template.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/postprocess/__init__.py` & `syn-commodore-1.9.1/commodore/postprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/postprocess/builtin_filters.py` & `syn-commodore-1.9.1/commodore/postprocess/builtin_filters.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/postprocess/jsonnet.py` & `syn-commodore-1.9.1/commodore/postprocess/jsonnet.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/refs.py` & `syn-commodore-1.9.1/commodore/refs.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/commodore/tokencache.py` & `syn-commodore-1.9.1/commodore/tokencache.py`

 * *Files identical despite different names*

### Comparing `syn-commodore-1.9.0/pyproject.toml` & `syn-commodore-1.9.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "syn-commodore"
-version = "v1.9.0"
+version = "v1.9.1"
 description = "Commodore provides opinionated tenant-aware management of Kapitan inventories and templates. Commodore uses Kapitan for the heavy lifting of rendering templates and resolving a hierachical configuration structure."
 readme = "README.md"
 authors = ["VSHN AG <info@vshn.ch>"]
 license = "BSD-3-Clause"
 homepage = "https://github.com/projectsyn/commodore"
 documentation = "https://syn.tools/commodore/index.html"
 packages = [
@@ -23,38 +23,38 @@
 # Kapitan requires exactly 3.1.24
 gitpython = "3.1.24"
 # Kapitan requires exactly 2.26.0
 # We explicitly request to use chardet on python3, so Poetry doesn't update
 # chartdet to v5.
 requests = {version = "2.26.0", extras = ["use_chardet_on_py3"]}
 url-normalize = "1.4.3"
-python-dotenv = "0.20.0"
+python-dotenv = "0.21.0"
 importlib-metadata = "4.12.0"
 pyxdg = "0.28"
 # Reenable dependency cruft once our patches are merged.
 # In the meantime we add typer as a top-level dependency since Cruft depends
 # on it.
 # cruft = {branch="patched-update", git="https://github.com/projectsyn/cruft.git"}
 typer = "0.6.1"
 # Kapitan requires exactly 3.1.1
 oauthlib = "3.1.1"
 # Kapitan requires exactly 2.1.0
 pyjwt = "2.1.0"
 PyGithub = "1.55"
 
 [tool.poetry.dev-dependencies]
-tox = "3.25.1"
-pytest = "7.1.2"
+tox = "3.26.0"
+pytest = "7.1.3"
 pytest-xdist = "2.5.0"
 pytest-benchmark = "3.4.1"
 responses = "0.21.0"
-black = "22.6.0"
-pyfakefs = "4.6.3"
-pytest-cov = "3.0.0"
-pylint = "2.15.0"
+black = "22.8.0"
+pyfakefs = "4.7.0"
+pytest-cov = "4.0.0"
+pylint = "2.15.3"
 types-toml = "0.10.8"
 examples = "1.0.2"
 pytest-mock = "^3.8.2"
 
 [tool.poetry.scripts]
 commodore = 'commodore.cli:main'
 local_reveal = 'tools.tools:reveal'
```

### Comparing `syn-commodore-1.9.0/setup.py` & `syn-commodore-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,34 +20,34 @@
  'click==8.1.3',
  'cookiecutter==2.1.1',
  'gitpython==3.1.24',
  'importlib-metadata==4.12.0',
  'kapitan==0.30.0',
  'oauthlib==3.1.1',
  'pyjwt==2.1.0',
- 'python-dotenv==0.20.0',
+ 'python-dotenv==0.21.0',
  'pyxdg==0.28',
  'requests[use_chardet_on_py3]==2.26.0',
  'typer==0.6.1',
  'url-normalize==1.4.3']
 
 entry_points = \
 {'console_scripts': ['commodore = commodore.cli:main',
                      'compile = tools.tools:compile',
                      'local_reveal = tools.tools:reveal']}
 
 setup_kwargs = {
     'name': 'syn-commodore',
-    'version': '1.9.0',
+    'version': '1.9.1',
     'description': 'Commodore provides opinionated tenant-aware management of Kapitan inventories and templates. Commodore uses Kapitan for the heavy lifting of rendering templates and resolving a hierachical configuration structure.',
     'long_description': '# Project Syn: Commodore\n\n[![Docker](https://github.com/projectsyn/commodore/actions/workflows/push.yml/badge.svg)](https://github.com/projectsyn/commodore/actions/workflows/push.yml)\n[![PyPI release](https://github.com/projectsyn/commodore/actions/workflows/publish-pypi.yml/badge.svg)](https://github.com/projectsyn/commodore/actions/workflows/publish-pypi.yml)\n[![GitHub Release](https://img.shields.io/github/v/release/projectsyn/commodore.svg)](https://github.com/projectsyn/commodore/releases)\n[![PyPI Release](https://img.shields.io/pypi/v/syn-commodore?color=blue)](https://pypi.org/project/syn-commodore)\n[![Maintainability](https://api.codeclimate.com/v1/badges/abb63d489a6d6e01939d/maintainability)](https://codeclimate.com/github/projectsyn/commodore/maintainability)\n[![Test Coverage](https://api.codeclimate.com/v1/badges/abb63d489a6d6e01939d/test_coverage)](https://codeclimate.com/github/projectsyn/commodore/test_coverage)\n\nThis repository is part of Project Syn.\nFor documentation on Project Syn and this component, see https://syn.tools.\n\n\nSee [GitHub Releases](https://github.com/projectsyn/commodore/releases) for changelogs of each release version of Commodore.\n\nSee [DockerHub](https://hub.docker.com/r/projectsyn/commodore) for pre-built Docker images of Commodore.\n\nCommodore is [published on PyPI](https://pypi.org/project/syn-commodore/)\n\n## Overview\n\nCommodore provides opinionated tenant-aware management of [Kapitan](https://kapitan.dev/) inventories and templates.\nCommodore uses Kapitan for the heavy lifting of rendering templates and resolving a hierachical configuration structure.\n\nCommodore introduces the concept of a component, which is a bundle of Kapitan templates and associated Kapitan classes which describe how to render the templates.\nCommodore fetches any components that are required for a given configuration before running Kapitan, and sets up symlinks so Kapitan can find the component classes.\n\nCommodore also supports additional processing on the output of Kapitan, such as patching in the desired namespace for a Helm chart which has been rendered using `helm template`.\n\n## System Requirements\n\n* Python 3.8 - 3.10 with `python3-dev` and `python3-venv` updated\n* [jsonnet-bundler](https://github.com/jsonnet-bundler/jsonnet-bundler)\n\n## Getting started\n\n1. Recommended: create a new virtual environment\n    ```console\n    python3 -m venv venv\n    source venv/bin/activate\n    ```\n1. Install commodore from PyPI\n    ```console\n    pip install syn-commodore\n    ```\n1. <a name="getting_started_jsonnet"></a>Install jsonnet-bundler according to upstream [documentation](https://github.com/jsonnet-bundler/jsonnet-bundler#install).\n\n1. For Commodore to work, you need to run an instance of [Lieutenant](https://syn.tools/syn/tutorials/getting-started.html#_kickstart_lieutenant) somewhere\n   (locally is fine too).\n\n\n1. Setup a `.env` file to configure Commodore (don\'t use quotes):\n\n   ```shell\n   # URL of Lieutenant API\n   COMMODORE_API_URL=https://lieutenant-api.example.com/\n   # Lieutenant API token\n   COMMODORE_API_TOKEN=<my-token>\n   # Your local user ID to be used in the container (optional, defaults to root)\n   USER_ID=<your-user-id>\n   # Your username to be used in the commits (optional, defaults to your local git config)\n   COMMODORE_USERNAME=<your name>\n   # Your user email to be used in the commits (optional, defaults to your local git config)\n   COMMODORE_USERMAIL=<your email>\n   ```\n1. Run commodore\n    ```console\n    commodore\n    ```\n\n## Run Commodore with poetry\n\n### Additional System Requirements\n\n* [Poetry](https://github.com/python-poetry/poetry) 1.1.0+\n* Docker\n\n\n1. Install requirements\n\n   Install poetry according to the upstream\n   [documentation](https://github.com/python-poetry/poetry#installation).\n\n   Create the Commodore environment:\n\n    ```console\n    poetry install\n    ```\n\n    Install jsonnet-bundler according to upstream [documentation](https://github.com/jsonnet-bundler/jsonnet-bundler#install).\n\n\n1. Finish setup as described [above](#getting_started_jsonnet)\n\n1. Run Commodore\n\n   ```console\n   poetry run commodore\n   ```\n\n1. Start hacking on Commodore\n\n   ```console\n   poetry shell\n   ```\n\n   - Write a line of test code, make the test fail\n   - Write a line of application code, make the test pass\n   - Repeat\n\n   Note: Commodore uses the [Black](https://github.com/psf/black) code formatter, and its formatting is encforced by CI.\n\n1. Run linting and tests\n\n   Auto format with autopep8\n   ```console\n   poetry run autopep\n   ```\n\n   List all Tox targets\n   ```console\n   poetry run tox -lv\n   ```\n\n   Run all linting and tests\n   ```console\n   poetry run tox\n   ```\n\n   Run just a specific target\n   ```console\n   poetry run tox -e py38\n   ```\n\n\n## Run Commodore in Docker\n\n**IMPORTANT:** After checking out this project, run `mkdir -p catalog inventory dependencies` in it before running any Docker commands.\nThis will ensure the folders are writable by the current user in the context of the Docker container.\n\nA docker-compose setup enables running Commodore in a container.\nThe environment variables are picked up from the local `.env` file.\nBy default your `~/.ssh/` directory is mounted into the container and an `ssh-agent` is started.\nYou can skip starting an agent by setting the `SSH_AUTH_SOCK` env variable and mounting the socket into the container.\n\n1. Build the Docker image inside of the cloned Commodore repository:\n\n```console\ndocker-compose build\n```\n\n1. Run the built image:\n\n```console\ndocker-compose run commodore catalog compile $CLUSTER_ID\n```\n\n## Documentation\n\nDocumentation for this component is written using [Asciidoc][asciidoc] and [Antora][antora].\nIt is located in the [docs/](docs) folder.\nThe [Divio documentation structure](https://documentation.divio.com/) is used to organize its content.\n\nRun the `make docs-serve` command in the root of the project, and then browse to http://localhost:2020 to see a preview of the current state of the documentation.\n\nAfter writing the documentation, please use the `make docs-vale` command and correct any warnings raised by the tool.\n\n## Contributing and license\n\nThis library is licensed under [BSD-3-Clause](LICENSE).\nFor information about how to contribute see [CONTRIBUTING](CONTRIBUTING.md).\n\n[asciidoc]: https://asciidoctor.org/\n[antora]: https://antora.org/\n',
     'author': 'VSHN AG',
     'author_email': 'info@vshn.ch',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/projectsyn/commodore',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.8,<3.11',
 }
```

### Comparing `syn-commodore-1.9.0/PKG-INFO` & `syn-commodore-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: syn-commodore
-Version: 1.9.0
+Version: 1.9.1
 Summary: Commodore provides opinionated tenant-aware management of Kapitan inventories and templates. Commodore uses Kapitan for the heavy lifting of rendering templates and resolving a hierachical configuration structure.
 Home-page: https://github.com/projectsyn/commodore
 License: BSD-3-Clause
 Author: VSHN AG
 Author-email: info@vshn.ch
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: PyGithub (==1.55)
 Requires-Dist: click (==8.1.3)
 Requires-Dist: cookiecutter (==2.1.1)
 Requires-Dist: gitpython (==3.1.24)
 Requires-Dist: importlib-metadata (==4.12.0)
 Requires-Dist: kapitan (==0.30.0)
 Requires-Dist: oauthlib (==3.1.1)
 Requires-Dist: pyjwt (==2.1.0)
-Requires-Dist: python-dotenv (==0.20.0)
+Requires-Dist: python-dotenv (==0.21.0)
 Requires-Dist: pyxdg (==0.28)
 Requires-Dist: requests[use_chardet_on_py3] (==2.26.0)
 Requires-Dist: typer (==0.6.1)
 Requires-Dist: url-normalize (==1.4.3)
 Project-URL: Documentation, https://syn.tools/commodore/index.html
 Description-Content-Type: text/markdown
```


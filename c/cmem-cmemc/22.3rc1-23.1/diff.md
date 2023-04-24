# Comparing `tmp/cmem-cmemc-22.3rc1.tar.gz` & `tmp/cmem_cmemc-23.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmem-cmemc-22.3rc1.tar", max compression
+gzip compressed data, was "cmem_cmemc-23.1.tar", max compression
```

## Comparing `cmem-cmemc-22.3rc1.tar` & `cmem_cmemc-23.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    11357 2022-12-14 07:50:55.915913 cmem-cmemc-22.3rc1/LICENSE
--rw-r--r--   0        0        0      808 2022-12-14 07:50:55.915913 cmem-cmemc-22.3rc1/README-public.md
--rw-r--r--   0        0        0      109 2022-12-14 07:50:55.915913 cmem-cmemc-22.3rc1/cmem/__init__.py
--rw-r--r--   0        0        0       28 2022-12-14 07:50:55.915913 cmem-cmemc-22.3rc1/cmem/cmemc/__init__.py
--rw-r--r--   0        0        0     5568 2022-12-14 07:50:55.915913 cmem-cmemc-22.3rc1/cmem/cmemc/cli/__init__.py
--rw-r--r--   0        0        0     3205 2022-12-14 07:50:55.915913 cmem-cmemc-22.3rc1/cmem/cmemc/cli/commands/__init__.py
--rw-r--r--   0        0        0     5801 2022-12-14 07:50:55.915913 cmem-cmemc-22.3rc1/cmem/cmemc/cli/commands/admin.py
--rw-r--r--   0        0        0     5553 2022-12-14 07:50:55.915913 cmem-cmemc-22.3rc1/cmem/cmemc/cli/commands/config.py
--rw-r--r--   0        0        0    27473 2022-12-14 07:50:55.915913 cmem-cmemc-22.3rc1/cmem/cmemc/cli/commands/dataset.py
--rw-r--r--   0        0        0    27077 2022-12-14 07:50:55.915913 cmem-cmemc-22.3rc1/cmem/cmemc/cli/commands/graph.py
--rw-r--r--   0        0        0     7808 2022-12-16 06:47:18.010590 cmem-cmemc-22.3rc1/cmem/cmemc/cli/commands/metrics.py
--rw-r--r--   0        0        0    17603 2022-12-14 07:50:55.915913 cmem-cmemc-22.3rc1/cmem/cmemc/cli/commands/project.py
--rw-r--r--   0        0        0     6959 2022-12-16 07:05:53.548255 cmem-cmemc-22.3rc1/cmem/cmemc/cli/commands/python.py
--rw-r--r--   0        0        0    27745 2022-12-18 23:12:48.403590 cmem-cmemc-22.3rc1/cmem/cmemc/cli/commands/query.py
--rw-r--r--   0        0        0     7545 2022-12-14 07:50:55.915913 cmem-cmemc-22.3rc1/cmem/cmemc/cli/commands/resource.py
--rw-r--r--   0        0        0     8474 2022-12-14 07:50:55.915913 cmem-cmemc-22.3rc1/cmem/cmemc/cli/commands/scheduler.py
--rw-r--r--   0        0        0     6926 2022-12-14 07:50:55.915913 cmem-cmemc-22.3rc1/cmem/cmemc/cli/commands/store.py
--rw-r--r--   0        0        0    16101 2022-12-16 07:28:05.583138 cmem-cmemc-22.3rc1/cmem/cmemc/cli/commands/vocabulary.py
--rw-r--r--   0        0        0    23182 2022-12-14 07:50:55.915913 cmem-cmemc-22.3rc1/cmem/cmemc/cli/commands/workflow.py
--rw-r--r--   0        0        0     4748 2022-12-14 07:50:55.915913 cmem-cmemc-22.3rc1/cmem/cmemc/cli/commands/workspace.py
--rw-r--r--   0        0        0    36489 2022-12-16 08:04:39.125349 cmem-cmemc-22.3rc1/cmem/cmemc/cli/completion.py
--rw-r--r--   0        0        0    15558 2022-12-14 07:50:55.919913 cmem-cmemc-22.3rc1/cmem/cmemc/cli/context.py
--rw-r--r--   0        0        0      139 2022-12-14 07:50:55.919913 cmem-cmemc-22.3rc1/cmem/cmemc/cli/exceptions.py
--rw-r--r--   0        0        0       43 2022-12-14 07:50:55.919913 cmem-cmemc-22.3rc1/cmem/cmemc/cli/manual_helper/__init__.py
--rw-r--r--   0        0        0     3261 2022-12-14 07:50:55.919913 cmem-cmemc-22.3rc1/cmem/cmemc/cli/manual_helper/graph.py
--rw-r--r--   0        0        0    10965 2022-12-16 08:11:22.488987 cmem-cmemc-22.3rc1/cmem/cmemc/cli/manual_helper/multi_page.py
--rw-r--r--   0        0        0     1303 2022-12-14 07:50:55.919913 cmem-cmemc-22.3rc1/cmem/cmemc/cli/manual_helper/single_page.py
--rw-r--r--   0        0        0     8147 2022-12-16 19:01:35.767097 cmem-cmemc-22.3rc1/cmem/cmemc/cli/utils.py
--rw-r--r--   0        0        0     2107 2022-12-23 09:37:20.976321 cmem-cmemc-22.3rc1/pyproject.toml
--rw-r--r--   0        0        0     1977 1970-01-01 00:00:00.000000 cmem-cmemc-22.3rc1/setup.py
--rw-r--r--   0        0        0     2371 1970-01-01 00:00:00.000000 cmem-cmemc-22.3rc1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-01-18 07:15:37.943836 cmem_cmemc-23.1/LICENSE
+-rw-r--r--   0        0        0      808 2023-01-18 07:15:37.943900 cmem_cmemc-23.1/README-public.md
+-rw-r--r--   0        0        0      109 2023-01-18 07:15:37.944108 cmem_cmemc-23.1/cmem/__init__.py
+-rw-r--r--   0        0        0       28 2023-01-18 07:15:37.944190 cmem_cmemc-23.1/cmem/cmemc/__init__.py
+-rw-r--r--   0        0        0     5570 2023-02-14 08:14:31.716989 cmem_cmemc-23.1/cmem/cmemc/cli/__init__.py
+-rw-r--r--   0        0        0     3311 2023-02-14 08:17:24.862278 cmem_cmemc-23.1/cmem/cmemc/cli/commands/__init__.py
+-rw-r--r--   0        0        0     6709 2023-04-21 12:08:15.190979 cmem_cmemc-23.1/cmem/cmemc/cli/commands/admin.py
+-rw-r--r--   0        0        0     5562 2023-03-15 16:42:29.626951 cmem_cmemc-23.1/cmem/cmemc/cli/commands/config.py
+-rw-r--r--   0        0        0    27505 2023-04-21 06:37:45.132177 cmem_cmemc-23.1/cmem/cmemc/cli/commands/dataset.py
+-rw-r--r--   0        0        0    27110 2023-03-15 16:42:29.627797 cmem_cmemc-23.1/cmem/cmemc/cli/commands/graph.py
+-rw-r--r--   0        0        0     7808 2023-03-15 16:42:29.628159 cmem_cmemc-23.1/cmem/cmemc/cli/commands/metrics.py
+-rw-r--r--   0        0        0    17612 2023-03-15 16:42:29.628389 cmem_cmemc-23.1/cmem/cmemc/cli/commands/project.py
+-rw-r--r--   0        0        0     6948 2023-03-15 16:42:29.628590 cmem_cmemc-23.1/cmem/cmemc/cli/commands/python.py
+-rw-r--r--   0        0        0    27725 2023-03-15 16:42:29.628916 cmem_cmemc-23.1/cmem/cmemc/cli/commands/query.py
+-rw-r--r--   0        0        0     7556 2023-03-15 16:42:29.629062 cmem_cmemc-23.1/cmem/cmemc/cli/commands/resource.py
+-rw-r--r--   0        0        0     8192 2023-03-15 16:42:29.629342 cmem_cmemc-23.1/cmem/cmemc/cli/commands/scheduler.py
+-rw-r--r--   0        0        0     6961 2023-03-15 16:42:29.629976 cmem_cmemc-23.1/cmem/cmemc/cli/commands/store.py
+-rw-r--r--   0        0        0    10654 2023-02-15 15:36:55.698463 cmem_cmemc-23.1/cmem/cmemc/cli/commands/user.py
+-rw-r--r--   0        0        0    16218 2023-03-15 16:42:29.630243 cmem_cmemc-23.1/cmem/cmemc/cli/commands/vocabulary.py
+-rw-r--r--   0        0        0    21832 2023-03-15 16:42:29.630535 cmem_cmemc-23.1/cmem/cmemc/cli/commands/workflow.py
+-rw-r--r--   0        0        0     4761 2023-03-15 16:42:29.630851 cmem_cmemc-23.1/cmem/cmemc/cli/commands/workspace.py
+-rw-r--r--   0        0        0    38221 2023-04-21 06:37:45.133132 cmem_cmemc-23.1/cmem/cmemc/cli/completion.py
+-rw-r--r--   0        0        0    15648 2023-04-24 20:44:46.137043 cmem_cmemc-23.1/cmem/cmemc/cli/context.py
+-rw-r--r--   0        0        0      139 2023-01-18 07:15:37.946025 cmem_cmemc-23.1/cmem/cmemc/cli/exceptions.py
+-rw-r--r--   0        0        0       43 2023-01-18 07:15:37.946113 cmem_cmemc-23.1/cmem/cmemc/cli/manual_helper/__init__.py
+-rw-r--r--   0        0        0     3261 2023-01-18 07:15:37.946179 cmem_cmemc-23.1/cmem/cmemc/cli/manual_helper/graph.py
+-rw-r--r--   0        0        0    11053 2023-02-14 08:14:31.718408 cmem_cmemc-23.1/cmem/cmemc/cli/manual_helper/multi_page.py
+-rw-r--r--   0        0        0     1303 2023-01-18 07:15:37.946315 cmem_cmemc-23.1/cmem/cmemc/cli/manual_helper/single_page.py
+-rw-r--r--   0        0        0     8086 2023-04-24 20:44:46.137197 cmem_cmemc-23.1/cmem/cmemc/cli/utils.py
+-rw-r--r--   0        0        0     2280 2023-04-24 20:54:37.794627 cmem_cmemc-23.1/pyproject.toml
+-rw-r--r--   0        0        0     2316 1970-01-01 00:00:00.000000 cmem_cmemc-23.1/PKG-INFO
```

### Comparing `cmem-cmemc-22.3rc1/LICENSE` & `cmem_cmemc-23.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cmem-cmemc-22.3rc1/README-public.md` & `cmem_cmemc-23.1/README-public.md`

 * *Files identical despite different names*

### Comparing `cmem-cmemc-22.3rc1/cmem/cmemc/cli/__init__.py` & `cmem_cmemc-23.1/cmem/cmemc/cli/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,18 +51,18 @@
         )
 
 # set the user-agent environment for the http request headers
 os.environ["CMEM_USER_AGENT"] = f"cmemc/{CMEMC_VERSION} " \
                                 f"(Python {PYTHON_VERSION})"
 
 # https://github.com/pallets/click/blob/master/examples/complex/complex/cli.py
-CONTEXT_SETTINGS = dict(
-    auto_envvar_prefix='CMEMC',
-    help_option_names=['-h', '--help']
-)
+CONTEXT_SETTINGS = {
+    "auto_envvar_prefix": 'CMEMC',
+    "help_option_names": ['-h', '--help']
+}
 
 
 @click.group(cls=CmemcGroup, context_settings=CONTEXT_SETTINGS)
 @click.option(
     '-c', '--connection',
     type=click.STRING,
     autocompletion=completion.connections,
@@ -112,15 +112,15 @@
     Groups are colored in white; Commands which change data are colored in
     red; all other commands as well as options are colored in green.
 
     Please also have a look at the cmemc online documentation:
 
                         https://eccenca.com/go/cmemc
 
-    cmemc is © 2022 eccenca GmbH, licensed under the Apache License 2.0.
+    cmemc is © 2023 eccenca GmbH, licensed under the Apache License 2.0.
     """
     ctx.obj = CONTEXT
     # hidden feature: 'CMEMC_MANUAL=true cmemc -q config list' will output
     #     the whole markdown manual
     if os.getenv("CMEMC_MANUAL_DIR"):
         create_multi_page_documentation(ctx, os.getenv('CMEMC_MANUAL_DIR'))
         ctx.exit()
```

### Comparing `cmem-cmemc-22.3rc1/cmem/cmemc/cli/commands/__init__.py` & `cmem_cmemc-23.1/cmem/cmemc/cli/commands/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         kwargs.setdefault("help_options_color", COLOR_FOR_OPTIONS)
         kwargs.setdefault(
             "help_options_custom_colors",
             {
                 "bootstrap": COLOR_FOR_WRITING_COMMANDS,
                 "showcase": COLOR_FOR_WRITING_COMMANDS,
                 "delete": COLOR_FOR_WRITING_COMMANDS,
+                "password": COLOR_FOR_WRITING_COMMANDS,
                 "upload": COLOR_FOR_WRITING_COMMANDS,
                 "import": COLOR_FOR_WRITING_COMMANDS,
                 "create": COLOR_FOR_WRITING_COMMANDS,
                 "enable": COLOR_FOR_WRITING_COMMANDS,
                 "disable": COLOR_FOR_WRITING_COMMANDS,
                 "execute": COLOR_FOR_WRITING_COMMANDS,
                 "replay": COLOR_FOR_WRITING_COMMANDS,
@@ -39,14 +40,15 @@
                 "install": COLOR_FOR_WRITING_COMMANDS,
                 "uninstall": COLOR_FOR_WRITING_COMMANDS,
                 "reload": COLOR_FOR_WRITING_COMMANDS,
                 "update": COLOR_FOR_WRITING_COMMANDS,
                 "eval": COLOR_FOR_WRITING_COMMANDS,
                 "cancel": COLOR_FOR_WRITING_COMMANDS,
                 "admin": COLOR_FOR_COMMAND_GROUPS,
+                "user": COLOR_FOR_COMMAND_GROUPS,
                 "store": COLOR_FOR_COMMAND_GROUPS,
                 "metrics": COLOR_FOR_COMMAND_GROUPS,
                 "config": COLOR_FOR_COMMAND_GROUPS,
                 "dataset": COLOR_FOR_COMMAND_GROUPS,
                 "graph": COLOR_FOR_COMMAND_GROUPS,
                 "project": COLOR_FOR_COMMAND_GROUPS,
                 "query": COLOR_FOR_COMMAND_GROUPS,
```

### Comparing `cmem-cmemc-22.3rc1/cmem/cmemc/cli/commands/admin.py` & `cmem_cmemc-23.1/cmem/cmemc/cli/commands/admin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """admin commands for cmem command line interface."""
-import sys
-
 import click
 
 import jwt
 
 from cmem.cmemc.cli import completion
+from cmem.cmemc.cli.commands.user import user
 from cmem.cmemc.cli.context import ApplicationContext
 from cmem.cmemc.cli.utils import struct_to_table
 from cmem.cmempy.api import (
     get_access_token, get_token
 )
 from cmem.cmemc.cli.commands import CmemcCommand, CmemcGroup
 from cmem.cmemc.cli.commands.metrics import metrics
@@ -24,66 +23,86 @@
     autocompletion=completion.status_keys,
     help="Get only specific key(s) from the status / info output. There are "
          "two special keys available: 'all' will list all available keys in "
          "the table, 'overall.healthy' with result in  UP in case all "
          "health flags are UP as well (otherwise DOWN)."
 )
 @click.option(
+    "--exit-1",
+    type=click.Choice(["never", "error", "always"]),
+    default="never",
+    show_default=True,
+    help="Specify, when this command returns with exit code 1. Available options are "
+         "'never' (exit 0 on errors and warnings), "
+         "'error' (exit 1 on errors, exit 0 on warnings), "
+         "'always' (exit 1 on errors and warnings)."
+)
+@click.option(
     "--enforce-table",
     is_flag=True,
     help="A single value with --key will be returned as plain text instead "
          "of a table with one row and the header. This default behaviour "
          "allows for more easy integration with scripts. This flag enforces "
          "the use of tabular output, even for single row tables."
 )
 @click.option(
     "--raw",
     is_flag=True,
     help="Outputs combined raw JSON output of the health/info endpoints."
 )
 @click.pass_obj
-def status_command(app: ApplicationContext, key, enforce_table, raw):
+def status_command(app: ApplicationContext, key, exit_1, enforce_table, raw):
     """Output health and version information.
 
     This command outputs version and health information of the
-    selected deployment. If the version information can not be retrieved,
-    UNKNOWN shown.
+    selected deployment. If the version information cannot be retrieved,
+    UNKNOWN is shown.
 
-    In addition to that, this command warns you if the
-    target version of your cmemc client is newer than the version of your
-    backend and if the ShapeCatalog has a different version then your
-    DataPlatform component.
+    Additionally, this command warns you if the target version of your
+    cmemc client is newer than the version of your backend and if the
+    ShapeCatalog has a different version than your DataPlatform
+    component.
 
     To get status information of all configured
     deployments use this command in combination with parallel.
 
     Example: cmemc config list | parallel --ctag cmemc -c {} admin status
     """
     _ = get_complete_status_info()
     if "error" in _["di"]:
         app.echo_debug(_["di"]["error"])
     if "error" in _["dp"]:
         app.echo_debug(_["dp"]["error"])
     if "error" in _["dm"]:
         app.echo_debug(_["dm"]["error"])
+    basic_status = (
+        _["dp"]["healthy"], _["di"]["healthy"], _["dm"]["healthy"],
+        _["shapes"]["healthy"], _["store"]["healthy"]
+    )
+    if exit_1 in ("always", "error")\
+            and ("DOWN" in basic_status or "UNKNOWN" in basic_status):
+        raise ValueError(
+            f"One or more major status flags are DOWN or UNKNOWN: {repr(_)}",
+        )
     if raw:
         app.echo_info_json(_)
         return
     if key:
         table = [
             line for line
             in struct_to_table(_)
             if line[0].startswith(key) or key == "all"
         ]
         if len(table) == 1 and not enforce_table:
             app.echo_info(table[0][1])
             return
         if len(table) == 0:
-            app.echo_error(f"No values for key(s) {key}.")
-            sys.exit(1)
+            raise ValueError(
+                f"No values for key(s): {key}"
+            )
         app.echo_info_table(
             table,
             headers=["Key", "Value"],
             sort_column=0
         )
         return
     table = [
@@ -96,18 +115,19 @@
     app.echo_info_table(
         table,
         headers=["Component", "Version", "Status"],
         sort_column=0
     )
     app.check_versions()
     if _["shapes"]["version"] not in (_["dp"]["version"], "UNKNOWN"):
-        app.echo_warning(
-            "Your ShapeCatalog version does not match your DataPlatform "
-            "version. Please consider updating your bootstrap data."
-        )
+        output = "Your ShapeCatalog version does not match your DataPlatform "\
+                 "version. Please consider updating your bootstrap data."
+        if exit_1 == "always":
+            raise ValueError(output)
+        app.echo_warning(output)
 
 
 @click.command(cls=CmemcCommand, name="token")
 @click.option(
     "--raw",
     is_flag=True,
     help="Outputs raw JSON. Note that this option will always try to fetch "
@@ -126,16 +146,16 @@
 
     This command can be used to check for correct authentication as well as
     to use the token with wget / curl or similar standard tools:
 
     Example: curl -H "Authorization: Bearer $(cmemc -c my admin token)"
     $(cmemc -c my config get DP_API_ENDPOINT)/api/custom/slug
 
-    Please be aware that this command can reveal secrets, which you do not
-    want to have in log files or on the screen.
+    Please be aware that this command can reveal secrets which you might
+    not want to be present in log files or on the screen.
     """
     # Note:
     # - get_access_token returns the token string which is maybe from conf
     # - get_token fetches a new token incl. envelope from keycloak
 
     if decode:
         token = get_access_token()
@@ -167,7 +187,8 @@
 
 
 admin.add_command(status_command)
 admin.add_command(token_command)
 admin.add_command(metrics)
 admin.add_command(workspace)
 admin.add_command(store)
+admin.add_command(user)
```

### Comparing `cmem-cmemc-22.3rc1/cmem/cmemc/cli/commands/config.py` & `cmem_cmemc-23.1/cmem/cmemc/cli/commands/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,24 +68,24 @@
     app.echo_info(str(value))
 
 
 @click.command(cls=CmemcCommand, name="eval")
 @click.option(
     "--unset",
     is_flag=True,
-    help="Instead of export all configuration keys, "
-         "this option will unset all key."
+    help="Instead of exporting all configuration keys, "
+         "this option will unset all keys."
 )
 @click.pass_obj
 def eval_command(app, unset):
     """Export all configuration values of a configuration for evaluation.
 
-    The output of this command is suitable to be used by a shells `eval`
+    The output of this command is suitable to be used by a shell's `eval`
     command. It will output the complete configuration as `export key="value"`
-    statements. This allows for preparation of a shell environment.
+    statements, which allow for the preparation of a shell environment.
 
     Example: eval $(cmemc -c my config eval)
 
     Warning: Please be aware that credential details are shown in cleartext
     with this command.
     """
     for key in sorted(KNOWN_CONFIG_KEYS):
```

### Comparing `cmem-cmemc-22.3rc1/cmem/cmemc/cli/commands/dataset.py` & `cmem_cmemc-23.1/cmem/cmemc/cli/commands/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,20 +30,20 @@
 from cmem.cmempy.workspace import (
     get_task_plugin_description,
     get_task_plugins
 )
 
 DATASET_FILTER_TYPES = sorted(['project', 'regex', 'tag', 'type'])
 DATASET_LIST_FILTER_HELP_TEXT = (
-    "List datasets based on meta data. First parameter --filter"
-    f" CHOICE can be one of {str(DATASET_FILTER_TYPES)}."
-    " The second parameter is based on CHOICE."
+    "Filter datasets based on metadata. First parameter"
+    f" can be one of the following values: {', '.join(DATASET_FILTER_TYPES)}."
+    " The options for the second parameter depend on the first parameter."
 )
 DATASET_DELETE_FILTER_HELP_TEXT = (
-    "Delete datasets based on meta data. First parameter --filter"
+    "Delete datasets based on metadata. First parameter --filter"
     f" CHOICE can be one of {str(DATASET_FILTER_TYPES)}."
     " The second parameter is based on CHOICE."
 )
 
 
 def _get_dataset_tag_labels(dataset_) -> list:
     """Output a list of tag labels from a single dataset."""
@@ -390,28 +390,28 @@
     multiple=True,
     autocompletion=completion.dataset_list_filter,
     help=DATASET_LIST_FILTER_HELP_TEXT,
 )
 @click.option(
     "--raw",
     is_flag=True,
-    help="Outputs raw JSON objects of dataset search API response."
+    help="Outputs raw JSON objects of the dataset search API response."
 )
 @click.option(
     "--id-only",
     is_flag=True,
-    help="Lists only dataset identifier and no labels or other meta data. "
-         "This is useful for piping the ids into other cmemc commands."
+    help="Lists only dataset IDs and no labels or other metadata. "
+         "This is useful for piping the IDs into other cmemc commands."
 )
 @click.pass_obj
 def list_command(app: ApplicationContext, filter_, raw, id_only):
     """List available datasets.
 
-    Outputs a list of datasets IDs which can be used as reference for
-    the dataset create and delete commands.
+    Output and filter a list of available datasets. Each dataset is listed
+    with its ID, type and label.
     """
     datasets = list_items(item_type="dataset")["results"]
     for _ in filter_:
         filter_type, filter_name = _
         datasets = _get_datasets_filtered(datasets, filter_type, filter_name)
 
     if raw:
@@ -536,15 +536,15 @@
         writable=True
     )
 )
 @click.option(
     "--replace",
     is_flag=True,
     help="Replace existing files. This is a dangerous option, "
-         "so use it with care.",
+         "so use it with care!",
 )
 @click.pass_obj
 def download_command(app, dataset_id, output_path, replace):
     """Download the resource file of a dataset.
 
     This command downloads the file resource of a dataset to your local
     file system or to standard out (`-`).
@@ -608,18 +608,18 @@
 )
 @click.pass_obj
 def upload_command(app, dataset_id, input_path):
     """Upload a resource file to a dataset.
 
     This command uploads a file to a dataset.
     The content of the uploaded file replaces the remote file resource.
-    The name of the remote file resource is not changed.
+    The name of the remote file resource will not be changed.
 
     Warning: If the remote file resource is used in more than one dataset,
-    the other datasets are also affected by this command.
+    all of these datasets are affected by this command.
 
     Warning: The content of the uploaded file is not tested, so uploading
     a JSON file to an XML dataset will result in errors.
 
     Note: Datasets can be listed by using the `dataset list` command.
 
     Example: cmemc dataset upload cmem:my-dataset new-file.csv
@@ -742,18 +742,18 @@
         project_id, dataset_id, dataset_type, parameter,
         help_parameter, help_types
 ):
     """Create a dataset.
 
     Datasets are created in projects and can have associated file
     resources. Each dataset has a type (such as `csv`) and a list of
-    parameter which can change or specify the dataset behaviour.
+    parameters which can alter or specify the dataset behaviour.
 
-    To get more information on possible dataset types and parameter on these
-    types, use the --help-types and --help-parameter options.
+    To get more information about available dataset types and associated
+    parameters, use the --help-types and --help-parameter options.
 
     Example: cmemc dataset create --project my-project --type csv my-file.csv
     """
     if help_types:
         _show_type_list(app)
         return
 
@@ -858,17 +858,17 @@
 @click.group(cls=CmemcGroup)
 def dataset():
     """List, create, delete, inspect, up-/download or open datasets.
 
     This command group allows for managing workspace datasets as well as
     dataset file resources. Datasets can be created and deleted.
     File resources can be uploaded and downloaded.
-    Details of dataset parameter can be listed with inspect.
+    Details of dataset parameters can be listed with inspect.
 
-    Datasets are identified with a combined key of the PROJECT_ID and
+    Datasets are identified by a combined key of the PROJECT_ID and
     a DATASET_ID (e.g: `my-project:my-dataset`).
 
     Note: To get a list of existing datasets, execute the `dataset list`
     command or use tab-completion.
     """
```

### Comparing `cmem-cmemc-22.3rc1/cmem/cmemc/cli/commands/graph.py` & `cmem_cmemc-23.1/cmem/cmemc/cli/commands/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -359,15 +359,15 @@
     is_flag=True,
     help="Outputs raw JSON of the graph importTree API response."
 )
 @click.option(
     "--id-only",
     is_flag=True,
     help="Lists only graph identifier (IRIs) and no labels or other "
-         "meta data. This is useful for piping the IRIs into other commands. "
+         "metadata. This is useful for piping the IRIs into other commands. "
          "The output with this option is a sorted, flat, de-duplicated list "
          "of existing graphs."
 )
 @click.argument(
     "iris",
     nargs=-1,
     type=click.STRING,
@@ -444,15 +444,15 @@
     is_flag=True,
     help="Outputs raw JSON of the graphs list API response."
 )
 @click.option(
     "--id-only",
     is_flag=True,
     help="Lists only graph identifier (IRIs) and no labels or other "
-         "meta data. This is useful for piping the IRIs into other commands."
+         "metadata. This is useful for piping the IRIs into other commands."
 )
 @click.option(
     "--filter", "filter_",
     type=click.Tuple([
         click.Choice(["access", 'imported-by']),
         str
     ]),
@@ -566,15 +566,15 @@
     nargs=-1,
     type=click.STRING,
     autocompletion=completion.graph_uris
 )
 @click.pass_obj
 def export_command(
         app, all_, include_imports, create_catalog,
-        output_dir, output_file, template, mime_type, iris
+        output_dir, output_file, template, mime_type, iris: tuple[str, ...]
 ):
     """Export graph(s) as NTriples to stdout (-), file or directory.
 
     In case of file export, data from all selected graphs will be concatenated
     in one file.
     In case of directory export, .graph and .ttl files will be created
     for each graph.
@@ -604,15 +604,15 @@
                 os.path.join(output_dir, _names[iri])
             )
             graph_file_name = triple_file_name + ".graph"
             # output directory is created lazy
             Path(
                 os.path.dirname(triple_file_name)
             ).mkdir(parents=True, exist_ok=True)
-            # create and write the .ttl.graph meta data file
+            # create and write the .ttl.graph metadata file
             graph_file = click.open_file(graph_file_name, "w")
             graph_file.write(iri + "\n")
             _get_graph_to_file(
                 iri, triple_file_name,
                 app,
                 numbers=(current, count),
                 mime_type=mime_type
@@ -669,21 +669,21 @@
 @click.argument(
     "iri",
     type=click.STRING,
     required=False,
     autocompletion=completion.graph_uris
 )
 @click.pass_obj
-def import_command(app, input_path, replace, skip_existing, iri):
+def import_command(app, input_path, replace, skip_existing, iri: tuple[str, ...]):
     """Import graph(s) to the store.
 
-    If input is a directory, it scans for file-pairs such as `xxx.ttl` and
-    `xxx.ttl.graph` where `xxx.ttl` is the actual triples file and
-    `xxx.ttl.graph` contains the graph IRI as one string:
-    `https://mygraph.de/xxx/`.
+    If input is a directory, it scans for file-pairs such as `xyz.ttl` and
+    `xyz.ttl.graph` where `xyz.ttl` is the actual triples file and
+    `xyz.ttl.graph` contains the graph IRI as one string:
+    `https://mygraph.de/xyz/`.
 
     If input is a file, content will be uploaded to IRI.
     If --replace is set, the data will be overwritten,
     if not, it will be added.
     """
     # is an array of tuples like this [('path/to/triple.file', 'graph IRI')]
     if replace and skip_existing:
@@ -751,15 +751,15 @@
 @click.argument(
     "iris",
     nargs=-1,
     type=click.STRING,
     autocompletion=completion.writable_graph_uris
 )
 @click.pass_obj
-def delete_command(app, all_, include_imports, iris):
+def delete_command(app, all_, include_imports, iris: tuple[str, ...]):
     """Delete graph(s) from the store."""
     graphs = get_graphs_as_dict(writeable=True, readonly=False)
     iris = _check_and_extend_exported_graphs(
         iris, all_, include_imports, graphs
     )
 
     count: int = len(iris)
@@ -806,29 +806,27 @@
 @click.argument(
     "iris",
     nargs=-1,
     type=click.STRING,
     autocompletion=completion.graph_uris
 )
 @click.pass_obj
-def count_command(app, all_, summarize, iris):
+def count_command(app, all_, summarize, iris: tuple[str, ...]):
     """Count triples in graph(s).
 
     This command lists graphs with their triple count.
-    Counts are done without following imported graphs.
+    Counts do not inlude imported graphs.
     """
     if iris == () and not all_:
         raise ValueError("Either specify at least one graph IRI "
                          + "or use the --all option to count all graphs.")
     if all_:
         # in case --all is given,
         # list of graphs is filled with all available graph IRIs
-        iris = (
-            [iri["iri"] for iri in get_graphs()]
-        )
+        iris = tuple(iri["iri"] for iri in get_graphs())
 
     count: int
     overall_sum: int = 0
     current: int = 1
     for iri in iris:
         count = count_graph(iri)
         overall_sum = overall_sum + count
```

### Comparing `cmem-cmemc-22.3rc1/cmem/cmemc/cli/commands/metrics.py` & `cmem_cmemc-23.1/cmem/cmemc/cli/commands/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
     help="Outputs raw JSON of the table data."
 )
 @click.pass_obj
 def inspect_command(app, metric_id, job_id, raw):
     """Inspect a metric.
 
     This command outputs the data of a metric.
-    The first table includes basic meta data about the metric.
+    The first table includes basic metadata about the metric.
     The second table includes sample labels and values.
     """
     family = metrics_get_family(job_id, metric_id)
     if raw:
         app.echo_info_json(
             {
                 "family": family.__dict__,
@@ -240,15 +240,15 @@
 @click.group(cls=CmemcGroup)
 def metrics():
     """List and get metrics.
 
     This command group consists of commands for reading and listing
     internal monitoring metrics of eccenca Corporate Memory. A
     deployment consists of multiple jobs (e.g. DP, DI), which provide
-    multiple metric families on an endpoint.
+    multiple metric families for an endpoint.
 
     Each metric family can consist of different samples identified by
     labels with a name and a value (dimensions). A metric has a specific
     type (counter, gauge, summary and histogram) and additional metadata.
 
     Please have a look at https://prometheus.io/docs/concepts/data_model/
     for further details.
```

### Comparing `cmem-cmemc-22.3rc1/cmem/cmemc/cli/commands/project.py` & `cmem_cmemc-23.1/cmem/cmemc/cli/commands/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 @click.pass_obj
 def open_command(app, project_ids):
     """Open projects in the browser.
 
     With this command, you can open a project in the workspace in
     your browser to change them.
 
-    The command accepts multiple projects IDs which results in
+    The command accepts multiple project IDs which results in
     opening multiple browser tabs.
     """
     projects = get_projects()
     for _ in project_ids:
         if _ not in (p["name"] for p in projects):
             raise ValueError(f"Project '{_}' not found.")
         open_project_uri = f"{get_di_api_endpoint()}/workbench/projects/{_}"
@@ -89,15 +89,15 @@
     is_flag=True,
     help="Outputs raw JSON."
 )
 @click.option(
     "--id-only",
     is_flag=True,
     help="Lists only project identifier and no labels or other "
-         "meta data. This is useful for piping the IDs into other commands."
+         "metadata. This is useful for piping the IDs into other commands."
 )
 @click.pass_obj
 def list_command(app, raw, id_only):
     """List available projects.
 
     Outputs a list of project IDs which can be used as reference for
     the project create, delete, export and import commands.
@@ -138,19 +138,20 @@
     type=click.STRING,
     autocompletion=completion.project_ids
 )
 @click.pass_obj
 def delete_command(app, all_, project_ids):
     """Delete projects.
 
-    This deletes existing data integration projects from Corporate Memory.
+    This command deletes existing data integration projects from Corporate
+    Memory.
 
     Warning: Projects will be deleted without prompting!
 
-    Note: Projects can be listed by using the `project list` command.
+    Note: Projects can be listed with the `project list` command.
     """
     all_projects = get_projects()
     if project_ids == () and not all_:
         raise ValueError("Either specify at least one project ID "
                          + "or use the --all option to delete all projects.")
     if all_:
         # in case --all is given, a list of project is fetched
@@ -184,15 +185,15 @@
     required=True,
     type=click.STRING
 )
 @click.pass_obj
 def create_command(app, project_ids):
     """Create projects.
 
-    This creates one or more new projects.
+    This command creates one or more new projects.
     Existing projects will not be overwritten.
 
     Note: Projects can be listed by using the `project list` command.
     """
     # avoid double creation
     project_ids = list(set(project_ids))
 
@@ -289,16 +290,16 @@
         template, output_dir, extract, help_types):
     """Export projects to files.
 
     Projects can be exported with different export formats.
     The default type is a zip archive which includes metadata as well
     as dataset resources.
     If more than one project is exported, a file is created for each project.
-    By default, these files are created in the current directory and with
-    a descriptive name (see --template option default).
+    By default, these files are created in the current directory with a
+    descriptive name (see --template option default).
 
     Note: Projects can be listed by using the `project list` command.
 
     You can use the template string to create subdirectories.
 
     Example: cmemc config list | parallel -I% cmemc -c % project export --all
     -t "dump/{{connection}}/{{date}}-{{id}}.project"
@@ -493,15 +494,15 @@
     autocompletion=completion.project_ids
 )
 @click.pass_obj
 def reload_command(app, all_, project_ids):
     """Reload projects from the workspace provider.
 
     This command reloads all tasks of a project from the workspace provider.
-    This is the same as the `workspace reload` command, but for a
+    This is similar to the `workspace reload` command, but for a
     single project only.
 
     Note: You need this in case you changed project data externally or loaded
     a project which uses plugins which are not installed yet.
     In this case, install the plugin(s) and reload the project afterwards.
 
     Warning: Depending on the size your datasets esp. your Knowledge Graphs,
```

### Comparing `cmem-cmemc-22.3rc1/cmem/cmemc/cli/commands/python.py` & `cmem_cmemc-23.1/cmem/cmemc/cli/commands/python.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,22 +36,21 @@
         dir_okay=False
     )
 )
 @click.pass_obj
 def install_command(app: ApplicationContext, package):
     """Install a python package to the workspace.
 
-    This command is basically a `pip install` in the remote python
+    This command is essentially a `pip install` in the remote python
     environment.
 
     You can install a package by uploading a source distribution
-    .tar.gz file, or by uploading a build distribution .whl file, or by
-    specifying a package name, more precisely, a pip requirement
-    specifier with a package name available on pypi.org
-    (e.g. `requests==2.27.1`).
+    .tar.gz file, by uploading a build distribution .whl file, or by
+    specifying a package name, i.e., a pip requirement specifier with a
+    package name available on pypi.org (e.g. `requests==2.27.1`).
     """
     app.echo_info(
         f"Install package {package} ... ",
         nl=False
     )
     try:
         response = install_package_by_file(package_file=package)
@@ -82,15 +81,15 @@
     "PACKAGE_NAME",
     autocompletion=completion.installed_package_names
 )
 @click.pass_obj
 def uninstall_command(app: ApplicationContext, package_name):
     """Uninstall a python package from the workspace.
 
-    This command is basically a `pip uninstall` in the remote
+    This command is essentially a `pip uninstall` in the remote
     python environment.
     """
     app.echo_info(
         f"Uninstall package {package_name} ... ",
         nl=False
     )
     packages = list_packages()
@@ -123,15 +122,15 @@
     help="Lists only package identifier. "
          "This is useful for piping the IDs into other commands."
 )
 @click.pass_obj
 def list_command(app: ApplicationContext, raw, id_only):
     """List installed python packages.
 
-    This command is basically a `pip list` in the remote python environment.
+    This command is essentially a `pip list` in the remote python environment.
 
     It outputs a table of python package identifiers with version information.
     """
     packages = list_packages()
     if raw:
         app.echo_info_json(packages)
         return
```

### Comparing `cmem-cmemc-22.3rc1/cmem/cmemc/cli/commands/query.py` & `cmem_cmemc-23.1/cmem/cmemc/cli/commands/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 import re
 import sys
 from hashlib import sha1
 from shutil import get_terminal_size
 from json import JSONDecodeError, load
 from time import sleep, time
-from typing import Dict, List
+from typing import Dict, List, Optional
 from uuid import uuid4
 
 import click
 
 from requests import HTTPError
 
 from cmem.cmemc.cli import completion
@@ -46,15 +46,15 @@
     total_duration: int = 0
     query_count: int = 0
     error_count: int = 0
     query_average: float = None   # type: ignore
     catalog = QUERY_CATALOG
     app: ApplicationContext = None   # type: ignore
 
-    def __init__(self, app, label: str = None):
+    def __init__(self, app, label: Optional[str] = None):
         """Initialize instance."""
         self.app = app
         self.label = label
 
     def init_loop(self) -> str:
         """Initialize a new loop and reset the loop counts/values."""
         loop_key = str(uuid4())
@@ -213,15 +213,15 @@
     return filtered_queries
 
 
 def _get_queries_filtered_by_slower_than(queries, time_ms):
     """Get queries filter by slower-than x ms filter.
 
     Args:
-        time_ms (int):time in milliseconds
+        time_ms: time in milliseconds
 
     Returns:
         filtered list of status reports
 
     Raises:
         ValueError
     """
@@ -260,39 +260,37 @@
         raise ValueError(
             f"This filter needs one of {valid_filter_values} as parameter."
         )
     filtered_queries = []
     if status == "running":
         filtered_queries = [
             _ for _ in queries
-            if _["executionTime"] is None
+            if _["queryExecutionState"] == "RUNNING"
         ]
     if status == "finished":
         filtered_queries = [
             _ for _ in queries
-            if _["executionTime"] is not None
+            if _["queryExecutionState"].startswith("FINISHED")
         ]
     # error -> List only queries which were NOT successfully executed.
     # interpreted as: do not include timeout and cancelled queries
     if status == "error":
         filtered_queries = [
             _ for _ in queries
-            if _["error"] is not None
-            and _.get("cancelled", False) is not True
-            and _.get("timedOut", False) is not True
+            if _["queryExecutionState"] == "FINISHED_ERROR"
         ]
     if status == "cancelled":
         filtered_queries = [
             _ for _ in queries
-            if _.get("cancelled", False) is True
+            if _["queryExecutionState"] == "FINISHED_CANCELLED"
         ]
     if status == "timeout":
         filtered_queries = [
             _ for _ in queries
-            if _.get("timedOut", False) is True
+            if _["queryExecutionState"] == "FINISHED_TIMEOUT"
         ]
     return filtered_queries
 
 
 def _get_queries_filtered_by_uuid(queries, uuid):
     """Get query status by uuid.
 
@@ -340,15 +338,15 @@
     if filter_name == "status":
         filtered_queries = _get_queries_filtered_by_status(
             queries, filter_value
         )
     # filter by slower-than
     if filter_name == "slower-than":
         filtered_queries = _get_queries_filtered_by_slower_than(
-            queries, int(filter_value)
+            queries, filter_value
         )
     # filter by type
     if filter_name == "type":
         filtered_queries = _get_queries_filtered_by_type(
             queries, filter_value
         )
     # filter by regex
@@ -408,15 +406,15 @@
     app.echo_info_sparql(status_dict["queryString"])
 
 
 @click.command(cls=CmemcCommand, name="list")
 @click.option(
     "--id-only",
     is_flag=True,
-    help="Lists only query identifier and no labels or other meta data. "
+    help="Lists only query identifier and no labels or other metadata. "
          "This is useful for piping the ids into other cmemc commands."
 )
 @click.pass_obj
 def list_command(app, id_only):
     """List available queries from the catalog.
 
     Outputs a list of query URIs which can be used as reference for
@@ -609,15 +607,15 @@
         click.launch(open_query_uri)
 
 
 @click.command(cls=CmemcCommand, name="status")
 @click.option(
     "--id-only",
     is_flag=True,
-    help="Lists only query identifier and no labels or other meta data. "
+    help="Lists only query identifier and no labels or other metadata. "
          "This is useful for piping the ids into other cmemc commands."
 )
 @click.option(
     "--raw",
     is_flag=True,
     help="Outputs raw JSON response of the query status API."
 )
```

### Comparing `cmem-cmemc-22.3rc1/cmem/cmemc/cli/commands/resource.py` & `cmem_cmemc-23.1/cmem/cmemc/cli/commands/resource.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     get_resource_metadata,
     get_resource_usage_data
 )
 
 RESOURCE_FILTER_TYPES = ["project", 'regex']
 RESOURCE_FILTER_TYPES_HIDDEN = ["ids"]
 RESOURCE_FILTER_TEXT = (
-    "Filter file resources based on a meta data. "
+    "Filter file resources based on metadata. "
     f"First parameter CHOICE can be one of {str(RESOURCE_FILTER_TYPES)}"
     ". The second parameter is based on CHOICE, e.g. a project "
     "ID or a regular expression string."
 )
 
 
 def _get_resources_filtered(resources, filter_name, filter_value):
@@ -50,15 +50,15 @@
     "--raw",
     is_flag=True,
     help="Outputs raw JSON."
 )
 @click.option(
     "--id-only",
     is_flag=True,
-    help="Lists only resource names and no other meta data. "
+    help="Lists only resource names and no other metadata. "
          "This is useful for piping the IDs into other commands."
 )
 @click.option(
     "--filter", "filters_",
     multiple=True,
     type=(str, str),
     autocompletion=completion.resource_list_filter,
@@ -121,17 +121,18 @@
     autocompletion=completion.resource_list_filter,
     help=RESOURCE_FILTER_TEXT
 )
 @click.pass_obj
 def delete_command(app, resource_ids, force, all_, filters_):
     """Delete file resources.
 
-    You have three selection mechanisms: with specific IDs, you will delete
-    only these resources; by using --filter your will delete resources based
-    on the filter type and value; by using --all will delete all resources.
+    There are three selection mechanisms: with specific IDs, only those
+    specified resources will be deleted; by using --filter, resources based
+    on the filter type and value will be deleted; using --all will delete
+    all resources.
     """
     if resource_ids == () and not all_ and filters_ == ():
         raise ValueError(
             "Either specify at least one resource ID or use the --all or "
             "--filter options to specify resources for deletion."
         )
 
@@ -188,15 +189,15 @@
 @click.option(
     "--raw",
     is_flag=True,
     help="Outputs raw JSON."
 )
 @click.pass_obj
 def inspect_command(app, resource_id, raw):
-    """Display all meta data of a file resource."""
+    """Display all metadata of a file resource."""
     project_id, resource_id = split_task_id(resource_id)
     resource_data = get_resource_metadata(project_id, resource_id)
     if raw:
         app.echo_info_json(resource_data)
     else:
         table = struct_to_table(resource_data)
         app.echo_info_table(
@@ -238,15 +239,15 @@
     app.echo_info_table(table, headers=headers, sort_column=2)
 
 
 @click.group(cls=CmemcGroup)
 def resource():
     """List, inspect or delete dataset file resources.
 
-    File resources are identified by its name and project ID.
+    File resources are identified by their paths and project IDs.
     """
 
 
 resource.add_command(list_command)
 resource.add_command(delete_command)
 resource.add_command(inspect_command)
 resource.add_command(usage_command)
```

### Comparing `cmem-cmemc-22.3rc1/cmem/cmemc/cli/commands/scheduler.py` & `cmem_cmemc-23.1/cmem/cmemc/cli/commands/scheduler.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     is_flag=True,
     help="Outputs raw JSON."
 )
 @click.option(
     "--id-only",
     is_flag=True,
     help="Lists only task identifier and no labels or other "
-         "meta data. This is useful for piping the IDs into other commands."
+         "metadata. This is useful for piping the IDs into other commands."
 )
 @click.pass_obj
 def list_command(app, raw, id_only):
     """List available scheduler.
 
     Outputs a table or a list of scheduler IDs which can be used as
     reference for the scheduler commands.
@@ -102,28 +102,20 @@
         for _ in sorted(s["projectId"] + ":" + s["id"] for s in schedulers):
             app.echo_result(_)
         return
     # output a user table
     table = []
     headers = ["Scheduler ID", "Interval", "Enabled", "Label"]
     for _ in schedulers:
-        if "parameters" in _:
-            row = [
-                _["projectId"] + ":" + _["id"],
-                _["parameters"]["interval"],
-                _["parameters"]["enabled"],
-                _["label"],
-            ]
-        else:
-            # This is the case for DI Version < 21.09
-            headers = ["Scheduler ID", "Label"]
-            row = [
-                _["projectId"] + ":" + _["id"],
-                _["label"],
-            ]
+        row = [
+            _["projectId"] + ":" + _["id"],
+            _["parameters"]["interval"],
+            _["parameters"]["enabled"],
+            _["label"],
+        ]
         table.append(row)
     # sort output by label - https://docs.python.org/3/howto/sorting.html
     app.echo_info_table(table, headers=headers, sort_column=1)
 
 
 @click.command(cls=CmemcCommand, name="inspect")
 @click.argument(
@@ -134,15 +126,15 @@
 @click.option(
     "--raw",
     is_flag=True,
     help="Outputs raw JSON."
 )
 @click.pass_obj
 def inspect_command(app, scheduler_id, raw):
-    """Display all meta data of a scheduler."""
+    """Display all metadata of a scheduler."""
     app.echo_debug(f"Scheduler ID is {scheduler_id}")
     project_id, scheduler_id = split_task_id(scheduler_id)
     task = get_task(project_id, scheduler_id)
     if raw:
         app.echo_info_json(task)
     else:
         table = struct_to_table(task)
```

### Comparing `cmem-cmemc-22.3rc1/cmem/cmemc/cli/commands/store.py` & `cmem_cmemc-23.1/cmem/cmemc/cli/commands/store.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,21 @@
     help="Delete existing bootstrap data if present and import bootstrap "
          "data which was delivered "
 )
 @click.pass_obj
 def bootstrap_command(app: ApplicationContext, import_):
     """Update/Import bootstrap data.
 
-    This command imports the bootstrap data needed for managing shapes,
-    access conditions, the query catalog and the vocabulary catalog.
+    This command imports the bootstrap data needed for managing shapes and
+    configuration objects.
 
-    Note: There is currently no deletion mechanism for the bootstrap data,
-    so you need to remove the graphs manually (or just remove all graphs).
+    Note: The command will first remove all existing bootstrap data
+    (identified with the isSystemResource flag) and will then import the new data
+    to the corresponding graphs (shape catalog, vocabulary catalog, configuration
+    graph).
     """
     if "store" not in sys.argv:
         app.echo_warning(
             "The 'admin bootstrap' command is deprecated and will be removed "
             "in the next major release.\n"
             "Please use the 'admin store bootstrap' command instead."
         )
@@ -65,17 +67,17 @@
     help="Delete existing showcase data if present."
 )
 @click.pass_obj
 def showcase_command(app, scale, create, delete):
     """Create showcase data.
 
     This command creates a showcase scenario of multiple graphs including
-    integration graphs, shapes, statement annotations etc.
+    integration graphs, shapes, statement annotations, etc.
 
-    Note: There is currently no deletion mechanism for the showcase data, so
+    Note: There is currently no deletion mechanism for the showcase data and
     you need to remove the showcase graphs manually (or just remove all
     graphs).
     """
     if "store" not in sys.argv:
         app.echo_warning(
             "The 'admin showcase' command is deprecated and will be removed "
             "in the next major release.\n"
@@ -114,16 +116,16 @@
     help="Overwrite existing files. "
          "This is a dangerous option, so use it with care.",
 )
 @click.pass_obj
 def export_command(app, backup_file, overwrite):
     """Backup all knowledge graphs to a ZIP archive.
 
-    The backup file is a ZIP archive containing all knowledge graphs as
-    Turtle files + configuration file for each graph.
+    The backup file is a ZIP archive containing all knowledge graphs (one
+    Turtle file + configuration file per graph).
 
     This command will create lots of load on the server.
     It can take a long time to complete.
     """
     if exists(backup_file) and overwrite is not True:
         raise ValueError(
             f"Export file {backup_file} already exists and --overwrite "
@@ -168,26 +170,26 @@
         dir_okay=False
     )
 )
 @click.pass_obj
 def import_command(app, backup_file):
     """Restore graphs from a ZIP archive.
 
-    The backup file is a ZIP archive containing all knowledge graphs as
-    Turtle files + configuration file for each graph.
+    The backup file is a ZIP archive containing all knowledge graphs  (one
+    Turtle file + configuration file per graph).
 
-    The command will load a single backup ZIP archive into the triple store,
+    The command will load a single backup ZIP archive into the triple store
     by replacing all graphs with the content of the Turtle files in the
     archive and deleting all graphs which are not in the archive.
 
     This command will create lots of load on the server.
     It can take a long time to complete.
     The backup file will be transferred to the server, then unzipped and
-    imported graph by graph. After the initial transfer, the network
-    connection is not used anymore, so it will be closed by proxies sometimes.
+    imported graph by graph. After the initial transfer the network
+    connection is not used anymore and may be closed by proxies.
     This does not mean that the import failed.
     """
     app.echo_info(f"Importing graphs backup from {backup_file} ...", nl=False)
     request = post_zip(backup_file)
     request.raise_for_status()
     app.echo_success(" done")
```

### Comparing `cmem-cmemc-22.3rc1/cmem/cmemc/cli/commands/vocabulary.py` & `cmem_cmemc-23.1/cmem/cmemc/cli/commands/vocabulary.py`

 * *Files 5% similar despite different names*

```diff
@@ -217,15 +217,15 @@
 
 
 @click.command(cls=CmemcCommand, name="list")
 @click.option(
     "--id-only",
     is_flag=True,
     help="Lists only vocabulary identifier (IRIs) and no labels or other "
-         "meta data. This is useful for piping the ids into other cmemc "
+         "metadata. This is useful for piping the ids into other cmemc "
          "commands."
 )
 @click.option(
     "--filter", "filter_",
     type=click.Choice(
         ["all", "installed", "installable"],
         case_sensitive=True
@@ -280,28 +280,28 @@
 )
 @click.option(
     "-a", "--all", "all_",
     is_flag=True,
     help="Install all vocabularies from the catalog."
 )
 @click.pass_obj
-def install_command(app, iris, all_):
+def install_command(app: ApplicationContext, iris: tuple[str, ...], all_):
     """Install one or more vocabularies from the catalog.
 
     Vocabularies are identified by their graph IRI.
     Installable vocabularies can be listed with the
     vocabulary list command.
     """
     if iris == () and not all_:
         raise ValueError("Either specify at least one vocabulary "
                          + "IRI or use the --all option to install all "
                            "vocabularies from the catalog.")
     if all_:
-        iris = (
-            [iri["iri"] for iri in get_vocabularies(filter_="installable")]
+        iris = tuple(
+            iri["iri"] for iri in get_vocabularies(filter_="installable")
         )
     count: int = len(iris)
     current: int = 1
     for iri in iris:
         app.echo_info(
             f"Install vocabulary {current}/{count}: {iri} ... ",
             nl=False
@@ -320,28 +320,28 @@
 )
 @click.option(
     "-a", "--all", "all_",
     is_flag=True,
     help="Uninstall all installed vocabularies."
 )
 @click.pass_obj
-def uninstall_command(app, iris, all_):
+def uninstall_command(app: ApplicationContext, iris: tuple[str, ...], all_):
     """Uninstall one or more vocabularies.
 
     Vocabularies are identified by their graph IRI.
     Already installed vocabularies can be listed with the
     vocabulary list command.
     """
     if iris == () and not all_:
         raise ValueError("Either specify at least one vocabulary "
                          + "IRI or use the --all option to uninstall all "
                            "installed vocabularies.")
     if all_:
-        iris = (
-            [iri["iri"] for iri in get_vocabularies(filter_="installed")]
+        iris = tuple(
+            iri["iri"] for iri in get_vocabularies(filter_="installed")
         )
     count: int = len(iris)
     current: int = 1
     for iri in iris:
         app.echo_info(
             f"Uninstall vocabulary {current}/{count}: {iri} ... ",
             nl=False
@@ -382,15 +382,15 @@
     and create a corresponding vocabulary catalog entry.
 
     The uploaded ontology file is analysed locally in order to discover the
     named graph and the prefix declaration. This requires an OWL ontology
     description which correctly uses the `vann:preferredNamespacePrefix` and
     `vann:preferredNamespaceUri` properties.
     """
-    # fetch meta data
+    # fetch metadata
     if namespace != (None, None):
         _validate_namespace(app, namespace)
         meta_data = _get_vocabulary_metadata_from_file(file, True)
         meta_data["prefix"] = namespace[0]
         meta_data["namespace"] = namespace[1]
     else:
         meta_data = _get_vocabulary_metadata_from_file(file, False)
@@ -441,23 +441,23 @@
 )
 @click.option(
     "-a", "--all", "all_",
     is_flag=True,
     help="Update cache for all installed vocabularies."
 )
 @click.pass_obj
-def cache_update_command(app, iris, all_):
+def cache_update_command(app: ApplicationContext, iris: tuple[str, ...], all_):
     """Reload / updates the data integration cache for a vocabulary."""
     if iris == () and not all_:
         raise ValueError("Either specify at least one vocabulary "
                          + "IRI or use the --all option to update the "
                            "cache for all installed vocabularies.")
     if all_:
-        iris = (
-            [iri["iri"] for iri in get_vocabularies(filter_="installed")]
+        iris = tuple(
+            iri["iri"] for iri in get_vocabularies(filter_="installed")
         )
     count: int = len(iris)
     current: int = 1
     for iri in iris:
         app.echo_info(
             f"Update cache {current}/{count}: {iri} ... ",
             nl=False
@@ -468,15 +468,15 @@
 
 
 @click.command(cls=CmemcCommand, name="list")
 @click.option(
     "--id-only",
     is_flag=True,
     help="Lists only vocabulary term identifier (IRIs) and no labels or other "
-         "meta data. This is useful for piping the ids into other cmemc "
+         "metadata. This is useful for piping the ids into other cmemc "
          "commands."
 )
 @click.option(
     "--raw",
     is_flag=True,
     help="Outputs raw JSON."
 )
```

### Comparing `cmem-cmemc-22.3rc1/cmem/cmemc/cli/commands/workflow.py` & `cmem_cmemc-23.1/cmem/cmemc/cli/commands/workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 import os
 import re
 import sys
 import time
 
 import click
 
-import requests
-
 import timeago
 
 from cmem.cmemc.cli import completion
 from cmem.cmemc.cli.commands import CmemcCommand, CmemcGroup
 from cmem.cmemc.cli.commands.scheduler import scheduler
 from cmem.cmempy.workflow import get_workflows
 from cmem.cmempy.workflow.workflow import (
@@ -32,15 +30,15 @@
     start_task_activity
 )
 from cmem.cmempy.workspace.projects.project import get_projects
 from cmem.cmempy.workspace.search import list_items
 
 WORKFLOW_FILTER_TYPES = sorted(['project', 'regex', 'tag', 'io'])
 WORKFLOW_LIST_FILTER_HELP_TEXT = (
-    "List workflows based on meta data. First parameter --filter"
+    "List workflows based on metadata. First parameter --filter"
     f" CHOICE can be one of {str(WORKFLOW_FILTER_TYPES)}."
     " The second parameter is based on CHOICE."
 )
 
 IO_WARNING_NO_RESULT = "The workflow was executed but produced no result."
 IO_WARNING_NO_OUTPUT_DEFINED = "The workflow was executed, a result was "\
                                "received but dropped."
@@ -271,41 +269,14 @@
         # wait until isRunning is false
         if not status['isRunning']:
             break
         time.sleep(polling_interval)
     return status
 
 
-def _status_command_pre_cmem_20_10(
-        app, raw, _filter, workflow_ids
-):
-    """Get status of workflows without new taskActivitiesStatus API."""
-    if workflow_ids == ():
-        workflow_ids += tuple(_workflows_get_ids())
-
-    for workflow_id in workflow_ids:
-        project_id, task_id = workflow_id.split(":")
-        status = get_activity_status(project_id, task_id)
-        # filter for running activities
-        if _filter == "running"\
-                and 'isRunning' in status and not status['isRunning']:
-            continue
-        # filter for failed activities
-        if _filter == "failed"\
-                and "failed" in status and not status['failed']:
-            continue
-        # output raw json if wanted
-        if raw:
-            app.echo_info_json(status)
-        # output single line status
-        else:
-            app.echo_info(f"{workflow_id} ... ", nl=False)
-            _workflow_echo_status(app, status)
-
-
 def _workflow_echo_status(app, status):
     """Print a colored status based on the returned JSON.
 
     Status can be Idle, Running, Canceling, Waiting, Finished
     isRunning is true for Running, Canceling, Waiting
     canceled only exists sometimes
     """
@@ -561,15 +532,15 @@
     autocompletion=completion.workflow_list_filter,
     help=WORKFLOW_LIST_FILTER_HELP_TEXT,
 )
 @click.option(
     "--id-only",
     is_flag=True,
     help="Lists only workflow identifier and no labels or other "
-         "meta data. This is useful for piping the IDs into other commands."
+         "metadata. This is useful for piping the IDs into other commands."
 )
 @click.option(
     "--raw",
     is_flag=True,
     help="Outputs raw JSON objects of workflow task search API response."
 )
 @click.pass_obj
@@ -630,34 +601,28 @@
     nargs=-1,
     type=click.STRING,
     autocompletion=completion.workflow_ids
 )
 @click.pass_obj
 def status_command(app, project_id, raw, _filter, workflow_ids):
     """Get status information of workflow(s)."""
-    try:
-        workflow_status = get_activities_status(
-            status=_filter,
-            project_name=project_id,
-            activity=ACTIVITY_TYPE_EXECUTE_DEFAULTWORKFLOW
-        )
-        for status in workflow_status:
-            workflow_id = status["project"] + ":" + status["task"]
-            if len(workflow_ids) == 0 or workflow_id in workflow_ids:
-                if raw:
-                    # TODO: output for more than one workflow is not valid JSON
-                    app.echo_info_json(status)
-                else:
-                    app.echo_info(f"{workflow_id} ... ", nl=False)
-                    _workflow_echo_status(app, status)
-    except requests.exceptions.HTTPError:
-        app.echo_warning("CMEM 20.10 taskActivitiesStatus API not available.\n"
-                         "Falling back to older and more slow API with less "
-                         "filter options.")
-        _status_command_pre_cmem_20_10(app, raw, _filter, workflow_ids)
+    workflow_status = get_activities_status(
+        status=_filter,
+        project_name=project_id,
+        activity=ACTIVITY_TYPE_EXECUTE_DEFAULTWORKFLOW
+    )
+    for status in workflow_status:
+        workflow_id = status["project"] + ":" + status["task"]
+        if len(workflow_ids) == 0 or workflow_id in workflow_ids:
+            if raw:
+                # TODO: output for more than one workflow is not valid JSON
+                app.echo_info_json(status)
+            else:
+                app.echo_info(f"{workflow_id} ... ", nl=False)
+                _workflow_echo_status(app, status)
 
 
 @click.command(cls=CmemcCommand, name="open")
 @click.argument(
     "workflow_id",
     type=click.STRING,
     autocompletion=completion.workflow_ids
```

### Comparing `cmem-cmemc-22.3rc1/cmem/cmemc/cli/commands/workspace.py` & `cmem_cmemc-23.1/cmem/cmemc/cli/commands/workspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,17 +52,17 @@
         dir_okay=False
     )
 )
 @click.pass_obj
 def export_command(app, overwrite, marshalling_plugin, template, file):
     """Export the complete workspace (all projects) to a ZIP file.
 
-    Depending on the requested type, this ZIP contains either a turtle file
-    for each project (type rdfTurtle) or a substructure of resource files and
-    XML descriptions (type xmlZip).
+    Depending on the requested export type, this ZIP file contains either one
+    Turtle file per project (type `rdfTurtle`) or a substructure of resource
+    files and XML descriptions (type `xmlZip`).
 
     The file name is optional and will be generated with by
     the template if absent.
     """
     ctx = click.get_current_context()
     if ctx.auto_envvar_prefix == "CMEMC_WORKSPACE_EXPORT":
         app.echo_warning(
```

### Comparing `cmem-cmemc-22.3rc1/cmem/cmemc/cli/completion.py` & `cmem_cmemc-23.1/cmem/cmemc/cli/completion.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """Utility functions for CLI auto-completion functionality."""
 # pylint: disable=unused-argument, broad-except, too-many-lines
 import os
 from collections import Counter
+from contextlib import suppress
 
 import requests
-
 from bs4 import BeautifulSoup
-
+from click import Context
 from natsort import natsorted, ns
-
 from prometheus_client.parser import text_string_to_metric_families
 
 from cmem.cmemc.cli.context import CONTEXT
 from cmem.cmemc.cli.utils import (
     get_graphs,
     metric_get_labels,
     metrics_get_dict, struct_to_table
 )
 from cmem.cmempy.dp.admin import get_prometheus_data
 from cmem.cmempy.health import get_complete_status_info
+from cmem.cmempy.keycloak.group import list_groups
+from cmem.cmempy.keycloak.user import list_users, get_user_by_username, user_groups
 from cmem.cmempy.plugins.marshalling import get_marshalling_plugins
 from cmem.cmempy.queries import QUERY_CATALOG, get_query_status
 from cmem.cmempy.vocabularies import get_vocabularies
 from cmem.cmempy.workflow.workflows import get_workflows_io
 from cmem.cmempy.workspace import (
     get_task_plugin_description,
     get_task_plugins,
@@ -123,15 +124,15 @@
         0,
         ("label", "Metadata: A name.")
     )
     return list_
 
 
 def dataset_parameter(ctx, args, incomplete):
-    """Prepare a list of dataset parameter for a dataset type."""
+    """Prepare a list of dataset parameters for a dataset type."""
     CONTEXT.set_connection_from_args(args)
     incomplete = incomplete.lower()
     # look if cursor is in value position of the -p option and
     # return nothing in case it is (values are not completed atm)
     if args[len(args) - 2] in ("-p", "--parameter"):
         return []
     # try to determine the dataset type
@@ -1224,7 +1225,61 @@
     status_info = struct_to_table(get_complete_status_info())
     for _ in status_info:
         options.append(_[0])
     return _finalize_completion(
         candidates=options,
         incomplete=incomplete
     )
+
+
+def user_ids(ctx, args, incomplete):
+    """Prepare a list of username for admin update/delete/password command."""
+    CONTEXT.set_connection_from_args(args)
+    options = []
+    for _ in list_users():
+        options.append(
+            (
+                _["username"]
+            )
+        )
+    return _finalize_completion(
+        candidates=options,
+        incomplete=incomplete,
+        sort_by=SORT_BY_DESC
+    )
+
+
+def user_group_ids(ctx: Context, args, incomplete):
+    """Prepare a list of group name for admin user update
+     --unassign-group/--assign-group parameter"""
+    CONTEXT.set_connection_from_args(args)
+    if not ctx.args:
+        return []
+    users = get_user_by_username(username=str(ctx.args[0]))
+    if not users:
+        return []
+
+    if args[len(args) - 1] == "--unassign-group":
+        groups = user_groups(user_id=users[0]["id"])
+    else:
+        user_group_names = (
+            [group["name"] for group in user_groups(user_id=users[0]["id"])]
+        )
+        groups = (
+            [group for group in list_groups() if group["name"] not in user_group_names]
+        )
+    options = []
+    for _ in groups:
+        options.append(
+            (
+                _["name"]
+            )
+        )
+    for num, arg in enumerate(args):
+        if num - 1 > 0 and args[num - 1] == args[len(args) - 1]:
+            with suppress(ValueError):
+                options.remove(arg)
+    return _finalize_completion(
+        candidates=options,
+        incomplete=incomplete,
+        sort_by=SORT_BY_DESC
+    )
```

### Comparing `cmem-cmemc-22.3rc1/cmem/cmemc/cli/context.py` & `cmem_cmemc-23.1/cmem/cmemc/cli/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,24 +27,26 @@
 from cmem.cmempy.health import (
     get_di_version,
     get_dp_version
 )
 from cmem.cmemc.cli.exceptions import (InvalidConfiguration)
 from cmem.cmemc.cli.utils import is_completing
 
-DI_TARGET_VERSION = "v22.2"
+DI_TARGET_VERSION = "v23.1"
 
-DP_TARGET_VERSION = "v22.2"
+DP_TARGET_VERSION = "v23.1"
 
 KNOWN_CONFIG_KEYS = {
     'CMEM_BASE_URI': cmempy_config.get_cmem_base_uri,
     'SSL_VERIFY': cmempy_config.get_ssl_verify,
     'REQUESTS_CA_BUNDLE': cmempy_config.get_requests_ca_bundle,
     'DP_API_ENDPOINT': cmempy_config.get_dp_api_endpoint,
     'DI_API_ENDPOINT': cmempy_config.get_di_api_endpoint,
+    'KEYCLOAK_BASE_URI': cmempy_config.get_keycloak_base_uri,
+    'KEYCLOAK_REALM_ID': cmempy_config.get_keycloak_realm_id,
     'OAUTH_TOKEN_URI': cmempy_config.get_oauth_token_uri,
     'OAUTH_GRANT_TYPE': cmempy_config.get_oauth_grant_type,
     'OAUTH_USER': cmempy_config.get_oauth_user,
     'OAUTH_PASSWORD': cmempy_config.get_oauth_password,
     'OAUTH_CLIENT_ID': cmempy_config.get_oauth_client_id,
     'OAUTH_CLIENT_SECRET': cmempy_config.get_oauth_client_secret,
     'OAUTH_ACCESS_TOKEN': cmempy_config.get_oauth_access_token
@@ -388,21 +390,20 @@
                 # if not in PATH, we try to parse it as list
                 parsed_list = list(ast.literal_eval(command))
             except SyntaxError as error:
                 raise ValueError(
                     f"'{command}' could not be found in PATH or the value "
                     "could not be parsed as list, e.g. ['echo', 'this']."
                 ) from error
-            else:
-                # if its a parsed list, we try to find the first element only
-                if which(parsed_list[0]) is None:
-                    raise ValueError(
-                        f"'{parsed_list[0]}' could not be found in PATH."
-                    )
-                parsed_list[0] = which(parsed_list[0])
+            # else: if it is a parsed list, we try to find the first element only
+            if which(parsed_list[0]) is None:
+                raise ValueError(
+                    f"'{parsed_list[0]}' could not be found in PATH."
+                )
+            parsed_list[0] = which(parsed_list[0])
         checked_command = parsed_list if parsed_list is not None else command
         if env.get("CMEMC_CREDENTIAL_PROCESS_NO_WARNING", "false") != "true":
             self.echo_warning(
                 "Consider possible security implications associated with "
                 "executing the external credential process:\n"
                 f"{checked_command}\n"
                 "You can suppress this warning by setting "
```

### Comparing `cmem-cmemc-22.3rc1/cmem/cmemc/cli/manual_helper/graph.py` & `cmem_cmemc-23.1/cmem/cmemc/cli/manual_helper/graph.py`

 * *Files identical despite different names*

### Comparing `cmem-cmemc-22.3rc1/cmem/cmemc/cli/manual_helper/multi_page.py` & `cmem_cmemc-23.1/cmem/cmemc/cli/manual_helper/multi_page.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 def get_icon_for_command_group(full_name):
     """Return in mkdocs material icon term for a command group."""
     return {
         "admin": "material/key-link",
         "admin metrics": "material/chart-line-variant",
         "admin store": "material/database-outline",
+        "admin user": "material/account-cog",
         "admin workspace": "material/folder-multiple-outline",
         "admin workspace python": "material/language-python",
         "config": "material/cog-outline",
         "dataset": "eccenca/artefact-dataset",
         "dataset resource": "eccenca/artefact-file",
         "project": "eccenca/artefact-project",
         "query": "eccenca/application-queries",
@@ -27,14 +28,15 @@
         "workflow": "eccenca/artefact-workflow",
         "workflow scheduler": "material/calendar"
     }.get(full_name, "octicons/cross-reference-24")
 
 
 def get_tags_for_command_group(full_name: str) -> str:
     """Get list of tags for a command group name as markdown head section."""
+    # pylint: disable=consider-using-join
     tags = {
         "admin": ["cmemc"],
         "admin metrics": ["cmemc"],
         "admin store": ["SPARQL", "cmemc"],
         "admin workspace": ["cmemc"],
         "admin workspace python": ["Python", "cmemc"],
         "config": ["cmemc"],
```

### Comparing `cmem-cmemc-22.3rc1/cmem/cmemc/cli/manual_helper/single_page.py` & `cmem_cmemc-23.1/cmem/cmemc/cli/manual_helper/single_page.py`

 * *Files identical despite different names*

### Comparing `cmem-cmemc-22.3rc1/cmem/cmemc/cli/utils.py` & `cmem_cmemc-23.1/cmem/cmemc/cli/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Utility functions for CLI interface."""
 import json
 import os
 import re
 import unicodedata
 from typing import Dict
 
+from importlib.metadata import version
 from prometheus_client import Metric
 from prometheus_client.parser import text_string_to_metric_families
 
 from cmem.cmempy.dp.admin import get_prometheus_data
 from cmem.cmempy.dp.proxy.graph import get_graphs_list
 
 NAMESPACES = {
@@ -20,19 +21,15 @@
     "sd": "http://www.w3.org/ns/sparql-service-description#"
 }
 
 
 def get_version():
     """Get the current version or SNAPSHOT."""
     # pylint: disable=import-outside-toplevel
-    try:
-        from cmem.cmemc.cli.version import VERSION
-        return VERSION
-    except ImportError:
-        return "SNAPSHOT"
+    return version('cmem-cmemc')
 
 
 def extract_error_message(error):
     """Extract a message from an exception."""
     # exceptions with response is HTTPError
     message = type(error).__name__ + ": " + str(error) + "\n"
     try:
```

### Comparing `cmem-cmemc-22.3rc1/pyproject.toml` & `cmem_cmemc-23.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [tool.poetry]
 name = "cmem-cmemc"
-version = "22.3rc1"
+version = "23.1"
 description = "Command line client for eccenca Corporate Memory"
 license = "Apache 2.0"
 classifiers = ["Development Status :: 5 - Production/Stable", "Intended Audience :: Developers", "Intended Audience :: Science/Research", "Intended Audience :: System Administrators", "License :: OSI Approved :: Apache Software License", "Programming Language :: Python :: 3.9", "Topic :: Software Development :: Testing", "Topic :: Database", "Topic :: Utilities"]
 homepage = "https://eccenca.com/go/cmemc"
 authors = ["eccenca <cmempy-developer@eccenca.com>", "Sebastian Tramp <sebastian.tramp@eccenca.com>"]
 readme = "README-public.md"
 packages = [
     { include = "cmem" }
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.9"
 beautifulsoup4 = "*"
 certifi = "*"
 click = "==7.1.2"
 click-didyoumean = "*"
 click-help-colors = "*"
-cmem-cmempy = "==22.3rc3"
+cmem-cmempy = "==23.1"
+# cmem-cmempy = { path = "cmempy", develop = true }
 configparser = "*"
 jinja2 = "*"
 natsort = "*"
 prometheus-client = "*"
 pygments = "*"
 pyjwt = "*"
 requests = "*"
@@ -30,33 +31,37 @@
 tabulate = "*"
 timeago = "*"
 treelib = "*"
 types-six = "*"
 types-tabulate = "*"
 urllib3 = "*"
 
-[tool.poetry.dev-dependencies]
-bandit = "^1.7.2"
+[tool.poetry.scripts]
+cmemc = 'cmem.cmemc.cli:main'
+
+[tool.poetry.group.dev.dependencies]
+bandit = "^1.7.4"
 coverage = "^6.3.2"
+coverage-badge = "^1.1.0"
 defusedxml = "^0.7.1"
 genbadge = "^1.0.6"
-mypy = "^0.931"
-nose = "^1.3.7"
 pre-commit = "2.20.0"
 pylint-junit = "^0.3.2"
 pytest = "^7.0"
 pytest-cov = "^4.0.0"
+pytest-memray = "^1.3.0"
 safety = "^1.10.3"
 types-requests = "^2.28.11.5"
-
-[tool.poetry.scripts]
-cmemc = 'cmem.cmemc.cli:main'
+mypy = "^0.991"
+flake8-formatter-junit-xml = "^0.0.6"
+wheel = "^0.38.4"
+types-setuptools = "^67.7.0.0"
 
 [build-system]
-requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
+requires = ["poetry-core>=1.2.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 dirty = true
 
@@ -77,8 +82,7 @@
 [tool.pylint.format]
 max-line-length = "88"
 min-similarity-lines=10
 
 [tool.mypy]
 warn_return_any = true
 ignore_missing_imports = true
-
```

### Comparing `cmem-cmemc-22.3rc1/PKG-INFO` & `cmem_cmemc-23.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: cmem-cmemc
-Version: 22.3rc1
+Version: 23.1
 Summary: Command line client for eccenca Corporate Memory
 Home-page: https://eccenca.com/go/cmemc
 License: Apache 2.0
 Author: eccenca
 Author-email: cmempy-developer@eccenca.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
 Requires-Dist: beautifulsoup4
 Requires-Dist: certifi
 Requires-Dist: click (==7.1.2)
 Requires-Dist: click-didyoumean
 Requires-Dist: click-help-colors
-Requires-Dist: cmem-cmempy (==22.3rc3)
+Requires-Dist: cmem-cmempy (==23.1)
 Requires-Dist: configparser
 Requires-Dist: jinja2
 Requires-Dist: natsort
 Requires-Dist: prometheus-client
 Requires-Dist: pygments
 Requires-Dist: pyjwt
 Requires-Dist: requests
```


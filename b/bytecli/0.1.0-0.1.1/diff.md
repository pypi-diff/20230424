# Comparing `tmp/bytecli-0.1.0.tar.gz` & `tmp/bytecli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytecli-0.1.0.tar", max compression
+gzip compressed data, was "bytecli-0.1.1.tar", max compression
```

## Comparing `bytecli-0.1.0.tar` & `bytecli-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1072 2023-04-24 19:11:01.565966 bytecli-0.1.0/LICENSE
--rw-r--r--   0        0        0      597 2023-04-24 19:11:01.565966 bytecli-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-24 19:11:01.565966 bytecli-0.1.0/bytecli/__init__.py
--rw-r--r--   0        0        0     2057 2023-04-24 19:11:01.565966 bytecli-0.1.0/bytecli/main.py
--rw-r--r--   0        0        0      456 2023-04-24 19:11:01.569967 bytecli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1164 1970-01-01 00:00:00.000000 bytecli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-24 19:19:24.275419 bytecli-0.1.1/LICENSE
+-rw-r--r--   0        0        0      597 2023-04-24 19:19:24.275419 bytecli-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-24 19:19:24.275419 bytecli-0.1.1/bytecli/__init__.py
+-rw-r--r--   0        0        0     2193 2023-04-24 19:19:24.275419 bytecli-0.1.1/bytecli/main.py
+-rw-r--r--   0        0        0      456 2023-04-24 19:19:24.275419 bytecli-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1164 1970-01-01 00:00:00.000000 bytecli-0.1.1/PKG-INFO
```

### Comparing `bytecli-0.1.0/LICENSE` & `bytecli-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bytecli-0.1.0/README.md` & `bytecli-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bytecli-0.1.0/bytecli/main.py` & `bytecli-0.1.1/bytecli/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,42 +29,47 @@
 
 def get_account_info(attribute: str):
     return requests.get(BASE_URL).json()[0][attribute]
 
 
 @app.command()
 def servername() -> None:
+    """Name of serverd"""
     console.print(
         f'[magenta]Server name:[/magenta] [green]{get_account_info("server_name")}[/green]'
     )
 
 
 @app.command()
 def diskquota() -> None:
+    """Disk usage quota"""
     console.print(
         f'[magenta]Disk Quota:[/magenta] [green]{get_account_info("pretty_disk_quota")}[/green]'
     )
 
 
 @app.command()
 def bandwidthquota() -> None:
+    """Bandwidth usage quota"""
     console.print(
         f'[magenta]Bandwidth Quota:[/magenta] [green]{get_account_info("pretty_bw_quota")}[/green]'
     )
 
 
 @app.command()
 def memoryusage() -> None:
+    """Memory usage"""
     console.print(
         f'[magenta]Memory Usage:[/magenta] [green]{round(get_account_info("memory_usage") / 1024, 2)} MB [/green]'
     )
 
 
 @app.command()
 def summary() -> None:
+    """Summary of server"""
     response = requests.get(BASE_URL).json()[0]
     table = Table(
         show_header=False,
         show_lines=False,
         title=f"Server Summary - [purple]{response['server_name']}[/purple]",
     )
     table.add_row(
```

### Comparing `bytecli-0.1.0/PKG-INFO` & `bytecli-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bytecli
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Allan
 Author-email: allanklp@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


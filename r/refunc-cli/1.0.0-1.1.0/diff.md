# Comparing `tmp/refunc-cli-1.0.0.tar.gz` & `tmp/refunc-cli-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refunc-cli-1.0.0.tar", last modified: Sun Apr 23 08:20:31 2023, max compression
+gzip compressed data, was "refunc-cli-1.1.0.tar", last modified: Mon Apr 24 03:02:15 2023, max compression
```

## Comparing `refunc-cli-1.0.0.tar` & `refunc-cli-1.1.0.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-04-23 08:20:30.993436 refunc-cli-1.0.0/
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      197 2023-04-23 02:26:55.000000 refunc-cli-1.0.0/MANIFEST.in
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      199 2023-04-23 08:20:30.993436 refunc-cli-1.0.0/PKG-INFO
--rw-rw-r--   0 arvin     (1000) arvin     (1000)       12 2023-04-23 02:20:07.000000 refunc-cli-1.0.0/README.md
-drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-04-23 08:20:30.993436 refunc-cli-1.0.0/refunc_cli.egg-info/
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      199 2023-04-23 08:20:30.000000 refunc-cli-1.0.0/refunc_cli.egg-info/PKG-INFO
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      517 2023-04-23 08:20:30.000000 refunc-cli-1.0.0/refunc_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 arvin     (1000) arvin     (1000)        1 2023-04-23 08:20:30.000000 refunc-cli-1.0.0/refunc_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 arvin     (1000) arvin     (1000)       45 2023-04-23 08:20:30.000000 refunc-cli-1.0.0/refunc_cli.egg-info/entry_points.txt
--rw-rw-r--   0 arvin     (1000) arvin     (1000)        1 2023-04-23 08:20:30.000000 refunc-cli-1.0.0/refunc_cli.egg-info/not-zip-safe
--rw-rw-r--   0 arvin     (1000) arvin     (1000)       76 2023-04-23 08:20:30.000000 refunc-cli-1.0.0/refunc_cli.egg-info/requires.txt
--rw-rw-r--   0 arvin     (1000) arvin     (1000)        6 2023-04-23 08:20:30.000000 refunc-cli-1.0.0/refunc_cli.egg-info/top_level.txt
--rw-rw-r--   0 arvin     (1000) arvin     (1000)       75 2023-04-23 06:14:01.000000 refunc-cli-1.0.0/requirements.txt
-drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-04-23 08:20:30.993436 refunc-cli-1.0.0/rfctl/
--rw-rw-r--   0 arvin     (1000) arvin     (1000)        0 2023-04-23 02:02:22.000000 refunc-cli-1.0.0/rfctl/__init__.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     2146 2023-04-23 07:30:10.000000 refunc-cli-1.0.0/rfctl/__main__.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     1594 2023-04-23 07:00:36.000000 refunc-cli-1.0.0/rfctl/awslocal.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     3681 2023-04-23 06:58:17.000000 refunc-cli-1.0.0/rfctl/build.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      799 2023-04-23 06:53:29.000000 refunc-cli-1.0.0/rfctl/create.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      498 2023-04-23 07:21:11.000000 refunc-cli-1.0.0/rfctl/create_url.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      433 2023-04-23 07:14:35.000000 refunc-cli-1.0.0/rfctl/delete.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      456 2023-04-23 07:21:59.000000 refunc-cli-1.0.0/rfctl/delete_url.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      422 2023-04-23 07:28:56.000000 refunc-cli-1.0.0/rfctl/get.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      441 2023-04-23 07:28:47.000000 refunc-cli-1.0.0/rfctl/get_url.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     2014 2023-04-23 03:35:02.000000 refunc-cli-1.0.0/rfctl/schema.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      638 2023-04-23 07:13:29.000000 refunc-cli-1.0.0/rfctl/update_code.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      645 2023-04-23 07:17:30.000000 refunc-cli-1.0.0/rfctl/update_config.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)       38 2023-04-23 08:20:30.993436 refunc-cli-1.0.0/setup.cfg
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     1033 2023-04-23 02:23:54.000000 refunc-cli-1.0.0/setup.py
+drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-04-24 03:02:15.358816 refunc-cli-1.1.0/
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      197 2023-04-23 02:26:55.000000 refunc-cli-1.1.0/MANIFEST.in
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      199 2023-04-24 03:02:15.358816 refunc-cli-1.1.0/PKG-INFO
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      494 2023-04-23 09:58:14.000000 refunc-cli-1.1.0/README.md
+drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-04-24 03:02:15.358816 refunc-cli-1.1.0/refunc_cli.egg-info/
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      199 2023-04-24 03:02:15.000000 refunc-cli-1.1.0/refunc_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      552 2023-04-24 03:02:15.000000 refunc-cli-1.1.0/refunc_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)        1 2023-04-24 03:02:15.000000 refunc-cli-1.1.0/refunc_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)       45 2023-04-24 03:02:15.000000 refunc-cli-1.1.0/refunc_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)        1 2023-04-24 03:02:14.000000 refunc-cli-1.1.0/refunc_cli.egg-info/not-zip-safe
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)       76 2023-04-24 03:02:15.000000 refunc-cli-1.1.0/refunc_cli.egg-info/requires.txt
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)        6 2023-04-24 03:02:15.000000 refunc-cli-1.1.0/refunc_cli.egg-info/top_level.txt
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)       75 2023-04-23 06:14:01.000000 refunc-cli-1.1.0/requirements.txt
+drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-04-24 03:02:15.358816 refunc-cli-1.1.0/rfctl/
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)        0 2023-04-23 02:02:22.000000 refunc-cli-1.1.0/rfctl/__init__.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     2432 2023-04-24 02:41:18.000000 refunc-cli-1.1.0/rfctl/__main__.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     1561 2023-04-24 02:58:19.000000 refunc-cli-1.1.0/rfctl/awslocal.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     3681 2023-04-23 06:58:17.000000 refunc-cli-1.1.0/rfctl/build.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      818 2023-04-24 02:57:03.000000 refunc-cli-1.1.0/rfctl/create.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      498 2023-04-23 07:21:11.000000 refunc-cli-1.1.0/rfctl/create_url.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      433 2023-04-23 07:14:35.000000 refunc-cli-1.1.0/rfctl/delete.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      456 2023-04-23 07:21:59.000000 refunc-cli-1.1.0/rfctl/delete_url.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      422 2023-04-23 07:28:56.000000 refunc-cli-1.1.0/rfctl/get.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      441 2023-04-23 07:28:47.000000 refunc-cli-1.1.0/rfctl/get_url.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     2965 2023-04-24 02:46:12.000000 refunc-cli-1.1.0/rfctl/init.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      191 2023-04-24 02:49:12.000000 refunc-cli-1.1.0/rfctl/init_source.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     2014 2023-04-23 03:35:02.000000 refunc-cli-1.1.0/rfctl/schema.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      657 2023-04-24 02:56:46.000000 refunc-cli-1.1.0/rfctl/update_code.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      645 2023-04-23 07:17:30.000000 refunc-cli-1.1.0/rfctl/update_config.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)       38 2023-04-24 03:02:15.358816 refunc-cli-1.1.0/setup.cfg
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     1033 2023-04-23 12:39:17.000000 refunc-cli-1.1.0/setup.py
```

### Comparing `refunc-cli-1.0.0/refunc_cli.egg-info/SOURCES.txt` & `refunc-cli-1.1.0/refunc_cli.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -15,10 +15,12 @@
 rfctl/build.py
 rfctl/create.py
 rfctl/create_url.py
 rfctl/delete.py
 rfctl/delete_url.py
 rfctl/get.py
 rfctl/get_url.py
+rfctl/init.py
+rfctl/init_source.py
 rfctl/schema.py
 rfctl/update_code.py
 rfctl/update_config.py
```

### Comparing `refunc-cli-1.0.0/rfctl/__main__.py` & `refunc-cli-1.1.0/rfctl/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,49 +4,58 @@
 from rfctl.delete import delete_command
 from rfctl.get import get_command
 from rfctl.update_code import update_code_command
 from rfctl.update_config import update_config_command
 from rfctl.create_url import create_url_command
 from rfctl.delete_url import delete_url_command
 from rfctl.get_url import get_url_command
+from rfctl.init import init_command
 import jsonschema
 import click
 import yaml
 import os
+import sys
 
 
 @click.group()
 @click.option('--endpoint', default=os.environ.get("AWS_DEFAULT_ENDPOINT", ""))
-@click.option('--manifest', default="lambda.yaml", type=click.Path(exists=True, dir_okay=False, resolve_path=True))
+@click.option('--manifest', default="lambda.yaml", type=click.Path(exists=False, dir_okay=False, resolve_path=True))
 @click.pass_context
 def cli(ctx: click.Context, endpoint, manifest):
+    ctx.obj = {"working_dir": os.getcwd(), "manifest": manifest}
+    os.chdir(os.path.dirname(manifest))
+    if ctx.invoked_subcommand in ["init"]:
+        return
+    if not os.path.isfile(manifest):
+        click.echo("Function manifest not found")
+        sys.exit(-1)
     click.echo("Function manifest founding in %s" % manifest)
-    ctx.obj, funcdef = {"working_dir": os.getcwd()}, {}
+    funcdef = {}
     validate_error = None
     with open(manifest, 'r', encoding="utf-8") as fd:
         funcdef = yaml.load(fd, Loader=yaml.FullLoader)
         validate_error = None
     try:
         jsonschema.validate(instance=funcdef, schema=funcdef_schema)
     except Exception as e:
         validate_error = "{}".format(e).split("\n", maxsplit=1)[0].strip()
     if not validate_error is None:
         click.echo("Function manifest error %s" % validate_error)
-        exit(-1)
+        sys.exit(-1)
     if not endpoint:
         click.echo("Endpoint can't be empty")
-        exit(-1)
-    os.chdir(os.path.dirname(manifest))
+        sys.exit(-1)
     os.environ.update({
         "AWS_DEFAULT_REGION": funcdef["metadata"]["namespace"]
     })
     ctx.obj["endpoint"] = endpoint
     ctx.obj["funcdef"] = set_funcdef_defaults(funcdef)
 
 
+cli.add_command(init_command, "init")
 cli.add_command(build_command, "build")
 cli.add_command(create_command, "create")
 cli.add_command(delete_command, "delete")
 cli.add_command(get_command, "get")
 cli.add_command(update_code_command, "update-code")
 cli.add_command(update_config_command, "update-config")
 cli.add_command(create_url_command, "create-url")
```

### Comparing `refunc-cli-1.0.0/rfctl/awslocal.py` & `refunc-cli-1.1.0/rfctl/awslocal.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,14 @@
                 out.flush()
 
     process = subprocess.Popen(cmd, stderr=subprocess.PIPE, stdout=subprocess.PIPE, stdin=subprocess.PIPE, env=env)
     Thread(target=output_reader, args=[process.stdout, sys.stdout]).start()
     Thread(target=output_reader, args=[process.stderr, sys.stderr]).start()
 
     process.wait()
-    sys.exit(process.returncode)
 
 
 def lambda_command(endpoint_url, args):
     # prepare cmd args
     cmd_args = ["aws", "--no-verify-ssl", "--endpoint-url", endpoint_url, "lambda"]
     cmd_args.extend([str(x) for x in args])
     role = False
```

### Comparing `refunc-cli-1.0.0/rfctl/build.py` & `refunc-cli-1.1.0/rfctl/build.py`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.0.0/rfctl/create.py` & `refunc-cli-1.1.0/rfctl/create.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,7 +14,8 @@
     lambda_args = ["create-function",
                    "--function-name", funcdef["metadata"]["name"],
                    "--handler", funcdef["spec"]["handler"],
                    "--zip-file", "fileb://{}".format(out),
                    "--runtime", funcdef["spec"]["runtime"],
                    "--timeout", funcdef["spec"]["timeout"]]
     lambda_command(ctx.obj["endpoint"], lambda_args)
+    os.remove(out)
```

### Comparing `refunc-cli-1.0.0/rfctl/schema.py` & `refunc-cli-1.1.0/rfctl/schema.py`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.0.0/rfctl/update_code.py` & `refunc-cli-1.1.0/rfctl/update_code.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,7 +11,8 @@
     out = os.path.join(ctx.obj["working_dir"], "lambda.zip")
     do_build(ctx, out)
     click.echo("Updating code for function %s/%s" % (funcdef["metadata"]["namespace"], funcdef["metadata"]["name"]))
     lambda_args = ["update-function-code",
                    "--function-name", funcdef["metadata"]["name"],
                    "--zip-file", "fileb://{}".format(out)]
     lambda_command(ctx.obj["endpoint"], lambda_args)
+    os.remove(out)
```

### Comparing `refunc-cli-1.0.0/rfctl/update_config.py` & `refunc-cli-1.1.0/rfctl/update_config.py`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.0.0/setup.py` & `refunc-cli-1.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages
 
 os.chdir(os.path.dirname(sys.argv[0]) or ".")
 here = os.path.abspath(os.path.dirname(__file__))
 
 setup_args = dict(
     name='refunc-cli',
-    version='1.0.0',
+    version='1.1.0',
     description='refunc command line tools',
     author='arvin',
     license='MIT',
     url='https://github.com/refunc/refunc-cli',
     author_email='arvintian8@gamil.com',
     packages=find_packages(),
     include_package_data=True,
```


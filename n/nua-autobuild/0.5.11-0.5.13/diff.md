# Comparing `tmp/nua_autobuild-0.5.11.tar.gz` & `tmp/nua_autobuild-0.5.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nua_autobuild-0.5.11.tar", max compression
+gzip compressed data, was "nua_autobuild-0.5.13.tar", max compression
```

## Comparing `nua_autobuild-0.5.11.tar` & `nua_autobuild-0.5.13.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      454 2023-01-16 17:32:32.163238 nua_autobuild-0.5.11/README.md
--rw-r--r--   0        0        0     1489 2023-04-18 16:55:06.696649 nua_autobuild-0.5.11/pyproject.toml
--rw-r--r--   0        0        0      100 2022-12-12 07:55:21.315857 nua_autobuild-0.5.11/src/nua/autobuild/__init__.py
--rw-r--r--   0        0        0      209 2023-02-28 08:14:12.792663 nua_autobuild-0.5.11/src/nua/autobuild/builders/Dockerfile_nua_builder_node14
--rw-r--r--   0        0        0      209 2023-02-28 08:14:12.793610 nua_autobuild-0.5.11/src/nua/autobuild/builders/Dockerfile_nua_builder_node16
--rw-r--r--   0        0        0      208 2023-02-28 08:14:12.794118 nua_autobuild-0.5.11/src/nua/autobuild/builders/Dockerfile_nua_builder_ruby27
--rw-r--r--   0        0        0      208 2023-02-28 08:14:12.794341 nua_autobuild-0.5.11/src/nua/autobuild/builders/Dockerfile_nua_builder_ruby272
--rw-r--r--   0        0        0      208 2023-02-28 08:14:12.794590 nua_autobuild-0.5.11/src/nua/autobuild/builders/Dockerfile_nua_builder_ruby31
--rw-r--r--   0        0        0      208 2023-02-28 08:14:12.794704 nua_autobuild-0.5.11/src/nua/autobuild/builders/Dockerfile_nua_builder_ruby32
--rw-r--r--   0        0        0        0 2023-02-28 08:14:12.794746 nua_autobuild-0.5.11/src/nua/autobuild/builders/__init__.py
--rw-r--r--   0        0        0      309 2023-02-28 08:14:12.795139 nua_autobuild-0.5.11/src/nua/autobuild/builders/node14.json
--rw-r--r--   0        0        0      309 2023-02-28 08:14:12.795558 nua_autobuild-0.5.11/src/nua/autobuild/builders/node16.json
--rw-r--r--   0        0        0      245 2023-02-28 08:14:12.795648 nua_autobuild-0.5.11/src/nua/autobuild/builders/ruby27.json
--rw-r--r--   0        0        0      225 2023-02-28 08:14:12.795727 nua_autobuild-0.5.11/src/nua/autobuild/builders/ruby272.json
--rw-r--r--   0        0        0      245 2023-02-28 08:14:12.795791 nua_autobuild-0.5.11/src/nua/autobuild/builders/ruby31.json
--rw-r--r--   0        0        0      245 2023-02-28 08:14:12.795854 nua_autobuild-0.5.11/src/nua/autobuild/builders/ruby32.json
--rw-r--r--   0        0        0      340 2023-04-17 20:51:18.651586 nua_autobuild-0.5.11/src/nua/autobuild/constants.py
--rw-r--r--   0        0        0     6145 2023-04-18 14:45:14.191295 nua_autobuild-0.5.11/src/nua/autobuild/docker_build_utils.py
--rw-r--r--   0        0        0      225 2023-02-06 17:21:30.495528 nua_autobuild-0.5.11/src/nua/autobuild/dockerfiles/Dockerfile_nua_builder_slim
--rw-r--r--   0        0        0     1556 2022-12-12 07:55:21.316202 nua_autobuild-0.5.11/src/nua/autobuild/dockerfiles/Dockerfile_nua_python_slim
--rw-r--r--   0        0        0        0 2022-12-20 18:49:45.394740 nua_autobuild-0.5.11/src/nua/autobuild/dockerfiles/__init__.py
--rw-r--r--   0        0        0     1651 2023-04-16 21:09:47.366763 nua_autobuild-0.5.11/src/nua/autobuild/main.py
--rw-r--r--   0        0        0     6604 2023-04-16 21:09:47.366818 nua_autobuild-0.5.11/src/nua/autobuild/nua_image_builder.py
--rw-r--r--   0        0        0     5234 2023-04-16 10:25:52.984339 nua_autobuild-0.5.11/src/nua/autobuild/nua_wheel_builder.py
--rw-r--r--   0        0        0     3234 2023-04-16 21:07:08.792194 nua_autobuild-0.5.11/src/nua/autobuild/register_builders.py
--rw-r--r--   0        0        0       85 2022-12-12 07:55:21.316458 nua_autobuild-0.5.11/src/nua/autobuild/version.py
--rw-r--r--   0        0        0     1153 1970-01-01 00:00:00.000000 nua_autobuild-0.5.11/PKG-INFO
+-rw-r--r--   0        0        0      805 2023-04-24 21:25:56.858863 nua_autobuild-0.5.13/README.md
+-rw-r--r--   0        0        0     1489 2023-04-24 21:27:50.225404 nua_autobuild-0.5.13/pyproject.toml
+-rw-r--r--   0        0        0      100 2022-12-12 07:55:21.315857 nua_autobuild-0.5.13/src/nua/autobuild/__init__.py
+-rw-r--r--   0        0        0      209 2023-02-28 08:14:12.792663 nua_autobuild-0.5.13/src/nua/autobuild/builders/Dockerfile_nua_builder_node14
+-rw-r--r--   0        0        0      209 2023-02-28 08:14:12.793610 nua_autobuild-0.5.13/src/nua/autobuild/builders/Dockerfile_nua_builder_node16
+-rw-r--r--   0        0        0      208 2023-02-28 08:14:12.794118 nua_autobuild-0.5.13/src/nua/autobuild/builders/Dockerfile_nua_builder_ruby27
+-rw-r--r--   0        0        0      208 2023-02-28 08:14:12.794341 nua_autobuild-0.5.13/src/nua/autobuild/builders/Dockerfile_nua_builder_ruby272
+-rw-r--r--   0        0        0      208 2023-02-28 08:14:12.794590 nua_autobuild-0.5.13/src/nua/autobuild/builders/Dockerfile_nua_builder_ruby31
+-rw-r--r--   0        0        0      208 2023-02-28 08:14:12.794704 nua_autobuild-0.5.13/src/nua/autobuild/builders/Dockerfile_nua_builder_ruby32
+-rw-r--r--   0        0        0        0 2023-02-28 08:14:12.794746 nua_autobuild-0.5.13/src/nua/autobuild/builders/__init__.py
+-rw-r--r--   0        0        0      309 2023-02-28 08:14:12.795139 nua_autobuild-0.5.13/src/nua/autobuild/builders/node14.json
+-rw-r--r--   0        0        0      309 2023-02-28 08:14:12.795558 nua_autobuild-0.5.13/src/nua/autobuild/builders/node16.json
+-rw-r--r--   0        0        0      245 2023-02-28 08:14:12.795648 nua_autobuild-0.5.13/src/nua/autobuild/builders/ruby27.json
+-rw-r--r--   0        0        0      225 2023-02-28 08:14:12.795727 nua_autobuild-0.5.13/src/nua/autobuild/builders/ruby272.json
+-rw-r--r--   0        0        0      245 2023-02-28 08:14:12.795791 nua_autobuild-0.5.13/src/nua/autobuild/builders/ruby31.json
+-rw-r--r--   0        0        0      245 2023-02-28 08:14:12.795854 nua_autobuild-0.5.13/src/nua/autobuild/builders/ruby32.json
+-rw-r--r--   0        0        0      340 2023-04-17 20:51:18.651586 nua_autobuild-0.5.13/src/nua/autobuild/constants.py
+-rw-r--r--   0        0        0     6231 2023-04-24 21:25:56.860466 nua_autobuild-0.5.13/src/nua/autobuild/docker_build_utils.py
+-rw-r--r--   0        0        0      225 2023-02-06 17:21:30.495528 nua_autobuild-0.5.13/src/nua/autobuild/dockerfiles/Dockerfile_nua_builder_slim
+-rw-r--r--   0        0        0     1556 2022-12-12 07:55:21.316202 nua_autobuild-0.5.13/src/nua/autobuild/dockerfiles/Dockerfile_nua_python_slim
+-rw-r--r--   0        0        0        0 2022-12-20 18:49:45.394740 nua_autobuild-0.5.13/src/nua/autobuild/dockerfiles/__init__.py
+-rw-r--r--   0        0        0     1651 2023-04-16 21:09:47.366763 nua_autobuild-0.5.13/src/nua/autobuild/main.py
+-rw-r--r--   0        0        0     6604 2023-04-16 21:09:47.366818 nua_autobuild-0.5.13/src/nua/autobuild/nua_image_builder.py
+-rw-r--r--   0        0        0     5234 2023-04-16 10:25:52.984339 nua_autobuild-0.5.13/src/nua/autobuild/nua_wheel_builder.py
+-rw-r--r--   0        0        0     3233 2023-04-24 21:25:56.860659 nua_autobuild-0.5.13/src/nua/autobuild/register_builders.py
+-rw-r--r--   0        0        0       85 2022-12-12 07:55:21.316458 nua_autobuild-0.5.13/src/nua/autobuild/version.py
+-rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 nua_autobuild-0.5.13/PKG-INFO
```

### Comparing `nua_autobuild-0.5.11/pyproject.toml` & `nua_autobuild-0.5.13/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "nua-autobuild"
-version = "0.5.11"
+version = "0.5.13"
 description = "Nua self builder"
 authors = ["Stefane Fermigier <sf@abilian.com>", "Jerome Dumonteil <jd@abilian.com>"]
 license = "AGPL"
 readme = "README.md"
 packages = [
   { include = "nua", from = "src" }
 ]
 
 [tool.poetry.scripts]
 nua-self-build = "nua.autobuild.main:app"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 setuptools = "*"
-nua-lib = "=0.5.11"
-nua-agent = "=0.5.11"
+nua-lib = "=0.5.13"
+nua-agent = "=0.5.13"
 tomli = "^2.0.1"
 tomli-w = "^1.0.0"
 docker = "^6.0"
 paramiko = "*"
 typer = {version = "^0.7.0", extras = ["all"]}
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `nua_autobuild-0.5.11/src/nua/autobuild/docker_build_utils.py` & `nua_autobuild-0.5.13/src/nua/autobuild/docker_build_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,54 +4,55 @@
 from functools import wraps
 
 import docker
 from docker import DockerClient
 from docker.errors import APIError, BuildError, ImageNotFound
 from docker.models.images import Image
 from docker.utils.json_stream import json_stream
-from nua.lib.console import print_blue_bright_no_lf, print_red
-from nua.lib.panic import Abort, print_log_stream, vprint, vprint_magenta
+from nua.lib.panic import Abort, debug, important, print_stream, red_line, vprint
 from nua.lib.tool.state import verbosity, verbosity_level
 
 LOCAL_CONFIG = {"size_unit_MiB": False}
 RE_SUCCESS = re.compile(r"(^Successfully built |sha256:)([0-9a-f]+)$")
 
 
-def vprint_log_stream(docker_log: list):
-    for line in docker_log:
-        if "stream" in line:
-            vprint("    ", line["stream"].strip())
+# def vprint_log_stream(docker_log: list):
+#     for line in docker_log:
+#         if "stream" in line:
+#             vprint("    ", line["stream"].strip())
 
 
 def docker_build_log_error(func):
     @wraps(func)
     def build_log_error_wrapper(*args, **kwargs):
         try:
             return func(*args, **kwargs)
 
         except BuildError as e:
-            print_red("=" * 60)
-            print_red("Something went wrong with image build!")
-            print_red(str(e))
-            print_red("=" * 60)
+            with verbosity(0):
+                red_line("=" * 60)
+                red_line("Something went wrong with image build!")
+                red_line(str(e))
+                red_line("=" * 60)
             raise Abort("Exiting.")
 
         except APIError as e:
-            message = ["=" * 60]
-            message.append("Something went wrong with image build!")
-            if e.is_client_error():
-                message.append(f"{e.response.status_code} Client Error")
-            elif e.is_server_error():
-                message.append(f"{e.response.status_code} Server Error")
-            message.append(f"URL: {e.response.url}")
-            message.append(f"Reason: {e.response.reason}")
-            message.append(f"Explanation: {e.explanation}")
-            message.append("=" * 60)
-            for line in message:
-                print_red(line)
+            with verbosity(0):
+                message = ["=" * 60]
+                message.append("Something went wrong with image build!")
+                if e.is_client_error():
+                    message.append(f"{e.response.status_code} Client Error")
+                elif e.is_server_error():
+                    message.append(f"{e.response.status_code} Server Error")
+                message.append(f"URL: {e.response.url}")
+                message.append(f"Reason: {e.response.reason}")
+                message.append(f"Explanation: {e.explanation}")
+                message.append("=" * 60)
+                for line in message:
+                    red_line(line)
             raise Abort("Exiting.")
 
     return build_log_error_wrapper
 
 
 def image_created_as_iso(image):
     return image.attrs["Created"][:19]
@@ -75,19 +76,19 @@
     image = docker_require(reference)
     if not image:
         return {}
     return image.labels
 
 
 def display_docker_img(image_name: str):
-    vprint_magenta(f"Docker image for '{image_name}':")
+    important(f"Docker image for '{image_name}':")
     client = DockerClient.from_env()
     result = client.images.list(filters={"reference": image_name})
     if not result:
-        vprint("No image found")
+        red_line("No image found")
         return
     for img in result:
         display_one_docker_img(img)
 
 
 def display_one_docker_img(image: Image):
     sid = image.id.split(":")[-1][:10]
@@ -107,15 +108,15 @@
 
 def docker_remove_locally(reference: str):
     client = DockerClient.from_env()
     try:
         image = client.images.get(reference)
         if image:
             with verbosity(3):
-                vprint(f"Image '{reference}' found in local Docker instance: remove it")
+                debug(f"Image '{reference}' found in local Docker instance: remove it")
             client.images.remove(image=image.id, force=True, noprune=False)
     except (APIError, ImageNotFound):
         pass
 
 
 def docker_get_locally(reference: str) -> Image | None:
     client = DockerClient.from_env()
@@ -147,15 +148,16 @@
 
 
 def _print_buffer_log(messages: list[str]):
     """Print messages buffered, without checking for verbosity.
 
     Dump retained messages when an error occured."""
     for message in messages:
-        print_blue_bright_no_lf(message)
+        with verbosity(0):
+            print_stream(message)
 
 
 def _docker_stream_chunk(
     chunk: dict,
     messages_buffer: list[str],
     result: dict,
 ) -> None:
@@ -164,15 +166,15 @@
         raise BuildError(chunk["error"], "")
     result["last_event"] = chunk
     message = chunk.get("stream")
     if message:
         if match := RE_SUCCESS.search(message):
             result["image_id"] = match.group(2)
         with verbosity(2):
-            print_log_stream(message)
+            print_stream(message)
         if verbosity_level() < 2:
             # store message for printing full log if later an error occurs
             messages_buffer.append(message)
 
 
 def docker_stream_build(
     path: str,
```

### Comparing `nua_autobuild-0.5.11/src/nua/autobuild/dockerfiles/Dockerfile_nua_python_slim` & `nua_autobuild-0.5.13/src/nua/autobuild/dockerfiles/Dockerfile_nua_python_slim`

 * *Files identical despite different names*

### Comparing `nua_autobuild-0.5.11/src/nua/autobuild/main.py` & `nua_autobuild-0.5.13/src/nua/autobuild/main.py`

 * *Files identical despite different names*

### Comparing `nua_autobuild-0.5.11/src/nua/autobuild/nua_image_builder.py` & `nua_autobuild-0.5.13/src/nua/autobuild/nua_image_builder.py`

 * *Files identical despite different names*

### Comparing `nua_autobuild-0.5.11/src/nua/autobuild/nua_wheel_builder.py` & `nua_autobuild-0.5.13/src/nua/autobuild/nua_wheel_builder.py`

 * *Files identical despite different names*

### Comparing `nua_autobuild-0.5.11/src/nua/autobuild/register_builders.py` & `nua_autobuild-0.5.13/src/nua/autobuild/register_builders.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Dockerfile.
 """
 import json
 from importlib import resources as rso
 from importlib.abc import Traversable
 from pprint import pformat
 
-from nua.lib.panic import vprint, vprint_magenta
+from nua.lib.panic import bold_debug, debug, warning
 from nua.lib.tool.state import verbosity
 
 
 def is_builder(name: str) -> bool:
     register_builders()
     return name in builder_registry.builder_names
 
@@ -58,17 +58,17 @@
             for file in rso.files(dir).iterdir():
                 if not file.is_file():
                     continue
                 records[file.name] = file
         return records
 
     def show_builders_info(self) -> None:
-        vprint_magenta("Builders registered:")
-        vprint("BUILDERS_DIRS:", pformat(self.builders_dirs))
-        vprint("BUILDERS:", pformat(self.builders))
+        bold_debug("Builders registered:")
+        debug("BUILDERS_DIRS:", pformat(self.builders_dirs))
+        debug("BUILDERS:", pformat(self.builders))
 
     def load_builder_configs(self, records: dict[str, Traversable]) -> None:
         for name, file in records.items():
             if name.startswith("_") or not name.endswith(".json"):
                 continue
             builder_config = json.loads(file.read_text(encoding="utf8"))
             if not builder_config or "app_id" not in builder_config:
@@ -76,15 +76,15 @@
             docker_file = self.read_docker_file(records, builder_config)
             self.register_builder_config(builder_config, docker_file)
 
     def read_docker_file(
         self, records: dict[str, Traversable], builder_config: dict
     ) -> str:
         if builder_config["container"] != "docker":
-            vprint("Only Docker builders are currently supported.")
+            warning("Only Docker builders are currently supported.")
             return ""
         return records[builder_config["dockerfile"]].read_text(encoding="utf8")
 
     def register_builder_config(self, builder_config: dict, docker_file: str):
         app_id = builder_config["app_id"]
         labels = builder_config["labels"]
         self.builders[app_id] = {
```


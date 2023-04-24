# Comparing `tmp/nua_build-0.5.11.tar.gz` & `tmp/nua_build-0.5.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nua_build-0.5.11.tar", max compression
+gzip compressed data, was "nua_build-0.5.13.tar", max compression
```

## Comparing `nua_build-0.5.11.tar` & `nua_build-0.5.13.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     2906 2023-04-05 18:16:53.727915 nua_build-0.5.11/README.md
--rw-r--r--   0        0        0     1697 2023-04-18 16:55:10.808361 nua_build-0.5.11/pyproject.toml
--rw-r--r--   0        0        0      208 2022-11-17 17:42:00.898773 nua_build-0.5.11/src/nua/build/__init__.py
--rw-r--r--   0        0        0       86 2023-01-06 12:47:38.576197 nua_build-0.5.11/src/nua/build/__main__.py
--rw-r--r--   0        0        0     2864 2023-04-08 16:30:34.934589 nua_build-0.5.11/src/nua/build/archive_search.py
--rw-r--r--   0        0        0      323 2023-04-16 17:02:10.325031 nua_build-0.5.11/src/nua/build/builders/__init__.py
--rw-r--r--   0        0        0     2311 2023-04-16 17:02:49.204408 nua_build-0.5.11/src/nua/build/builders/base.py
--rw-r--r--   0        0        0     7437 2023-04-16 21:09:47.366876 nua_build-0.5.11/src/nua/build/builders/docker.py
--rw-r--r--   0        0        0     2367 2023-04-16 17:03:59.696210 nua_build-0.5.11/src/nua/build/builders/factory.py
--rw-r--r--   0        0        0     2455 2023-04-16 17:04:27.640836 nua_build-0.5.11/src/nua/build/builders/wrap.py
--rw-r--r--   0        0        0      178 2022-12-20 18:49:45.395907 nua_build-0.5.11/src/nua/build/config.py
--rw-r--r--   0        0        0        0 2022-12-20 18:49:45.396072 nua_build-0.5.11/src/nua/build/default_conf/__init__.py
--rw-r--r--   0        0        0       65 2022-12-20 18:49:45.396131 nua_build-0.5.11/src/nua/build/default_conf/config.toml
--rw-r--r--   0        0        0      151 2023-01-19 17:57:22.672446 nua_build-0.5.11/src/nua/build/defaults/Dockerfile
--rw-r--r--   0        0        0       76 2022-12-03 19:23:00.336307 nua_build-0.5.11/src/nua/build/defaults/__init__.py
--rw-r--r--   0        0        0     1970 2023-04-16 15:14:14.157924 nua_build-0.5.11/src/nua/build/main.py
--rw-r--r--   0        0        0        0 2022-11-17 17:42:00.899795 nua_build-0.5.11/src/nua/build/scripts/__init__.py
--rw-r--r--   0        0        0     1750 2023-04-08 16:32:16.237367 nua_build-0.5.11/src/nua/build/scripts/test_replace_domain.py
--rw-r--r--   0        0        0       81 2022-11-17 17:42:00.900100 nua_build-0.5.11/src/nua/build/version.py
--rw-r--r--   0        0        0     3660 1970-01-01 00:00:00.000000 nua_build-0.5.11/PKG-INFO
+-rw-r--r--   0        0        0     3241 2023-04-24 21:25:56.860904 nua_build-0.5.13/README.md
+-rw-r--r--   0        0        0     1810 2023-04-24 21:27:54.721199 nua_build-0.5.13/pyproject.toml
+-rw-r--r--   0        0        0      208 2022-11-17 17:42:00.898773 nua_build-0.5.13/src/nua/build/__init__.py
+-rw-r--r--   0        0        0       86 2023-01-06 12:47:38.576197 nua_build-0.5.13/src/nua/build/__main__.py
+-rw-r--r--   0        0        0     2864 2023-04-08 16:30:34.934589 nua_build-0.5.13/src/nua/build/archive_search.py
+-rw-r--r--   0        0        0      323 2023-04-16 17:02:10.325031 nua_build-0.5.13/src/nua/build/builders/__init__.py
+-rw-r--r--   0        0        0     3074 2023-04-24 21:25:56.862074 nua_build-0.5.13/src/nua/build/builders/base.py
+-rw-r--r--   0        0        0     7471 2023-04-24 21:25:56.862204 nua_build-0.5.13/src/nua/build/builders/docker.py
+-rw-r--r--   0        0        0     2455 2023-04-24 21:25:56.862424 nua_build-0.5.13/src/nua/build/builders/factory.py
+-rw-r--r--   0        0        0     2489 2023-04-24 21:25:56.862526 nua_build-0.5.13/src/nua/build/builders/wrap.py
+-rw-r--r--   0        0        0      178 2022-12-20 18:49:45.395907 nua_build-0.5.13/src/nua/build/config.py
+-rw-r--r--   0        0        0        0 2022-12-20 18:49:45.396072 nua_build-0.5.13/src/nua/build/default_conf/__init__.py
+-rw-r--r--   0        0        0       65 2022-12-20 18:49:45.396131 nua_build-0.5.13/src/nua/build/default_conf/config.toml
+-rw-r--r--   0        0        0      151 2023-01-19 17:57:22.672446 nua_build-0.5.13/src/nua/build/defaults/Dockerfile
+-rw-r--r--   0        0        0       76 2022-12-03 19:23:00.336307 nua_build-0.5.13/src/nua/build/defaults/__init__.py
+-rw-r--r--   0        0        0     1883 2023-04-24 21:25:56.862754 nua_build-0.5.13/src/nua/build/main.py
+-rw-r--r--   0        0        0        0 2022-11-17 17:42:00.899795 nua_build-0.5.13/src/nua/build/scripts/__init__.py
+-rw-r--r--   0        0        0     1750 2023-04-08 16:32:16.237367 nua_build-0.5.13/src/nua/build/scripts/test_replace_domain.py
+-rw-r--r--   0        0        0       81 2022-11-17 17:42:00.900100 nua_build-0.5.13/src/nua/build/version.py
+-rw-r--r--   0        0        0     3995 1970-01-01 00:00:00.000000 nua_build-0.5.13/PKG-INFO
```

### Comparing `nua_build-0.5.11/README.md` & `nua_build-0.5.13/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Nua-build
 
 Build system for Nua packages.
 
+[Nua](https://nua.rocks/) is an open source, self-hosted cloud platform project (a PaaS - platform as a service).
+
+This packaged is mostly used internally. The main entry point is the `nua` command line tool (see: [Nua on PyPI](https://pypi.org/project/nua/) or [nua-cli on GitHub](https://github.com/abilian/nua/tree/main/nua-cli)).
+
 
 ## Purpose
 
 The `nua-build` package is used to build packages deployable by the Nua orchestrator.
 
 The current version of nua-build builds Docker images for an amd64 Linux environment. There are plans to extend the system to other container and isolation architectures in future releases.
```

### Comparing `nua_build-0.5.11/pyproject.toml` & `nua_build-0.5.13/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nua-build"
-version = "0.5.11"
+version = "0.5.13"
 description = "Nua build package (currently: build, core build, agent)"
 authors = [
     "Stefane Fermigier <sf@abilian.com>",
     "Jerome Dumonteil <jd@abilian.com>",
 ]
 license = "AGPL"
 readme = "README.md"
@@ -16,17 +16,17 @@
 [tool.poetry.scripts]
 nua-build = "nua.build.main:app"
 nua_test_replace_domain = "nua.build.scripts.test_replace_domain:main"
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
-nua-lib = "=0.5.11"
-nua-agent = "=0.5.11"
-nua-autobuild = "=0.5.11"
+nua-lib = "=0.5.13"
+nua-agent = "=0.5.13"
+nua-autobuild = "=0.5.13"
 tomli = "^2.0.1"
 pyyaml = "^6"
 snoop = "^0.4.3"
 typer = {version = "^0.7.0", extras = ["all"]}
 docker = {version = "^6", extras = ["ssh"]}
 
 [tool.poetry.group.dev.dependencies]
@@ -34,23 +34,30 @@
 nox = "*"
 
 types-setuptools = "*"
 types-pyyaml = "*"
 
 # To please poetry
 platformdirs = "<3.0.0"
+devtools = "^0.11.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 # ------------------------------------------------------------------------------
 
 [tool.pytest.ini_options]
-filterwarnings = ["ignore:.*distutils package:DeprecationWarning", "ignore::DeprecationWarning"]
+filterwarnings = [
+    "ignore:.*distutils package:DeprecationWarning",
+    "ignore::DeprecationWarning",
+]
+markers = [
+    "slow: marks tests as slow (deselect with '-m \"not slow\"')",
+]
 
 # ------------------------------------------------------------------------------
 
 [tool.ruff]
 # Do not remove
 
 # ------------------------------------------------------------------------------
```

### Comparing `nua_build-0.5.11/src/nua/build/archive_search.py` & `nua_build-0.5.13/src/nua/build/archive_search.py`

 * *Files identical despite different names*

### Comparing `nua_build-0.5.11/src/nua/build/builders/base.py` & `nua_build-0.5.13/src/nua/build/builders/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import logging
 import tempfile
 from abc import abstractmethod
 from pathlib import Path
 
 from docker.models.images import Image
 from nua.agent.nua_config import NuaConfig
-from nua.lib.panic import info, show, title, vfprint, vprint
+from nua.lib.panic import info, show, title, vfprint, vprint, warning
 from nua.lib.tool.state import verbosity
 
 from .. import config as build_config
 
 logging.basicConfig(level=logging.INFO)
 CLIENT_TIMEOUT = 600
 
@@ -42,14 +42,36 @@
         self.nua_base = ""
         self.build_dir = self.make_build_dir()
 
     @abstractmethod
     def run(self):
         raise NotImplementedError()
 
+    def post_build_notices(self):
+        """Post build analysis and possible usefull information."""
+        self._notice_local_volumes()
+
+    def _notice_local_volumes(self) -> None:
+        bind_volumes = [
+            volume.get("source", "unknown")
+            for volume in self.config.volume
+            if volume.get("type") == "bind"
+        ]
+        if not bind_volumes:
+            return
+        lines = [
+            "Declaration of volume of type Docker 'bind'.",
+            "The contents of these volumes will NOT be deleted when removing the ",
+            "application instance:",
+        ]
+        for volume in bind_volumes:
+            lines.append(f"    {volume}")
+        with verbosity(0):
+            warning("\n".join(lines))
+
     def _title_build(self):
         title(f"Building the image for {self.config.app_id}")
 
     def make_build_dir(self) -> Path:
         build_dir_parent = Path(
             build_config.get("build", {}).get("build_dir", "/var/tmp")  # noqa S108
         )
```

### Comparing `nua_build-0.5.11/src/nua/build/builders/docker.py` & `nua_build-0.5.13/src/nua/build/builders/docker.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 
         self.check_allowed_base_image()
         self.ensure_base_image_profile_availability()
         self.select_base_image()
         self._title_build()
         self.detect_nua_folder()
         self.build_docker_image()
+        self.post_build_notices()
 
     def check_allowed_base_image(self):
         builder = self.config.builder
         if not builder:
             return
         if not is_builder(builder):
             raise BuilderError(f"Unknown Nua builder: '{builder}'")
```

### Comparing `nua_build-0.5.11/src/nua/build/builders/factory.py` & `nua_build-0.5.13/src/nua/build/builders/factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,14 +23,17 @@
 
 @dataclass(frozen=True)
 class BuilderFactory:
     """Factory to create a Builder instance."""
 
     config: NuaConfig
 
+    def __post_init__(self) -> None:
+        assert isinstance(self.config, NuaConfig)
+
     def get_builder(self) -> Builder:
         with verbosity(4):
             vprint(pformat(self.config.as_dict()))
 
         # Not used at this stage
         # container_type = self.detect_container_type()
         build_method = self.detect_build_method()
```

### Comparing `nua_build-0.5.11/src/nua/build/builders/wrap.py` & `nua_build-0.5.13/src/nua/build/builders/wrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         self._title_build()
         # FIXME:
         # if self.container_type != "docker":
         #     raise NotImplementedError(f"Container type '{self.container_type}'")
         self.write_wrap_dockerfile()
         self.build_wrap_with_docker_stream()
         rm_fr(self.build_dir)
+        self.post_build_notices()
 
     def write_wrap_dockerfile(self):
         self.config.dump_json(self.build_dir)
         docker_file = self.build_dir / "Dockerfile"
         if self.config.docker_user:
             content = (
                 "ARG nua_wrap_tag\n"
```

### Comparing `nua_build-0.5.11/src/nua/build/main.py` & `nua_build-0.5.13/src/nua/build/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-"""Script to build a nua package (experimental)
+"""Script to build a nua package
 
 - information come from a mandatory local file: "nua-config" (.toml, .json, .yaml)
 - origin may be a source tar.gz or a git repository or a docker image...
 - build locally or wrap docker image
 
 Note: **currently use "nua-build ..." for command line**.
 See later if move this to "nua ...".
 """
 from typing import Optional
 
 import snoop
 import typer
+
 from nua.lib.panic import Abort
 from nua.lib.tool.state import set_color, set_verbosity
+from nua.agent.nua_config import NuaConfigError
 
 from . import __version__
 from .builders import BuilderError, get_builder
 
 snoop.install()
 
 app = typer.Typer()
@@ -48,34 +50,30 @@
 option_color = typer.Option(True, "--color/--no-color", help="Colorize messages. ")
 
 
 def _version_string() -> None:
     typer.echo(f"nua-build version: {__version__}")
 
 
-# def usage():
-#     _version_string()
-#     typer.echo(
-#         "Usage: nua-build [OPTIONS] COMMAND [ARGS]...\n\n"
-#         "Try 'nua-build --help' for help."
-#     )
-#     raise typer.Exit(0)
-
-
 # @app.callback(invoke_without_command=True)
 @app.command()
 def main(
     # ctx: typer.Context,
     config_file: Optional[str] = argument_config,
     version: Optional[bool] = option_version,
     verbose: int = option_verbose,
     colorize: bool = option_color,
 ) -> None:
     """Nua-build CLI inferface."""
+
     set_verbosity(verbose)
     set_color(colorize)
 
-    builder = get_builder(config_file)
+    try:
+        builder = get_builder(config_file)
+    except NuaConfigError as e:
+        raise Abort(e.args[0])
+
     try:
         builder.run()
     except BuilderError as e:
         raise Abort from e
```

### Comparing `nua_build-0.5.11/src/nua/build/scripts/test_replace_domain.py` & `nua_build-0.5.13/src/nua/build/scripts/test_replace_domain.py`

 * *Files identical despite different names*

### Comparing `nua_build-0.5.11/PKG-INFO` & `nua_build-0.5.13/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: nua-build
-Version: 0.5.11
+Version: 0.5.13
 Summary: Nua build package (currently: build, core build, agent)
 License: AGPL
 Author: Stefane Fermigier
 Author-email: sf@abilian.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: docker[ssh] (>=6,<7)
-Requires-Dist: nua-agent (==0.5.11)
-Requires-Dist: nua-autobuild (==0.5.11)
-Requires-Dist: nua-lib (==0.5.11)
+Requires-Dist: nua-agent (==0.5.13)
+Requires-Dist: nua-autobuild (==0.5.13)
+Requires-Dist: nua-lib (==0.5.13)
 Requires-Dist: pyyaml (>=6,<7)
 Requires-Dist: snoop (>=0.4.3,<0.5.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 # Nua-build
 
 Build system for Nua packages.
 
+[Nua](https://nua.rocks/) is an open source, self-hosted cloud platform project (a PaaS - platform as a service).
+
+This packaged is mostly used internally. The main entry point is the `nua` command line tool (see: [Nua on PyPI](https://pypi.org/project/nua/) or [nua-cli on GitHub](https://github.com/abilian/nua/tree/main/nua-cli)).
+
 
 ## Purpose
 
 The `nua-build` package is used to build packages deployable by the Nua orchestrator.
 
 The current version of nua-build builds Docker images for an amd64 Linux environment. There are plans to extend the system to other container and isolation architectures in future releases.
```


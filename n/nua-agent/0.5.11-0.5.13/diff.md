# Comparing `tmp/nua_agent-0.5.11.tar.gz` & `tmp/nua_agent-0.5.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nua_agent-0.5.11.tar", max compression
+gzip compressed data, was "nua_agent-0.5.13.tar", max compression
```

## Comparing `nua_agent-0.5.11.tar` & `nua_agent-0.5.13.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0      471 2023-04-05 18:16:23.471948 nua_agent-0.5.11/README.md
--rw-r--r--   0        0        0     1436 2023-04-18 16:55:02.165889 nua_agent-0.5.11/pyproject.toml
--rw-r--r--   0        0        0      330 2023-04-06 11:40:42.165489 nua_agent-0.5.11/src/nua/agent/__init__.py
--rw-r--r--   0        0        0     1028 2023-04-18 14:45:14.188589 nua_agent-0.5.11/src/nua/agent/auto_install.py
--rw-r--r--   0        0        0      346 2023-02-28 08:14:12.790866 nua_agent-0.5.11/src/nua/agent/constants.py
--rw-r--r--   0        0        0        0 2023-02-06 17:21:30.492413 nua_agent-0.5.11/src/nua/agent/db/__init__.py
--rw-r--r--   0        0        0     1437 2023-02-06 17:21:30.492736 nua_agent-0.5.11/src/nua/agent/db/db_manager.py
--rw-r--r--   0        0        0     6233 2023-02-13 14:04:49.212138 nua_agent-0.5.11/src/nua/agent/db/mariadb_manager.py
--rw-r--r--   0        0        0     8651 2023-04-14 13:29:17.685138 nua_agent-0.5.11/src/nua/agent/db/postgres_manager.py
--rw-r--r--   0        0        0     2203 2023-02-15 19:18:03.537136 nua_agent-0.5.11/src/nua/agent/db/sqlite_manager.py
--rw-r--r--   0        0        0        0 2023-02-06 17:21:30.493328 nua_agent-0.5.11/src/nua/agent/deps/__init__.py
--rw-r--r--   0        0        0       75 2023-02-06 17:21:30.493417 nua_agent-0.5.11/src/nua/agent/deps/meta_packages.json
--rw-r--r--   0        0        0      173 2023-04-18 14:45:14.188686 nua_agent-0.5.11/src/nua/agent/detectors/__init__.py
--rw-r--r--   0        0        0      362 2023-04-18 14:45:14.188751 nua_agent-0.5.11/src/nua/agent/detectors/base_detector.py
--rw-r--r--   0        0        0      531 2023-04-18 14:45:14.188819 nua_agent-0.5.11/src/nua/agent/detectors/python_source.py
--rw-r--r--   0        0        0      414 2023-04-18 14:45:14.188875 nua_agent-0.5.11/src/nua/agent/detectors/python_wheels.py
--rw-r--r--   0        0        0      497 2023-03-03 15:29:31.726769 nua_agent-0.5.11/src/nua/agent/meta_packages.py
--rw-r--r--   0        0        0    12823 2023-04-16 21:09:47.366664 nua_agent-0.5.11/src/nua/agent/nua_config.py
--rw-r--r--   0        0        0      544 2023-04-04 16:08:31.312095 nua_agent-0.5.11/src/nua/agent/nua_tag.py
--rw-r--r--   0        0        0        0 2023-02-06 17:21:30.493877 nua_agent-0.5.11/src/nua/agent/scripts/__init__.py
--rw-r--r--   0        0        0    10292 2023-04-18 14:45:14.189467 nua_agent-0.5.11/src/nua/agent/scripts/app_builder.py
--rw-r--r--   0        0        0     1583 2023-04-08 16:31:17.756437 nua_agent-0.5.11/src/nua/agent/templates.py
--rw-r--r--   0        0        0       81 2023-02-06 17:21:30.494088 nua_agent-0.5.11/src/nua/agent/version.py
--rw-r--r--   0        0        0     1041 1970-01-01 00:00:00.000000 nua_agent-0.5.11/PKG-INFO
+-rw-r--r--   0        0        0      793 2023-04-24 21:25:56.856175 nua_agent-0.5.13/README.md
+-rw-r--r--   0        0        0     1436 2023-04-24 21:27:45.984067 nua_agent-0.5.13/pyproject.toml
+-rw-r--r--   0        0        0      330 2023-04-06 11:40:42.165489 nua_agent-0.5.13/src/nua/agent/__init__.py
+-rw-r--r--   0        0        0     1699 2023-04-24 21:25:56.857554 nua_agent-0.5.13/src/nua/agent/auto_install.py
+-rw-r--r--   0        0        0      346 2023-02-28 08:14:12.790866 nua_agent-0.5.13/src/nua/agent/constants.py
+-rw-r--r--   0        0        0        0 2023-02-06 17:21:30.492413 nua_agent-0.5.13/src/nua/agent/db/__init__.py
+-rw-r--r--   0        0        0     1437 2023-02-06 17:21:30.492736 nua_agent-0.5.13/src/nua/agent/db/db_manager.py
+-rw-r--r--   0        0        0     6233 2023-02-13 14:04:49.212138 nua_agent-0.5.13/src/nua/agent/db/mariadb_manager.py
+-rw-r--r--   0        0        0     8651 2023-04-14 13:29:17.685138 nua_agent-0.5.13/src/nua/agent/db/postgres_manager.py
+-rw-r--r--   0        0        0     2203 2023-02-15 19:18:03.537136 nua_agent-0.5.13/src/nua/agent/db/sqlite_manager.py
+-rw-r--r--   0        0        0        0 2023-02-06 17:21:30.493328 nua_agent-0.5.13/src/nua/agent/deps/__init__.py
+-rw-r--r--   0        0        0       75 2023-02-06 17:21:30.493417 nua_agent-0.5.13/src/nua/agent/deps/meta_packages.json
+-rw-r--r--   0        0        0        0 2023-04-24 21:25:56.857636 nua_agent-0.5.13/src/nua/agent/detectors/__init__.py
+-rw-r--r--   0        0        0     1114 2023-04-24 21:25:56.857882 nua_agent-0.5.13/src/nua/agent/detectors/base_detector.py
+-rw-r--r--   0        0        0      950 2023-04-24 21:25:56.857950 nua_agent-0.5.13/src/nua/agent/detectors/nodejs_yarn.py
+-rw-r--r--   0        0        0      646 2023-04-24 21:25:56.858041 nua_agent-0.5.13/src/nua/agent/detectors/python_source.py
+-rw-r--r--   0        0        0      567 2023-04-24 21:25:56.858137 nua_agent-0.5.13/src/nua/agent/detectors/python_wheels.py
+-rw-r--r--   0        0        0      497 2023-03-03 15:29:31.726769 nua_agent-0.5.13/src/nua/agent/meta_packages.py
+-rw-r--r--   0        0        0    13027 2023-04-24 21:25:56.858265 nua_agent-0.5.13/src/nua/agent/nua_config.py
+-rw-r--r--   0        0        0      544 2023-04-04 16:08:31.312095 nua_agent-0.5.13/src/nua/agent/nua_tag.py
+-rw-r--r--   0        0        0        0 2023-02-06 17:21:30.493877 nua_agent-0.5.13/src/nua/agent/scripts/__init__.py
+-rw-r--r--   0        0        0    11212 2023-04-24 21:25:56.858401 nua_agent-0.5.13/src/nua/agent/scripts/app_builder.py
+-rw-r--r--   0        0        0     1583 2023-04-08 16:31:17.756437 nua_agent-0.5.13/src/nua/agent/templates.py
+-rw-r--r--   0        0        0       81 2023-02-06 17:21:30.494088 nua_agent-0.5.13/src/nua/agent/version.py
+-rw-r--r--   0        0        0     1363 1970-01-01 00:00:00.000000 nua_agent-0.5.13/PKG-INFO
```

### Comparing `nua_agent-0.5.11/pyproject.toml` & `nua_agent-0.5.13/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nua-agent"
-version = "0.5.11"
+version = "0.5.13"
 description = "Nua agent"
 authors = [
     "Stefane Fermigier <sf@abilian.com>",
     "Jerome Dumonteil <jd@abilian.com>",
 ]
 license = "AGPL"
 readme = "README.md"
@@ -12,15 +12,15 @@
     { include = "nua", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 setuptools = "*"
 packaging = "*"
-nua-lib = "=0.5.11"
+nua-lib = "=0.5.13"
 tomli = "^2.0.1"
 pyyaml = "^6.0"
 
 [tool.poetry.group.dev.dependencies]
 abilian-devtools = "*"
 nox = "*"
 types-setuptools = "*"
```

### Comparing `nua_agent-0.5.11/src/nua/agent/db/db_manager.py` & `nua_agent-0.5.13/src/nua/agent/db/db_manager.py`

 * *Files identical despite different names*

### Comparing `nua_agent-0.5.11/src/nua/agent/db/mariadb_manager.py` & `nua_agent-0.5.13/src/nua/agent/db/mariadb_manager.py`

 * *Files identical despite different names*

### Comparing `nua_agent-0.5.11/src/nua/agent/db/postgres_manager.py` & `nua_agent-0.5.13/src/nua/agent/db/postgres_manager.py`

 * *Files identical despite different names*

### Comparing `nua_agent-0.5.11/src/nua/agent/db/sqlite_manager.py` & `nua_agent-0.5.13/src/nua/agent/db/sqlite_manager.py`

 * *Files identical despite different names*

### Comparing `nua_agent-0.5.11/src/nua/agent/nua_config.py` & `nua_agent-0.5.13/src/nua/agent/nua_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,15 +226,15 @@
             )
         self.metadata["checksum"] = checksum
 
     def _nomalize_env_values(self):
         self._data["env"] = nomalize_env_values(self.env)
 
     def __getitem__(self, key: str) -> Any:
-        """will return {} is key not found, assuming some parts are not
+        """will return {} if key not found, assuming some parts are not
         mandatory and first level element are usually dict."""
         return self._data.get(key) or {}
 
     # metadata ######################################################
 
     @property
     def metadata(self) -> dict:
@@ -392,14 +392,21 @@
 
     # docker env ####################################################
 
     @property
     def docker(self) -> dict:
         return self["docker"]
 
+    # volumes declaration ###########################################
+
+    @property
+    def volume(self) -> list:
+        """The list of declared volumes."""
+        return self._data.get("volume", [])
+
     # resource ######################################################
 
     @property
     def resource(self) -> list:
         """The list of resources (tag 'resource')."""
         return self._data.get("resource", [])
```

### Comparing `nua_agent-0.5.11/src/nua/agent/nua_tag.py` & `nua_agent-0.5.13/src/nua/agent/nua_tag.py`

 * *Files identical despite different names*

### Comparing `nua_agent-0.5.11/src/nua/agent/scripts/app_builder.py` & `nua_agent-0.5.13/src/nua/agent/scripts/app_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,20 +15,26 @@
     apt_remove_lists,
     install_build_packages,
     install_git_source,
     install_meta_packages,
     install_packages,
     install_pip_packages,
     install_source,
+    installed_packages,
 )
 from nua.lib.backports import chdir
-from nua.lib.exec import exec_as_nua
-from nua.lib.panic import Abort, info, show, vprint
+from nua.lib.exec import exec_as_nua, exec_as_root
+from nua.lib.panic import Abort, info, show, vprint, warning
 from nua.lib.shell import chmod_r, chown_r, mkdir_p, rm_fr, sh
-from nua.lib.tool.state import set_verbosity, verbosity, verbosity_level
+from nua.lib.tool.state import (
+    set_packages_updated,
+    set_verbosity,
+    verbosity,
+    verbosity_level,
+)
 
 from ..auto_install import detect_and_install
 from ..constants import (
     NUA_APP_PATH,
     NUA_BUILD_PATH,
     NUA_METADATA_PATH,
     NUA_SCRIPTS_PATH,
@@ -45,14 +51,15 @@
     """Class to hold config and other state information during build."""
 
     def __init__(self):
         if "nua_verbosity" in os.environ:
             set_verbosity(int(os.environ["nua_verbosity"]))
             with verbosity(3):
                 info("verbosity:", verbosity_level())
+        set_packages_updated(False)
 
         self.build_dir = Path(NUA_BUILD_PATH)
         if not self.build_dir.is_dir():
             raise Abort(f"Build directory does not exist: '{self.build_dir}'")
 
         chdir(self.build_dir)
         self.config = NuaConfig(self.build_dir)
@@ -60,32 +67,23 @@
 
     def build(self):
         self.make_dirs()
         with chdir(self.config.root_dir):
             self.pre_build()
             with verbosity(1):
                 info("******** Stage: build")
-            with install_build_packages(self.config.build_packages):
+            with install_build_packages(
+                self.config.build_packages,
+                installed=installed_packages(),
+            ):
                 code_installed = self.install_project_code()
-                pip_installed = install_pip_packages(self.config.pip_install)
-                built = False
-                if code_installed:
-                    built = detect_and_install(self.source)
-                if not any((pip_installed, code_installed)):
-                    # no package installed through install_pip_packages and
-                    # no other way. Let's assume there is a local project.
-                    show("Try install from some local project")
-                    built = detect_and_install(".")
-                if (code_installed or pip_installed or built) and os.getuid() == 0:
+                chown_r("/nua/build", "nua")
+                built = self.run_build_script(code_installed)
+                if (code_installed or built) and os.getuid() == 0:
                     chown_r("/nua/build", "nua")
-                # if code_installed:
-                # always run build script: maybe no code source,
-                # but only configuration of standard .deb packages
-                self.run_build_script()
-
         self.post_build()
         self.test_build()
         with verbosity(1):
             show("******** Build done.")
 
     def infer_meta_packages(self) -> list:
         """Return packages inferred from the nua-config requirements."""
@@ -153,15 +151,18 @@
         path = self.find_start_script()
         if path:
             with verbosity(2):
                 vprint("Copying start script:", path)
             copy2(path, script_dir)
             return
         with verbosity(2):
-            vprint("Writing debug start script")
+            warning(
+                "Neither start script or start-command found.\n"
+                "Writing a debug start script showing container's environment."
+            )
             return self._write_start_script(script_dir, ["env"])
 
     def _write_start_script(self, script_dir: Path, start_cmd: list):
         data = deepcopy(self.config.metadata_rendered)
         cwd = repr(str(self.source))
         cmd = dedent(
             f"""\
@@ -199,44 +200,70 @@
         path = path.absolute().resolve()
         if path.is_file():
             with verbosity(3):
                 info(f"found build script: {path}")
             return path
         return None
 
-    def run_build_script(self):
+    def run_build_script(self, code_installed: bool) -> bool:
         """Process the 'build.py' script if exists or the build-command.
 
         The script is run from the directory of the nua-config.toml
         file.
         """
+        pip_installed = install_pip_packages(self.config.pip_install)
         if self.config.build_command:
-            return self.build_command()
-        script_path = self.find_build_script()
-        if not script_path:
-            return
-        # assuming it is a python script
-        env = dict(os.environ)
-        with verbosity(2):
-            cmd = "python --version"
-            sh(cmd, env=env)
-        cmd = f"python {script_path}"
-        sh(cmd, env=env, timeout=1800)
+            return self.build_with_command()
+        if script_path := self.find_build_script():
+            return self.build_with_script(script_path)
+        return self.build_with_auto_detection(code_installed, pip_installed)
 
-    def build_command(self):
+    def build_with_command(self) -> bool:
         """Process the 'build-command' commands.
 
         The script is run from the source directory.
         """
-        if not self.config.build_command:
-            return
         with chdir(self.source):
             with verbosity(2):
                 show("Execution of build-command")
-            exec_as_nua(self.config.build_command)
+            env = dict(os.environ)
+            if self.config.build.get("build-as-root", False):
+                exec_as_root(self.config.build_command, env=env, timeout=1800)
+            else:
+                exec_as_nua(self.config.build_command, env=env, timeout=1800)
+        return True
+
+    def build_with_script(self, script_path: Path) -> bool:
+        """Build with a python script."""
+        env = dict(os.environ)
+        cmd = f"python {script_path}"
+        if self.config.build.get("build-as-root", False):
+            exec_as_root(cmd, env=env, timeout=1800)
+        else:
+            exec_as_nua(cmd, env=env, timeout=1800)
+        return True
+
+    def build_with_auto_detection(
+        self,
+        code_installed: bool,
+        pip_installed: bool,
+    ) -> bool:
+        """Build with a auto detect/install.
+
+        Rem: detect_and_install() is launched as root (the current user),
+             it's the responsability of auto installer to switch to user nua.
+        """
+        if code_installed:
+            return detect_and_install(self.source)
+        if not any((pip_installed, code_installed)):
+            # no package installed through install_pip_packages and
+            # no other way. Let's assume there is a local project.
+            show("Try install from some local project")
+            return detect_and_install(".")
+        return False
 
     def install_project_code(self) -> bool:
         installed = False
         if self.config.src_url:
             self.source = install_source(
                 self.config.src_url,
                 "/nua/build",
```

### Comparing `nua_agent-0.5.11/src/nua/agent/templates.py` & `nua_agent-0.5.13/src/nua/agent/templates.py`

 * *Files identical despite different names*

### Comparing `nua_agent-0.5.11/PKG-INFO` & `nua_agent-0.5.13/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 Metadata-Version: 2.1
 Name: nua-agent
-Version: 0.5.11
+Version: 0.5.13
 Summary: Nua agent
 License: AGPL
 Author: Stefane Fermigier
 Author-email: sf@abilian.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: nua-lib (==0.5.11)
+Requires-Dist: nua-lib (==0.5.13)
 Requires-Dist: packaging
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: setuptools
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Nua Agent
 
+[Nua](https://nua.rocks/) is an open source, self-hosted cloud platform project (a PaaS - platform as a service).
+
+This packaged is used internally. The main entry point is the `nua` command line tool (see: [Nua on PyPI](https://pypi.org/project/nua/) or [nua-cli on GitHub](https://github.com/abilian/nua/tree/main/nua-cli)).
+
 The `nua-agent` package is included in every Nua application image.
 
 It will provide the following features (TBC):
 
 -   Application licycle management
 -   Smoke tests and health checks
 -   Logging and monitoring
 
 ## Content
 
 `nua-agent` provides:
 
--   `nua_config`: library to read the embedded `nua-config` file (introspection),
--   `app_builder`: actual builder of the application inside the Docker image.
--   `db`: collection of tools to manage databases
+- `nua_config`: library to read the embedded `nua-config` file (introspection),
+- `app_builder`: actual builder of the application inside the Docker image.
+- `db`: collection of tools to manage databases
```


# Comparing `tmp/pyproject-generator-0.0.3.tar.gz` & `tmp/pyproject-generator-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject-generator-0.0.3.tar", last modified: Sun Apr 16 17:45:19 2023, max compression
+gzip compressed data, was "pyproject-generator-0.0.4.tar", last modified: Mon Apr 24 15:30:19 2023, max compression
```

## Comparing `pyproject-generator-0.0.3.tar` & `pyproject-generator-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-16 17:45:19.609700 pyproject-generator-0.0.3/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1159 2023-04-16 17:45:19.609886 pyproject-generator-0.0.3/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)      640 2023-04-13 21:07:05.000000 pyproject-generator-0.0.3/README.md
--rw-r--r--   0 cangyuanli   (501) staff       (20)      232 2023-04-12 22:11:58.000000 pyproject-generator-0.0.3/pyproject.toml
--rw-r--r--   0 cangyuanli   (501) staff       (20)      834 2023-04-16 17:45:19.611256 pyproject-generator-0.0.3/setup.cfg
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-16 17:45:19.570465 pyproject-generator-0.0.3/src/
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-16 17:45:19.580610 pyproject-generator-0.0.3/src/pyproject/
--rw-r--r--   0 cangyuanli   (501) staff       (20)       37 2023-04-13 20:46:07.000000 pyproject-generator-0.0.3/src/pyproject/__init__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)       22 2023-04-16 17:45:10.000000 pyproject-generator-0.0.3/src/pyproject/__version__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)     2361 2023-04-15 15:52:22.000000 pyproject-generator-0.0.3/src/pyproject/cli.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-16 17:45:19.581602 pyproject-generator-0.0.3/src/pyproject/config/
--rw-r--r--   0 cangyuanli   (501) staff       (20)      237 2023-04-16 17:42:35.000000 pyproject-generator-0.0.3/src/pyproject/config/config.json
--rw-r--r--   0 cangyuanli   (501) staff       (20)     7346 2023-04-16 17:44:32.000000 pyproject-generator-0.0.3/src/pyproject/project_builder.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-16 17:45:19.597284 pyproject-generator-0.0.3/src/pyproject/templates/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1477 2023-04-13 18:28:38.000000 pyproject-generator-0.0.3/src/pyproject/templates/gitignore.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      231 2023-04-12 23:53:39.000000 pyproject-generator-0.0.3/src/pyproject/templates/pyproject.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      398 2023-04-14 17:01:55.000000 pyproject-generator-0.0.3/src/pyproject/templates/readme.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      578 2023-04-14 17:03:04.000000 pyproject-generator-0.0.3/src/pyproject/templates/setup.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      649 2023-04-13 18:27:11.000000 pyproject-generator-0.0.3/src/pyproject/templates/tests.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      402 2023-04-12 23:45:24.000000 pyproject-generator-0.0.3/src/pyproject/templates/tox.template
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-16 17:45:19.608485 pyproject-generator-0.0.3/src/pyproject_generator.egg-info/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1159 2023-04-16 17:45:19.000000 pyproject-generator-0.0.3/src/pyproject_generator.egg-info/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)      679 2023-04-16 17:45:19.000000 pyproject-generator-0.0.3/src/pyproject_generator.egg-info/SOURCES.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-04-16 17:45:19.000000 pyproject-generator-0.0.3/src/pyproject_generator.egg-info/dependency_links.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       49 2023-04-16 17:45:19.000000 pyproject-generator-0.0.3/src/pyproject_generator.egg-info/entry_points.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       10 2023-04-16 17:45:19.000000 pyproject-generator-0.0.3/src/pyproject_generator.egg-info/top_level.txt
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-16 17:45:19.609307 pyproject-generator-0.0.3/tests/
--rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-12 22:11:58.000000 pyproject-generator-0.0.3/tests/test_pyproject.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-24 15:30:19.862052 pyproject-generator-0.0.4/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1958 2023-04-24 15:30:19.862223 pyproject-generator-0.0.4/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1439 2023-04-19 15:24:26.000000 pyproject-generator-0.0.4/README.md
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      232 2023-04-19 15:24:26.000000 pyproject-generator-0.0.4/pyproject.toml
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      834 2023-04-24 15:30:19.863127 pyproject-generator-0.0.4/setup.cfg
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-24 15:30:19.843238 pyproject-generator-0.0.4/src/
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-24 15:30:19.848259 pyproject-generator-0.0.4/src/pyproject/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       37 2023-04-19 15:24:27.000000 pyproject-generator-0.0.4/src/pyproject/__init__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       22 2023-04-24 15:30:11.000000 pyproject-generator-0.0.4/src/pyproject/__version__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     2570 2023-04-24 14:59:13.000000 pyproject-generator-0.0.4/src/pyproject/cli.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-24 15:30:19.849579 pyproject-generator-0.0.4/src/pyproject/config/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      237 2023-04-19 15:24:27.000000 pyproject-generator-0.0.4/src/pyproject/config/config.json
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      237 2023-04-24 14:54:50.000000 pyproject-generator-0.0.4/src/pyproject/config/default_config.json
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     7975 2023-04-24 15:28:44.000000 pyproject-generator-0.0.4/src/pyproject/project_builder.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-24 15:30:19.856940 pyproject-generator-0.0.4/src/pyproject/templates/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1477 2023-04-13 18:28:38.000000 pyproject-generator-0.0.4/src/pyproject/templates/gitignore.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      231 2023-04-12 23:53:39.000000 pyproject-generator-0.0.4/src/pyproject/templates/pyproject.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      398 2023-04-14 17:01:55.000000 pyproject-generator-0.0.4/src/pyproject/templates/readme.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      578 2023-04-14 17:03:04.000000 pyproject-generator-0.0.4/src/pyproject/templates/setup.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      649 2023-04-13 18:27:11.000000 pyproject-generator-0.0.4/src/pyproject/templates/tests.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      402 2023-04-12 23:45:24.000000 pyproject-generator-0.0.4/src/pyproject/templates/tox.template
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-24 15:30:19.860996 pyproject-generator-0.0.4/src/pyproject_generator.egg-info/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1958 2023-04-24 15:30:19.000000 pyproject-generator-0.0.4/src/pyproject_generator.egg-info/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      720 2023-04-24 15:30:19.000000 pyproject-generator-0.0.4/src/pyproject_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-04-24 15:30:19.000000 pyproject-generator-0.0.4/src/pyproject_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       49 2023-04-24 15:30:19.000000 pyproject-generator-0.0.4/src/pyproject_generator.egg-info/entry_points.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       10 2023-04-24 15:30:19.000000 pyproject-generator-0.0.4/src/pyproject_generator.egg-info/top_level.txt
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-24 15:30:19.861671 pyproject-generator-0.0.4/tests/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-19 15:24:26.000000 pyproject-generator-0.0.4/tests/test_pyproject.py
```

### Comparing `pyproject-generator-0.0.3/setup.cfg` & `pyproject-generator-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.3/src/pyproject/cli.py` & `pyproject-generator-0.0.4/src/pyproject/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,20 @@
     parser = argparse.ArgumentParser(description="Generate python project")
 
     parser.add_argument("action", type=str, choices=ACTIONS, help="Action")
     parser.add_argument(
         "project_name", type=str, nargs="?", default=None, help="Name of the project"
     )
 
+    parser.add_argument(
+        "--reset_config",
+        required=False,
+        action="store_true",
+        help="Reset configuration to default settings",
+    )
     parser.add_argument("--pypi_username", type=str, help="Set PyPI username")
     parser.add_argument("--pypi_password", type=str, help="Set PyPI password")
     parser.add_argument("--github_url", type=str, help="Set Github URL")
     parser.add_argument("--author", type=str, help="Set author name")
     parser.add_argument("--email", type=str, help="Set author email")
     parser.add_argument(
         "--set_dependencies",
@@ -64,14 +70,15 @@
         "pypi_password": args.pypi_password,
         "github_url": args.github_url,
         "author": args.author,
         "email": args.email,
         "set_dependencies": args.set_dependencies,
         "add_dependencies": args.add_dependencies,
         "remove_dependencies": args.remove_dependencies,
+        "reset_config": args.reset_config,
     }
 
     builder = ProjectBuilder(project_name=args.project_name, config=config)
     builder.dispatch(action=args.action)
 
 
 if __name__ == "__main__":
```

### Comparing `pyproject-generator-0.0.3/src/pyproject/project_builder.py` & `pyproject-generator-0.0.4/src/pyproject/project_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Imports
 
+import os
 import json
 from pathlib import Path
 import re
 import shutil
 import subprocess
 import string
 from types import SimpleNamespace
@@ -11,15 +12,15 @@
 import venv
 
 Action = Literal["init", "upload", "config"]
 PathLike = Union[Path, str]
 
 BASE_PATH = Path(__file__).resolve().parents[0]
 TEMPLATE_PATH = BASE_PATH / "templates"
-CONFIG_PATH = BASE_PATH / "config/config.json"
+CONFIG_PATH = BASE_PATH / "config"
 
 
 class _EnvBuilder(venv.EnvBuilder):
     def __init__(self, venv_path: PathLike, *args, **kwargs) -> None:
         self.context: Optional[SimpleNamespace] = None
         self.venv_path = Path(venv_path)
         super().__init__(*args, **kwargs)
@@ -56,15 +57,16 @@
         template_path: PathLike = TEMPLATE_PATH,
         config_path: PathLike = CONFIG_PATH,
         config: Optional[dict[str, str]] = None,
     ) -> None:
         if project_name is not None:
             self._validate_project_name(project_name)
             self._project_name = project_name
-            self._project_path = Path(project_name)
+
+        self._project_path = Path().cwd()
 
         self._template_path = Path(template_path)
         self._config_path = Path(config_path)
         self._config = self._set_config(config)
 
     @staticmethod
     def _validate_project_name(project_name: str) -> None:
@@ -144,29 +146,34 @@
         for dep in ("black", "mypy", "build", "tox", "pytest"):
             venv_builder.run_bin_in_venv(["pip", "install", dep])
 
         # Create requirements_dev file
         reqs = venv_builder.run_bin_in_venv(["pip", "freeze"], capture_output=True)
         (self._project_path / "requirements_dev.txt").write_bytes(reqs.stdout)
 
-    def _parse_config_file(self) -> dict:
-        with open(self._config_path) as f:
+    def _parse_config_file(self, filename: PathLike) -> dict:
+        with open(self._config_path / filename) as f:
             config: dict = json.load(f)
 
         return config
 
     @staticmethod
     def _parse_arg_to_set(string: Optional[str], sep: str) -> set[str]:
         if string is None:
             return set()
 
         return set(word.strip() for word in string.split(sep))
 
     def _set_config(self, config: dict[str, str]) -> dict:
-        saved_config = self._parse_config_file()
+        if config["reset_config"]:
+            saved_path = "default_config.json"
+        else:
+            saved_path = "config.json"
+
+        saved_config = self._parse_config_file(saved_path)
 
         if config["set_dependencies"] is None:
             config["dependencies"] = set(saved_config["dependencies"])
         else:
             config["dependencies"] = self._parse_arg_to_set(
                 config["set_dependencies"], sep=","
             )
@@ -194,22 +201,37 @@
         with open(self._config_path, "w") as f:
             json.dump(config, f, indent=4)
 
     def upload(self):
         username = self._config["pypi_username"]
         password = self._config["pypi_password"]
 
+        try:
+            venv_path = Path(os.environ["VIRTUAL_ENV"]) / "bin"
+        except KeyError:
+            venv_path = ""
+
+        # TODO: Make EnvBuilder class capable of handling existing venvs, removing
+        # the need for this duplicate function
+        def run_bin_in_venv(
+            command: list[str], **kwargs
+        ) -> subprocess.CompletedProcess[bytes]:
+            command[0] = Path(venv_path).joinpath(command[0]).as_posix()
+
+            return subprocess.run(command, check=True, **kwargs)
+
         shutil.rmtree(self._project_path / "dist", ignore_errors=True)
-        venv_builder = _EnvBuilder(self._project_path / "venv", with_pip=True)
-        venv_builder.run_python_in_venv(["-m", "build"])
+
+        run_bin_in_venv(["python", "-m", "build"])
+        run_bin_in_venv(["twine", "check", "dist/*"])
 
         if "" in (username, password):
-            venv_builder.run_bin_in_venv(["twine", "upload", "dist/*"])
+            run_bin_in_venv(["twine", "upload", "dist/*"])
         else:
-            venv_builder.run_bin_in_venv(
+            run_bin_in_venv(
                 ["twine", "upload", "dist/*", "-u", username, "-p", password]
             )
 
     def dispatch(self, action: Action):
         if action == "init":
             self.init_project()
         elif action == "upload":
```

### Comparing `pyproject-generator-0.0.3/src/pyproject/templates/gitignore.template` & `pyproject-generator-0.0.4/src/pyproject/templates/gitignore.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.3/src/pyproject/templates/setup.template` & `pyproject-generator-0.0.4/src/pyproject/templates/setup.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.3/src/pyproject/templates/tests.template` & `pyproject-generator-0.0.4/src/pyproject/templates/tests.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.3/src/pyproject_generator.egg-info/SOURCES.txt` & `pyproject-generator-0.0.4/src/pyproject_generator.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 pyproject.toml
 setup.cfg
 src/pyproject/__init__.py
 src/pyproject/__version__.py
 src/pyproject/cli.py
 src/pyproject/project_builder.py
 src/pyproject/config/config.json
+src/pyproject/config/default_config.json
 src/pyproject/templates/gitignore.template
 src/pyproject/templates/pyproject.template
 src/pyproject/templates/readme.template
 src/pyproject/templates/setup.template
 src/pyproject/templates/tests.template
 src/pyproject/templates/tox.template
 src/pyproject_generator.egg-info/PKG-INFO
```


# Comparing `tmp/nua_lib-0.5.13.tar.gz` & `tmp/nua_lib-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nua_lib-0.5.13.tar", max compression
+gzip compressed data, was "nua_lib-0.5.9.tar", max compression
```

## Comparing `nua_lib-0.5.13.tar` & `nua_lib-0.5.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      791 2023-04-24 21:25:56.867782 nua_lib-0.5.13/README.md
--rw-r--r--   0        0        0     1241 2023-04-24 21:27:35.121645 nua_lib-0.5.13/pyproject.toml
--rw-r--r--   0        0        0      218 2023-02-06 17:21:30.499791 nua_lib-0.5.13/src/nua/lib/__init__.py
--rw-r--r--   0        0        0    21879 2023-04-24 21:25:56.869296 nua_lib-0.5.13/src/nua/lib/actions.py
--rw-r--r--   0        0        0      769 2023-01-11 17:39:15.272394 nua_lib-0.5.13/src/nua/lib/backports.py
--rw-r--r--   0        0        0     1621 2023-04-24 21:25:56.869539 nua_lib-0.5.13/src/nua/lib/console.py
--rw-r--r--   0        0        0     5600 2023-03-06 16:13:43.253043 nua_lib-0.5.13/src/nua/lib/exec.py
--rw-r--r--   0        0        0      828 2023-04-08 16:30:34.876808 nua_lib-0.5.13/src/nua/lib/gen_password.py
--rw-r--r--   0        0        0     3361 2023-04-24 21:25:56.869718 nua_lib-0.5.13/src/nua/lib/panic.py
--rw-r--r--   0        0        0     3932 2023-04-08 16:18:44.073176 nua_lib-0.5.13/src/nua/lib/shell.py
--rw-r--r--   0        0        0       60 2023-02-06 17:21:30.499928 nua_lib-0.5.13/src/nua/lib/tool/__init__.py
--rw-r--r--   0        0        0     3572 2023-04-24 21:25:56.869858 nua_lib-0.5.13/src/nua/lib/tool/color_str.py
--rw-r--r--   0        0        0     1420 2023-04-24 21:25:56.870074 nua_lib-0.5.13/src/nua/lib/tool/state.py
--rw-r--r--   0        0        0     2077 2023-03-21 16:25:52.745820 nua_lib-0.5.13/src/nua/lib/unarchiver.py
--rw-r--r--   0        0        0       79 2023-01-03 14:14:59.347734 nua_lib-0.5.13/src/nua/lib/version.py
--rw-r--r--   0        0        0     1275 1970-01-01 00:00:00.000000 nua_lib-0.5.13/PKG-INFO
+-rw-r--r--   0        0        0      544 2023-02-06 17:21:30.498783 nua_lib-0.5.9/README.md
+-rw-r--r--   0        0        0     1240 2023-04-18 16:37:02.790822 nua_lib-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0      218 2023-02-06 17:21:30.499791 nua_lib-0.5.9/src/nua/lib/__init__.py
+-rw-r--r--   0        0        0    21348 2023-04-18 14:45:14.195218 nua_lib-0.5.9/src/nua/lib/actions.py
+-rw-r--r--   0        0        0      769 2023-01-11 17:39:15.272394 nua_lib-0.5.9/src/nua/lib/backports.py
+-rw-r--r--   0        0        0     1344 2023-04-18 14:45:14.195754 nua_lib-0.5.9/src/nua/lib/console.py
+-rw-r--r--   0        0        0     5600 2023-03-06 16:13:43.253043 nua_lib-0.5.9/src/nua/lib/exec.py
+-rw-r--r--   0        0        0      828 2023-04-08 16:30:34.876808 nua_lib-0.5.9/src/nua/lib/gen_password.py
+-rw-r--r--   0        0        0     1948 2023-04-18 14:45:14.196144 nua_lib-0.5.9/src/nua/lib/panic.py
+-rw-r--r--   0        0        0     3932 2023-04-08 16:18:44.073176 nua_lib-0.5.9/src/nua/lib/shell.py
+-rw-r--r--   0        0        0       60 2023-02-06 17:21:30.499928 nua_lib-0.5.9/src/nua/lib/tool/__init__.py
+-rw-r--r--   0        0        0     3509 2023-04-08 16:30:35.028834 nua_lib-0.5.9/src/nua/lib/tool/color_str.py
+-rw-r--r--   0        0        0     1133 2023-02-13 14:04:49.214475 nua_lib-0.5.9/src/nua/lib/tool/state.py
+-rw-r--r--   0        0        0     2077 2023-03-21 16:25:52.745820 nua_lib-0.5.9/src/nua/lib/unarchiver.py
+-rw-r--r--   0        0        0       79 2023-01-03 14:14:59.347734 nua_lib-0.5.9/src/nua/lib/version.py
+-rw-r--r--   0        0        0     1027 1970-01-01 00:00:00.000000 nua_lib-0.5.9/PKG-INFO
```

### Comparing `nua_lib-0.5.13/pyproject.toml` & `nua_lib-0.5.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nua-lib"
-version = "0.5.13"
+version = "0.5.9"
 description = "Nua common library"
 authors = ["Stefane Fermigier <sf@abilian.com>", "Jerome Dumonteil <jd@abilian.com>"]
 license = "AGPL"
 readme = "README.md"
 packages = [
   { include = "nua", from = "src" }
 ]
```

### Comparing `nua_lib-0.5.13/src/nua/lib/actions.py` & `nua_lib-0.5.9/src/nua/lib/actions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,46 @@
 """Nua scripting: action commands."""
 import importlib.util
 import mmap
 import os
 import re
 import sys
 import tempfile
-from collections.abc import Iterable
 from contextlib import contextmanager
 from glob import glob
 from hashlib import sha256
 from importlib import resources as rso
 from pathlib import Path
 from urllib.parse import urlparse
 from urllib.request import urlopen
 
 from jinja2 import Template
 
 from .backports import chdir
 from .panic import Abort, info, show, warning
 from .shell import chown_r, sh
-from .tool.state import packages_updated, set_packages_updated, verbosity
+from .tool.state import verbosity
 from .unarchiver import unarchive
 
 LONG_TIMEOUT = 1800
 SHORT_TIMEOUT = 300
 
 
 #
 # Builder for Python projects
 #
-def build_python(path: str | Path = "", user: str = ""):
+def build_python(path: str | Path = ""):
     root = Path(path).expanduser().resolve()
     requirements = root / "requirements.txt"
     pyproject = root / "pyproject.toml"
     setup_py = root / "setup.py"
-    if user:
-        prefix = f"sudo -nu {user} "
-    else:
-        prefix = ""
     if requirements.is_file():
-        sh(f"{prefix}python -m pip install -r {requirements} .", cwd=root)
+        sh(f"python -m pip install -r {requirements} .", cwd=root)
     elif setup_py.is_file() or pyproject.is_file():
-        sh(f"{prefix}python -m pip install .", cwd=root)
+        sh("python -m pip install .", cwd=root)
     else:
         warning(f"No method found to build the python project in '{root}'")
 
 
 #
 # Other stuff
 #
@@ -64,40 +59,35 @@
             show("install packages")
         install_package_list(packages, keep_lists=keep_lists)
 
 
 @contextmanager
 def install_build_packages(
     packages: list | str,
+    update: bool = True,
     keep_lists: bool = False,
-    installed: Iterable[str] | None = None,
 ):
     success = True
-    if installed:
-        already = set(installed)
-    else:
-        already = set()
     if isinstance(packages, str):
         packages = packages.strip().split()
-    needed = [package for package in packages if package not in already]
-    if needed:
+    if packages:
         with verbosity(2):
             show("Install temporary build packages")
-        _install_packages(needed)
+        _install_packages(packages, update)
     try:
         yield
     except SystemExit:
         success = False
         raise
     finally:
         if success:
-            if needed:
+            if packages:
                 with verbosity(2):
                     show("Remove temporary build packages")
-                _purge_packages(needed)
+                _purge_packages(packages)
             apt_final_clean()
             if not keep_lists:
                 apt_remove_lists()
 
 
 def install_python(version: str = "3.10", venv: str = "", keep_lists: bool = False):
     PY_UBUNTU = {"2.7", "3.10"}
@@ -131,15 +121,15 @@
         packages = [
             "software-properties-common",
             py,
             f"{py}-dev",
             f"{py}-venv",
             f"{py}-distutils",
         ]
-    _install_packages(packages)
+    _install_packages(packages, True)
 
 
 def _venv_environ(venv: str) -> dict[str, str]:
     env = os.environ.copy()
     env["VIRTUAL_ENV"] = venv
     env["PATH"] = f"{venv}/bin:{env['PATH']}"
     return env
@@ -199,15 +189,14 @@
         extended.extend(glob_result)
     return extended
 
 
 def apt_remove_lists():
     environ = os.environ.copy()
     sh("rm -rf /var/lib/apt/lists/*", env=environ, timeout=SHORT_TIMEOUT)
-    set_packages_updated(False)
 
 
 def apt_update():
     environ = os.environ.copy()
     environ["DEBIAN_FRONTEND"] = "noninteractive"
     cmd = "apt-get update --fix-missing"
     sh(cmd, env=environ, timeout=LONG_TIMEOUT, show_cmd=False)
@@ -216,25 +205,21 @@
 def apt_final_clean():
     environ = os.environ.copy()
     environ["DEBIAN_FRONTEND"] = "noninteractive"
     cmd = "apt-get autoremove -y; apt-get clean"
     sh(cmd, env=environ, timeout=SHORT_TIMEOUT)
 
 
-def _install_packages(packages: list):
+def _install_packages(packages: list, update: bool):
     if packages:
         environ = os.environ.copy()
         environ["DEBIAN_FRONTEND"] = "noninteractive"
-        if not packages_updated():
-            cmd = "apt-get update --fix-missing; "
-        else:
-            cmd = ""
+        cmd = "apt-get update --fix-missing; " if update else ""
         cmd += f"apt-get install --no-install-recommends -y {' '.join(packages)}"
         sh(cmd, env=environ, timeout=LONG_TIMEOUT)
-        set_packages_updated(True)
     else:
         warning("install_package(): nothing to install")
 
 
 def _purge_packages(packages: list):
     if not packages:
         return
@@ -244,20 +229,21 @@
     for package in packages:
         cmd = f"apt-get purge -y {package} 2>/dev/null || true"
         sh(cmd, env=environ, timeout=SHORT_TIMEOUT, show_cmd=False)
 
 
 def install_package_list(
     packages: list | str,
+    update: bool = True,
     clean: bool = True,
     keep_lists: bool = False,
 ):
     if isinstance(packages, str):
         packages = packages.strip().split()
-    _install_packages(packages)
+    _install_packages(packages, update)
     if clean:
         apt_final_clean()
     if not keep_lists:
         apt_remove_lists()
 
 
 def purge_package_list(packages: list | str):
@@ -266,19 +252,20 @@
     _purge_packages(packages)
     apt_final_clean()
 
 
 @contextmanager
 def tmp_install_package_list(
     packages: list | str,
-    keep_lists: bool = True,
+    update: bool = True,
+    keep_lists: bool = False,
 ):
     if isinstance(packages, str):
         packages = packages.strip().split()
-    _install_packages(packages)
+    _install_packages(packages, update)
     try:
         yield
     finally:
         _purge_packages(packages)
         apt_final_clean()
         if not keep_lists:
             apt_remove_lists()
@@ -416,30 +403,22 @@
     sh(cmd)
     cmd = f"ruby-install --system --cleanup -j4 {version} -- {options}"
     sh(cmd)
     if not keep_lists:
         apt_remove_lists()
 
 
-def pip_install(
-    packages: list | str,
-    update: bool = False,
-    user: str = "",
-) -> bool:
+def pip_install(packages: list | str, update: bool = False) -> bool:
     if isinstance(packages, str):
         packages = packages.strip().split()
     if not packages:
         warning("pip_install(): nothing to install")
         return False
     option = "-U " if update else " "
-    if user:
-        prefix = f"sudo -nu {user} "
-    else:
-        prefix = ""
-    cmd = f"{prefix}python -m pip install {option}{' '.join(packages)}"
+    cmd = f"python -m pip install {option}{' '.join(packages)}"
     sh(cmd)
     return True
 
 
 def pip_install_glob(pattern: str) -> None:
     packages = [str(f) for f in Path.cwd().glob(pattern)]
     if not packages:
@@ -469,16 +448,15 @@
         [
             "python3-dev",
             "libmariadb3",
             "libmariadb-dev",
             "mariadb-client",
             "unzip",
             "build-essential",
-        ],
-        keep_lists=True,
+        ]
     )
     with tempfile.TemporaryDirectory(dir="/var/tmp") as tmpdirname:  # noqa S108
         cmd = f"python -m pip download mariadb=={version}"
         result = sh(cmd, cwd=tmpdirname, capture_output=True)
         saved_file = re.search("Saved(.*)\n", result).group(1).strip()  # type: ignore
         archive = Path(saved_file).name
         stem = Path(archive).stem
@@ -503,15 +481,15 @@
     install_package_list("libmariadb3 mariadb-client", keep_lists=keep_lists)
     with tmp_install_package_list(
         "libmariadb-dev python3-dev build-essential", keep_lists=True
     ):
         pip_install("mariadb")
 
 
-def install_psycopg2_python(keep_lists: bool = True):
+def install_psycopg2_python(keep_lists: bool = False):
     """Connector for PostgreSQL."""
     install_package_list(["libpq-dev"], keep_lists=keep_lists)
     pip_install("psycopg2-binary")
 
 
 def download_extract(
     url: str,
```

### Comparing `nua_lib-0.5.13/src/nua/lib/backports.py` & `nua_lib-0.5.9/src/nua/lib/backports.py`

 * *Files identical despite different names*

### Comparing `nua_lib-0.5.13/src/nua/lib/console.py` & `nua_lib-0.5.9/src/nua/lib/console.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,59 +17,39 @@
 
 @if_color
 def print_green(msg: str):
     print(ColorStr.green(msg))
 
 
 @if_color
-def print_gray(msg: str):
-    print(ColorStr.gray(msg))
-
-
-@if_color
 def print_blue(msg: str):
     print(ColorStr.blue(msg))
 
 
 @if_color
-def print_bold_blue(msg: str):
-    print(ColorStr.blue_bold(msg))
-
-
-@if_color
 def print_magenta(msg: str):
     print(ColorStr.magenta(msg))
 
 
 @if_color
 def print_red(msg: str):
-    print(ColorStr.red(msg))
-
-
-@if_color
-def print_bold_red(msg: str):
     print(ColorStr.red_bold(msg))
 
 
 @if_color
 def print_bold(msg: str):
     print(ColorStr.colorize(msg, bold=True))
 
 
 @if_color
 def print_bold_yellow(msg: str):
     print(ColorStr.yellow_bold(msg))
 
 
 @if_color
-def print_cyan(msg: str):
-    print(ColorStr.cyan(msg))
-
-
-@if_color
 def print_bold_yellow_white(msg: str):
     parts = msg.rsplit(" ", 1)
     if len(parts) == 2:
         print(ColorStr.yellow_bold(parts[0]), ColorStr.white_bold(parts[1]))
     else:
         print(ColorStr.yellow_bold(msg))
 
@@ -80,10 +60,10 @@
     if len(parts) == 2:
         print(ColorStr.green(parts[0]), ColorStr.cyan(parts[1]))
     else:
         print(ColorStr.green(msg))
 
 
 @if_color
-def print_magenta_no_lf(msg: str):
+def print_blue_bright_no_lf(msg: str):
     """Print specialized for lines including a LF (Docker build log)."""
-    print(ColorStr.magenta(msg), end="")
+    print(ColorStr.blue_bright(msg), end="")
```

### Comparing `nua_lib-0.5.13/src/nua/lib/exec.py` & `nua_lib-0.5.9/src/nua/lib/exec.py`

 * *Files identical despite different names*

### Comparing `nua_lib-0.5.13/src/nua/lib/gen_password.py` & `nua_lib-0.5.9/src/nua/lib/gen_password.py`

 * *Files identical despite different names*

### Comparing `nua_lib-0.5.13/src/nua/lib/shell.py` & `nua_lib-0.5.9/src/nua/lib/shell.py`

 * *Files identical despite different names*

### Comparing `nua_lib-0.5.13/src/nua/lib/tool/color_str.py` & `nua_lib-0.5.9/src/nua/lib/tool/color_str.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,15 +66,14 @@
         kwargs are bools for keys "bright", "bold", "underline" and
         "reversed".
         """
         cmd = cls._command(color=color, bgcolor=bgcolor, **kwargs)
         return f"{cmd}{txt}{cls.COL['reset']}"
 
     black = partialmethod(colorize, color="black")
-    gray = partialmethod(colorize, color="black", bright=True)
     red = partialmethod(colorize, color="red")
     green = partialmethod(colorize, color="green")
     yellow = partialmethod(colorize, color="yellow")
     blue = partialmethod(colorize, color="blue")
     magenta = partialmethod(colorize, color="magenta")
     cyan = partialmethod(colorize, color="cyan")
     white = partialmethod(colorize, color="white")
```

### Comparing `nua_lib-0.5.13/src/nua/lib/tool/state.py` & `nua_lib-0.5.9/src/nua/lib/tool/state.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,24 @@
 import os
 from contextlib import contextmanager
 from functools import cache
 from pathlib import Path
 
-STATE = {
-    "verbose": 0,
-    "colorize": True,
-    "verbose_threshold": -1,
-    "packages_updated": False,
-}
+STATE = {"verbose": 0, "colorize": True, "verbose_threshold": -1}
 
 
 def set_verbosity(value: int):
-    assert isinstance(value, int)
     STATE["verbose"] = value
 
 
 def verbosity_level() -> int:
     return STATE["verbose"]
 
 
 def set_color(flag: bool):
-    assert isinstance(flag, bool)
     STATE["colorize"] = flag
     if flag:
         os.environ.pop("NO_COLOR", None)
     else:
         os.environ["NO_COLOR"] = "1"
 
 
@@ -52,15 +45,7 @@
 @cache
 def is_inside_container() -> bool:
     """Test if current execution environment is inside a container."""
     try:
         return Path("/nua/metadata/nua-config.json").is_file()
     except PermissionError:
         return False
-
-
-def set_packages_updated(flag: bool) -> None:
-    STATE["packages_updated"] = flag
-
-
-def packages_updated() -> bool:
-    return bool(STATE.get("packages_updated", False))
```

### Comparing `nua_lib-0.5.13/src/nua/lib/unarchiver.py` & `nua_lib-0.5.9/src/nua/lib/unarchiver.py`

 * *Files identical despite different names*

### Comparing `nua_lib-0.5.13/PKG-INFO` & `nua_lib-0.5.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nua-lib
-Version: 0.5.13
+Version: 0.5.9
 Summary: Nua common library
 License: AGPL
 Author: Stefane Fermigier
 Author-email: sf@abilian.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -12,21 +12,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: setuptools
 Description-Content-Type: text/markdown
 
 # Nua Lib
 
-[Nua](https://nua.rocks/) is an open source, self-hosted cloud platform project (a PaaS - platform as a service)
+This subproject contains code that is shared between the various Nua subprojects.
 
-This subproject contains code that is shared between the various [Nua](https://nua.rocks/) subprojects.
-
-It is not intended to be useful outside of Nua, and is not intended to be used as a standalone library.
-
-Since the `nua-lib` code beeing used by `nua-agent`, it should have as little dependencies as possible
+The `nua-lib` code beeing used by `nua-agent`, It should have as little dependencies as possible
 
 ## Content
 
 `nua-lib` provides:
 
 - `shell`: shell shortcuts (mostly wrappers above subprocess and shutil)
 - `exec`: shortcuts to execute sub commands like exec_as_root(), exec_as_root()
```


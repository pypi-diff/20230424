# Comparing `tmp/collect_unexported-0.1.0.tar.gz` & `tmp/collect_unexported-0.1.1.tar.gz`

## Comparing `collect_unexported-0.1.0.tar` & `collect_unexported-0.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/.editorconfig
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/collect-unexported.toml
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/mkdocs.yml
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/tox.ini
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/.reuse/dep5
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/LICENSES/BSD-2-Clause.txt
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/config/ruff-all/pyproject.toml
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/config/ruff-base/pyproject.toml
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/config/ruff-most/pyproject.toml
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/docs/changes.md
--rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/docs/index.md
--rw-r--r--   0        0        0     5145 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/docs/reference/cmdline.md
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/docs/reference/python-api.md
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/nix/python-pytest.nix
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/nix/reformat.sh
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/requirements/install.txt
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/requirements/test.txt
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/src/collect_unexported/__init__.py
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/src/collect_unexported/__main__.py
--rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/src/collect_unexported/collect-unexported.1
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/src/collect_unexported/defs.py
--rw-r--r--   0        0        0     6477 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/src/collect_unexported/examine.py
--rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/src/collect_unexported/gitrepo.py
--rw-r--r--   0        0        0     5698 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/src/collect_unexported/parse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/src/collect_unexported/py.typed
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/test_data/frobinator/debian/changelog
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/test_data/frobinator/debian/upstream/metadata
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/test_data/unexp/.gitattributes
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/test_data/unexp/defs.txt
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/test_data/unexp/tests/file.txt
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/test_data/unexp/tests/subdir/more.txt
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/unit_tests/__init__.py
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/unit_tests/test_examine.py
--rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/unit_tests/test_functional.py
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/unit_tests/test_gitrepo.py
--rw-r--r--   0        0        0     5179 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/unit_tests/test_parse.py
--rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/unit_tests/util.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/.gitignore
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/README.md
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 collect_unexported-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/.editorconfig
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/collect-unexported.toml
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/mkdocs.yml
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/tox.ini
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/.reuse/dep5
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/LICENSES/BSD-2-Clause.txt
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/config/ruff-all/pyproject.toml
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/config/ruff-base/pyproject.toml
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/config/ruff-most/pyproject.toml
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/docs/changes.md
+-rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/docs/index.md
+-rw-r--r--   0        0        0     5145 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/docs/reference/cmdline.md
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/docs/reference/python-api.md
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/nix/python-pytest.nix
+-rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/nix/reformat.sh
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/requirements/install.txt
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/requirements/test.txt
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/src/collect_unexported/__init__.py
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/src/collect_unexported/__main__.py
+-rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/src/collect_unexported/collect-unexported.1
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/src/collect_unexported/defs.py
+-rw-r--r--   0        0        0     6477 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/src/collect_unexported/examine.py
+-rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/src/collect_unexported/gitrepo.py
+-rw-r--r--   0        0        0     5698 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/src/collect_unexported/parse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/src/collect_unexported/py.typed
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/test_data/frobinator/debian/changelog
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/test_data/frobinator/debian/upstream/metadata
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/test_data/unexp/.gitattributes
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/test_data/unexp/defs.txt
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/test_data/unexp/tests/file.txt
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/test_data/unexp/tests/subdir/more.txt
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/unit_tests/__init__.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/unit_tests/test_examine.py
+-rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/unit_tests/test_functional.py
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/unit_tests/test_gitrepo.py
+-rw-r--r--   0        0        0     5179 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/unit_tests/test_parse.py
+-rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/unit_tests/util.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/.gitignore
+-rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/README.md
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4566 2020-02-02 00:00:00.000000 collect_unexported-0.1.1/PKG-INFO
```

### Comparing `collect_unexported-0.1.0/.editorconfig` & `collect_unexported-0.1.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `collect_unexported-0.1.0/mkdocs.yml` & `collect_unexported-0.1.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `collect_unexported-0.1.0/tox.ini` & `collect_unexported-0.1.1/tox.ini`

 * *Files identical despite different names*

### Comparing `collect_unexported-0.1.0/LICENSES/BSD-2-Clause.txt` & `collect_unexported-0.1.1/LICENSES/BSD-2-Clause.txt`

 * *Files identical despite different names*

### Comparing `collect_unexported-0.1.0/config/ruff-base/pyproject.toml` & `collect_unexported-0.1.1/config/ruff-base/pyproject.toml`

 * *Files identical despite different names*

### Comparing `collect_unexported-0.1.0/config/ruff-most/pyproject.toml` & `collect_unexported-0.1.1/config/ruff-most/pyproject.toml`

 * *Files identical despite different names*

### Comparing `collect_unexported-0.1.0/docs/index.md` & `collect_unexported-0.1.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `collect_unexported-0.1.0/docs/reference/cmdline.md` & `collect_unexported-0.1.1/docs/reference/cmdline.md`

 * *Files identical despite different names*

### Comparing `collect_unexported-0.1.0/docs/reference/python-api.md` & `collect_unexported-0.1.1/docs/reference/python-api.md`

 * *Files identical despite different names*

### Comparing `collect_unexported-0.1.0/nix/python-pytest.nix` & `collect_unexported-0.1.1/nix/python-pytest.nix`

 * *Files identical despite different names*

### Comparing `collect_unexported-0.1.0/src/collect_unexported/__main__.py` & `collect_unexported-0.1.1/src/collect_unexported/__main__.py`

 * *Files identical despite different names*

### Comparing `collect_unexported-0.1.0/src/collect_unexported/collect-unexported.1` & `collect_unexported-0.1.1/src/collect_unexported/collect-unexported.1`

 * *Files identical despite different names*

### Comparing `collect_unexported-0.1.0/src/collect_unexported/defs.py` & `collect_unexported-0.1.1/src/collect_unexported/defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import cfg_diag
 
 
 if typing.TYPE_CHECKING:
     import pathlib
 
 
-VERSION = "0.1.0"
+VERSION = "0.1.1"
 """The version of the collect-unexported tool."""
 
 
 @dataclasses.dataclass
 class CollectError(Exception):
     """Base class for errors that occur during the collect-unexported operation."""
```

### Comparing `collect_unexported-0.1.0/src/collect_unexported/examine.py` & `collect_unexported-0.1.1/src/collect_unexported/examine.py`

 * *Files identical despite different names*

### Comparing `collect_unexported-0.1.0/src/collect_unexported/gitrepo.py` & `collect_unexported-0.1.1/src/collect_unexported/gitrepo.py`

 * *Files identical despite different names*

### Comparing `collect_unexported-0.1.0/src/collect_unexported/parse.py` & `collect_unexported-0.1.1/src/collect_unexported/parse.py`

 * *Files identical despite different names*

### Comparing `collect_unexported-0.1.0/unit_tests/test_examine.py` & `collect_unexported-0.1.1/unit_tests/test_examine.py`

 * *Files identical despite different names*

### Comparing `collect_unexported-0.1.0/unit_tests/test_functional.py` & `collect_unexported-0.1.1/unit_tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `collect_unexported-0.1.0/unit_tests/test_gitrepo.py` & `collect_unexported-0.1.1/unit_tests/test_gitrepo.py`

 * *Files identical despite different names*

### Comparing `collect_unexported-0.1.0/unit_tests/test_parse.py` & `collect_unexported-0.1.1/unit_tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `collect_unexported-0.1.0/unit_tests/util.py` & `collect_unexported-0.1.1/unit_tests/util.py`

 * *Files identical despite different names*

### Comparing `collect_unexported-0.1.0/pyproject.toml` & `collect_unexported-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -35,14 +35,19 @@
   "Topic :: Utilities",
   "Typing :: Typed",
 ]
 
 [project.scripts]
 collect-unexported = "collect_unexported.__main__:main"
 
+[project.urls]
+Homepage = "https://devel.ringlet.net/misc/collect-unexported/"
+Changelog = "https://devel.ringlet.net/misc/collect-unexported/changes/"
+Repository = "https://gitlab.com/ppentchev/collect-unexported"
+
 [tool.hatch.build.targets.wheel]
 packages = ["src/collect_unexported"]
 
 [tool.hatch.metadata.hooks.requirements_txt]
 files = ["requirements/install.txt"]
 
 [tool.hatch.version]
```


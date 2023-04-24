# Comparing `tmp/ibuilder-3.2.1.tar.gz` & `tmp/ibuilder-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibuilder-3.2.1.tar", max compression
+gzip compressed data, was "ibuilder-3.3.0.tar", max compression
```

## Comparing `ibuilder-3.2.1.tar` & `ibuilder-3.3.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0    32471 2022-05-11 12:07:56.761894 ibuilder-3.2.1/LICENSE
--rw-r--r--   0        0        0     4626 2022-09-28 16:07:22.347586 ibuilder-3.2.1/README.md
--rw-r--r--   0        0        0        0 2022-09-18 10:33:27.426657 ibuilder-3.2.1/ibuilder/__init__.py
--rw-r--r--   0        0        0       43 2022-09-18 10:33:27.429990 ibuilder-3.2.1/ibuilder/__main__.py
--rw-r--r--   0        0        0     4255 2022-09-18 10:33:27.433324 ibuilder-3.2.1/ibuilder/config/config.py
--rw-r--r--   0        0        0     2124 2022-09-18 10:33:27.433324 ibuilder-3.2.1/ibuilder/config/models.py
--rwxr-xr-x   0        0        0     5297 2022-09-18 10:33:27.436657 ibuilder-3.2.1/ibuilder/history.py
--rwxr-xr-x   0        0        0     3735 2022-09-18 10:33:27.426657 ibuilder-3.2.1/ibuilder/images.py
--rwxr-xr-x   0        0        0    13713 2022-11-30 19:05:15.165222 ibuilder-3.2.1/ibuilder/main.py
--rw-r--r--   0        0        0     1590 2022-09-18 10:33:27.429990 ibuilder-3.2.1/ibuilder/models.py
--rw-r--r--   0        0        0    15058 2022-09-28 16:11:32.572182 ibuilder-3.2.1/ibuilder/utils.py
--rw-r--r--   0        0        0     1145 2022-11-30 17:17:59.224934 ibuilder-3.2.1/pyproject.toml
--rw-r--r--   0        0        0     5724 1970-01-01 00:00:00.000000 ibuilder-3.2.1/setup.py
--rw-r--r--   0        0        0     5873 1970-01-01 00:00:00.000000 ibuilder-3.2.1/PKG-INFO
+-rw-r--r--   0        0        0    32471 2022-05-11 12:07:56.761894 ibuilder-3.3.0/LICENSE
+-rw-r--r--   0        0        0     4888 2023-01-28 12:17:31.533924 ibuilder-3.3.0/README.md
+-rw-r--r--   0        0        0        0 2022-09-18 10:33:27.426657 ibuilder-3.3.0/ibuilder/__init__.py
+-rw-r--r--   0        0        0       43 2022-09-18 10:33:27.429990 ibuilder-3.3.0/ibuilder/__main__.py
+-rw-r--r--   0        0        0     4255 2022-09-18 10:33:27.433324 ibuilder-3.3.0/ibuilder/config/config.py
+-rw-r--r--   0        0        0     2124 2022-09-18 10:33:27.433324 ibuilder-3.3.0/ibuilder/config/models.py
+-rwxr-xr-x   0        0        0     5297 2022-09-18 10:33:27.436657 ibuilder-3.3.0/ibuilder/history.py
+-rwxr-xr-x   0        0        0     3735 2022-09-18 10:33:27.426657 ibuilder-3.3.0/ibuilder/images.py
+-rwxr-xr-x   0        0        0    13713 2022-11-30 19:05:15.165222 ibuilder-3.3.0/ibuilder/main.py
+-rw-r--r--   0        0        0     1590 2022-09-18 10:33:27.429990 ibuilder-3.3.0/ibuilder/models.py
+-rw-r--r--   0        0        0    15058 2022-09-28 16:11:32.572182 ibuilder-3.3.0/ibuilder/utils.py
+-rw-r--r--   0        0        0     1123 2023-04-24 14:06:09.658551 ibuilder-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6121 1970-01-01 00:00:00.000000 ibuilder-3.3.0/PKG-INFO
```

### Comparing `ibuilder-3.2.1/LICENSE` & `ibuilder-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ibuilder-3.2.1/README.md` & `ibuilder-3.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 ibuilder is a [cli](https://en.wikipedia.org/wiki/Command-line_interface) based builder of [docker](https://hub.docker.com/) images. It provides an interface for building and pushing the image, signing images, as well as for tagging source code after build with a build version and other common image tasks.
 
 ### New
 
 - add ability to sign on repush
 - upgrade packages (arrow, docker, pydantic, requests, rich, and typer)
 
+
+### NOTICES
+
+- this app uses tomli for toml parsing, python 3.11 has tomllib included which we will move to at some point in the near future. We realize this could be a large burden on users so we have delayed this task until python 3.11 is more widely used.
+
+
 ### Features
 
 - build: build docker images
 - push: push images to any container registry
 - sign: sign images for container signing and verification
 - source control: tag and push when you build an image
 - history: retain build history for quick/easy access to past build info
```

### Comparing `ibuilder-3.2.1/ibuilder/config/config.py` & `ibuilder-3.3.0/ibuilder/config/config.py`

 * *Files identical despite different names*

### Comparing `ibuilder-3.2.1/ibuilder/config/models.py` & `ibuilder-3.3.0/ibuilder/config/models.py`

 * *Files identical despite different names*

### Comparing `ibuilder-3.2.1/ibuilder/history.py` & `ibuilder-3.3.0/ibuilder/history.py`

 * *Files identical despite different names*

### Comparing `ibuilder-3.2.1/ibuilder/images.py` & `ibuilder-3.3.0/ibuilder/images.py`

 * *Files identical despite different names*

### Comparing `ibuilder-3.2.1/ibuilder/main.py` & `ibuilder-3.3.0/ibuilder/main.py`

 * *Files identical despite different names*

### Comparing `ibuilder-3.2.1/ibuilder/models.py` & `ibuilder-3.3.0/ibuilder/models.py`

 * *Files identical despite different names*

### Comparing `ibuilder-3.2.1/ibuilder/utils.py` & `ibuilder-3.3.0/ibuilder/utils.py`

 * *Files identical despite different names*

### Comparing `ibuilder-3.2.1/pyproject.toml` & `ibuilder-3.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 [internal]
 created = 2019-06-15
 
 [tool.poetry]
 name = "ibuilder"
-version = "3.2.1"
+version = "3.3.0"
 description = "build, tag, push, and sign docker images"
-authors = ["David Rader <sa@adercon.com>"]
-maintainers = ["David Rader <sa@adercon.com>"]
+authors = ["drad <sa@adercon.com>"]
+maintainers = ["drad <sa@adercon.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://gitlab.com/drad/ibuilder"
 repository = "https://gitlab.com/drad/ibuilder"
 keywords = ["cli", "docker", "containers", "build", "ci", "cd", "image", "tag", "git", "push", "sign", "cosign"]
 
 [tool.poetry.scripts]
 ib = "ibuilder.main:app"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 arrow = "^1.2.3"
 click = "^8.1.3"
 docker = "^6.0.0"
-packaging = "^21.3"
-pydantic = "^1.10.2"
-requests = "^2.28.1"
-rich = "^12.6.1"
-tinydb = "^4.7.0"
+packaging = "^23.1"
+pydantic = "^1.10.7"
+requests = "^2.28.2"
+rich = "^13.3.4"
+tinydb = "^4.7.1"
 tomli = "^2.0.1"
 typer = "^0.7.0"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 88
-target-version = ['py36', 'py37', 'py38', 'py39', 'py310']
+target-version = ['py37', 'py38', 'py39', 'py310']
 include = '\.pyi?$'
 exclude = '''
 /(
     \.eggs
   | \.git
   | \.hg
   | \.mypy_cache
```

### Comparing `ibuilder-3.2.1/PKG-INFO` & `ibuilder-3.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,54 @@
 Metadata-Version: 2.1
 Name: ibuilder
-Version: 3.2.1
+Version: 3.3.0
 Summary: build, tag, push, and sign docker images
 Home-page: https://gitlab.com/drad/ibuilder
 License: GPL-3.0-only
 Keywords: cli,docker,containers,build,ci,cd,image,tag,git,push,sign,cosign
-Author: David Rader
+Author: drad
 Author-email: sa@adercon.com
-Maintainer: David Rader
+Maintainer: drad
 Maintainer-email: sa@adercon.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: arrow (>=1.2.3,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: docker (>=6.0.0,<7.0.0)
-Requires-Dist: packaging (>=21.3,<22.0)
-Requires-Dist: pydantic (>=1.10.2,<2.0.0)
-Requires-Dist: requests (>=2.28.1,<3.0.0)
-Requires-Dist: rich (>=12.6.1,<13.0.0)
-Requires-Dist: tinydb (>=4.7.0,<5.0.0)
+Requires-Dist: packaging (>=23.1,<24.0)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: rich (>=13.3.4,<14.0.0)
+Requires-Dist: tinydb (>=4.7.1,<5.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Project-URL: Repository, https://gitlab.com/drad/ibuilder
 Description-Content-Type: text/markdown
 
 # README
 
 ibuilder is a [cli](https://en.wikipedia.org/wiki/Command-line_interface) based builder of [docker](https://hub.docker.com/) images. It provides an interface for building and pushing the image, signing images, as well as for tagging source code after build with a build version and other common image tasks.
 
 ### New
 
 - add ability to sign on repush
 - upgrade packages (arrow, docker, pydantic, requests, rich, and typer)
 
+
+### NOTICES
+
+- this app uses tomli for toml parsing, python 3.11 has tomllib included which we will move to at some point in the near future. We realize this could be a large burden on users so we have delayed this task until python 3.11 is more widely used.
+
+
 ### Features
 
 - build: build docker images
 - push: push images to any container registry
 - sign: sign images for container signing and verification
 - source control: tag and push when you build an image
 - history: retain build history for quick/easy access to past build info
```


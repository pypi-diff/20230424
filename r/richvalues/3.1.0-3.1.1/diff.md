# Comparing `tmp/richvalues-3.1.0.tar.gz` & `tmp/richvalues-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "richvalues-3.1.0.tar", last modified: Mon Apr 24 07:44:48 2023, max compression
+gzip compressed data, was "richvalues-3.1.1.tar", last modified: Mon Apr 24 09:09:37 2023, max compression
```

## Comparing `richvalues-3.1.0.tar` & `richvalues-3.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 andresmegias   (501) staff       (20)        0 2023-04-24 07:44:48.932227 richvalues-3.1.0/
--rw-rw-r--   0 andresmegias   (501) staff       (20)     1532 2023-04-20 22:48:48.000000 richvalues-3.1.0/LICENSE
--rw-r--r--   0 andresmegias   (501) staff       (20)     1319 2023-04-24 07:44:48.931796 richvalues-3.1.0/PKG-INFO
--rw-rw-r--   0 andresmegias   (501) staff       (20)      848 2023-04-24 07:29:24.000000 richvalues-3.1.0/README.md
--rw-rw-r--   0 andresmegias   (501) staff       (20)      655 2023-04-24 07:41:47.000000 richvalues-3.1.0/pyproject.toml
-drwxr-xr-x   0 andresmegias   (501) staff       (20)        0 2023-04-24 07:44:48.929056 richvalues-3.1.0/richvalues/
--rw-rw-r--   0 andresmegias   (501) staff       (20)   155180 2023-04-24 07:25:15.000000 richvalues-3.1.0/richvalues/__init__.py
-drwxr-xr-x   0 andresmegias   (501) staff       (20)        0 2023-04-24 07:44:48.931282 richvalues-3.1.0/richvalues.egg-info/
--rw-r--r--   0 andresmegias   (501) staff       (20)     1319 2023-04-24 07:44:48.000000 richvalues-3.1.0/richvalues.egg-info/PKG-INFO
--rw-r--r--   0 andresmegias   (501) staff       (20)      233 2023-04-24 07:44:48.000000 richvalues-3.1.0/richvalues.egg-info/SOURCES.txt
--rw-r--r--   0 andresmegias   (501) staff       (20)        1 2023-04-24 07:44:48.000000 richvalues-3.1.0/richvalues.egg-info/dependency_links.txt
--rw-r--r--   0 andresmegias   (501) staff       (20)       30 2023-04-24 07:44:48.000000 richvalues-3.1.0/richvalues.egg-info/requires.txt
--rw-r--r--   0 andresmegias   (501) staff       (20)       11 2023-04-24 07:44:48.000000 richvalues-3.1.0/richvalues.egg-info/top_level.txt
--rw-r--r--   0 andresmegias   (501) staff       (20)       38 2023-04-24 07:44:48.932370 richvalues-3.1.0/setup.cfg
--rw-rw-r--   0 andresmegias   (501) staff       (20)      748 2023-04-24 07:35:45.000000 richvalues-3.1.0/setup.py
+drwxr-xr-x   0 andresmegias   (501) staff       (20)        0 2023-04-24 09:09:37.776116 richvalues-3.1.1/
+-rw-rw-r--   0 andresmegias   (501) staff       (20)     1532 2023-04-20 22:48:48.000000 richvalues-3.1.1/LICENSE
+-rw-r--r--   0 andresmegias   (501) staff       (20)     1319 2023-04-24 09:09:37.775865 richvalues-3.1.1/PKG-INFO
+-rw-rw-r--   0 andresmegias   (501) staff       (20)      848 2023-04-24 07:29:24.000000 richvalues-3.1.1/README.md
+-rw-rw-r--   0 andresmegias   (501) staff       (20)      671 2023-04-24 09:09:00.000000 richvalues-3.1.1/pyproject.toml
+drwxr-xr-x   0 andresmegias   (501) staff       (20)        0 2023-04-24 09:09:37.773193 richvalues-3.1.1/richvalues/
+-rw-rw-r--   0 andresmegias   (501) staff       (20)   155180 2023-04-24 09:08:47.000000 richvalues-3.1.1/richvalues/__init__.py
+drwxr-xr-x   0 andresmegias   (501) staff       (20)        0 2023-04-24 09:09:37.775371 richvalues-3.1.1/richvalues.egg-info/
+-rw-r--r--   0 andresmegias   (501) staff       (20)     1319 2023-04-24 09:09:37.000000 richvalues-3.1.1/richvalues.egg-info/PKG-INFO
+-rw-r--r--   0 andresmegias   (501) staff       (20)      233 2023-04-24 09:09:37.000000 richvalues-3.1.1/richvalues.egg-info/SOURCES.txt
+-rw-r--r--   0 andresmegias   (501) staff       (20)        1 2023-04-24 09:09:37.000000 richvalues-3.1.1/richvalues.egg-info/dependency_links.txt
+-rw-r--r--   0 andresmegias   (501) staff       (20)       30 2023-04-24 09:09:37.000000 richvalues-3.1.1/richvalues.egg-info/requires.txt
+-rw-r--r--   0 andresmegias   (501) staff       (20)       11 2023-04-24 09:09:37.000000 richvalues-3.1.1/richvalues.egg-info/top_level.txt
+-rw-r--r--   0 andresmegias   (501) staff       (20)       38 2023-04-24 09:09:37.776203 richvalues-3.1.1/setup.cfg
+-rw-rw-r--   0 andresmegias   (501) staff       (20)      748 2023-04-24 09:09:25.000000 richvalues-3.1.1/setup.py
```

### Comparing `richvalues-3.1.0/LICENSE` & `richvalues-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `richvalues-3.1.0/PKG-INFO` & `richvalues-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: richvalues
-Version: 3.1.0
+Version: 3.1.1
 Summary: Python library for working with uncertainties and upper/lower limits
 Home-page: https://github.com/andresmegias/richvalues/
 Author: Andrés Megías Toledano
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `richvalues-3.1.0/README.md` & `richvalues-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `richvalues-3.1.0/pyproject.toml` & `richvalues-3.1.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "richvalues"
-version = "3.1.0"
+version = "3.1.1"
 description = "Python library for working with uncertainties and upper/lower limits"
 license = {file="LICENSE"}
 authors = [{name="Andrés Megías Toledano"}]
 readme = "README.md"
 dependencies = ["numpy", "pandas", "scipy", "matplotlib"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent"]
+
+[project.urls]
 homepage = "https://github.com/andresmegias/richvalues/"
 documentation = "https://github.com/andresmegias/richvalues/blob/main/userguide.pdf"
```

### Comparing `richvalues-3.1.0/richvalues/__init__.py` & `richvalues-3.1.1/richvalues/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
 HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT,
 STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING
 IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 POSSIBILITY OF SUCH DAMAGE.
 """
 
-__version__ = '3.1.0'
+__version__ = '3.1.1'
 __author__ = 'Andrés Megías Toledano'
 
 import copy
 import math
 import inspect
 import itertools
 import numpy as np
```

### Comparing `richvalues-3.1.0/richvalues.egg-info/PKG-INFO` & `richvalues-3.1.1/richvalues.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: richvalues
-Version: 3.1.0
+Version: 3.1.1
 Summary: Python library for working with uncertainties and upper/lower limits
 Home-page: https://github.com/andresmegias/richvalues/
 Author: Andrés Megías Toledano
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `richvalues-3.1.0/setup.py` & `richvalues-3.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 setuptools.setup(
     name = 'richvalues',
-    version = '3.1.0',
+    version = '3.1.1',
     license = 'BSD-3-Clause',
     author = 'Andrés Megías Toledano',
     description = 'Python library for working with uncertainties and upper/lower limits',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     packages = setuptools.find_packages('.'),
     url = 'https://github.com/andresmegias/richvalues/',
```


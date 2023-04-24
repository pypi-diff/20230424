# Comparing `tmp/dep_graph_vh-0.0.1.tar.gz` & `tmp/dep_graph_vh-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dep_graph_vh-0.0.1.tar", last modified: Mon Apr 24 02:54:56 2023, max compression
+gzip compressed data, was "dep_graph_vh-0.1.2.tar", last modified: Mon Apr 24 11:02:03 2023, max compression
```

## Comparing `dep_graph_vh-0.0.1.tar` & `dep_graph_vh-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 02:54:56.620244 dep_graph_vh-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-04-22 19:39:56.000000 dep_graph_vh-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2856 2023-04-24 02:54:56.619240 dep_graph_vh-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1106 2023-04-24 02:11:19.000000 dep_graph_vh-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 02:54:56.611277 dep_graph_vh-0.0.1/dep_graph_vh/
--rw-rw-rw-   0        0        0      156 2023-04-24 02:12:56.000000 dep_graph_vh-0.0.1/dep_graph_vh/__init__.py
--rw-rw-rw-   0        0        0      124 2023-04-23 20:10:46.000000 dep_graph_vh-0.0.1/dep_graph_vh/__main__.py
--rw-rw-rw-   0        0        0      258 2023-04-23 19:29:45.000000 dep_graph_vh-0.0.1/dep_graph_vh/exceptions.py
--rw-rw-rw-   0        0        0     1147 2023-04-23 19:39:52.000000 dep_graph_vh-0.0.1/dep_graph_vh/reader.py
--rw-rw-rw-   0        0        0     2971 2023-04-23 20:09:13.000000 dep_graph_vh-0.0.1/dep_graph_vh/resolver.py
--rw-rw-rw-   0        0        0     1224 2023-04-23 20:13:02.000000 dep_graph_vh-0.0.1/dep_graph_vh/visualizer.py
-drwxrwxrwx   0        0        0        0 2023-04-24 02:54:56.615257 dep_graph_vh-0.0.1/dep_graph_vh.egg-info/
--rw-rw-rw-   0        0        0     2856 2023-04-24 02:54:56.000000 dep_graph_vh-0.0.1/dep_graph_vh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-04-24 02:54:56.000000 dep_graph_vh-0.0.1/dep_graph_vh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 02:54:56.000000 dep_graph_vh-0.0.1/dep_graph_vh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-24 02:54:56.000000 dep_graph_vh-0.0.1/dep_graph_vh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      713 2023-04-24 01:59:16.000000 dep_graph_vh-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-24 02:54:56.620244 dep_graph_vh-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-24 02:54:56.618243 dep_graph_vh-0.0.1/test/
--rw-rw-rw-   0        0        0      941 2023-04-23 23:13:34.000000 dep_graph_vh-0.0.1/test/test_reader.py
--rw-rw-rw-   0        0        0     1883 2023-04-23 23:15:15.000000 dep_graph_vh-0.0.1/test/test_resolver.py
--rw-rw-rw-   0        0        0     1774 2023-04-23 19:19:13.000000 dep_graph_vh-0.0.1/test/test_visualizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:02:03.452182 dep_graph_vh-0.1.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2023-04-24 11:01:29.000000 dep_graph_vh-0.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2847 2023-04-24 11:02:03.452182 dep_graph_vh-0.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2023-04-24 11:01:29.000000 dep_graph_vh-0.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:02:03.450182 dep_graph_vh-0.1.2/dep_graph_vh/
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-04-24 11:01:29.000000 dep_graph_vh-0.1.2/dep_graph_vh/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      234 2023-04-24 11:01:29.000000 dep_graph_vh-0.1.2/dep_graph_vh/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      304 2023-04-24 11:01:29.000000 dep_graph_vh-0.1.2/dep_graph_vh/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1296 2023-04-24 11:01:29.000000 dep_graph_vh-0.1.2/dep_graph_vh/reader.py
+-rw-rw-rw-   0 root         (0) root         (0)     3426 2023-04-24 11:01:29.000000 dep_graph_vh-0.1.2/dep_graph_vh/resolver.py
+-rw-rw-rw-   0 root         (0) root         (0)     1308 2023-04-24 11:01:29.000000 dep_graph_vh-0.1.2/dep_graph_vh/visualizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:02:03.451182 dep_graph_vh-0.1.2/dep_graph_vh.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2847 2023-04-24 11:02:03.000000 dep_graph_vh-0.1.2/dep_graph_vh.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      394 2023-04-24 11:02:03.000000 dep_graph_vh-0.1.2/dep_graph_vh.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 11:02:03.000000 dep_graph_vh-0.1.2/dep_graph_vh.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 11:02:03.000000 dep_graph_vh-0.1.2/dep_graph_vh.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      721 2023-04-24 11:01:29.000000 dep_graph_vh-0.1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 11:02:03.453182 dep_graph_vh-0.1.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 11:02:03.452182 dep_graph_vh-0.1.2/test/
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2023-04-24 11:01:29.000000 dep_graph_vh-0.1.2/test/test_reader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1970 2023-04-24 11:01:29.000000 dep_graph_vh-0.1.2/test/test_resolver.py
+-rw-rw-rw-   0 root         (0) root         (0)     1798 2023-04-24 11:01:29.000000 dep_graph_vh-0.1.2/test/test_visualizer.py
```

### Comparing `dep_graph_vh-0.0.1/LICENSE` & `dep_graph_vh-0.1.2/LICENSE`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Hyhyniak Viktor
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2023 Hyhyniak Viktor
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `dep_graph_vh-0.0.1/PKG-INFO` & `dep_graph_vh-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,87 +1,96 @@
-Metadata-Version: 2.1
-Name: dep_graph_vh
-Version: 0.0.1
-Summary: Simple dependency graph resolver with JSON input
-Author-email: Viktor Hyhyniak <hyhyniak.victor@gmail.com>
-License: MIT License
-        
-        Copyright (c) 2023 Hyhyniak Viktor
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-Project-URL: repository, https://gitlab.com/hyhyniak.victor/dep_graph
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Simple dependency graph resolver
-
-## Description
-
-This is a simple graph dependency resolver.
-It can parse dependencies in json files from the provided or default system-specific location
-(`/tmp/deps.json` or `C:\tmp\deps.json`).
-Parsed dependencies can be transformed into a fully resolved dedicated `DependencyGraph` object
-that later may be converted into a string representation.
-
-## Installation
-
-```
-git clone https://gitlab.com/hyhyniak.victor/dep_graph.git
-cd dep_graph
-pip install .
-```
-
-WIP approach: `pip install dep_graph_vh`
-
-## Usage
-
-#### Print graph from default location:
-
-```
-python -m dep_graph_vh
-```
-
-#### Obtain a fully resolved dependency graph object from the provided or default location:
-
-```python
-import dep_graph_vh as dg
-
-dg.get_graph(file_location)  # from specific location
-dg.get_graph()  # from default system-dependent
-```
-
-#### Print dependency graph object:
-
-```python
-import dep_graph_vh as dg
-
-graph = dg.get_graph()
-dg.print_dep_graph(graph)
-```
-
-## Unit Tests
-
-Run tests
-
-```
-$ python -m unittest discover
-```
+Metadata-Version: 2.1
+Name: dep_graph_vh
+Version: 0.1.2
+Summary: Simple dependency graph resolver with JSON input
+Author-email: Viktor Hyhyniak <hyhyniak.victor@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2023 Hyhyniak Viktor
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+Project-URL: repository, https://gitlab.com/hyhyniak.victor/dep_graph
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Simple dependency graph resolver
+
+## Description
+
+This is a simple graph dependency resolver.
+It can parse dependencies in json files from the provided or default system-specific location
+(`/tmp/deps.json` or `C:\tmp\deps.json`).
+Parsed dependencies can be transformed into a fully resolved dedicated `DependencyGraph` object
+that later may be converted into a string representation.
+
+## Installation
+
+```
+pip install dep_graph_vh
+```
+
+## Usage
+
+#### Print graph from default location:
+
+```
+python -m dep_graph_vh
+```
+
+#### Obtain a fully resolved dependency graph object from the provided or default location:
+
+```python
+import dep_graph_vh as dg
+
+dg.get_graph(file_location)  # from specific location
+dg.get_graph()  # from default system-dependent
+```
+
+#### Print dependency graph object:
+
+```python
+import dep_graph_vh as dg
+
+graph = dg.get_graph()
+dg.print_dep_graph(graph)
+```
+
+## Development
+
+```
+git clone https://gitlab.com/hyhyniak.victor/dep_graph.git
+cd dep_graph
+pip install -e .
+
+pip install -r dev_requirements.txt
+```
+
+## Tests and Quality Assurance
+
+```
+python -m unittest
+
+mypy .
+
+pylint dep_graph_vh test
+
+```
```

### Comparing `dep_graph_vh-0.0.1/README.md` & `dep_graph_vh-0.1.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,62 @@
-# Simple dependency graph resolver
-
-## Description
-
-This is a simple graph dependency resolver.
-It can parse dependencies in json files from the provided or default system-specific location
-(`/tmp/deps.json` or `C:\tmp\deps.json`).
-Parsed dependencies can be transformed into a fully resolved dedicated `DependencyGraph` object
-that later may be converted into a string representation.
-
-## Installation
-
-```
-git clone https://gitlab.com/hyhyniak.victor/dep_graph.git
-cd dep_graph
-pip install .
-```
-
-WIP approach: `pip install dep_graph_vh`
-
-## Usage
-
-#### Print graph from default location:
-
-```
-python -m dep_graph_vh
-```
-
-#### Obtain a fully resolved dependency graph object from the provided or default location:
-
-```python
-import dep_graph_vh as dg
-
-dg.get_graph(file_location)  # from specific location
-dg.get_graph()  # from default system-dependent
-```
-
-#### Print dependency graph object:
-
-```python
-import dep_graph_vh as dg
-
-graph = dg.get_graph()
-dg.print_dep_graph(graph)
-```
-
-## Unit Tests
-
-Run tests
-
-```
-$ python -m unittest discover
-```
+# Simple dependency graph resolver
+
+## Description
+
+This is a simple graph dependency resolver.
+It can parse dependencies in json files from the provided or default system-specific location
+(`/tmp/deps.json` or `C:\tmp\deps.json`).
+Parsed dependencies can be transformed into a fully resolved dedicated `DependencyGraph` object
+that later may be converted into a string representation.
+
+## Installation
+
+```
+pip install dep_graph_vh
+```
+
+## Usage
+
+#### Print graph from default location:
+
+```
+python -m dep_graph_vh
+```
+
+#### Obtain a fully resolved dependency graph object from the provided or default location:
+
+```python
+import dep_graph_vh as dg
+
+dg.get_graph(file_location)  # from specific location
+dg.get_graph()  # from default system-dependent
+```
+
+#### Print dependency graph object:
+
+```python
+import dep_graph_vh as dg
+
+graph = dg.get_graph()
+dg.print_dep_graph(graph)
+```
+
+## Development
+
+```
+git clone https://gitlab.com/hyhyniak.victor/dep_graph.git
+cd dep_graph
+pip install -e .
+
+pip install -r dev_requirements.txt
+```
+
+## Tests and Quality Assurance
+
+```
+python -m unittest
+
+mypy .
+
+pylint dep_graph_vh test
+
+```
```

### Comparing `dep_graph_vh-0.0.1/dep_graph_vh/resolver.py` & `dep_graph_vh-0.1.2/dep_graph_vh/resolver.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,80 @@
-from typing import List, Dict, Set
-
-from . import reader
-from .exceptions import CyclicDependencyException, MissingDependencyException
-
-
-class DependencyGraph:
-    """
-    A class that represents a fully resolved dependency graph.
-    It consists of a dictionary of packages and their corresponding resolved dependency graphs.
-    """""
-    resolved_dependencies: Dict[str, 'DependencyGraph']
-
-    def __init__(self):
-        self.resolved_dependencies = {}
-
-
-def resolve_dfs(packages: List[str], visited: Set[str], dep_dict: Dict[str, List[str]]) -> DependencyGraph:
-    """
-    A recursive function that resolves a dependency graph using depth-first search approach.
-    It keeps track of the visited nodes in order to spot the cyclic dependencies.
-    It verifies that all packages (including the ones with empty dependencies list) are present in the dep_dict
-
-    :param packages: list of packages to be resolved and added into the resolved_dependencies dict
-    :param visited: set of packages that the current recursion stack have already visited
-    :param dep_dict: dictionary of packages and their corresponding dependencies
-    :raises CyclicDependencyException: when a cyclic dependencies have been found
-    :raises MissingDependencyException: when a package is missing from the dep_dict
-    :return: fully resolved dependency graph
-    """
-    graph = DependencyGraph()
-    for package in packages:
-        if package in visited:
-            raise CyclicDependencyException(
-                f'Cycle in dependencies has been detected when processing "{package}" package')
-        if package not in dep_dict:
-            raise MissingDependencyException(f'Missing "{package}" package from the input json')
-        visited.add(package)
-        graph.resolved_dependencies[package] = resolve_dfs(dep_dict[package], visited, dep_dict)
-        visited.remove(package)
-    return graph
-
-
-def resolve_dependencies(dep_dict: Dict[str, List[str]]) -> DependencyGraph:
-    """
-    Fully resolve dependency graph based on the provided dictionary of packages and their corresponding dependencies.
-    Will raise exceptions in case of cyclic dependencies or missing packages
-
-    :param dep_dict: dictionary of packages and their corresponding dependencies
-    :return: fully resolved dependency graph object
-    """
-    packages = list(dep_dict.keys())
-    return resolve_dfs(packages, set(), dep_dict)
-
-
-def get_graph(path: str = reader.get_default_file_path()) -> DependencyGraph:
-    """
-    Constructs a fully resolved dependency graph object based on the provided path to the input json file.
-    If path parameter is not specified, use the system-specific default path ("/tmp/deps.json" or "C:\\tmp\\deps.json")
-
-    :param path: optional location of the input json file
-    :return: fully resolved graph object
-    """
-    deps = reader.read_dependencies(path)
-    return resolve_dependencies(deps)
+"""
+This module contains the logic for resolving parsed dependencies from reader.py
+and constructing the fully resolved dependency graph.
+Additional checks are performed to ensure that the dependency graph is valid:
+    - No cyclic dependencies
+    - No missing packages
+
+:raises CyclicDependencyException: when a cyclic dependencies have been found
+:raises MissingDependencyException: when a package is missing from the dep_dict
+"""
+from typing import List, Dict, Set
+
+from . import reader
+from .exceptions import CyclicDependencyException, MissingDependencyException
+
+
+class DependencyGraph:  # pylint: disable=too-few-public-methods
+    """
+    A class that represents a fully resolved dependency graph.
+    It consists of a dictionary of packages and their corresponding resolved dependency graphs.
+    """""
+    resolved_dependencies: Dict[str, 'DependencyGraph']
+
+    def __init__(self):
+        self.resolved_dependencies = {}
+
+
+def resolve_dfs(packages: List[str],
+                visited: Set[str],
+                dep_dict: Dict[str, List[str]]) -> DependencyGraph:
+    """
+    A recursive function that resolves a dependency graph using depth-first search approach.
+    It keeps track of the visited nodes in order to spot the cyclic dependencies.
+    It verifies that all packages (including the ones with empty dependencies list)
+    are present in the dep_dict
+
+    :param packages: list of packages to be resolved and added into the resolved_dependencies dict
+    :param visited: set of packages that the current recursion stack have already visited
+    :param dep_dict: dictionary of packages and their corresponding dependencies
+    :raises CyclicDependencyException: when a cyclic dependencies have been found
+    :raises MissingDependencyException: when a package is missing from the dep_dict
+    :return: fully resolved dependency graph
+    """
+    graph = DependencyGraph()
+    for package in packages:
+        if package in visited:
+            raise CyclicDependencyException(
+                f'Cycle in dependencies has been detected when processing "{package}" package')
+        if package not in dep_dict:
+            raise MissingDependencyException(f'Missing "{package}" package from the input json')
+        visited.add(package)
+        graph.resolved_dependencies[package] = resolve_dfs(dep_dict[package], visited, dep_dict)
+        visited.remove(package)
+    return graph
+
+
+def resolve_dependencies(dep_dict: Dict[str, List[str]]) -> DependencyGraph:
+    """
+    Fully resolve dependency graph based on the provided dictionary of packages
+    and their corresponding dependencies.
+    Will raise exceptions in case of cyclic dependencies or missing packages
+
+    :param dep_dict: dictionary of packages and their corresponding dependencies
+    :return: fully resolved dependency graph object
+    """
+    packages = list(dep_dict.keys())
+    return resolve_dfs(packages, set(), dep_dict)
+
+
+def get_graph(path: str = reader.get_default_file_path()) -> DependencyGraph:
+    """
+    Constructs a fully resolved dependency graph object based on the provided path
+    to the input json file. If path parameter is not specified,
+    use the system-specific default path ("/tmp/deps.json" or "C:\\tmp\\deps.json")
+
+    :param path: optional location of the input json file
+    :return: fully resolved graph object
+    """
+    deps = reader.read_dependencies(path)
+    return resolve_dependencies(deps)
```

### Comparing `dep_graph_vh-0.0.1/dep_graph_vh/visualizer.py` & `dep_graph_vh-0.1.2/dep_graph_vh/visualizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,44 @@
-from typing import List
-
-from .resolver import DependencyGraph
-
-PADDING = '  '
-
-
-def convert_with_padding(graph: DependencyGraph, level: int = 0) -> List[str]:
-    """
-    Convert recursively the dependency graph with the added level of padding
-
-    :param graph: the dependency graph to be converted
-    :param level: the level of the graph. Used to add the padding.
-    :return: string list representing graph with added padding
-    """
-    res = list()
-    for package, dep_graph in graph.resolved_dependencies.items():
-        res.append(f'{PADDING * level}- {package}')
-        res += convert_with_padding(dep_graph, level + 1)
-    return res
-
-
-def convert_dep_graph_to_string(graph: DependencyGraph) -> str:
-    """
-    Convert the dependency graph to string representation
-
-    :param graph: the dependency graph to be converted
-    :return: string representation of the provided graph
-    """
-    return '\n'.join(convert_with_padding(graph, 0))
-
-
-def print_dep_graph(graph: DependencyGraph) -> None:
-    """
-    Print the dependency graph to sdtout
-
-    :param graph: the dependency graph to be printed
-    :return: None
-    """
-    print(convert_dep_graph_to_string(graph))
+"""
+This module contains the functions to convert the dependency graph to string representation
+and print it to the sdtout.
+"""
+from typing import List
+
+from .resolver import DependencyGraph
+
+PADDING = '  '
+
+
+def convert_with_padding(graph: DependencyGraph, level: int = 0) -> List[str]:
+    """
+    Convert recursively the dependency graph with the added level of padding
+
+    :param graph: the dependency graph to be converted
+    :param level: the level of the graph. Used to add the padding.
+    :return: string list representing graph with added padding
+    """
+    res = []
+    for package, dep_graph in graph.resolved_dependencies.items():
+        res.append(f'{PADDING * level}- {package}')
+        res += convert_with_padding(dep_graph, level + 1)
+    return res
+
+
+def convert_dep_graph_to_string(graph: DependencyGraph) -> str:
+    """
+    Convert the dependency graph to string representation
+
+    :param graph: the dependency graph to be converted
+    :return: string representation of the provided graph
+    """
+    return '\n'.join(convert_with_padding(graph, 0))
+
+
+def print_dep_graph(graph: DependencyGraph) -> None:
+    """
+    Print the dependency graph to sdtout
+
+    :param graph: the dependency graph to be printed
+    :return: None
+    """
+    print(convert_dep_graph_to_string(graph))
```

### Comparing `dep_graph_vh-0.0.1/dep_graph_vh.egg-info/PKG-INFO` & `dep_graph_vh-0.1.2/dep_graph_vh.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,96 @@
-Metadata-Version: 2.1
-Name: dep-graph-vh
-Version: 0.0.1
-Summary: Simple dependency graph resolver with JSON input
-Author-email: Viktor Hyhyniak <hyhyniak.victor@gmail.com>
-License: MIT License
-        
-        Copyright (c) 2023 Hyhyniak Viktor
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-Project-URL: repository, https://gitlab.com/hyhyniak.victor/dep_graph
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Simple dependency graph resolver
-
-## Description
-
-This is a simple graph dependency resolver.
-It can parse dependencies in json files from the provided or default system-specific location
-(`/tmp/deps.json` or `C:\tmp\deps.json`).
-Parsed dependencies can be transformed into a fully resolved dedicated `DependencyGraph` object
-that later may be converted into a string representation.
-
-## Installation
-
-```
-git clone https://gitlab.com/hyhyniak.victor/dep_graph.git
-cd dep_graph
-pip install .
-```
-
-WIP approach: `pip install dep_graph_vh`
-
-## Usage
-
-#### Print graph from default location:
-
-```
-python -m dep_graph_vh
-```
-
-#### Obtain a fully resolved dependency graph object from the provided or default location:
-
-```python
-import dep_graph_vh as dg
-
-dg.get_graph(file_location)  # from specific location
-dg.get_graph()  # from default system-dependent
-```
-
-#### Print dependency graph object:
-
-```python
-import dep_graph_vh as dg
-
-graph = dg.get_graph()
-dg.print_dep_graph(graph)
-```
-
-## Unit Tests
-
-Run tests
-
-```
-$ python -m unittest discover
-```
+Metadata-Version: 2.1
+Name: dep-graph-vh
+Version: 0.1.2
+Summary: Simple dependency graph resolver with JSON input
+Author-email: Viktor Hyhyniak <hyhyniak.victor@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2023 Hyhyniak Viktor
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+Project-URL: repository, https://gitlab.com/hyhyniak.victor/dep_graph
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Simple dependency graph resolver
+
+## Description
+
+This is a simple graph dependency resolver.
+It can parse dependencies in json files from the provided or default system-specific location
+(`/tmp/deps.json` or `C:\tmp\deps.json`).
+Parsed dependencies can be transformed into a fully resolved dedicated `DependencyGraph` object
+that later may be converted into a string representation.
+
+## Installation
+
+```
+pip install dep_graph_vh
+```
+
+## Usage
+
+#### Print graph from default location:
+
+```
+python -m dep_graph_vh
+```
+
+#### Obtain a fully resolved dependency graph object from the provided or default location:
+
+```python
+import dep_graph_vh as dg
+
+dg.get_graph(file_location)  # from specific location
+dg.get_graph()  # from default system-dependent
+```
+
+#### Print dependency graph object:
+
+```python
+import dep_graph_vh as dg
+
+graph = dg.get_graph()
+dg.print_dep_graph(graph)
+```
+
+## Development
+
+```
+git clone https://gitlab.com/hyhyniak.victor/dep_graph.git
+cd dep_graph
+pip install -e .
+
+pip install -r dev_requirements.txt
+```
+
+## Tests and Quality Assurance
+
+```
+python -m unittest
+
+mypy .
+
+pylint dep_graph_vh test
+
+```
```

### Comparing `dep_graph_vh-0.0.1/test/test_visualizer.py` & `dep_graph_vh-0.1.2/test/test_visualizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,62 @@
-from unittest import TestCase
-
-from dep_graph_vh import visualizer
-from dep_graph_vh.resolver import DependencyGraph
-
-
-class TestVisualizer(TestCase):
-    @staticmethod
-    def build_valid_test_graph() -> DependencyGraph:
-        """
-        Build a valid graph for testing purposes.
-
-        {
-          "pkg1": {"pkg2": {}, "pkg3": {}},
-          "pkg2": {},
-          "pkg3": {}
-        }
-
-        :return: The test graph object.
-        """
-        graph = DependencyGraph()
-
-        graph1 = DependencyGraph()
-        graph1.resolved_dependencies['pkg2'] = DependencyGraph()
-        graph1.resolved_dependencies['pkg3'] = DependencyGraph()
-
-        graph.resolved_dependencies['pkg3'] = DependencyGraph()
-        graph.resolved_dependencies['pkg2'] = DependencyGraph()
-        graph.resolved_dependencies['pkg1'] = graph1
-        return graph
-
-    @staticmethod
-    def get_valid_test_graph_str_representation() -> str:
-        """
-        Provide correct string representation for graph:
-
-        {
-          "pkg1": {"pkg2": {}, "pkg3": {}},
-          "pkg2": {},
-          "pkg3": {}
-        }
-
-        :return: Correct test graph string representation.
-        """
-        return '- pkg3\n' \
-               '- pkg2\n' \
-               '- pkg1\n' \
-               '  - pkg2\n' \
-               '  - pkg3'
-
-    def test_convert_dep_graph_to_string(self):
-        """
-        Test the correct conversion of the dependency graph to string.
-        """
-        graph = TestVisualizer.build_valid_test_graph()
-
-        converted = visualizer.convert_dep_graph_to_string(graph)
-        correct_string = TestVisualizer.get_valid_test_graph_str_representation()
-        self.assertEqual(converted, correct_string)
+"""
+Test for the visualizer module.
+"""
+from unittest import TestCase
+
+from dep_graph_vh import visualizer
+from dep_graph_vh.resolver import DependencyGraph
+
+
+class TestVisualizer(TestCase):  # pylint: disable=missing-class-docstring
+    @staticmethod
+    def build_valid_test_graph() -> DependencyGraph:
+        """
+        Build a valid graph for testing purposes.
+
+        {
+          "pkg1": {"pkg2": {}, "pkg3": {}},
+          "pkg2": {},
+          "pkg3": {}
+        }
+
+        :return: The test graph object.
+        """
+        graph = DependencyGraph()
+
+        graph1 = DependencyGraph()
+        graph1.resolved_dependencies['pkg2'] = DependencyGraph()
+        graph1.resolved_dependencies['pkg3'] = DependencyGraph()
+
+        graph.resolved_dependencies['pkg3'] = DependencyGraph()
+        graph.resolved_dependencies['pkg2'] = DependencyGraph()
+        graph.resolved_dependencies['pkg1'] = graph1
+        return graph
+
+    @staticmethod
+    def get_valid_test_graph_str_representation() -> str:
+        """
+        Provide correct string representation for graph:
+
+        {
+          "pkg1": {"pkg2": {}, "pkg3": {}},
+          "pkg2": {},
+          "pkg3": {}
+        }
+
+        :return: Correct test graph string representation.
+        """
+        return '- pkg3\n' \
+               '- pkg2\n' \
+               '- pkg1\n' \
+               '  - pkg2\n' \
+               '  - pkg3'
+
+    def test_convert_dep_graph_to_string(self):
+        """
+        Test the correct conversion of the dependency graph to string.
+        """
+        graph = TestVisualizer.build_valid_test_graph()
+
+        converted = visualizer.convert_dep_graph_to_string(graph)
+        correct_string = TestVisualizer.get_valid_test_graph_str_representation()
+        self.assertEqual(converted, correct_string)
```


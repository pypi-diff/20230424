# Comparing `tmp/servir-0.0.5.tar.gz` & `tmp/servir-0.0.6.tar.gz`

## Comparing `servir-0.0.5.tar` & `servir-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 servir-0.0.5/.github/workflows/ci.yml
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 servir-0.0.5/.github/workflows/release.yml
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 servir-0.0.5/src/servir/__init__.py
--rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 servir-0.0.5/src/servir/_background_server.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 servir-0.0.5/src/servir/_protocols.py
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 servir-0.0.5/src/servir/_provide.py
--rw-r--r--   0        0        0     5936 2020-02-02 00:00:00.000000 servir-0.0.5/src/servir/_resources.py
--rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 servir-0.0.5/src/servir/_tilesets.py
--rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 servir-0.0.5/src/servir/_util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 servir-0.0.5/src/servir/py.typed
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 servir-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 servir-0.0.5/tests/test_provider.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 servir-0.0.5/tests/test_servir.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 servir-0.0.5/tests/test_tilesets.py
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 servir-0.0.5/tests/test_util.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 servir-0.0.5/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 servir-0.0.5/LICENSE
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 servir-0.0.5/README.md
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 servir-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 servir-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 servir-0.0.6/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 servir-0.0.6/.github/workflows/release.yml
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 servir-0.0.6/src/servir/__init__.py
+-rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 servir-0.0.6/src/servir/_background_server.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 servir-0.0.6/src/servir/_protocols.py
+-rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 servir-0.0.6/src/servir/_provide.py
+-rw-r--r--   0        0        0     5936 2020-02-02 00:00:00.000000 servir-0.0.6/src/servir/_resources.py
+-rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 servir-0.0.6/src/servir/_tilesets.py
+-rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 servir-0.0.6/src/servir/_util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 servir-0.0.6/src/servir/py.typed
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 servir-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 servir-0.0.6/tests/test_provider.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 servir-0.0.6/tests/test_servir.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 servir-0.0.6/tests/test_tilesets.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 servir-0.0.6/tests/test_util.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 servir-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 servir-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 servir-0.0.6/README.md
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 servir-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 servir-0.0.6/PKG-INFO
```

### Comparing `servir-0.0.5/.github/workflows/ci.yml` & `servir-0.0.6/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `servir-0.0.5/src/servir/_background_server.py` & `servir-0.0.6/src/servir/_background_server.py`

 * *Files identical despite different names*

### Comparing `servir-0.0.5/src/servir/_protocols.py` & `servir-0.0.6/src/servir/_protocols.py`

 * *Files identical despite different names*

### Comparing `servir-0.0.5/src/servir/_resources.py` & `servir-0.0.6/src/servir/_resources.py`

 * *Files identical despite different names*

### Comparing `servir-0.0.5/src/servir/_tilesets.py` & `servir-0.0.6/src/servir/_tilesets.py`

 * *Files identical despite different names*

### Comparing `servir-0.0.5/src/servir/_util.py` & `servir-0.0.6/src/servir/_util.py`

 * *Files identical despite different names*

### Comparing `servir-0.0.5/tests/test_provider.py` & `servir-0.0.6/tests/test_provider.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,82 +1,86 @@
 from __future__ import annotations
 
 import json
 import pathlib
 import typing
+import weakref
 
-import pytest
 import requests
 
 from servir._provide import Provider
 from servir._tilesets import TilesetResource
 
 
-@pytest.fixture(scope="module")
-def provider() -> typing.Iterator[Provider]:
+def test_files(tmp_path: pathlib.Path) -> None:
     provider = Provider()
-    yield provider
-    provider.stop()
 
-
-def test_files(provider: Provider, tmp_path: pathlib.Path) -> None:
     with open(tmp_path / "hello.txt", "w") as f:
         f.write("hello, world")
 
     server_resource = provider.create(tmp_path / "hello.txt")
     response = requests.get(server_resource.url)
     assert response.text == "hello, world"
     assert "text/plain" in response.headers["Content-Type"]
 
     response = requests.get(provider.url + "/foo.txt")
     assert response.status_code == 404
 
 
-def test_file_content_type_json(provider: Provider, tmp_path: pathlib.Path) -> None:
+def test_file_content_type_json(tmp_path: pathlib.Path) -> None:
+    provider = Provider()
+
     data = {"hello": "world"}
 
     with open(tmp_path / "hello.json", "w") as f:
         json.dump(data, f)
 
     server_resource = provider.create(tmp_path / "hello.json")
     response = requests.get(server_resource.url)
     assert response.json() == data
     assert "application/json" in response.headers["Content-Type"]
 
 
-def test_file_content_type_csv(provider: Provider, tmp_path: pathlib.Path) -> None:
+def test_file_content_type_csv(tmp_path: pathlib.Path) -> None:
+    provider = Provider()
+
     path = tmp_path / "data.csv"
 
     with open(path, mode="w", newline="\n") as f:
         f.write("a,b,c\n1,2,3\n4,5,6")
 
     server_resource = provider.create(path)
     response = requests.get(server_resource.url)
     assert response.text == path.read_text()
     assert "text/csv" in response.headers["Content-Type"]
 
 
-def test_content(provider: Provider) -> None:
+def test_content() -> None:
+    provider = Provider()
+
     content = "hello, world"
     str_resource = provider.create(content)
     response = requests.get(str_resource.url)
     assert response.text == content
     assert "text/plain" in response.headers["Content-Type"]
 
 
-def test_content_explicit_extension(provider: Provider) -> None:
+def test_content_explicit_extension() -> None:
+    provider = Provider()
     data = "a,b,c,\n1,2,3,\n4,5,6"
 
     content_resource = provider.create(data, extension=".csv")
     response = requests.get(content_resource.url)
     assert response.text == data
     assert "text/csv" in response.headers["Content-Type"]
 
 
-def test_directory_resource(provider: Provider, tmp_path: pathlib.Path) -> None:
+def test_directory_resource(tmp_path: pathlib.Path) -> None:
+    provider = Provider()
+
     root = tmp_path / "data_dir"
     root.mkdir()
     (root / "hello.txt").write_text("hello, world")
     (root / "nested_dir").mkdir()
     (root / "nested_dir" / "foo.txt").write_text("foo")
 
     server_resource = provider.create(root)
@@ -85,15 +89,17 @@
     response = requests.get(server_resource.url + "/hello.txt")
     assert response.text == "hello, world"
 
     response = requests.get(server_resource.url + "/nested_dir/foo.txt")
     assert response.text == "foo"
 
 
-def test_tileset_resource(provider: Provider) -> None:
+def test_tileset_resource() -> None:
+    provider = Provider()
+
     class Tileset:
         @property
         def uid(self) -> str:
             return "aaaaaaaaaa"
 
         def tiles(self, tile_ids: typing.Sequence[str]) -> list[typing.Any]:
             return [(tid, None) for tid in tile_ids]
@@ -107,7 +113,32 @@
 
     resource_url = f"{resource.server}tileset_info/?d={resource.uid}"
     info = requests.get(resource_url).json()
     assert info[resource.uid] == "tile_info"
     tile_url = resource_url.replace("tileset_info", "tiles") + ".0.0"
     tiles = requests.get(tile_url).json()
     assert f"{resource.uid}.0.0" in tiles
+
+
+def test_resource_cleanup() -> None:
+    provider = Provider()
+    assert not provider._resources
+
+    content = "hello, world"
+
+    resource1 = provider.create(content)
+    resource_ref = weakref.ref(resource1)
+    assert len(provider._resources) == 1
+
+    resource2 = provider.create(content)
+    assert resource1 == resource2
+    assert len(provider._resources) == 1
+
+    # should not trigger cleanup
+    del resource1
+    assert len(provider._resources) == 1
+    assert resource_ref() is resource2
+
+    # should trigger cleanup
+    del resource2
+    assert len(provider._resources) == 0
+    assert resource_ref() is None
```

### Comparing `servir-0.0.5/tests/test_util.py` & `servir-0.0.6/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `servir-0.0.5/LICENSE` & `servir-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `servir-0.0.5/README.md` & `servir-0.0.6/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -59,10 +59,15 @@
 
 content_resource = provider.create(data, extension=".csv")
 response = requests.get(content_resource.url)
 assert response.text == data
 assert "text/csv" in response.headers["Content-Type"]
 ```
 
+> **Note**: the `Provider` holds a _weak reference_ to each resource it creates.
+> This allows the provider to cleanup unused resources and prevent memory leaks.
+> As an end user, you must hold a **strong** reference each resource returned
+> by the provider so long as you'd like that endpoint to remain avaiable.
+
 ## license
 
 `servir` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `servir-0.0.5/pyproject.toml` & `servir-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `servir-0.0.5/PKG-INFO` & `servir-0.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servir
-Version: 0.0.5
+Version: 0.0.6
 Summary: an extensible async background server
 Project-URL: Documentation, https://github.com/unknown/servir#readme
 Project-URL: Issues, https://github.com/unknown/servir/issues
 Project-URL: Source, https://github.com/unknown/servir
 Author-email: Trevor Manz <trevor.j.manz@gmail.com>
 License: MIT
 License-File: LICENSE
@@ -84,10 +84,15 @@
 
 content_resource = provider.create(data, extension=".csv")
 response = requests.get(content_resource.url)
 assert response.text == data
 assert "text/csv" in response.headers["Content-Type"]
 ```
 
+> **Note**: the `Provider` holds a _weak reference_ to each resource it creates.
+> This allows the provider to cleanup unused resources and prevent memory leaks.
+> As an end user, you must hold a **strong** reference each resource returned
+> by the provider so long as you'd like that endpoint to remain avaiable.
+
 ## license
 
 `servir` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```


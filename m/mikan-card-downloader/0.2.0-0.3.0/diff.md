# Comparing `tmp/mikan_card_downloader-0.2.0.tar.gz` & `tmp/mikan_card_downloader-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mikan_card_downloader-0.2.0.tar", max compression
+gzip compressed data, was "mikan_card_downloader-0.3.0.tar", max compression
```

## Comparing `mikan_card_downloader-0.2.0.tar` & `mikan_card_downloader-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2021-11-29 13:57:47.295968 mikan_card_downloader-0.2.0/LICENSE
--rw-r--r--   0        0        0     1041 2023-04-21 04:15:33.143336 mikan_card_downloader-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-0.2.0/src/mikan/__init__.py
--rw-r--r--   0        0        0     3952 2023-04-20 20:32:09.133338 mikan_card_downloader-0.2.0/src/mikan/classes.py
--rw-r--r--   0        0        0     1306 2023-04-21 03:31:38.850291 mikan_card_downloader-0.2.0/src/mikan/config.py
--rw-r--r--   0        0        0     4984 2023-04-20 20:32:09.133338 mikan_card_downloader-0.2.0/src/mikan/downloader.py
--rw-r--r--   0        0        0     7007 2023-04-20 20:32:09.133338 mikan_card_downloader-0.2.0/src/mikan/html_parser.py
--rw-r--r--   0        0        0     1629 2023-04-20 20:32:09.133338 mikan_card_downloader-0.2.0/src/mikan/json_utils.py
--rwxr-xr-x   0        0        0     2095 2023-04-21 03:29:22.382978 mikan_card_downloader-0.2.0/src/mikan/main.py
--rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-0.2.0/src/mikan/py.typed
--rw-r--r--   0        0        0      911 1970-01-01 00:00:00.000000 mikan_card_downloader-0.2.0/setup.py
--rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 mikan_card_downloader-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2021-11-29 13:57:47.295968 mikan_card_downloader-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1041 2023-04-23 22:20:01.579058 mikan_card_downloader-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-0.3.0/src/mikan/__init__.py
+-rw-r--r--   0        0        0     1253 2023-04-23 14:42:49.133150 mikan_card_downloader-0.3.0/src/mikan/classes.py
+-rw-r--r--   0        0        0     1306 2023-04-21 03:31:38.850291 mikan_card_downloader-0.3.0/src/mikan/config.py
+-rw-r--r--   0        0        0     4518 2023-04-23 20:47:08.508195 mikan_card_downloader-0.3.0/src/mikan/downloader.py
+-rw-r--r--   0        0        0     5802 2023-04-23 15:20:19.047035 mikan_card_downloader-0.3.0/src/mikan/html_parser.py
+-rw-r--r--   0        0        0     1382 2023-04-23 20:48:44.204752 mikan_card_downloader-0.3.0/src/mikan/json_utils.py
+-rwxr-xr-x   0        0        0     2149 2023-04-23 20:44:25.688821 mikan_card_downloader-0.3.0/src/mikan/main.py
+-rw-r--r--   0        0        0        0 2023-04-20 20:32:09.133338 mikan_card_downloader-0.3.0/src/mikan/py.typed
+-rw-r--r--   0        0        0      911 1970-01-01 00:00:00.000000 mikan_card_downloader-0.3.0/setup.py
+-rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 mikan_card_downloader-0.3.0/PKG-INFO
```

### Comparing `mikan_card_downloader-0.2.0/LICENSE` & `mikan_card_downloader-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-0.2.0/pyproject.toml` & `mikan_card_downloader-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mikan-card-downloader"
-version = "0.2.0"
+version = "0.3.0"
 description = "Downloads cards and stills from SIFAS and SIF."
 authors = ["DemonicSavage"]
 license = "GPLv3"
 packages = [
     {include = "mikan", from = "src"}
 ]
```

### Comparing `mikan_card_downloader-0.2.0/src/mikan/config.py` & `mikan_card_downloader-0.3.0/src/mikan/config.py`

 * *Files identical despite different names*

### Comparing `mikan_card_downloader-0.2.0/src/mikan/downloader.py` & `mikan_card_downloader-0.3.0/src/mikan/downloader.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,91 +19,76 @@
 from typing import Any, Coroutine
 
 import aiohttp
 from tqdm.asyncio import tqdm
 
 import mikan.html_parser as parser
 from mikan import json_utils
-from mikan.classes import Card, Item, SIFCard
+from mikan.classes import Item, SIFCard
 
 
 class Downloader:
-    def __init__(self, path: Path, img_type: type[Item]):
-        self.path = path.expanduser()
-        self.objs: dict[int, Item] = {}
+    def __init__(self, data_path: Path, config_path: Path, img_type: type[Item]):
+        self.base_path = data_path.expanduser()
+        self.path = self.base_path / img_type.results_dir
+        self.objs: dict[str, dict[str, list[str]]] = {}
+
+        self.config_path = config_path
 
         self.img_type = img_type
+        self.objs[self.img_type.results_dir] = {}
 
         self.session = aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=None))
 
-        json_utils.load_cards(self.path, self.objs, self.img_type)
+        json_utils.load_cards(self.objs, self.config_path)
 
         self.list_parser: parser.ListParser | parser.SIFListParser = (
             parser.ListParser(self.img_type)
             if self.img_type != SIFCard
             else parser.SIFListParser()
         )
         self.item_parser = getattr(parser, f"{img_type.__name__}Parser")()
 
-        self.updateables: list[int] = []
-
     async def __aenter__(self) -> Downloader:
         self.list_parser.set_session(self.session)
         self.item_parser.set_session(self.session)
 
         return self
 
     async def __aexit__(self, ext_type: None, value: None, trace: None) -> None:
         await self.session.close()
 
-    async def request_from_server(self, dest: Path, url: str) -> None:
-        res = await self.session.get(f"https:{url}")
-
-        if res.status == 200:
-            res_data = await res.read()
-            dest.parent.mkdir(exist_ok=True, parents=True)
-
-            with open(dest, "wb") as file:
-                file.write(res_data)
-
-    async def download_file(self, path: Path, item: Item, i: int) -> None:
+    async def download_file(self, item: str) -> None:
         try:
-            await self.request_from_server(path, item.get_urls()[i])
+            res = await self.session.get(f"https:{item}")
+            if res.status == 200:
+                res_data = await res.read()
+                self.path.mkdir(exist_ok=True, parents=True)
+
+                with open(self.path / self.get_card_image_name(item), "wb") as file:
+                    file.write(res_data)
 
-            message = f"Downloaded item {item.key}"
-            if isinstance(item, Card):
-                message += f", {'idolized' if i == 1 else 'normal'}"
-            message += "."
+                message = f"Downloaded item {self.get_card_image_name(item)}."
 
         except aiohttp.ClientError as e:
-            message = f"Couldn't download item {item.key}: {e}"
+            message = f"Couldn't download item {item}: {e}"
 
         tqdm.write(message)
 
-    async def update_if_needed(self, item: Item) -> None:
-        if item.needs_update():
-            _, updated_item = await self.item_parser.get_item(item.key)
-
-            if item.get_urls()[0] != updated_item.get_urls()[0]:
-                self.updateables.append(item.key)
-
-            for i in range(len(item.get_urls())):
-                item.set_url(i, updated_item.get_urls()[i])
-
     async def add_item_to_object_list(self, item: int) -> None:
         i, obj = await self.item_parser.get_item(item)
-        self.objs[i] = obj
+        self.objs[self.img_type.results_dir][i] = obj
         print(f"Getting item {i}.")
 
     async def get_page(self, idx: int) -> list[None]:
         tasks: list[Coroutine[Any, Any, None]] = []
         page = await self.list_parser.get_page(idx)
 
         for item in page:
-            if item not in self.objs:
+            if str(item) not in self.objs[self.img_type.results_dir]:
                 tasks.append(self.add_item_to_object_list(item))
 
         res: list[None] = await asyncio.gather(*tasks, return_exceptions=False)
 
         return res
 
     async def get_cards_from_parser(self) -> None:
@@ -112,36 +97,36 @@
         for _ in range(1, num_pages):
             current_page = await self.get_page(current_num)
             if not current_page and self.img_type != SIFCard:
                 break
 
             current_num += 1
 
+    def get_card_image_name(self, url: str) -> str:
+        return url.split("/")[-1]
+
     async def get(self) -> None:
         tasks: list[Coroutine[Any, Any, None]] = []
 
-        for _, item in self.objs.items():
-            paths = item.get_paths(self.path)
+        for _, item in self.objs[self.img_type.results_dir].items():
             tasks.extend(
                 [
-                    self.download_file(path, item, i)
-                    for i, path in enumerate(paths)
-                    if not path.exists() or item.key in self.updateables
+                    self.download_file(card)
+                    for card in item
+                    if not (self.path / self.get_card_image_name(card)).exists()
                 ]
             )
 
         await tqdm.gather(*tasks, disable=len(tasks) == 0)
 
     async def update(self) -> None:
         print("Searching for new or missing items...")
         await self.get_cards_from_parser()
 
-        print("Checking if items can be updated to better resolution...")
-        for _, item in self.objs.items():
-            await self.update_if_needed(item)
-
         self.update_json_file()
         print("Updated items database.")
 
     def update_json_file(self) -> None:
-        self.objs = dict(sorted(self.objs.items(), reverse=True))
-        json_utils.dump_to_file(json_utils.to_json(self.objs), self.path, self.img_type)
+        self.objs[self.img_type.results_dir] = dict(
+            sorted(self.objs[self.img_type.results_dir].items(), reverse=True)
+        )
+        json_utils.dump_to_file(self.objs, self.config_path)
```

### Comparing `mikan_card_downloader-0.2.0/src/mikan/main.py` & `mikan_card_downloader-0.3.0/src/mikan/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -49,19 +49,21 @@
             )
 
     data_dir = config.get_data_dir(path)
     if data_dir.exists() and not data_dir.is_dir():  # pragma: no cover
         raise InvalidPathException(
             "The specified directory is not valid (is a regular file)."
         )
-    await card_searcher(data_dir, img_type)
+    await card_searcher(data_dir, path, img_type)
 
 
-async def card_searcher(path: Path, img_type: type[Item]) -> None:
-    async with Downloader(path, img_type) as downloader:
+async def card_searcher(
+    data_path: Path, config_path: Path, img_type: type[Item]
+) -> None:
+    async with Downloader(data_path, config_path, img_type) as downloader:
         await downloader.update()
         await downloader.get()
 
 
 def main() -> None:  # pragma: no cover
     if sys.platform.startswith("win"):
         asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
```

### Comparing `mikan_card_downloader-0.2.0/setup.py` & `mikan_card_downloader-0.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'tqdm>=4.64.0,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['mikan = mikan.main:main']}
 
 setup_kwargs = {
     'name': 'mikan-card-downloader',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': 'Downloads cards and stills from SIFAS and SIF.',
     'long_description': 'None',
     'author': 'DemonicSavage',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mikan_card_downloader-0.2.0/PKG-INFO` & `mikan_card_downloader-0.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mikan-card-downloader
-Version: 0.2.0
+Version: 0.3.0
 Summary: Downloads cards and stills from SIFAS and SIF.
 License: GPLv3
 Author: DemonicSavage
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```


# Comparing `tmp/pokelance-0.1.3.tar.gz` & `tmp/pokelance-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokelance-0.1.3.tar", max compression
+gzip compressed data, was "pokelance-0.1.4.tar", max compression
```

## Comparing `pokelance-0.1.3.tar` & `pokelance-0.1.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1068 2023-04-24 08:36:52.557566 pokelance-0.1.3/LICENSE
--rw-r--r--   0        0        0     3731 2023-04-24 08:36:52.557566 pokelance-0.1.3/README.md
--rw-r--r--   0        0        0      106 2023-04-24 08:36:52.557566 pokelance-0.1.3/pokelance/__init__.py
--rw-r--r--   0        0        0      431 2023-04-24 08:36:52.557566 pokelance-0.1.3/pokelance/cache/__init__.py
--rw-r--r--   0        0        0    14534 2023-04-24 08:36:52.557566 pokelance-0.1.3/pokelance/cache/cache.py
--rw-r--r--   0        0        0    13942 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/cache/cache_manager.py
--rw-r--r--   0        0        0     9015 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/client.py
--rw-r--r--   0        0        0     5886 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/constants.py
--rw-r--r--   0        0        0     3868 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/exceptions.py
--rw-r--r--   0        0        0      530 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/ext/__init__.py
--rw-r--r--   0        0        0     3163 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/ext/_base.py
--rw-r--r--   0        0        0     7196 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/ext/berry.py
--rw-r--r--   0        0        0     7189 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/ext/contest.py
--rw-r--r--   0        0        0     7747 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/ext/encounter.py
--rw-r--r--   0        0        0     4990 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/ext/evolution.py
--rw-r--r--   0        0        0     8348 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/ext/game.py
--rw-r--r--   0        0        0    11273 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/ext/item.py
--rw-r--r--   0        0        0     9049 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/ext/location.py
--rw-r--r--   0        0        0     2625 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/ext/machine.py
--rw-r--r--   0        0        0    15682 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/ext/move.py
--rw-r--r--   0        0        0    33460 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/ext/pokemon.py
--rw-r--r--   0        0        0     4724 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/http/__init__.py
--rw-r--r--   0        0        0    20467 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/http/endpoints.py
--rw-r--r--   0        0        0     9677 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/languages.py
--rw-r--r--   0        0        0     3588 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/logger.py
--rw-r--r--   0        0        0     1919 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/models/__init__.py
--rw-r--r--   0        0        0      529 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/models/_base.py
--rw-r--r--   0        0        0     1873 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/models/abstract/__init__.py
--rw-r--r--   0        0        0     5528 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/models/abstract/berry.py
--rw-r--r--   0        0        0     4083 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/models/abstract/contest.py
--rw-r--r--   0        0        0     3507 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/models/abstract/encounter.py
--rw-r--r--   0        0        0     2410 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/models/abstract/evolution.py
--rw-r--r--   0        0        0     7628 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/models/abstract/game.py
--rw-r--r--   0        0        0     8794 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/models/abstract/item.py
--rw-r--r--   0        0        0     6706 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/models/abstract/location.py
--rw-r--r--   0        0        0     1222 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/models/abstract/machine.py
--rw-r--r--   0        0        0    12765 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/models/abstract/move.py
--rw-r--r--   0        0        0    35329 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/models/abstract/pokemon.py
--rw-r--r--   0        0        0     1351 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/models/abstract/showdown.py
--rw-r--r--   0        0        0     2506 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/models/abstract/utils/__init__.py
--rw-r--r--   0        0        0     1494 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/models/abstract/utils/berries.py
--rw-r--r--   0        0        0      943 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/models/abstract/utils/contests.py
--rw-r--r--   0        0        0     6255 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/models/abstract/utils/evolutions.py
--rw-r--r--   0        0        0      890 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/models/abstract/utils/games.py
--rw-r--r--   0        0        0     2284 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/models/abstract/utils/items.py
--rw-r--r--   0        0        0     3546 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/models/abstract/utils/locations.py
--rw-r--r--   0        0        0     7112 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/models/abstract/utils/moves.py
--rw-r--r--   0        0        0    42172 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/models/abstract/utils/pokemons.py
--rw-r--r--   0        0        0      650 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/models/common/__init__.py
--rw-r--r--   0        0        0    10868 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/models/common/models.py
--rw-r--r--   0        0        0     1063 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/models/common/resources.py
--rw-r--r--   0        0        0        0 2023-04-24 08:36:52.561566 pokelance-0.1.3/pokelance/py.typed
--rw-r--r--   0        0        0     1114 2023-04-24 08:36:52.561566 pokelance-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4477 1970-01-01 00:00:00.000000 pokelance-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-24 10:04:43.080728 pokelance-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3817 2023-04-24 10:04:43.080728 pokelance-0.1.4/README.md
+-rw-r--r--   0        0        0      106 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/__init__.py
+-rw-r--r--   0        0        0      431 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/cache/__init__.py
+-rw-r--r--   0        0        0    14722 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/cache/cache.py
+-rw-r--r--   0        0        0    13942 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/cache/cache_manager.py
+-rw-r--r--   0        0        0     9646 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/client.py
+-rw-r--r--   0        0        0     7050 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/constants.py
+-rw-r--r--   0        0        0     3868 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/exceptions.py
+-rw-r--r--   0        0        0      530 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/ext/__init__.py
+-rw-r--r--   0        0        0     3163 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/ext/_base.py
+-rw-r--r--   0        0        0     7196 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/ext/berry.py
+-rw-r--r--   0        0        0     7189 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/ext/contest.py
+-rw-r--r--   0        0        0     7747 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/ext/encounter.py
+-rw-r--r--   0        0        0     4990 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/ext/evolution.py
+-rw-r--r--   0        0        0     8348 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/ext/game.py
+-rw-r--r--   0        0        0    11273 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/ext/item.py
+-rw-r--r--   0        0        0     9049 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/ext/location.py
+-rw-r--r--   0        0        0     2625 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/ext/machine.py
+-rw-r--r--   0        0        0    15682 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/ext/move.py
+-rw-r--r--   0        0        0    33460 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/ext/pokemon.py
+-rw-r--r--   0        0        0     4724 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/http/__init__.py
+-rw-r--r--   0        0        0    20467 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/http/endpoints.py
+-rw-r--r--   0        0        0     9677 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/languages.py
+-rw-r--r--   0        0        0     3588 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/logger.py
+-rw-r--r--   0        0        0     1919 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/models/__init__.py
+-rw-r--r--   0        0        0      550 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/models/_base.py
+-rw-r--r--   0        0        0     1873 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/models/abstract/__init__.py
+-rw-r--r--   0        0        0     5528 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/models/abstract/berry.py
+-rw-r--r--   0        0        0     4083 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/models/abstract/contest.py
+-rw-r--r--   0        0        0     3507 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/models/abstract/encounter.py
+-rw-r--r--   0        0        0     2410 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/models/abstract/evolution.py
+-rw-r--r--   0        0        0     7628 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/models/abstract/game.py
+-rw-r--r--   0        0        0     8794 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/models/abstract/item.py
+-rw-r--r--   0        0        0     6706 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/models/abstract/location.py
+-rw-r--r--   0        0        0     1222 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/models/abstract/machine.py
+-rw-r--r--   0        0        0    12765 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/models/abstract/move.py
+-rw-r--r--   0        0        0    35329 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/models/abstract/pokemon.py
+-rw-r--r--   0        0        0     1137 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/models/abstract/showdown.py
+-rw-r--r--   0        0        0     2506 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/models/abstract/utils/__init__.py
+-rw-r--r--   0        0        0     1494 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/models/abstract/utils/berries.py
+-rw-r--r--   0        0        0      943 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/models/abstract/utils/contests.py
+-rw-r--r--   0        0        0     6255 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/models/abstract/utils/evolutions.py
+-rw-r--r--   0        0        0      890 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/models/abstract/utils/games.py
+-rw-r--r--   0        0        0     2284 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/models/abstract/utils/items.py
+-rw-r--r--   0        0        0     3546 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/models/abstract/utils/locations.py
+-rw-r--r--   0        0        0     7112 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/models/abstract/utils/moves.py
+-rw-r--r--   0        0        0    42176 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/models/abstract/utils/pokemons.py
+-rw-r--r--   0        0        0      650 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/models/common/__init__.py
+-rw-r--r--   0        0        0    10868 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/models/common/models.py
+-rw-r--r--   0        0        0     1063 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/models/common/resources.py
+-rw-r--r--   0        0        0        0 2023-04-24 10:04:43.084728 pokelance-0.1.4/pokelance/py.typed
+-rw-r--r--   0        0        0     1114 2023-04-24 10:04:43.084728 pokelance-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4563 1970-01-01 00:00:00.000000 pokelance-0.1.4/PKG-INFO
```

### Comparing `pokelance-0.1.3/LICENSE` & `pokelance-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/README.md` & `pokelance-0.1.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -83,24 +83,28 @@
         print(client.berry.get_berry_firmness("very-soft"))
         # The client will be closed automatically when the async context manager exits
     return None
 
 asyncio.run(main())
 ```
 
+# Examples
+
+[Examples](https://fallendeity.github.io/PokeLance/guide/basic_usage/)
+
+Following examples are available open an issue if you want more examples or more details on certain examples.
+- Basic Usage
+- Advanced cache usage
+- Discord bot example
+- FastAPI example
+
+
 ## Important Links
 
 
 - [PokeAPI](https://pokeapi.co/)
 - [PokeAPI Documentation](https://pokeapi.co/docs/v2)
 - [PokeLance Documentation](https://FallenDeity.github.io/PokeLance/)
 - [PokeLance ReadTheDocs](https://pokelance.readthedocs.io/en/latest/)
 - [PokeLance GitHub](https://github.com/FallenDeity/PokeLance)
 - [PokeLance PyPI](https://pypi.org/project/PokeLance/)
 - [PokeLance Discord](https://discord.gg/yeyEvT5V2J)
-
----
-
-!!! note "Note"
-    This is a work in progress. If you find any bugs or have any suggestions, please open an issue [here](https://github.com/FallenDeity/PokeLance/issues/new).
-
----
```

### Comparing `pokelance-0.1.3/pokelance/cache/cache.py` & `pokelance-0.1.4/pokelance/cache/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import importlib
 import json
 import pathlib
 import typing as t
 from collections.abc import MutableMapping
 
 import aiofiles
@@ -196,28 +197,33 @@
         data: typing.List[typing.Dict[str, str]]
             The data to load.
         """
         for document in data:
             self._endpoints[document["name"]] = Endpoint(url=document["url"], id=int(document["url"].split("/")[-2]))
         self._endpoints_cached = True
 
-    async def save(self, path: str = "") -> None:
+    async def wait_until_ready(self) -> None:
+        """Wait until the cache is ready."""
+        while not self._endpoints_cached:
+            await asyncio.sleep(0.5)
+
+    async def save(self, path: str = ".") -> None:
         """Save the cache to a file.
 
         Parameters
         ----------
         path: str
             The path to save the cache to.
         """
         pathlib.Path(path).mkdir(parents=True, exist_ok=True)
         dummy: t.Dict[str, t.Dict[str, t.Any]] = {k.endpoint: attrs.asdict(v) for k, v in self.items()}
         async with aiofiles.open(pathlib.Path(f"{path}/{self.__class__.__name__}.json"), "w") as f:
             await f.write(json.dumps(dummy, indent=4, ensure_ascii=False))
 
-    async def load(self, path: str = "") -> None:
+    async def load(self, path: str = ".") -> None:
         """Load the cache from a file.
 
         Parameters
         ----------
         path: str
             The path to load the cache from.
         """
```

### Comparing `pokelance-0.1.3/pokelance/cache/cache_manager.py` & `pokelance-0.1.4/pokelance/cache/cache_manager.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/client.py` & `pokelance-0.1.4/pokelance/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,18 +219,41 @@
         bulbasaur
         """
         if isinstance(ext, str) and (ext := str(ext).title()) not in ExtensionEnum.__members__:
             raise ValueError(f"Invalid extension: {ext}")
         categories = ExtensionEnum.get_categories(ext) if isinstance(ext, str) else ext.categories  # type: ignore
         if (category := category.lower()) not in categories:
             raise ValueError(f"Invalid category: {category}")
-        ext_ = getattr(self, ext) if isinstance(ext, str) else getattr(self, ext.name.lower())
+        ext_ = getattr(self, ext.lower()) if isinstance(ext, str) else getattr(self, ext.name.lower())
         get_, fetch_ = getattr(ext_, f"get_{category}"), getattr(ext_, f"fetch_{category}")
         return t.cast(BaseType, get_(id_) or await fetch_(id_))
 
+    async def from_url(self, url: str) -> t.Optional[BaseType]:
+        """
+        Constructs a request from urls present in the data.
+
+        Parameters
+        ----------
+        url : str
+            The URL to construct the request from.
+
+        Returns
+        -------
+        typing.Optional[BaseType]
+            The data.
+
+        Raises
+        ------
+        ValueError
+            If the url is invalid.
+        """
+        if params := ExtensionEnum.validate_url(url):
+            return await self.getch_data(params.extension, params.category, params.value)
+        raise ValueError(f"Invalid URL: {url}")
+
     async def get_image_async(self, url: str) -> bytes:
         """
         Gets an image from the url asynchronously.
 
         Parameters
         ----------
         url : str
```

### Comparing `pokelance-0.1.3/pokelance/constants.py` & `pokelance-0.1.4/pokelance/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import enum
+import re
 import typing as t
 
 import attrs
 
 __all__: t.Final[t.Tuple[str, ...]] = (
     "BaseEnum",
     "Extension",
@@ -16,34 +17,58 @@
     "ItemExtension",
     "LocationExtension",
     "MachineExtension",
     "MoveExtension",
     "PokemonExtension",
     "ExtensionEnum",
     "ExtensionsL",
+    "ShowdownEnum",
 )
 
 
 ExtensionsL = t.Literal[
     "berry", "contest", "encounter", "evolution", "game", "item", "location", "machine", "move", "pokemon"
 ]
+PATH: str = "https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/other/showdown/"
+EXTENSION_PATTERN: t.Pattern[str] = re.compile(r"https://pokeapi.co/api/v2/(\w+)/(\d+)/")
+
+
+@attrs.define
+class RequestObject:
+    extension: str
+    category: str
+    value: str
 
 
 class BaseEnum(enum.Enum):
     """
     Base enum class for all enums in the library.
     """
 
     def __get__(self, instance: t.Any, owner: t.Any) -> t.Any:
         """
         Get the value of the enum.
         """
         return self.value
 
 
+class ShowdownEnum(BaseEnum):
+    """
+    Represents a showdown enum.
+    """
+
+    FRONT_DEFAULT = PATH + "{}.gif"
+    FRONT_SHINY = PATH + "shiny/{}.gif"
+    BACK_DEFAULT = PATH + "back/{}.gif"
+    BACK_SHINY = PATH + "/back/shiny/{}.gif"
+
+    def __str__(self) -> str:
+        return self.value
+
+
 @attrs.define(slots=True, frozen=True)
 class Extension:
     """
     Represents an extension.
     """
 
     name: str
@@ -253,9 +278,22 @@
     Item = ItemExtension(name="item")
     Location = LocationExtension(name="location")
     Machine = MachineExtension(name="machine")
     Move = MoveExtension(name="move")
     Pokemon = PokemonExtension(name="pokemon")
 
     @classmethod
+    def validate_url(cls, url: str) -> t.Optional[RequestObject]:
+        """
+        Validate the url.
+        """
+        if not url.startswith("https://pokeapi.co/api/v2/") or not (groups := re.match(EXTENSION_PATTERN, url)):
+            raise ValueError(f"Invalid url: {url}")
+        category, value = groups.groups()
+        for i in cls:
+            if category.lower() in i.value.categories:
+                return RequestObject(extension=i.name, category=category, value=value)
+        raise ValueError(f"Invalid url: {url}")
+
+    @classmethod
     def get_categories(cls, name: str) -> t.List[str]:
         return [i.replace("-", "_") for i in getattr(cls[name].value, "categories", [])]
```

### Comparing `pokelance-0.1.3/pokelance/exceptions.py` & `pokelance-0.1.4/pokelance/exceptions.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/ext/__init__.py` & `pokelance-0.1.4/pokelance/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/ext/_base.py` & `pokelance-0.1.4/pokelance/ext/_base.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/ext/berry.py` & `pokelance-0.1.4/pokelance/ext/berry.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/ext/contest.py` & `pokelance-0.1.4/pokelance/ext/contest.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/ext/encounter.py` & `pokelance-0.1.4/pokelance/ext/encounter.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/ext/evolution.py` & `pokelance-0.1.4/pokelance/ext/evolution.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/ext/game.py` & `pokelance-0.1.4/pokelance/ext/game.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/ext/item.py` & `pokelance-0.1.4/pokelance/ext/item.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/ext/location.py` & `pokelance-0.1.4/pokelance/ext/location.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/ext/machine.py` & `pokelance-0.1.4/pokelance/ext/machine.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/ext/move.py` & `pokelance-0.1.4/pokelance/ext/move.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/ext/pokemon.py` & `pokelance-0.1.4/pokelance/ext/pokemon.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/http/__init__.py` & `pokelance-0.1.4/pokelance/http/__init__.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/http/endpoints.py` & `pokelance-0.1.4/pokelance/http/endpoints.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/languages.py` & `pokelance-0.1.4/pokelance/languages.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/logger.py` & `pokelance-0.1.4/pokelance/logger.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/models/__init__.py` & `pokelance-0.1.4/pokelance/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/models/_base.py` & `pokelance-0.1.4/pokelance/models/_base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import typing as t
 
 import attrs
 
 
 @attrs.define(hash=True, slots=True, kw_only=True)
-class BaseModel:
+class BaseModel(attrs.AttrsInstance):
     """Base model for all models"""
 
     @classmethod
     def from_payload(cls, payload: t.Dict[str, t.Any]) -> "BaseModel":
         """Create a model from a payload
 
         Parameters
```

### Comparing `pokelance-0.1.3/pokelance/models/abstract/__init__.py` & `pokelance-0.1.4/pokelance/models/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/models/abstract/berry.py` & `pokelance-0.1.4/pokelance/models/abstract/berry.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/models/abstract/contest.py` & `pokelance-0.1.4/pokelance/models/abstract/contest.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/models/abstract/encounter.py` & `pokelance-0.1.4/pokelance/models/abstract/encounter.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/models/abstract/evolution.py` & `pokelance-0.1.4/pokelance/models/abstract/evolution.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/models/abstract/game.py` & `pokelance-0.1.4/pokelance/models/abstract/game.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/models/abstract/item.py` & `pokelance-0.1.4/pokelance/models/abstract/item.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/models/abstract/location.py` & `pokelance-0.1.4/pokelance/models/abstract/location.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/models/abstract/machine.py` & `pokelance-0.1.4/pokelance/models/abstract/machine.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/models/abstract/move.py` & `pokelance-0.1.4/pokelance/models/abstract/move.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/models/abstract/pokemon.py` & `pokelance-0.1.4/pokelance/models/abstract/pokemon.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/models/abstract/utils/__init__.py` & `pokelance-0.1.4/pokelance/models/abstract/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/models/abstract/utils/berries.py` & `pokelance-0.1.4/pokelance/models/abstract/utils/berries.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/models/abstract/utils/contests.py` & `pokelance-0.1.4/pokelance/models/abstract/utils/contests.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/models/abstract/utils/evolutions.py` & `pokelance-0.1.4/pokelance/models/abstract/utils/evolutions.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/models/abstract/utils/games.py` & `pokelance-0.1.4/pokelance/models/abstract/utils/games.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/models/abstract/utils/items.py` & `pokelance-0.1.4/pokelance/models/abstract/utils/items.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/models/abstract/utils/locations.py` & `pokelance-0.1.4/pokelance/models/abstract/utils/locations.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/models/abstract/utils/moves.py` & `pokelance-0.1.4/pokelance/models/abstract/utils/moves.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/models/abstract/utils/pokemons.py` & `pokelance-0.1.4/pokelance/models/abstract/utils/pokemons.py`

 * *Files 0% similar despite different names*

```diff
@@ -1110,26 +1110,26 @@
 class MoveStatEffect(BaseModel):
     """A move stat effect resource.
 
     Attributes
     ----------
     change: int
         The maximum amount of change to the referenced stat.
-    stat: NamedResource
-        The stat being affected.
+    move: NamedResource
+        The move causing the effect.
     """
 
     change: int = attrs.field(factory=int)
-    stat: NamedResource = attrs.field(factory=NamedResource)
+    move: NamedResource = attrs.field(factory=NamedResource)
 
     @classmethod
     def from_payload(cls, payload: t.Dict[str, t.Any]) -> "MoveStatEffect":
         return cls(
             change=payload.get("change", 0),
-            stat=NamedResource.from_payload(payload.get("stat", {}) or {}),
+            move=NamedResource.from_payload(payload.get("move", {}) or {}),
         )
 
 
 @attrs.define(slots=True, kw_only=True)
 class MoveStatAffectSets(BaseModel):
     """A move stat affect sets resource.
```

### Comparing `pokelance-0.1.3/pokelance/models/common/__init__.py` & `pokelance-0.1.4/pokelance/models/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/models/common/models.py` & `pokelance-0.1.4/pokelance/models/common/models.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pokelance/models/common/resources.py` & `pokelance-0.1.4/pokelance/models/common/resources.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.3/pyproject.toml` & `pokelance-0.1.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "pokelance"
-version = "0.1.3"
+version = "0.1.4"
 description = "A flexible and easy to use pokemon library."
 authors = ["FallenDeity <61227305+FallenDeity@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-attrs = "^22.1.0"
 aiohttp = "^3.8.3"
 aiofiles = "^23.1.0"
 types-aiofiles = "^23.1.0.1"
+attrs = "^23.1.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 isort = "^5.10.1"
 ruff = "^0.0.171"
 pygments = "^2.13.0"
```

### Comparing `pokelance-0.1.3/PKG-INFO` & `pokelance-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pokelance
-Version: 0.1.3
+Version: 0.1.4
 Summary: A flexible and easy to use pokemon library.
 License: MIT
 Author: FallenDeity
 Author-email: 61227305+FallenDeity@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
-Requires-Dist: attrs (>=22.1.0,<23.0.0)
+Requires-Dist: attrs (>=23.1.0,<24.0.0)
 Requires-Dist: types-aiofiles (>=23.1.0.1,<24.0.0.0)
 Description-Content-Type: text/markdown
 
 <h1 align="center"><b>PokeLance</b></h1>
 <p align="center">
 <img src="https://raw.githubusercontent.com/FallenDeity/PokeLance/master/docs/assets/pokelance.png" width=450 alt="logo"><br><br>
 <img src="https://img.shields.io/github/license/FallenDeity/PokeLance?style=flat-square" alt="license">
@@ -103,25 +103,29 @@
         print(client.berry.get_berry_firmness("very-soft"))
         # The client will be closed automatically when the async context manager exits
     return None
 
 asyncio.run(main())
 ```
 
+# Examples
+
+[Examples](https://fallendeity.github.io/PokeLance/guide/basic_usage/)
+
+Following examples are available open an issue if you want more examples or more details on certain examples.
+- Basic Usage
+- Advanced cache usage
+- Discord bot example
+- FastAPI example
+
+
 ## Important Links
 
 
 - [PokeAPI](https://pokeapi.co/)
 - [PokeAPI Documentation](https://pokeapi.co/docs/v2)
 - [PokeLance Documentation](https://FallenDeity.github.io/PokeLance/)
 - [PokeLance ReadTheDocs](https://pokelance.readthedocs.io/en/latest/)
 - [PokeLance GitHub](https://github.com/FallenDeity/PokeLance)
 - [PokeLance PyPI](https://pypi.org/project/PokeLance/)
 - [PokeLance Discord](https://discord.gg/yeyEvT5V2J)
 
----
-
-!!! note "Note"
-    This is a work in progress. If you find any bugs or have any suggestions, please open an issue [here](https://github.com/FallenDeity/PokeLance/issues/new).
-
----
-
```


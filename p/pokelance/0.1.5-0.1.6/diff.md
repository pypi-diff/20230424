# Comparing `tmp/pokelance-0.1.5.tar.gz` & `tmp/pokelance-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokelance-0.1.5.tar", max compression
+gzip compressed data, was "pokelance-0.1.6.tar", max compression
```

## Comparing `pokelance-0.1.5.tar` & `pokelance-0.1.6.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1068 2023-04-24 10:08:39.981570 pokelance-0.1.5/LICENSE
--rw-r--r--   0        0        0     3817 2023-04-24 10:08:39.981570 pokelance-0.1.5/README.md
--rw-r--r--   0        0        0      106 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/__init__.py
--rw-r--r--   0        0        0      431 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/cache/__init__.py
--rw-r--r--   0        0        0    14722 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/cache/cache.py
--rw-r--r--   0        0        0    13942 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/cache/cache_manager.py
--rw-r--r--   0        0        0     9646 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/client.py
--rw-r--r--   0        0        0     7050 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/constants.py
--rw-r--r--   0        0        0     3868 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/exceptions.py
--rw-r--r--   0        0        0      530 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/ext/__init__.py
--rw-r--r--   0        0        0     3163 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/ext/_base.py
--rw-r--r--   0        0        0     7196 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/ext/berry.py
--rw-r--r--   0        0        0     7189 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/ext/contest.py
--rw-r--r--   0        0        0     7747 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/ext/encounter.py
--rw-r--r--   0        0        0     4990 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/ext/evolution.py
--rw-r--r--   0        0        0     8348 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/ext/game.py
--rw-r--r--   0        0        0    11273 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/ext/item.py
--rw-r--r--   0        0        0     9049 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/ext/location.py
--rw-r--r--   0        0        0     2625 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/ext/machine.py
--rw-r--r--   0        0        0    15682 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/ext/move.py
--rw-r--r--   0        0        0    33460 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/ext/pokemon.py
--rw-r--r--   0        0        0     4724 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/http/__init__.py
--rw-r--r--   0        0        0    20467 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/http/endpoints.py
--rw-r--r--   0        0        0     9677 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/languages.py
--rw-r--r--   0        0        0     3588 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/logger.py
--rw-r--r--   0        0        0     1919 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/models/__init__.py
--rw-r--r--   0        0        0      550 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/models/_base.py
--rw-r--r--   0        0        0     1873 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/models/abstract/__init__.py
--rw-r--r--   0        0        0     5528 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/models/abstract/berry.py
--rw-r--r--   0        0        0     4083 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/models/abstract/contest.py
--rw-r--r--   0        0        0     3507 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/models/abstract/encounter.py
--rw-r--r--   0        0        0     2410 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/models/abstract/evolution.py
--rw-r--r--   0        0        0     7628 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/models/abstract/game.py
--rw-r--r--   0        0        0     8794 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/models/abstract/item.py
--rw-r--r--   0        0        0     6706 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/models/abstract/location.py
--rw-r--r--   0        0        0     1222 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/models/abstract/machine.py
--rw-r--r--   0        0        0    12765 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/models/abstract/move.py
--rw-r--r--   0        0        0    35329 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/models/abstract/pokemon.py
--rw-r--r--   0        0        0     1137 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/models/abstract/showdown.py
--rw-r--r--   0        0        0     2506 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/models/abstract/utils/__init__.py
--rw-r--r--   0        0        0     1494 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/models/abstract/utils/berries.py
--rw-r--r--   0        0        0      943 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/models/abstract/utils/contests.py
--rw-r--r--   0        0        0     6255 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/models/abstract/utils/evolutions.py
--rw-r--r--   0        0        0      890 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/models/abstract/utils/games.py
--rw-r--r--   0        0        0     2284 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/models/abstract/utils/items.py
--rw-r--r--   0        0        0     3546 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/models/abstract/utils/locations.py
--rw-r--r--   0        0        0     7112 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/models/abstract/utils/moves.py
--rw-r--r--   0        0        0    42176 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/models/abstract/utils/pokemons.py
--rw-r--r--   0        0        0      650 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/models/common/__init__.py
--rw-r--r--   0        0        0    10868 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/models/common/models.py
--rw-r--r--   0        0        0     1063 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/models/common/resources.py
--rw-r--r--   0        0        0        0 2023-04-24 10:08:39.985570 pokelance-0.1.5/pokelance/py.typed
--rw-r--r--   0        0        0     1114 2023-04-24 10:08:39.985570 pokelance-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     4563 1970-01-01 00:00:00.000000 pokelance-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-24 10:17:02.838422 pokelance-0.1.6/LICENSE
+-rw-r--r--   0        0        0     3817 2023-04-24 10:17:02.838422 pokelance-0.1.6/README.md
+-rw-r--r--   0        0        0      106 2023-04-24 10:17:02.842422 pokelance-0.1.6/pokelance/__init__.py
+-rw-r--r--   0        0        0      431 2023-04-24 10:17:02.842422 pokelance-0.1.6/pokelance/cache/__init__.py
+-rw-r--r--   0        0        0    14722 2023-04-24 10:17:02.842422 pokelance-0.1.6/pokelance/cache/cache.py
+-rw-r--r--   0        0        0    13942 2023-04-24 10:17:02.842422 pokelance-0.1.6/pokelance/cache/cache_manager.py
+-rw-r--r--   0        0        0     9646 2023-04-24 10:17:02.842422 pokelance-0.1.6/pokelance/client.py
+-rw-r--r--   0        0        0     7071 2023-04-24 10:17:02.842422 pokelance-0.1.6/pokelance/constants.py
+-rw-r--r--   0        0        0     3868 2023-04-24 10:17:02.842422 pokelance-0.1.6/pokelance/exceptions.py
+-rw-r--r--   0        0        0      530 2023-04-24 10:17:02.842422 pokelance-0.1.6/pokelance/ext/__init__.py
+-rw-r--r--   0        0        0     3163 2023-04-24 10:17:02.842422 pokelance-0.1.6/pokelance/ext/_base.py
+-rw-r--r--   0        0        0     7196 2023-04-24 10:17:02.842422 pokelance-0.1.6/pokelance/ext/berry.py
+-rw-r--r--   0        0        0     7189 2023-04-24 10:17:02.842422 pokelance-0.1.6/pokelance/ext/contest.py
+-rw-r--r--   0        0        0     7747 2023-04-24 10:17:02.842422 pokelance-0.1.6/pokelance/ext/encounter.py
+-rw-r--r--   0        0        0     4990 2023-04-24 10:17:02.842422 pokelance-0.1.6/pokelance/ext/evolution.py
+-rw-r--r--   0        0        0     8348 2023-04-24 10:17:02.842422 pokelance-0.1.6/pokelance/ext/game.py
+-rw-r--r--   0        0        0    11273 2023-04-24 10:17:02.842422 pokelance-0.1.6/pokelance/ext/item.py
+-rw-r--r--   0        0        0     9049 2023-04-24 10:17:02.842422 pokelance-0.1.6/pokelance/ext/location.py
+-rw-r--r--   0        0        0     2625 2023-04-24 10:17:02.842422 pokelance-0.1.6/pokelance/ext/machine.py
+-rw-r--r--   0        0        0    15682 2023-04-24 10:17:02.842422 pokelance-0.1.6/pokelance/ext/move.py
+-rw-r--r--   0        0        0    33460 2023-04-24 10:17:02.842422 pokelance-0.1.6/pokelance/ext/pokemon.py
+-rw-r--r--   0        0        0     4724 2023-04-24 10:17:02.842422 pokelance-0.1.6/pokelance/http/__init__.py
+-rw-r--r--   0        0        0    20467 2023-04-24 10:17:02.842422 pokelance-0.1.6/pokelance/http/endpoints.py
+-rw-r--r--   0        0        0     9677 2023-04-24 10:17:02.842422 pokelance-0.1.6/pokelance/languages.py
+-rw-r--r--   0        0        0     3588 2023-04-24 10:17:02.842422 pokelance-0.1.6/pokelance/logger.py
+-rw-r--r--   0        0        0     1919 2023-04-24 10:17:02.842422 pokelance-0.1.6/pokelance/models/__init__.py
+-rw-r--r--   0        0        0      550 2023-04-24 10:17:02.842422 pokelance-0.1.6/pokelance/models/_base.py
+-rw-r--r--   0        0        0     1873 2023-04-24 10:17:02.846422 pokelance-0.1.6/pokelance/models/abstract/__init__.py
+-rw-r--r--   0        0        0     5528 2023-04-24 10:17:02.846422 pokelance-0.1.6/pokelance/models/abstract/berry.py
+-rw-r--r--   0        0        0     4083 2023-04-24 10:17:02.846422 pokelance-0.1.6/pokelance/models/abstract/contest.py
+-rw-r--r--   0        0        0     3507 2023-04-24 10:17:02.846422 pokelance-0.1.6/pokelance/models/abstract/encounter.py
+-rw-r--r--   0        0        0     2410 2023-04-24 10:17:02.846422 pokelance-0.1.6/pokelance/models/abstract/evolution.py
+-rw-r--r--   0        0        0     7628 2023-04-24 10:17:02.846422 pokelance-0.1.6/pokelance/models/abstract/game.py
+-rw-r--r--   0        0        0     8794 2023-04-24 10:17:02.846422 pokelance-0.1.6/pokelance/models/abstract/item.py
+-rw-r--r--   0        0        0     6706 2023-04-24 10:17:02.846422 pokelance-0.1.6/pokelance/models/abstract/location.py
+-rw-r--r--   0        0        0     1222 2023-04-24 10:17:02.846422 pokelance-0.1.6/pokelance/models/abstract/machine.py
+-rw-r--r--   0        0        0    12765 2023-04-24 10:17:02.846422 pokelance-0.1.6/pokelance/models/abstract/move.py
+-rw-r--r--   0        0        0    35329 2023-04-24 10:17:02.846422 pokelance-0.1.6/pokelance/models/abstract/pokemon.py
+-rw-r--r--   0        0        0     1137 2023-04-24 10:17:02.846422 pokelance-0.1.6/pokelance/models/abstract/showdown.py
+-rw-r--r--   0        0        0     2506 2023-04-24 10:17:02.846422 pokelance-0.1.6/pokelance/models/abstract/utils/__init__.py
+-rw-r--r--   0        0        0     1494 2023-04-24 10:17:02.846422 pokelance-0.1.6/pokelance/models/abstract/utils/berries.py
+-rw-r--r--   0        0        0      943 2023-04-24 10:17:02.846422 pokelance-0.1.6/pokelance/models/abstract/utils/contests.py
+-rw-r--r--   0        0        0     6255 2023-04-24 10:17:02.846422 pokelance-0.1.6/pokelance/models/abstract/utils/evolutions.py
+-rw-r--r--   0        0        0      890 2023-04-24 10:17:02.846422 pokelance-0.1.6/pokelance/models/abstract/utils/games.py
+-rw-r--r--   0        0        0     2284 2023-04-24 10:17:02.846422 pokelance-0.1.6/pokelance/models/abstract/utils/items.py
+-rw-r--r--   0        0        0     3546 2023-04-24 10:17:02.846422 pokelance-0.1.6/pokelance/models/abstract/utils/locations.py
+-rw-r--r--   0        0        0     7112 2023-04-24 10:17:02.846422 pokelance-0.1.6/pokelance/models/abstract/utils/moves.py
+-rw-r--r--   0        0        0    42176 2023-04-24 10:17:02.846422 pokelance-0.1.6/pokelance/models/abstract/utils/pokemons.py
+-rw-r--r--   0        0        0      650 2023-04-24 10:17:02.846422 pokelance-0.1.6/pokelance/models/common/__init__.py
+-rw-r--r--   0        0        0    10868 2023-04-24 10:17:02.846422 pokelance-0.1.6/pokelance/models/common/models.py
+-rw-r--r--   0        0        0     1063 2023-04-24 10:17:02.846422 pokelance-0.1.6/pokelance/models/common/resources.py
+-rw-r--r--   0        0        0        0 2023-04-24 10:17:02.846422 pokelance-0.1.6/pokelance/py.typed
+-rw-r--r--   0        0        0     1114 2023-04-24 10:17:02.846422 pokelance-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     4563 1970-01-01 00:00:00.000000 pokelance-0.1.6/PKG-INFO
```

### Comparing `pokelance-0.1.5/LICENSE` & `pokelance-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/README.md` & `pokelance-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/cache/cache.py` & `pokelance-0.1.6/pokelance/cache/cache.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/cache/cache_manager.py` & `pokelance-0.1.6/pokelance/cache/cache_manager.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/client.py` & `pokelance-0.1.6/pokelance/client.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/constants.py` & `pokelance-0.1.6/pokelance/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     "LocationExtension",
     "MachineExtension",
     "MoveExtension",
     "PokemonExtension",
     "ExtensionEnum",
     "ExtensionsL",
     "ShowdownEnum",
+    "RequestObject",
 )
 
 
 ExtensionsL = t.Literal[
     "berry", "contest", "encounter", "evolution", "game", "item", "location", "machine", "move", "pokemon"
 ]
 PATH: str = "https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/other/showdown/"
```

### Comparing `pokelance-0.1.5/pokelance/exceptions.py` & `pokelance-0.1.6/pokelance/exceptions.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/ext/__init__.py` & `pokelance-0.1.6/pokelance/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/ext/_base.py` & `pokelance-0.1.6/pokelance/ext/_base.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/ext/berry.py` & `pokelance-0.1.6/pokelance/ext/berry.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/ext/contest.py` & `pokelance-0.1.6/pokelance/ext/contest.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/ext/encounter.py` & `pokelance-0.1.6/pokelance/ext/encounter.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/ext/evolution.py` & `pokelance-0.1.6/pokelance/ext/evolution.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/ext/game.py` & `pokelance-0.1.6/pokelance/ext/game.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/ext/item.py` & `pokelance-0.1.6/pokelance/ext/item.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/ext/location.py` & `pokelance-0.1.6/pokelance/ext/location.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/ext/machine.py` & `pokelance-0.1.6/pokelance/ext/machine.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/ext/move.py` & `pokelance-0.1.6/pokelance/ext/move.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/ext/pokemon.py` & `pokelance-0.1.6/pokelance/ext/pokemon.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/http/__init__.py` & `pokelance-0.1.6/pokelance/http/__init__.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/http/endpoints.py` & `pokelance-0.1.6/pokelance/http/endpoints.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/languages.py` & `pokelance-0.1.6/pokelance/languages.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/logger.py` & `pokelance-0.1.6/pokelance/logger.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/models/__init__.py` & `pokelance-0.1.6/pokelance/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/models/_base.py` & `pokelance-0.1.6/pokelance/models/_base.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/models/abstract/__init__.py` & `pokelance-0.1.6/pokelance/models/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/models/abstract/berry.py` & `pokelance-0.1.6/pokelance/models/abstract/berry.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/models/abstract/contest.py` & `pokelance-0.1.6/pokelance/models/abstract/contest.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/models/abstract/encounter.py` & `pokelance-0.1.6/pokelance/models/abstract/encounter.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/models/abstract/evolution.py` & `pokelance-0.1.6/pokelance/models/abstract/evolution.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/models/abstract/game.py` & `pokelance-0.1.6/pokelance/models/abstract/game.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/models/abstract/item.py` & `pokelance-0.1.6/pokelance/models/abstract/item.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/models/abstract/location.py` & `pokelance-0.1.6/pokelance/models/abstract/location.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/models/abstract/machine.py` & `pokelance-0.1.6/pokelance/models/abstract/machine.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/models/abstract/move.py` & `pokelance-0.1.6/pokelance/models/abstract/move.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/models/abstract/pokemon.py` & `pokelance-0.1.6/pokelance/models/abstract/pokemon.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/models/abstract/showdown.py` & `pokelance-0.1.6/pokelance/models/abstract/showdown.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/models/abstract/utils/__init__.py` & `pokelance-0.1.6/pokelance/models/abstract/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/models/abstract/utils/berries.py` & `pokelance-0.1.6/pokelance/models/abstract/utils/berries.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/models/abstract/utils/contests.py` & `pokelance-0.1.6/pokelance/models/abstract/utils/contests.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/models/abstract/utils/evolutions.py` & `pokelance-0.1.6/pokelance/models/abstract/utils/evolutions.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/models/abstract/utils/games.py` & `pokelance-0.1.6/pokelance/models/abstract/utils/games.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/models/abstract/utils/items.py` & `pokelance-0.1.6/pokelance/models/abstract/utils/items.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/models/abstract/utils/locations.py` & `pokelance-0.1.6/pokelance/models/abstract/utils/locations.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/models/abstract/utils/moves.py` & `pokelance-0.1.6/pokelance/models/abstract/utils/moves.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/models/abstract/utils/pokemons.py` & `pokelance-0.1.6/pokelance/models/abstract/utils/pokemons.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/models/common/__init__.py` & `pokelance-0.1.6/pokelance/models/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/models/common/models.py` & `pokelance-0.1.6/pokelance/models/common/models.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pokelance/models/common/resources.py` & `pokelance-0.1.6/pokelance/models/common/resources.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.1.5/pyproject.toml` & `pokelance-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pokelance"
-version = "0.1.5"
+version = "0.1.6"
 description = "A flexible and easy to use pokemon library."
 authors = ["FallenDeity <61227305+FallenDeity@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `pokelance-0.1.5/PKG-INFO` & `pokelance-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pokelance
-Version: 0.1.5
+Version: 0.1.6
 Summary: A flexible and easy to use pokemon library.
 License: MIT
 Author: FallenDeity
 Author-email: 61227305+FallenDeity@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


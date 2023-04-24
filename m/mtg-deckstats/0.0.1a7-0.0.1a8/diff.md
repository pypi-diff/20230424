# Comparing `tmp/mtg_deckstats-0.0.1a7.tar.gz` & `tmp/mtg_deckstats-0.0.1a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtg_deckstats-0.0.1a7.tar", max compression
+gzip compressed data, was "mtg_deckstats-0.0.1a8.tar", max compression
```

## Comparing `mtg_deckstats-0.0.1a7.tar` & `mtg_deckstats-0.0.1a8.tar`

### file list

```diff
@@ -1,22 +1,20 @@
--rw-r--r--   0        0        0     1074 2022-06-25 21:00:35.231171 mtg_deckstats-0.0.1a7/LICENSE
--rw-r--r--   0        0        0     1038 2022-07-03 20:52:49.994471 mtg_deckstats-0.0.1a7/README.md
--rw-r--r--   0        0        0     1302 2022-10-16 21:04:51.508776 mtg_deckstats-0.0.1a7/pyproject.toml
--rw-r--r--   0        0        0      161 2022-10-16 21:25:25.678201 mtg_deckstats-0.0.1a7/src/mtg_deckstats/__init__.py
--rw-r--r--   0        0        0      300 2022-08-24 20:52:02.265947 mtg_deckstats-0.0.1a7/src/mtg_deckstats/base_step.py
--rw-r--r--   0        0        0      982 2022-08-24 20:52:06.401004 mtg_deckstats-0.0.1a7/src/mtg_deckstats/canadian_highlander_step.py
--rw-r--r--   0        0        0     3417 2022-08-24 20:52:09.840655 mtg_deckstats-0.0.1a7/src/mtg_deckstats/combo_potential_step.py
--rw-r--r--   0        0        0     1385 2022-08-24 21:01:18.728333 mtg_deckstats-0.0.1a7/src/mtg_deckstats/commander_tier_step.py
--rw-r--r--   0        0        0      219 2022-08-24 20:52:16.391736 mtg_deckstats-0.0.1a7/src/mtg_deckstats/create_report_step.py
--rw-r--r--   0        0        0     1373 2022-10-16 21:16:54.409682 mtg_deckstats-0.0.1a7/src/mtg_deckstats/deck_composition_step.py
--rw-r--r--   0        0        0     2074 2022-06-26 09:52:26.240774 mtg_deckstats-0.0.1a7/src/mtg_deckstats/graph.py
--rw-r--r--   0        0        0     2970 2022-07-18 21:52:04.359654 mtg_deckstats-0.0.1a7/src/mtg_deckstats/mana_base_step.py
--rw-r--r--   0        0        0      501 2022-08-24 20:52:26.108988 mtg_deckstats-0.0.1a7/src/mtg_deckstats/mana_producers_step.py
--rw-r--r--   0        0        0      621 2022-08-24 20:52:29.329501 mtg_deckstats-0.0.1a7/src/mtg_deckstats/mana_value_step.py
--rw-r--r--   0        0        0     1319 2022-08-24 20:52:34.609677 mtg_deckstats-0.0.1a7/src/mtg_deckstats/parse_deck_step.py
--rw-r--r--   0        0        0     3746 2022-10-16 21:25:25.679006 mtg_deckstats-0.0.1a7/src/mtg_deckstats/rank.py
--rw-r--r--   0        0        0      343 2022-08-24 20:52:40.348213 mtg_deckstats-0.0.1a7/src/mtg_deckstats/rarity_step.py
--rw-r--r--   0        0        0     2313 2022-10-16 21:16:54.411424 mtg_deckstats-0.0.1a7/src/mtg_deckstats/report.py
--rw-r--r--   0        0        0     1285 2022-10-16 19:47:18.139184 mtg_deckstats-0.0.1a7/src/mtg_deckstats/salt_step.py
--rw-r--r--   0        0        0      322 2022-08-24 20:53:02.211927 mtg_deckstats-0.0.1a7/src/mtg_deckstats/utils.py
--rw-r--r--   0        0        0     1958 2022-10-16 21:25:26.860532 mtg_deckstats-0.0.1a7/setup.py
--rw-r--r--   0        0        0     1988 2022-10-16 21:25:26.861051 mtg_deckstats-0.0.1a7/PKG-INFO
+-rw-r--r--   0        0        0     1074 2022-06-25 21:00:35.231171 mtg_deckstats-0.0.1a8/LICENSE
+-rw-r--r--   0        0        0     1038 2022-07-03 20:52:49.994471 mtg_deckstats-0.0.1a8/README.md
+-rw-r--r--   0        0        0     1375 2023-04-24 20:19:01.196336 mtg_deckstats-0.0.1a8/pyproject.toml
+-rw-r--r--   0        0        0      188 2023-04-24 20:20:39.985421 mtg_deckstats-0.0.1a8/src/mtg_deckstats/__init__.py
+-rw-r--r--   0        0        0       71 2023-04-24 20:20:39.985923 mtg_deckstats-0.0.1a8/src/mtg_deckstats/__version__.py
+-rw-r--r--   0        0        0     1147 2023-04-24 19:00:30.272932 mtg_deckstats-0.0.1a8/src/mtg_deckstats/canadian_highlander_step.py
+-rw-r--r--   0        0        0     3593 2023-04-24 19:00:47.228945 mtg_deckstats-0.0.1a8/src/mtg_deckstats/combo_potential_step.py
+-rw-r--r--   0        0        0     1617 2023-04-24 19:01:05.090951 mtg_deckstats-0.0.1a8/src/mtg_deckstats/commander_tier_step.py
+-rw-r--r--   0        0        0      219 2022-08-24 20:52:16.391736 mtg_deckstats-0.0.1a8/src/mtg_deckstats/create_report_step.py
+-rw-r--r--   0        0        0     1564 2023-04-24 19:01:29.817586 mtg_deckstats-0.0.1a8/src/mtg_deckstats/deck_composition_step.py
+-rw-r--r--   0        0        0     2074 2022-06-26 09:52:26.240774 mtg_deckstats-0.0.1a8/src/mtg_deckstats/graph.py
+-rw-r--r--   0        0        0      501 2022-08-24 20:52:26.108988 mtg_deckstats-0.0.1a8/src/mtg_deckstats/mana_producers_step.py
+-rw-r--r--   0        0        0      621 2022-08-24 20:52:29.329501 mtg_deckstats-0.0.1a8/src/mtg_deckstats/mana_value_step.py
+-rw-r--r--   0        0        0     1403 2023-04-24 19:03:29.260576 mtg_deckstats-0.0.1a8/src/mtg_deckstats/parse_deck_step.py
+-rw-r--r--   0        0        0     3766 2023-04-24 20:20:39.986496 mtg_deckstats-0.0.1a8/src/mtg_deckstats/rank.py
+-rw-r--r--   0        0        0      343 2022-08-24 20:52:40.348213 mtg_deckstats-0.0.1a8/src/mtg_deckstats/rarity_step.py
+-rw-r--r--   0        0        0     2792 2023-04-24 20:20:39.987200 mtg_deckstats-0.0.1a8/src/mtg_deckstats/report.py
+-rw-r--r--   0        0        0     1450 2023-04-24 19:04:55.039869 mtg_deckstats-0.0.1a8/src/mtg_deckstats/salt_step.py
+-rw-r--r--   0        0        0      321 2023-04-24 20:06:51.034922 mtg_deckstats-0.0.1a8/src/mtg_deckstats/utils.py
+-rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 mtg_deckstats-0.0.1a8/PKG-INFO
```

### Comparing `mtg_deckstats-0.0.1a7/LICENSE` & `mtg_deckstats-0.0.1a8/LICENSE`

 * *Files identical despite different names*

### Comparing `mtg_deckstats-0.0.1a7/README.md` & `mtg_deckstats-0.0.1a8/README.md`

 * *Files identical despite different names*

### Comparing `mtg_deckstats-0.0.1a7/pyproject.toml` & `mtg_deckstats-0.0.1a8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "mtg_deckstats"
-version = "0.0.1-alpha.7"
+version = "0.0.1a8"
 license = "MIT"
 description = "Magic: the Gathering deckstats"
 readme = "README.md"
 authors = ["Ludovic Heyberger <940408+lheyberger@users.noreply.github.com>"]
 homepage = "https://github.com/lheyberger/mtg-deckstats"
 repository = "https://github.com/lheyberger/mtg-deckstats"
 documentation = "https://github.com/lheyberger/mtg-deckstats"
 
 
+[tool.poetry.scripts]
+pre_cache = "scripts.pre_cache:main"
+
+
 [tool.poetry.dependencies]
+beautifulsoup4 = "^4.12.2"
+more-itertools = "^9.1.0"
+mtg-parser = "^0.0.1a28"
 python = "^3.7"
-requests = "^2.25.1"
-beautifulsoup4 = "^4.9.3"
-mtg-parser = "^0.0.1-alpha.26"
-more-itertools = "^8.13.0"
+requests = "^2.28.2"
 
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
+check-wheel-contents = "^0.4.0"
+click = "^8.1.3"
 coverage = {extras = ["toml"], version = "^5.5"}
-pytest = "^6.2.2"
-check-wheel-contents = "^0.2.0"
-pylint = "^2.7.4"
 flake8 = "^3.9.0"
-requests-mock = "^1.8.0"
 Jinja2 = "^3.1.2"
+pylint = "^2.7.4"
+pytest = "^7.3.1"
+requests-mock = "^1.10.0"
 
 
 [tool.pylint."MESSAGES CONTROL"]
 disable = [
     "missing-module-docstring",
     "missing-class-docstring",
     "missing-function-docstring",
```

### Comparing `mtg_deckstats-0.0.1a7/src/mtg_deckstats/combo_potential_step.py` & `mtg_deckstats-0.0.1a8/src/mtg_deckstats/combo_potential_step.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from functools import reduce
 from operator import itemgetter
 import requests
-from mtg_deckstats.base_step import BaseStep
 
 
 __all__ = []
 
 
-class ComboPotentialStep(BaseStep):
+class ComboPotentialStep():
+
+    def __init__(self, data: dict = None, session=None):
+        self._data = (data or {}).get(self.__class__.__name__)
+        self._session = session
 
     def __call__(self, deck):
-        combo_list = self.data or self.load_data()
+        combo_list = self._data or self.load_data(self._session)
 
         cards = deck.get('cards', [])
         card_names = set(card.get('name') for card in cards)
 
         color_identities = (
             set(card.get('color_identity', ()))
             for card in cards
@@ -29,15 +32,15 @@
 
         combo_list = (
             c for c in combo_list
             if not color_identity_filter & set(c['ci'])
         )
         combo_list = (
             c for c in combo_list
-            if c['cards'] <= card_names
+            if set(c['cards']) <= card_names
         )
 
         combos = []
         for combo in combo_list:
             combo_cards = list(
                 c for c in cards
                 if c.get('name') in combo.get('cards')
@@ -82,22 +85,23 @@
         combo_levels = map(
             lambda c: next((level for level, f in levels if f(c)), 0),
             combos
         )
         return max(combo_levels, default=0)
 
     @classmethod
-    def load_data(cls):
+    def load_data(cls, session=None):
+        session = session or requests
         url = (
             'https://docs.google.com/spreadsheets/d/'
             '1KqyDRZRCgy8YgMFnY0tHSw_3jC99Z0zFvJrPbfm66vA/export'
             '?format=tsv&id=1KqyDRZRCgy8YgMFnY0tHSw_3jC99Z0zFvJrPbfm66vA&gid=0'
         )
         lines = (
-            requests
+            session
             .get(url)
             .content
             .decode('utf-8')
             .split('\r\n')
         )
         lines = [line.split('\t') for line in lines]
         lines = lines[1:]
@@ -107,12 +111,12 @@
             if not line[17]:
                 continue
 
             cards = set(line[1:10])
             cards.discard('')
 
             combo_list.append({
-                'cards': cards,
+                'cards': list(cards),
                 'ci': ''.join(set('wubrg') & set(line[11])),
             })
 
         return combo_list
```

### Comparing `mtg_deckstats-0.0.1a7/src/mtg_deckstats/commander_tier_step.py` & `mtg_deckstats-0.0.1a8/src/mtg_deckstats/commander_tier_step.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,47 +1,57 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
+import requests
 import mtg_parser
 from more_itertools import flatten
 from mtg_deckstats.utils import cleanup_name
-from mtg_deckstats.base_step import BaseStep
 
 
 __all__ = []
 
 
-class CommanderTierStep(BaseStep):
+class CommanderTierStep():
 
-    def __call__(self, deck):
-        cmdrs, tiers, default = self.data or self.load_data()
-
-        power = deck.get('cards', [])
-        power = filter(lambda c: 'commander' in c.get('tags', ()), power)
-        power = map(lambda c: cleanup_name(c.get('name')), power)
-        power = map(lambda name: cmdrs.get(name, default), power)
-        power = map(lambda t: max(9 - tiers.index(t), 0), power)
-        power = max(power)
+    def __init__(self, data: dict = None, session=None):
+        self._data = (data or {}).get(self.__class__.__name__)
+        self._session = session
 
+    def __call__(self, deck):
+        cmdrs = self._data or self.load_data(self._session)
+        cards = deck.get('cards', [])
+        commanders = filter(lambda c: 'commander' in c.get('tags', ()), cards)
+        names = map(lambda c: cleanup_name(c.get('name')), commanders)
+        powers = map(lambda name: cmdrs.get(name, 0), names)
+        power = max(powers)
         return {
             'commander_power_tier': power,
         }
 
     @classmethod
-    def load_data(cls):
+    def load_data(cls, session=None):
+        session = session or requests
         sources = [
             (
                 'https://tappedout.net/'
                 'mtg-decks/best-commanders-in-edh-tier-list-part-1/'
             ),
             (
                 'https://tappedout.net/'
                 'mtg-decks/best-commanders-in-edh-tier-list-part-2/'
             ),
         ]
-        decks = map(mtg_parser.parse_deck, sources)
-        cmdrs = flatten(decks)
-        cmdrs = dict(map(lambda c: (c.name, ' '.join(c.tags)), cmdrs))
-        tiers = sorted(set(value for value in cmdrs.values() if value))
-        default = tiers[-1]
 
-        return cmdrs, tiers, default
+        decks = (mtg_parser.parse_deck(src, session) for src in sources)
+        cards = flatten(decks)
+
+        cmdrs = {}
+        tiers = set()
+        for card in cards:
+            name = cleanup_name(card.name)
+            tier = ''.join(card.tags)
+            cmdrs[name] = tier
+            tiers.add(tier)
+
+        tiers = sorted(tiers)
+
+        return {k: max(9 - tiers.index(v), 0) for k, v in cmdrs.items()}
```

### Comparing `mtg_deckstats-0.0.1a7/src/mtg_deckstats/deck_composition_step.py` & `mtg_deckstats-0.0.1a8/src/mtg_deckstats/deck_composition_step.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
+import requests
 import mtg_parser
-from mtg_deckstats.base_step import BaseStep
 
 
 __all__ = []
 
 
-class DeckCompositionStep(BaseStep):
+class DeckCompositionStep():
+
+    def __init__(self, data: dict = None, session=None):
+        self._data = (data or {}).get(self.__class__.__name__)
+        self._session = session
 
     def __call__(self, deck):
-        categories = self.data or self.load_data()
+        categories = self._data or self.load_data(self._session)
         card_names = set(c.get('name') for c in deck.get('cards', []))
 
         def how_many(category):
             return len(card_names & categories.get(category, set()))
 
         return {
             'board_wipes': how_many('board_wipes'),
             'target_answers': how_many('target_answers'),
             'steady_draw': how_many('steady_draw'),
             'burst_draw': how_many('burst_draw'),
             'tutors': how_many('tutors'),
         }
 
     @classmethod
-    def load_data(cls):
+    def load_data(cls, session=None):
+        session = session or requests
         sources = {
             'board_wipes':
                 'https://tappedout.net/mtg-decks/mh-mass-answers/',
             'target_answers':
                 'https://tappedout.net/mtg-decks/mh-targeted-answers/',
             'steady_draw':
                 'https://tappedout.net/mtg-decks/mh-draw-s/',
             'burst_draw':
                 'https://tappedout.net/mtg-decks/mh-draw-b/',
             'tutors':
                 'https://tappedout.net/mtg-decks/mh-tutors/',
         }
         return {
-            cat: set(card.name for card in mtg_parser.parse_deck(src))
+            cat: set(card.name for card in mtg_parser.parse_deck(src, session))
             for cat, src in sources.items()
         }
```

### Comparing `mtg_deckstats-0.0.1a7/src/mtg_deckstats/graph.py` & `mtg_deckstats-0.0.1a8/src/mtg_deckstats/graph.py`

 * *Files identical despite different names*

### Comparing `mtg_deckstats-0.0.1a7/src/mtg_deckstats/mana_value_step.py` & `mtg_deckstats-0.0.1a8/src/mtg_deckstats/mana_value_step.py`

 * *Files identical despite different names*

### Comparing `mtg_deckstats-0.0.1a7/src/mtg_deckstats/parse_deck_step.py` & `mtg_deckstats-0.0.1a8/src/mtg_deckstats/parse_deck_step.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,28 +17,29 @@
         'type_line',
         'cmc',
         'color_identity',
         'produced_mana',
         'rarity',
     ]
 
-    def __init__(self, deck_url):
-        self._deck_url_ = deck_url
+    def __init__(self, deck_url, session=None):
+        self._deck_url = deck_url
+        self._session = session or requests
 
     def __call__(self):
-        cards = mtg_parser.parse_deck(self._deck_url_)
+        cards = mtg_parser.parse_deck(self._deck_url, session=self._session)
         cards = list(cards)
         half = int(len(cards)/2)
 
         new_cardlist = []
 
         for batch in (cards[:half], cards[half:]):
             identifiers = [{'name': cleanup_name(card.name)} for card in batch]
             payload = {'identifiers': identifiers}
-            response = requests.post(self._endpoint_, json=payload)
+            response = self._session.post(self._endpoint_, json=payload)
             j = response.json()
             new_cardlist.extend(map(
                 lambda c: {k: v for (k, v) in c.items() if k in self._fields_},
                 j.get('data', [])
             ))
 
         for card in cards:
```

### Comparing `mtg_deckstats-0.0.1a7/src/mtg_deckstats/rank.py` & `mtg_deckstats-0.0.1a8/src/mtg_deckstats/rank.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from mtg_deckstats.report import compute
+from mtg_deckstats.__version__ import __version__
 
 
 __all__ = ['rank_source', 'rank_report']
-__version__ = '0.0.1-alpha.7'
 
 
 def rank_source(src: str, data: dict = None) -> dict:
 
     report = compute(src, data=data)
 
     return rank_report(report)
```

### Comparing `mtg_deckstats-0.0.1a7/src/mtg_deckstats/report.py` & `mtg_deckstats-0.0.1a8/src/mtg_deckstats/report.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
+from multiprocessing.pool import ThreadPool as Pool
+
+import requests
+
+from mtg_deckstats.__version__ import __version__
 from mtg_deckstats.graph import run_graph
 from mtg_deckstats.canadian_highlander_step import CanadianHighlanderStep
 from mtg_deckstats.combo_potential_step import ComboPotentialStep
 from mtg_deckstats.commander_tier_step import CommanderTierStep
 from mtg_deckstats.create_report_step import CreateReportStep
 from mtg_deckstats.deck_composition_step import DeckCompositionStep
 from mtg_deckstats.mana_producers_step import ManaProducersStep
@@ -13,24 +18,29 @@
 from mtg_deckstats.rarity_step import RarityStep
 from mtg_deckstats.salt_step import SaltStep
 
 
 __all__ = ['compute', 'pre_cache']
 
 
-def compute(src: str, data: dict = None) -> dict:
+def compute(src: str, data: dict = None, session=None) -> dict:
+    session = session or requests
+    context = {
+        'data': data,
+        'session': session,
+    }
     functions = {
-        'parse_deck': ParseDeckStep(src),
+        'parse_deck': ParseDeckStep(src, session=session),
         'mana_value': ManaValueStep(),
         'rarity': RarityStep(),
-        'canadian_highlander': CanadianHighlanderStep(data=data),
-        'salt': SaltStep(data=data),
-        'commander_tier': CommanderTierStep(data=data),
-        'deck_composition': DeckCompositionStep(data=data),
-        'combo_potential': ComboPotentialStep(data=data),
+        'canadian_highlander': CanadianHighlanderStep(**context),
+        'salt': SaltStep(**context),
+        'commander_tier': CommanderTierStep(**context),
+        'deck_composition': DeckCompositionStep(**context),
+        'combo_potential': ComboPotentialStep(**context),
         'mana_producers': ManaProducersStep(),
         'create_report': CreateReportStep(),
     }
     dependencies = {
         'parse_deck': [],
         'mana_value': ['parse_deck'],
         'rarity': ['parse_deck'],
@@ -54,18 +64,26 @@
 
     results = run_graph(functions, dependencies)
     result = results.get('create_report', {})
 
     return {'src': src, **result}
 
 
-def pre_cache():
+def pre_cache(session=None):
+    session = session or requests
     steps = [
         CanadianHighlanderStep,
         SaltStep,
         CommanderTierStep,
         DeckCompositionStep,
         ComboPotentialStep,
     ]
 
-    cache = {step.__name__: step.load_data() for step in steps}
+    def load_data(step):
+        return step.__name__, step.load_data(session)
+
+    with Pool(processes=max(len(steps), 5)) as pool:
+        results = pool.map(load_data, steps)
+
+    cache = dict(results)
+    cache['version'] = __version__
     return cache
```

### Comparing `mtg_deckstats-0.0.1a7/src/mtg_deckstats/salt_step.py` & `mtg_deckstats-0.0.1a8/src/mtg_deckstats/salt_step.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,34 +2,38 @@
 # -*- coding: utf-8 -*-
 
 import re
 import itertools
 import requests
 import more_itertools
 from mtg_deckstats.utils import yield_cards
-from mtg_deckstats.base_step import BaseStep
 
 
 __all__ = []
 
 
-class SaltStep(BaseStep):
+class SaltStep():
+
+    def __init__(self, data: dict = None, session=None):
+        self._data = (data or {}).get(self.__class__.__name__)
+        self._session = session
 
     def __call__(self, deck):
-        salt_score = self.data or self.load_data()
+        salt_score = self._data or self.load_data(self._session)
         card_names = [card.get('name') for card in yield_cards(deck)]
         score = sum(v for k, v in salt_score.items() if k in card_names)
         return {
             'salt_score': round(score, 2),
         }
 
     @classmethod
-    def load_data(cls):
+    def load_data(cls, session=None):
+        session = session or requests
         cardlists = (
-            requests
+            session
             .get('https://json.edhrec.com/pages/top/salt-2021.json')
             .json()
             .get('container', {})
             .get('json_dict', {})
             .get('cardlists', [])
         )
         cardviews = (c.get('cardviews', {}) for c in cardlists)
```

### Comparing `mtg_deckstats-0.0.1a7/PKG-INFO` & `mtg_deckstats-0.0.1a8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: mtg-deckstats
-Version: 0.0.1a7
+Version: 0.0.1a8
 Summary: Magic: the Gathering deckstats
 Home-page: https://github.com/lheyberger/mtg-deckstats
 License: MIT
 Author: Ludovic Heyberger
 Author-email: 940408+lheyberger@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: beautifulsoup4 (>=4.9.3,<5.0.0)
-Requires-Dist: more-itertools (>=8.13.0,<9.0.0)
-Requires-Dist: mtg-parser (>=0.0.1-alpha.26,<0.0.2)
-Requires-Dist: requests (>=2.25.1,<3.0.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
+Requires-Dist: more-itertools (>=9.1.0,<10.0.0)
+Requires-Dist: mtg-parser (>=0.0.1a28,<0.0.2)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Documentation, https://github.com/lheyberger/mtg-deckstats
 Project-URL: Repository, https://github.com/lheyberger/mtg-deckstats
 Description-Content-Type: text/markdown
 
 # mtg-deckstats
 
 ![PyPI](https://img.shields.io/pypi/v/mtg-deckstats)
```


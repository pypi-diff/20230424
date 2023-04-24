# Comparing `tmp/pokerlib-2.1.1.tar.gz` & `tmp/pokerlib-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokerlib-2.1.1.tar", max compression
+gzip compressed data, was "pokerlib-2.2.0.tar", max compression
```

## Comparing `pokerlib-2.1.1.tar` & `pokerlib-2.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35147 2022-10-03 17:39:48.345471 pokerlib-2.1.1/LICENSE
--rw-r--r--   0        0        0     6833 2023-04-03 20:53:18.762679 pokerlib-2.1.1/README.md
--rw-r--r--   0        0        0      493 2023-04-07 09:40:14.276227 pokerlib-2.1.1/pokerlib/__init__.py
--rw-r--r--   0        0        0     8934 2023-02-23 20:42:05.954724 pokerlib-2.1.1/pokerlib/_handparser.py
--rw-r--r--   0        0        0     4149 2023-04-03 19:34:35.852712 pokerlib-2.1.1/pokerlib/_player.py
--rw-r--r--   0        0        0    14917 2023-04-07 09:35:55.186229 pokerlib-2.1.1/pokerlib/_round.py
--rw-r--r--   0        0        0     6936 2023-04-07 09:33:14.596230 pokerlib-2.1.1/pokerlib/_table.py
--rw-r--r--   0        0        0     1523 2023-04-04 09:05:46.153989 pokerlib-2.1.1/pokerlib/enums.py
--rw-r--r--   0        0        0      107 2023-04-03 19:58:33.722702 pokerlib-2.1.1/pokerlib/implementations/__init__.py
--rw-r--r--   0        0        0     2473 2023-04-07 09:34:44.876229 pokerlib-2.1.1/pokerlib/implementations/_table_with_choice_to_show_cards.py
--rw-r--r--   0        0        0      663 2023-04-07 09:39:18.996227 pokerlib-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     7602 1970-01-01 00:00:00.000000 pokerlib-2.1.1/setup.py
--rw-r--r--   0        0        0     7558 1970-01-01 00:00:00.000000 pokerlib-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35147 2022-10-03 17:39:48.345471 pokerlib-2.2.0/LICENSE
+-rw-r--r--   0        0        0     6276 2023-04-24 16:13:38.139069 pokerlib-2.2.0/README.md
+-rw-r--r--   0        0        0      493 2023-04-24 16:14:50.939071 pokerlib-2.2.0/pokerlib/__init__.py
+-rw-r--r--   0        0        0     9058 2023-04-20 19:59:08.048593 pokerlib-2.2.0/pokerlib/_handparser.py
+-rw-r--r--   0        0        0     5387 2023-04-20 21:01:45.318611 pokerlib-2.2.0/pokerlib/_player.py
+-rw-r--r--   0        0        0    17502 2023-04-24 10:35:35.288769 pokerlib-2.2.0/pokerlib/_round.py
+-rw-r--r--   0        0        0     6936 2023-04-07 09:33:14.596230 pokerlib-2.2.0/pokerlib/_table.py
+-rw-r--r--   0        0        0     1652 2023-04-20 20:01:46.748594 pokerlib-2.2.0/pokerlib/enums.py
+-rw-r--r--   0        0        0      122 2023-04-20 19:44:07.068589 pokerlib-2.2.0/pokerlib/implementations/__init__.py
+-rw-r--r--   0        0        0      462 2023-04-20 19:43:30.238589 pokerlib-2.2.0/pokerlib/implementations/_no_muck_showdown_table.py
+-rw-r--r--   0        0        0      360 2023-04-20 19:50:58.588591 pokerlib-2.2.0/pokerlib/implementations/_no_muck_table.py
+-rw-r--r--   0        0        0      663 2023-04-24 16:14:19.719070 pokerlib-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7001 1970-01-01 00:00:00.000000 pokerlib-2.2.0/PKG-INFO
```

### Comparing `pokerlib-2.1.1/LICENSE` & `pokerlib-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pokerlib-2.1.1/README.md` & `pokerlib-2.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -135,42 +135,17 @@
 table.publicIn(player2.id, RoundPublicInId.CHECK)
 table.publicIn(player1.id, RoundPublicInId.ALLIN)
 table.publicIn(player2.id, RoundPublicInId.CALL)
 ```
 
 Wrong inputs are mostly ignored, though they can produce a response, when it seems useful. As noted before, when providing input, the `table` object responds with output ids (e.g. `PLAYERACTIONREQUIRED`) along with additional data that depends on the output id. For all possible outputs, check `RoundPublicInId` and `TablePublicInId` enums.
 
-A new round has to be initiated by one of the players every time the previous one ends (or at the beginning). A simple command line game, where you respond by enum names, can be implemented as below (for working version check `tests/round_test.py`).
+A new round has to be initiated by one of the players every time the previous one ends (or at the beginning). A simple command line game, where you respond by enum names, can be implemented simply as in `examples/round_simulate.py`.
 
-```python
-# define a table with fixed players as before
-table = ...
-while table:
-    while table and not table.round:
-        table.publicIn(
-            table.players[0].id,
-            TablePublicInId.STARTROUND
-        )
-
-    player = table.round.current_player
-    inp = input(f"require input from {player.id}: ")
-
-    if inp in RoundPublicInId.__members__:
-        action, raise_by = RoundPublicInId.__members__[inp], 0
-    elif inp.startswith(RoundPublicInId.RAISE.name):
-        raise_by = int(inp.split()[1])
-        action = RoundPublicInId.RAISE
-    else:
-        continue
-
-    table.publicIn(player.id, action, raise_by=raise_by)
-```
-
-Note that you can define your own IO identifiers for a generalized game,
-as shown in one example [here](https://github.com/kuco23/pokerlib/blob/master/pokerlib/implementations/_table_with_choice_to_show_cards.py).
+The library is highly customizable, allowing you to override specific class methods such as `_showdown` that let you define the way that cards get shown (see `pokerlib/implementations/_no_muck_showdown_table.py`). The IO identifiers can also be extended or reduced and set either as `Table` or `Round` class attributes.
 
 ## Tests
 Basic tests for this library are included. You can test HandParser by running
 ```bash
 python tests/handparser_reactive.py
 ```
 initiate a poker round simulation with
```

### Comparing `pokerlib-2.1.1/pokerlib/_handparser.py` & `pokerlib-2.2.0/pokerlib/_handparser.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,14 +102,20 @@
         if self.handenum != other.handenum:
             return self.handenum < other.handenum
         for (s_val, _), (o_val, _) in zip(self.handfullcards,
                                           other.handfullcards):
             if s_val != o_val: return s_val < o_val
         return False
 
+    def __ge__(self, other):
+        return not self < other
+
+    def __le__(self, other):
+        return not other > self
+
     def __iadd__(self, cards):
         if len(cards) > 0:
             self._addCards(cards)
         return self
 
     def _addCards(self, cards):
         self._parsed = False
```

### Comparing `pokerlib-2.1.1/pokerlib/_player.py` & `pokerlib-2.2.0/pokerlib/_player.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
+from operator import add
+
 class Player:
 
     def __init__(self, table_id, _id, name, money):
         self.table_id = table_id
         self.id = _id
         self.name = name
         self.money = money
-
         self.cards = tuple()
         self.hand = None
+        self.group_kickers = None
         self.is_folded = False
         self.is_all_in = False
-
         self.stake = 0
         self.turn_stake = [0, 0, 0, 0]
-
         self.played_turn = False
 
     @property
     def is_active(self):
         return not (self.is_folded or self.is_all_in)
 
     def __repr__(self):
@@ -28,31 +28,46 @@
 
     def __eq__(self, other):
         return self.id == other.id
 
     def resetState(self):
         self.cards = tuple()
         self.hand = None
+        self.group_kickers = None
         self.is_folded = False
         self.is_all_in = False
         self.stake = 0
         self.turn_stake = [0, 0, 0, 0]
         self.played_turn = False
 
 
 class PlayerGroup(list):
 
     def __getitem__(self, i):
-        ret = super().__getitem__(i)
-        isl = isinstance(ret, list)
-        return type(self)(ret) if isl else ret
+        is_slice = isinstance(i, slice)
+        ret = super().__getitem__(i if is_slice else i % len(self))
+        return type(self)(ret) if is_slice else ret
 
     def __add__(self, other):
         return type(self)(super().__add__(other))
 
+    def countActivePlayers(self):
+        counter = 0
+        for player in self:
+            if player.is_active:
+                counter += 1
+        return counter
+
+    def countUnfoldedPlayers(self):
+        counter = 0
+        for player in self:
+            if not player.is_folded:
+                counter += 1
+        return counter
+
     def getPlayerById(self, _id):
         for player in self:
             if player.id == _id:
                 return player
 
     def previousActivePlayer(self, i):
         j = self.previousActiveIndex(i)
@@ -70,14 +85,26 @@
 
     def nextActiveIndex(self, i):
         n = len(self)
         rn = range(i + 1, i + n)
         for k in map(lambda j: j % n, rn):
             if self[k].is_active: return k
 
+    def nextUnfoldedIndex(self, i):
+        n = len(self)
+        rn = range(i + 1, i + n)
+        for k in map(lambda j: j % n, rn):
+            if not self[k].is_folded: return k
+
+    def previousUnfoldedIndex(self, i):
+        n = len(self)
+        rn = reversed(range(i + 1, i + n))
+        for k in map(lambda j: j % n, rn):
+            if not self[k].is_folded: return k
+
     def getActivePlayers(self):
         return type(self)(filter(
             lambda player: player.is_active,
             self
         ))
 
     def getNotFoldedPlayers(self):
@@ -94,14 +121,26 @@
 
     def winners(self):
         winner = max(self, key=lambda x: x.hand)
         return type(self)(
             [player for player in self if player.hand == winner.hand]
         )
 
+    def sortedByWinningAmountProspect(self):
+        return type(self)(add(
+            sorted(
+                [player for player in self if player.is_all_in],
+                key = lambda player: player.stake
+            ),
+            sorted(
+                [player for player in self if player.is_active],
+                key = lambda player: player.stake
+            )
+        ))
+
 
 class PlayerSeats(list):
 
     def __add__(self, other):
         copy = type(self)(super().__add__([]))
         for p in other:
             copy.append(p)
```

### Comparing `pokerlib-2.1.1/pokerlib/_round.py` & `pokerlib-2.2.0/pokerlib/_round.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from operator import add
 from math import inf
 from random import sample
 from collections import namedtuple, deque
 from abc import ABC
 
 from .enums import Rank, Suit, Turn, RoundPublicInId, RoundPrivateOutId, RoundPublicOutId
 from ._handparser import HandParser, HandParserGroup
@@ -39,57 +38,59 @@
     PublicOutId = RoundPublicOutId
     PrivateOutId = RoundPrivateOutId
     __deck = [[rank, suit] for suit in Suit for rank in Rank]
 
     def __init__(self, _id, players, button, small_blind, big_blind):
         self.id = _id
         self.finished = False
+        self.closed = False
 
         self.small_blind = small_blind
         self.big_blind = big_blind
 
         self.players = players
         self.button = button
-        self.current_index = button
+        self.current_index = button # it will move
 
         self.board = list()
         self.turn = None
 
         self._deck = self._deckIterator()
         self._turn_generator = self._turnGenerator()
+        self._muck_optioned_player_ids = []
 
-        self.publicOut(self.PublicOutId.NEWROUND)
-
-        for player in self.players:
-            player.resetState()
-            player.cards = (next(self._deck), next(self._deck))
-            player.hand = HandParser(list(player.cards))
-
-            self.privateOut(
-                player.id,
-                self.PrivateOutId.DEALTCARDS
-            )
-
-        next(self._turn_generator)
-        self._dealBlinds()
-        self._postActionStateUpdate()
+        self._startRound()
 
     def __repr__(self):
         return f'Round({self.players}, {self.board})'
 
     def __bool__(self):
-        return not self.finished
+        return not self.closed
 
     def __contains__(self, player):
         return player in self.players
 
     def __getitem__(self, _id):
         return self.players.getPlayerById(_id)
 
     @property
+    def starting_player_index(self):
+        return self.players.nextUnfoldedIndex(self.button)
+    @property
+    def last_aggressor_index(self):
+        return self.players.previousUnfoldedIndex(
+            self.current_index)
+    @property
+    def small_blind_player_index(self):
+        return self.button - 2 if len(self.players) > 2 else self.button - 1
+    @property
+    def big_blind_player_index(self):
+        return self.button - 1 if len(self.players) > 2 else self.button
+
+    @property
     def current_player(self):
         return self.players[self.current_index]
 
     @property
     def turn_stake(self):
         return max(map(
             lambda player: player.turn_stake[self.turn],
@@ -127,19 +128,15 @@
             self.publicOut(
                 self.PublicOutId.NEWTURN,
                 turn = turn
             )
 
             yield
 
-    def _shiftCurrentPlayer(self):
-        i = self.current_index
-        self.current_index = self.players.nextActiveIndex(i)
-
-    def _pots_balanced(self):
+    def _potsBalanced(self):
         active_pots = [
             player.turn_stake[self.turn]
             for player in self.players
             if player.is_active
         ] or [inf]
 
         all_in_max_pot = max([
@@ -169,60 +166,70 @@
             self.publicOut(
                 self.PublicOutId.PLAYERISALLIN,
                 player_id = player.id,
                 all_in_stake = all_in_stake
             )
             return all_in_stake
 
-    def _dealBlinds(self):
-        i = self.current_index
+    def _startRound(self):
+        self.publicOut(self.PublicOutId.NEWROUND)
+
+        for player in self.players:
+            player.resetState()
+            player.cards = (next(self._deck), next(self._deck))
+            player.hand = HandParser(list(player.cards))
+
+            self.privateOut(
+                player.id,
+                self.PrivateOutId.DEALTCARDS
+            )
 
-        previous_player = self.players.previousActivePlayer(i)
-        paid_amount = self._addToPot(previous_player, self.small_blind)
+        next(self._turn_generator)
+        self._dealSmallBlind()
+        self._dealBigBlind()
+        self._postActionStateUpdate()
+
+    def _dealSmallBlind(self):
+        small_blind_player = self.players[self.small_blind_player_index]
+        paid_amount = self._addToPot(small_blind_player, self.small_blind)
         self.publicOut(
             self.PublicOutId.SMALLBLIND,
-            player_id = previous_player.id,
+            player_id = small_blind_player.id,
             paid_amount = paid_amount
         )
 
-        paid_amount = self._addToPot(self.current_player, self.big_blind)
+    def _dealBigBlind(self):
+        big_blind_player = self.players[self.big_blind_player_index]
+        paid_amount = self._addToPot(big_blind_player, self.big_blind)
         self.publicOut(
             self.PublicOutId.BIGBLIND,
-            player_id = self.current_player.id,
+            player_id = big_blind_player.id,
             paid_amount = paid_amount
         )
 
     def _dealPrematureWinnings(self):
         winner, = self.players.getNotFoldedPlayers()
         won = sum(self.pot_size)
         winner.money += won
 
         self.publicOut(
             self.PublicOutId.DECLAREPREMATUREWINNER,
             player_id = winner.id,
             money_won = won,
         )
 
-    def _dealWinnings(self):
-        stake_sorted = type(self.players)(add(
-            sorted(
-                [player for player in self.players if player.is_all_in],
-                key = lambda player: player.stake
-            ),
-            sorted(
-                [player for player in self.players if player.is_active],
-                key = lambda player: player.stake
-            )
-        ))
+        self._muck_optioned_player_ids.append(winner.id)
 
-        for competitor in stake_sorted:
-            self.publicOut(
-                self.PublicOutId.PUBLICCARDSHOW,
-                player_id = competitor.id
-            )
+        self.publicOut(
+            self.PublicOutId.PLAYERCHOICEREQUIRED,
+            player_id = winner.id
+        )
+
+    def _dealWinnings(self):
+        stake_sorted = self.players.sortedByWinningAmountProspect()
 
         grouped_indexes = [0]
         for i in range(1, len(stake_sorted)):
             if stake_sorted[i - 1].stake < stake_sorted[i].stake:
                 grouped_indexes.append(i)
 
         for i in grouped_indexes:
@@ -249,52 +256,80 @@
 
                 for player, take in zip(self.players, take_from):
                     win_took += take
                     player.stake -= take
 
                 if round(win_took):
                     win_split.money += round(win_took)
+                    win_split.group_kickers = kickers
 
                     self.publicOut(
                         self.PublicOutId.DECLAREFINISHEDWINNER,
                         player_id = win_split.id,
-                        money_won = round(win_took),
-                        kickers = kickers
+                        money_won = round(win_took)
                     )
 
+        self._showdown()
+
+    def _showdown(self):
+        showdown_initiator_index = self.last_aggressor_index \
+            if self.turn_stake > 0 else self.starting_player_index
+        current_best_hand = self.players[showdown_initiator_index].hand
+        for i in range(len(self.players)):
+            player = self.players[showdown_initiator_index + i]
+            if player.is_folded: continue
+            if i == 0 or player.hand >= current_best_hand:
+                current_best_hand = player.hand
+                self.publicOut(
+                    self.PublicOutId.PUBLICCARDSHOW,
+                    player_id = player.id,
+                    cards = player.cards,
+                    kickers = player.group_kickers
+                )
+            else:
+                self._muck_optioned_player_ids.append(player.id)
+                self.publicOut(
+                    self.PublicOutId.PLAYERCHOICEREQUIRED,
+                    player_id = player.id,
+                )
+
+    def _shiftCurrentPlayer(self):
+        self.current_index = self.players.nextActiveIndex(
+            self.current_index)
+
     def _moveToNextPlayer(self):
         self._shiftCurrentPlayer()
         called = self.current_player.turn_stake[self.turn]
         self.publicOut(
             self.PublicOutId.PLAYERACTIONREQUIRED,
             player_id = self.current_player.id,
             to_call = self.turn_stake - called
         )
 
     def _postActionStateUpdate(self, is_update_after_forcefold=False):
-        active = len(self.players.getActivePlayers())
-        not_folded = len(self.players.getNotFoldedPlayers())
-        pots_balanced = self._pots_balanced()
+        active = self.players.countActivePlayers()
+        not_folded = self.players.countUnfoldedPlayers()
+        pots_balanced = self._potsBalanced()
 
         if not_folded == 0:
             return self._close()
 
         elif not_folded == 1:
             self._dealPrematureWinnings()
-            return self._close()
+            return self._finish()
 
         elif active <= 1 and pots_balanced:
             for _ in self._turn_generator: pass
             self._dealWinnings()
-            return self._close()
+            return self._finish()
 
         elif self.players.allPlayedTurn() and pots_balanced:
             if self.turn == Turn.RIVER:
                 self._dealWinnings()
-                return self._close()
+                return self._finish()
             else:
                 next(self._turn_generator)
                 self.current_index = self.button
                 return self._moveToNextPlayer()
 
         # this function can be called after a non-current-player's
         # hand is force-folded, in which case we don't want to move
@@ -339,35 +374,63 @@
         paid_amount = self._addToPot(cp, cp.money)
         self.publicOut(
             self.PublicOutId.PLAYERWENTALLIN,
             player_id = self.current_player.id,
             paid_amount = paid_amount
         )
 
+    def _show(self, player_id):
+        self._muck_optioned_player_ids.remove(player_id)
+        player = self.players.getPlayerById(player_id)
+        self.publicOut(
+            self.PublicOutId.PLAYERREVEALCARDS,
+            player_id = player_id,
+            cards = player.cards
+        )
+
+    def _muck(self, player_id):
+        self._muck_optioned_player_ids.remove(player_id)
+        self.publicOut(
+            self.PublicOutId.PLAYERMUCKCARDS,
+            player_id = player_id
+        )
+
     def _executeAction(self, action, raise_by):
         if action is self.PublicInId.FOLD:
             self._fold()
         elif action is self.PublicInId.CHECK:
             self._check()
         elif action is self.PublicInId.CALL:
             self._call()
         elif action is self.PublicInId.RAISE:
             self._raise(raise_by)
         elif action is self.PublicInId.ALLIN:
             self._allin()
 
+    def _executeChoice(self, choice, player_id):
+        if choice is self.PublicInId.SHOW:
+            self._show(player_id)
+        elif choice is self.PublicInId.MUCK:
+            self._muck(player_id)
+        if self._muck_optioned_player_ids == []:
+            self._close()
+
     def _processAction(self, action, raise_by=0):
         self._executeAction(action, raise_by)
         self.current_player.played_turn = True
         self._postActionStateUpdate()
 
-    def _close(self):
+    def _finish(self):
         self.finished = True
         self.publicOut(self.PublicOutId.ROUNDFINISHED)
 
+    def _close(self):
+        self.closed = True
+        self.publicOut(self.PublicOutId.ROUNDCLOSED)
+
     def publicIn(self, player_id, action, **kwargs):
         """Processes invalidated user input"""
         ...
 
     def privateOut(self, player_id, out_id, **kwargs):
         """Override player out implementation"""
         ...
@@ -383,29 +446,33 @@
 
     def __init__(self, *args):
         self.public_out_queue = deque([])
         self.private_out_queue = deque([])
         super().__init__(*args)
 
     def publicIn(self, player_id, action, raise_by=0):
-        # public in must come from current player
-        player = self.current_player
-        if player_id != player.id: return
-
-        to_call = self.turn_stake - player.turn_stake[self.turn]
-        if action is self.PublicInId.CHECK and to_call == 0:
-            self._processAction(self.PublicInId.CHECK)
-        elif action is self.PublicInId.RAISE:
-           if to_call < player.money:
-                self._processAction(self.PublicInId.RAISE, raise_by)
+        if action is self.PublicInId.SHOW or action is self.PublicInId.MUCK:
+            if player_id in self._muck_optioned_player_ids:
+                self._executeChoice(action, player_id)
         elif (
+            action is self.PublicInId.CHECK or
             action is self.PublicInId.CALL or
+            action is self.PublicInId.FOLD or
             action is self.PublicInId.ALLIN or
-            action is self.PublicInId.FOLD
-        ): self._processAction(action, raise_by)
+            action is self.PublicInId.RAISE
+        ):
+            player = self.current_player
+            if player_id != player.id: return
+            to_call = self.turn_stake - player.turn_stake[self.turn]
+            if action is self.PublicInId.CHECK and to_call == 0:
+                self._processAction(self.PublicInId.CHECK)
+            elif action is self.PublicInId.RAISE:
+                if to_call < player.money:
+                    self._processAction(self.PublicInId.RAISE, raise_by)
+            else: self._processAction(action, raise_by)
 
     def privateOut(self, player_id, out_id, **kwargs):
         """Player out implementation"""
         # A solution for interacting with an outside io
         kwargs.update(self.extendedPrivateOut(player_id, out_id, kwargs))
         out = self.PrivateOut(player_id, out_id, kwargs)
         self.private_out_queue.append(out)
```

### Comparing `pokerlib-2.1.1/pokerlib/_table.py` & `pokerlib-2.2.0/pokerlib/_table.py`

 * *Files identical despite different names*

### Comparing `pokerlib-2.1.1/pokerlib/enums.py` & `pokerlib-2.2.0/pokerlib/enums.py`

 * *Files 23% similar despite different names*

```diff
@@ -40,14 +40,16 @@
 
 class RoundPublicInId(IntEnum):
     FOLD = 0
     CHECK = 1
     CALL = 2
     RAISE = 3
     ALLIN = 4
+    SHOW = 5
+    MUCK = 6
 
 # codes sent from round to player
 class RoundPrivateOutId(IntEnum):
     DEALTCARDS = 0
 
 # codes sent from round to players
 class RoundPublicOutId(IntEnum):
@@ -57,19 +59,23 @@
     BIGBLIND = 3
     PLAYERCHECK = 4
     PLAYERCALL = 5
     PLAYERFOLD = 6
     PLAYERRAISE = 7
     PLAYERISALLIN = 8
     PLAYERWENTALLIN = 9
-    PLAYERACTIONREQUIRED = 10
-    PUBLICCARDSHOW = 11
-    DECLAREPREMATUREWINNER = 12
-    DECLAREFINISHEDWINNER = 13
-    ROUNDFINISHED = 14
+    PLAYERREVEALCARDS = 10
+    PLAYERMUCKCARDS = 11
+    PLAYERACTIONREQUIRED = 12
+    PLAYERCHOICEREQUIRED = 13
+    PUBLICCARDSHOW = 14
+    DECLAREPREMATUREWINNER = 15
+    DECLAREFINISHEDWINNER = 16
+    ROUNDFINISHED = 17
+    ROUNDCLOSED = 18
 
 class TablePublicInId(IntEnum):
     BUYIN = 0
     STARTROUND = 1
     LEAVETABLE = 2
 
 class TablePublicOutId(IntEnum):
```

### Comparing `pokerlib-2.1.1/pyproject.toml` & `pokerlib-2.2.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pokerlib"
-version = "2.1.1"
+version = "2.2.0"
 description = "Python poker library"
 repository = "https://github.com/kuco23/pokerlib/"
 authors = ["kuco23 <nseverkar@gmail.com>"]
 keywords = ['python', 'poker', 'library']
 readme = "README.md"
 classifiers=  [
     'Development Status :: 3 - Alpha',
```

### Comparing `pokerlib-2.1.1/setup.py` & `pokerlib-2.2.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,182 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pokerlib
+Version: 2.2.0
+Summary: Python poker library
+Home-page: https://github.com/kuco23/pokerlib/
+Keywords: python,poker,library
+Author: kuco23
+Author-email: nseverkar@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: Free For Home Use
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Build Tools
+Project-URL: Repository, https://github.com/kuco23/pokerlib/
+Description-Content-Type: text/markdown
 
-packages = \
-['pokerlib', 'pokerlib.implementations']
+# pokerlib
+[![PyPI version](https://badge.fury.io/py/pokerlib.svg)](https://pypi.org/project/pokerlib)
 
-package_data = \
-{'': ['*']}
+A lightweight Python poker library, focusing on simplifying a Texas hold'em poker game implementation, when its io is supplied. It includes modules that help with hand parsing and poker game continuation.
 
-setup_kwargs = {
-    'name': 'pokerlib',
-    'version': '2.1.1',
-    'description': 'Python poker library',
-    'long_description': '# pokerlib\n[![PyPI version](https://badge.fury.io/py/pokerlib.svg)](https://pypi.org/project/pokerlib)\n\nA lightweight Python poker library, focusing on simplifying a Texas hold\'em poker game implementation, when its io is supplied. It includes modules that help with hand parsing and poker game continuation.\n\nTo install, run\n```bash\npip install pokerlib\n```\n\n## Usage\nLibrary consists of a module for parsing cards, which can be used separately, and modules that aid in running a poker game.\n\n### HandParser\nThis module takes care of hand parsing. A hand usually consists of 2 dealt cards plus 5 on the board, and `HandParser` is heavily optimized to work with up to 7 cards (with more than 7 cards, this is no longer Texas hold\'em). A card is defined as a pair of two enums - Rank and Suit. All of the enums used are of `IntEnum` type, so you can also freely interchange them for integers. Below is an example of how to construct two different hands and then compare them.\n\n```python\nfrom pokerlib import HandParser\nfrom pokerib.enums import Rank, Suit\n\nhand1 = HandParser([\n    (Rank.KING, Suit.SPADE),\n    (Rank.ACE, Suit.SPADE)\n])\n\nhand2 = HandParser([\n    (Rank.NINE, Suit.SPADE),\n    (Rank.TWO, Suit.CLUB)\n])\n\nboard = [\n    (Rank.EIGHT, Suit.SPADE),\n    (Rank.TEN, Suit.SPADE),\n    (Rank.JACK, Suit.SPADE),\n    (Rank.QUEEN, Suit.SPADE),\n    (Rank.TWO, Suit.HEART)\n]\n\n# add new cards to each hand\nhand1 += board # add the board to hand1\nhand2 += board # add the board to hand2\n\nprint(hand1.handenum) # Hand.STRAIGHTFLUSH\nprint(hand2.handenum) # Hand.STRAIGHTFLUSH\nprint(hand1 > hand2) # True\n```\n\n> **note:**\n> In the previous version, each hand had to be parsed manually with `hand.parse()`, now calling any of the methods requiring the hand to be parsed, triggers parsing automatically. This only happens once, except if the cards in a given hand change. The only way cards in a hand should change is through the `__iadd__` method. If this method is called with hand already parsed, the hand is considered unparsed.\n\nIt is also possible to fetch hand\'s kickers.\n\n```python\nhand = HandParser([\n    (Rank.TWO, Suit.DIAMOND),\n    (Rank.ACE, Suit.CLUB),\n    (Rank.TWO, Suit.SPADE),\n    (Rank.THREE, Suit.DIAMOND),\n    (Rank.TEN, Suit.HEART),\n    (Rank.SIX, Suit.HEART),\n    (Rank.KING, Suit.CLUB)\n])\n\nprint(list(hand.kickercards))\n# [\n#   (<Rank.ACE: 12>, <Suit.CLUB: 1>),\n#   (<Rank.KING: 11>, <Suit.CLUB: 1>),\n#   (<Rank.TEN: 8>, <Suit.HEART: 3>)\n# ]\n```\nUsing HandParser, we can [estimate the probability](https://github.com/kuco23/pokerlib/blob/master/examples/winning_probability.py) of a given hand winning the game with given known cards on the table (as implemented in another python cli-app [here](https://github.com/cookpete/poker-odds)). We do this by repeatedly random-sampling hands, then averaging the wins. Mathematically, this process converges to the probability by the law of large numbers.\n\n\n### Poker Game\nA poker table can be established by providing its configuration.\nA poker table object responds to given input with appropriate output,\nwhich can be customized by overriding the two functions producing it.\n\n```python\nfrom pokerlib import Table, Player, PlayerSeats\n\n# table that prints outputs\nclass MyTable(Table):\n    def publicOut(self, out_id, **kwargs):\n        print(out_id, kwargs)\n    def privateOut(self, player_id, out_id, **kwargs):\n        print(out_id, kwargs)\n\n# define a new table\ntable = MyTable(\n    table_id = 0\n    seats = PlayerSeats([None] * 9)\n    buyin = 100\n    small_blind = 5\n    big_blind = 10\n)\n```\n\nWe could have seated players on the `seats` inside `MyTable` constructor,\nbut let\'s add them to the defined table.\n\n```python\nplayer1 = Player(\n    table_id = table.id,\n    _id = 1,\n    name = \'alice\',\n    money = table.buyin\n)\nplayer2 = Player(\n    table_id = table.id,\n    _id = 2,\n    name = \'bob\',\n    money = table.buyin\n)\n# seat player1 at the first seat\ntable += player1, 0\n# seat player2 at the first free seat\ntable += player2\n```\n\nCommunication with the `table` object is established through specified enums,\nwhich can be modified by overriding table\'s `publicIn` method.\nUsing enum IO identifiers, we can implement a poker game as shown below.\n\n```python\nfrom pokerlib.enums import RoundPublicInId, TablePublicInId\n\ntable.publicIn(player1.id, TablePublicInId.STARTROUND)\ntable.publicIn(player1.id, RoundPublicInId.CALL)\ntable.publicIn(player2.id, RoundPublicInId.CHECK)\ntable.publicIn(player1.id, RoundPublicInId.CHECK)\ntable.publicIn(player2.id, RoundPublicInId.RAISE, raise_by=50)\ntable.publicIn(player1.id, RoundPublicInId.CALL)\ntable.publicIn(player1.id, RoundPublicInId.CHECK)\ntable.publicIn(player2.id, RoundPublicInId.CHECK)\ntable.publicIn(player1.id, RoundPublicInId.ALLIN)\ntable.publicIn(player2.id, RoundPublicInId.CALL)\n```\n\nWrong inputs are mostly ignored, though they can produce a response, when it seems useful. As noted before, when providing input, the `table` object responds with output ids (e.g. `PLAYERACTIONREQUIRED`) along with additional data that depends on the output id. For all possible outputs, check `RoundPublicInId` and `TablePublicInId` enums.\n\nA new round has to be initiated by one of the players every time the previous one ends (or at the beginning). A simple command line game, where you respond by enum names, can be implemented as below (for working version check `tests/round_test.py`).\n\n```python\n# define a table with fixed players as before\ntable = ...\nwhile table:\n    while table and not table.round:\n        table.publicIn(\n            table.players[0].id,\n            TablePublicInId.STARTROUND\n        )\n\n    player = table.round.current_player\n    inp = input(f"require input from {player.id}: ")\n\n    if inp in RoundPublicInId.__members__:\n        action, raise_by = RoundPublicInId.__members__[inp], 0\n    elif inp.startswith(RoundPublicInId.RAISE.name):\n        raise_by = int(inp.split()[1])\n        action = RoundPublicInId.RAISE\n    else:\n        continue\n\n    table.publicIn(player.id, action, raise_by=raise_by)\n```\n\nNote that you can define your own IO identifiers for a generalized game,\nas shown in one example [here](https://github.com/kuco23/pokerlib/blob/master/pokerlib/implementations/_table_with_choice_to_show_cards.py).\n\n## Tests\nBasic tests for this library are included. You can test HandParser by running\n```bash\npython tests/handparser_reactive.py\n```\ninitiate a poker round simulation with\n```bash\npython tests/round_test.py <number_of_players>\n```\nwhich will run a poker game simulation with raw data getting printed to stdout. The HandParser functionality was also tested against another poker library [pokerface](https://github.com/AussieSeaweed/pokerface). You can run those tests with\n```bash\npython tests/handparser_against_pokerface.py\n```\n\n## License\nGNU General Public License v3.0\n',
-    'author': 'kuco23',
-    'author_email': 'nseverkar@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/kuco23/pokerlib/',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.10,<4.0',
-}
+To install, run
+```bash
+pip install pokerlib
+```
 
+## Usage
+Library consists of a module for parsing cards, which can be used separately, and modules that aid in running a poker game.
+
+### HandParser
+This module takes care of hand parsing. A hand usually consists of 2 dealt cards plus 5 on the board, and `HandParser` is heavily optimized to work with up to 7 cards (with more than 7 cards, this is no longer Texas hold'em). A card is defined as a pair of two enums - Rank and Suit. All of the enums used are of `IntEnum` type, so you can also freely interchange them for integers. Below is an example of how to construct two different hands and then compare them.
+
+```python
+from pokerlib import HandParser
+from pokerib.enums import Rank, Suit
+
+hand1 = HandParser([
+    (Rank.KING, Suit.SPADE),
+    (Rank.ACE, Suit.SPADE)
+])
+
+hand2 = HandParser([
+    (Rank.NINE, Suit.SPADE),
+    (Rank.TWO, Suit.CLUB)
+])
+
+board = [
+    (Rank.EIGHT, Suit.SPADE),
+    (Rank.TEN, Suit.SPADE),
+    (Rank.JACK, Suit.SPADE),
+    (Rank.QUEEN, Suit.SPADE),
+    (Rank.TWO, Suit.HEART)
+]
+
+# add new cards to each hand
+hand1 += board # add the board to hand1
+hand2 += board # add the board to hand2
+
+print(hand1.handenum) # Hand.STRAIGHTFLUSH
+print(hand2.handenum) # Hand.STRAIGHTFLUSH
+print(hand1 > hand2) # True
+```
+
+> **note:**
+> In the previous version, each hand had to be parsed manually with `hand.parse()`, now calling any of the methods requiring the hand to be parsed, triggers parsing automatically. This only happens once, except if the cards in a given hand change. The only way cards in a hand should change is through the `__iadd__` method. If this method is called with hand already parsed, the hand is considered unparsed.
+
+It is also possible to fetch hand's kickers.
+
+```python
+hand = HandParser([
+    (Rank.TWO, Suit.DIAMOND),
+    (Rank.ACE, Suit.CLUB),
+    (Rank.TWO, Suit.SPADE),
+    (Rank.THREE, Suit.DIAMOND),
+    (Rank.TEN, Suit.HEART),
+    (Rank.SIX, Suit.HEART),
+    (Rank.KING, Suit.CLUB)
+])
+
+print(list(hand.kickercards))
+# [
+#   (<Rank.ACE: 12>, <Suit.CLUB: 1>),
+#   (<Rank.KING: 11>, <Suit.CLUB: 1>),
+#   (<Rank.TEN: 8>, <Suit.HEART: 3>)
+# ]
+```
+Using HandParser, we can [estimate the probability](https://github.com/kuco23/pokerlib/blob/master/examples/winning_probability.py) of a given hand winning the game with given known cards on the table (as implemented in another python cli-app [here](https://github.com/cookpete/poker-odds)). We do this by repeatedly random-sampling hands, then averaging the wins. Mathematically, this process converges to the probability by the law of large numbers.
+
+
+### Poker Game
+A poker table can be established by providing its configuration.
+A poker table object responds to given input with appropriate output,
+which can be customized by overriding the two functions producing it.
+
+```python
+from pokerlib import Table, Player, PlayerSeats
+
+# table that prints outputs
+class MyTable(Table):
+    def publicOut(self, out_id, **kwargs):
+        print(out_id, kwargs)
+    def privateOut(self, player_id, out_id, **kwargs):
+        print(out_id, kwargs)
+
+# define a new table
+table = MyTable(
+    table_id = 0
+    seats = PlayerSeats([None] * 9)
+    buyin = 100
+    small_blind = 5
+    big_blind = 10
+)
+```
+
+We could have seated players on the `seats` inside `MyTable` constructor,
+but let's add them to the defined table.
+
+```python
+player1 = Player(
+    table_id = table.id,
+    _id = 1,
+    name = 'alice',
+    money = table.buyin
+)
+player2 = Player(
+    table_id = table.id,
+    _id = 2,
+    name = 'bob',
+    money = table.buyin
+)
+# seat player1 at the first seat
+table += player1, 0
+# seat player2 at the first free seat
+table += player2
+```
+
+Communication with the `table` object is established through specified enums,
+which can be modified by overriding table's `publicIn` method.
+Using enum IO identifiers, we can implement a poker game as shown below.
+
+```python
+from pokerlib.enums import RoundPublicInId, TablePublicInId
+
+table.publicIn(player1.id, TablePublicInId.STARTROUND)
+table.publicIn(player1.id, RoundPublicInId.CALL)
+table.publicIn(player2.id, RoundPublicInId.CHECK)
+table.publicIn(player1.id, RoundPublicInId.CHECK)
+table.publicIn(player2.id, RoundPublicInId.RAISE, raise_by=50)
+table.publicIn(player1.id, RoundPublicInId.CALL)
+table.publicIn(player1.id, RoundPublicInId.CHECK)
+table.publicIn(player2.id, RoundPublicInId.CHECK)
+table.publicIn(player1.id, RoundPublicInId.ALLIN)
+table.publicIn(player2.id, RoundPublicInId.CALL)
+```
+
+Wrong inputs are mostly ignored, though they can produce a response, when it seems useful. As noted before, when providing input, the `table` object responds with output ids (e.g. `PLAYERACTIONREQUIRED`) along with additional data that depends on the output id. For all possible outputs, check `RoundPublicInId` and `TablePublicInId` enums.
+
+A new round has to be initiated by one of the players every time the previous one ends (or at the beginning). A simple command line game, where you respond by enum names, can be implemented simply as in `examples/round_simulate.py`.
+
+The library is highly customizable, allowing you to override specific class methods such as `_showdown` that let you define the way that cards get shown (see `pokerlib/implementations/_no_muck_showdown_table.py`). The IO identifiers can also be extended or reduced and set either as `Table` or `Round` class attributes.
+
+## Tests
+Basic tests for this library are included. You can test HandParser by running
+```bash
+python tests/handparser_reactive.py
+```
+initiate a poker round simulation with
+```bash
+python tests/round_test.py <number_of_players>
+```
+which will run a poker game simulation with raw data getting printed to stdout. The HandParser functionality was also tested against another poker library [pokerface](https://github.com/AussieSeaweed/pokerface). You can run those tests with
+```bash
+python tests/handparser_against_pokerface.py
+```
+
+## License
+GNU General Public License v3.0
 
-setup(**setup_kwargs)
```


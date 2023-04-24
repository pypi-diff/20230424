# Comparing `tmp/re3py-0.35.tar.gz` & `tmp/re3py-0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/re3py-0.35.tar", last modified: Tue Dec 29 13:10:28 2020, max compression
+gzip compressed data, was "re3py-0.36.tar", last modified: Mon Apr 24 12:22:43 2023, max compression
```

## Comparing `re3py-0.35.tar` & `re3py-0.36.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 blazs     (1000) blazs     (1000)        0 2020-12-29 13:10:28.171814 re3py-0.35/
--rw-rw-r--   0 blazs     (1000) blazs     (1000)       54 2020-12-29 13:08:37.000000 re3py-0.35/MANIFEST.in
--rw-rw-r--   0 blazs     (1000) blazs     (1000)      283 2020-12-29 13:10:28.171814 re3py-0.35/PKG-INFO
--rw-rw-r--   0 blazs     (1000) blazs     (1000)     3334 2020-12-29 13:08:37.000000 re3py-0.35/README.md
-drwxrwxr-x   0 blazs     (1000) blazs     (1000)        0 2020-12-29 13:10:28.167814 re3py-0.35/re3py/
--rw-rw-r--   0 blazs     (1000) blazs     (1000)       22 2020-12-29 13:08:38.000000 re3py-0.35/re3py/__init__.py
-drwxrwxr-x   0 blazs     (1000) blazs     (1000)        0 2020-12-29 13:10:28.167814 re3py-0.35/re3py/data/
--rw-rw-r--   0 blazs     (1000) blazs     (1000)        0 2020-12-29 13:08:38.000000 re3py-0.35/re3py/data/__init__.py
--rw-rw-r--   0 blazs     (1000) blazs     (1000)    22681 2020-12-29 13:08:38.000000 re3py-0.35/re3py/data/data_and_statistics.py
--rw-rw-r--   0 blazs     (1000) blazs     (1000)    13734 2020-12-29 13:08:38.000000 re3py-0.35/re3py/data/relation.py
--rw-rw-r--   0 blazs     (1000) blazs     (1000)     9855 2020-12-29 13:08:38.000000 re3py-0.35/re3py/data/task_settings.py
-drwxrwxr-x   0 blazs     (1000) blazs     (1000)        0 2020-12-29 13:10:28.167814 re3py-0.35/re3py/eval/
--rw-rw-r--   0 blazs     (1000) blazs     (1000)        0 2020-12-29 13:08:38.000000 re3py-0.35/re3py/eval/__init__.py
--rw-rw-r--   0 blazs     (1000) blazs     (1000)     9272 2020-12-29 13:08:38.000000 re3py-0.35/re3py/eval/evaluation.py
-drwxrwxr-x   0 blazs     (1000) blazs     (1000)        0 2020-12-29 13:10:28.167814 re3py-0.35/re3py/learners/
--rw-rw-r--   0 blazs     (1000) blazs     (1000)        0 2020-12-29 13:08:38.000000 re3py-0.35/re3py/learners/__init__.py
--rw-rw-r--   0 blazs     (1000) blazs     (1000)    22271 2020-12-29 13:08:38.000000 re3py-0.35/re3py/learners/boosting.py
-drwxrwxr-x   0 blazs     (1000) blazs     (1000)        0 2020-12-29 13:10:28.171814 re3py-0.35/re3py/learners/core/
--rw-rw-r--   0 blazs     (1000) blazs     (1000)        0 2020-12-29 13:08:38.000000 re3py-0.35/re3py/learners/core/__init__.py
--rw-rw-r--   0 blazs     (1000) blazs     (1000)     6143 2020-12-29 13:08:38.000000 re3py-0.35/re3py/learners/core/aggregators.py
--rw-rw-r--   0 blazs     (1000) blazs     (1000)     4681 2020-12-29 13:08:38.000000 re3py-0.35/re3py/learners/core/communicate_with_java.py
--rw-rw-r--   0 blazs     (1000) blazs     (1000)     1341 2020-12-29 13:08:38.000000 re3py-0.35/re3py/learners/core/comparators.py
--rw-rw-r--   0 blazs     (1000) blazs     (1000)     2581 2020-12-29 13:08:38.000000 re3py-0.35/re3py/learners/core/heuristic.py
--rw-rw-r--   0 blazs     (1000) blazs     (1000)     9518 2020-12-29 13:08:38.000000 re3py-0.35/re3py/learners/core/tree_node_split.py
--rw-rw-r--   0 blazs     (1000) blazs     (1000)     1684 2020-12-29 13:08:38.000000 re3py-0.35/re3py/learners/core/variables.py
--rw-rw-r--   0 blazs     (1000) blazs     (1000)      803 2020-12-29 13:08:38.000000 re3py-0.35/re3py/learners/predictive_model.py
--rw-rw-r--   0 blazs     (1000) blazs     (1000)     3869 2020-12-29 13:08:38.000000 re3py-0.35/re3py/learners/random_forest.py
--rw-rw-r--   0 blazs     (1000) blazs     (1000)    63705 2020-12-29 13:08:38.000000 re3py-0.35/re3py/learners/tree.py
-drwxrwxr-x   0 blazs     (1000) blazs     (1000)        0 2020-12-29 13:10:28.171814 re3py-0.35/re3py/ranking/
--rw-rw-r--   0 blazs     (1000) blazs     (1000)        0 2020-12-29 13:08:38.000000 re3py-0.35/re3py/ranking/__init__.py
--rw-rw-r--   0 blazs     (1000) blazs     (1000)     8784 2020-12-29 13:08:38.000000 re3py-0.35/re3py/ranking/ensemble_ranking.py
-drwxrwxr-x   0 blazs     (1000) blazs     (1000)        0 2020-12-29 13:10:28.171814 re3py-0.35/re3py/utilities/
--rw-rw-r--   0 blazs     (1000) blazs     (1000)        0 2020-12-29 13:08:38.000000 re3py-0.35/re3py/utilities/__init__.py
--rw-rw-r--   0 blazs     (1000) blazs     (1000)     2770 2020-12-29 13:08:38.000000 re3py-0.35/re3py/utilities/cross_validation.py
--rw-rw-r--   0 blazs     (1000) blazs     (1000)       98 2020-12-29 13:08:38.000000 re3py-0.35/re3py/utilities/my_exceptions.py
--rw-rw-r--   0 blazs     (1000) blazs     (1000)       24 2020-12-29 13:08:38.000000 re3py-0.35/re3py/utilities/my_memo.py
--rw-rw-r--   0 blazs     (1000) blazs     (1000)     4264 2020-12-29 13:08:38.000000 re3py-0.35/re3py/utilities/my_utils.py
--rw-rw-r--   0 blazs     (1000) blazs     (1000)     3415 2020-12-29 13:08:38.000000 re3py-0.35/re3py/utilities/table_to_relations.py
--rw-rw-r--   0 blazs     (1000) blazs     (1000)    12929 2020-12-29 13:08:38.000000 re3py-0.35/re3py/utilities/user_defined_relation.py
-drwxrwxr-x   0 blazs     (1000) blazs     (1000)        0 2020-12-29 13:10:28.167814 re3py-0.35/re3py.egg-info/
--rw-rw-r--   0 blazs     (1000) blazs     (1000)      283 2020-12-29 13:10:27.000000 re3py-0.35/re3py.egg-info/PKG-INFO
--rw-rw-r--   0 blazs     (1000) blazs     (1000)     1080 2020-12-29 13:10:27.000000 re3py-0.35/re3py.egg-info/SOURCES.txt
--rw-rw-r--   0 blazs     (1000) blazs     (1000)        1 2020-12-29 13:10:27.000000 re3py-0.35/re3py.egg-info/dependency_links.txt
--rw-rw-r--   0 blazs     (1000) blazs     (1000)        1 2020-12-29 13:10:16.000000 re3py-0.35/re3py.egg-info/not-zip-safe
--rw-rw-r--   0 blazs     (1000) blazs     (1000)       32 2020-12-29 13:10:27.000000 re3py-0.35/re3py.egg-info/requires.txt
--rw-rw-r--   0 blazs     (1000) blazs     (1000)        6 2020-12-29 13:10:27.000000 re3py-0.35/re3py.egg-info/top_level.txt
--rw-rw-r--   0 blazs     (1000) blazs     (1000)       32 2020-12-29 13:08:38.000000 re3py-0.35/requirements.txt
--rw-rw-r--   0 blazs     (1000) blazs     (1000)       38 2020-12-29 13:10:28.171814 re3py-0.35/setup.cfg
--rw-rw-r--   0 blazs     (1000) blazs     (1000)      853 2020-12-29 13:10:08.000000 re3py-0.35/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:22:43.684624 re3py-0.36/
+-rw-rw-rw-   0        0        0       57 2023-04-20 15:32:14.000000 re3py-0.36/MANIFEST.in
+-rw-rw-rw-   0        0        0      253 2023-04-24 12:22:43.673617 re3py-0.36/PKG-INFO
+-rw-rw-rw-   0        0        0    11146 2023-04-20 17:18:58.000000 re3py-0.36/README.md
+drwxrwxrwx   0        0        0        0 2023-04-24 12:22:43.470617 re3py-0.36/re3py/
+-rw-rw-rw-   0        0        0       23 2023-04-20 15:32:15.000000 re3py-0.36/re3py/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:22:43.529621 re3py-0.36/re3py/data/
+-rw-rw-rw-   0        0        0        0 2023-04-20 15:32:15.000000 re3py-0.36/re3py/data/__init__.py
+-rw-rw-rw-   0        0        0    23324 2023-04-20 15:32:15.000000 re3py-0.36/re3py/data/data_and_statistics.py
+-rw-rw-rw-   0        0        0    14083 2023-04-20 15:32:15.000000 re3py-0.36/re3py/data/relation.py
+-rw-rw-rw-   0        0        0    10072 2023-04-20 15:32:15.000000 re3py-0.36/re3py/data/task_settings.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:22:43.543646 re3py-0.36/re3py/eval/
+-rw-rw-rw-   0        0        0        0 2023-04-20 15:32:15.000000 re3py-0.36/re3py/eval/__init__.py
+-rw-rw-rw-   0        0        0     9529 2023-04-20 15:32:15.000000 re3py-0.36/re3py/eval/evaluation.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:22:43.572618 re3py-0.36/re3py/learners/
+-rw-rw-rw-   0        0        0        0 2023-04-20 15:32:15.000000 re3py-0.36/re3py/learners/__init__.py
+-rw-rw-rw-   0        0        0    22817 2023-04-20 16:36:57.000000 re3py-0.36/re3py/learners/boosting.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:22:43.615627 re3py-0.36/re3py/learners/core/
+-rw-rw-rw-   0        0        0        0 2023-04-20 15:32:15.000000 re3py-0.36/re3py/learners/core/__init__.py
+-rw-rw-rw-   0        0        0     6379 2023-04-20 15:32:15.000000 re3py-0.36/re3py/learners/core/aggregators.py
+-rw-rw-rw-   0        0        0     4807 2023-04-20 15:32:15.000000 re3py-0.36/re3py/learners/core/communicate_with_java.py
+-rw-rw-rw-   0        0        0     1411 2023-04-20 15:32:15.000000 re3py-0.36/re3py/learners/core/comparators.py
+-rw-rw-rw-   0        0        0     2643 2023-04-20 15:32:15.000000 re3py-0.36/re3py/learners/core/heuristic.py
+-rw-rw-rw-   0        0        0     9730 2023-04-20 15:32:16.000000 re3py-0.36/re3py/learners/core/tree_node_split.py
+-rw-rw-rw-   0        0        0     1753 2023-04-20 15:32:16.000000 re3py-0.36/re3py/learners/core/variables.py
+-rw-rw-rw-   0        0        0      823 2023-04-20 16:37:20.000000 re3py-0.36/re3py/learners/predictive_model.py
+-rw-rw-rw-   0        0        0     3954 2023-04-20 16:36:57.000000 re3py-0.36/re3py/learners/random_forest.py
+-rw-rw-rw-   0        0        0    65176 2023-04-20 16:36:56.000000 re3py-0.36/re3py/learners/tree.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:22:43.624621 re3py-0.36/re3py/ranking/
+-rw-rw-rw-   0        0        0        0 2023-04-20 15:32:16.000000 re3py-0.36/re3py/ranking/__init__.py
+-rw-rw-rw-   0        0        0     8991 2023-04-20 16:40:42.000000 re3py-0.36/re3py/ranking/ensemble_ranking.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:22:43.668621 re3py-0.36/re3py/utilities/
+-rw-rw-rw-   0        0        0        0 2023-04-20 15:32:16.000000 re3py-0.36/re3py/utilities/__init__.py
+-rw-rw-rw-   0        0        0     2841 2023-04-20 16:29:23.000000 re3py-0.36/re3py/utilities/cross_validation.py
+-rw-rw-rw-   0        0        0      104 2023-04-20 15:32:16.000000 re3py-0.36/re3py/utilities/my_exceptions.py
+-rw-rw-rw-   0        0        0       25 2023-04-20 15:32:16.000000 re3py-0.36/re3py/utilities/my_memo.py
+-rw-rw-rw-   0        0        0     4423 2023-04-20 15:32:16.000000 re3py-0.36/re3py/utilities/my_utils.py
+-rw-rw-rw-   0        0        0     3509 2023-04-20 15:32:16.000000 re3py-0.36/re3py/utilities/table_to_relations.py
+-rw-rw-rw-   0        0        0    13198 2023-04-20 15:32:16.000000 re3py-0.36/re3py/utilities/user_defined_relation.py
+drwxrwxrwx   0        0        0        0 2023-04-24 12:22:43.506624 re3py-0.36/re3py.egg-info/
+-rw-rw-rw-   0        0        0      253 2023-04-24 12:22:43.000000 re3py-0.36/re3py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1080 2023-04-24 12:22:43.000000 re3py-0.36/re3py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 12:22:43.000000 re3py-0.36/re3py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-20 16:16:36.000000 re3py-0.36/re3py.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       37 2023-04-24 12:22:43.000000 re3py-0.36/re3py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-24 12:22:43.000000 re3py-0.36/re3py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 16:20:39.000000 re3py-0.36/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 12:22:43.684624 re3py-0.36/setup.cfg
+-rw-rw-rw-   0        0        0      879 2023-04-20 16:20:46.000000 re3py-0.36/setup.py
```

### Comparing `re3py-0.35/re3py/data/relation.py` & `re3py-0.36/re3py/data/relation.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,349 +1,349 @@
-from typing import Set, Tuple, List, Union
-import re
-from ..utilities.my_utils import *
-from ..learners.core.variables import Variable
-from ..utilities.my_exceptions import WrongValueException
-import numpy as np
-
-
-class Relation:
-    constant_nominal = "nominal"
-    constant_numeric = "numeric"
-    constant_multi_target = "multi_target["
-    relation_type_constant = [
-        constant_nominal, constant_numeric, constant_multi_target
-    ]
-    allowed_chars = "-.,+ A-Za-z0-9_\\[\\]"
-    # constant_type = "constant"
-    tuple_pattern = "{{}}\\(([{} ,]+)\\)".format(allowed_chars)
-    time_efficient_search_bound = 3
-
-    def __init__(self, name: str, related_objects: Union[Set[Tuple[str]],
-                                                         None],
-                 file: Union[str, None], types):
-        self.name = name
-        self.all_tuples = set()
-        self.types = types
-        self.different_values = [-1] * len(self.types)
-        self.arity = len(self.types)
-        self.all_tuples_by_subsets = {}
-        self.init_all_tuples_by_subsets()
-        self.file = file
-        p1 = related_objects is None
-        p2 = self.file is None
-        assert p1 + p2 == 1
-        if p1:
-            with open(file) as f:
-                for whole_line in f:
-                    line = whole_line[:whole_line.find("//")]  # comments
-                    if line:
-                        self.try_add_tuple(line)
-        else:
-            self.all_tuples = related_objects
-            # TODO: This does not update tuples by subsets?
-
-    def __repr__(self):
-        set_part = []
-        total_len = 0
-        for t in self.all_tuples:
-            if total_len > 30:
-                set_part.append("...")
-                break
-            set_part.append(str(t))
-            total_len += len(set_part[-1])
-        return "Relation({}, {{{}}})".format(self.name, ", ".join(set_part))
-
-    def __eq__(self, other):
-        return self.name == other.name  # and self.types == other.types and self.all_tuples == other.all_tuples
-
-    def should_use_tuples_by_subsets(self):
-        return 1 <= self.arity <= Relation.time_efficient_search_bound
-
-    def init_all_tuples_by_subsets(self):
-        if self.should_use_tuples_by_subsets():
-            pattern = "{{:0>{}b}}".format(self.arity)
-            subset_codes = [
-                pattern.format(i) for i in range(1, 2**self.arity - 1)
-            ]
-            for subset_code in subset_codes:
-                self.all_tuples_by_subsets[subset_code] = {}
-            for t in self.all_tuples:
-                self.try_add_one_to_tuples_by_subsets(t)
-
-    def try_add_tuple(self, line: str):
-        """
-        Converts 'r(x,y)' to (x, y) and adds it to all tuples.
-
-        :param line: a string of form <relation name>(obj1, obj2, ...)
-        """
-        related_list = parse_relation_arguments(line, self.name)
-        relation_tuple = tuple(
-            Relation.intelligent_parse(v_type, v_value)
-            for v_type, v_value in zip(self.types, related_list))
-        self.add_parsed_tuple(relation_tuple)
-
-    def add_parsed_tuple(self, t):
-        self.all_tuples.add(t)
-        if self.should_use_tuples_by_subsets():
-            self.try_add_one_to_tuples_by_subsets(t)
-
-    def try_add_one_to_tuples_by_subsets_old(self, relation_tuple):
-        pattern = "{{:0>{}b}}".format(self.arity)
-        subset_codes = [pattern.format(i) for i in range(1, 2**self.arity - 1)]
-        for subset_code in subset_codes:
-            subset_dict = self.all_tuples_by_subsets[subset_code]
-            key_part = []
-            value_part = []
-            for tuple_component, code_component in zip(relation_tuple,
-                                                       subset_code):
-                if code_component == "1":
-                    key_part.append(tuple_component)
-                else:
-                    value_part.append(tuple_component)
-            key_part = tuple(key_part)
-            value_part = tuple(value_part)
-            if key_part not in subset_dict:
-                subset_dict[key_part] = set()
-            subset_dict[key_part].add(value_part)
-
-    def try_add_one_to_tuples_by_subsets(self, relation_tuple):
-        pattern = "{{:0>{}b}}".format(self.arity)
-        subset_codes = [pattern.format(i) for i in range(1, 2**self.arity - 1)]
-        for subset_code in subset_codes:
-            subset_dict = self.all_tuples_by_subsets[subset_code]
-            key_part = []
-            # value_part = []
-            for tuple_component, code_component in zip(relation_tuple,
-                                                       subset_code):
-                if code_component == "1":
-                    key_part.append(tuple_component)
-                # else:
-                #     value_part.append(tuple_component)
-            key_part = tuple(key_part)
-            value_part = relation_tuple  # tuple(value_part)
-            if key_part not in subset_dict:
-                subset_dict[key_part] = []  # set()
-            # subset_dict[key_part].add(value_part)
-            subset_dict[key_part].append(value_part)
-
-    def get_all_old(self, variables: List[Variable],
-                    known_values: List[int]) -> List[Tuple[Variable]]:
-        """
-        :param variables: e.g., [X0(2.1), X1(?), X2('b')]
-        :param known_values: list of indices of the variables that have known value, e.g., [0, 2]
-        :return: list of tuples that satisfy the constraints, e.g., all triplets (x, y, z), for which
-          x == 2.1 and z = 'b'.
-        """
-        def check_ok(related):
-            for j in known_values:
-                if variables[j].get_value() != related[j]:
-                    return False
-            return True
-
-        def merge(known_part, unknown_part):
-            merged = [None] * len(subset_code)
-            i_known = 0
-            i_unknown = 0
-            for j in range(len(merged)):
-                if subset_code[j] == "1":
-                    merged[j] = known_part[i_known]
-                    i_known += 1
-                else:
-                    merged[j] = unknown_part[i_unknown]
-                    i_unknown += 1
-            return tuple(merged)
-
-        if not self.should_use_tuples_by_subsets():
-            return [t for t in self.all_tuples if check_ok(t)]
-        else:
-            key_part = tuple([variables[i].get_value() for i in known_values])
-            if len(known_values) == self.arity:
-                return [key_part] if key_part in self.all_tuples else []
-            elif len(known_values) == 0:
-                return list(self.all_tuples)
-            else:
-                subset_code = ["0"] * self.arity
-                for i in known_values:
-                    subset_code[i] = "1"
-                subset_code = "".join(subset_code)
-                subset_dict = self.all_tuples_by_subsets[subset_code]
-                if key_part in subset_dict:
-                    value_parts = subset_dict[key_part]
-                else:
-                    value_parts = set()
-                return [
-                    merge(key_part, value_part) for value_part in value_parts
-                ]
-
-    def get_all(self, variables: List[Variable],
-                known_values: List[int]) -> List[Tuple[Variable]]:
-        """
-        :param variables: e.g., [X0(2.1), X1(?), X2('b')]
-        :param known_values: list of indices of the variables that have known value, e.g., [0, 2]
-        :return: list of tuples that satisfy the constraints, e.g., all triplets (x, y, z), for which
-          x == 2.1 and z = 'b'.
-        """
-        def check_ok(related):
-            for j in known_values:
-                if variables[j].get_value() != related[j]:
-                    return False
-            return True
-
-        if not self.should_use_tuples_by_subsets():
-            return [t for t in self.all_tuples if check_ok(t)]
-        else:
-            key_part = tuple([variables[i].get_value() for i in known_values])
-            if len(known_values) == self.arity:
-                return [key_part] if key_part in self.all_tuples else []
-            elif len(known_values) == 0:
-                return list(self.all_tuples)
-            else:
-                subset_code = ["0"] * self.arity
-                for i in known_values:
-                    subset_code[i] = "1"
-                subset_code = "".join(subset_code)
-                subset_dict = self.all_tuples_by_subsets[subset_code]
-                if key_part in subset_dict:
-                    return subset_dict[key_part]
-                else:
-                    return []
-
-    def get_all_values(self, position):
-        return sorted({t[position] for t in self.all_tuples})
-
-    def get_nb_all_values(self, position):
-        if self.different_values[position] < 0:
-            self.different_values[position] = len(
-                self.get_all_values(position))
-        return self.different_values[position]
-
-    def get_name(self):
-        return self.name
-
-    def get_types(self):
-        return self.types
-
-    @staticmethod
-    def intelligent_parse(variable_type, variable_value):
-        if Relation.is_numeric_type(variable_type):
-            # constant numeric
-            return try_convert_to_number(variable_value)
-        elif Relation.is_nominal_type(variable_type):
-            # constant nominal
-            return variable_value
-        elif Relation.is_multi_target_type(variable_type):
-            # multi_target[some type]
-            type_of_targets = Relation.get_inner_type_of_multi_target(
-                variable_type)
-            if not (variable_value.startswith('[')
-                    and variable_value.endswith(']')):
-                raise WrongValueException(
-                    "Multi-target value {} wrongly specified!".format(
-                        variable_value))
-            target_values_string = intelligent_split(variable_value[1:-1])
-            target_values = [
-                Relation.intelligent_parse(type_of_targets, v)
-                for v in target_values_string
-            ]
-            if Relation.is_numeric_type(type_of_targets):
-                return np.array(target_values)
-        else:
-            # user-defined
-            return variable_value
-
-    @staticmethod
-    def is_constant_type(variable_type):
-        return Relation.is_nominal_type(variable_type) or Relation.is_numeric_type(variable_type) or\
-               Relation.is_multi_target_type(variable_type)
-
-    @staticmethod
-    def is_nominal_type(variable_type):
-        return variable_type.startswith(Relation.constant_nominal)
-
-    @staticmethod
-    def is_numeric_type(variable_type):
-        return variable_type.startswith(Relation.constant_numeric)
-
-    @staticmethod
-    def is_multi_target_type(variable_type):
-        return variable_type.startswith(Relation.constant_multi_target)
-
-    @staticmethod
-    def get_inner_type_of_multi_target(variable_type):
-        assert Relation.is_multi_target_type(variable_type)
-        i0, i1 = variable_type.find('['), variable_type.rfind(']')
-        if min(i0, i1) < 0:
-            raise WrongValueException(
-                "Multi-target type {} wrongly specified!".format(
-                    variable_type))
-        return variable_type[i0 + 1:i1].strip()
-
-    @staticmethod
-    def check_has_ok_types(relation_types):
-        for t in relation_types:
-            if t[0] == t[0].lower() and not Relation.is_constant_type(t):
-                message = "Type {} should either start with a capital letter, " \
-                          "or be of form <element><appendix>, where <element> is in {}."
-                raise WrongValueException(
-                    message.format(t, Relation.relation_type_constant))
-
-
-def parse_relation_arguments(line: str, relation_name: str):
-    assert line.startswith(relation_name)
-    tuple_pattern = Relation.tuple_pattern.format(relation_name)
-    try:
-        related_str = re.search(tuple_pattern, line).group(1).strip()
-    except AttributeError:
-        print("Relation {}: tuple {} does not match pattern {}".format(
-            relation_name, line, tuple_pattern))
-        raise
-    related_list = intelligent_split(related_str)
-    object_name = "^[{}]+$".format(Relation.allowed_chars)
-    for o in related_list:
-        if re.match(object_name, o) is None:
-            if o == "":
-                print("Empty string detected in {}".format(line))
-            else:
-                raise WrongValueException(
-                    "{} in {} contains forbidden characters or is empty.".
-                    format(o, related_str))
-    return related_list
-
-
-def intelligent_split(line):
-    inside_list = False
-    inside_quotation = False
-    elements = []
-    start = 0
-    for i, c in enumerate(line):
-        if c == '"':
-            if i > 0 and line[i - 1] == '\\':
-                pass  # escaped quotation
-            else:
-                inside_quotation = not inside_quotation
-        if inside_quotation:
-            continue
-        if c == '[':
-            inside_list = True
-        elif c == ']':
-            inside_list = False
-        elif c == ',' and not inside_list:
-            elements.append(line[start:i])
-            start = i + 1
-    elements.append(line[start:])
-    return [e.strip() for e in elements]
-
-
-def parse_relation_name(line):
-    name_pattern = "([{}]+)\\(".format(Relation.allowed_chars)
-    try:
-        return re.match(name_pattern, line).group(1)
-    except AttributeError:
-        print(f"Pattern {name_pattern} did not match {line}")
-        raise
-
-
-def parse_relation(line):
-    relation_name = parse_relation_name(line)
-    related_list = parse_relation_arguments(line, relation_name)
-    return relation_name, related_list
+from typing import Set, Tuple, List, Union
+import re
+from ..utilities.my_utils import *
+from ..learners.core.variables import Variable
+from ..utilities.my_exceptions import WrongValueException
+import numpy as np
+
+
+class Relation:
+    constant_nominal = "nominal"
+    constant_numeric = "numeric"
+    constant_multi_target = "multi_target["
+    relation_type_constant = [
+        constant_nominal, constant_numeric, constant_multi_target
+    ]
+    allowed_chars = "-.,+ A-Za-z0-9_\\[\\]"
+    # constant_type = "constant"
+    tuple_pattern = "{{}}\\(([{} ,]+)\\)".format(allowed_chars)
+    time_efficient_search_bound = 3
+
+    def __init__(self, name: str, related_objects: Union[Set[Tuple[str]],
+                                                         None],
+                 file: Union[str, None], types):
+        self.name = name
+        self.all_tuples = set()
+        self.types = types
+        self.different_values = [-1] * len(self.types)
+        self.arity = len(self.types)
+        self.all_tuples_by_subsets = {}
+        self.init_all_tuples_by_subsets()
+        self.file = file
+        p1 = related_objects is None
+        p2 = self.file is None
+        assert p1 + p2 == 1
+        if p1:
+            with open(file) as f:
+                for whole_line in f:
+                    line = whole_line[:whole_line.find("//")]  # comments
+                    if line:
+                        self.try_add_tuple(line)
+        else:
+            self.all_tuples = related_objects
+            # TODO: This does not update tuples by subsets?
+
+    def __repr__(self):
+        set_part = []
+        total_len = 0
+        for t in self.all_tuples:
+            if total_len > 30:
+                set_part.append("...")
+                break
+            set_part.append(str(t))
+            total_len += len(set_part[-1])
+        return "Relation({}, {{{}}})".format(self.name, ", ".join(set_part))
+
+    def __eq__(self, other):
+        return self.name == other.name  # and self.types == other.types and self.all_tuples == other.all_tuples
+
+    def should_use_tuples_by_subsets(self):
+        return 1 <= self.arity <= Relation.time_efficient_search_bound
+
+    def init_all_tuples_by_subsets(self):
+        if self.should_use_tuples_by_subsets():
+            pattern = "{{:0>{}b}}".format(self.arity)
+            subset_codes = [
+                pattern.format(i) for i in range(1, 2**self.arity - 1)
+            ]
+            for subset_code in subset_codes:
+                self.all_tuples_by_subsets[subset_code] = {}
+            for t in self.all_tuples:
+                self.try_add_one_to_tuples_by_subsets(t)
+
+    def try_add_tuple(self, line: str):
+        """
+        Converts 'r(x,y)' to (x, y) and adds it to all tuples.
+
+        :param line: a string of form <relation name>(obj1, obj2, ...)
+        """
+        related_list = parse_relation_arguments(line, self.name)
+        relation_tuple = tuple(
+            Relation.intelligent_parse(v_type, v_value)
+            for v_type, v_value in zip(self.types, related_list))
+        self.add_parsed_tuple(relation_tuple)
+
+    def add_parsed_tuple(self, t):
+        self.all_tuples.add(t)
+        if self.should_use_tuples_by_subsets():
+            self.try_add_one_to_tuples_by_subsets(t)
+
+    def try_add_one_to_tuples_by_subsets_old(self, relation_tuple):
+        pattern = "{{:0>{}b}}".format(self.arity)
+        subset_codes = [pattern.format(i) for i in range(1, 2**self.arity - 1)]
+        for subset_code in subset_codes:
+            subset_dict = self.all_tuples_by_subsets[subset_code]
+            key_part = []
+            value_part = []
+            for tuple_component, code_component in zip(relation_tuple,
+                                                       subset_code):
+                if code_component == "1":
+                    key_part.append(tuple_component)
+                else:
+                    value_part.append(tuple_component)
+            key_part = tuple(key_part)
+            value_part = tuple(value_part)
+            if key_part not in subset_dict:
+                subset_dict[key_part] = set()
+            subset_dict[key_part].add(value_part)
+
+    def try_add_one_to_tuples_by_subsets(self, relation_tuple):
+        pattern = "{{:0>{}b}}".format(self.arity)
+        subset_codes = [pattern.format(i) for i in range(1, 2**self.arity - 1)]
+        for subset_code in subset_codes:
+            subset_dict = self.all_tuples_by_subsets[subset_code]
+            key_part = []
+            # value_part = []
+            for tuple_component, code_component in zip(relation_tuple,
+                                                       subset_code):
+                if code_component == "1":
+                    key_part.append(tuple_component)
+                # else:
+                #     value_part.append(tuple_component)
+            key_part = tuple(key_part)
+            value_part = relation_tuple  # tuple(value_part)
+            if key_part not in subset_dict:
+                subset_dict[key_part] = []  # set()
+            # subset_dict[key_part].add(value_part)
+            subset_dict[key_part].append(value_part)
+
+    def get_all_old(self, variables: List[Variable],
+                    known_values: List[int]) -> List[Tuple[Variable]]:
+        """
+        :param variables: e.g., [X0(2.1), X1(?), X2('b')]
+        :param known_values: list of indices of the variables that have known value, e.g., [0, 2]
+        :return: list of tuples that satisfy the constraints, e.g., all triplets (x, y, z), for which
+          x == 2.1 and z = 'b'.
+        """
+        def check_ok(related):
+            for j in known_values:
+                if variables[j].get_value() != related[j]:
+                    return False
+            return True
+
+        def merge(known_part, unknown_part):
+            merged = [None] * len(subset_code)
+            i_known = 0
+            i_unknown = 0
+            for j in range(len(merged)):
+                if subset_code[j] == "1":
+                    merged[j] = known_part[i_known]
+                    i_known += 1
+                else:
+                    merged[j] = unknown_part[i_unknown]
+                    i_unknown += 1
+            return tuple(merged)
+
+        if not self.should_use_tuples_by_subsets():
+            return [t for t in self.all_tuples if check_ok(t)]
+        else:
+            key_part = tuple([variables[i].get_value() for i in known_values])
+            if len(known_values) == self.arity:
+                return [key_part] if key_part in self.all_tuples else []
+            elif len(known_values) == 0:
+                return list(self.all_tuples)
+            else:
+                subset_code = ["0"] * self.arity
+                for i in known_values:
+                    subset_code[i] = "1"
+                subset_code = "".join(subset_code)
+                subset_dict = self.all_tuples_by_subsets[subset_code]
+                if key_part in subset_dict:
+                    value_parts = subset_dict[key_part]
+                else:
+                    value_parts = set()
+                return [
+                    merge(key_part, value_part) for value_part in value_parts
+                ]
+
+    def get_all(self, variables: List[Variable],
+                known_values: List[int]) -> List[Tuple[Variable]]:
+        """
+        :param variables: e.g., [X0(2.1), X1(?), X2('b')]
+        :param known_values: list of indices of the variables that have known value, e.g., [0, 2]
+        :return: list of tuples that satisfy the constraints, e.g., all triplets (x, y, z), for which
+          x == 2.1 and z = 'b'.
+        """
+        def check_ok(related):
+            for j in known_values:
+                if variables[j].get_value() != related[j]:
+                    return False
+            return True
+
+        if not self.should_use_tuples_by_subsets():
+            return [t for t in self.all_tuples if check_ok(t)]
+        else:
+            key_part = tuple([variables[i].get_value() for i in known_values])
+            if len(known_values) == self.arity:
+                return [key_part] if key_part in self.all_tuples else []
+            elif len(known_values) == 0:
+                return list(self.all_tuples)
+            else:
+                subset_code = ["0"] * self.arity
+                for i in known_values:
+                    subset_code[i] = "1"
+                subset_code = "".join(subset_code)
+                subset_dict = self.all_tuples_by_subsets[subset_code]
+                if key_part in subset_dict:
+                    return subset_dict[key_part]
+                else:
+                    return []
+
+    def get_all_values(self, position):
+        return sorted({t[position] for t in self.all_tuples})
+
+    def get_nb_all_values(self, position):
+        if self.different_values[position] < 0:
+            self.different_values[position] = len(
+                self.get_all_values(position))
+        return self.different_values[position]
+
+    def get_name(self):
+        return self.name
+
+    def get_types(self):
+        return self.types
+
+    @staticmethod
+    def intelligent_parse(variable_type, variable_value):
+        if Relation.is_numeric_type(variable_type):
+            # constant numeric
+            return try_convert_to_number(variable_value)
+        elif Relation.is_nominal_type(variable_type):
+            # constant nominal
+            return variable_value
+        elif Relation.is_multi_target_type(variable_type):
+            # multi_target[some type]
+            type_of_targets = Relation.get_inner_type_of_multi_target(
+                variable_type)
+            if not (variable_value.startswith('[')
+                    and variable_value.endswith(']')):
+                raise WrongValueException(
+                    "Multi-target value {} wrongly specified!".format(
+                        variable_value))
+            target_values_string = intelligent_split(variable_value[1:-1])
+            target_values = [
+                Relation.intelligent_parse(type_of_targets, v)
+                for v in target_values_string
+            ]
+            if Relation.is_numeric_type(type_of_targets):
+                return np.array(target_values)
+        else:
+            # user-defined
+            return variable_value
+
+    @staticmethod
+    def is_constant_type(variable_type):
+        return Relation.is_nominal_type(variable_type) or Relation.is_numeric_type(variable_type) or\
+               Relation.is_multi_target_type(variable_type)
+
+    @staticmethod
+    def is_nominal_type(variable_type):
+        return variable_type.startswith(Relation.constant_nominal)
+
+    @staticmethod
+    def is_numeric_type(variable_type):
+        return variable_type.startswith(Relation.constant_numeric)
+
+    @staticmethod
+    def is_multi_target_type(variable_type):
+        return variable_type.startswith(Relation.constant_multi_target)
+
+    @staticmethod
+    def get_inner_type_of_multi_target(variable_type):
+        assert Relation.is_multi_target_type(variable_type)
+        i0, i1 = variable_type.find('['), variable_type.rfind(']')
+        if min(i0, i1) < 0:
+            raise WrongValueException(
+                "Multi-target type {} wrongly specified!".format(
+                    variable_type))
+        return variable_type[i0 + 1:i1].strip()
+
+    @staticmethod
+    def check_has_ok_types(relation_types):
+        for t in relation_types:
+            if t[0] == t[0].lower() and not Relation.is_constant_type(t):
+                message = "Type {} should either start with a capital letter, " \
+                          "or be of form <element><appendix>, where <element> is in {}."
+                raise WrongValueException(
+                    message.format(t, Relation.relation_type_constant))
+
+
+def parse_relation_arguments(line: str, relation_name: str):
+    assert line.startswith(relation_name)
+    tuple_pattern = Relation.tuple_pattern.format(relation_name)
+    try:
+        related_str = re.search(tuple_pattern, line).group(1).strip()
+    except AttributeError:
+        print("Relation {}: tuple {} does not match pattern {}".format(
+            relation_name, line, tuple_pattern))
+        raise
+    related_list = intelligent_split(related_str)
+    object_name = "^[{}]+$".format(Relation.allowed_chars)
+    for o in related_list:
+        if re.match(object_name, o) is None:
+            if o == "":
+                print("Empty string detected in {}".format(line))
+            else:
+                raise WrongValueException(
+                    "{} in {} contains forbidden characters or is empty.".
+                    format(o, related_str))
+    return related_list
+
+
+def intelligent_split(line):
+    inside_list = False
+    inside_quotation = False
+    elements = []
+    start = 0
+    for i, c in enumerate(line):
+        if c == '"':
+            if i > 0 and line[i - 1] == '\\':
+                pass  # escaped quotation
+            else:
+                inside_quotation = not inside_quotation
+        if inside_quotation:
+            continue
+        if c == '[':
+            inside_list = True
+        elif c == ']':
+            inside_list = False
+        elif c == ',' and not inside_list:
+            elements.append(line[start:i])
+            start = i + 1
+    elements.append(line[start:])
+    return [e.strip() for e in elements]
+
+
+def parse_relation_name(line):
+    name_pattern = "([{}]+)\\(".format(Relation.allowed_chars)
+    try:
+        return re.match(name_pattern, line).group(1)
+    except AttributeError:
+        print(f"Pattern {name_pattern} did not match {line}")
+        raise
+
+
+def parse_relation(line):
+    relation_name = parse_relation_name(line)
+    related_list = parse_relation_arguments(line, relation_name)
+    return relation_name, related_list
```

### Comparing `re3py-0.35/re3py/learners/boosting.py` & `re3py-0.36/re3py/learners/boosting.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,533 +1,533 @@
-from rrank.learners.tree import DecisionTree, create_constant_tree
-from learners.predictive_model import TreeEnsemble
-from learners.core.heuristic import *
-from math import exp, log
-from rrank.ranking.ensemble_ranking import EnsembleRanking
-from data.data_and_statistics import get_all_target_values
-
-
-class GradientBoostingTask:
-    heuristic = HeuristicVariance()
-
-    @staticmethod
-    def create_default_model(data: Dataset):
-        raise NotImplementedError("This should be implemented by a subclass.")
-
-    @staticmethod
-    def minus_partial_derivative(true_values, predictions):
-        raise NotImplementedError("This should be implemented by a subclass.")
-
-    @staticmethod
-    def modify_tree(shrinkage, step, optimize_step, tree: DecisionTree):
-        """
-        Boosting node statistics take care of the optimal predictions in the leaves, i.e.,
-        the optimal step is 1, thus predictions in the leaves of the tree are multiplied by
-        shrinkage if we optimize for step, and shrinkage * step otherwise.
-        :param shrinkage:
-        :param step:
-        :param optimize_step:
-        :param tree:
-        :return: None
-        """
-        if optimize_step:
-            step = 1.0
-        factor = shrinkage * step
-        if factor != 1.0:
-            for node in tree:
-                if node.is_leaf():
-                    current_prediction = node.get_stats().get_prediction()
-                    node.get_stats().set_prediction(current_prediction *
-                                                    factor)
-
-    @staticmethod
-    def is_classification():
-        return False
-
-    @staticmethod
-    def is_binary_classification():
-        return False
-
-    @staticmethod
-    def is_multiclass_classification():
-        return False
-
-    @staticmethod
-    def is_regression():
-        return False
-
-
-class GradientBoostingRegression(GradientBoostingTask):
-    @staticmethod
-    def create_default_model(data: Dataset):
-        return create_constant_tree(GradientBoostingTask.heuristic, data)
-
-    @staticmethod
-    def minus_partial_derivative(true_values, predictions):
-        return [t - p for t, p in zip(true_values, predictions)]
-
-    @staticmethod
-    def is_regression():
-        return True
-
-
-class GradientBoostingBinaryClassification(GradientBoostingTask):
-    @staticmethod
-    def create_default_model_friedman(data: Dataset):
-        """
-        The optimal initial value is log[(1 + average) / (1 - average)] / 2,
-        where the targets in the data are +-1.
-        :param data:
-        :return:
-        """
-        tree = create_constant_tree(GradientBoostingTask.heuristic, data)
-        regression_stats = NodeStatisticsRegression()
-        regression_stats.add_examples(data.get_target_data())
-        regression_stats.create_predictions()
-        average = regression_stats.get_prediction()
-        if abs(average - 1.0) < 10**-10:
-            prediction = float('inf')  # TODO: ?
-        elif abs(average + 1.0) < 10**-10:
-            prediction = float('-inf')  # TODO: ?
-        else:
-            prediction = log((1 + average) / (1 - average)) / 2
-        tree.root_node.get_stats().set_prediction(prediction)
-        return tree
-
-    @staticmethod
-    def create_default_model(data: Dataset):
-        return GradientBoostingRegression.create_default_model(data)
-
-    @staticmethod
-    def minus_partial_derivative_friedman(true_values, predictions):
-        ans = []
-        for t, p in zip(true_values, predictions):
-            try:
-                ans.append(2 * t / (1 + exp(2 * t * p)))
-            except OverflowError:
-                ans.append(t * 10**-10)  # t * float('inf')) TODO: ?
-        return ans
-
-    @staticmethod
-    def minus_partial_derivative(true_values, predictions):
-        return GradientBoostingRegression.minus_partial_derivative(
-            true_values, predictions)
-
-    @staticmethod
-    def is_classification():
-        return True
-
-    @staticmethod
-    def is_binary_classification():
-        return True
-
-
-class GradientBoostingMulticlassClassification(GradientBoostingTask):
-    @staticmethod
-    def create_default_model_friedman(data: Dataset):
-        """
-        Default model returns zero. We could leave it out, but technically it may be better to do this.
-        :param data:
-        :return:
-        """
-        tree = create_constant_tree(GradientBoostingTask.heuristic, data)
-        tree.root_node.get_stats().set_prediction(0.0)
-        return tree
-
-    @staticmethod
-    def create_default_model(data: Dataset):
-        return GradientBoostingRegression.create_default_model(data)
-
-    @staticmethod
-    def minus_partial_derivative_friedman(true_values, predictions):
-        examples = len(predictions[0])
-        classes = len(predictions)
-        predictions_exp = [[exp(p) for p in ps]
-                           for ps in predictions]  # TODO: numpy? :)
-        normalizers = [
-            sum(predictions_exp[k][i] for k in range(classes))
-            for i in range(examples)
-        ]
-        prob = [[
-            predictions_exp[k][i] / normalizers[i] for i in range(examples)
-        ] for k in range(classes)]
-        return [[true_values[k][i] - prob[k][i] for i in range(examples)]
-                for k in range(classes)]
-
-    @staticmethod
-    def minus_partial_derivative(true_values, predictions):
-        return [
-            GradientBoostingRegression.minus_partial_derivative(t, p)
-            for t, p in zip(true_values, predictions)
-        ]
-
-    @staticmethod
-    def is_classification():
-        return True
-
-    @staticmethod
-    def is_multiclass_classification():
-        return True
-
-
-class GradientBoosting(TreeEnsemble):
-    friedman = False
-    binary_classification = GradientBoostingBinaryClassification
-    multi_class_classification = GradientBoostingMulticlassClassification
-    regression = GradientBoostingRegression
-
-    def __init__(self,
-                 nb_trees_to_build=100,
-                 shrinkage=1.0,
-                 optimize_step_size=True,
-                 step_size=1.0,
-                 chosen_examples=1.0,
-                 random_seed=112,
-                 **tree_parameters):
-        self.nb_trees = nb_trees_to_build
-        self.shrinkage = shrinkage
-        self.optimize_step_size = optimize_step_size
-        self.step_sizes = self.compute_step_sizes(step_size)
-        self.chosen_examples = chosen_examples
-        self.ensemble_random = EnsembleRandomGenerator(random_seed)
-        self.tree_parameters = tree_parameters
-        self.task = None
-        self.alphas = 0
-        self.trees = []  # type: List[DecisionTree]
-        self.trees_per_class = []  # type: List[List[DecisionTree]]
-        self.class_dictionary = {}
-
-    def compute_step_sizes(self, step_size):
-        try:
-            return [s for s in step_size]
-        except TypeError:
-            return [step_size] * self.nb_trees
-
-    @staticmethod
-    def find_task(target_data: List[Datum]):
-        data_type = type(target_data[0].get_target())
-        if data_type == float or data_type == int:
-            return GradientBoosting.regression
-        elif data_type == str:
-            c = len(get_all_target_values(target_data))
-            if c == 2:
-                return GradientBoosting.binary_classification
-            elif c > 2:
-                return GradientBoosting.multi_class_classification
-            else:
-                raise WrongValueException(
-                    "Weird number of classes: {}".format(c))
-        else:
-            raise WrongValueException(
-                "Wrong target type: {}".format(data_type))
-
-    def build(self, input_data: Dataset):
-        # find task
-        self.task = GradientBoosting.find_task(input_data.get_target_data())
-        if self.task in [
-                GradientBoosting.binary_classification,
-                GradientBoosting.regression
-        ]:
-            self.build_helper1(input_data)
-        elif self.task in [GradientBoosting.multi_class_classification]:
-            self.build_helper2(input_data)
-
-    def build_helper1(self, input_data: Dataset):
-        # preprocess data
-        data, class_dictionary = self.preprocess(input_data)
-        true_values = [datum.get_target() for datum in data.get_target_data()]
-        self.class_dictionary = class_dictionary
-        # build default model
-        self.trees.append(self.task.create_default_model(data))
-        current_predictions = self.trees[-1].predict_all(
-            data.get_target_data())
-        # build boosted trees
-        for t in range(self.nb_trees):
-            ys = self.task.minus_partial_derivative(true_values,
-                                                    current_predictions)
-            modified_data = self.modify_dataset(data, ys)
-            print("Building tree {}".format(t + 1))
-            self.tree_parameters[
-                'random_seed'] = self.ensemble_random.next_tree_seed()
-            self.tree_parameters['heuristic'] = HeuristicVariance()
-            self.trees.append(DecisionTree(**self.tree_parameters))
-            self.trees[-1].build(modified_data)
-            self.task.modify_tree(self.shrinkage, self.step_sizes[t],
-                                  self.optimize_step_size, self.trees[-1])
-            GradientBoosting.update_current_predictions(
-                self.trees[-1], current_predictions, data.get_target_data())
-
-    def build_helper2(self, input_data: Dataset):
-        # preprocess data
-        datasets, class_dictionary = self.preprocess(input_data)
-        k = len(datasets)
-        true_values = [[
-            datum.get_target() for datum in data.get_target_data()
-        ] for data in datasets]
-        self.class_dictionary = class_dictionary
-        # build default model, for each class
-        self.trees_per_class.append([])
-        current_predictions = []
-        for i in range(k):
-            self.trees_per_class[-1].append(
-                self.task.create_default_model(datasets[i]))
-            current_predictions.append(self.trees_per_class[-1][i].predict_all(
-                datasets[i].get_target_data()))
-        # build boosted trees, for each class
-        for t in range(self.nb_trees):
-            ys = self.task.minus_partial_derivative(true_values,
-                                                    current_predictions)
-            modified_datasets = []
-            self.trees_per_class.append([])
-            for i in range(k):
-                modified_datasets.append(
-                    self.modify_dataset(datasets[i], ys[i]))
-                print("Building tree {} for class {}".format(t + 1, i + 1))
-                self.tree_parameters[
-                    'random_seed'] = self.ensemble_random.next_tree_seed()
-                self.tree_parameters['heuristic'] = HeuristicVariance()
-                self.trees_per_class[-1].append(
-                    DecisionTree(**self.tree_parameters))
-                self.trees_per_class[-1][i].build(modified_datasets[i])
-                self.task.modify_tree(self.shrinkage, self.step_sizes[t],
-                                      self.optimize_step_size,
-                                      self.trees_per_class[-1][i])
-                GradientBoosting.update_current_predictions(
-                    self.trees_per_class[-1][i], current_predictions[i],
-                    datasets[i].get_target_data())
-
-    @staticmethod
-    def update_current_predictions(tree, current_predictions,
-                                   data: List[Datum]):
-        for i, datum in enumerate(data):
-            current_predictions[i] += tree.predict(datum)
-
-    def preprocess(self, data: Dataset):
-        """
-        The statistics of the data are changed to boosting statistics.
-        For classification, targets are converted into numeric values.
-        :param data:
-        :return:
-        """
-        if self.task.is_binary_classification():
-            # convert the two target names into +-1 for friedman and 0/1 otherwise
-            dictionary = {}
-            for target_tuple in data:
-                t = target_tuple.get_target()
-                if t not in dictionary:
-                    value = len(
-                        dictionary
-                    ) * 2 - 1 if GradientBoosting.friedman else len(dictionary)
-                    dictionary[t] = value
-            assert len(dictionary) == 2
-            new_target_values = []  # type: List[Datum]
-            for datum in data:
-                new_target_values.append(
-                    Datum(datum.get_descriptive(),
-                          dictionary[datum.get_target()], datum.get_weight(),
-                          datum.identifier))
-            if GradientBoosting.friedman:
-                new_statistics = NodeStatisticsBinaryClassificationBoosting()
-            else:
-                new_statistics = NodeStatisticsRegressionBoosting()
-            new_statistics.add_examples(new_target_values)
-            return Dataset(settings=data.settings,
-                           data_file=data.data_file,
-                           descriptive_relations=data.get_descriptive_data(),
-                           target_data=new_target_values,
-                           statistics=new_statistics), {
-                               y: x
-                               for x, y in dictionary.items()
-                           }
-        elif self.task.is_multiclass_classification():
-            # convert to k datasets
-            dictionary = {}
-            for target_tuple in data:
-                t = target_tuple.get_target()
-                if t not in dictionary:
-                    value = len(dictionary)
-                    dictionary[t] = value
-            k = len(dictionary)
-            # assert k > 2
-            new_target_values = [[]
-                                 for _ in range(k)]  # type: List[List[Datum]]
-            for datum in data:
-                for i in range(k):
-                    new_target_values[i].append(
-                        Datum(datum.get_descriptive(), 0.0, datum.get_weight(),
-                              datum.identifier))
-            if GradientBoosting.friedman:
-                new_statistics = NodeStatisticsMulticlassClassificationBoosting(
-                    k)
-            else:
-                new_statistics = NodeStatisticsRegressionBoosting()
-            dataset_params = {
-                'settings': data.settings,
-                'descriptive_relations': data.get_descriptive_data(),
-                'statistics': new_statistics
-            }
-            datasets = []
-            for i in range(k):
-                dataset_params['target_data'] = new_target_values[i]
-                dataset_params['statistics'] = new_statistics.get_copy()
-                dataset_params['data_file'] = data.data_file
-                datasets.append(Dataset(**dataset_params))
-            for i, datum in enumerate(data):
-                non_zero = dictionary[datum.get_target()]
-                datasets[non_zero].get_target_data()[i].set_target(1.0)
-            for dataset in datasets:
-                dataset.statistics.add_examples(dataset.get_target_data())
-            return datasets, {y: x for x, y in dictionary.items()}
-        elif self.task.is_regression():
-            new_statistics = NodeStatisticsRegressionBoosting()
-            new_statistics.add_examples(data.get_target_data())
-            return Dataset(settings=data.settings,
-                           data_file=data.data_file,
-                           descriptive_relations=data.get_descriptive_data(),
-                           target_data=data.get_target_data(),
-                           statistics=new_statistics), None
-        else:
-            raise WrongValueException("Wrong task: {}".format(self.task))
-
-    def modify_dataset(self, data: Dataset, ys):
-        # update targets
-        new_target_data = []
-        for datum, y in zip(data.get_target_data(), ys):
-            new_datum = Datum(datum.get_descriptive(), y, datum.get_weight(),
-                              datum.identifier)
-            assert new_datum.get_weight() == 1
-            new_target_data.append(new_datum)
-        # subsample
-        if self.chosen_examples < 1.0:
-            n = len(new_target_data)
-            k = int(n * self.chosen_examples)
-            random.seed(self.ensemble_random.next_sample_rows_seed())
-            chosen_indices = random.sample(range(n), k=k)
-            new_target_data = [new_target_data[i] for i in chosen_indices]
-        return Dataset(settings=data.settings,
-                       data_file=data.data_file,
-                       descriptive_relations=data.get_descriptive_data(),
-                       target_data=new_target_data,
-                       statistics=data.get_copy_statistics())
-
-    def compute_ranking(self, ranking_type):
-        feature_ranking = EnsembleRanking({}, {}, ranking_type, self.nb_trees)
-        for i in range(self.nb_trees):
-            if self.task in [
-                    GradientBoosting.binary_classification,
-                    GradientBoosting.regression
-            ]:
-                trees = [self.trees[i + 1]]
-            elif self.task in [GradientBoosting.multi_class_classification]:
-                trees = self.trees_per_class[i + 1]
-            else:
-                raise WrongValueException("Unknown task: {}.".format(
-                    self.task))
-            scores = [
-                feature_ranking.compute_tree_contribution(tree)
-                for tree in trees
-            ]
-            average_scores = []
-            for j in range(2):
-                average_scores.append(
-                    average_of_dictionaries([pair[j] for pair in scores]))
-            feature_ranking.update_attributes(average_scores[0],
-                                              average_scores[1], i)
-        # We do not normalize the ranking ... feature_ranking.normalize()
-        return feature_ranking
-
-    def predict(self, d: Datum, nb_trees=None):
-        """
-        Predict the target values of datum d.
-        :param d:
-        :param nb_trees: Number of trees that are used for prediction. Maximal value is the value of the
-        argument nb_trees_to_build from the constructor. If set to 0, only default predictions are used.
-        :return: Prediction for datum d.
-        """
-        if nb_trees is None:
-            nb_trees = self.nb_trees + 1
-        else:
-            nb_trees += 1
-        if self.task in [
-                GradientBoosting.binary_classification,
-                GradientBoosting.regression
-        ]:
-            return self.predict_helper1(d, nb_trees)
-        elif self.task in [GradientBoosting.multi_class_classification]:
-            return self.predict_helper2(d, nb_trees)
-        else:
-            raise NotImplementedError(":D")
-
-    def predict_helper1(self, d: Datum, nb_trees):
-        predictions_stats = []  # type: List[NodeStatistics]
-        for tree in self.trees[:nb_trees]:
-            predictions_stats.append(tree.predict(d, True))
-        # statistics_class = predictions_stats[0].__class__
-        prediction = 0.0
-        for s in predictions_stats:
-            prediction += s.get_prediction()
-        if self.task == GradientBoosting.binary_classification:
-            numeric_classes = [-1, 1] if GradientBoosting.friedman else [0, 1]
-            original_classes = [
-                self.class_dictionary[n] for n in numeric_classes
-            ]
-            if GradientBoosting.friedman:
-                p_numeric_classes = []
-                for n in numeric_classes:
-                    try:
-                        p_numeric_classes.append(
-                            1 / (1 + exp(-2 * n * prediction)))
-                    except OverflowError:
-                        p_numeric_classes.append(0.0)
-            else:
-                p_numeric_classes = [1 - prediction, prediction]
-            return original_classes[arg_max(p_numeric_classes)]
-        elif self.task == GradientBoosting.regression:
-            return prediction
-        else:
-            return WrongValueException("Wrong task: {}".format(self.task))
-
-    def predict_helper2(self, d: Datum, nb_trees):
-        k = len(self.class_dictionary)
-        predictions_stats = []  # type: List[List[NodeStatistics]]
-        for tree_ind in range(nb_trees):
-            predictions_stats.append([])
-            for class_ind in range(k):
-                tree = self.trees_per_class[tree_ind][class_ind]
-                predictions_stats[-1].append(tree.predict(d, True))
-        prediction = [0.0 for _ in range(k)]
-        for s in predictions_stats:
-            for class_ind in range(k):
-                prediction[class_ind] += s[class_ind].get_prediction()
-        if self.task == GradientBoosting.multi_class_classification:
-            numeric_classes = list(range(k))
-            original_classes = [
-                self.class_dictionary[n] for n in numeric_classes
-            ]
-            if GradientBoosting.friedman:
-                # exp is monotonic, so we do not need it for arg max, but nevertheless ...
-                prediction = [exp(p) for p in prediction]
-            prediction_sum = sum(prediction)
-            p_numeric_classes = [p / prediction_sum for p in prediction]
-            return original_classes[arg_max(p_numeric_classes)]
-        else:
-            return WrongValueException("Wrong task: {}".format(self.task))
-
-    def print_model(self, file_name):
-        f = open(file_name, "w")
-        if self.class_dictionary:
-            print("Class encoding: {}".format(self.class_dictionary), file=f)
-        if self.task in [
-                GradientBoosting.binary_classification,
-                GradientBoosting.regression
-        ]:
-            for i, tree in enumerate(self.trees):
-                print("Tree {}:".format(i), file=f)
-                print(str(tree), file=f)
-                print("", file=f)
-        elif self.task in [GradientBoosting.multi_class_classification]:
-            for i, trees in enumerate(self.trees_per_class):
-                for c, tree in enumerate(trees):
-                    print("Tree {} for class {}:".format(i, c + 1), file=f)
-                    print(str(tree), file=f)
-                    print("", file=f)
-        f.close()
+from re3py.learners.tree import DecisionTree, create_constant_tree
+from re3py.learners.predictive_model import TreeEnsemble
+from re3py.learners.core.heuristic import *
+from math import exp, log
+from re3py.ranking.ensemble_ranking import EnsembleRanking
+from re3py.data.data_and_statistics import get_all_target_values
+
+
+class GradientBoostingTask:
+    heuristic = HeuristicVariance()
+
+    @staticmethod
+    def create_default_model(data: Dataset):
+        raise NotImplementedError("This should be implemented by a subclass.")
+
+    @staticmethod
+    def minus_partial_derivative(true_values, predictions):
+        raise NotImplementedError("This should be implemented by a subclass.")
+
+    @staticmethod
+    def modify_tree(shrinkage, step, optimize_step, tree: DecisionTree):
+        """
+        Boosting node statistics take care of the optimal predictions in the leaves, i.e.,
+        the optimal step is 1, thus predictions in the leaves of the tree are multiplied by
+        shrinkage if we optimize for step, and shrinkage * step otherwise.
+        :param shrinkage:
+        :param step:
+        :param optimize_step:
+        :param tree:
+        :return: None
+        """
+        if optimize_step:
+            step = 1.0
+        factor = shrinkage * step
+        if factor != 1.0:
+            for node in tree:
+                if node.is_leaf():
+                    current_prediction = node.get_stats().get_prediction()
+                    node.get_stats().set_prediction(current_prediction *
+                                                    factor)
+
+    @staticmethod
+    def is_classification():
+        return False
+
+    @staticmethod
+    def is_binary_classification():
+        return False
+
+    @staticmethod
+    def is_multiclass_classification():
+        return False
+
+    @staticmethod
+    def is_regression():
+        return False
+
+
+class GradientBoostingRegression(GradientBoostingTask):
+    @staticmethod
+    def create_default_model(data: Dataset):
+        return create_constant_tree(GradientBoostingTask.heuristic, data)
+
+    @staticmethod
+    def minus_partial_derivative(true_values, predictions):
+        return [t - p for t, p in zip(true_values, predictions)]
+
+    @staticmethod
+    def is_regression():
+        return True
+
+
+class GradientBoostingBinaryClassification(GradientBoostingTask):
+    @staticmethod
+    def create_default_model_friedman(data: Dataset):
+        """
+        The optimal initial value is log[(1 + average) / (1 - average)] / 2,
+        where the targets in the data are +-1.
+        :param data:
+        :return:
+        """
+        tree = create_constant_tree(GradientBoostingTask.heuristic, data)
+        regression_stats = NodeStatisticsRegression()
+        regression_stats.add_examples(data.get_target_data())
+        regression_stats.create_predictions()
+        average = regression_stats.get_prediction()
+        if abs(average - 1.0) < 10**-10:
+            prediction = float('inf')  # TODO: ?
+        elif abs(average + 1.0) < 10**-10:
+            prediction = float('-inf')  # TODO: ?
+        else:
+            prediction = log((1 + average) / (1 - average)) / 2
+        tree.root_node.get_stats().set_prediction(prediction)
+        return tree
+
+    @staticmethod
+    def create_default_model(data: Dataset):
+        return GradientBoostingRegression.create_default_model(data)
+
+    @staticmethod
+    def minus_partial_derivative_friedman(true_values, predictions):
+        ans = []
+        for t, p in zip(true_values, predictions):
+            try:
+                ans.append(2 * t / (1 + exp(2 * t * p)))
+            except OverflowError:
+                ans.append(t * 10**-10)  # t * float('inf')) TODO: ?
+        return ans
+
+    @staticmethod
+    def minus_partial_derivative(true_values, predictions):
+        return GradientBoostingRegression.minus_partial_derivative(
+            true_values, predictions)
+
+    @staticmethod
+    def is_classification():
+        return True
+
+    @staticmethod
+    def is_binary_classification():
+        return True
+
+
+class GradientBoostingMulticlassClassification(GradientBoostingTask):
+    @staticmethod
+    def create_default_model_friedman(data: Dataset):
+        """
+        Default model returns zero. We could leave it out, but technically it may be better to do this.
+        :param data:
+        :return:
+        """
+        tree = create_constant_tree(GradientBoostingTask.heuristic, data)
+        tree.root_node.get_stats().set_prediction(0.0)
+        return tree
+
+    @staticmethod
+    def create_default_model(data: Dataset):
+        return GradientBoostingRegression.create_default_model(data)
+
+    @staticmethod
+    def minus_partial_derivative_friedman(true_values, predictions):
+        examples = len(predictions[0])
+        classes = len(predictions)
+        predictions_exp = [[exp(p) for p in ps]
+                           for ps in predictions]  # TODO: numpy? :)
+        normalizers = [
+            sum(predictions_exp[k][i] for k in range(classes))
+            for i in range(examples)
+        ]
+        prob = [[
+            predictions_exp[k][i] / normalizers[i] for i in range(examples)
+        ] for k in range(classes)]
+        return [[true_values[k][i] - prob[k][i] for i in range(examples)]
+                for k in range(classes)]
+
+    @staticmethod
+    def minus_partial_derivative(true_values, predictions):
+        return [
+            GradientBoostingRegression.minus_partial_derivative(t, p)
+            for t, p in zip(true_values, predictions)
+        ]
+
+    @staticmethod
+    def is_classification():
+        return True
+
+    @staticmethod
+    def is_multiclass_classification():
+        return True
+
+
+class GradientBoosting(TreeEnsemble):
+    friedman = False
+    binary_classification = GradientBoostingBinaryClassification
+    multi_class_classification = GradientBoostingMulticlassClassification
+    regression = GradientBoostingRegression
+
+    def __init__(self,
+                 nb_trees_to_build=100,
+                 shrinkage=1.0,
+                 optimize_step_size=True,
+                 step_size=1.0,
+                 chosen_examples=1.0,
+                 random_seed=112,
+                 **tree_parameters):
+        self.nb_trees = nb_trees_to_build
+        self.shrinkage = shrinkage
+        self.optimize_step_size = optimize_step_size
+        self.step_sizes = self.compute_step_sizes(step_size)
+        self.chosen_examples = chosen_examples
+        self.ensemble_random = EnsembleRandomGenerator(random_seed)
+        self.tree_parameters = tree_parameters
+        self.task = None
+        self.alphas = 0
+        self.trees = []  # type: List[DecisionTree]
+        self.trees_per_class = []  # type: List[List[DecisionTree]]
+        self.class_dictionary = {}
+
+    def compute_step_sizes(self, step_size):
+        try:
+            return [s for s in step_size]
+        except TypeError:
+            return [step_size] * self.nb_trees
+
+    @staticmethod
+    def find_task(target_data: List[Datum]):
+        data_type = type(target_data[0].get_target())
+        if data_type == float or data_type == int:
+            return GradientBoosting.regression
+        elif data_type == str:
+            c = len(get_all_target_values(target_data))
+            if c == 2:
+                return GradientBoosting.binary_classification
+            elif c > 2:
+                return GradientBoosting.multi_class_classification
+            else:
+                raise WrongValueException(
+                    "Weird number of classes: {}".format(c))
+        else:
+            raise WrongValueException(
+                "Wrong target type: {}".format(data_type))
+
+    def fit(self, input_data: Dataset):
+        # find task
+        self.task = GradientBoosting.find_task(input_data.get_target_data())
+        if self.task in [
+                GradientBoosting.binary_classification,
+                GradientBoosting.regression
+        ]:
+            self.build_helper1(input_data)
+        elif self.task in [GradientBoosting.multi_class_classification]:
+            self.build_helper2(input_data)
+
+    def build_helper1(self, input_data: Dataset):
+        # preprocess data
+        data, class_dictionary = self.preprocess(input_data)
+        true_values = [datum.get_target() for datum in data.get_target_data()]
+        self.class_dictionary = class_dictionary
+        # build default model
+        self.trees.append(self.task.create_default_model(data))
+        current_predictions = self.trees[-1].predict_all(
+            data.get_target_data())
+        # build boosted trees
+        for t in range(self.nb_trees):
+            ys = self.task.minus_partial_derivative(true_values,
+                                                    current_predictions)
+            modified_data = self.modify_dataset(data, ys)
+            print("Building tree {}".format(t + 1))
+            self.tree_parameters[
+                'random_seed'] = self.ensemble_random.next_tree_seed()
+            self.tree_parameters['heuristic'] = HeuristicVariance()
+            self.trees.append(DecisionTree(**self.tree_parameters))
+            self.trees[-1].fit(modified_data)
+            self.task.modify_tree(self.shrinkage, self.step_sizes[t],
+                                  self.optimize_step_size, self.trees[-1])
+            GradientBoosting.update_current_predictions(
+                self.trees[-1], current_predictions, data.get_target_data())
+
+    def build_helper2(self, input_data: Dataset):
+        # preprocess data
+        datasets, class_dictionary = self.preprocess(input_data)
+        k = len(datasets)
+        true_values = [[
+            datum.get_target() for datum in data.get_target_data()
+        ] for data in datasets]
+        self.class_dictionary = class_dictionary
+        # build default model, for each class
+        self.trees_per_class.append([])
+        current_predictions = []
+        for i in range(k):
+            self.trees_per_class[-1].append(
+                self.task.create_default_model(datasets[i]))
+            current_predictions.append(self.trees_per_class[-1][i].predict_all(
+                datasets[i].get_target_data()))
+        # build boosted trees, for each class
+        for t in range(self.nb_trees):
+            ys = self.task.minus_partial_derivative(true_values,
+                                                    current_predictions)
+            modified_datasets = []
+            self.trees_per_class.append([])
+            for i in range(k):
+                modified_datasets.append(
+                    self.modify_dataset(datasets[i], ys[i]))
+                print("Building tree {} for class {}".format(t + 1, i + 1))
+                self.tree_parameters[
+                    'random_seed'] = self.ensemble_random.next_tree_seed()
+                self.tree_parameters['heuristic'] = HeuristicVariance()
+                self.trees_per_class[-1].append(
+                    DecisionTree(**self.tree_parameters))
+                self.trees_per_class[-1][i].fit(modified_datasets[i])
+                self.task.modify_tree(self.shrinkage, self.step_sizes[t],
+                                      self.optimize_step_size,
+                                      self.trees_per_class[-1][i])
+                GradientBoosting.update_current_predictions(
+                    self.trees_per_class[-1][i], current_predictions[i],
+                    datasets[i].get_target_data())
+
+    @staticmethod
+    def update_current_predictions(tree, current_predictions,
+                                   data: List[Datum]):
+        for i, datum in enumerate(data):
+            current_predictions[i] += tree.predict(datum)
+
+    def preprocess(self, data: Dataset):
+        """
+        The statistics of the data are changed to boosting statistics.
+        For classification, targets are converted into numeric values.
+        :param data:
+        :return:
+        """
+        if self.task.is_binary_classification():
+            # convert the two target names into +-1 for friedman and 0/1 otherwise
+            dictionary = {}
+            for target_tuple in data:
+                t = target_tuple.get_target()
+                if t not in dictionary:
+                    value = len(
+                        dictionary
+                    ) * 2 - 1 if GradientBoosting.friedman else len(dictionary)
+                    dictionary[t] = value
+            assert len(dictionary) == 2
+            new_target_values = []  # type: List[Datum]
+            for datum in data:
+                new_target_values.append(
+                    Datum(datum.get_descriptive(),
+                          dictionary[datum.get_target()], datum.get_weight(),
+                          datum.identifier))
+            if GradientBoosting.friedman:
+                new_statistics = NodeStatisticsBinaryClassificationBoosting()
+            else:
+                new_statistics = NodeStatisticsRegressionBoosting()
+            new_statistics.add_examples(new_target_values)
+            return Dataset(settings=data.settings,
+                           data_file=data.data_file,
+                           descriptive_relations=data.get_descriptive_data(),
+                           target_data=new_target_values,
+                           statistics=new_statistics), {
+                               y: x
+                               for x, y in dictionary.items()
+                           }
+        elif self.task.is_multiclass_classification():
+            # convert to k datasets
+            dictionary = {}
+            for target_tuple in data:
+                t = target_tuple.get_target()
+                if t not in dictionary:
+                    value = len(dictionary)
+                    dictionary[t] = value
+            k = len(dictionary)
+            # assert k > 2
+            new_target_values = [[]
+                                 for _ in range(k)]  # type: List[List[Datum]]
+            for datum in data:
+                for i in range(k):
+                    new_target_values[i].append(
+                        Datum(datum.get_descriptive(), 0.0, datum.get_weight(),
+                              datum.identifier))
+            if GradientBoosting.friedman:
+                new_statistics = NodeStatisticsMulticlassClassificationBoosting(
+                    k)
+            else:
+                new_statistics = NodeStatisticsRegressionBoosting()
+            dataset_params = {
+                'settings': data.settings,
+                'descriptive_relations': data.get_descriptive_data(),
+                'statistics': new_statistics
+            }
+            datasets = []
+            for i in range(k):
+                dataset_params['target_data'] = new_target_values[i]
+                dataset_params['statistics'] = new_statistics.get_copy()
+                dataset_params['data_file'] = data.data_file
+                datasets.append(Dataset(**dataset_params))
+            for i, datum in enumerate(data):
+                non_zero = dictionary[datum.get_target()]
+                datasets[non_zero].get_target_data()[i].set_target(1.0)
+            for dataset in datasets:
+                dataset.statistics.add_examples(dataset.get_target_data())
+            return datasets, {y: x for x, y in dictionary.items()}
+        elif self.task.is_regression():
+            new_statistics = NodeStatisticsRegressionBoosting()
+            new_statistics.add_examples(data.get_target_data())
+            return Dataset(settings=data.settings,
+                           data_file=data.data_file,
+                           descriptive_relations=data.get_descriptive_data(),
+                           target_data=data.get_target_data(),
+                           statistics=new_statistics), None
+        else:
+            raise WrongValueException("Wrong task: {}".format(self.task))
+
+    def modify_dataset(self, data: Dataset, ys):
+        # update targets
+        new_target_data = []
+        for datum, y in zip(data.get_target_data(), ys):
+            new_datum = Datum(datum.get_descriptive(), y, datum.get_weight(),
+                              datum.identifier)
+            assert new_datum.get_weight() == 1
+            new_target_data.append(new_datum)
+        # subsample
+        if self.chosen_examples < 1.0:
+            n = len(new_target_data)
+            k = int(n * self.chosen_examples)
+            random.seed(self.ensemble_random.next_sample_rows_seed())
+            chosen_indices = random.sample(range(n), k=k)
+            new_target_data = [new_target_data[i] for i in chosen_indices]
+        return Dataset(settings=data.settings,
+                       data_file=data.data_file,
+                       descriptive_relations=data.get_descriptive_data(),
+                       target_data=new_target_data,
+                       statistics=data.get_copy_statistics())
+
+    def compute_ranking(self, ranking_type):
+        feature_ranking = EnsembleRanking({}, {}, ranking_type, self.nb_trees)
+        for i in range(self.nb_trees):
+            if self.task in [
+                    GradientBoosting.binary_classification,
+                    GradientBoosting.regression
+            ]:
+                trees = [self.trees[i + 1]]
+            elif self.task in [GradientBoosting.multi_class_classification]:
+                trees = self.trees_per_class[i + 1]
+            else:
+                raise WrongValueException("Unknown task: {}.".format(
+                    self.task))
+            scores = [
+                feature_ranking.compute_tree_contribution(tree)
+                for tree in trees
+            ]
+            average_scores = []
+            for j in range(2):
+                average_scores.append(
+                    average_of_dictionaries([pair[j] for pair in scores]))
+            feature_ranking.update_attributes(average_scores[0],
+                                              average_scores[1], i)
+        # We do not normalize the ranking ... feature_ranking.normalize()
+        return feature_ranking
+
+    def predict(self, d: Datum, nb_trees=None):
+        """
+        Predict the target values of datum d.
+        :param d:
+        :param nb_trees: Number of trees that are used for prediction. Maximal value is the value of the
+        argument nb_trees_to_build from the constructor. If set to 0, only default predictions are used.
+        :return: Prediction for datum d.
+        """
+        if nb_trees is None:
+            nb_trees = self.nb_trees + 1
+        else:
+            nb_trees += 1
+        if self.task in [
+                GradientBoosting.binary_classification,
+                GradientBoosting.regression
+        ]:
+            return self.predict_helper1(d, nb_trees)
+        elif self.task in [GradientBoosting.multi_class_classification]:
+            return self.predict_helper2(d, nb_trees)
+        else:
+            raise NotImplementedError(":D")
+
+    def predict_helper1(self, d: Datum, nb_trees):
+        predictions_stats = []  # type: List[NodeStatistics]
+        for tree in self.trees[:nb_trees]:
+            predictions_stats.append(tree.predict(d, True))
+        # statistics_class = predictions_stats[0].__class__
+        prediction = 0.0
+        for s in predictions_stats:
+            prediction += s.get_prediction()
+        if self.task == GradientBoosting.binary_classification:
+            numeric_classes = [-1, 1] if GradientBoosting.friedman else [0, 1]
+            original_classes = [
+                self.class_dictionary[n] for n in numeric_classes
+            ]
+            if GradientBoosting.friedman:
+                p_numeric_classes = []
+                for n in numeric_classes:
+                    try:
+                        p_numeric_classes.append(
+                            1 / (1 + exp(-2 * n * prediction)))
+                    except OverflowError:
+                        p_numeric_classes.append(0.0)
+            else:
+                p_numeric_classes = [1 - prediction, prediction]
+            return original_classes[arg_max(p_numeric_classes)]
+        elif self.task == GradientBoosting.regression:
+            return prediction
+        else:
+            return WrongValueException("Wrong task: {}".format(self.task))
+
+    def predict_helper2(self, d: Datum, nb_trees):
+        k = len(self.class_dictionary)
+        predictions_stats = []  # type: List[List[NodeStatistics]]
+        for tree_ind in range(nb_trees):
+            predictions_stats.append([])
+            for class_ind in range(k):
+                tree = self.trees_per_class[tree_ind][class_ind]
+                predictions_stats[-1].append(tree.predict(d, True))
+        prediction = [0.0 for _ in range(k)]
+        for s in predictions_stats:
+            for class_ind in range(k):
+                prediction[class_ind] += s[class_ind].get_prediction()
+        if self.task == GradientBoosting.multi_class_classification:
+            numeric_classes = list(range(k))
+            original_classes = [
+                self.class_dictionary[n] for n in numeric_classes
+            ]
+            if GradientBoosting.friedman:
+                # exp is monotonic, so we do not need it for arg max, but nevertheless ...
+                prediction = [exp(p) for p in prediction]
+            prediction_sum = sum(prediction)
+            p_numeric_classes = [p / prediction_sum for p in prediction]
+            return original_classes[arg_max(p_numeric_classes)]
+        else:
+            return WrongValueException("Wrong task: {}".format(self.task))
+
+    def dump_to_text(self, file_name):
+        f = open(file_name, "w")
+        if self.class_dictionary:
+            print("Class encoding: {}".format(self.class_dictionary), file=f)
+        if self.task in [
+                GradientBoosting.binary_classification,
+                GradientBoosting.regression
+        ]:
+            for i, tree in enumerate(self.trees):
+                print("Tree {}:".format(i), file=f)
+                print(str(tree), file=f)
+                print("", file=f)
+        elif self.task in [GradientBoosting.multi_class_classification]:
+            for i, trees in enumerate(self.trees_per_class):
+                for c, tree in enumerate(trees):
+                    print("Tree {} for class {}:".format(i, c + 1), file=f)
+                    print(str(tree), file=f)
+                    print("", file=f)
+        f.close()
```

### Comparing `re3py-0.35/re3py/learners/core/aggregators.py` & `re3py-0.36/re3py/learners/core/aggregators.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,236 +1,236 @@
-from typing import List
-import statistics as st
-import itertools
-
-MODE_OF_EMPTY_LIST = "Nothing to see here"
-TYPE_NUMERIC = "numeric"
-TYPE_NOMINAL = "nominal"
-TYPE_TYPE = "type"
-TYPE_TUPLE = "tuple"
-TYPE_SAME_AS_INPUT = "as input"
-
-
-class Aggregator:
-    def __init__(self, name):
-        self.name = name
-        self.input_types = set()
-        self.output_type = None
-        self.is_projection = False
-
-    def __repr__(self):
-        return self.name
-
-    def get_name(self):
-        return self.name
-
-    def aggregate_flat(self, a_list):
-        raise NotImplementedError("Should be implemented by a subclass!")
-
-    def aggregate(self, ls):
-        return [self.aggregate_flat(a_list) for a_list in ls]
-
-    def __eq__(self, other):
-        return self.name == other.name
-
-    def __hash__(self):
-        return hash(self.name)
-
-    def __lt__(self, other):
-        return self.get_name() < other.get_name()
-
-
-class Count(Aggregator):
-    def __init__(self):
-        super().__init__("count")
-        self.input_types = {TYPE_NUMERIC, TYPE_NOMINAL, TYPE_TYPE, TYPE_TUPLE}
-        self.output_type = TYPE_NUMERIC
-
-    def aggregate_flat(self, a_list):
-        return len(a_list)
-
-
-class CountUnique(Aggregator):
-    def __init__(self):
-        super().__init__("countUnique")
-        self.input_types = {TYPE_NUMERIC, TYPE_NOMINAL, TYPE_TYPE,
-                            TYPE_TUPLE}  # Should numeric be removed?
-        self.output_type = TYPE_NUMERIC
-
-    def aggregate_flat(self, a_list):
-        return len(set(a_list))
-
-
-class Min(Aggregator):
-    def __init__(self):
-        super().__init__("min")
-        self.input_types = {TYPE_NUMERIC}
-        self.output_type = TYPE_NUMERIC
-
-    def aggregate_flat(self, a_list):
-        return min(a_list) if a_list else float("inf")
-
-
-class Max(Aggregator):
-    def __init__(self):
-        super().__init__("max")
-        self.input_types = {TYPE_NUMERIC}
-        self.output_type = TYPE_NUMERIC
-
-    def aggregate_flat(self, a_list):
-        return max(a_list) if a_list else float("-inf")
-
-
-class Mean(Aggregator):
-    def __init__(self):
-        super().__init__("mean")
-        self.input_types = {TYPE_NUMERIC}
-        self.output_type = TYPE_NUMERIC
-
-    def aggregate_flat(self, a_list):
-        return st.mean(a_list) if a_list else float(
-            "inf")  # slightly better than 0? None?
-
-
-class Sum(Aggregator):
-    def __init__(self):
-        super().__init__("sum")
-        self.input_types = {TYPE_NUMERIC}
-        self.output_type = TYPE_NUMERIC
-
-    def aggregate_flat(self, a_list):
-        return sum(a_list)
-
-
-class Mode(Aggregator):
-    def __init__(self):
-        super().__init__("mode")
-        self.input_types = {TYPE_NOMINAL, TYPE_TYPE}
-        self.output_type = TYPE_SAME_AS_INPUT
-
-    def aggregate_flat(self, a_list):
-        d = {}
-        for j in a_list:
-            if j not in d:
-                d[j] = 1
-            else:
-                d[j] += 1
-        if d:
-            return max(sorted(d),
-                       key=lambda t: d[t])  # Every time the same element
-        else:
-            return MODE_OF_EMPTY_LIST  # float("inf")
-
-
-class Flatten(Aggregator):
-    def __init__(self):
-        super().__init__("flatten")
-        self.input_types = {TYPE_NUMERIC, TYPE_NOMINAL, TYPE_TYPE}
-        self.output_type = TYPE_SAME_AS_INPUT
-
-    def aggregate(self, ls):
-        return list(itertools.chain.from_iterable(ls))
-
-    def aggregate_flat(self, a_list):
-        return a_list
-
-
-class FlattenUnique(Aggregator):
-    def __init__(self):
-        super().__init__("flattenUnique")
-        self.input_types = {TYPE_NUMERIC, TYPE_NOMINAL, TYPE_TYPE}
-        self.output_type = TYPE_SAME_AS_INPUT
-
-    def aggregate(self, ls):
-        return list(set(itertools.chain.from_iterable(ls)))
-
-    def aggregate_flat(self, a_list):
-        return a_list
-
-
-class Project(Aggregator):
-    def __init__(self, component, aggregator):
-        super().__init__("projection{}".format(component))
-        self.input_types = {TYPE_TUPLE}
-        self.output_type = "unknown"
-        self.is_projection = True
-        self.component = component
-        self.aggregator = aggregator
-        if self.aggregator is not None:
-            self.name += "_" + self.aggregator.name
-            self.output_type = self.aggregator.output_type
-
-    def aggregate_flat(self, a_list):
-        return self.aggregator.aggregate_flat(
-            [e[self.component] for e in a_list])
-
-
-class Project0(Project):
-    def __init__(self, aggregator):
-        super().__init__(0, aggregator)
-
-
-class Project1(Project):
-    def __init__(self, aggregator):
-        super().__init__(1, aggregator)
-
-
-class Project2(Project):
-    def __init__(self, aggregator):
-        super().__init__(2, aggregator)
-
-
-class Project3(Project):
-    def __init__(self, aggregator):
-        super().__init__(3, aggregator)
-
-
-class Project4(Project):
-    def __init__(self, aggregator):
-        super().__init__(4, aggregator)
-
-
-class Project5(Project):
-    def __init__(self, aggregator):
-        super().__init__(5, aggregator)
-
-
-class Project6(Project):
-    def __init__(self, aggregator):
-        super().__init__(6, aggregator)
-
-
-class Project7(Project):
-    def __init__(self, aggregator):
-        super().__init__(7, aggregator)
-
-
-FLATTEN = Flatten()
-FLATTEN_UNIQUE = FlattenUnique()
-COUNT = Count()
-COUNT_UNIQUE = CountUnique()
-MIN = Min()
-MAX = Max()
-MEAN = Mean()
-SUM = Sum()
-MODE = Mode()
-PROJECT = Project("", None)
-PROJECTIONS = [
-    Project0, Project1, Project2, Project3, Project4, Project5, Project6,
-    Project7
-]
-
-ALL_AGGREGATORS = [
-    FLATTEN, FLATTEN_UNIQUE, COUNT, COUNT_UNIQUE, MIN, MAX, MEAN, SUM, MODE,
-    PROJECT
-]  # type: List['Aggregator']
-NUMERIC_AGGREGATORS = [
-    a for a in ALL_AGGREGATORS if TYPE_NUMERIC in a.input_types
-]  # type: List['Aggregator']
-NOMINAL_AGGREGATORS = [
-    a for a in ALL_AGGREGATORS
-    if TYPE_NOMINAL in a.input_types and TYPE_TYPE in a.input_types
-]  # type: List['Aggregator']
-COMPLEX_ENOUGH_AGGREGATORS = [
-    a for a in ALL_AGGREGATORS if TYPE_TUPLE in a.input_types
-]
-CRITICAL_VALUES = [float("inf"), float("-inf"), MODE_OF_EMPTY_LIST]
+from typing import List
+import statistics as st
+import itertools
+
+MODE_OF_EMPTY_LIST = "Nothing to see here"
+TYPE_NUMERIC = "numeric"
+TYPE_NOMINAL = "nominal"
+TYPE_TYPE = "type"
+TYPE_TUPLE = "tuple"
+TYPE_SAME_AS_INPUT = "as input"
+
+
+class Aggregator:
+    def __init__(self, name):
+        self.name = name
+        self.input_types = set()
+        self.output_type = None
+        self.is_projection = False
+
+    def __repr__(self):
+        return self.name
+
+    def get_name(self):
+        return self.name
+
+    def aggregate_flat(self, a_list):
+        raise NotImplementedError("Should be implemented by a subclass!")
+
+    def aggregate(self, ls):
+        return [self.aggregate_flat(a_list) for a_list in ls]
+
+    def __eq__(self, other):
+        return self.name == other.name
+
+    def __hash__(self):
+        return hash(self.name)
+
+    def __lt__(self, other):
+        return self.get_name() < other.get_name()
+
+
+class Count(Aggregator):
+    def __init__(self):
+        super().__init__("count")
+        self.input_types = {TYPE_NUMERIC, TYPE_NOMINAL, TYPE_TYPE, TYPE_TUPLE}
+        self.output_type = TYPE_NUMERIC
+
+    def aggregate_flat(self, a_list):
+        return len(a_list)
+
+
+class CountUnique(Aggregator):
+    def __init__(self):
+        super().__init__("countUnique")
+        self.input_types = {TYPE_NUMERIC, TYPE_NOMINAL, TYPE_TYPE,
+                            TYPE_TUPLE}  # Should numeric be removed?
+        self.output_type = TYPE_NUMERIC
+
+    def aggregate_flat(self, a_list):
+        return len(set(a_list))
+
+
+class Min(Aggregator):
+    def __init__(self):
+        super().__init__("min")
+        self.input_types = {TYPE_NUMERIC}
+        self.output_type = TYPE_NUMERIC
+
+    def aggregate_flat(self, a_list):
+        return min(a_list) if a_list else float("inf")
+
+
+class Max(Aggregator):
+    def __init__(self):
+        super().__init__("max")
+        self.input_types = {TYPE_NUMERIC}
+        self.output_type = TYPE_NUMERIC
+
+    def aggregate_flat(self, a_list):
+        return max(a_list) if a_list else float("-inf")
+
+
+class Mean(Aggregator):
+    def __init__(self):
+        super().__init__("mean")
+        self.input_types = {TYPE_NUMERIC}
+        self.output_type = TYPE_NUMERIC
+
+    def aggregate_flat(self, a_list):
+        return st.mean(a_list) if a_list else float(
+            "inf")  # slightly better than 0? None?
+
+
+class Sum(Aggregator):
+    def __init__(self):
+        super().__init__("sum")
+        self.input_types = {TYPE_NUMERIC}
+        self.output_type = TYPE_NUMERIC
+
+    def aggregate_flat(self, a_list):
+        return sum(a_list)
+
+
+class Mode(Aggregator):
+    def __init__(self):
+        super().__init__("mode")
+        self.input_types = {TYPE_NOMINAL, TYPE_TYPE}
+        self.output_type = TYPE_SAME_AS_INPUT
+
+    def aggregate_flat(self, a_list):
+        d = {}
+        for j in a_list:
+            if j not in d:
+                d[j] = 1
+            else:
+                d[j] += 1
+        if d:
+            return max(sorted(d),
+                       key=lambda t: d[t])  # Every time the same element
+        else:
+            return MODE_OF_EMPTY_LIST  # float("inf")
+
+
+class Flatten(Aggregator):
+    def __init__(self):
+        super().__init__("flatten")
+        self.input_types = {TYPE_NUMERIC, TYPE_NOMINAL, TYPE_TYPE}
+        self.output_type = TYPE_SAME_AS_INPUT
+
+    def aggregate(self, ls):
+        return list(itertools.chain.from_iterable(ls))
+
+    def aggregate_flat(self, a_list):
+        return a_list
+
+
+class FlattenUnique(Aggregator):
+    def __init__(self):
+        super().__init__("flattenUnique")
+        self.input_types = {TYPE_NUMERIC, TYPE_NOMINAL, TYPE_TYPE}
+        self.output_type = TYPE_SAME_AS_INPUT
+
+    def aggregate(self, ls):
+        return list(set(itertools.chain.from_iterable(ls)))
+
+    def aggregate_flat(self, a_list):
+        return a_list
+
+
+class Project(Aggregator):
+    def __init__(self, component, aggregator):
+        super().__init__("projection{}".format(component))
+        self.input_types = {TYPE_TUPLE}
+        self.output_type = "unknown"
+        self.is_projection = True
+        self.component = component
+        self.aggregator = aggregator
+        if self.aggregator is not None:
+            self.name += "_" + self.aggregator.name
+            self.output_type = self.aggregator.output_type
+
+    def aggregate_flat(self, a_list):
+        return self.aggregator.aggregate_flat(
+            [e[self.component] for e in a_list])
+
+
+class Project0(Project):
+    def __init__(self, aggregator):
+        super().__init__(0, aggregator)
+
+
+class Project1(Project):
+    def __init__(self, aggregator):
+        super().__init__(1, aggregator)
+
+
+class Project2(Project):
+    def __init__(self, aggregator):
+        super().__init__(2, aggregator)
+
+
+class Project3(Project):
+    def __init__(self, aggregator):
+        super().__init__(3, aggregator)
+
+
+class Project4(Project):
+    def __init__(self, aggregator):
+        super().__init__(4, aggregator)
+
+
+class Project5(Project):
+    def __init__(self, aggregator):
+        super().__init__(5, aggregator)
+
+
+class Project6(Project):
+    def __init__(self, aggregator):
+        super().__init__(6, aggregator)
+
+
+class Project7(Project):
+    def __init__(self, aggregator):
+        super().__init__(7, aggregator)
+
+
+FLATTEN = Flatten()
+FLATTEN_UNIQUE = FlattenUnique()
+COUNT = Count()
+COUNT_UNIQUE = CountUnique()
+MIN = Min()
+MAX = Max()
+MEAN = Mean()
+SUM = Sum()
+MODE = Mode()
+PROJECT = Project("", None)
+PROJECTIONS = [
+    Project0, Project1, Project2, Project3, Project4, Project5, Project6,
+    Project7
+]
+
+ALL_AGGREGATORS = [
+    FLATTEN, FLATTEN_UNIQUE, COUNT, COUNT_UNIQUE, MIN, MAX, MEAN, SUM, MODE,
+    PROJECT
+]  # type: List['Aggregator']
+NUMERIC_AGGREGATORS = [
+    a for a in ALL_AGGREGATORS if TYPE_NUMERIC in a.input_types
+]  # type: List['Aggregator']
+NOMINAL_AGGREGATORS = [
+    a for a in ALL_AGGREGATORS
+    if TYPE_NOMINAL in a.input_types and TYPE_TYPE in a.input_types
+]  # type: List['Aggregator']
+COMPLEX_ENOUGH_AGGREGATORS = [
+    a for a in ALL_AGGREGATORS if TYPE_TUPLE in a.input_types
+]
+CRITICAL_VALUES = [float("inf"), float("-inf"), MODE_OF_EMPTY_LIST]
```

### Comparing `re3py-0.35/re3py/learners/core/communicate_with_java.py` & `re3py-0.36/re3py/learners/core/communicate_with_java.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-from ...data.data_and_statistics import Dataset, Datum
-from .variables import Variable
-# from relation import Relation
-from typing import Dict, List, Tuple, Union
-from py4j.java_collections import ListConverter, MapConverter
-from ...data.relation import Relation
-from .aggregators import Aggregator
-
-
-def send_data(data: Dataset, client, wrapper):
-    def l_convert(l0):
-        return list_converter.convert(l0, client)
-
-    def m_convert(m0):
-        return map_converter.convert(m0, client)
-
-    list_converter = ListConverter()
-    map_converter = MapConverter()
-
-    # send target_data: we can send only descriptive parts of the data
-    simplified_target = []
-    for d in data:
-        simplified_target.append([d.identifier])
-        simplified_target[-1] += list(d.get_descriptive())
-        simplified_target[-1] = l_convert(simplified_target[-1])
-    simplified_target = l_convert(simplified_target)
-    # target data
-    wrapper.load_target_data(simplified_target)
-    # relations
-    relations = {
-        r.name: l_convert(r.get_types())
-        for r in data.get_descriptive_data().values()
-    }
-    wrapper.load_relations(m_convert(relations), data.data_file)
-
-    # wrapper.load(l_convert([m_convert({2: "we", 3: "d"}), m_convert({"3": 2, "21": 21})]))
-
-
-def send_variables(example: Dict[str, Variable], client, wrapper):
-    def l_convert(l0):
-        return list_converter.convert(l0, client)
-
-    list_converter = ListConverter()
-
-    variables = []
-    for variable in example.values():
-        v_name = variable.get_name()
-        v_type = variable.value_type
-        v_value = variable.get_value()
-        v_can_vary = variable.can_vary()
-        variables.append(l_convert([v_name, v_type, v_value, v_can_vary]))
-    wrapper.load_variables(l_convert(variables))
-
-
-def compute_test_values(target_data: List[Datum],
-                        target_relation_vars: List[str],
-                        rc_modified: List[Tuple[Relation, List[str]]],
-                        filtered_agg_chains: List[List[Aggregator]],
-                        r_key: Tuple[Tuple[str, Tuple[bool],
-                                           Tuple[Union[str, int, Variable]]]],
-                        a_keys: List[Tuple[str]], nb_fresh_vars: int,
-                        fresh_indices: List[int],
-                        known_unknown: List[List[List[int]]], client, wrapper):
-    def l_convert(l0):
-        return list_converter.convert(l0, client)
-
-    # def m_convert(m0):
-    #     return map_converter.convert(m0, client)
-
-    list_converter = ListConverter()
-    # map_converter = MapConverter()
-
-    # set_example_values_time = 0
-    # find_values_time = 0
-
-    # conversion
-    target_data_converted = l_convert([d.identifier for d in target_data])
-
-    target_relation_vars_converted = l_convert(target_relation_vars)
-
-    rc_modified_converted = []
-    for r, variables in rc_modified:
-        rc_modified_converted.append(l_convert([r.get_name()] + variables))
-    rc_modified_converted = l_convert(rc_modified_converted)
-
-    filtered_agg_chains_converted = []
-    for aggregators in filtered_agg_chains:
-        filtered_agg_chains_converted.append(
-            l_convert([a.get_name() for a in aggregators]))
-    filtered_agg_chains_converted = l_convert(filtered_agg_chains_converted)
-
-    if r_key is None:
-        r_key_converted = None
-    else:
-        r_key_converted = []
-        for name, booleans, variables in r_key:
-            n = len(booleans)
-            assert n == len(variables)
-            new_element = ["" for _ in range(1 + 2 * n)]
-            new_element[0] = name
-            for i in range(n):
-                new_element[1 + i] = str(booleans[i]).lower()
-                new_element[1 + n + i] = variables[i]
-            r_key_converted.append(l_convert(new_element))
-        r_key_converted = l_convert(r_key_converted)
-
-    a_keys_converted = []
-    for t in a_keys:
-        a_keys_converted.append(l_convert(list(t)))
-    a_keys_converted = l_convert(a_keys_converted)
-
-    fresh_indices_converted = l_convert(fresh_indices)
-
-    known_unknown_converted = []
-    for known, unknown in known_unknown:
-        known_unknown_converted.append(
-            l_convert([l_convert(known), l_convert(unknown)]))
-    known_unknown_converted = l_convert(known_unknown_converted)
-
-    values = wrapper.compute_test_values(
-        target_data_converted, target_relation_vars_converted,
-        rc_modified_converted, filtered_agg_chains_converted, r_key_converted,
-        a_keys_converted, nb_fresh_vars, fresh_indices_converted,
-        known_unknown_converted)
-    all_test_values = [[x for x in part] for part in values]
-    return all_test_values
+from ...data.data_and_statistics import Dataset, Datum
+from .variables import Variable
+# from relation import Relation
+from typing import Dict, List, Tuple, Union
+from py4j.java_collections import ListConverter, MapConverter
+from ...data.relation import Relation
+from .aggregators import Aggregator
+
+
+def send_data(data: Dataset, client, wrapper):
+    def l_convert(l0):
+        return list_converter.convert(l0, client)
+
+    def m_convert(m0):
+        return map_converter.convert(m0, client)
+
+    list_converter = ListConverter()
+    map_converter = MapConverter()
+
+    # send target_data: we can send only descriptive parts of the data
+    simplified_target = []
+    for d in data:
+        simplified_target.append([d.identifier])
+        simplified_target[-1] += list(d.get_descriptive())
+        simplified_target[-1] = l_convert(simplified_target[-1])
+    simplified_target = l_convert(simplified_target)
+    # target data
+    wrapper.load_target_data(simplified_target)
+    # relations
+    relations = {
+        r.name: l_convert(r.get_types())
+        for r in data.get_descriptive_data().values()
+    }
+    wrapper.load_relations(m_convert(relations), data.data_file)
+
+    # wrapper.load(l_convert([m_convert({2: "we", 3: "d"}), m_convert({"3": 2, "21": 21})]))
+
+
+def send_variables(example: Dict[str, Variable], client, wrapper):
+    def l_convert(l0):
+        return list_converter.convert(l0, client)
+
+    list_converter = ListConverter()
+
+    variables = []
+    for variable in example.values():
+        v_name = variable.get_name()
+        v_type = variable.value_type
+        v_value = variable.get_value()
+        v_can_vary = variable.can_vary()
+        variables.append(l_convert([v_name, v_type, v_value, v_can_vary]))
+    wrapper.load_variables(l_convert(variables))
+
+
+def compute_test_values(target_data: List[Datum],
+                        target_relation_vars: List[str],
+                        rc_modified: List[Tuple[Relation, List[str]]],
+                        filtered_agg_chains: List[List[Aggregator]],
+                        r_key: Tuple[Tuple[str, Tuple[bool],
+                                           Tuple[Union[str, int, Variable]]]],
+                        a_keys: List[Tuple[str]], nb_fresh_vars: int,
+                        fresh_indices: List[int],
+                        known_unknown: List[List[List[int]]], client, wrapper):
+    def l_convert(l0):
+        return list_converter.convert(l0, client)
+
+    # def m_convert(m0):
+    #     return map_converter.convert(m0, client)
+
+    list_converter = ListConverter()
+    # map_converter = MapConverter()
+
+    # set_example_values_time = 0
+    # find_values_time = 0
+
+    # conversion
+    target_data_converted = l_convert([d.identifier for d in target_data])
+
+    target_relation_vars_converted = l_convert(target_relation_vars)
+
+    rc_modified_converted = []
+    for r, variables in rc_modified:
+        rc_modified_converted.append(l_convert([r.get_name()] + variables))
+    rc_modified_converted = l_convert(rc_modified_converted)
+
+    filtered_agg_chains_converted = []
+    for aggregators in filtered_agg_chains:
+        filtered_agg_chains_converted.append(
+            l_convert([a.get_name() for a in aggregators]))
+    filtered_agg_chains_converted = l_convert(filtered_agg_chains_converted)
+
+    if r_key is None:
+        r_key_converted = None
+    else:
+        r_key_converted = []
+        for name, booleans, variables in r_key:
+            n = len(booleans)
+            assert n == len(variables)
+            new_element = ["" for _ in range(1 + 2 * n)]
+            new_element[0] = name
+            for i in range(n):
+                new_element[1 + i] = str(booleans[i]).lower()
+                new_element[1 + n + i] = variables[i]
+            r_key_converted.append(l_convert(new_element))
+        r_key_converted = l_convert(r_key_converted)
+
+    a_keys_converted = []
+    for t in a_keys:
+        a_keys_converted.append(l_convert(list(t)))
+    a_keys_converted = l_convert(a_keys_converted)
+
+    fresh_indices_converted = l_convert(fresh_indices)
+
+    known_unknown_converted = []
+    for known, unknown in known_unknown:
+        known_unknown_converted.append(
+            l_convert([l_convert(known), l_convert(unknown)]))
+    known_unknown_converted = l_convert(known_unknown_converted)
+
+    values = wrapper.compute_test_values(
+        target_data_converted, target_relation_vars_converted,
+        rc_modified_converted, filtered_agg_chains_converted, r_key_converted,
+        a_keys_converted, nb_fresh_vars, fresh_indices_converted,
+        known_unknown_converted)
+    all_test_values = [[x for x in part] for part in values]
+    return all_test_values
```

### Comparing `re3py-0.35/re3py/learners/core/comparators.py` & `re3py-0.36/re3py/learners/core/comparators.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-class Comparator:
-    def __init__(self, name):
-        self.name = name
-
-    def compare(self, v1, v2):
-        raise NotImplementedError("This should be implemented by subclass")
-
-
-class IsSmaller(Comparator):
-    def __init__(self):
-        super().__init__("SMALLER")
-
-    def __repr__(self):
-        return "<"
-
-    def compare(self, v1, v2):
-        return v1 < v2
-
-
-class IsBigger(Comparator):
-    def __init__(self):
-        super().__init__("BIGGER")
-
-    def __repr__(self):
-        return ">"
-
-    def compare(self, v1, v2):
-        return v1 > v2
-
-
-class IsEqual(Comparator):
-    def __init__(self):
-        super().__init__("EQUAL")
-
-    def __repr__(self):
-        return "=="
-
-    def compare(self, v1, v2):
-        return v1 == v2
-
-
-class Contains(Comparator):
-    def __init__(self):
-        super().__init__("CONTAINS")
-
-    def __repr__(self):
-        return "in"
-
-    def compare(self, v1, v2):
-        return v1 in v2
-
-
-class DoesNotContain(Comparator):
-    def __init__(self):
-        super().__init__("CONTAINS_NOT")
-
-    def __repr__(self):
-        return "not in"
-
-    def compare(self, v1, v2):
-        return v1 not in v2
-
-
-SMALLER = IsSmaller()
-BIGGER = IsBigger()
-EQUAL = IsEqual()
-CONTAINS = Contains()
-DOES_NOT_CONTAIN = DoesNotContain()
-
-ALL_COMPARATORS = [SMALLER, BIGGER, EQUAL, CONTAINS, DOES_NOT_CONTAIN]
+class Comparator:
+    def __init__(self, name):
+        self.name = name
+
+    def compare(self, v1, v2):
+        raise NotImplementedError("This should be implemented by subclass")
+
+
+class IsSmaller(Comparator):
+    def __init__(self):
+        super().__init__("SMALLER")
+
+    def __repr__(self):
+        return "<"
+
+    def compare(self, v1, v2):
+        return v1 < v2
+
+
+class IsBigger(Comparator):
+    def __init__(self):
+        super().__init__("BIGGER")
+
+    def __repr__(self):
+        return ">"
+
+    def compare(self, v1, v2):
+        return v1 > v2
+
+
+class IsEqual(Comparator):
+    def __init__(self):
+        super().__init__("EQUAL")
+
+    def __repr__(self):
+        return "=="
+
+    def compare(self, v1, v2):
+        return v1 == v2
+
+
+class Contains(Comparator):
+    def __init__(self):
+        super().__init__("CONTAINS")
+
+    def __repr__(self):
+        return "in"
+
+    def compare(self, v1, v2):
+        return v1 in v2
+
+
+class DoesNotContain(Comparator):
+    def __init__(self):
+        super().__init__("CONTAINS_NOT")
+
+    def __repr__(self):
+        return "not in"
+
+    def compare(self, v1, v2):
+        return v1 not in v2
+
+
+SMALLER = IsSmaller()
+BIGGER = IsBigger()
+EQUAL = IsEqual()
+CONTAINS = Contains()
+DOES_NOT_CONTAIN = DoesNotContain()
+
+ALL_COMPARATORS = [SMALLER, BIGGER, EQUAL, CONTAINS, DOES_NOT_CONTAIN]
```

### Comparing `re3py-0.35/re3py/learners/core/heuristic.py` & `re3py-0.36/re3py/learners/core/heuristic.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-from ...data.data_and_statistics import *
-from typing import List
-import numpy as np
-
-class Heuristic:
-    def compute_variability(self, tree_node_stat):
-        raise NotImplementedError("This should be implemented by a subclass.")
-
-    def evaluate_split(self, parent_stats: NodeStatistics,
-                       children_stats: List[NodeStatistics]):
-        # TODO: make this efficient (h_parent is not necessary for arg max etc.)
-        examples_p = parent_stats.get_total_number_examples()
-        examples_cs = [c.get_total_number_examples() for c in children_stats]
-        branch_freq = [examples_c / examples_p for examples_c in examples_cs]
-        # h_p = self.compute_variability(parent_stats)
-        h_cs = [self.compute_variability(c) for c in children_stats]
-        # branch_freq = parent_stats.get_branch_frequencies()
-        # return h_p - sum(p * h_c for p, h_c in zip(branch_freq, h_cs))
-        return sum(p * h_c for p, h_c in zip(branch_freq, h_cs))
-
-
-class HeuristicGini(Heuristic):
-    def compute_variability(self,
-                            tree_node_stat: NodeStatisticsClassification):
-        return gini(tree_node_stat.get_per_class_probabilities())
-
-
-def gini(probabilities):
-    return 1 - sum(p**2 for p in probabilities)
-
-
-class HeuristicVariance(Heuristic):
-    def compute_variability(self, tree_node_stat: NodeStatisticsRegression):
-        """
-        Computes the estimate of the variance E[Y^2] - E[Y]^2.
-        Since the examples are weighted and can have small weights, we compute the biased estimate,
-        i.e., instead of ... / (n - 1), we return ... / n.
-        :param tree_node_stat:
-        :return:
-        """
-        n = tree_node_stat.get_total_number_examples(
-        )  # n > 0 when this is called
-        s1 = tree_node_stat.get_sum_of_values()
-        s2 = tree_node_stat.get_sum_of_squared_values()
-        return max(0, (s2 - s1**2 / n) / n)
-
-
-class HeuristicMultitargetVariance(Heuristic):
-    def compute_variability(
-            self, tree_node_stat: NodeStatisticsMultitargetRegression):
-        """
-        Computes the sum of estimates of the variance E[Y^2] - E[Y]^2, for each target variable.
-        Basically, the sum of HeuristicVariance.compute_variability ...
-        :param tree_node_stat:
-        :return:
-        """
-        n = tree_node_stat.get_total_number_examples(
-        )  # n > 0 when this is called
-        s1 = tree_node_stat.get_sum_of_values()[2:]
-        s2 = tree_node_stat.get_sum_of_squared_values()[2:]
-        v = np.mean(s2 - s1**2 / n) / n
-        return v if v > 0 else 0
+from ...data.data_and_statistics import *
+from typing import List
+import numpy as np
+
+class Heuristic:
+    def compute_variability(self, tree_node_stat):
+        raise NotImplementedError("This should be implemented by a subclass.")
+
+    def evaluate_split(self, parent_stats: NodeStatistics,
+                       children_stats: List[NodeStatistics]):
+        # TODO: make this efficient (h_parent is not necessary for arg max etc.)
+        examples_p = parent_stats.get_total_number_examples()
+        examples_cs = [c.get_total_number_examples() for c in children_stats]
+        branch_freq = [examples_c / examples_p for examples_c in examples_cs]
+        # h_p = self.compute_variability(parent_stats)
+        h_cs = [self.compute_variability(c) for c in children_stats]
+        # branch_freq = parent_stats.get_branch_frequencies()
+        # return h_p - sum(p * h_c for p, h_c in zip(branch_freq, h_cs))
+        return sum(p * h_c for p, h_c in zip(branch_freq, h_cs))
+
+
+class HeuristicGini(Heuristic):
+    def compute_variability(self,
+                            tree_node_stat: NodeStatisticsClassification):
+        return gini(tree_node_stat.get_per_class_probabilities())
+
+
+def gini(probabilities):
+    return 1 - sum(p**2 for p in probabilities)
+
+
+class HeuristicVariance(Heuristic):
+    def compute_variability(self, tree_node_stat: NodeStatisticsRegression):
+        """
+        Computes the estimate of the variance E[Y^2] - E[Y]^2.
+        Since the examples are weighted and can have small weights, we compute the biased estimate,
+        i.e., instead of ... / (n - 1), we return ... / n.
+        :param tree_node_stat:
+        :return:
+        """
+        n = tree_node_stat.get_total_number_examples(
+        )  # n > 0 when this is called
+        s1 = tree_node_stat.get_sum_of_values()
+        s2 = tree_node_stat.get_sum_of_squared_values()
+        return max(0, (s2 - s1**2 / n) / n)
+
+
+class HeuristicMultitargetVariance(Heuristic):
+    def compute_variability(
+            self, tree_node_stat: NodeStatisticsMultitargetRegression):
+        """
+        Computes the sum of estimates of the variance E[Y^2] - E[Y]^2, for each target variable.
+        Basically, the sum of HeuristicVariance.compute_variability ...
+        :param tree_node_stat:
+        :return:
+        """
+        n = tree_node_stat.get_total_number_examples(
+        )  # n > 0 when this is called
+        s1 = tree_node_stat.get_sum_of_values()[2:]
+        s2 = tree_node_stat.get_sum_of_squared_values()[2:]
+        v = np.mean(s2 - s1**2 / n) / n
+        return v if v > 0 else 0
```

### Comparing `re3py-0.35/re3py/learners/core/tree_node_split.py` & `re3py-0.36/re3py/learners/core/tree_node_split.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,212 +1,212 @@
-from typing import List, Tuple, Union, Dict, Set
-from ...data.relation import Relation
-from .comparators import Comparator
-from .variables import Variable
-from .aggregators import Aggregator, CRITICAL_VALUES
-
-# from my_exceptions import WrongValueException
-# from my_memo import used_comp_memo
-
-# tree node split memo
-TEST_VALUE_MEMO = {}
-
-
-class BinarySplit:
-    use_memo = True
-    worst_split_score = float('inf')
-
-    def __init__(self, atom_tests: List[Tuple[Relation, List[str],
-                                              Aggregator]],
-                 comparator: Union[Comparator,
-                                   None], threshold: Union[float, str,
-                                                           Set[str]],
-                 ignore_critical_values, is_variable_free):
-        self.test = atom_tests
-        self.comparator = comparator
-        self.threshold = threshold
-        self.ignore_critical_values = ignore_critical_values
-        self.fresh_variables = {}  # type: Dict[str, Variable]
-        self.is_variable_free = is_variable_free
-        self.used_for_relation_computation = False
-
-    def __str__(self, var_dict=None):
-        tests_str = []
-        for r, vs, a in self.test:
-            test_str = (r.get_name(), [None] * len(vs), a)
-            for i, v in enumerate(vs):
-                if var_dict is not None and not var_dict[v].is_unset():
-                    s = var_dict[v].get_value()
-                else:
-                    s = v
-                test_str[1][i] = s
-            tests_str.append(str(test_str))
-        if type(self.threshold) == set:
-            th_for_str = "{{{}}}".format(str(sorted(self.threshold))[1:-1])
-        else:
-            th_for_str = self.threshold
-        return "{} {} {}".format(", ".join(tests_str), self.comparator,
-                                 th_for_str)
-
-    def get_test(self):
-        return self.test
-
-    def get_fresh_variables(self):
-        return self.fresh_variables
-
-    def add_fresh_variables(self, vs):
-        for n, v in vs.items():
-            self.fresh_variables[n] = v
-
-    def evaluate_all(self, example: Dict[str, Variable],
-                     chain_relations: List[Tuple[Relation, List[str]]],
-                     chains_aggregators: List[Tuple[Aggregator]],
-                     comparators: List[Comparator],
-                     thresholds: List[Union[str, float]]):
-        values = self.get_test_values(example, chain_relations,
-                                      chains_aggregators, None, [], None, -1,
-                                      None, None)
-        return [
-            c.compare(v, t) for c, v, t in zip(comparators, values, thresholds)
-        ]
-
-    def evaluate(self, example: Dict[str, Variable]):
-        # example contains all name: variable pairs, maybe values of some is unknown
-        chain_relations = [(r, vs) for r, vs, _ in self.test]
-        chains_agg = [tuple([a for _, _, a in self.test])]
-        if self.is_variable_free:
-            compare_with = self.threshold
-        else:
-            compare_with = {example[v].value for v in self.threshold}
-        outcome = self.evaluate_all(example, chain_relations, chains_agg,
-                                    [self.comparator], [compare_with])
-        return outcome[0]
-
-    def get_test_values(self, example: Dict[str, Variable],
-                        chain_relations: List[Tuple[Relation, List[str]]],
-                        chains_aggregators: List[Tuple[Aggregator]],
-                        relation_key, aggregator_keys, tuple_id, nb_fresh_vars,
-                        fresh_indices, known_unknown):
-        n_as = len(chains_aggregators)
-        values = [None] * n_as
-        should_memo = BinarySplit.use_memo and relation_key is not None
-        d1 = None
-        if should_memo:
-            filtered_chains_aggregators = []
-            filtered_aggregator_keys = []
-            d0 = TEST_VALUE_MEMO[tuple_id]
-            for i, chain_aggregators in enumerate(chains_aggregators):
-                if relation_key in d0:
-                    d1 = d0[relation_key]
-                else:
-                    d1 = {}
-                    d0[relation_key] = d1
-                a_key = aggregator_keys[i]
-                if a_key in d1:
-                    values[i] = d1[a_key]
-                    # used_comp_memo[0] += 1
-                else:
-                    filtered_chains_aggregators.append(chain_aggregators)
-                    filtered_aggregator_keys.append(a_key)
-                    # used_comp_memo[1] += 1
-        else:
-            filtered_chains_aggregators = chains_aggregators
-            filtered_aggregator_keys = [None] * len(chains_aggregators)
-        if filtered_chains_aggregators:
-            values_partial_all = self.get_test_value_helper(
-                example, chain_relations, filtered_chains_aggregators,
-                nb_fresh_vars, fresh_indices, known_unknown)
-        else:
-            values_partial_all = []
-        where_to = 0
-        for agg_key, chain_aggregators, values_partial in zip(
-                filtered_aggregator_keys, filtered_chains_aggregators,
-                values_partial_all):
-            v = chain_aggregators[0].aggregate_flat(values_partial)
-            # assert v is not None
-            while values[where_to] is not None:
-                where_to += 1
-            values[where_to] = v
-            if should_memo:
-                d1[agg_key] = v
-        return values
-
-    def get_test_value_helper(self,
-                              example,
-                              chain_relations,
-                              chains_aggregators,
-                              nb_fresh_vars,
-                              fresh_indices,
-                              known_unknown_list,
-                              depth=1):
-        def results_generator(related_objects):
-            for r in related_objects:
-                # set
-                for i in unknown:
-                    rel_variables[i].set_value(r[i])
-                # compute
-                yield self.get_test_value_helper(example, chain_relations,
-                                                 chains_aggregators,
-                                                 nb_fresh_vars, fresh_indices,
-                                                 known_unknown_list, depth + 1)
-                # unset
-                for i in unknown:
-                    rel_variables[i].unset_value()
-
-        def should_keep_value(value):
-            return not (self.ignore_critical_values
-                        and value in CRITICAL_VALUES)
-
-        # for chain_aggregators in chains_aggregators:
-        #     assert len(chain_relations) == len(chain_aggregators)
-        relation, rel_variables_names = chain_relations[depth - 1]
-        rel_variables = [example[n] for n in rel_variables_names]
-        # aggregators = [chain[0] for chain in chains_aggregators]
-        if known_unknown_list is None:
-            known_unknown = [[], []]  # type: List[List[int]]
-            for i, v in enumerate(rel_variables_names):
-                known_unknown[example[v].is_unset()].append(i)
-        else:
-            known_unknown = known_unknown_list[depth - 1]
-        known, unknown = known_unknown
-        related = relation.get_all(rel_variables, known)
-        if len(chain_relations) == depth:
-            if nb_fresh_vars < 0:
-                fresh_indices = [
-                    i for i in unknown if rel_variables[i].can_vary()
-                ]
-                nb_fresh_vars = len(
-                    set(rel_variables[i].get_name() for i in fresh_indices))
-            if nb_fresh_vars == 0:
-                # everything known, more or less, this is only the proof of (non)existence
-                # There should be either 0 or 1 results, we pass their number.
-                # This can happen in the cases such as isFriend(x, Y), isFriend(Y, z),
-                # when Y has already a value after searching for the results isFriend(x, Y).
-                # hits = len(related)
-                # assert hits <= 1
-                to_aggregate = [len(related)]
-                # to_aggregate = related TODO: This more sense?
-            elif nb_fresh_vars == 1:
-                to_aggregate = [r[fresh_indices[0]]
-                                for r in related]  # flattened
-            else:
-                to_aggregate = related  # [[r[i] for i in fresh_indices] for r in related]
-                # if not all([aggregator in COMPLEX_ENOUGH_AGGREGATORS for aggregator in aggregators]):
-                #     raise WrongValueException("Your aggregators: {}. Allowed: {}".format(aggregators,
-                #                                                                          COMPLEX_ENOUGH_AGGREGATORS))
-            return [to_aggregate for _ in range(len(chains_aggregators))]
-        else:
-            next_aggregators = [chain[depth] for chain in chains_aggregators
-                                ]  # type: List[Aggregator]
-            to_aggregate = []
-            for res in results_generator(related):
-                to_aggregate.append(res)
-            answer = []
-            for a_ind, a in enumerate(next_aggregators):
-                ls = [neigh[a_ind] for neigh in to_aggregate]
-                out = [x for x in a.aggregate(ls) if should_keep_value(x)]
-                answer.append(out)
-            return answer
-
-    @staticmethod
-    def is_better_than_previous(new_score, previous_score):
-        return new_score < previous_score
+from typing import List, Tuple, Union, Dict, Set
+from ...data.relation import Relation
+from .comparators import Comparator
+from .variables import Variable
+from .aggregators import Aggregator, CRITICAL_VALUES
+
+# from my_exceptions import WrongValueException
+# from my_memo import used_comp_memo
+
+# tree node split memo
+TEST_VALUE_MEMO = {}
+
+
+class BinarySplit:
+    use_memo = True
+    worst_split_score = float('inf')
+
+    def __init__(self, atom_tests: List[Tuple[Relation, List[str],
+                                              Aggregator]],
+                 comparator: Union[Comparator,
+                                   None], threshold: Union[float, str,
+                                                           Set[str]],
+                 ignore_critical_values, is_variable_free):
+        self.test = atom_tests
+        self.comparator = comparator
+        self.threshold = threshold
+        self.ignore_critical_values = ignore_critical_values
+        self.fresh_variables = {}  # type: Dict[str, Variable]
+        self.is_variable_free = is_variable_free
+        self.used_for_relation_computation = False
+
+    def __str__(self, var_dict=None):
+        tests_str = []
+        for r, vs, a in self.test:
+            test_str = (r.get_name(), [None] * len(vs), a)
+            for i, v in enumerate(vs):
+                if var_dict is not None and not var_dict[v].is_unset():
+                    s = var_dict[v].get_value()
+                else:
+                    s = v
+                test_str[1][i] = s
+            tests_str.append(str(test_str))
+        if type(self.threshold) == set:
+            th_for_str = "{{{}}}".format(str(sorted(self.threshold))[1:-1])
+        else:
+            th_for_str = self.threshold
+        return "{} {} {}".format(", ".join(tests_str), self.comparator,
+                                 th_for_str)
+
+    def get_test(self):
+        return self.test
+
+    def get_fresh_variables(self):
+        return self.fresh_variables
+
+    def add_fresh_variables(self, vs):
+        for n, v in vs.items():
+            self.fresh_variables[n] = v
+
+    def evaluate_all(self, example: Dict[str, Variable],
+                     chain_relations: List[Tuple[Relation, List[str]]],
+                     chains_aggregators: List[Tuple[Aggregator]],
+                     comparators: List[Comparator],
+                     thresholds: List[Union[str, float]]):
+        values = self.get_test_values(example, chain_relations,
+                                      chains_aggregators, None, [], None, -1,
+                                      None, None)
+        return [
+            c.compare(v, t) for c, v, t in zip(comparators, values, thresholds)
+        ]
+
+    def evaluate(self, example: Dict[str, Variable]):
+        # example contains all name: variable pairs, maybe values of some is unknown
+        chain_relations = [(r, vs) for r, vs, _ in self.test]
+        chains_agg = [tuple([a for _, _, a in self.test])]
+        if self.is_variable_free:
+            compare_with = self.threshold
+        else:
+            compare_with = {example[v].value for v in self.threshold}
+        outcome = self.evaluate_all(example, chain_relations, chains_agg,
+                                    [self.comparator], [compare_with])
+        return outcome[0]
+
+    def get_test_values(self, example: Dict[str, Variable],
+                        chain_relations: List[Tuple[Relation, List[str]]],
+                        chains_aggregators: List[Tuple[Aggregator]],
+                        relation_key, aggregator_keys, tuple_id, nb_fresh_vars,
+                        fresh_indices, known_unknown):
+        n_as = len(chains_aggregators)
+        values = [None] * n_as
+        should_memo = BinarySplit.use_memo and relation_key is not None
+        d1 = None
+        if should_memo:
+            filtered_chains_aggregators = []
+            filtered_aggregator_keys = []
+            d0 = TEST_VALUE_MEMO[tuple_id]
+            for i, chain_aggregators in enumerate(chains_aggregators):
+                if relation_key in d0:
+                    d1 = d0[relation_key]
+                else:
+                    d1 = {}
+                    d0[relation_key] = d1
+                a_key = aggregator_keys[i]
+                if a_key in d1:
+                    values[i] = d1[a_key]
+                    # used_comp_memo[0] += 1
+                else:
+                    filtered_chains_aggregators.append(chain_aggregators)
+                    filtered_aggregator_keys.append(a_key)
+                    # used_comp_memo[1] += 1
+        else:
+            filtered_chains_aggregators = chains_aggregators
+            filtered_aggregator_keys = [None] * len(chains_aggregators)
+        if filtered_chains_aggregators:
+            values_partial_all = self.get_test_value_helper(
+                example, chain_relations, filtered_chains_aggregators,
+                nb_fresh_vars, fresh_indices, known_unknown)
+        else:
+            values_partial_all = []
+        where_to = 0
+        for agg_key, chain_aggregators, values_partial in zip(
+                filtered_aggregator_keys, filtered_chains_aggregators,
+                values_partial_all):
+            v = chain_aggregators[0].aggregate_flat(values_partial)
+            # assert v is not None
+            while values[where_to] is not None:
+                where_to += 1
+            values[where_to] = v
+            if should_memo:
+                d1[agg_key] = v
+        return values
+
+    def get_test_value_helper(self,
+                              example,
+                              chain_relations,
+                              chains_aggregators,
+                              nb_fresh_vars,
+                              fresh_indices,
+                              known_unknown_list,
+                              depth=1):
+        def results_generator(related_objects):
+            for r in related_objects:
+                # set
+                for i in unknown:
+                    rel_variables[i].set_value(r[i])
+                # compute
+                yield self.get_test_value_helper(example, chain_relations,
+                                                 chains_aggregators,
+                                                 nb_fresh_vars, fresh_indices,
+                                                 known_unknown_list, depth + 1)
+                # unset
+                for i in unknown:
+                    rel_variables[i].unset_value()
+
+        def should_keep_value(value):
+            return not (self.ignore_critical_values
+                        and value in CRITICAL_VALUES)
+
+        # for chain_aggregators in chains_aggregators:
+        #     assert len(chain_relations) == len(chain_aggregators)
+        relation, rel_variables_names = chain_relations[depth - 1]
+        rel_variables = [example[n] for n in rel_variables_names]
+        # aggregators = [chain[0] for chain in chains_aggregators]
+        if known_unknown_list is None:
+            known_unknown = [[], []]  # type: List[List[int]]
+            for i, v in enumerate(rel_variables_names):
+                known_unknown[example[v].is_unset()].append(i)
+        else:
+            known_unknown = known_unknown_list[depth - 1]
+        known, unknown = known_unknown
+        related = relation.get_all(rel_variables, known)
+        if len(chain_relations) == depth:
+            if nb_fresh_vars < 0:
+                fresh_indices = [
+                    i for i in unknown if rel_variables[i].can_vary()
+                ]
+                nb_fresh_vars = len(
+                    set(rel_variables[i].get_name() for i in fresh_indices))
+            if nb_fresh_vars == 0:
+                # everything known, more or less, this is only the proof of (non)existence
+                # There should be either 0 or 1 results, we pass their number.
+                # This can happen in the cases such as isFriend(x, Y), isFriend(Y, z),
+                # when Y has already a value after searching for the results isFriend(x, Y).
+                # hits = len(related)
+                # assert hits <= 1
+                to_aggregate = [len(related)]
+                # to_aggregate = related TODO: This more sense?
+            elif nb_fresh_vars == 1:
+                to_aggregate = [r[fresh_indices[0]]
+                                for r in related]  # flattened
+            else:
+                to_aggregate = related  # [[r[i] for i in fresh_indices] for r in related]
+                # if not all([aggregator in COMPLEX_ENOUGH_AGGREGATORS for aggregator in aggregators]):
+                #     raise WrongValueException("Your aggregators: {}. Allowed: {}".format(aggregators,
+                #                                                                          COMPLEX_ENOUGH_AGGREGATORS))
+            return [to_aggregate for _ in range(len(chains_aggregators))]
+        else:
+            next_aggregators = [chain[depth] for chain in chains_aggregators
+                                ]  # type: List[Aggregator]
+            to_aggregate = []
+            for res in results_generator(related):
+                to_aggregate.append(res)
+            answer = []
+            for a_ind, a in enumerate(next_aggregators):
+                ls = [neigh[a_ind] for neigh in to_aggregate]
+                out = [x for x in a.aggregate(ls) if should_keep_value(x)]
+                answer.append(out)
+            return answer
+
+    @staticmethod
+    def is_better_than_previous(new_score, previous_score):
+        return new_score < previous_score
```

### Comparing `re3py-0.35/re3py/learners/core/variables.py` & `re3py-0.36/re3py/learners/core/variables.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-class Variable:
-    def __init__(self, name: str, value_type, value):
-        self.name = name
-        self.value_type = value_type
-        self.value = value
-
-    def __repr__(self):
-        v = self.value if not self.is_unset() else "?"
-        return "{}({})".format(self.name, v)
-
-    def __eq__(self, other):
-        return self.name == other.name
-
-    def __lt__(self, other):
-        return self.name < other.name
-
-    def __hash__(self):
-        return hash(self.name)
-
-    def rename(self, n):
-        self.name = n
-
-    def get_name(self):
-        return self.name
-
-    def set_value(self, v):
-        self.value = v
-
-    def unset_value(self):
-        self.value = None
-
-    def is_unset(self):
-        return self.value is None
-
-    def get_value(self):
-        return self.value
-
-    def is_constant(self):
-        return False
-
-    def can_vary(self):
-        return False
-
-    def make_copy(self):
-        raise NotImplementedError("This should be implemented by a subclass.")
-
-
-class ConstantVariable(Variable):
-    def __init__(self, name, variable_type, value):
-        super().__init__(name, variable_type, value)
-        assert self.name.startswith("C")
-
-    def is_constant(self):
-        return True
-
-    def make_copy(self):
-        return ConstantVariable(self.name, self.value_type, self.value)
-
-
-class VariableVariable(Variable):
-    def __init__(self, name, variable_type, value):
-        super().__init__(name, variable_type, value)
-        assert self.name[0] in "XY"  # X for the initial ones, Y for the others
-
-    def can_vary(self):
-        return True
-
-    def make_copy(self):
-        return VariableVariable(self.name, self.value_type, self.value)
+class Variable:
+    def __init__(self, name: str, value_type, value):
+        self.name = name
+        self.value_type = value_type
+        self.value = value
+
+    def __repr__(self):
+        v = self.value if not self.is_unset() else "?"
+        return "{}({})".format(self.name, v)
+
+    def __eq__(self, other):
+        return self.name == other.name
+
+    def __lt__(self, other):
+        return self.name < other.name
+
+    def __hash__(self):
+        return hash(self.name)
+
+    def rename(self, n):
+        self.name = n
+
+    def get_name(self):
+        return self.name
+
+    def set_value(self, v):
+        self.value = v
+
+    def unset_value(self):
+        self.value = None
+
+    def is_unset(self):
+        return self.value is None
+
+    def get_value(self):
+        return self.value
+
+    def is_constant(self):
+        return False
+
+    def can_vary(self):
+        return False
+
+    def make_copy(self):
+        raise NotImplementedError("This should be implemented by a subclass.")
+
+
+class ConstantVariable(Variable):
+    def __init__(self, name, variable_type, value):
+        super().__init__(name, variable_type, value)
+        assert self.name.startswith("C")
+
+    def is_constant(self):
+        return True
+
+    def make_copy(self):
+        return ConstantVariable(self.name, self.value_type, self.value)
+
+
+class VariableVariable(Variable):
+    def __init__(self, name, variable_type, value):
+        super().__init__(name, variable_type, value)
+        assert self.name[0] in "XY"  # X for the initial ones, Y for the others
+
+    def can_vary(self):
+        return True
+
+    def make_copy(self):
+        return VariableVariable(self.name, self.value_type, self.value)
```

### Comparing `re3py-0.35/re3py/learners/predictive_model.py` & `re3py-0.36/re3py/learners/predictive_model.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from ..data.data_and_statistics import Datum
-import pickle
-
-
-class PredictiveModel:
-    def build(self, *args):
-        raise NotImplementedError("This should be implemented by a subclass.")
-
-    def predict(self, d: Datum):
-        raise NotImplementedError("This should be implemented by a subclass.")
-
-    def print_model(self, file_name):
-        raise NotImplementedError("This should be implemented by a subclass.")
-
-    def save_model(self, file_name):
-        pickle.dump(self, open(file_name, 'wb'))
-
-    @staticmethod
-    def load_model(file_name):
-        return pickle.load(open(file_name, 'rb'))
-
-
-# noinspection PyAbstractClass
-class TreeEnsemble(PredictiveModel):
-    def compute_ranking(self, ranking_type):
-        raise NotImplementedError("This should be implemented by a subclass.")
+from ..data.data_and_statistics import Datum
+import pickle
+
+
+class PredictiveModel:
+    def fit(self, *args):
+        raise NotImplementedError("This should be implemented by a subclass.")
+
+    def predict(self, d: Datum):
+        raise NotImplementedError("This should be implemented by a subclass.")
+
+    def dump_to_text(self, file_name):
+        raise NotImplementedError("This should be implemented by a subclass.")
+
+    def dump_to_bin(self, file_name):
+        pickle.dump(self, open(file_name, 'wb'))
+
+    @staticmethod
+    def load(file_name):
+        return pickle.load(open(file_name, 'rb'))
+
+
+# noinspection PyAbstractClass
+class TreeEnsemble(PredictiveModel):
+    def compute_ranking(self, ranking_type):
+        raise NotImplementedError("This should be implemented by a subclass.")
```

### Comparing `re3py-0.35/re3py/learners/random_forest.py` & `re3py-0.36/re3py/learners/random_forest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-from .tree import DecisionTree
-from ..data.data_and_statistics import *
-from .predictive_model import TreeEnsemble
-from ..ranking.ensemble_ranking import EnsembleRanking
-from typing import List
-
-
-class RandomForest(TreeEnsemble):
-    zero_one_aggregator = "ZERO-ONE"
-    proportions_aggregator = "PROPORTIONS"
-    votes_aggregators = [zero_one_aggregator, proportions_aggregator]
-
-    def __init__(self,
-                 nb_trees_to_build=100,
-                 votes_aggregator=proportions_aggregator,
-                 random_seed=314159,
-                 **tree_parameters):
-        self.trees = []  # type: List[DecisionTree]
-        self.nb_trees = nb_trees_to_build
-        self.votes_aggregator = votes_aggregator
-        self.ensemble_random = EnsembleRandomGenerator(random_seed)
-        self.tree_parameters = tree_parameters
-        self.sanity_check()
-
-    def sanity_check(self):
-        if self.votes_aggregator not in RandomForest.votes_aggregators:
-            message = "Wrong votes aggregator: {}. Allowed values: {}."
-            raise WrongValueException(
-                message.format(self.votes_aggregator,
-                               RandomForest.votes_aggregators))
-
-    def build(self, data: Dataset):
-        for t in range(self.nb_trees):
-            print("Building tree {}".format(t + 1))
-            self.tree_parameters[
-                'random_seed'] = self.ensemble_random.next_tree_seed()
-            self.trees.append(DecisionTree(**self.tree_parameters))
-            tree_data = data.bootstrap_replicate(
-                self.ensemble_random.next_bootstrap_seed(),
-                per_class=self.trees[-1].per_class_bootstrap)
-            self.trees[-1].build(tree_data)
-
-    def compute_ranking(self, ranking_type):
-        feature_ranking = EnsembleRanking({}, {}, ranking_type, self.nb_trees)
-        for i, tree in enumerate(self.trees):
-            attribute_scores, aggregate_scores = feature_ranking.compute_tree_contribution(
-                tree)
-            feature_ranking.update_attributes(attribute_scores,
-                                              aggregate_scores, i)
-        feature_ranking.normalize()
-        return feature_ranking
-
-    def predict(self, d: Datum, nb_trees=None):
-        if nb_trees is None:
-            nb_trees = len(self.trees)
-        predictions_stats = []  # type: List[NodeStatistics]
-        for tree in self.trees[:nb_trees]:
-            predictions_stats.append(tree.predict(d, True))
-        statistics_class = predictions_stats[0].__class__
-        ensemble_stats = statistics_class.construct_from_parent(
-            predictions_stats[0])
-        for s in predictions_stats:
-            ensemble_stats.add_other_for_ensemble_prediction(s, 1)
-        if statistics_class == NodeStatisticsClassification:
-            if self.votes_aggregator == RandomForest.zero_one_aggregator:
-                values = ensemble_stats.get_nb_examples_per_class()
-            elif self.votes_aggregator == RandomForest.proportions_aggregator:
-                values = ensemble_stats.get_per_class_probabilities()
-            else:
-                raise WrongValueException("Wrong vote aggregator: {}".format(
-                    self.votes_aggregator))
-            class_names = ensemble_stats.get_class_names()
-            return class_names[arg_max(values)]
-        elif statistics_class in [
-                NodeStatisticsRegression, NodeStatisticsMultitargetRegression
-        ]:
-            ensemble_stats.create_predictions()
-            return ensemble_stats.get_prediction()
-        else:
-            raise NotImplementedError(":DD")
-
-    def print_model(self, file_name):
-        f = open(file_name, "w")
-        for i, tree in enumerate(self.trees):
-            print("Tree {}:".format(i + 1), file=f)
-            print(str(tree), file=f)
-            print("", file=f)
-        f.close()
+from .tree import DecisionTree
+from ..data.data_and_statistics import *
+from .predictive_model import TreeEnsemble
+from ..ranking.ensemble_ranking import EnsembleRanking
+from typing import List
+
+
+class RandomForest(TreeEnsemble):
+    zero_one_aggregator = "ZERO-ONE"
+    proportions_aggregator = "PROPORTIONS"
+    votes_aggregators = [zero_one_aggregator, proportions_aggregator]
+
+    def __init__(self,
+                 nb_trees_to_build=100,
+                 votes_aggregator=proportions_aggregator,
+                 random_seed=314159,
+                 **tree_parameters):
+        self.trees = []  # type: List[DecisionTree]
+        self.nb_trees = nb_trees_to_build
+        self.votes_aggregator = votes_aggregator
+        self.ensemble_random = EnsembleRandomGenerator(random_seed)
+        self.tree_parameters = tree_parameters
+        self.sanity_check()
+
+    def sanity_check(self):
+        if self.votes_aggregator not in RandomForest.votes_aggregators:
+            message = "Wrong votes aggregator: {}. Allowed values: {}."
+            raise WrongValueException(
+                message.format(self.votes_aggregator,
+                               RandomForest.votes_aggregators))
+
+    def fit(self, data: Dataset):
+        for t in range(self.nb_trees):
+            print("Building tree {}".format(t + 1))
+            self.tree_parameters[
+                'random_seed'] = self.ensemble_random.next_tree_seed()
+            self.trees.append(DecisionTree(**self.tree_parameters))
+            tree_data = data.bootstrap_replicate(
+                self.ensemble_random.next_bootstrap_seed(),
+                per_class=self.trees[-1].per_class_bootstrap)
+            self.trees[-1].fit(tree_data)
+
+    def compute_ranking(self, ranking_type):
+        feature_ranking = EnsembleRanking({}, {}, ranking_type, self.nb_trees)
+        for i, tree in enumerate(self.trees):
+            attribute_scores, aggregate_scores = feature_ranking.compute_tree_contribution(
+                tree)
+            feature_ranking.update_attributes(attribute_scores,
+                                              aggregate_scores, i)
+        feature_ranking.normalize()
+        return feature_ranking
+
+    def predict(self, d: Datum, nb_trees=None):
+        if nb_trees is None:
+            nb_trees = len(self.trees)
+        predictions_stats = []  # type: List[NodeStatistics]
+        for tree in self.trees[:nb_trees]:
+            predictions_stats.append(tree.predict(d, True))
+        statistics_class = predictions_stats[0].__class__
+        ensemble_stats = statistics_class.construct_from_parent(
+            predictions_stats[0])
+        for s in predictions_stats:
+            ensemble_stats.add_other_for_ensemble_prediction(s, 1)
+        if statistics_class == NodeStatisticsClassification:
+            if self.votes_aggregator == RandomForest.zero_one_aggregator:
+                values = ensemble_stats.get_nb_examples_per_class()
+            elif self.votes_aggregator == RandomForest.proportions_aggregator:
+                values = ensemble_stats.get_per_class_probabilities()
+            else:
+                raise WrongValueException("Wrong vote aggregator: {}".format(
+                    self.votes_aggregator))
+            class_names = ensemble_stats.get_class_names()
+            return class_names[arg_max(values)]
+        elif statistics_class in [
+                NodeStatisticsRegression, NodeStatisticsMultitargetRegression
+        ]:
+            ensemble_stats.create_predictions()
+            return ensemble_stats.get_prediction()
+        else:
+            raise NotImplementedError(":DD")
+
+    def dump_to_text(self, file_name):
+        f = open(file_name, "w")
+        for i, tree in enumerate(self.trees):
+            print("Tree {}:".format(i + 1), file=f)
+            print(str(tree), file=f)
+            print("", file=f)
+        f.close()
```

### Comparing `re3py-0.35/re3py/learners/tree.py` & `re3py-0.36/re3py/learners/tree.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,1414 +1,1414 @@
-from typing import Iterable
-from .core.aggregators import *
-from .core.comparators import *
-from .core.tree_node_split import BinarySplit
-from .core.heuristic import Heuristic
-from ..data.data_and_statistics import *
-from ..data.task_settings import Settings
-from .core.variables import *
-from ..data.relation import Relation
-from ..utilities.my_exceptions import WrongValueException
-from ..utilities.my_utils import *
-import itertools
-import random
-from .predictive_model import PredictiveModel
-from time import clock
-import math
-import copy
-from .core.tree_node_split import TEST_VALUE_MEMO
-# from my_memo import used_comp_memo
-import subprocess
-from .core.communicate_with_java import send_data, send_variables, compute_test_values
-from py4j.java_gateway import JavaGateway, GatewayParameters
-
-
-class TreeNode:
-    positive_branch = 0
-    negative_branch = 1
-
-    def __init__(self, description, parent, children,
-                 binary_split: Union[BinarySplit, None],
-                 stats: Union[NodeStatistics, None], depth: int):
-        self.description = description
-        self.parent = parent  # type: 'TreeNode'
-        self.children = children
-        self.split = binary_split  # type: BinarySplit
-        self.stats = stats  # type: NodeStatistics
-        self.depth = depth
-
-    def get_parent(self) -> 'TreeNode':
-        return self.parent
-
-    def get_split(self):
-        return self.split
-
-    def set_depth(self, d):
-        self.depth = d
-
-    def get_depth(self):
-        return self.depth
-
-    def set_split(self, s):
-        self.split = s
-
-    def set_parent(self, other):
-        self.parent = other
-
-    def get_child(self, i):
-        return self.children[i]
-
-    def get_children(self):
-        return self.children
-
-    def add_child(self, other):
-        self.add_children([other])
-
-    def add_children(self, others):
-        if self.children is None:
-            self.children = []
-        self.children += others
-
-    def is_leaf(self):
-        return len(self.children) == 0
-
-    def get_stats(self):
-        return self.stats
-
-    def set_stats(self, s):
-        self.stats = s
-
-
-class DecisionTree(PredictiveModel):
-    root_node_depth = 1
-    eps = 10**-10
-    left_child_indicator = "0"
-    right_child_indicator = "1"
-    root_indicator = "root"
-
-    square_root = "sqrt"
-    log2 = "log"
-    allowed_n_tests = [square_root, log2]
-
-    def __init__(
-            self,
-            heuristic=None,
-            statistics=None,
-            root_node=None,
-            max_number_internal_nodes=float('inf'),
-            max_number_atom_tests=1,
-            allowed_atom_tests=None,
-            allowed_aggregators: Union[None, Iterable[str]] = None,
-            max_depth=float("inf"),
-            minimal_examples_in_leaf=1,
-            max_number_of_evaluated_tests_per_node=float("inf"),
-            max_relative_number_of_evaluated_tests_per_node: Union[float,
-                                                                   str] = 1.0,
-            random_seed=2718281828,
-            java_port: Union[None, int] = None,
-            is_outer_java=False,
-            longest_atom_test_chain=4,
-            class_weights: Union[None, Dict[str, float]] = None,
-            per_class_bootstrap=False,
-            only_existential=False,
-            minimal_impurity=10**-16):
-        self.heuristic = Heuristic() if heuristic is None else heuristic
-        self.target_data_stat = statistics
-        self.max_number_internal_nodes = max_number_internal_nodes
-        self.max_number_atom_tests = max_number_atom_tests
-        self.allowed_atom_tests = {} if allowed_atom_tests is None else allowed_atom_tests  # the structured version
-        self.allowed_aggregators = set(
-        ) if allowed_aggregators is None else set(allowed_aggregators)
-        self.max_depth = max_depth
-        self.minimal_examples_in_leaf = minimal_examples_in_leaf
-        self.max_number_of_evaluated_tests_per_node = max_number_of_evaluated_tests_per_node
-        self.max_relative_number_of_evaluated_tests_per_node = max_relative_number_of_evaluated_tests_per_node
-        self.relative_number_tests_sanity_check()
-        self.random_seed = random_seed
-        self.java_port = java_port
-        self.is_outer_java = is_outer_java
-        self.longest_atom_test_chain = longest_atom_test_chain
-        self.class_weights = class_weights
-        self.per_class_bootstrap = per_class_bootstrap
-        self.only_existential = only_existential
-        self.update_allowed_aggregates()
-        self.minimal_impurity = minimal_impurity  # relative
-
-        self.root_node = root_node  # type: Union['TreeNode', None]
-        self.target_relation_description = None
-        # tree building fields
-        self.target_relation_variables = []  # type: List[Variable]
-        self.descriptive_data = {}  # type: Dict[str, Relation]
-        self.var_count = {"XY": 0, "C": 0}  # TODO: less hard-coded?:)
-        self.temp_var_count = 0
-        self.current_number_internal_nodes = 0
-        self.all_variables = {}
-        self.induce_tree_time = 0.0
-        self.statistics_time = 0.0
-        self.get_test_value_time = 0.0
-        self.split_eval_time = 0.0
-        self.set_example_values_time = 0.0
-        self.find_values_time = 0.0
-        self.nominal_tests = 0
-        self.nominal_tests_time = 0
-        self.numeric_tests = 0
-        self.numeric_tests_time = 0
-
-        self.p = None
-        self.wrapper = None
-        self.client = None
-        self.gateway = None
-
-    def print_times(self):
-        times = [
-            self.induce_tree_time, self.statistics_time,
-            self.get_test_value_time, self.split_eval_time,
-            self.set_example_values_time, self.find_values_time,
-            self.nominal_tests, self.nominal_tests_time, self.numeric_tests,
-            self.numeric_tests_time
-        ]
-        names = [
-            "induce", "statistics", "test value", "eval split",
-            "example values", "find values", "nominal tests", "nom. t. time",
-            "numeric tests", "num t. time"
-        ]
-        for time, name in zip(times, names):
-            print("{: <14}:".format(name), time)
-        print()
-
-    def __str__(self):
-        def helper(node: TreeNode):
-            branches_names = ["YES", "NO"]
-            spaces = "  " * node.get_depth()
-            if node.is_leaf():
-                return "{}{}".format(spaces, node.get_stats())
-            else:
-                parts = [
-                    "{}IF {}:".format(spaces,
-                                      node.split.__str__(self.all_variables))
-                ]
-                for b_name, child in zip(branches_names, node.children):
-                    parts.append("{}{}".format(spaces, b_name))
-                    parts.append(helper(child))
-                return "\n".join(parts)
-
-        header = "Tree for {}:".format(self.target_relation_description)
-        tree = helper(self.root_node)
-        return "\n".join([header, tree])
-
-    def __iter__(self):
-        """
-        Iterates over the nodes in the tree: yields root, then 'recursively' visits the left and the right subtree.
-        :return:
-        """
-        if self.root_node is not None:
-            stack = [self.root_node]
-            while stack:
-                node = stack.pop()
-                yield node
-                stack += node.get_children()[::-1]
-
-    def print_model(self, file_name):
-        f = open(file_name, "w")
-        print(str(self), file=f)
-        f.close()
-
-    def get_absolute_number_tests_from_relative(self, nb_tests):
-        n_rel = self.max_relative_number_of_evaluated_tests_per_node
-        if isinstance(n_rel, str):
-            if n_rel == DecisionTree.square_root:
-                return round(math.sqrt(nb_tests))
-            elif n_rel == DecisionTree.log2:
-                return round(math.log2(nb_tests))
-            else:
-                raise ValueError("Wrong function: {}".format(n_rel))
-        elif isinstance(n_rel, float):
-            return round(n_rel * nb_tests)
-        else:
-            raise ValueError(
-                "Wrong relative number of tests: {}.".format(n_rel))
-
-    def relative_number_tests_sanity_check(self):
-        if isinstance(self.max_relative_number_of_evaluated_tests_per_node,
-                      str):
-            if self.max_relative_number_of_evaluated_tests_per_node not in DecisionTree.allowed_n_tests:
-                message = "Wrong number of tests: {}. If string, it should be an element of {}"
-                raise ValueError(
-                    message.format(
-                        self.max_relative_number_of_evaluated_tests_per_node,
-                        DecisionTree.allowed_n_tests))
-        elif isinstance(self.max_relative_number_of_evaluated_tests_per_node,
-                        float):
-            if not (0.0 <= self.max_relative_number_of_evaluated_tests_per_node
-                    <= 1):
-                message = "Wrong relative number of tests: {}. If float, should be in the interval (0, 1]"
-                raise ValueError(
-                    message.format(
-                        self.max_relative_number_of_evaluated_tests_per_node))
-        else:
-            raise ValueError(
-                "Relative number of tests should be string or float.")
-
-    def chosen_tests(self, tests_generator, current_vars_per_type):
-        nb_tests = 0
-        nb_chains = 0
-        for jj, chain in enumerate(tests_generator):
-            # if jj % 10**2 == 0:
-            #     print("-", end="")
-            # if jj % 10**4 == 0:
-            #     print()
-            nb_chains += 1
-            _, relation_chain, aggregator_chains, _ = chain
-            # print(relation_chain)
-            num_aggregator_chains = len(list(aggregator_chains))
-            _, _, _, _, c_num = self.create_example_and_chains(
-                relation_chain, current_vars_per_type)
-            nb_tests += num_aggregator_chains * c_num
-        # print()
-        k_proportion = self.get_absolute_number_tests_from_relative(nb_tests)
-        k_absolute = self.max_number_of_evaluated_tests_per_node
-        k = min(k_proportion,
-                k_absolute)  # Select the more restrictive criterion
-        k = max(k, 1)  # but at least one
-        k = min(k, nb_tests)  # but at most all tests
-        return set(random.sample(range(nb_tests), k=k)), nb_tests, nb_chains
-
-    def generate_next_var_name(self, first_letter):
-        key = None
-        if first_letter == "C":
-            key = "C"
-        elif first_letter in "XY":
-            key = "XY"
-        c = self.var_count[key]
-        self.var_count[key] += 1
-        return "{}{}".format(first_letter, c)
-
-    def generate_temp_var_name(self, first_letter):
-        return self.generate_temp_var_names(first_letter, [1])[0]
-
-    def generate_temp_var_names(self, first_letter, offsets):
-        names = [
-            "{}{}".format(first_letter, self.temp_var_count - offset)
-            for offset in offsets
-        ]
-        if names:
-            self.temp_var_count -= max(offsets)
-        return names
-
-    def reset_temp_var_count(self):
-        self.temp_var_count = 0
-
-    @staticmethod
-    def get_first_var_letter(object_type, is_input):
-        if object_type == Settings.atom_test_type_constant:
-            return "C"
-        elif is_input:
-            return "X"
-        else:
-            return "Y"
-
-    def initialize_statistics(self, node: TreeNode, data: List[Datum]):
-        t0 = clock()
-        statistics_class = self.target_data_stat.__class__
-        initial_stats = statistics_class.construct_from_parent(
-            self.target_data_stat)
-        initial_stats.add_examples(data)
-        node.set_stats(initial_stats)
-        variability = self.heuristic.compute_variability(node.get_stats())
-        node.get_stats().set_variability(variability)
-        t1 = clock()
-        self.statistics_time += t1 - t0
-
-    def build(self, data: Dataset):
-        t0 = clock()
-        random.seed(self.random_seed)
-        self.target_data_stat = data.get_copy_statistics()
-        target_relation = data.get_target_relation()  # no examples - ok?
-        self.descriptive_data = data.get_descriptive_data(
-        )  # type: Dict[str, Relation]
-        target_data = data.get_target_data()  # type: List[Datum]
-        if BinarySplit.use_memo:
-            DecisionTree.populate_dict(target_data)
-        current_vars_per_type = [{}]  # type: List[Dict[str, Set[Variable]]]
-        target_var_names = []
-        self.target_relation_variables = []  # type: List[Variable]
-        for object_type in target_relation.get_types()[:-1]:
-            var_name = self.generate_next_var_name(
-                DecisionTree.get_first_var_letter(object_type, True))
-            assert not var_name.startswith("C")
-            new_var = VariableVariable(var_name, object_type, None)
-            if object_type not in current_vars_per_type[-1]:
-                current_vars_per_type[-1][object_type] = set()
-            current_vars_per_type[-1][object_type].add(new_var)
-            self.target_relation_variables.append(new_var)
-            target_var_names.append(new_var.get_name())
-
-        self.target_relation_description = "{}, {}".format(
-            target_relation.get_name(), target_var_names)
-        all_variable_names = set(target_var_names)
-        self.root_node = TreeNode(DecisionTree.root_indicator, None, [], None,
-                                  None, DecisionTree.root_node_depth)
-        # initial statistics
-        self.initialize_statistics(self.root_node, target_data)
-
-        if self.java_port is not None:
-            self.java_on()
-
-        if self.java_port is not None:
-            send_data(data, self.client, self.wrapper)
-
-        # manipulate target data
-        self.target_data_induction_preparation(target_data)
-        self.build_helper(target_data, self.root_node, current_vars_per_type,
-                          target_var_names, all_variable_names)
-        # un-manipulate target data
-        self.reverse_target_data_induction_preparation(target_data)
-
-        for v in self.target_relation_variables:
-            assert v.can_vary()
-            v.unset_value()
-        for v in self.target_relation_variables:
-            self.all_variables[v.get_name()] = v
-        t1 = clock()
-        self.induce_tree_time = t1 - t0
-        self.print_times()
-        # s = max(1, sum(used_comp_memo))
-        # print("Memo vs. compute: {:.4f} : {:.4f}; all: {}".format(used_comp_memo[0] / s,
-        #                                                           used_comp_memo[1] / s,
-        #                                                           s))
-        # used_comp_memo[0] = 0
-        # used_comp_memo[1] = 0
-
-        if self.java_port is not None:
-            self.java_off()
-
-    def java_on(self):
-        if not self.is_outer_java:
-            # open server
-            this_dir = os.path.dirname(os.path.abspath(__file__))
-            path = os.path.join(this_dir, "core", "speedUp.jar")
-            if not os.path.exists(path):
-                path = "speedUp.jar"
-            self.p = subprocess.Popen(r"java -jar {} {}".format(
-                path, self.java_port),
-                                      shell=True)
-            for counter in range(10**8):
-                _ = 21 + 21
-        gateway_parameters = GatewayParameters(port=self.java_port)
-        self.gateway = JavaGateway(gateway_parameters=gateway_parameters)
-        self.wrapper = self.gateway.entry_point.get_wrapper()
-        self.client = self.gateway._gateway_client
-
-    def java_off(self):
-        if not self.is_outer_java:
-            self.gateway.shutdown()
-            self.p.kill()
-        self.wrapper = None
-        self.client = None
-        self.gateway = None
-        self.p = None
-
-    def update_allowed_aggregates(self):
-        if self.only_existential:
-            self.allowed_aggregators = {COUNT.get_name()}
-            print(
-                "Existential tests only ==> The allowed aggregates changed to {}"
-                .format(self.allowed_aggregators))
-
-    def build_helper(self, target_data: List[Datum], current_node: TreeNode,
-                     current_vars_per_type, target_relation_vars,
-                     all_variable_names: Set[str]):
-        # print("Current vars before inducing", current_node.description)
-        # print("cur_ver_per_type, all_names", current_vars_per_type, all_variable_names)
-        print("{}Building node on depth {}".format(
-            "  " * current_node.get_depth(), current_node.get_depth()))
-        current_var_names = [{
-            t: {v.get_name()
-                for v in vs}
-            for t, vs in d.items()
-        } for d in current_vars_per_type]
-        # print("curr var names", current_var_names)
-        # find a split
-        bs = BinarySplit([], None, None, True, None)
-        best_score = BinarySplit.worst_split_score
-        best_configuration = (None, None, None, None, None, None)
-        if self.should_try_find_a_split(current_node, target_data):
-            parents_test = []
-            node = current_node
-            while node.parent is not None:
-                if node == node.get_parent().children[0]:
-                    parents_test = node.get_parent().get_split().get_test()
-                    break
-                node = node.get_parent()
-            attributes_counting = self.generate_possible_attributes(
-                copy.deepcopy(current_var_names), parents_test,
-                target_relation_vars)
-            self.reset_temp_var_count()
-            attributes = self.generate_possible_attributes(
-                current_var_names, parents_test, target_relation_vars)
-
-        else:
-            attributes_counting = iter([])
-            attributes = iter([])
-        chosen_attributes, all_attributes_computed, all_chains_computed = self.chosen_tests(
-            attributes_counting, current_vars_per_type)
-        # print("{}Attributes generated: {}".format("  " * current_node.get_depth(), all_attributes_computed))
-        all_attributes_counted = 0
-        all_chains_counted = 0
-        for chain in attributes:
-            all_chains_counted += 1
-            # print(".", end="")
-            # if all_chains_counted % 100 == 0:
-            #     print("{}".format("  " * current_node.get_depth()), end="")
-            starting_index, relation_chain, aggregator_chains, fresh_vars = chain
-            # print("{}relation chain: {}".format("  " * current_node.get_depth(), relation_chain))
-            nb_fresh_vars = len(fresh_vars[0])
-            fresh_indices = fresh_vars[1]
-            # print(relation_chain)
-            example, rc_modified, c_values, c_var_names, c_num = self.create_example_and_chains(
-                relation_chain, current_vars_per_type)
-            a_ch = list(aggregator_chains)
-            # print(a_ch)
-            known_unknown = None
-            temp_counter = 0
-            for c_vs in c_values:
-                filtered_agg_chains = []
-                filtered_output_types = []
-                for i, agg_chain in enumerate(a_ch):
-                    if all_attributes_counted in chosen_attributes:
-                        filtered_agg_chains.append(agg_chain[0])
-                        filtered_output_types.append(agg_chain[1])
-                    all_attributes_counted += 1
-                    temp_counter += 1
-                # print("   csv -->", c_vs)
-                for c_name, c_v in zip(c_var_names, c_vs):
-                    example[c_name].set_value(c_v)
-                if BinarySplit.use_memo or known_unknown is None:
-                    # unset target variables
-                    for init_var_name in target_relation_vars:
-                        example[init_var_name].unset_value()
-                    r_key, a_keys, known_unknown = DecisionTree.test_values_memo_keys(
-                        example, rc_modified, filtered_agg_chains)
-                else:
-                    r_key, a_keys = None, []
-                t0 = clock()
-
-                if self.java_port is not None:
-                    # do stuff here
-                    send_variables(example, self.client, self.wrapper)
-                    all_test_values = compute_test_values(
-                        target_data, target_relation_vars, rc_modified,
-                        filtered_agg_chains, r_key, a_keys, nb_fresh_vars,
-                        fresh_indices, known_unknown, self.client,
-                        self.wrapper)
-                else:
-                    all_test_values = []
-                    for jj, datum in enumerate(target_data):
-                        u0 = clock()
-                        for init_var_name, train_value in zip(
-                                target_relation_vars, datum.get_descriptive()):
-                            example[init_var_name].set_value(train_value)
-                        u1 = clock()
-                        self.set_example_values_time += u1 - u0
-                        u0 = clock()
-                        all_test_values.append(
-                            bs.get_test_values(example, rc_modified,
-                                               filtered_agg_chains, r_key,
-                                               a_keys, datum.identifier,
-                                               nb_fresh_vars, fresh_indices,
-                                               known_unknown))
-                        u1 = clock()
-                        self.find_values_time += u1 - u0
-                        # if jj % 10 == 0:
-                        #     print(".", end="")
-
-                # n_target_examples = len(target_data)
-                # assert n_target_examples == len(all_test_values1) == len(all_test_values2)
-                # for i, v1, v2 in zip(range(n_target_examples), all_test_values1, all_test_values2):
-                #     if v1 != v2:
-                #         print(i, v1, v2, target_data[i])
-                #         raise ValueError("... :)")
-                # print()
-
-                t1 = clock()
-                self.get_test_value_time += t1 - t0
-                t0 = clock()
-                score, configuration = self.evaluate_candidate_splits(
-                    current_node, all_test_values, target_data,
-                    current_vars_per_type[0], filtered_output_types)
-                t1 = clock()
-                self.split_eval_time += t1 - t0
-                if BinarySplit.is_better_than_previous(score, best_score):
-                    best_score = score
-                    a_chain_ind, comparator, theta, partition, is_variable_free = configuration
-                    best_configuration = (rc_modified,
-                                          filtered_agg_chains[a_chain_ind],
-                                          c_vs, c_var_names, comparator, theta,
-                                          partition, is_variable_free,
-                                          starting_index)
-            # unset constants
-            for c_name in c_var_names:
-                example[c_name].unset_value()
-            # unset target variables
-            for init_var_name in target_relation_vars:
-                example[init_var_name].unset_value()
-            # sanity check
-            if temp_counter != c_num * len(a_ch):
-                print(temp_counter, c_num, len(a_ch))
-                print(example, rc_modified, c_values, c_var_names, c_num, a_ch)
-                print(relation_chain)
-                raise WrongValueException("Wrong value of counted attributes!")
-        # sanity check
-        if all_attributes_computed != all_attributes_counted or all_chains_computed != all_chains_counted:
-            message = "\nPredicted number of attributes: {} Number of attributes counted: {}\n" \
-                      "Predicted number of chains: {} Counted number of chains: {}"
-            raise WrongValueException(
-                message.format(all_attributes_computed, all_attributes_counted,
-                               all_chains_computed, all_chains_counted))
-        # create internal node or leaf
-        if BinarySplit.is_better_than_previous(best_score,
-                                               BinarySplit.worst_split_score):
-            self.current_number_internal_nodes += 1
-            r_chain, a_chain, c_vs, c_var_names, comparator, theta, partition, is_variable_free, starting_index = \
-                best_configuration
-            # print("---> r chain, c_var names", r_chain, c_var_names, sep="\n")
-            r_chain_fresh_part = len(r_chain) - starting_index + 1
-            split_test = []
-            # [d1, ...], d2: {type1: {freshVariable1, ...}, ...}
-            fresh_variables_chains = [{} for _ in range(r_chain_fresh_part)]
-            fresh_variables = {}  # Union of the upper
-            const_name_to_value = {n: v for n, v in zip(c_var_names, c_vs)}
-            temp_to_fix_name = {}
-            # find fresh variables, get rid of temporary names
-            for i_relation, ((r, var_names),
-                             a) in enumerate(zip(r_chain, a_chain)):
-                new_names = []
-                for var_name, var_type in zip(
-                        var_names,
-                        self.descriptive_data[r.get_name()].get_types()):
-                    # not seen in previous chains?
-                    condition1 = var_name not in all_variable_names
-                    condition2 = int(var_name[1:]) < 0
-                    if condition1 != condition2:
-                        print(var_name, all_variable_names)
-                        print(r_chain)
-                        exit(-12345)
-                    if condition1:
-                        assert i_relation + 1 >= starting_index
-                        fresh_variables_chain = fresh_variables_chains[
-                            i_relation - (starting_index - 1)]
-                        # not seen in this chain also?
-                        if var_name not in temp_to_fix_name:
-                            # we see this name for the first time --> rename from temp name
-                            new_var_name = self.generate_next_var_name(
-                                var_name[0])
-                            # set the value of constant variables
-                            is_const1 = var_name in const_name_to_value
-                            is_const2 = var_name[0] == "C"
-                            assert is_const1 == is_const2
-                            value = const_name_to_value[
-                                var_name] if is_const2 else None
-                            new_var = create_new_variable(
-                                new_var_name, var_type, value)
-                            if var_type not in fresh_variables_chain:
-                                fresh_variables_chain[var_type] = set()
-                            fresh_variables_chain[var_type].add(new_var)
-                            temp_to_fix_name[var_name] = new_var_name
-                            fresh_variables[new_var_name] = new_var
-                        else:
-                            new_var_name = temp_to_fix_name[var_name]
-                    else:
-                        new_var_name = var_name
-                    new_names.append(new_var_name)
-                split_test.append((r, new_names, a))
-            self.all_variables.update(fresh_variables)
-            fresh_variables_names = set(fresh_variables.keys())
-            self.reset_temp_var_count()
-            # set the split
-            bs = BinarySplit(split_test, comparator, theta, True,
-                             is_variable_free)
-            bs.add_fresh_variables(fresh_variables)
-            current_node.set_split(bs)
-            # branch frequencies
-            nb_examples = target_data_weight(target_data)
-            branch_frequencies = [
-                target_data_weight(target_data, part) / nb_examples
-                for part in partition
-            ]
-            current_node.get_stats().set_branch_frequencies(branch_frequencies)
-            # create children etc.
-            current_variables_children = [
-                current_vars_per_type[:starting_index] +
-                fresh_variables_chains, current_vars_per_type
-            ]
-            # print("variables before/fresh after inducing", current_node.description)
-            # print(all_variable_names, fresh_variables_names)
-            for i, part in enumerate(partition):
-                assert i < 2
-                label = current_node.description + ".{}".format(i)
-                child = TreeNode(label, current_node, [], None, None,
-                                 current_node.get_depth() + 1)
-                current_node.add_child(child)
-                target_data_child = [target_data[i] for i in part]
-                self.initialize_statistics(child, target_data_child)
-                current_variables_child = current_variables_children[i]
-                all_variable_names_child = all_variable_names | fresh_variables_names if i == 0 else all_variable_names
-                self.build_helper(target_data_child, child,
-                                  current_variables_child,
-                                  target_relation_vars,
-                                  all_variable_names_child)
-        else:
-            current_node.get_stats().create_predictions()
-
-    def should_try_find_a_split(self, current_node: TreeNode,
-                                target_data: List[Datum]):
-        if current_node.get_depth() >= self.max_depth:
-            return False
-        elif self.current_number_internal_nodes >= self.max_number_internal_nodes:
-            return False
-        elif target_data_weight(
-                target_data
-        ) <= 2 * self.minimal_examples_in_leaf - DecisionTree.eps:
-            return False
-        elif current_node.get_stats(
-        ).variability < DecisionTree.eps * self.root_node.get_stats(
-        ).variability:
-            # print("Variability too low: ", self.heuristic.compute_variability(current_node.get_stats()))
-            return False
-        else:
-            return True
-
-    def evaluate_candidate_splits(self, parent, test_values, target_data,
-                                  target_relation_vars, filtered_output_types):
-        n_aggregators = len(test_values[0])
-        best_score = BinarySplit.worst_split_score
-        best_configuration = None
-        for i in range(n_aggregators):
-            xs = [x[i] for x in test_values]
-            if filtered_output_types[i] == TYPE_NUMERIC:  # is numeric
-                t0 = clock()
-                score, comparator, theta, partition = self.find_best_numeric(
-                    parent, xs, target_data)
-                is_variable_free = True
-                t1 = clock()
-                self.numeric_tests += 1
-                self.numeric_tests_time += t1 - t0
-            else:  # is nominal: 'constant' or user defined type
-                t0 = clock()
-                output_type = filtered_output_types[i]
-                if output_type in target_relation_vars:
-                    var_candidates = sorted(
-                        [v.name for v in target_relation_vars[output_type]])
-                else:
-                    var_candidates = []
-                score, comparator, theta, partition, is_variable_free = self.find_best_nominal(
-                    parent, xs, target_data, var_candidates, output_type)
-                t1 = clock()
-                self.nominal_tests_time += t1 - t0
-            if BinarySplit.is_better_than_previous(score, best_score):
-                best_score = score
-                best_configuration = (i, comparator, theta, partition,
-                                      is_variable_free)
-        return best_score, best_configuration
-
-    def find_best_nominal(self, parent: TreeNode, xs: List[str], target_data: List[Datum],
-                          target_relation_vars: List[str], output_type: str, max_set_size=5) \
-            -> Tuple[float, Comparator, Set[str], List[List[int]], bool]:
-        if self.only_existential:
-            raise ValueError(
-                "Only existential tests cannot leave to nominal tests.")
-        is_usual_nominal = Relation.is_nominal_type(output_type)
-        if is_usual_nominal:
-            different_values = sorted(set(
-                xs))  # better than list, so that the order is always the same
-            different_values_helper = []
-            target_relation_var_indices = []
-        else:
-            different_values_helper = target_relation_vars
-            different_values = list(range(len(different_values_helper)))
-            target_relation_var_indices = [
-                int(v[1:]) for v in target_relation_vars
-            ]
-        n = len(different_values)
-        m = min(n, max_set_size)
-        if is_usual_nominal:
-            options = 2**(
-                m - 1
-            )  # Half of them suffice, empty set skipped later if necessary
-        else:
-            # Possible values are:
-            # - value of (at least one of) the target variable(s)
-            # - something else (including MODE_OF_EMPTY_LIST)
-            # We implicitly skip all the subsets of the form {'something else', ...},
-            # so we have to generate 2 ** m options (-1 for the empty one).
-            options = 2**m
-        if n > max_set_size:
-            # message = "Warning: Nominal split: Too many subsets of a set with size = {}." \
-            #           " Will evaluate {} randomly chosen ones."
-            # print(message.format(n, options))
-            subsets = random_subsets(different_values, options)
-        else:
-            subsets = subsets_of_list(different_values, options)
-            next(subsets)  # skip the empty set
-        best_score = BinarySplit.worst_split_score
-        best_comparator = None
-        best_subset = None
-        best_partition = None
-        generic_statistic = self.target_data_stat.__class__.construct_from_parent(
-            parent.get_stats())
-        left = []  # to prevent "unbound" warnings
-        for left_list, _ in subsets:
-            self.nominal_tests += 1
-            if is_usual_nominal:
-                left = set(left_list)
-            partition = [[], []]  # type: List[List[int]]
-            statistics = [
-                generic_statistic.get_copy() for _ in range(len(partition))
-            ]
-            for datum_in, (test_value,
-                           datum) in enumerate(zip(xs, target_data)):
-                j = 1
-                if is_usual_nominal:
-                    if test_value in left:
-                        j = 0
-                else:
-                    for chosen in left_list:
-                        if datum.descriptive_part[target_relation_var_indices[
-                                chosen]] == test_value:
-                            j = 0
-                            break
-                partition[j].append(datum_in)
-                statistics[j].add_example_during_split_eval(datum)
-            # update all stats
-            for sta in statistics:
-                sta.after_split_evaluation_update()
-            if self.is_split_valid(statistics):
-                score = self.heuristic.evaluate_split(parent.get_stats(),
-                                                      statistics)
-            else:
-                score = BinarySplit.worst_split_score
-            if BinarySplit.is_better_than_previous(score, best_score):
-                best_score = score
-                best_partition = partition
-                transpose_branches = DecisionTree.should_transpose_branches(
-                    statistics)
-                if transpose_branches:
-                    # best_partition = best_partition[::-1]
-                    best_comparator = DOES_NOT_CONTAIN
-                else:
-                    best_comparator = CONTAINS
-                if is_usual_nominal:
-                    best_subset = left  # right if transpose_branches else left
-                else:
-                    best_subset = {
-                        different_values_helper[chosen]
-                        for chosen in left_list
-                    }
-        return best_score, best_comparator, best_subset, best_partition, is_usual_nominal
-
-    def find_best_numeric(self, parent: TreeNode, xs: List[float], target_data: List[Datum]) \
-            -> Tuple[float, Comparator, float, List[List[int]]]:
-        n = len(xs)
-        sorted_indices = sorted(range(n), key=lambda t: xs[t])
-        best_score = BinarySplit.worst_split_score
-        best_comparator = SMALLER
-        best_threshold = -float('inf')
-        best_i = None
-        best_partition = None
-        transpose_branches = None
-        generic_statistic = self.target_data_stat.__class__.construct_from_parent(
-            parent.get_stats())
-        statistics = [generic_statistic,
-                      parent.get_stats().get_copy()
-                      ]  # type: List[NodeStatistics]
-        previous_value = xs[sorted_indices[0]]
-        if self.only_existential:
-            # The only possible test is x > 0, so the xs are converted into ones and zeros
-            min_x, max_x = xs[sorted_indices[0]], xs[sorted_indices[-1]]
-            if min_x < 0 or max_x == float("inf"):
-                message = "Counting should result in numbers from [0, inf). Your range: [{}, {}]"
-                raise ValueError(message.format(min_x, max_x))
-            # modify: 0 --> 0 and > 0 --> 1 to ensure only one test below
-            xs_modified = xs[:]
-            for i in range(n):
-                xs_modified[i] = 0 if xs[i] == 0 else 1
-        else:
-            xs_modified = xs
-
-        for i in range(n):
-            datum = target_data[sorted_indices[i]]
-            x = xs_modified[sorted_indices[i]]
-            if x > previous_value:
-                if x < float('inf'):
-                    if previous_value > float('-inf'):
-                        threshold = previous_value + (
-                            x - previous_value) / 2  # element of (previous, x)
-                    else:
-                        threshold = x - 21.21  # element of (-inf, x)
-                else:
-                    threshold = previous_value + 21.21  # element of (previous, inf)
-                previous_value = x
-                if self.is_split_valid(statistics):
-                    score = self.heuristic.evaluate_split(
-                        parent.get_stats(), statistics)
-                else:
-                    score = BinarySplit.worst_split_score
-                if BinarySplit.is_better_than_previous(score, best_score):
-                    best_score = score
-                    best_threshold = threshold
-                    best_i = i
-                    transpose_branches = DecisionTree.should_transpose_branches(
-                        statistics)
-            statistics[TreeNode.
-                       negative_branch].remove_example_during_split_eval(datum)
-            statistics[TreeNode.positive_branch].add_example_during_split_eval(
-                datum)
-        if BinarySplit.is_better_than_previous(best_score,
-                                               BinarySplit.worst_split_score):
-            best_partition = [sorted_indices[:best_i], sorted_indices[best_i:]]
-        if transpose_branches:
-            best_comparator = BIGGER
-            best_partition = best_partition[::-1]
-        return best_score, best_comparator, best_threshold, best_partition
-
-    def is_split_valid(self, stats: List[NodeStatistics]):
-        for stat in stats:
-            if stat.get_total_number_examples(
-            ) <= self.minimal_examples_in_leaf - DecisionTree.eps:
-                return False
-        return True
-
-    @staticmethod
-    def should_transpose_branches(statistics: List[NodeStatistics]):
-        weight_positive = statistics[0].get_total_number_examples()
-        weight_negative = statistics[1].get_total_number_examples()
-        return weight_positive < weight_negative
-
-    def generate_possible_attributes(self, current_var_names,
-                                     current_atom_tests,
-                                     target_relation_vars: List[str]):
-        # Forward: generate chain of new atom tests
-        # Backward: generated possible aggregator combinations
-        # print("generating attr's from ", current_var_names, current_atom_tests, sep="\n")
-        if len(current_atom_tests) < self.longest_atom_test_chain:
-            # reset everything
-            current_atom_tests = []
-            current_var_names = current_var_names[:1]
-
-        if len(current_var_names) - 1 != len(current_atom_tests):
-            raise WrongValueException(
-                "Lengths do not differ by one::\n{}\n{}".format(
-                    current_var_names, current_atom_tests))
-        var_names_up_to_here = {}
-        current_atom_tests_modified = []
-
-        for r, vs, a in current_atom_tests:
-            current_atom_tests_modified.append(
-                (r.get_name(), list(zip(vs, r.get_types()))))
-        for start_index in range(1, 1 + len(current_var_names)):
-            var_names_up_to_here = union_of_two_dicts(
-                var_names_up_to_here, current_var_names[start_index - 1])
-            test_chain = current_atom_tests_modified[:start_index - 1]
-            for new_tests_chain in self.generate_possible_attributes_helper_all_steps(
-                    1, var_names_up_to_here):
-                created_chain = test_chain + new_tests_chain
-                if is_relation_chain_valid(created_chain):
-                    fresh_v, fresh_i = DecisionTree.fresh_in_last_relation(
-                        created_chain, target_relation_vars)
-                    aggregator_chains = self.generate_possible_aggregator_chains(
-                        len(created_chain), fresh_v, fresh_i)
-                    yield start_index, created_chain, aggregator_chains, (
-                        set(fresh_v), fresh_i)
-
-    @staticmethod
-    def fresh_in_last_relation(tests_chain, target_relation_vars):
-        # compute the last fresh variable(s)
-        last_fresh = []
-        last_fresh_indices = []
-        initial_var_names_set = set(target_relation_vars)
-        non_fresh = set()
-        for test in tests_chain[:-1]:
-            _, var_names_types = test
-            non_fresh |= set(var_names_types)
-        relation_name, var_names_types = tests_chain[-1]
-        for i, var_name_type in enumerate(var_names_types):
-            var_name, var_type = var_name_type
-            p0 = var_name[0] != "C"
-            p1 = var_name not in initial_var_names_set
-            p2 = var_name_type not in non_fresh
-            p3 = var_type != Settings.atom_test_type_constant
-            if p0 and p1 and p2 and p3:
-                last_fresh.append(var_name_type)
-                last_fresh_indices.append(i)
-        return last_fresh, last_fresh_indices
-
-    def generate_possible_aggregator_chains(self, tests_chain_len,
-                                            last_fresh_variables,
-                                            last_fresh_indices):
-        def last_step_helper(fresh: int, current_type: str):
-            if fresh == 0:
-                # In this case, the aggregate should return 0 from [0] and 1 from [1] --> sum suffices
-                options = []
-                is_complex = False
-            else:
-                if current_type == TYPE_TUPLE:
-                    options = COMPLEX_ENOUGH_AGGREGATORS
-                    is_complex = True
-                elif current_type == TYPE_NOMINAL:
-                    options = NOMINAL_AGGREGATORS
-                    is_complex = False
-                elif current_type == TYPE_NUMERIC:
-                    options = NUMERIC_AGGREGATORS
-                    is_complex = False
-                elif current_type == TYPE_TYPE:
-                    # some user defined type like Person, Atom etc.
-                    options = NOMINAL_AGGREGATORS
-                    is_complex = False
-                else:
-                    raise WrongValueException(
-                        "Unknown type: {}".format(current_type))
-            chosen = []
-            if is_complex and PROJECT.name in self.allowed_aggregators:
-                for i, var_index in enumerate(last_fresh_indices):
-                    chosen += [
-                        PROJECTIONS[var_index](o)
-                        for o in last_step_helper(1, last_super_types[i])
-                        if o.name != COUNT.name
-                    ]
-            chosen += [
-                a for a in options if a.name in self.allowed_aggregators
-                and a.name != PROJECT.name
-            ]
-            yield from chosen
-
-        def generator_chains_helper(current_options_gen, current_super_type,
-                                    current_types, position):
-            current_options = list(current_options_gen)
-            if force_use_sum[0]:
-                if len(current_options) == 0:
-                    current_options = {SUM}
-                else:
-                    force_use_sum[0] = False
-            for o in current_options:
-                next_super_type, next_types = get_out_type(
-                    current_super_type, current_types, o)
-                if position == 0:
-                    if o not in forbidden_first:
-                        yield [o], next_types[0]
-                else:
-                    i = None
-                    o_real = o.aggregator if o.is_projection else o
-                    for i, g in enumerate(groups):
-                        if o_real in g:
-                            break
-                    next_options = is_followed_by[next_super_type][i]
-                    for left_part, left_type in generator_chains_helper(
-                            next_options, next_super_type, next_types,
-                            position - 1):
-                        yield left_part + [o], left_type
-
-        def get_super_type(k, t):
-            """
-            :param k: number of variables that are considered
-            :param t: ignored if k != 1, variable type as given in relation definition in the settings.
-            :return: Type of (the group of) the fresh variables
-            """
-            # behaves as numeric if no fresh
-            # or precisely one which is numeric
-            if k == 0:
-                return TYPE_NUMERIC
-            elif k > 1:
-                return TYPE_TUPLE
-            else:
-                if t.startswith(Relation.constant_numeric):
-                    return TYPE_NUMERIC
-                elif t.startswith(Relation.constant_nominal):
-                    return TYPE_NOMINAL
-                else:
-                    # user defined
-                    return TYPE_TYPE
-
-        def get_out_type(current_super_type, current_types,
-                         a: Union[Aggregator, Project]):
-            t = a.output_type
-            if current_super_type == TYPE_TUPLE:
-                # counting or projecting
-                if t == TYPE_NUMERIC:
-                    # counting, numeric projections
-                    return TYPE_NUMERIC, [
-                        TYPE_NUMERIC
-                    ]  # new type can be also simply numeric
-                elif t == TYPE_SAME_AS_INPUT:
-                    # nominal projection
-                    if not a.is_projection:
-                        raise ValueError("Should be projection")
-                    new_type = current_types[absolute_to_relative_positions[
-                        a.component]]
-                    new_super_type = get_super_type(1, new_type)
-                    return new_super_type, [new_type]
-                else:
-                    raise WrongValueException(
-                        "Wrong output type: {}".format(t))
-            else:
-                if t == TYPE_SAME_AS_INPUT:
-                    return current_super_type, current_types
-                elif t == TYPE_NUMERIC:
-                    return TYPE_NUMERIC, [
-                        TYPE_NUMERIC
-                    ]  # new type can be also simply numeric
-                else:
-                    raise WrongValueException(
-                        "Wrong output type: {}".format(t))
-
-        group0 = {MIN, MAX, MEAN, SUM}
-        group1 = {COUNT, COUNT_UNIQUE}
-        group2 = {MODE}
-        group3 = {FLATTEN, FLATTEN_UNIQUE}
-        groups = [[a for a in g if a.get_name() in self.allowed_aggregators]
-                  for g in [group0, group1, group2, group3]]
-        forbidden_first = {FLATTEN_UNIQUE, FLATTEN}
-        base_followed_dict = {
-            0: groups[0],
-            1: groups[0],
-            2: groups[1] + groups[2] + groups[3]
-        }
-        is_followed_by_numeric = {x: y for x, y in base_followed_dict.items()}
-        is_followed_by_nominal = {x: y for x, y in base_followed_dict.items()}
-        is_followed_by_tuple = {x: y for x, y in base_followed_dict.items()}
-        is_followed_by_type = {x: y for x, y in base_followed_dict.items()}
-        # update with group3 followers
-        is_followed_by_numeric.update({3: groups[0] + groups[1] + groups[3]})
-        is_followed_by_nominal.update({3: groups[1] + groups[2] + groups[3]})
-        is_followed_by_tuple.update({3: groups[1] + groups[3]})
-        is_followed_by_type.update({3: groups[1] + groups[2] + groups[3]})
-        is_followed_by = {
-            TYPE_NUMERIC: is_followed_by_numeric,
-            TYPE_NOMINAL: is_followed_by_nominal,
-            TYPE_TUPLE: is_followed_by_tuple,
-            TYPE_TYPE: is_followed_by_type
-        }
-        last_types = [value_type for _, value_type in last_fresh_variables]
-        last_super_types = [
-            get_super_type(1, value_type)
-            for _, value_type in last_fresh_variables
-        ]
-        nb_fresh = len(set(last_fresh_variables))
-        last_fresh_type = None if nb_fresh != 1 else last_fresh_variables[0][1]
-        last_super_type = get_super_type(nb_fresh, last_fresh_type)
-        force_use_sum = [nb_fresh == 0
-                         ]  # to prevent initialisation in helping functions
-        absolute_to_relative_positions = {
-            a: r
-            for r, a in enumerate(last_fresh_indices)
-        }
-        yield from generator_chains_helper(
-            last_step_helper(nb_fresh, last_super_type), last_super_type,
-            last_types, tests_chain_len - 1)
-
-    def generate_possible_attributes_helper_all_steps(
-            self, depth, var_counts_up_to_here: Dict[str, Set[str]]):
-        for head in self.generate_possible_attributes_helper_one_step(
-                var_counts_up_to_here):
-            yield [head]
-            if depth < self.max_number_atom_tests:
-                # update counts
-                _, var_names_types = head
-                fresh_dict = {}  # type: Dict[str, Set[str]]
-                for var_name, var_type in var_names_types:
-                    if var_type not in fresh_dict:
-                        fresh_dict[var_type] = set()
-                    fresh_dict[var_type].add(var_name)
-                new_counts = union_of_two_dicts(var_counts_up_to_here,
-                                                fresh_dict)
-                for tail in self.generate_possible_attributes_helper_all_steps(
-                        depth + 1, new_counts):
-                    yield [head] + tail
-
-    def generate_possible_attributes_helper_one_step(self,
-                                                     var_counts_up_to_here):
-        for rel_spec in sorted(self.allowed_atom_tests):
-            counts = self.allowed_atom_tests[rel_spec]
-            relation_name, var_specifications, var_types = rel_spec
-            arity = len(var_specifications)
-            o_types = sorted(counts.keys())
-            for needed_keys, configuration in generate_variable_configurations(
-                    var_counts_up_to_here, counts, o_types):
-                assert len(configuration) == len(counts)  # one for each type
-                variable_names = [None for _ in range(arity)]
-                none_counter = arity
-                for type_config, o_type in zip(configuration, o_types):
-                    (ind_old, ind_new), (names_old,
-                                         relative_counts_new) = type_config
-                    # place old
-                    for i_old, n_old in zip(ind_old, names_old):
-                        assert variable_names[i_old] is None
-                        none_counter -= 1
-                        variable_names[i_old] = n_old
-                    # place new
-                    temp_new_var_names = self.generate_temp_var_names(
-                        "Y", relative_counts_new)
-                    for i_new, n_new in zip(ind_new, temp_new_var_names):
-                        assert variable_names[i_new] is None
-                        none_counter -= 1
-                        variable_names[i_new] = n_new
-                    # place constants
-                    for i_const in counts[o_type][2]:  # TODO: hard-coded 2 ...
-                        assert variable_names[i_const] is None
-                        none_counter -= 1
-                        variable_names[i_const] = self.generate_temp_var_name(
-                            "C")
-                assert none_counter == 0
-                var_names_types = list(zip(variable_names, var_types))
-                yield relation_name, var_names_types
-
-    def create_example_and_chains(self, relations, current_vars):
-        def const_value_generator(c_name):
-            r_name, position = constants[c_name]
-            yield from self.descriptive_data[r_name].get_all_values(position)
-
-        def num_const_values():
-            product = 1
-            for c_name in constant_var_names:
-                r_name, position = constants[c_name]
-                product *= self.descriptive_data[r_name].get_nb_all_values(
-                    position)
-            return product
-
-        relation_chain = []
-        example = {}
-        constants = {}
-        # current
-        for d in current_vars:
-            for vs in d.values():
-                for v in vs:
-                    n = v.get_name()
-                    assert n not in example
-                    example[n] = v
-        # extended
-        for relation_name, var_names in relations:
-            for i, (n, t) in enumerate(var_names):
-                if n not in example:
-                    if n[0] == "C":
-                        assert n not in example  # always fresh constant variables
-                        example[n] = ConstantVariable(n, t, None)
-                        constants[n] = (relation_name, i)
-                    elif n[0] in "XY" and n not in example:
-                        example[n] = VariableVariable(n, t, None)
-                    elif n[0] not in "CXY":
-                        raise WrongValueException(
-                            "Wrong variable name {}".format(n))
-            relation_chain.append((self.descriptive_data[relation_name],
-                                   [n for n, _ in var_names]))
-
-        constant_var_names = sorted(constants.keys())
-        c_values = itertools.product(
-            *[const_value_generator(c) for c in constant_var_names])
-        return example, relation_chain, c_values, constant_var_names, num_const_values(
-        )
-
-    def predict(self, d: Datum, is_for_ensemble=False):
-        example = {}  # type: Dict[str, Variable]
-        for var, value in zip(self.target_relation_variables,
-                              d.get_descriptive()):
-            example[var.get_name()] = var
-            var.set_value(value)
-        current_node = self.root_node  # type: TreeNode
-        while not current_node.is_leaf():
-            # extend the example
-            for name, var in current_node.get_split().get_fresh_variables(
-            ).items():
-                example[name] = var
-            # get test value and send example to one of the children
-            is_positive = current_node.get_split().evaluate(example)
-            if is_positive:
-                current_node = current_node.get_child(TreeNode.positive_branch)
-            else:
-                current_node = current_node.get_child(TreeNode.negative_branch)
-        if is_for_ensemble:
-            prediction = current_node.get_stats().get_prediction_for_ensemble()
-        else:
-            prediction = current_node.get_stats().get_prediction()
-        for var in example.values():
-            if var.can_vary():
-                var.unset_value()
-        return prediction
-
-    def predict_all(self, ds: List[Datum], is_for_ensemble=False):
-        return [self.predict(d, is_for_ensemble) for d in ds]
-
-    def target_data_induction_preparation(self, target_data: List[Datum]):
-        if self.class_weights is None:
-            return None
-        for d in target_data:
-            d.set_weight(d.get_weight() * self.class_weights[d.get_target()])
-
-    def reverse_target_data_induction_preparation(self,
-                                                  target_data: List[Datum]):
-        if self.class_weights is None:
-            return None
-        for d in target_data:
-            d.set_weight(d.get_weight() / self.class_weights[d.get_target()])
-
-    @staticmethod
-    def populate_dict(target_data: List[Datum]):
-        for datum in target_data:
-            if datum.identifier not in TEST_VALUE_MEMO:
-                TEST_VALUE_MEMO[datum.identifier] = {}
-
-    @staticmethod
-    def test_values_memo_keys(example: Dict[str, Variable],
-                              relation_chain: List[Tuple[Relation, List[str]]],
-                              aggregation_chains: List[Tuple[Aggregator]]):
-        """
-
-        :param example:
-        :param relation_chain:
-        :param aggregation_chains:
-        :return: A 3-tuple: (relations_as_key, aggregators_as_keys, known_unknown_separated) where
-        - relations_as_key: (relation name, known_unknown, values) where
-            - relation name: str
-            - known_unknown: [is value known for variable1, ...]
-            - values:
-                - if variable is set to some value, then this equals its value
-                - elif variable is input variable, i.e., starts with 'X': name of the variable
-                - else: an integer
-        - aggregators_as_keys: tuple of tuples of aggregator names
-        - known_unknown_separated: indices of the variables with (un)known values
-        """
-        parts = []
-        known_unknown_separated = []
-        counters = {}
-        max_overall = -1
-        for r_vs in relation_chain:
-            r, vs = r_vs
-            known_unknown = []
-            known_unknown_separated_part = [[], []]  # type: List[List[int]]
-            out_values = []
-            max_part = -1
-            for i, v in enumerate(vs):
-                u = example[v].is_unset(
-                )  # target variables should not be set here yet
-                known_unknown.append(not u)
-                if u:
-                    if v[0] == 'X':
-                        out_values.append(v)
-                        known_unknown_separated_part[0].append(
-                            i)  # but are considered known
-                    else:
-                        if v not in counters:
-                            counters[v] = len(counters)
-                        value = counters[v]
-                        out_values.append(value)
-                        if value <= max_overall:
-                            known_unknown_separated_part[0].append(
-                                i)  # seen in the previous parts
-                        else:
-                            known_unknown_separated_part[1].append(
-                                i)  # unknown until this part
-                        max_part = max(max_part, value)
-                else:
-                    # assert v[0] != "X"
-                    out_values.append(example[v].get_value())
-                    known_unknown_separated_part[0].append(i)  # known
-            parts.append((r.name, tuple(known_unknown), tuple(out_values)))
-            max_overall = max(max_part, max_overall)
-            known_unknown_separated.append(known_unknown_separated_part)
-        relations_as_key = tuple(parts)
-        aggregators_as_keys = [
-            tuple(a.name for a in a_s) for a_s in aggregation_chains
-        ]
-        return relations_as_key, aggregators_as_keys, known_unknown_separated
-
-
-def is_relation_chain_valid(chain: List[Tuple[str, List[Tuple[str, str]]]]):
-    """
-    We check whether
-    0) At least one of the fresh (Y) variables in the relation r_i is used in r_{i + 1}
-    1) 2nd, 3rd, ... relation contains at least one variable from the previous relation.
-    2) no two elements are equal
-    :param chain: [(rel1, var_name_types1), ...], var_name_types1 = [('Y2', 'Person'), ...]
-    :return:
-    """
-    # 0)
-    for i in range(len(chain) - 1):
-        link_ok = True
-        has_fresh = False
-        for name, _1 in chain[i][1]:
-            if name[0] == "Y":
-                has_fresh = True
-                link_ok = False
-                for next_name, _2 in chain[i + 1][1]:
-                    if name == next_name:
-                        link_ok = True
-                        break
-            if has_fresh and link_ok:
-                break
-        if not link_ok:
-            return False
-    # 1)
-    for i in range(1, len(chain)):
-        link_ok = False
-        for name, _1 in chain[i][1]:
-            for prev_name, _2 in chain[i - 1][1]:
-                if prev_name == name:
-                    link_ok = True
-                    break
-            if link_ok:
-                break
-        if not link_ok:
-            return False
-    # 2)
-    chain_copy = chain[::]
-    chain_copy.sort()
-    for i in range(1, len(chain)):
-        if chain_copy[i] == chain_copy[i - 1]:
-            return False
-    return True
-
-
-def generate_variable_configurations(present, needed, needed_keys):
-    def generate_config_one_type(p, n):
-        old, new, _ = n
-        for additional_old, brand_new in subsets_of_list(new):
-            true_old = old + additional_old
-            true_new = brand_new  # new + brand_new?
-            old_configs = generalized_counting(
-                sorted(p), len(true_old))  # [['X1', 'X2', 'X1'], ...]
-            new_configs = canonic_sequences_of_new_variables(
-                len(true_new))  # [[1, 3, 2, 1], ...]
-            for combo in itertools.product(old_configs, new_configs):
-                yield (true_old, true_new), combo
-
-    # extend present with empty lists
-    for t in needed_keys:
-        if t not in present:
-            present[t] = set()
-    pairs = [(present[t], needed[t]) for t in needed_keys]
-    # cartesian product over the types
-    for combined in itertools.product(
-            *[generate_config_one_type(p, n) for p, n in pairs]):
-        yield needed_keys, combined
-
-
-def random_subsets(a_list, nb_subsets, random_seed=None):
-    if random_seed is not None:
-        random.seed(random_seed)
-    for _ in range(nb_subsets):
-        left_right = [[], []]
-        for x in a_list:
-            left_right[random.random() > 0.5].append(x)
-        yield left_right
-
-
-def create_new_variable(v_name, v_type, value=None):
-    if v_name[0] == "C":
-        return ConstantVariable(v_name, v_type, value)
-    elif v_name[0] in "XY":
-        return VariableVariable(v_name, v_type, value)
-    elif v_name[0] not in "CXY":
-        raise WrongValueException("Wrong variable name {}".format(v_name))
-
-
-def create_constant_tree(heuristic: Heuristic, data: Dataset):
-    t = DecisionTree(heuristic=heuristic, max_number_internal_nodes=0)
-    t.build(data)
-    return t
+from typing import Iterable, Union
+from .core.aggregators import *
+from .core.comparators import *
+from .core.tree_node_split import BinarySplit
+from .core.heuristic import Heuristic
+from ..data.data_and_statistics import *
+from ..data.task_settings import Settings
+from .core.variables import *
+from ..data.relation import Relation
+from ..utilities.my_exceptions import WrongValueException
+from ..utilities.my_utils import *
+import itertools
+import random
+from .predictive_model import PredictiveModel
+import time
+import math
+import copy
+from .core.tree_node_split import TEST_VALUE_MEMO
+# from my_memo import used_comp_memo
+import subprocess
+from .core.communicate_with_java import send_data, send_variables, compute_test_values
+from py4j.java_gateway import JavaGateway, GatewayParameters
+
+
+class TreeNode:
+    positive_branch = 0
+    negative_branch = 1
+
+    def __init__(self, description, parent, children,
+                 binary_split: Union[BinarySplit, None],
+                 stats: Union[NodeStatistics, None], depth: int):
+        self.description = description
+        self.parent = parent  # type: 'TreeNode'
+        self.children = children
+        self.split = binary_split  # type: BinarySplit
+        self.stats = stats  # type: NodeStatistics
+        self.depth = depth
+
+    def get_parent(self) -> 'TreeNode':
+        return self.parent
+
+    def get_split(self):
+        return self.split
+
+    def set_depth(self, d):
+        self.depth = d
+
+    def get_depth(self):
+        return self.depth
+
+    def set_split(self, s):
+        self.split = s
+
+    def set_parent(self, other):
+        self.parent = other
+
+    def get_child(self, i):
+        return self.children[i]
+
+    def get_children(self):
+        return self.children
+
+    def add_child(self, other):
+        self.add_children([other])
+
+    def add_children(self, others):
+        if self.children is None:
+            self.children = []
+        self.children += others
+
+    def is_leaf(self):
+        return len(self.children) == 0
+
+    def get_stats(self):
+        return self.stats
+
+    def set_stats(self, s):
+        self.stats = s
+
+
+class DecisionTree(PredictiveModel):
+    root_node_depth = 1
+    eps = 10**-10
+    left_child_indicator = "0"
+    right_child_indicator = "1"
+    root_indicator = "root"
+
+    square_root = "sqrt"
+    log2 = "log"
+    allowed_n_tests = [square_root, log2]
+
+    def __init__(
+            self,
+            heuristic=None,
+            statistics=None,
+            root_node=None,
+            max_number_internal_nodes=float('inf'),
+            max_number_atom_tests=1,
+            allowed_atom_tests=None,
+            allowed_aggregators: Union[None, Iterable[str]] = None,
+            max_depth=float("inf"),
+            minimal_examples_in_leaf=1,
+            max_number_of_evaluated_tests_per_node=float("inf"),
+            max_relative_number_of_evaluated_tests_per_node: Union[float,
+                                                                   str] = 1.0,
+            random_seed=2718281828,
+            java_port: Union[None, int] = None,
+            is_outer_java=False,
+            longest_atom_test_chain=4,
+            class_weights: Union[None, Dict[str, float]] = None,
+            per_class_bootstrap=False,
+            only_existential=False,
+            minimal_impurity=10**-16):
+        self.heuristic = Heuristic() if heuristic is None else heuristic
+        self.target_data_stat = statistics
+        self.max_number_internal_nodes = max_number_internal_nodes
+        self.max_number_atom_tests = max_number_atom_tests
+        self.allowed_atom_tests = {} if allowed_atom_tests is None else allowed_atom_tests  # the structured version
+        self.allowed_aggregators = set(
+        ) if allowed_aggregators is None else set(allowed_aggregators)
+        self.max_depth = max_depth
+        self.minimal_examples_in_leaf = minimal_examples_in_leaf
+        self.max_number_of_evaluated_tests_per_node = max_number_of_evaluated_tests_per_node
+        self.max_relative_number_of_evaluated_tests_per_node = max_relative_number_of_evaluated_tests_per_node
+        self.relative_number_tests_sanity_check()
+        self.random_seed = random_seed
+        self.java_port = java_port
+        self.is_outer_java = is_outer_java
+        self.longest_atom_test_chain = longest_atom_test_chain
+        self.class_weights = class_weights
+        self.per_class_bootstrap = per_class_bootstrap
+        self.only_existential = only_existential
+        self.update_allowed_aggregates()
+        self.minimal_impurity = minimal_impurity  # relative
+
+        self.root_node = root_node  # type: Union['TreeNode', None]
+        self.target_relation_description = None
+        # tree building fields
+        self.target_relation_variables = []  # type: List[Variable]
+        self.descriptive_data = {}  # type: Dict[str, Relation]
+        self.var_count = {"XY": 0, "C": 0}  # TODO: less hard-coded?:)
+        self.temp_var_count = 0
+        self.current_number_internal_nodes = 0
+        self.all_variables = {}
+        self.induce_tree_time = 0.0
+        self.statistics_time = 0.0
+        self.get_test_value_time = 0.0
+        self.split_eval_time = 0.0
+        self.set_example_values_time = 0.0
+        self.find_values_time = 0.0
+        self.nominal_tests = 0
+        self.nominal_tests_time = 0
+        self.numeric_tests = 0
+        self.numeric_tests_time = 0
+
+        self.p = None
+        self.wrapper = None
+        self.client = None
+        self.gateway = None
+
+    def print_times(self):
+        times = [
+            self.induce_tree_time, self.statistics_time,
+            self.get_test_value_time, self.split_eval_time,
+            self.set_example_values_time, self.find_values_time,
+            self.nominal_tests, self.nominal_tests_time, self.numeric_tests,
+            self.numeric_tests_time
+        ]
+        names = [
+            "induce", "statistics", "test value", "eval split",
+            "example values", "find values", "nominal tests", "nom. t. time",
+            "numeric tests", "num t. time"
+        ]
+        for time, name in zip(times, names):
+            print("{: <14}:".format(name), time)
+        print()
+
+    def __str__(self):
+        def helper(node: TreeNode):
+            branches_names = ["YES", "NO"]
+            spaces = "  " * node.get_depth()
+            if node.is_leaf():
+                return "{}{}".format(spaces, node.get_stats())
+            else:
+                parts = [
+                    "{}IF {}:".format(spaces,
+                                      node.split.__str__(self.all_variables))
+                ]
+                for b_name, child in zip(branches_names, node.children):
+                    parts.append("{}{}".format(spaces, b_name))
+                    parts.append(helper(child))
+                return "\n".join(parts)
+
+        header = "Tree for {}:".format(self.target_relation_description)
+        tree = helper(self.root_node)
+        return "\n".join([header, tree])
+
+    def __iter__(self):
+        """
+        Iterates over the nodes in the tree: yields root, then 'recursively' visits the left and the right subtree.
+        :return:
+        """
+        if self.root_node is not None:
+            stack = [self.root_node]
+            while stack:
+                node = stack.pop()
+                yield node
+                stack += node.get_children()[::-1]
+
+    def dump_to_text(self, file_name):
+        f = open(file_name, "w")
+        print(str(self), file=f)
+        f.close()
+
+    def get_absolute_number_tests_from_relative(self, nb_tests):
+        n_rel = self.max_relative_number_of_evaluated_tests_per_node
+        if isinstance(n_rel, str):
+            if n_rel == DecisionTree.square_root:
+                return round(math.sqrt(nb_tests))
+            elif n_rel == DecisionTree.log2:
+                return round(math.log2(nb_tests))
+            else:
+                raise ValueError("Wrong function: {}".format(n_rel))
+        elif isinstance(n_rel, float):
+            return round(n_rel * nb_tests)
+        else:
+            raise ValueError(
+                "Wrong relative number of tests: {}.".format(n_rel))
+
+    def relative_number_tests_sanity_check(self):
+        if isinstance(self.max_relative_number_of_evaluated_tests_per_node,
+                      str):
+            if self.max_relative_number_of_evaluated_tests_per_node not in DecisionTree.allowed_n_tests:
+                message = "Wrong number of tests: {}. If string, it should be an element of {}"
+                raise ValueError(
+                    message.format(
+                        self.max_relative_number_of_evaluated_tests_per_node,
+                        DecisionTree.allowed_n_tests))
+        elif isinstance(self.max_relative_number_of_evaluated_tests_per_node,
+                        float):
+            if not (0.0 <= self.max_relative_number_of_evaluated_tests_per_node
+                    <= 1):
+                message = "Wrong relative number of tests: {}. If float, should be in the interval (0, 1]"
+                raise ValueError(
+                    message.format(
+                        self.max_relative_number_of_evaluated_tests_per_node))
+        else:
+            raise ValueError(
+                "Relative number of tests should be string or float.")
+
+    def chosen_tests(self, tests_generator, current_vars_per_type):
+        nb_tests = 0
+        nb_chains = 0
+        for jj, chain in enumerate(tests_generator):
+            # if jj % 10**2 == 0:
+            #     print("-", end="")
+            # if jj % 10**4 == 0:
+            #     print()
+            nb_chains += 1
+            _, relation_chain, aggregator_chains, _ = chain
+            # print(relation_chain)
+            num_aggregator_chains = len(list(aggregator_chains))
+            _, _, _, _, c_num = self.create_example_and_chains(
+                relation_chain, current_vars_per_type)
+            nb_tests += num_aggregator_chains * c_num
+        # print()
+        k_proportion = self.get_absolute_number_tests_from_relative(nb_tests)
+        k_absolute = self.max_number_of_evaluated_tests_per_node
+        k = min(k_proportion,
+                k_absolute)  # Select the more restrictive criterion
+        k = max(k, 1)  # but at least one
+        k = min(k, nb_tests)  # but at most all tests
+        return set(random.sample(range(nb_tests), k=k)), nb_tests, nb_chains
+
+    def generate_next_var_name(self, first_letter):
+        key = None
+        if first_letter == "C":
+            key = "C"
+        elif first_letter in "XY":
+            key = "XY"
+        c = self.var_count[key]
+        self.var_count[key] += 1
+        return "{}{}".format(first_letter, c)
+
+    def generate_temp_var_name(self, first_letter):
+        return self.generate_temp_var_names(first_letter, [1])[0]
+
+    def generate_temp_var_names(self, first_letter, offsets):
+        names = [
+            "{}{}".format(first_letter, self.temp_var_count - offset)
+            for offset in offsets
+        ]
+        if names:
+            self.temp_var_count -= max(offsets)
+        return names
+
+    def reset_temp_var_count(self):
+        self.temp_var_count = 0
+
+    @staticmethod
+    def get_first_var_letter(object_type, is_input):
+        if object_type == Settings.atom_test_type_constant:
+            return "C"
+        elif is_input:
+            return "X"
+        else:
+            return "Y"
+
+    def initialize_statistics(self, node: TreeNode, data: List[Datum]):
+        t0 = time.time()
+        statistics_class = self.target_data_stat.__class__
+        initial_stats = statistics_class.construct_from_parent(
+            self.target_data_stat)
+        initial_stats.add_examples(data)
+        node.set_stats(initial_stats)
+        variability = self.heuristic.compute_variability(node.get_stats())
+        node.get_stats().set_variability(variability)
+        t1 = time.time()
+        self.statistics_time += t1 - t0
+
+    def fit(self, data: Dataset):
+        t0 = time.time()
+        random.seed(self.random_seed)
+        self.target_data_stat = data.get_copy_statistics()
+        target_relation = data.get_target_relation()  # no examples - ok?
+        self.descriptive_data = data.get_descriptive_data(
+        )  # type: Dict[str, Relation]
+        target_data = data.get_target_data()  # type: List[Datum]
+        if BinarySplit.use_memo:
+            DecisionTree.populate_dict(target_data)
+        current_vars_per_type = [{}]  # type: List[Dict[str, Set[Variable]]]
+        target_var_names = []
+        self.target_relation_variables = []  # type: List[Variable]
+        for object_type in target_relation.get_types()[:-1]:
+            var_name = self.generate_next_var_name(
+                DecisionTree.get_first_var_letter(object_type, True))
+            assert not var_name.startswith("C")
+            new_var = VariableVariable(var_name, object_type, None)
+            if object_type not in current_vars_per_type[-1]:
+                current_vars_per_type[-1][object_type] = set()
+            current_vars_per_type[-1][object_type].add(new_var)
+            self.target_relation_variables.append(new_var)
+            target_var_names.append(new_var.get_name())
+
+        self.target_relation_description = "{}, {}".format(
+            target_relation.get_name(), target_var_names)
+        all_variable_names = set(target_var_names)
+        self.root_node = TreeNode(DecisionTree.root_indicator, None, [], None,
+                                  None, DecisionTree.root_node_depth)
+        # initial statistics
+        self.initialize_statistics(self.root_node, target_data)
+
+        if self.java_port is not None:
+            self.java_on()
+
+        if self.java_port is not None:
+            send_data(data, self.client, self.wrapper)
+
+        # manipulate target data
+        self.target_data_induction_preparation(target_data)
+        self.build_helper(target_data, self.root_node, current_vars_per_type,
+                          target_var_names, all_variable_names)
+        # un-manipulate target data
+        self.reverse_target_data_induction_preparation(target_data)
+
+        for v in self.target_relation_variables:
+            assert v.can_vary()
+            v.unset_value()
+        for v in self.target_relation_variables:
+            self.all_variables[v.get_name()] = v
+        t1 = time.time()
+        self.induce_tree_time = t1 - t0
+        self.print_times()
+        # s = max(1, sum(used_comp_memo))
+        # print("Memo vs. compute: {:.4f} : {:.4f}; all: {}".format(used_comp_memo[0] / s,
+        #                                                           used_comp_memo[1] / s,
+        #                                                           s))
+        # used_comp_memo[0] = 0
+        # used_comp_memo[1] = 0
+
+        if self.java_port is not None:
+            self.java_off()
+
+    def java_on(self):
+        if not self.is_outer_java:
+            # open server
+            this_dir = os.path.dirname(os.path.abspath(__file__))
+            path = os.path.join(this_dir, "core", "speedUp.jar")
+            if not os.path.exists(path):
+                path = "speedUp.jar"
+            self.p = subprocess.Popen(r"java -jar {} {}".format(
+                path, self.java_port),
+                                      shell=True)
+            for counter in range(10**8):
+                _ = 21 + 21
+        gateway_parameters = GatewayParameters(port=self.java_port)
+        self.gateway = JavaGateway(gateway_parameters=gateway_parameters)
+        self.wrapper = self.gateway.entry_point.get_wrapper()
+        self.client = self.gateway._gateway_client
+
+    def java_off(self):
+        if not self.is_outer_java:
+            self.gateway.shutdown()
+            self.p.kill()
+        self.wrapper = None
+        self.client = None
+        self.gateway = None
+        self.p = None
+
+    def update_allowed_aggregates(self):
+        if self.only_existential:
+            self.allowed_aggregators = {COUNT.get_name()}
+            print(
+                "Existential tests only ==> The allowed aggregates changed to {}"
+                .format(self.allowed_aggregators))
+
+    def build_helper(self, target_data: List[Datum], current_node: TreeNode,
+                     current_vars_per_type, target_relation_vars,
+                     all_variable_names: Set[str]):
+        # print("Current vars before inducing", current_node.description)
+        # print("cur_ver_per_type, all_names", current_vars_per_type, all_variable_names)
+        print("{}Building node on depth {}".format(
+            "  " * current_node.get_depth(), current_node.get_depth()))
+        current_var_names = [{
+            t: {v.get_name()
+                for v in vs}
+            for t, vs in d.items()
+        } for d in current_vars_per_type]
+        # print("curr var names", current_var_names)
+        # find a split
+        bs = BinarySplit([], None, None, True, None)
+        best_score = BinarySplit.worst_split_score
+        best_configuration = (None, None, None, None, None, None)
+        if self.should_try_find_a_split(current_node, target_data):
+            parents_test = []
+            node = current_node
+            while node.parent is not None:
+                if node == node.get_parent().children[0]:
+                    parents_test = node.get_parent().get_split().get_test()
+                    break
+                node = node.get_parent()
+            attributes_counting = self.generate_possible_attributes(
+                copy.deepcopy(current_var_names), parents_test,
+                target_relation_vars)
+            self.reset_temp_var_count()
+            attributes = self.generate_possible_attributes(
+                current_var_names, parents_test, target_relation_vars)
+
+        else:
+            attributes_counting = iter([])
+            attributes = iter([])
+        chosen_attributes, all_attributes_computed, all_chains_computed = self.chosen_tests(
+            attributes_counting, current_vars_per_type)
+        # print("{}Attributes generated: {}".format("  " * current_node.get_depth(), all_attributes_computed))
+        all_attributes_counted = 0
+        all_chains_counted = 0
+        for chain in attributes:
+            all_chains_counted += 1
+            # print(".", end="")
+            # if all_chains_counted % 100 == 0:
+            #     print("{}".format("  " * current_node.get_depth()), end="")
+            starting_index, relation_chain, aggregator_chains, fresh_vars = chain
+            # print("{}relation chain: {}".format("  " * current_node.get_depth(), relation_chain))
+            nb_fresh_vars = len(fresh_vars[0])
+            fresh_indices = fresh_vars[1]
+            # print(relation_chain)
+            example, rc_modified, c_values, c_var_names, c_num = self.create_example_and_chains(
+                relation_chain, current_vars_per_type)
+            a_ch = list(aggregator_chains)
+            # print(a_ch)
+            known_unknown = None
+            temp_counter = 0
+            for c_vs in c_values:
+                filtered_agg_chains = []
+                filtered_output_types = []
+                for i, agg_chain in enumerate(a_ch):
+                    if all_attributes_counted in chosen_attributes:
+                        filtered_agg_chains.append(agg_chain[0])
+                        filtered_output_types.append(agg_chain[1])
+                    all_attributes_counted += 1
+                    temp_counter += 1
+                # print("   csv -->", c_vs)
+                for c_name, c_v in zip(c_var_names, c_vs):
+                    example[c_name].set_value(c_v)
+                if BinarySplit.use_memo or known_unknown is None:
+                    # unset target variables
+                    for init_var_name in target_relation_vars:
+                        example[init_var_name].unset_value()
+                    r_key, a_keys, known_unknown = DecisionTree.test_values_memo_keys(
+                        example, rc_modified, filtered_agg_chains)
+                else:
+                    r_key, a_keys = None, []
+                t0 = time.time()
+
+                if self.java_port is not None:
+                    # do stuff here
+                    send_variables(example, self.client, self.wrapper)
+                    all_test_values = compute_test_values(
+                        target_data, target_relation_vars, rc_modified,
+                        filtered_agg_chains, r_key, a_keys, nb_fresh_vars,
+                        fresh_indices, known_unknown, self.client,
+                        self.wrapper)
+                else:
+                    all_test_values = []
+                    for jj, datum in enumerate(target_data):
+                        u0 = time.time()
+                        for init_var_name, train_value in zip(
+                                target_relation_vars, datum.get_descriptive()):
+                            example[init_var_name].set_value(train_value)
+                        u1 = time.time()
+                        self.set_example_values_time += u1 - u0
+                        u0 = time.time()
+                        all_test_values.append(
+                            bs.get_test_values(example, rc_modified,
+                                               filtered_agg_chains, r_key,
+                                               a_keys, datum.identifier,
+                                               nb_fresh_vars, fresh_indices,
+                                               known_unknown))
+                        u1 = time.time()
+                        self.find_values_time += u1 - u0
+                        # if jj % 10 == 0:
+                        #     print(".", end="")
+
+                # n_target_examples = len(target_data)
+                # assert n_target_examples == len(all_test_values1) == len(all_test_values2)
+                # for i, v1, v2 in zip(range(n_target_examples), all_test_values1, all_test_values2):
+                #     if v1 != v2:
+                #         print(i, v1, v2, target_data[i])
+                #         raise ValueError("... :)")
+                # print()
+
+                t1 = time.time()
+                self.get_test_value_time += t1 - t0
+                t0 = time.time()
+                score, configuration = self.evaluate_candidate_splits(
+                    current_node, all_test_values, target_data,
+                    current_vars_per_type[0], filtered_output_types)
+                t1 = time.time()
+                self.split_eval_time += t1 - t0
+                if BinarySplit.is_better_than_previous(score, best_score):
+                    best_score = score
+                    a_chain_ind, comparator, theta, partition, is_variable_free = configuration
+                    best_configuration = (rc_modified,
+                                          filtered_agg_chains[a_chain_ind],
+                                          c_vs, c_var_names, comparator, theta,
+                                          partition, is_variable_free,
+                                          starting_index)
+            # unset constants
+            for c_name in c_var_names:
+                example[c_name].unset_value()
+            # unset target variables
+            for init_var_name in target_relation_vars:
+                example[init_var_name].unset_value()
+            # sanity check
+            if temp_counter != c_num * len(a_ch):
+                print(temp_counter, c_num, len(a_ch))
+                print(example, rc_modified, c_values, c_var_names, c_num, a_ch)
+                print(relation_chain)
+                raise WrongValueException("Wrong value of counted attributes!")
+        # sanity check
+        if all_attributes_computed != all_attributes_counted or all_chains_computed != all_chains_counted:
+            message = "\nPredicted number of attributes: {} Number of attributes counted: {}\n" \
+                      "Predicted number of chains: {} Counted number of chains: {}"
+            raise WrongValueException(
+                message.format(all_attributes_computed, all_attributes_counted,
+                               all_chains_computed, all_chains_counted))
+        # create internal node or leaf
+        if BinarySplit.is_better_than_previous(best_score,
+                                               BinarySplit.worst_split_score):
+            self.current_number_internal_nodes += 1
+            r_chain, a_chain, c_vs, c_var_names, comparator, theta, partition, is_variable_free, starting_index = \
+                best_configuration
+            # print("---> r chain, c_var names", r_chain, c_var_names, sep="\n")
+            r_chain_fresh_part = len(r_chain) - starting_index + 1
+            split_test = []
+            # [d1, ...], d2: {type1: {freshVariable1, ...}, ...}
+            fresh_variables_chains = [{} for _ in range(r_chain_fresh_part)]
+            fresh_variables = {}  # Union of the upper
+            const_name_to_value = {n: v for n, v in zip(c_var_names, c_vs)}
+            temp_to_fix_name = {}
+            # find fresh variables, get rid of temporary names
+            for i_relation, ((r, var_names),
+                             a) in enumerate(zip(r_chain, a_chain)):
+                new_names = []
+                for var_name, var_type in zip(
+                        var_names,
+                        self.descriptive_data[r.get_name()].get_types()):
+                    # not seen in previous chains?
+                    condition1 = var_name not in all_variable_names
+                    condition2 = int(var_name[1:]) < 0
+                    if condition1 != condition2:
+                        print(var_name, all_variable_names)
+                        print(r_chain)
+                        exit(-12345)
+                    if condition1:
+                        assert i_relation + 1 >= starting_index
+                        fresh_variables_chain = fresh_variables_chains[
+                            i_relation - (starting_index - 1)]
+                        # not seen in this chain also?
+                        if var_name not in temp_to_fix_name:
+                            # we see this name for the first time --> rename from temp name
+                            new_var_name = self.generate_next_var_name(
+                                var_name[0])
+                            # set the value of constant variables
+                            is_const1 = var_name in const_name_to_value
+                            is_const2 = var_name[0] == "C"
+                            assert is_const1 == is_const2
+                            value = const_name_to_value[
+                                var_name] if is_const2 else None
+                            new_var = create_new_variable(
+                                new_var_name, var_type, value)
+                            if var_type not in fresh_variables_chain:
+                                fresh_variables_chain[var_type] = set()
+                            fresh_variables_chain[var_type].add(new_var)
+                            temp_to_fix_name[var_name] = new_var_name
+                            fresh_variables[new_var_name] = new_var
+                        else:
+                            new_var_name = temp_to_fix_name[var_name]
+                    else:
+                        new_var_name = var_name
+                    new_names.append(new_var_name)
+                split_test.append((r, new_names, a))
+            self.all_variables.update(fresh_variables)
+            fresh_variables_names = set(fresh_variables.keys())
+            self.reset_temp_var_count()
+            # set the split
+            bs = BinarySplit(split_test, comparator, theta, True,
+                             is_variable_free)
+            bs.add_fresh_variables(fresh_variables)
+            current_node.set_split(bs)
+            # branch frequencies
+            nb_examples = target_data_weight(target_data)
+            branch_frequencies = [
+                target_data_weight(target_data, part) / nb_examples
+                for part in partition
+            ]
+            current_node.get_stats().set_branch_frequencies(branch_frequencies)
+            # create children etc.
+            current_variables_children = [
+                current_vars_per_type[:starting_index] +
+                fresh_variables_chains, current_vars_per_type
+            ]
+            # print("variables before/fresh after inducing", current_node.description)
+            # print(all_variable_names, fresh_variables_names)
+            for i, part in enumerate(partition):
+                assert i < 2
+                label = current_node.description + ".{}".format(i)
+                child = TreeNode(label, current_node, [], None, None,
+                                 current_node.get_depth() + 1)
+                current_node.add_child(child)
+                target_data_child = [target_data[i] for i in part]
+                self.initialize_statistics(child, target_data_child)
+                current_variables_child = current_variables_children[i]
+                all_variable_names_child = all_variable_names | fresh_variables_names if i == 0 else all_variable_names
+                self.build_helper(target_data_child, child,
+                                  current_variables_child,
+                                  target_relation_vars,
+                                  all_variable_names_child)
+        else:
+            current_node.get_stats().create_predictions()
+
+    def should_try_find_a_split(self, current_node: TreeNode,
+                                target_data: List[Datum]):
+        if current_node.get_depth() >= self.max_depth:
+            return False
+        elif self.current_number_internal_nodes >= self.max_number_internal_nodes:
+            return False
+        elif target_data_weight(
+                target_data
+        ) <= 2 * self.minimal_examples_in_leaf - DecisionTree.eps:
+            return False
+        elif current_node.get_stats(
+        ).variability < DecisionTree.eps * self.root_node.get_stats(
+        ).variability:
+            # print("Variability too low: ", self.heuristic.compute_variability(current_node.get_stats()))
+            return False
+        else:
+            return True
+
+    def evaluate_candidate_splits(self, parent, test_values, target_data,
+                                  target_relation_vars, filtered_output_types):
+        n_aggregators = len(test_values[0])
+        best_score = BinarySplit.worst_split_score
+        best_configuration = None
+        for i in range(n_aggregators):
+            xs = [x[i] for x in test_values]
+            if filtered_output_types[i] == TYPE_NUMERIC:  # is numeric
+                t0 = time.time()
+                score, comparator, theta, partition = self.find_best_numeric(
+                    parent, xs, target_data)
+                is_variable_free = True
+                t1 = time.time()
+                self.numeric_tests += 1
+                self.numeric_tests_time += t1 - t0
+            else:  # is nominal: 'constant' or user defined type
+                t0 = time.time()
+                output_type = filtered_output_types[i]
+                if output_type in target_relation_vars:
+                    var_candidates = sorted(
+                        [v.name for v in target_relation_vars[output_type]])
+                else:
+                    var_candidates = []
+                score, comparator, theta, partition, is_variable_free = self.find_best_nominal(
+                    parent, xs, target_data, var_candidates, output_type)
+                t1 = time.time()
+                self.nominal_tests_time += t1 - t0
+            if BinarySplit.is_better_than_previous(score, best_score):
+                best_score = score
+                best_configuration = (i, comparator, theta, partition,
+                                      is_variable_free)
+        return best_score, best_configuration
+
+    def find_best_nominal(self, parent: TreeNode, xs: List[str], target_data: List[Datum],
+                          target_relation_vars: List[str], output_type: str, max_set_size=5) \
+            -> Tuple[float, Comparator, Set[str], List[List[int]], bool]:
+        if self.only_existential:
+            raise ValueError(
+                "Only existential tests cannot leave to nominal tests.")
+        is_usual_nominal = Relation.is_nominal_type(output_type)
+        if is_usual_nominal:
+            different_values = sorted(set(
+                xs))  # better than list, so that the order is always the same
+            different_values_helper = []
+            target_relation_var_indices = []
+        else:
+            different_values_helper = target_relation_vars
+            different_values = list(range(len(different_values_helper)))
+            target_relation_var_indices = [
+                int(v[1:]) for v in target_relation_vars
+            ]
+        n = len(different_values)
+        m = min(n, max_set_size)
+        if is_usual_nominal:
+            options = 2**(
+                m - 1
+            )  # Half of them suffice, empty set skipped later if necessary
+        else:
+            # Possible values are:
+            # - value of (at least one of) the target variable(s)
+            # - something else (including MODE_OF_EMPTY_LIST)
+            # We implicitly skip all the subsets of the form {'something else', ...},
+            # so we have to generate 2 ** m options (-1 for the empty one).
+            options = 2**m
+        if n > max_set_size:
+            # message = "Warning: Nominal split: Too many subsets of a set with size = {}." \
+            #           " Will evaluate {} randomly chosen ones."
+            # print(message.format(n, options))
+            subsets = random_subsets(different_values, options)
+        else:
+            subsets = subsets_of_list(different_values, options)
+            next(subsets)  # skip the empty set
+        best_score = BinarySplit.worst_split_score
+        best_comparator = None
+        best_subset = None
+        best_partition = None
+        generic_statistic = self.target_data_stat.__class__.construct_from_parent(
+            parent.get_stats())
+        left = []  # to prevent "unbound" warnings
+        for left_list, _ in subsets:
+            self.nominal_tests += 1
+            if is_usual_nominal:
+                left = set(left_list)
+            partition = [[], []]  # type: List[List[int]]
+            statistics = [
+                generic_statistic.get_copy() for _ in range(len(partition))
+            ]
+            for datum_in, (test_value,
+                           datum) in enumerate(zip(xs, target_data)):
+                j = 1
+                if is_usual_nominal:
+                    if test_value in left:
+                        j = 0
+                else:
+                    for chosen in left_list:
+                        if datum.descriptive_part[target_relation_var_indices[
+                                chosen]] == test_value:
+                            j = 0
+                            break
+                partition[j].append(datum_in)
+                statistics[j].add_example_during_split_eval(datum)
+            # update all stats
+            for sta in statistics:
+                sta.after_split_evaluation_update()
+            if self.is_split_valid(statistics):
+                score = self.heuristic.evaluate_split(parent.get_stats(),
+                                                      statistics)
+            else:
+                score = BinarySplit.worst_split_score
+            if BinarySplit.is_better_than_previous(score, best_score):
+                best_score = score
+                best_partition = partition
+                transpose_branches = DecisionTree.should_transpose_branches(
+                    statistics)
+                if transpose_branches:
+                    # best_partition = best_partition[::-1]
+                    best_comparator = DOES_NOT_CONTAIN
+                else:
+                    best_comparator = CONTAINS
+                if is_usual_nominal:
+                    best_subset = left  # right if transpose_branches else left
+                else:
+                    best_subset = {
+                        different_values_helper[chosen]
+                        for chosen in left_list
+                    }
+        return best_score, best_comparator, best_subset, best_partition, is_usual_nominal
+
+    def find_best_numeric(self, parent: TreeNode, xs: List[float], target_data: List[Datum]) \
+            -> Tuple[float, Comparator, float, List[List[int]]]:
+        n = len(xs)
+        sorted_indices = sorted(range(n), key=lambda t: xs[t])
+        best_score = BinarySplit.worst_split_score
+        best_comparator = SMALLER
+        best_threshold = -float('inf')
+        best_i = None
+        best_partition = None
+        transpose_branches = None
+        generic_statistic = self.target_data_stat.__class__.construct_from_parent(
+            parent.get_stats())
+        statistics = [generic_statistic,
+                      parent.get_stats().get_copy()
+                      ]  # type: List[NodeStatistics]
+        previous_value = xs[sorted_indices[0]]
+        if self.only_existential:
+            # The only possible test is x > 0, so the xs are converted into ones and zeros
+            min_x, max_x = xs[sorted_indices[0]], xs[sorted_indices[-1]]
+            if min_x < 0 or max_x == float("inf"):
+                message = "Counting should result in numbers from [0, inf). Your range: [{}, {}]"
+                raise ValueError(message.format(min_x, max_x))
+            # modify: 0 --> 0 and > 0 --> 1 to ensure only one test below
+            xs_modified = xs[:]
+            for i in range(n):
+                xs_modified[i] = 0 if xs[i] == 0 else 1
+        else:
+            xs_modified = xs
+
+        for i in range(n):
+            datum = target_data[sorted_indices[i]]
+            x = xs_modified[sorted_indices[i]]
+            if x > previous_value:
+                if x < float('inf'):
+                    if previous_value > float('-inf'):
+                        threshold = previous_value + (
+                            x - previous_value) / 2  # element of (previous, x)
+                    else:
+                        threshold = x - 21.21  # element of (-inf, x)
+                else:
+                    threshold = previous_value + 21.21  # element of (previous, inf)
+                previous_value = x
+                if self.is_split_valid(statistics):
+                    score = self.heuristic.evaluate_split(
+                        parent.get_stats(), statistics)
+                else:
+                    score = BinarySplit.worst_split_score
+                if BinarySplit.is_better_than_previous(score, best_score):
+                    best_score = score
+                    best_threshold = threshold
+                    best_i = i
+                    transpose_branches = DecisionTree.should_transpose_branches(
+                        statistics)
+            statistics[TreeNode.
+                       negative_branch].remove_example_during_split_eval(datum)
+            statistics[TreeNode.positive_branch].add_example_during_split_eval(
+                datum)
+        if BinarySplit.is_better_than_previous(best_score,
+                                               BinarySplit.worst_split_score):
+            best_partition = [sorted_indices[:best_i], sorted_indices[best_i:]]
+        if transpose_branches:
+            best_comparator = BIGGER
+            best_partition = best_partition[::-1]
+        return best_score, best_comparator, best_threshold, best_partition
+
+    def is_split_valid(self, stats: List[NodeStatistics]):
+        for stat in stats:
+            if stat.get_total_number_examples(
+            ) <= self.minimal_examples_in_leaf - DecisionTree.eps:
+                return False
+        return True
+
+    @staticmethod
+    def should_transpose_branches(statistics: List[NodeStatistics]):
+        weight_positive = statistics[0].get_total_number_examples()
+        weight_negative = statistics[1].get_total_number_examples()
+        return weight_positive < weight_negative
+
+    def generate_possible_attributes(self, current_var_names,
+                                     current_atom_tests,
+                                     target_relation_vars: List[str]):
+        # Forward: generate chain of new atom tests
+        # Backward: generated possible aggregator combinations
+        # print("generating attr's from ", current_var_names, current_atom_tests, sep="\n")
+        if len(current_atom_tests) < self.longest_atom_test_chain:
+            # reset everything
+            current_atom_tests = []
+            current_var_names = current_var_names[:1]
+
+        if len(current_var_names) - 1 != len(current_atom_tests):
+            raise WrongValueException(
+                "Lengths do not differ by one::\n{}\n{}".format(
+                    current_var_names, current_atom_tests))
+        var_names_up_to_here = {}
+        current_atom_tests_modified = []
+
+        for r, vs, a in current_atom_tests:
+            current_atom_tests_modified.append(
+                (r.get_name(), list(zip(vs, r.get_types()))))
+        for start_index in range(1, 1 + len(current_var_names)):
+            var_names_up_to_here = union_of_two_dicts(
+                var_names_up_to_here, current_var_names[start_index - 1])
+            test_chain = current_atom_tests_modified[:start_index - 1]
+            for new_tests_chain in self.generate_possible_attributes_helper_all_steps(
+                    1, var_names_up_to_here):
+                created_chain = test_chain + new_tests_chain
+                if is_relation_chain_valid(created_chain):
+                    fresh_v, fresh_i = DecisionTree.fresh_in_last_relation(
+                        created_chain, target_relation_vars)
+                    aggregator_chains = self.generate_possible_aggregator_chains(
+                        len(created_chain), fresh_v, fresh_i)
+                    yield start_index, created_chain, aggregator_chains, (
+                        set(fresh_v), fresh_i)
+
+    @staticmethod
+    def fresh_in_last_relation(tests_chain, target_relation_vars):
+        # compute the last fresh variable(s)
+        last_fresh = []
+        last_fresh_indices = []
+        initial_var_names_set = set(target_relation_vars)
+        non_fresh = set()
+        for test in tests_chain[:-1]:
+            _, var_names_types = test
+            non_fresh |= set(var_names_types)
+        relation_name, var_names_types = tests_chain[-1]
+        for i, var_name_type in enumerate(var_names_types):
+            var_name, var_type = var_name_type
+            p0 = var_name[0] != "C"
+            p1 = var_name not in initial_var_names_set
+            p2 = var_name_type not in non_fresh
+            p3 = var_type != Settings.atom_test_type_constant
+            if p0 and p1 and p2 and p3:
+                last_fresh.append(var_name_type)
+                last_fresh_indices.append(i)
+        return last_fresh, last_fresh_indices
+
+    def generate_possible_aggregator_chains(self, tests_chain_len,
+                                            last_fresh_variables,
+                                            last_fresh_indices):
+        def last_step_helper(fresh: int, current_type: str):
+            if fresh == 0:
+                # In this case, the aggregate should return 0 from [0] and 1 from [1] --> sum suffices
+                options = []
+                is_complex = False
+            else:
+                if current_type == TYPE_TUPLE:
+                    options = COMPLEX_ENOUGH_AGGREGATORS
+                    is_complex = True
+                elif current_type == TYPE_NOMINAL:
+                    options = NOMINAL_AGGREGATORS
+                    is_complex = False
+                elif current_type == TYPE_NUMERIC:
+                    options = NUMERIC_AGGREGATORS
+                    is_complex = False
+                elif current_type == TYPE_TYPE:
+                    # some user defined type like Person, Atom etc.
+                    options = NOMINAL_AGGREGATORS
+                    is_complex = False
+                else:
+                    raise WrongValueException(
+                        "Unknown type: {}".format(current_type))
+            chosen = []
+            if is_complex and PROJECT.name in self.allowed_aggregators:
+                for i, var_index in enumerate(last_fresh_indices):
+                    chosen += [
+                        PROJECTIONS[var_index](o)
+                        for o in last_step_helper(1, last_super_types[i])
+                        if o.name != COUNT.name
+                    ]
+            chosen += [
+                a for a in options if a.name in self.allowed_aggregators
+                and a.name != PROJECT.name
+            ]
+            yield from chosen
+
+        def generator_chains_helper(current_options_gen, current_super_type,
+                                    current_types, position):
+            current_options = list(current_options_gen)
+            if force_use_sum[0]:
+                if len(current_options) == 0:
+                    current_options = {SUM}
+                else:
+                    force_use_sum[0] = False
+            for o in current_options:
+                next_super_type, next_types = get_out_type(
+                    current_super_type, current_types, o)
+                if position == 0:
+                    if o not in forbidden_first:
+                        yield [o], next_types[0]
+                else:
+                    i = None
+                    o_real = o.aggregator if o.is_projection else o
+                    for i, g in enumerate(groups):
+                        if o_real in g:
+                            break
+                    next_options = is_followed_by[next_super_type][i]
+                    for left_part, left_type in generator_chains_helper(
+                            next_options, next_super_type, next_types,
+                            position - 1):
+                        yield left_part + [o], left_type
+
+        def get_super_type(k, t):
+            """
+            :param k: number of variables that are considered
+            :param t: ignored if k != 1, variable type as given in relation definition in the settings.
+            :return: Type of (the group of) the fresh variables
+            """
+            # behaves as numeric if no fresh
+            # or precisely one which is numeric
+            if k == 0:
+                return TYPE_NUMERIC
+            elif k > 1:
+                return TYPE_TUPLE
+            else:
+                if t.startswith(Relation.constant_numeric):
+                    return TYPE_NUMERIC
+                elif t.startswith(Relation.constant_nominal):
+                    return TYPE_NOMINAL
+                else:
+                    # user defined
+                    return TYPE_TYPE
+
+        def get_out_type(current_super_type, current_types,
+                         a: Union[Aggregator, Project]):
+            t = a.output_type
+            if current_super_type == TYPE_TUPLE:
+                # counting or projecting
+                if t == TYPE_NUMERIC:
+                    # counting, numeric projections
+                    return TYPE_NUMERIC, [
+                        TYPE_NUMERIC
+                    ]  # new type can be also simply numeric
+                elif t == TYPE_SAME_AS_INPUT:
+                    # nominal projection
+                    if not a.is_projection:
+                        raise ValueError("Should be projection")
+                    new_type = current_types[absolute_to_relative_positions[
+                        a.component]]
+                    new_super_type = get_super_type(1, new_type)
+                    return new_super_type, [new_type]
+                else:
+                    raise WrongValueException(
+                        "Wrong output type: {}".format(t))
+            else:
+                if t == TYPE_SAME_AS_INPUT:
+                    return current_super_type, current_types
+                elif t == TYPE_NUMERIC:
+                    return TYPE_NUMERIC, [
+                        TYPE_NUMERIC
+                    ]  # new type can be also simply numeric
+                else:
+                    raise WrongValueException(
+                        "Wrong output type: {}".format(t))
+
+        group0 = {MIN, MAX, MEAN, SUM}
+        group1 = {COUNT, COUNT_UNIQUE}
+        group2 = {MODE}
+        group3 = {FLATTEN, FLATTEN_UNIQUE}
+        groups = [[a for a in g if a.get_name() in self.allowed_aggregators]
+                  for g in [group0, group1, group2, group3]]
+        forbidden_first = {FLATTEN_UNIQUE, FLATTEN}
+        base_followed_dict = {
+            0: groups[0],
+            1: groups[0],
+            2: groups[1] + groups[2] + groups[3]
+        }
+        is_followed_by_numeric = {x: y for x, y in base_followed_dict.items()}
+        is_followed_by_nominal = {x: y for x, y in base_followed_dict.items()}
+        is_followed_by_tuple = {x: y for x, y in base_followed_dict.items()}
+        is_followed_by_type = {x: y for x, y in base_followed_dict.items()}
+        # update with group3 followers
+        is_followed_by_numeric.update({3: groups[0] + groups[1] + groups[3]})
+        is_followed_by_nominal.update({3: groups[1] + groups[2] + groups[3]})
+        is_followed_by_tuple.update({3: groups[1] + groups[3]})
+        is_followed_by_type.update({3: groups[1] + groups[2] + groups[3]})
+        is_followed_by = {
+            TYPE_NUMERIC: is_followed_by_numeric,
+            TYPE_NOMINAL: is_followed_by_nominal,
+            TYPE_TUPLE: is_followed_by_tuple,
+            TYPE_TYPE: is_followed_by_type
+        }
+        last_types = [value_type for _, value_type in last_fresh_variables]
+        last_super_types = [
+            get_super_type(1, value_type)
+            for _, value_type in last_fresh_variables
+        ]
+        nb_fresh = len(set(last_fresh_variables))
+        last_fresh_type = None if nb_fresh != 1 else last_fresh_variables[0][1]
+        last_super_type = get_super_type(nb_fresh, last_fresh_type)
+        force_use_sum = [nb_fresh == 0
+                         ]  # to prevent initialisation in helping functions
+        absolute_to_relative_positions = {
+            a: r
+            for r, a in enumerate(last_fresh_indices)
+        }
+        yield from generator_chains_helper(
+            last_step_helper(nb_fresh, last_super_type), last_super_type,
+            last_types, tests_chain_len - 1)
+
+    def generate_possible_attributes_helper_all_steps(
+            self, depth, var_counts_up_to_here: Dict[str, Set[str]]):
+        for head in self.generate_possible_attributes_helper_one_step(
+                var_counts_up_to_here):
+            yield [head]
+            if depth < self.max_number_atom_tests:
+                # update counts
+                _, var_names_types = head
+                fresh_dict = {}  # type: Dict[str, Set[str]]
+                for var_name, var_type in var_names_types:
+                    if var_type not in fresh_dict:
+                        fresh_dict[var_type] = set()
+                    fresh_dict[var_type].add(var_name)
+                new_counts = union_of_two_dicts(var_counts_up_to_here,
+                                                fresh_dict)
+                for tail in self.generate_possible_attributes_helper_all_steps(
+                        depth + 1, new_counts):
+                    yield [head] + tail
+
+    def generate_possible_attributes_helper_one_step(self,
+                                                     var_counts_up_to_here):
+        for rel_spec in sorted(self.allowed_atom_tests):
+            counts = self.allowed_atom_tests[rel_spec]
+            relation_name, var_specifications, var_types = rel_spec
+            arity = len(var_specifications)
+            o_types = sorted(counts.keys())
+            for needed_keys, configuration in generate_variable_configurations(
+                    var_counts_up_to_here, counts, o_types):
+                assert len(configuration) == len(counts)  # one for each type
+                variable_names = [None for _ in range(arity)]
+                none_counter = arity
+                for type_config, o_type in zip(configuration, o_types):
+                    (ind_old, ind_new), (names_old,
+                                         relative_counts_new) = type_config
+                    # place old
+                    for i_old, n_old in zip(ind_old, names_old):
+                        assert variable_names[i_old] is None
+                        none_counter -= 1
+                        variable_names[i_old] = n_old
+                    # place new
+                    temp_new_var_names = self.generate_temp_var_names(
+                        "Y", relative_counts_new)
+                    for i_new, n_new in zip(ind_new, temp_new_var_names):
+                        assert variable_names[i_new] is None
+                        none_counter -= 1
+                        variable_names[i_new] = n_new
+                    # place constants
+                    for i_const in counts[o_type][2]:  # TODO: hard-coded 2 ...
+                        assert variable_names[i_const] is None
+                        none_counter -= 1
+                        variable_names[i_const] = self.generate_temp_var_name(
+                            "C")
+                assert none_counter == 0
+                var_names_types = list(zip(variable_names, var_types))
+                yield relation_name, var_names_types
+
+    def create_example_and_chains(self, relations, current_vars):
+        def const_value_generator(c_name):
+            r_name, position = constants[c_name]
+            yield from self.descriptive_data[r_name].get_all_values(position)
+
+        def num_const_values():
+            product = 1
+            for c_name in constant_var_names:
+                r_name, position = constants[c_name]
+                product *= self.descriptive_data[r_name].get_nb_all_values(
+                    position)
+            return product
+
+        relation_chain = []
+        example = {}
+        constants = {}
+        # current
+        for d in current_vars:
+            for vs in d.values():
+                for v in vs:
+                    n = v.get_name()
+                    assert n not in example
+                    example[n] = v
+        # extended
+        for relation_name, var_names in relations:
+            for i, (n, t) in enumerate(var_names):
+                if n not in example:
+                    if n[0] == "C":
+                        assert n not in example  # always fresh constant variables
+                        example[n] = ConstantVariable(n, t, None)
+                        constants[n] = (relation_name, i)
+                    elif n[0] in "XY" and n not in example:
+                        example[n] = VariableVariable(n, t, None)
+                    elif n[0] not in "CXY":
+                        raise WrongValueException(
+                            "Wrong variable name {}".format(n))
+            relation_chain.append((self.descriptive_data[relation_name],
+                                   [n for n, _ in var_names]))
+
+        constant_var_names = sorted(constants.keys())
+        c_values = itertools.product(
+            *[const_value_generator(c) for c in constant_var_names])
+        return example, relation_chain, c_values, constant_var_names, num_const_values(
+        )
+
+    def predict(self, d: Datum, is_for_ensemble=False):
+        example = {}  # type: Dict[str, Variable]
+        for var, value in zip(self.target_relation_variables,
+                              d.get_descriptive()):
+            example[var.get_name()] = var
+            var.set_value(value)
+        current_node = self.root_node  # type: TreeNode
+        while not current_node.is_leaf():
+            # extend the example
+            for name, var in current_node.get_split().get_fresh_variables(
+            ).items():
+                example[name] = var
+            # get test value and send example to one of the children
+            is_positive = current_node.get_split().evaluate(example)
+            if is_positive:
+                current_node = current_node.get_child(TreeNode.positive_branch)
+            else:
+                current_node = current_node.get_child(TreeNode.negative_branch)
+        if is_for_ensemble:
+            prediction = current_node.get_stats().get_prediction_for_ensemble()
+        else:
+            prediction = current_node.get_stats().get_prediction()
+        for var in example.values():
+            if var.can_vary():
+                var.unset_value()
+        return prediction
+
+    def predict_all(self, ds: List[Datum], is_for_ensemble=False):
+        return [self.predict(d, is_for_ensemble) for d in ds]
+
+    def target_data_induction_preparation(self, target_data: List[Datum]):
+        if self.class_weights is None:
+            return None
+        for d in target_data:
+            d.set_weight(d.get_weight() * self.class_weights[d.get_target()])
+
+    def reverse_target_data_induction_preparation(self,
+                                                  target_data: List[Datum]):
+        if self.class_weights is None:
+            return None
+        for d in target_data:
+            d.set_weight(d.get_weight() / self.class_weights[d.get_target()])
+
+    @staticmethod
+    def populate_dict(target_data: List[Datum]):
+        for datum in target_data:
+            if datum.identifier not in TEST_VALUE_MEMO:
+                TEST_VALUE_MEMO[datum.identifier] = {}
+
+    @staticmethod
+    def test_values_memo_keys(example: Dict[str, Variable],
+                              relation_chain: List[Tuple[Relation, List[str]]],
+                              aggregation_chains: List[Tuple[Aggregator]]):
+        """
+
+        :param example:
+        :param relation_chain:
+        :param aggregation_chains:
+        :return: A 3-tuple: (relations_as_key, aggregators_as_keys, known_unknown_separated) where
+        - relations_as_key: (relation name, known_unknown, values) where
+            - relation name: str
+            - known_unknown: [is value known for variable1, ...]
+            - values:
+                - if variable is set to some value, then this equals its value
+                - elif variable is input variable, i.e., starts with 'X': name of the variable
+                - else: an integer
+        - aggregators_as_keys: tuple of tuples of aggregator names
+        - known_unknown_separated: indices of the variables with (un)known values
+        """
+        parts = []
+        known_unknown_separated = []
+        counters = {}
+        max_overall = -1
+        for r_vs in relation_chain:
+            r, vs = r_vs
+            known_unknown = []
+            known_unknown_separated_part = [[], []]  # type: List[List[int]]
+            out_values = []
+            max_part = -1
+            for i, v in enumerate(vs):
+                u = example[v].is_unset(
+                )  # target variables should not be set here yet
+                known_unknown.append(not u)
+                if u:
+                    if v[0] == 'X':
+                        out_values.append(v)
+                        known_unknown_separated_part[0].append(
+                            i)  # but are considered known
+                    else:
+                        if v not in counters:
+                            counters[v] = len(counters)
+                        value = counters[v]
+                        out_values.append(value)
+                        if value <= max_overall:
+                            known_unknown_separated_part[0].append(
+                                i)  # seen in the previous parts
+                        else:
+                            known_unknown_separated_part[1].append(
+                                i)  # unknown until this part
+                        max_part = max(max_part, value)
+                else:
+                    # assert v[0] != "X"
+                    out_values.append(example[v].get_value())
+                    known_unknown_separated_part[0].append(i)  # known
+            parts.append((r.name, tuple(known_unknown), tuple(out_values)))
+            max_overall = max(max_part, max_overall)
+            known_unknown_separated.append(known_unknown_separated_part)
+        relations_as_key = tuple(parts)
+        aggregators_as_keys = [
+            tuple(a.name for a in a_s) for a_s in aggregation_chains
+        ]
+        return relations_as_key, aggregators_as_keys, known_unknown_separated
+
+
+def is_relation_chain_valid(chain: List[Tuple[str, List[Tuple[str, str]]]]):
+    """
+    We check whether
+    0) At least one of the fresh (Y) variables in the relation r_i is used in r_{i + 1}
+    1) 2nd, 3rd, ... relation contains at least one variable from the previous relation.
+    2) no two elements are equal
+    :param chain: [(rel1, var_name_types1), ...], var_name_types1 = [('Y2', 'Person'), ...]
+    :return:
+    """
+    # 0)
+    for i in range(len(chain) - 1):
+        link_ok = True
+        has_fresh = False
+        for name, _1 in chain[i][1]:
+            if name[0] == "Y":
+                has_fresh = True
+                link_ok = False
+                for next_name, _2 in chain[i + 1][1]:
+                    if name == next_name:
+                        link_ok = True
+                        break
+            if has_fresh and link_ok:
+                break
+        if not link_ok:
+            return False
+    # 1)
+    for i in range(1, len(chain)):
+        link_ok = False
+        for name, _1 in chain[i][1]:
+            for prev_name, _2 in chain[i - 1][1]:
+                if prev_name == name:
+                    link_ok = True
+                    break
+            if link_ok:
+                break
+        if not link_ok:
+            return False
+    # 2)
+    chain_copy = chain[::]
+    chain_copy.sort()
+    for i in range(1, len(chain)):
+        if chain_copy[i] == chain_copy[i - 1]:
+            return False
+    return True
+
+
+def generate_variable_configurations(present, needed, needed_keys):
+    def generate_config_one_type(p, n):
+        old, new, _ = n
+        for additional_old, brand_new in subsets_of_list(new):
+            true_old = old + additional_old
+            true_new = brand_new  # new + brand_new?
+            old_configs = generalized_counting(
+                sorted(p), len(true_old))  # [['X1', 'X2', 'X1'], ...]
+            new_configs = canonic_sequences_of_new_variables(
+                len(true_new))  # [[1, 3, 2, 1], ...]
+            for combo in itertools.product(old_configs, new_configs):
+                yield (true_old, true_new), combo
+
+    # extend present with empty lists
+    for t in needed_keys:
+        if t not in present:
+            present[t] = set()
+    pairs = [(present[t], needed[t]) for t in needed_keys]
+    # cartesian product over the types
+    for combined in itertools.product(
+            *[generate_config_one_type(p, n) for p, n in pairs]):
+        yield needed_keys, combined
+
+
+def random_subsets(a_list, nb_subsets, random_seed=None):
+    if random_seed is not None:
+        random.seed(random_seed)
+    for _ in range(nb_subsets):
+        left_right = [[], []]
+        for x in a_list:
+            left_right[random.random() > 0.5].append(x)
+        yield left_right
+
+
+def create_new_variable(v_name, v_type, value=None):
+    if v_name[0] == "C":
+        return ConstantVariable(v_name, v_type, value)
+    elif v_name[0] in "XY":
+        return VariableVariable(v_name, v_type, value)
+    elif v_name[0] not in "CXY":
+        raise WrongValueException("Wrong variable name {}".format(v_name))
+
+
+def create_constant_tree(heuristic: Heuristic, data: Dataset):
+    t = DecisionTree(heuristic=heuristic, max_number_internal_nodes=0)
+    t.fit(data)
+    return t
```

### Comparing `re3py-0.35/re3py/utilities/cross_validation.py` & `re3py-0.36/re3py/utilities/cross_validation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,73 +1,74 @@
-from typing import List, Union
-from ..data.data_and_statistics import Dataset
-import random
-
-def create_folds(data: Dataset,
-                 folds_file: Union[str, None] = None,
-                 example_ids: Union[List[List[str]], None] = None,
-                 random_seed: Union[int, None] = 2864,
-                 n_folds=10):
-    """
-    Creates folds iterator.
-    :param data: a Dataset object
-    :param folds_file: one can specify their own test folds in a file of the following form:
-    |||
-    exampleID1_fold1
-    ...
-    exampleIDn1_fold1
-    |||
-    ...
-    |||
-    exampleID1_fold_k
-    ...
-    exampleIDn_k_fold_k
-    |||
-    :param example_ids: example IDs can be directly provided as a list of list of strings
-    :param random_seed: used for reproducibility when neither folds_file nor example_ids are provided, and the data
-    is randomly subdivided into folds
-    :param n_folds:
-    :return: for each fold, a training and test Dataset objects are yielded
-    """
-    target_relation = data.get_target_data()
-    id_to_datum = {d.descriptive_part[0]: d for d in target_relation}
-    folds = []
-    fresh_fold = None
-    fold_separator = "|||"
-    if folds_file is not None:
-        with open(folds_file) as f:
-            for line in f:
-                if line.startswith(fold_separator):
-                    if fresh_fold:
-                        folds.append(fresh_fold)
-                    fresh_fold = []
-                elif fresh_fold is not None:
-                    fresh_fold.append(line.strip())
-    else:
-        if example_ids is None:
-            example_ids = [[] for _ in range(n_folds)]
-            examples = list(id_to_datum.keys())
-            if random_seed is not None:
-                random.seed(random_seed)
-                random.shuffle(examples)
-            for i, example in enumerate(examples):
-                example_ids[i % n_folds].append(example)
-        folds = example_ids
-    assert folds is not None
-    for i, fold1 in enumerate(folds):
-        training_testing_target = [[], []]
-        for j, fold2 in enumerate(folds):
-            for d in fold2:
-                training_testing_target[i == j].append(id_to_datum[d])
-        training_data = Dataset(
-            settings=data.settings,
-            data_file=data.data_file,
-            descriptive_relations=data.get_descriptive_data(),
-            target_data=training_testing_target[0],
-            statistics=data.get_copy_statistics())
-        testing_data = Dataset(
-            settings=data.settings,
-            data_file=data.data_file,
-            descriptive_relations=data.get_descriptive_data(),
-            target_data=training_testing_target[1],
-            statistics=data.get_copy_statistics())
-        yield training_data, testing_data
+from typing import List, Union
+from ..data.data_and_statistics import Dataset
+import random
+
+
+def create_folds(data: Dataset,
+                 folds_file: Union[str, None] = None,
+                 example_ids: Union[List[List[str]], None] = None,
+                 random_seed: Union[int, None] = 2864,
+                 n_folds=10):
+    """
+    Creates folds iterator.
+    :param data: a Dataset object
+    :param folds_file: one can specify their own test folds in a file of the following form:
+    |||
+    exampleID1_fold1
+    ...
+    exampleIDn1_fold1
+    |||
+    ...
+    |||
+    exampleID1_fold_k
+    ...
+    exampleIDn_k_fold_k
+    |||
+    :param example_ids: example IDs can be directly provided as a list of list of strings
+    :param random_seed: used for reproducibility when neither folds_file nor example_ids are provided, and the data
+    is randomly subdivided into folds
+    :param n_folds:
+    :return: for each fold, a training and test Dataset objects are yielded
+    """
+    target_relation = data.get_target_data()
+    id_to_datum = {d.descriptive_part[0]: d for d in target_relation}
+    folds = []
+    fresh_fold = None
+    fold_separator = "|||"
+    if folds_file is not None:
+        with open(folds_file) as f:
+            for line in f:
+                if line.startswith(fold_separator):
+                    if fresh_fold:
+                        folds.append(fresh_fold)
+                    fresh_fold = []
+                elif fresh_fold is not None:
+                    fresh_fold.append(line.strip())
+    else:
+        if example_ids is None:
+            example_ids = [[] for _ in range(n_folds)]
+            examples = list(id_to_datum.keys())
+            if random_seed is not None:
+                random.seed(random_seed)
+                random.shuffle(examples)
+            for i, example in enumerate(examples):
+                example_ids[i % n_folds].append(example)
+        folds = example_ids
+    assert folds is not None
+    for i, _ in enumerate(folds):
+        training_testing_target = [[], []]
+        for j, fold2 in enumerate(folds):
+            for d in fold2:
+                training_testing_target[i == j].append(id_to_datum[d])
+        training_data = Dataset(
+            settings=data.settings,
+            data_file=data.data_file,
+            descriptive_relations=data.get_descriptive_data(),
+            target_data=training_testing_target[0],
+            statistics=data.get_copy_statistics())
+        testing_data = Dataset(
+            settings=data.settings,
+            data_file=data.data_file,
+            descriptive_relations=data.get_descriptive_data(),
+            target_data=training_testing_target[1],
+            statistics=data.get_copy_statistics())
+        yield training_data, testing_data
```

### Comparing `re3py-0.35/re3py/utilities/my_utils.py` & `re3py-0.36/re3py/utilities/my_utils.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,159 +1,159 @@
-import random
-
-
-class EnsembleRandomGenerator:
-    upper_bound = 12345
-
-    def __init__(self, random_seed):
-        self.meta_random = random.Random(random_seed)
-        self.tree_seeds = random.Random(self.next_seed())
-        self.bootstrap_seeds = random.Random(self.next_seed())
-        self.sample_rows_seeds = random.Random(self.next_seed())
-
-    def next_seed(self):
-        return int(self.meta_random.random() *
-                   EnsembleRandomGenerator.upper_bound)
-
-    def next_tree_seed(self):
-        return int(self.tree_seeds.random() *
-                   EnsembleRandomGenerator.upper_bound)
-
-    def next_bootstrap_seed(self):
-        return int(self.bootstrap_seeds.random() *
-                   EnsembleRandomGenerator.upper_bound)
-
-    def next_sample_rows_seed(self):
-        return int(self.sample_rows_seeds.random() *
-                   EnsembleRandomGenerator.upper_bound)
-
-
-def try_convert_to_number(s):
-    # try:
-    #     return int(s)
-    # except ValueError:
-    #     pass
-    try:
-        return float(s)
-    except ValueError:
-        pass
-    return s
-
-
-def union_of_two_dicts(d1, d2):
-    """
-    Computes the union of two dictionaries whose values are lists.
-    :param d1: dictionary, e.g.,  {'Person': {'X1', 'X2'}, 'Animal': {'Y1'}}
-    :param d2: same as d1, e.g., {'Person': {'X4'}, 'House': {'X3'}}
-    :return: a union of dictionaries, e.g., {'Person': {'X1', 'X2', 'X4'}, 'Animal': {'Y1'}, 'House': {'X3'}}
-    """
-    d = {k: {n for n in v} for k, v in d1.items()}
-    for k, v in d2.items():
-        if k not in d:
-            d[k] = v
-        else:
-            d[k] |= v
-    return d
-
-
-def average_of_dictionaries(ds):
-    n = len(ds)
-    together = {}
-    # sum
-    for d in ds:
-        for k, v in d.items():
-            if k not in together:
-                together[k] = 0.0
-            together[k] += v
-    # division
-    if n > 1:
-        for k in together:
-            together[k] /= n
-    return together
-
-
-def canonic_sequences_of_new_variables(n):
-    """
-    For example, if n == 5, we would get
-    1 1 1 1 1
-    1 1 1 1 2
-    1 1 1 2 1
-    ...
-    1 2 1 2 1
-    ...
-    but not 2 2 2 2 2, 2 1 2 1 2 etc.
-    :param n: The length of the sequence
-    :return: All possible sequences of indices of new variables.
-    """
-    def helper(k):
-        if k == 1:
-            yield [1], 1
-        else:
-            for s, m in helper(k - 1):
-                for i in range(1, m + 2):
-                    yield s + [i], max(i, m)
-
-    if n == 0:
-        yield []
-    else:
-        for t, _ in helper(n):
-            yield t
-
-
-def subsets_of_list(a_list, max_nb_generated=None):
-    n = len(a_list)
-    nb_subsets = 2**n
-    pattern = "{{:0>{}b}}".format(n)
-    if max_nb_generated is None:
-        max_nb_generated = nb_subsets
-    bound = min(nb_subsets, max_nb_generated)
-    for i in range(bound):
-        s = pattern.format(i)
-        chosen_and_not = [[], []]
-        for c, e in zip(s, a_list):
-            chosen_and_not[c == "0"].append(e)
-        yield chosen_and_not
-
-
-def generalized_counting(a_list, k):
-    n = len(a_list)
-    indices = [0] * k
-    if n > 0:
-        while True:
-            yield [a_list[i] for i in indices]
-            which = k - 1
-            while which >= 0 and indices[which] == n - 1:
-                which -= 1
-            if which < 0:
-                break
-            for after in range(which + 1, k):
-                indices[after] = 0
-            indices[which] += 1
-    elif k == 0:
-        yield []
-
-
-def get_an_element_of_set(s):
-    return next(iter(s))
-
-
-def arg_max(values):
-    m = -float("inf")
-    chosen = None
-    for i, v in enumerate(values):
-        if v > m:
-            m = v
-            chosen = i
-    return chosen
-
-
-def float_as_string(x, significant_places):
-    float_to_str_pattern = "{{:.{}e}}".format(significant_places)
-    x_str = float_to_str_pattern.format(float(x))
-    # Different lengths can occur:
-    # 1) '-' sign at the beginning
-    # 2) Different lengths of exponent: we assume that it is either e+12 or e+100
-    has_minus = x_str.startswith('-')
-    exponent_len = len(x_str) - x_str.find("e") - 2  # either 2 or 3
-    start = "" if has_minus else " "
-    end = "" if exponent_len == 3 else " "
-    return start + x_str + end
+import random
+
+
+class EnsembleRandomGenerator:
+    upper_bound = 12345
+
+    def __init__(self, random_seed):
+        self.meta_random = random.Random(random_seed)
+        self.tree_seeds = random.Random(self.next_seed())
+        self.bootstrap_seeds = random.Random(self.next_seed())
+        self.sample_rows_seeds = random.Random(self.next_seed())
+
+    def next_seed(self):
+        return int(self.meta_random.random() *
+                   EnsembleRandomGenerator.upper_bound)
+
+    def next_tree_seed(self):
+        return int(self.tree_seeds.random() *
+                   EnsembleRandomGenerator.upper_bound)
+
+    def next_bootstrap_seed(self):
+        return int(self.bootstrap_seeds.random() *
+                   EnsembleRandomGenerator.upper_bound)
+
+    def next_sample_rows_seed(self):
+        return int(self.sample_rows_seeds.random() *
+                   EnsembleRandomGenerator.upper_bound)
+
+
+def try_convert_to_number(s):
+    # try:
+    #     return int(s)
+    # except ValueError:
+    #     pass
+    try:
+        return float(s)
+    except ValueError:
+        pass
+    return s
+
+
+def union_of_two_dicts(d1, d2):
+    """
+    Computes the union of two dictionaries whose values are lists.
+    :param d1: dictionary, e.g.,  {'Person': {'X1', 'X2'}, 'Animal': {'Y1'}}
+    :param d2: same as d1, e.g., {'Person': {'X4'}, 'House': {'X3'}}
+    :return: a union of dictionaries, e.g., {'Person': {'X1', 'X2', 'X4'}, 'Animal': {'Y1'}, 'House': {'X3'}}
+    """
+    d = {k: {n for n in v} for k, v in d1.items()}
+    for k, v in d2.items():
+        if k not in d:
+            d[k] = v
+        else:
+            d[k] |= v
+    return d
+
+
+def average_of_dictionaries(ds):
+    n = len(ds)
+    together = {}
+    # sum
+    for d in ds:
+        for k, v in d.items():
+            if k not in together:
+                together[k] = 0.0
+            together[k] += v
+    # division
+    if n > 1:
+        for k in together:
+            together[k] /= n
+    return together
+
+
+def canonic_sequences_of_new_variables(n):
+    """
+    For example, if n == 5, we would get
+    1 1 1 1 1
+    1 1 1 1 2
+    1 1 1 2 1
+    ...
+    1 2 1 2 1
+    ...
+    but not 2 2 2 2 2, 2 1 2 1 2 etc.
+    :param n: The length of the sequence
+    :return: All possible sequences of indices of new variables.
+    """
+    def helper(k):
+        if k == 1:
+            yield [1], 1
+        else:
+            for s, m in helper(k - 1):
+                for i in range(1, m + 2):
+                    yield s + [i], max(i, m)
+
+    if n == 0:
+        yield []
+    else:
+        for t, _ in helper(n):
+            yield t
+
+
+def subsets_of_list(a_list, max_nb_generated=None):
+    n = len(a_list)
+    nb_subsets = 2**n
+    pattern = "{{:0>{}b}}".format(n)
+    if max_nb_generated is None:
+        max_nb_generated = nb_subsets
+    bound = min(nb_subsets, max_nb_generated)
+    for i in range(bound):
+        s = pattern.format(i)
+        chosen_and_not = [[], []]
+        for c, e in zip(s, a_list):
+            chosen_and_not[c == "0"].append(e)
+        yield chosen_and_not
+
+
+def generalized_counting(a_list, k):
+    n = len(a_list)
+    indices = [0] * k
+    if n > 0:
+        while True:
+            yield [a_list[i] for i in indices]
+            which = k - 1
+            while which >= 0 and indices[which] == n - 1:
+                which -= 1
+            if which < 0:
+                break
+            for after in range(which + 1, k):
+                indices[after] = 0
+            indices[which] += 1
+    elif k == 0:
+        yield []
+
+
+def get_an_element_of_set(s):
+    return next(iter(s))
+
+
+def arg_max(values):
+    m = -float("inf")
+    chosen = None
+    for i, v in enumerate(values):
+        if v > m:
+            m = v
+            chosen = i
+    return chosen
+
+
+def float_as_string(x, significant_places):
+    float_to_str_pattern = "{{:.{}e}}".format(significant_places)
+    x_str = float_to_str_pattern.format(float(x))
+    # Different lengths can occur:
+    # 1) '-' sign at the beginning
+    # 2) Different lengths of exponent: we assume that it is either e+12 or e+100
+    has_minus = x_str.startswith('-')
+    exponent_len = len(x_str) - x_str.find("e") - 2  # either 2 or 3
+    start = "" if has_minus else " "
+    end = "" if exponent_len == 3 else " "
+    return start + x_str + end
```

### Comparing `re3py-0.35/re3py/utilities/table_to_relations.py` & `re3py-0.36/re3py/utilities/table_to_relations.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-from utilities.my_exceptions import WrongValueException
-from utilities.my_utils import try_convert_to_number
-import os
-import re
-
-numeric = "numeric"
-nominal = "nominal"
-key = "key"
-
-
-def append_to_file_name(f_name, appendix):
-    i = f_name.rfind(".")
-    if i < 0:
-        return f_name + appendix
-    else:
-        return f_name[:i] + appendix + f_name[i:]
-
-
-def arff_to_relations(arff_file, target_index, out_dir, key_index=None):
-    """
-    Converts non-sparse arff to the relational form.
-    This results in two files: one for target relation and one for descriptive relations.
-    :param arff_file:
-    :param target_index: 0-based index of the target attribute
-    :param out_dir:
-    :param key_index: None of 0-based index of the key attribute
-    :return:
-    """
-    def get_attribute_type(vs):
-        if vs.lower() == numeric:
-            return numeric
-        elif vs[0] == "{" and vs[-1] == "}":
-            return nominal
-        elif vs.lower() == key:
-            return key
-        else:
-            raise WrongValueException("Don't know the type of {}.".format(vs))
-
-    def get_file_name(path):
-        normalized = re.sub("\\\\", "/", path)
-        return normalized[normalized.rfind("/") + 1:]
-
-    def make_out_dir_if_necessary(path):
-        normalized = re.sub("\\\\", "/", path)
-        if "/" not in normalized:
-            normalized += "/"
-        output_dir = normalized[:normalized.rfind("/")]
-        if not os.path.exists(output_dir):
-            os.makedirs(output_dir)
-
-    # handle the output file names etc.
-    arff_name = get_file_name(arff_file)
-    out_dir = re.sub("\\\\", "/", out_dir)
-    if out_dir[-1] != "/":
-        out_dir += "/"
-    descriptive_relations_file = out_dir + append_to_file_name(
-        arff_name, "_descriptive")
-    target_relations_file = out_dir + append_to_file_name(arff_name, "_target")
-    make_out_dir_if_necessary(target_relations_file)
-    make_out_dir_if_necessary(descriptive_relations_file)
-    # convert
-    f = open(arff_file)
-    attributes = []  # [(attribute name, type), ...]
-    data = "@data"
-    attribute = "@attribute"
-    for raw_line in f:
-        if data in raw_line.lower():
-            break
-        if raw_line.lower().startswith(attribute):
-            pattern = "{} +([^ ]+) +(.+)".format(attribute)
-            match = re.search(pattern, raw_line, flags=re.I)
-            name, values = match.group(1), match.group(2).strip()
-            attributes.append((name, get_attribute_type(values)))
-    out_descriptive = open(descriptive_relations_file, "w")
-    out_target = open(target_relations_file, "w")
-    examples = 0
-    for raw_line in f:
-        line = raw_line.strip()
-        if line:
-            examples += 1
-            values = [v.strip() for v in line.split(",")]
-            assert len(values) == len(attributes)
-            example_id = "ex{}".format(
-                examples) if key_index is None else values[key_index]
-            for i, (v, (a_name, a_type)) in enumerate(zip(values, attributes)):
-                if i != key_index and v != "?":
-                    if a_type == numeric:
-                        v = try_convert_to_number(v)
-                    out_f = out_descriptive if i != target_index else out_target
-                    print("{}({}, {})".format(a_name, example_id, v),
-                          file=out_f)
-    out_descriptive.close()
-    out_target.close()
-    f.close()
+from utilities.my_exceptions import WrongValueException
+from utilities.my_utils import try_convert_to_number
+import os
+import re
+
+numeric = "numeric"
+nominal = "nominal"
+key = "key"
+
+
+def append_to_file_name(f_name, appendix):
+    i = f_name.rfind(".")
+    if i < 0:
+        return f_name + appendix
+    else:
+        return f_name[:i] + appendix + f_name[i:]
+
+
+def arff_to_relations(arff_file, target_index, out_dir, key_index=None):
+    """
+    Converts non-sparse arff to the relational form.
+    This results in two files: one for target relation and one for descriptive relations.
+    :param arff_file:
+    :param target_index: 0-based index of the target attribute
+    :param out_dir:
+    :param key_index: None of 0-based index of the key attribute
+    :return:
+    """
+    def get_attribute_type(vs):
+        if vs.lower() == numeric:
+            return numeric
+        elif vs[0] == "{" and vs[-1] == "}":
+            return nominal
+        elif vs.lower() == key:
+            return key
+        else:
+            raise WrongValueException("Don't know the type of {}.".format(vs))
+
+    def get_file_name(path):
+        normalized = re.sub("\\\\", "/", path)
+        return normalized[normalized.rfind("/") + 1:]
+
+    def make_out_dir_if_necessary(path):
+        normalized = re.sub("\\\\", "/", path)
+        if "/" not in normalized:
+            normalized += "/"
+        output_dir = normalized[:normalized.rfind("/")]
+        if not os.path.exists(output_dir):
+            os.makedirs(output_dir)
+
+    # handle the output file names etc.
+    arff_name = get_file_name(arff_file)
+    out_dir = re.sub("\\\\", "/", out_dir)
+    if out_dir[-1] != "/":
+        out_dir += "/"
+    descriptive_relations_file = out_dir + append_to_file_name(
+        arff_name, "_descriptive")
+    target_relations_file = out_dir + append_to_file_name(arff_name, "_target")
+    make_out_dir_if_necessary(target_relations_file)
+    make_out_dir_if_necessary(descriptive_relations_file)
+    # convert
+    f = open(arff_file)
+    attributes = []  # [(attribute name, type), ...]
+    data = "@data"
+    attribute = "@attribute"
+    for raw_line in f:
+        if data in raw_line.lower():
+            break
+        if raw_line.lower().startswith(attribute):
+            pattern = "{} +([^ ]+) +(.+)".format(attribute)
+            match = re.search(pattern, raw_line, flags=re.I)
+            name, values = match.group(1), match.group(2).strip()
+            attributes.append((name, get_attribute_type(values)))
+    out_descriptive = open(descriptive_relations_file, "w")
+    out_target = open(target_relations_file, "w")
+    examples = 0
+    for raw_line in f:
+        line = raw_line.strip()
+        if line:
+            examples += 1
+            values = [v.strip() for v in line.split(",")]
+            assert len(values) == len(attributes)
+            example_id = "ex{}".format(
+                examples) if key_index is None else values[key_index]
+            for i, (v, (a_name, a_type)) in enumerate(zip(values, attributes)):
+                if i != key_index and v != "?":
+                    if a_type == numeric:
+                        v = try_convert_to_number(v)
+                    out_f = out_descriptive if i != target_index else out_target
+                    print("{}({}, {})".format(a_name, example_id, v),
+                          file=out_f)
+    out_descriptive.close()
+    out_target.close()
+    f.close()
```

### Comparing `re3py-0.35/re3py/utilities/user_defined_relation.py` & `re3py-0.36/re3py/utilities/user_defined_relation.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,269 +1,269 @@
-from typing import Dict, List
-from learners.core.tree_node_split import BinarySplit
-from learners.core.variables import ConstantVariable, VariableVariable
-from data.relation import Relation, parse_relation_arguments
-from learners.core.aggregators import Aggregator, CRITICAL_VALUES, ALL_AGGREGATORS
-from learners.core.comparators import ALL_COMPARATORS
-from utilities.my_exceptions import WrongValueException
-from data.data_and_statistics import compute_all_values_of_types
-import itertools
-
-
-class BinarySplitForRelation(BinarySplit):
-    def __init__(self, relation_updaters, *super_args):
-        super().__init__(*super_args)
-        self.relation_updaters = relation_updaters
-
-    def get_test_value_helper(self,
-                              example,
-                              chain_relations,
-                              chains_aggregators,
-                              nb_fresh_vars,
-                              fresh_indices,
-                              known_unknown_list,
-                              depth=1):
-        def results_generator(related_objects):
-            for r in related_objects:
-                # set
-                for i in unknown:
-                    rel_variables[i].set_value(r[i])
-                # compute
-                yield self.get_test_value_helper(example, chain_relations,
-                                                 chains_aggregators,
-                                                 nb_fresh_vars, fresh_indices,
-                                                 known_unknown_list, depth + 1)
-                # unset
-                for i in unknown:
-                    rel_variables[i].unset_value()
-
-        def should_keep_value(value):
-            return not (self.ignore_critical_values
-                        and value in CRITICAL_VALUES)
-
-        # for chain_aggregators in chains_aggregators:
-        #     assert len(chain_relations) == len(chain_aggregators)
-        relation, rel_variables_names = chain_relations[depth - 1]
-        rel_variables = [example[n] for n in rel_variables_names]
-        # aggregators = [chain[0] for chain in chains_aggregators]
-        if known_unknown_list is None:
-            known_unknown = [[], []]  # type: List[List[int]]
-            for i, v in enumerate(rel_variables_names):
-                known_unknown[example[v].is_unset()].append(i)
-        else:
-            known_unknown = known_unknown_list[depth - 1]
-        known, unknown = known_unknown
-        updater = self.relation_updaters[depth - 1]
-        if updater is not None:
-            updater.is_related(
-                tuple([rel_variables[i_known].value for i_known in known]))
-        related = relation.get_all(rel_variables, known)
-        if len(chain_relations) == depth:
-            if nb_fresh_vars is None:
-                fresh_indices = [
-                    i for i in unknown if rel_variables[i].can_vary()
-                ]
-                nb_fresh_vars = len(
-                    set(rel_variables[i].get_name() for i in fresh_indices))
-            if nb_fresh_vars == 0:
-                to_aggregate = [len(related)]
-            elif nb_fresh_vars == 1:
-                to_aggregate = [r[fresh_indices[0]]
-                                for r in related]  # flattened
-            else:
-                to_aggregate = [[r[i] for i in fresh_indices] for r in related]
-            return [to_aggregate for _ in range(len(chains_aggregators))]
-        else:
-            next_aggregators = [chain[depth] for chain in chains_aggregators
-                                ]  # type: List[Aggregator]
-            to_aggregate = []
-            for res in results_generator(related):
-                to_aggregate.append(res)
-            answer = []
-            for a_ind, a in enumerate(next_aggregators):
-                ls = [neigh[a_ind] for neigh in to_aggregate]
-                out = [x for x in a.aggregate(ls) if should_keep_value(x)]
-                answer.append(out)
-            return answer
-
-
-class RelationConstructor:
-    def __init__(self, relation, variables,
-                 binary_splits_for_relation: List['BinarySplitForRelation']):
-        self.relation = relation
-        self.input_variables = variables
-        self.binary_splits_for_relation = binary_splits_for_relation
-        self.memo = set()
-        self.all_variables = {v.name: v for v in self.input_variables}
-        for v in self.input_variables:
-            v.unset_value()
-
-    def update_all_variables(self):
-        for binary_split in self.binary_splits_for_relation:
-            for atom_test in binary_split.test:
-                relation_types = atom_test[0].types
-                var_names = atom_test[1]
-                for n, t in zip(var_names, relation_types):
-                    if n not in self.all_variables:
-                        self.all_variables[
-                            n] = RelationConstructor.create_variable(n, t)
-
-    def is_related(self, input_tuple):
-        if input_tuple not in self.memo:
-            example = {n: v.make_copy() for n, v in self.all_variables.items()}
-            for variable, value in zip(self.input_variables, input_tuple):
-                example[variable.name].value = value
-            y = False
-            for binary_test in self.binary_splits_for_relation:
-                y = binary_test.evaluate(example)
-                if y:
-                    break
-            self.memo.add(input_tuple)
-            if y:
-                self.relation.add_parsed_tuple(input_tuple)
-
-    def populate_relation(self, values_per_type):
-        options = [values_per_type[t] for t in self.relation.types]
-        for t in itertools.product(*options):
-            self.is_related(t)
-
-    @staticmethod
-    def create_variable(name, t):
-        if name[0] == "C":
-            v = ConstantVariable(name, t, None)
-        elif name[0] in "XY":
-            v = VariableVariable(name, t, None)
-        else:
-            raise WrongValueException("Wrong variable name {}".format(name))
-        return v
-
-
-def compute_new_relations(known_relations: Dict[str, Relation],
-                          new_relations_descriptions: List[Dict]):
-    """
-    :param known_relations: As in Dataset.descriptive_relations
-    :param new_relations_descriptions: Each element of this list is a 3-tuple that describes one of the
-     newly defined relations. Examples.
-
-     First, we define the relation sibling via already existing relations sister(Person, Person)
-     and brother(Person, Person) as follows: sibling(X0, X1) <==> sister(X0, X1) OR brother(X0, X1).
-     The corresponding 3-tuple is ('sibling(Person, Person)', ['X0', 'X1'], [description1, description2], True),
-     where
-     - 1st component gives new relation name and variable types
-     - 2nd component is a list of input variable names
-     - 3rd component gives the descriptions of the ways in which sibling(X, Y) is evaluated to True. In the concrete
-       example, the descriptions are
-       description1 = ([('sister', ['X0', 'X1'], 'SUM')], 'BIGGER', 0),
-       description2 = ([('brother', ['X0', 'X1'], 'SUM')], 'BIGGER', 0),
-       i.e., one of relations 'sister' and 'brother' should contain a tuple (X0, X1).
-
-       In general, the first component of each description mimics the tests used in the BinarySplits of the trees.
-     - 4th component tells whether we should ignore critical values when computing the aggregations from the conditions,
-       given in the 3rd component.
-
-    Next, the relation grandParent is defined via existing relation parent(Person, Person) as follows:
-    grandParent(X0, X1) <==> exists Y: parent(X0, Y) AND parent(Y, X1), and the corresponding 3-tuple is
-    ('grandParent(Person, Person)', ['X0', 'X1'], [description1], True),
-    where the 3rd component has now only one element, since there is only one way in which grandParent is evaluated
-    to True. This component is now
-    description1 = ([('parent', ['X0', 'Y'], 'SUM'), ('parent', ['Y', 'X1'], 'SUM')], 'BIGGER', 0),
-    i.e., its first component has now two elements.
-
-    Next, we give the 3-tuple for grandParent given in terms of mother, father, parent relations:
-    grandParent(X0, X1) <==>
-       (exists Y1: parent(X0, Y1) AND mother(Y1, X1)) OR
-       (exists Y1: parent(X0, Y1) AND father(Y1, X1))
-
-    Now, the 3-tuple is ('grandParent(Person, Person)', ['X0', 'X1'], [d1, d2], True),
-    where
-    d1 = ([('parent', ['X0', 'Y1'], 'SUM'), ('mother', ['Y1', 'X1'], 'SUM')], 'BIGGER', 0),
-    d2 = ([('parent', ['X0', 'Y1'], 'SUM'), ('father', ['Y1', 'X1'], 'SUM')], 'BIGGER', 0).
-
-    Note that the formalism does not allow for a (in this case) simpler definition
-    grandParent(X0, X1) <==> exists Y1: parent(X0, Y1 AND (mother(Y1, X1) OR father(Y1, X1))
-
-    Next, we give an example of recursively defined relation of ancestor via the relation of parent:
-    ancestor(X0, X1) <==> parent(X0, X1) OR (exists Y: parent(Y, X1) AND ancestor(X0, Y)).
-
-    The 3-tuple is ('ancestor(Person, Person)', ['X0', 'X1'], [d1, d2], True),
-    where
-    d1 = ([('parent', ['X0', 'X1'], 'SUM')], 'BIGGER', 0)
-    d2 = ([('parent', ['Y', 'X1'], 'SUM'), ('ancestor', ['X0', 'Y'], 'SUM')], 'BIGGER', 0).
-
-    Finally, we construct a relation hasLessThanThreeKids via relation isChild(Person, Person) as follows:
-     hasLessThanThreeKids(X0) <==> |{Y | isChild(Y, X0)}| < 3.
-
-    The 3-tuple is ('hasLessThanThreeKids(Person)', ['X0'], [d1], True),
-    where
-    d1 = ([('isChild', ['Y', 'X0'], 'COUNT')], 'BIGGER', 3).
-
-    :return: The new relations.
-    """
-    allowed_comparators = {c.name: c for c in ALL_COMPARATORS}
-    allowed_aggregators = {a.name: a for a in ALL_AGGREGATORS}
-    fresh = {}
-    fresh_helpers = {}
-    # define
-    for t in new_relations_descriptions:
-        name_and_types, variable_names, options, ignore_critical = t
-        relation_name = name_and_types[:name_and_types.find("(")]
-        relation_types = parse_relation_arguments(name_and_types,
-                                                  relation_name)
-        Relation.check_has_ok_types(relation_types)
-        fresh[relation_name] = Relation(relation_name, set(), None,
-                                        relation_types)
-        variables = [
-            RelationConstructor.create_variable(n, t)
-            for n, t in zip(variable_names, relation_types)
-        ]
-        fresh_helpers[relation_name] = RelationConstructor(
-            fresh[relation_name], variables, [])
-        # some sanity checks
-        for v in variable_names:
-            if v[0] != "X":
-                raise WrongValueException("Wrong variable name: {}".format(v))
-        for description in options:
-            atom_tests, comparator_name, threshold = description
-            if comparator_name not in allowed_comparators:
-                raise WrongValueException("Wrong comparator name: {}".format(
-                    description[1]))
-            for atom_test in atom_tests:
-                if atom_test[2] not in allowed_aggregators:
-                    raise WrongValueException(
-                        "Wrong aggregator name: {}".format(atom_test[2]))
-    all_relations = {}
-    for r_name, r in fresh.items():
-        all_relations[r_name] = (True, r)
-    for r_name, r in known_relations.items():
-        all_relations[r_name] = (False, r)
-    # properly initialize
-    for t in new_relations_descriptions:
-        name_and_types, variable_names, options, ignore_critical = t
-        relation_name = name_and_types[:name_and_types.find("(")]
-        relation_constructor = fresh_helpers[relation_name]
-        for description in options:
-            atom_tests, comparator_name, threshold = description
-            # some conversion
-            relation_updaters = []
-            bs_atom_tests = []
-            bs_comparator = allowed_comparators[comparator_name]
-            bs_threshold = threshold
-            bs_ignore = ignore_critical
-            for atom_test in atom_tests:
-                r_name, r_variable_names, aggregator_name = atom_test
-                is_fresh, r = all_relations[r_name]
-                bs_atom_tests.append((r, r_variable_names,
-                                      allowed_aggregators[aggregator_name]))
-                updater = fresh_helpers[r_name] if r_name in fresh else None
-                relation_updaters.append(updater)
-            # TODO: compute return Type etc.
-            bs = BinarySplitForRelation(relation_updaters, bs_atom_tests,
-                                        bs_comparator, bs_threshold, bs_ignore,
-                                        True)
-            relation_constructor.binary_splits_for_relation.append(bs)
-        relation_constructor.update_all_variables()
-    # fill with values
-    values_per_type = compute_all_values_of_types(
-        list(known_relations.values()))
-    for updater in fresh_helpers.values():
-        updater.populate_relation(values_per_type)
-    return fresh
+from typing import Dict, List
+from learners.core.tree_node_split import BinarySplit
+from learners.core.variables import ConstantVariable, VariableVariable
+from data.relation import Relation, parse_relation_arguments
+from learners.core.aggregators import Aggregator, CRITICAL_VALUES, ALL_AGGREGATORS
+from learners.core.comparators import ALL_COMPARATORS
+from utilities.my_exceptions import WrongValueException
+from data.data_and_statistics import compute_all_values_of_types
+import itertools
+
+
+class BinarySplitForRelation(BinarySplit):
+    def __init__(self, relation_updaters, *super_args):
+        super().__init__(*super_args)
+        self.relation_updaters = relation_updaters
+
+    def get_test_value_helper(self,
+                              example,
+                              chain_relations,
+                              chains_aggregators,
+                              nb_fresh_vars,
+                              fresh_indices,
+                              known_unknown_list,
+                              depth=1):
+        def results_generator(related_objects):
+            for r in related_objects:
+                # set
+                for i in unknown:
+                    rel_variables[i].set_value(r[i])
+                # compute
+                yield self.get_test_value_helper(example, chain_relations,
+                                                 chains_aggregators,
+                                                 nb_fresh_vars, fresh_indices,
+                                                 known_unknown_list, depth + 1)
+                # unset
+                for i in unknown:
+                    rel_variables[i].unset_value()
+
+        def should_keep_value(value):
+            return not (self.ignore_critical_values
+                        and value in CRITICAL_VALUES)
+
+        # for chain_aggregators in chains_aggregators:
+        #     assert len(chain_relations) == len(chain_aggregators)
+        relation, rel_variables_names = chain_relations[depth - 1]
+        rel_variables = [example[n] for n in rel_variables_names]
+        # aggregators = [chain[0] for chain in chains_aggregators]
+        if known_unknown_list is None:
+            known_unknown = [[], []]  # type: List[List[int]]
+            for i, v in enumerate(rel_variables_names):
+                known_unknown[example[v].is_unset()].append(i)
+        else:
+            known_unknown = known_unknown_list[depth - 1]
+        known, unknown = known_unknown
+        updater = self.relation_updaters[depth - 1]
+        if updater is not None:
+            updater.is_related(
+                tuple([rel_variables[i_known].value for i_known in known]))
+        related = relation.get_all(rel_variables, known)
+        if len(chain_relations) == depth:
+            if nb_fresh_vars is None:
+                fresh_indices = [
+                    i for i in unknown if rel_variables[i].can_vary()
+                ]
+                nb_fresh_vars = len(
+                    set(rel_variables[i].get_name() for i in fresh_indices))
+            if nb_fresh_vars == 0:
+                to_aggregate = [len(related)]
+            elif nb_fresh_vars == 1:
+                to_aggregate = [r[fresh_indices[0]]
+                                for r in related]  # flattened
+            else:
+                to_aggregate = [[r[i] for i in fresh_indices] for r in related]
+            return [to_aggregate for _ in range(len(chains_aggregators))]
+        else:
+            next_aggregators = [chain[depth] for chain in chains_aggregators
+                                ]  # type: List[Aggregator]
+            to_aggregate = []
+            for res in results_generator(related):
+                to_aggregate.append(res)
+            answer = []
+            for a_ind, a in enumerate(next_aggregators):
+                ls = [neigh[a_ind] for neigh in to_aggregate]
+                out = [x for x in a.aggregate(ls) if should_keep_value(x)]
+                answer.append(out)
+            return answer
+
+
+class RelationConstructor:
+    def __init__(self, relation, variables,
+                 binary_splits_for_relation: List['BinarySplitForRelation']):
+        self.relation = relation
+        self.input_variables = variables
+        self.binary_splits_for_relation = binary_splits_for_relation
+        self.memo = set()
+        self.all_variables = {v.name: v for v in self.input_variables}
+        for v in self.input_variables:
+            v.unset_value()
+
+    def update_all_variables(self):
+        for binary_split in self.binary_splits_for_relation:
+            for atom_test in binary_split.test:
+                relation_types = atom_test[0].types
+                var_names = atom_test[1]
+                for n, t in zip(var_names, relation_types):
+                    if n not in self.all_variables:
+                        self.all_variables[
+                            n] = RelationConstructor.create_variable(n, t)
+
+    def is_related(self, input_tuple):
+        if input_tuple not in self.memo:
+            example = {n: v.make_copy() for n, v in self.all_variables.items()}
+            for variable, value in zip(self.input_variables, input_tuple):
+                example[variable.name].value = value
+            y = False
+            for binary_test in self.binary_splits_for_relation:
+                y = binary_test.evaluate(example)
+                if y:
+                    break
+            self.memo.add(input_tuple)
+            if y:
+                self.relation.add_parsed_tuple(input_tuple)
+
+    def populate_relation(self, values_per_type):
+        options = [values_per_type[t] for t in self.relation.types]
+        for t in itertools.product(*options):
+            self.is_related(t)
+
+    @staticmethod
+    def create_variable(name, t):
+        if name[0] == "C":
+            v = ConstantVariable(name, t, None)
+        elif name[0] in "XY":
+            v = VariableVariable(name, t, None)
+        else:
+            raise WrongValueException("Wrong variable name {}".format(name))
+        return v
+
+
+def compute_new_relations(known_relations: Dict[str, Relation],
+                          new_relations_descriptions: List[Dict]):
+    """
+    :param known_relations: As in Dataset.descriptive_relations
+    :param new_relations_descriptions: Each element of this list is a 3-tuple that describes one of the
+     newly defined relations. Examples.
+
+     First, we define the relation sibling via already existing relations sister(Person, Person)
+     and brother(Person, Person) as follows: sibling(X0, X1) <==> sister(X0, X1) OR brother(X0, X1).
+     The corresponding 3-tuple is ('sibling(Person, Person)', ['X0', 'X1'], [description1, description2], True),
+     where
+     - 1st component gives new relation name and variable types
+     - 2nd component is a list of input variable names
+     - 3rd component gives the descriptions of the ways in which sibling(X, Y) is evaluated to True. In the concrete
+       example, the descriptions are
+       description1 = ([('sister', ['X0', 'X1'], 'SUM')], 'BIGGER', 0),
+       description2 = ([('brother', ['X0', 'X1'], 'SUM')], 'BIGGER', 0),
+       i.e., one of relations 'sister' and 'brother' should contain a tuple (X0, X1).
+
+       In general, the first component of each description mimics the tests used in the BinarySplits of the trees.
+     - 4th component tells whether we should ignore critical values when computing the aggregations from the conditions,
+       given in the 3rd component.
+
+    Next, the relation grandParent is defined via existing relation parent(Person, Person) as follows:
+    grandParent(X0, X1) <==> exists Y: parent(X0, Y) AND parent(Y, X1), and the corresponding 3-tuple is
+    ('grandParent(Person, Person)', ['X0', 'X1'], [description1], True),
+    where the 3rd component has now only one element, since there is only one way in which grandParent is evaluated
+    to True. This component is now
+    description1 = ([('parent', ['X0', 'Y'], 'SUM'), ('parent', ['Y', 'X1'], 'SUM')], 'BIGGER', 0),
+    i.e., its first component has now two elements.
+
+    Next, we give the 3-tuple for grandParent given in terms of mother, father, parent relations:
+    grandParent(X0, X1) <==>
+       (exists Y1: parent(X0, Y1) AND mother(Y1, X1)) OR
+       (exists Y1: parent(X0, Y1) AND father(Y1, X1))
+
+    Now, the 3-tuple is ('grandParent(Person, Person)', ['X0', 'X1'], [d1, d2], True),
+    where
+    d1 = ([('parent', ['X0', 'Y1'], 'SUM'), ('mother', ['Y1', 'X1'], 'SUM')], 'BIGGER', 0),
+    d2 = ([('parent', ['X0', 'Y1'], 'SUM'), ('father', ['Y1', 'X1'], 'SUM')], 'BIGGER', 0).
+
+    Note that the formalism does not allow for a (in this case) simpler definition
+    grandParent(X0, X1) <==> exists Y1: parent(X0, Y1 AND (mother(Y1, X1) OR father(Y1, X1))
+
+    Next, we give an example of recursively defined relation of ancestor via the relation of parent:
+    ancestor(X0, X1) <==> parent(X0, X1) OR (exists Y: parent(Y, X1) AND ancestor(X0, Y)).
+
+    The 3-tuple is ('ancestor(Person, Person)', ['X0', 'X1'], [d1, d2], True),
+    where
+    d1 = ([('parent', ['X0', 'X1'], 'SUM')], 'BIGGER', 0)
+    d2 = ([('parent', ['Y', 'X1'], 'SUM'), ('ancestor', ['X0', 'Y'], 'SUM')], 'BIGGER', 0).
+
+    Finally, we construct a relation hasLessThanThreeKids via relation isChild(Person, Person) as follows:
+     hasLessThanThreeKids(X0) <==> |{Y | isChild(Y, X0)}| < 3.
+
+    The 3-tuple is ('hasLessThanThreeKids(Person)', ['X0'], [d1], True),
+    where
+    d1 = ([('isChild', ['Y', 'X0'], 'COUNT')], 'BIGGER', 3).
+
+    :return: The new relations.
+    """
+    allowed_comparators = {c.name: c for c in ALL_COMPARATORS}
+    allowed_aggregators = {a.name: a for a in ALL_AGGREGATORS}
+    fresh = {}
+    fresh_helpers = {}
+    # define
+    for t in new_relations_descriptions:
+        name_and_types, variable_names, options, ignore_critical = t
+        relation_name = name_and_types[:name_and_types.find("(")]
+        relation_types = parse_relation_arguments(name_and_types,
+                                                  relation_name)
+        Relation.check_has_ok_types(relation_types)
+        fresh[relation_name] = Relation(relation_name, set(), None,
+                                        relation_types)
+        variables = [
+            RelationConstructor.create_variable(n, t)
+            for n, t in zip(variable_names, relation_types)
+        ]
+        fresh_helpers[relation_name] = RelationConstructor(
+            fresh[relation_name], variables, [])
+        # some sanity checks
+        for v in variable_names:
+            if v[0] != "X":
+                raise WrongValueException("Wrong variable name: {}".format(v))
+        for description in options:
+            atom_tests, comparator_name, threshold = description
+            if comparator_name not in allowed_comparators:
+                raise WrongValueException("Wrong comparator name: {}".format(
+                    description[1]))
+            for atom_test in atom_tests:
+                if atom_test[2] not in allowed_aggregators:
+                    raise WrongValueException(
+                        "Wrong aggregator name: {}".format(atom_test[2]))
+    all_relations = {}
+    for r_name, r in fresh.items():
+        all_relations[r_name] = (True, r)
+    for r_name, r in known_relations.items():
+        all_relations[r_name] = (False, r)
+    # properly initialize
+    for t in new_relations_descriptions:
+        name_and_types, variable_names, options, ignore_critical = t
+        relation_name = name_and_types[:name_and_types.find("(")]
+        relation_constructor = fresh_helpers[relation_name]
+        for description in options:
+            atom_tests, comparator_name, threshold = description
+            # some conversion
+            relation_updaters = []
+            bs_atom_tests = []
+            bs_comparator = allowed_comparators[comparator_name]
+            bs_threshold = threshold
+            bs_ignore = ignore_critical
+            for atom_test in atom_tests:
+                r_name, r_variable_names, aggregator_name = atom_test
+                is_fresh, r = all_relations[r_name]
+                bs_atom_tests.append((r, r_variable_names,
+                                      allowed_aggregators[aggregator_name]))
+                updater = fresh_helpers[r_name] if r_name in fresh else None
+                relation_updaters.append(updater)
+            # TODO: compute return Type etc.
+            bs = BinarySplitForRelation(relation_updaters, bs_atom_tests,
+                                        bs_comparator, bs_threshold, bs_ignore,
+                                        True)
+            relation_constructor.binary_splits_for_relation.append(bs)
+        relation_constructor.update_all_variables()
+    # fill with values
+    values_per_type = compute_all_values_of_types(
+        list(known_relations.values()))
+    for updater in fresh_helpers.values():
+        updater.populate_relation(values_per_type)
+    return fresh
```

### Comparing `re3py-0.35/re3py.egg-info/SOURCES.txt` & `re3py-0.36/re3py.egg-info/SOURCES.txt`

 * *Files identical despite different names*


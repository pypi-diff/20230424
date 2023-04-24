# Comparing `tmp/CoBaIR-2.1.0.tar.gz` & `tmp/CoBaIR-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CoBaIR-2.1.0.tar", last modified: Fri Mar 24 09:54:41 2023, max compression
+gzip compressed data, was "CoBaIR-3.0.0.tar", last modified: Mon Apr 24 06:37:07 2023, max compression
```

## Comparing `CoBaIR-2.1.0.tar` & `CoBaIR-3.0.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 09:54:41.422287 CoBaIR-2.1.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 09:54:41.418287 CoBaIR-2.1.0/CoBaIR/
--rw-rw-rw-   0 root         (0) root         (0)       20 2022-01-24 13:06:34.000000 CoBaIR-2.1.0/CoBaIR/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    37727 2023-02-23 12:23:51.000000 CoBaIR-2.1.0/CoBaIR/bayes_net.py
--rw-rw-rw-   0 root         (0) root         (0)    54996 2023-03-24 08:28:22.000000 CoBaIR-2.1.0/CoBaIR/configurator.py
--rw-rw-rw-   0 root         (0) root         (0)     1305 2022-08-05 09:56:01.000000 CoBaIR-2.1.0/CoBaIR/default_discretizer.py
--rw-rw-rw-   0 root         (0) root         (0)     1453 2022-08-05 09:56:01.000000 CoBaIR-2.1.0/CoBaIR/random_base_count.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 09:54:41.418287 CoBaIR-2.1.0/CoBaIR.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6767 2023-03-24 09:54:41.000000 CoBaIR-2.1.0/CoBaIR.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      629 2023-03-24 09:54:41.000000 CoBaIR-2.1.0/CoBaIR.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-24 09:54:41.000000 CoBaIR-2.1.0/CoBaIR.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       76 2023-03-24 09:54:41.000000 CoBaIR-2.1.0/CoBaIR.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-03-24 09:54:41.000000 CoBaIR-2.1.0/CoBaIR.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1533 2023-02-02 10:00:20.000000 CoBaIR-2.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6767 2023-03-24 09:54:41.422287 CoBaIR-2.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5985 2023-03-22 15:50:47.000000 CoBaIR-2.1.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-24 09:54:41.422287 CoBaIR-2.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1366 2023-03-20 10:30:53.000000 CoBaIR-2.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 09:54:41.422287 CoBaIR-2.1.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        7 2022-01-24 13:06:34.000000 CoBaIR-2.1.0/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3554 2022-10-28 18:37:31.000000 CoBaIR-2.1.0/tests/test_add_context.py
--rw-rw-rw-   0 root         (0) root         (0)     2437 2022-10-28 18:37:31.000000 CoBaIR-2.1.0/tests/test_add_intention.py
--rw-rw-rw-   0 root         (0) root         (0)     2603 2022-08-18 08:04:05.000000 CoBaIR-2.1.0/tests/test_create_bayesNet.py
--rw-rw-rw-   0 root         (0) root         (0)     2473 2023-01-23 09:29:09.000000 CoBaIR-2.1.0/tests/test_delete_context.py
--rw-rw-rw-   0 root         (0) root         (0)     2396 2023-01-23 09:29:09.000000 CoBaIR-2.1.0/tests/test_delete_intention.py
--rw-rw-rw-   0 root         (0) root         (0)     6673 2023-01-23 09:29:09.000000 CoBaIR-2.1.0/tests/test_edit_context.py
--rw-rw-rw-   0 root         (0) root         (0)     1205 2023-01-23 09:29:09.000000 CoBaIR-2.1.0/tests/test_edit_intention.py
--rw-rw-rw-   0 root         (0) root         (0)     3639 2022-10-28 18:37:31.000000 CoBaIR-2.1.0/tests/test_infer.py
--rw-rw-rw-   0 root         (0) root         (0)     1733 2023-01-23 09:29:09.000000 CoBaIR-2.1.0/tests/test_load.py
--rw-rw-rw-   0 root         (0) root         (0)     5424 2023-01-23 09:29:09.000000 CoBaIR-2.1.0/tests/test_new_combined_influence.py
--rw-rw-rw-   0 root         (0) root         (0)     1822 2023-01-23 09:29:10.000000 CoBaIR-2.1.0/tests/test_remove_combined_influence.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 06:37:07.802347 CoBaIR-3.0.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 06:37:07.798347 CoBaIR-3.0.0/CoBaIR/
+-rw-rw-rw-   0 root         (0) root         (0)       20 2022-01-24 13:06:34.000000 CoBaIR-3.0.0/CoBaIR/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    37882 2023-04-19 14:56:52.000000 CoBaIR-3.0.0/CoBaIR/bayes_net.py
+-rw-rw-rw-   0 root         (0) root         (0)    52168 2023-04-19 14:56:52.000000 CoBaIR-3.0.0/CoBaIR/configurator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1305 2022-08-05 09:56:01.000000 CoBaIR-3.0.0/CoBaIR/default_discretizer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1453 2022-08-05 09:56:01.000000 CoBaIR-3.0.0/CoBaIR/random_base_count.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 06:37:07.798347 CoBaIR-3.0.0/CoBaIR.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6771 2023-04-24 06:37:07.000000 CoBaIR-3.0.0/CoBaIR.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      629 2023-04-24 06:37:07.000000 CoBaIR-3.0.0/CoBaIR.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 06:37:07.000000 CoBaIR-3.0.0/CoBaIR.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       76 2023-04-24 06:37:07.000000 CoBaIR-3.0.0/CoBaIR.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 06:37:07.000000 CoBaIR-3.0.0/CoBaIR.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1533 2023-02-02 10:00:20.000000 CoBaIR-3.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6771 2023-04-24 06:37:07.802347 CoBaIR-3.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5985 2023-03-22 15:50:47.000000 CoBaIR-3.0.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 06:37:07.802347 CoBaIR-3.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1413 2023-04-17 12:59:19.000000 CoBaIR-3.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 06:37:07.802347 CoBaIR-3.0.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        7 2022-01-24 13:06:34.000000 CoBaIR-3.0.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3554 2022-10-28 18:37:31.000000 CoBaIR-3.0.0/tests/test_add_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     2437 2022-10-28 18:37:31.000000 CoBaIR-3.0.0/tests/test_add_intention.py
+-rw-rw-rw-   0 root         (0) root         (0)     2603 2022-08-18 08:04:05.000000 CoBaIR-3.0.0/tests/test_create_bayesNet.py
+-rw-rw-rw-   0 root         (0) root         (0)     2473 2023-01-23 09:29:09.000000 CoBaIR-3.0.0/tests/test_delete_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     2396 2023-01-23 09:29:09.000000 CoBaIR-3.0.0/tests/test_delete_intention.py
+-rw-rw-rw-   0 root         (0) root         (0)     6673 2023-01-23 09:29:09.000000 CoBaIR-3.0.0/tests/test_edit_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     1226 2023-04-17 12:59:19.000000 CoBaIR-3.0.0/tests/test_edit_intention.py
+-rw-rw-rw-   0 root         (0) root         (0)     4068 2023-04-19 14:56:52.000000 CoBaIR-3.0.0/tests/test_infer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1771 2023-04-17 12:59:19.000000 CoBaIR-3.0.0/tests/test_load.py
+-rw-rw-rw-   0 root         (0) root         (0)     4785 2023-04-17 12:59:19.000000 CoBaIR-3.0.0/tests/test_new_combined_influence.py
+-rw-rw-rw-   0 root         (0) root         (0)     1828 2023-04-17 12:59:19.000000 CoBaIR-3.0.0/tests/test_remove_combined_influence.py
```

### Comparing `CoBaIR-2.1.0/CoBaIR/bayes_net.py` & `CoBaIR-3.0.0/CoBaIR/bayes_net.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,53 +1,64 @@
-'''
+""" 
 This module provides a class for a two-layer bayes net for context based intention recognition.
-'''
+"""
 
 # System imports
 from __future__ import annotations
 import itertools
 from collections import defaultdict
 from collections.abc import Hashable
 from copy import deepcopy
-import warnings
-import os
 
 # 3rd party imports
 import bnlearn as bn
 from pgmpy.factors.discrete import TabularCPD
-import numpy as np
 import yaml
 # local imports
 from .random_base_count import Counter
 
 # end file header
 __author__ = 'Adrian Lubitz'
 
 # https://stackoverflow.com/questions/9169025/how-can-i-add-a-python-tuple-to-a-yaml-file-using-pyyaml
 
 
 class PrettySafeLoader(yaml.SafeLoader):
+    """A YAML loader that constructs Python tuples from YAML sequences."""
+
     def construct_python_tuple(self, node):
+        """
+        Construct a Python tuple from a YAML sequence node.
+
+        Args:
+            node (Any): The YAML sequence node to construct a tuple from.
+
+        Returns:
+            tuple: The constructed tuple.
+        """
         return tuple(self.construct_sequence(node))
 
 
 PrettySafeLoader.add_constructor(
-    u'tag:yaml.org,2002:python/tuple',
+    'tag:yaml.org,2002:python/tuple',
     PrettySafeLoader.construct_python_tuple)
 
 
 class BayesNet():
     def __init__(self, config: dict = None, bn_verbosity: int = 0, validate: bool = True) -> None:
         '''
         Initializes the BayesNet with the given config.
 
         Args:
             config: A dict with a config following the config format.
-            bn_verbosity: sets the verbose flag for bnlearn. See [bnlearn API](https://erdogant.github.io/bnlearn/pages/html/bnlearn.bnlearn.html?highlight=verbose#bnlearn.bnlearn.make_DAG) for more information
-            validate: Flag if the given config should be validated or not. This is necessary to load invalid configs
+            bn_verbosity: sets the verbose flag for bnlearn. See [bnlearn API](
+                https://erdogant.github.io/bnlearn/pages/html/bnlearn.bnlearn.html?highlight=verbose
+                #bnlearn.bnlearn.make_DAG) for more information
+            validate: Flag if the given config should be validated or not. 
+                This is necessary to load invalid configs
         '''
 
         self.valid = False
         self.bn_verbosity = bn_verbosity
         self.discretization_functions = {}
 
         if config is None:
@@ -88,63 +99,66 @@
     def _create_value_to_card(self):
         '''
         Initializes the translation dict for the context values to card numbers for bnlearn
         '''
         self.value_to_card = defaultdict(dict)
         for context, probabilities in self.config['contexts'].items():
             count = 0
-            for key, val in probabilities.items():
+            for key, _ in probabilities.items():
                 self.value_to_card[context][key] = count
                 count += 1
 
     def _create_card_to_value(self):
         '''
         Initializes the backtranslation dict for the context values to card numbers for bnlearn
         '''
         self.card_to_value = defaultdict(dict)
         for context, values in self.value_to_card.items():
             for name, num in values.items():
                 self.card_to_value[context][num] = name
 
     def _create_context_cpts(self):
         '''
-        Create the Conditional Probability Tables for all context nodes in the DAG and APPENDS them to self.cpts
+        Create the Conditional Probability Tables for all context nodes in the DAG and 
+            APPENDS them to self.cpts
         '''
         for context, probabilities in self.config['contexts'].items():
             values = [None] * len(probabilities)
             for value in probabilities:
                 values[self.value_to_card[context][value]] = [
                     probabilities[value]]
             self.cpts.append(TabularCPD(variable=context,
                              variable_card=len(probabilities), values=values))
 
     def _create_intention_cpts(self):
         '''
-        Create the Conditional Probability Tables for all intention nodes in the DAG and APPENDS them to self.cpts
+        Create the Conditional Probability Tables for all intention nodes in the DAG and 
+            APPENDS them to self.cpts
         '''
         for intention, context_influence in self.config['intentions'].items():
             values = self._calculate_probability_values(context_influence)
             # create a TabularCPD
-            self.cpts.append(TabularCPD(variable=intention, variable_card=2,  # intentions are always binary
-                                        # see https://pgmpy.org/factors/discrete.html?highlight=cpd#module-pgmpy.factors.discrete.CPD
-                                        values=values,
-                                        evidence=self.evidence,
-                                        evidence_card=self.evidence_card))
+            self.cpts.append(
+                TabularCPD(variable=intention,
+                           variable_card=2,  # intentions are always binary
+                           values=values,
+                           evidence=self.evidence,
+                           evidence_card=self.evidence_card)
+            )
 
     def _create_evidence_card(self):
         '''
         create the evidence_card for bnlearn
         '''
         self.evidence_card = []
         for evidence_variable in self.evidence:
             self.evidence_card.append(
                 len(self.config['contexts'][evidence_variable]))
 
     def _create_combined_context(self, context_influence: dict) -> dict:
-        # TODO: adjust example to use tuples
         """
         Creates a dict with the combined contexts in card index format from context_influence.
 
         Args:
             context_influence:
                 A dict with the influence values for contexts.
                 Example: {'speech commands':
@@ -163,21 +177,22 @@
         combined_context = {}
         for context in context_influence:
             if isinstance(context, tuple):
                 combined_context[tuple(map(self.evidence.index, context))
                                  ] = context_influence[context]
         return combined_context
 
-    def _alter_combined_context(self, count: Counter, context_influence: dict, combined_context: dict) -> dict:
-        # TODO: adjust example to use tuples
+    def _alter_combined_context(self, count: Counter, context_influence: dict,
+                                combined_context: dict) -> dict:
         """
         Overwrites the influence values for the cases of combined influence.
 
         Args:
-            count: A counter that indicates for which combination of context the average is calculated
+            count: 
+                A counter that indicates for which combination of context the average is calculated
             context_influence: 
                 A dict with the influence values for contexts.
                 Example: {'speech commands':
                             {'pickup': 5, 'handover': 0, 'other': 0},
                           'human holding object':
                             {True: 1, False: 4},
                           'human activity':
@@ -210,25 +225,25 @@
             value_tuple = list(values.keys())[0]
             for i, context_index in enumerate(context_tuple):
                 if active_case[context_index] != value_tuple[i]:
                     combined_case = False
                     break
             if combined_case:
                 for i, index in enumerate(context_tuple):
-                    altered_context_influence[self.evidence[index]][value_tuple[i]
-                                                                    ] = combined_context[context_tuple][value_tuple]
+                    altered_context_influence[self.evidence[index]][value_tuple[i]] = \
+                        combined_context[context_tuple][value_tuple]
                 break
         return altered_context_influence
 
     def _calculate_probability_values(self, context_influence: dict) -> list:
-        # TODO: adjust example to use tuples
         '''
         Calculates the probability values with the given context_influence from the config.
 
-        Influence on the positive case(intention is true) is calculated as the average over all influences for the given context.
+        Influence on the positive case(intention is true) is calculated as the 
+            average over all influences for the given context.
         The influence mapping is given in
         self.value_to_prob = {5: 0.95, 4: 0.75,
             3: 0.5, 2: 0.25, 1: 0.05, 0: 0.0}
         Args:
             context_influence:
                 A dict with the influence values for contexts.
                 Example: {'speech commands':
@@ -236,15 +251,15 @@
                           'human holding object':
                             {True: 1, False: 4},
                           'human activity':
                             {'idle': 4, 'working': 3}
                           }
         Returns:
             list:
-            A list of lists containing the probability values for the negative and positive respectively.
+            A list of lists containing the probability values for the negative and positive.
             Example:
 
             [[0.416, 0.5, 0.183, 0.266, 0.733, 0.816, 0.5, 0.583, 0.733, 0.816, 0.5, 0.583],
 
              [0.583, 0.5, 0.816, 0.733, 0.266, 0.183, 0.5, 0.416, 0.266, 0.183, 0.5, 0.416]]
         '''
         # For every intention calculate the average of their influencing contexts
@@ -258,16 +273,18 @@
             # alternate context_influence
             altered_context_influence = self._alter_combined_context(
                 count, context_influence, combined_context)
 
             ####
 
             for i in range(len(self.evidence_card)):
-                average += self.value_to_prob[altered_context_influence[self.evidence[i]
-                                                                        ][self.card_to_value[self.evidence[i]][count[i]]]]
+                value = self.card_to_value[self.evidence[i]][count[i]]
+                influence = altered_context_influence[self.evidence[i]][value]
+                prob = self.value_to_prob[influence]
+                average += prob
             average /= len(self.evidence)
             pos_values.append(average)
         # create neg_values
         neg_values = [1-value for value in pos_values]
         return [neg_values, pos_values]
 
     def valid_evidence(self, context: str, instantiation) -> tuple[bool, str]:
@@ -279,52 +296,59 @@
             context: a context
             instantiation: an instantiation of the context
         Returns:
             tuple[bool, str]:
             A tuple of bool to indicate validity and str for error message
         """
         if context not in self.config['contexts'] or instantiation is None:
-            # ignoring unrelated contexts and Nonetype # TODO: if I ignore it anyways then I can as well say it is valid
             return False, 'ignore'
-        if not isinstance(instantiation, Hashable) or not instantiation in self.config['contexts'][context].keys():
-            return False, f'{instantiation} is not a valid instantiation for {context}. Must be one of {list(self.config["contexts"][context].keys())}'
-        else:
-            return True, ''
+        if not isinstance(instantiation, Hashable) or \
+                not instantiation in self.config['contexts'][context].keys():
+            invalid_msg = f'{instantiation} is not a valid instantiation for {context}. '
+            valid_options = list(self.config["contexts"][context].keys())
+            valid_options_msg = f'Must be one of {valid_options}'
+            return False, invalid_msg + valid_options_msg
+        return True, ''
 
     def bind_discretization_function(self, context, discretization_function):
         """
         binds a discretization_function to a specific context.
 
 
         Args:
             context: One of the possible contexts from the config
-            discretization_function: A discretization function which has to take one parameter and return one of the possible discrete context instantiations.
+            discretization_function: A discretization function which has to take one parameter and 
+                return one of the possible discrete context instantiations.
         """
         if context not in self.contexts:
             raise ValueError(
                 f'Cannot bind discretization function to {context}. Context does not exist!')
         self.discretization_functions[context] = discretization_function
 
     def infer(self, evidence, normalized=True, decision_threshold=None) -> dict:
         '''
         infers the probabilities for the intentions with given evidence.
 
         Args:
             evidence:
                 Evidence to infer the probabilities of all intentions.
-                Evidence can contain context which is not in the config as well as it must not contain all possible contexts.
+                Evidence can contain context which is not in the config; 
+                    it must not contain all possible contexts.
                 Example:
                     {'speech commands': 'pickup',
                      'human holding object': True,
                      'human activity': 'idle'}
-            decision_threshold: a threshold for picking the most likely intention. Must be between 0 and 1. If not given the decision_threshold defined on initialization is taken. 
+            decision_threshold: a threshold for picking the most likely intention. 
+                Must be between 0 and 1. 
+                If not given the decision_threshold defined on initialization is taken. 
             normalized: Flag if the returned inference is normalized to sum up to 1.
         Returns:
             tuple:
-            Returns the highest ranking intention (or None if decision_threshold is not reached) and a dictionary of intentions and the corresponding probabilities.
+            Returns the highest ranking intention (or None if decision_threshold is not reached) and 
+                a dictionary of intentions and the corresponding probabilities.
         '''
         # check if evidence values are in instantiations and create a card form of bnlearn
         if decision_threshold is None:
             decision_threshold = self.config['decision_threshold']
         card_evidence = {}
         for context, instantiation in evidence.items():
             valid, err_msg = self.valid_evidence(context, instantiation)
@@ -334,39 +358,44 @@
                 discrete_instantiation = self.discretization_functions[context](
                     instantiation)
                 valid, err_msg = self.valid_evidence(
                     context, discrete_instantiation)
                 if valid:
                     card_evidence[context] = self.value_to_card[context][discrete_instantiation]
                 else:
-                    if not err_msg == 'ignore':  # A discretizer function should still be able to output None
+                    if not err_msg == 'ignore':
                         raise ValueError(err_msg)
             else:
                 if not err_msg == 'ignore':
                     raise ValueError(err_msg)
 
         if self.valid:
             inference = {}
             for intention in self.intentions:
                 # only True values of binary intentions will be saved
                 inference[intention] = bn.inference.fit(
-                    self.DAG, variables=[intention], evidence=card_evidence, verbose=self.bn_verbosity).values[1]
+                    self.DAG,
+                    variables=[intention],
+                    evidence=card_evidence,
+                    verbose=self.bn_verbosity
+                ).values[1]
+
             if normalized:
                 inference = self.normalize_inference(inference)
             max_intention = max(inference, key=inference.get)
             max_intention = max_intention if inference[max_intention] > decision_threshold else None
-            return max_intention, inference
+            return max_intention, decision_threshold, inference
         else:
-            raise Exception('Configuration is invalid')
+            raise ValueError('Invalid configuration')
 
     def normalize_inference(self, inference: dict) -> dict:
         '''
         Normalizes the inference to a proper probability distribution.
 
-        Inference which is not normalized will just be normalized for one intention being True or False,
+        Inference which is not normalized will be normalized for one intention being True or False,
         which leads to uninterpretable results for inference of multiple intentions.
 
         Args:
             inference: dictionary of intentions and the corresponding probabilities
         Returns:
             dict: dictionary of intentions and the corresponding normalized probabilities.
 
@@ -380,71 +409,79 @@
     def validate_config(self):
         '''
         validate that the current config follows the correct format.
 
         Raises:
             AssertionError: An AssertionError is raised if the config is not valid.
         '''
-        # TODO: add validation that decision_threshold is a float
         # TODO: add validation that apriorio values are float
         # contexts and intentions need to be defined
         assert 'contexts' in self.config, 'Field "contexts" must be defined in the config'
         assert 'intentions' in self.config, 'Field "intentions" must be defined in the config'
         assert len(self.config['contexts']), 'No contexts defined'
         assert len(self.config['intentions']), 'No intentions defined'
-        assert isinstance(self.config['decision_threshold'], float) and self.config['decision_threshold'] >= 0 and self.config[
-            'decision_threshold'] < 1, 'Decision threshold must be a number between 0 and 1'
+        assert isinstance(self.config['decision_threshold'], float) and \
+            self.config['decision_threshold'] >= 0 and \
+            self.config['decision_threshold'] < 1, \
+            'Decision threshold must be a number between 0 and 1'
 
-        # Intentions need to have influence values for all contexts and their possible instantiations
+        # Intentions need to have influence value for all contexts and their possible instantiations
         for intention, context_influences in self.config['intentions'].items():
             for context, influences in context_influences.items():
 
                 if isinstance(context, str):
-                    assert context in self.config[
-                        'contexts'], f'Context influence {context} cannot be found in the defined contexts!'
+                    assert context in self.config['contexts'], \
+                        f'Context influence {context} cannot be found in the defined contexts!'
                 # assert influences.keys() == self.config['contexts'][context].keys(
-                # ), f'An influence needs to be defined for all instantiations! {intention}.{context} does not fit the defined instantiations for {context}'
+                # ), f'An influence needs to be defined for all instantiations!
+                # {intention}.{context} does not fit the defined instantiations for {context}'
+
                 for instantiation, influence in influences.items():
-                    if type(instantiation) is not tuple:
-                        assert 5 >= influence >= 0 and isinstance(
-                            influence, int), f'Influence Value for {intention}.{context}.{instantiation} must be an integer between 0 and 5! Is {influence}'
-                        assert instantiation in self.config['contexts'][context].keys(
-                        ), f'An influence needs to be defined for all instantiations! {intention}.{context}.{instantiation} does not fit the defined instantiations for {context}'
+                    if not isinstance(instantiation, tuple):
+                        assert 5 >= influence >= 0 and isinstance(influence, int), \
+                            f'Influence Value for {intention}.{context}.{instantiation} must be an integer between 0 and 5!' \
+                            f'Is {influence}'
+                        assert instantiation in self.config['contexts'][context].keys(), \
+                            f'An influence needs to be defined for all instantiations! {intention}.{context}.{instantiation}' \
+                            f'does not fit the defined instantiations for {context}'
+
         # Probabilities need to sum up to 1
         for context, instantiations in self.config['contexts'].items():
             for instantiation, value in instantiations.items():
                 assert isinstance(
                     value, float), f'Apriori probability of context "{context}.{instantiation}" is not a number'
-            assert sum(instantiations.values(
-            )) == 1.0, f'The sum of probabilities for context instantiations must be 1 - For "{context}" it is {sum(instantiations.values())}!'
+            assert sum(instantiations.values()) == 1.0, \
+                f'The sum of probabilities for context instantiations must be 1 - For "{context}" it is {sum(instantiations.values())}!'
             # This is the config of the currently running BayesNet
         self.valid_config = deepcopy(self.config)
         self.valid = True
 
     def _create_zero_influence_dict(self, context_with_instantiations: dict) -> defaultdict:
         """
-        This uses the context dict from config['contexts'] to instantiate a dict that can be used in config['intentions']['some_context']
+        This uses the context dict from config['contexts'] to instantiate a dict that can be used in 
+            config['intentions']['some_context']
 
         Args:
-            context_with_instantiations: a dict holding contexts, their instantiations and corresponding apriori probabilities
+            context_with_instantiations: 
+                a dict holding contexts, their instantiations and corresponding apriori probabilities
         Returns:
             defaultdict:
             A dictionary with zero-initialized influence values for every given context.
             Example:
             {some_context:{
                 inst_1:0,
                 inst_2:0,
                 ...
                 inst_3:0
                 }
             }
         """
         zeros = defaultdict(lambda: defaultdict(dict))
         for context, instantiations in context_with_instantiations.items():
-            for instantiation, value in instantiations.items():
+            for instantiation, _ in instantiations.items():
                 zeros[context][instantiation] = 0
         return zeros
 
     def add_context(self, context: str, instantiations: dict):
         """
         This will add a new context to the config and updates the bayesNet.
 
@@ -461,17 +498,14 @@
         # check if context exists already
         if context in self.config['contexts']:
             raise ValueError(
                 'Cannot add existing context - use edit_context to edit an existing context')
         # fill in the new context
         self.config['contexts'][context] = instantiations
         # add this context in every intention with instantiations and values beeing zero.
-        # for intention in self.config['intentions']:
-        #     self.config['intentions'][intention] = {**self.config['intentions'][intention], **self._create_zero_influence_dict(
-        #         {context: instantiations})}
         self._transport_context_into_intentions()
         # reinizialize
         self.__init__(self.config)
 
     def add_intention(self, intention: str):
         """
         This will add a new intention to the config and updates the bayesNet.
@@ -499,15 +533,16 @@
         self.__init__(self.config)
 
     def edit_context(self, context: str, instantiations: dict, new_name: str = None):
         """
         Edits an existing context - this can also be used to remove instantiations
 
         !!! note
-            Changing the name of an instantiation will always set the influence value of this instantiation to zero for all intentions!
+            Changing the name of an instantiation will always set the influence value of this 
+                instantiation to zero for all intentions!
 
         Args:
             context: Name of the context to edit
             instantiations:
                 A Dict of instantiations and their corresponding apriori probabilities.
                 Example: {True: 0.6, False: 0.4}
             new_name: A new name for the context
@@ -518,20 +553,20 @@
             AssertionError: An AssertionError is raised if the resulting config is not valid.
         """
         # check if context exists already - only then I can edit
         if context not in self.config['contexts']:
             raise ValueError(
                 'Cannot edit non existing context - use add_context to add a new context')
         if new_name:  # del old names context
-            del (self.config['contexts'][context])
+            del self.config['contexts'][context]
             # rename all occurences in intentions
             for intention in self.config['intentions']:
                 old_instantiations = deepcopy(
                     self.config['intentions'][intention][context])
-                del (self.config['intentions'][intention][context])
+                del self.config['intentions'][intention][context]
                 self.config['intentions'][intention][new_name] = old_instantiations
             context = new_name
 
         self.config['contexts'][context] = instantiations
         self._remove_context_from_intentions()
         self._transport_context_into_intentions()
         # reinizialize
@@ -553,15 +588,15 @@
         if intention not in self.config['intentions']:
             raise ValueError(
                 'Cannot edit non existing intention - use add_intention to add a new intention')
         if new_name in self.config['intentions']:
             raise ValueError(
                 f'{new_name} exists - cannot be given as the new name for {intention}')
         old_values = deepcopy(self.config['intentions'][intention])
-        del (self.config['intentions'][intention])
+        del self.config['intentions'][intention]
         self.config['intentions'][new_name] = old_values
         # reinizialize
         self.__init__(self.config)
 
     def del_context(self, context: str):
         """
         removes a context.
@@ -573,15 +608,15 @@
             AssertionError: An AssertionError is raised if the resulting config is not valid.
             ValueError: An ValueError is raised if the context is not in self.config.
         """
         # check if context exists already - only then I can edit
         if context not in self.config['contexts']:
             raise ValueError(
                 'Cannot delete non existing context - use add_context to add a new context')
-        del (self.config['contexts'][context])
+        del self.config['contexts'][context]
         self._remove_context_from_intentions()
         self._transport_context_into_intentions()
         # reinizialize
         self.__init__(self.config)
 
     def del_intention(self, intention):
         """
@@ -593,33 +628,34 @@
         Raises:
             AssertionError: An AssertionError is raised if the resulting config is not valid.
             ValueError: An ValueError is raised if the intention is not in self.config.
         """
         if intention not in self.config['intentions']:
             raise ValueError(
                 'Cannot delete non existing intention - use add_intention to add a new intention')
-        del (self.config['intentions'][intention])
+        del self.config['intentions'][intention]
         # reinizialize
         self.__init__(self.config)
 
     def save(self, path: str, save_invalid: bool = False):
         """
         saves the config of the bayesNet to a yml file.
 
         Args:
             path: path to the file the config will be saved in
             save_invalid: Flag to decide if invalid configs can be saved
         Raises:
-            ValueError: A ValueError is raised if `save_invalid` is `False` and the config is not valid
+            ValueError: 
+                A ValueError is raised if `save_invalid` is `False` and the config is not valid
         """
         if not self.valid and not save_invalid:
             raise ValueError(
                 "saving invalid config is only possible if save_invalid is set to True")
 
-        with open(path, 'w') as save_file:
+        with open(path, 'w', encoding='utf-8') as save_file:
             yaml.dump(default_to_regular(self.config), save_file)
 
     def load(self, path: str):
         """
         Loads a config from file and reinitializes the bayesNet.
 
         Args:
@@ -639,52 +675,55 @@
             context: Name of the context
             instantiation: The instantiation for which the apriori value needs to be changed
             value: the new apriori value
         Raises:
             ValueError: Raises a ValueError if the instantiation does not exists in the config
             AssertionError: An AssertionError is raised if the resulting config is not valid.
         """
-        # check if this value already exists because I'm using defaultdict - otherwise you can just add values
+        # check if this value already exists because I'm using defaultdict
+        # otherwise you can just add values
         if instantiation in self.config['contexts'][context]:
             self.config['contexts'][context][instantiation] = value
             # reinizialize
             self.__init__(self.config)
         else:
             raise ValueError(
                 'change_context_apriori_value can only change values that exist already')
 
     def change_influence_value(self, intention: str, context: str, instantiation, value: int):
         """
-        Change the influence value for a specific instantiation of a context for a specific intention.
+        Update the influence value of a specific intention for a particular context instance..
 
         Args:
             intention: Name of the intention
             context: name of the context
             instantiation: The instantiation for which the influence value should be changed
             value: the new influence value. Can be one out of [0, 1, 2, 3, 4, 5]
         Raises:
             ValueError: Raises a ValueError if the instantiation does not exists in the config
             AssertionError: An AssertionError is raised if the resulting config is not valid.
         """
-        # check if this value already exists because I'm using defaultdict - otherwise you can just add values
+        # check if this value already exists because I'm using defaultdict
+        # otherwise you can just add values
         if instantiation in self.config['intentions'][intention][context]:
             self.config['intentions'][intention][context][instantiation] = value
             self.__init__(self.config)
         else:
             raise ValueError(
                 'change_influence_value can only change values that exist already')
 
-    def add_combined_influence(self, intention: str, contexts: tuple, instantiations: tuple, value: int):
+    def add_combined_influence(self, intention: str, contexts: tuple,
+                               instantiations: tuple, value: int):
         """
         Adds an influence value for a combination of context instantiations.
 
         Args:
             intention: Name of the intention
             contexts: tuple containing the names of the contexts
-            instantiations: tuple of context instantiations for which the influence value should be set
+            instantiations: Tuple of context instances to set influence value for.
             value: influence value. Can be one out of [0, 1, 2, 3, 4, 5]
         Raises:
             ValueError: Raises a ValueError if the instantiation does not exists in the config
             AssertionError: An AssertionError is raised if the resulting config is not valid.
         """
         for i, instantiation in enumerate(instantiations):
             if instantiation not in self.config['intentions'][intention][contexts[i]]:
@@ -703,31 +742,32 @@
             instantiations: tuple of context instantiations
         Raises:
             ValueError: Raises a ValueError if the instantiation does not exists in the config
             AssertionError: An AssertionError is raised if the resulting config is not valid.
         """
         if instantiations not in self.config['intentions'][intention][contexts]:
             raise ValueError(
-                'remove_combined_influence can only remove combined context instantiations that already exist')
-        del (self.config['intentions'][intention][contexts])
+                'Combined context instantiations must exist to be removed.')
+        del self.config['intentions'][intention][contexts]
 
     def _transport_context_into_intentions(self):
         """
-        Transports contexts and their instantiations defined in the config['contexts'] into config['intentions'] as influencing context if not present.
+        Transports contexts and their instantiations defined in the config['contexts'] into 
+            config['intentions'] as influencing context if not present.
         """
         for context in self.config['contexts']:
             for instantiation in self.config['contexts'][context]:
                 for intention in self.config['intentions']:
                     if instantiation not in self.config['intentions'][intention][context]:
                         # This only works if it is a defaultdict
                         self.config['intentions'][intention][context][instantiation] = 0
 
     def _remove_context_from_intentions(self):
         """
-        This removes context or instantiations after removing/changing instantiations and/or context.
+        This removes context or instantiation after removing/changing instantiations and/or context.
         """
         # This is a hack because you can't edit while iterating a dict
         contexts_to_remove_from_intentions = []
         context_instantiations_to_remove_from_intentions = []
         for intention in self.config['intentions']:
             for context in self.config['intentions'][intention]:
                 if context not in self.config['contexts']:
@@ -735,17 +775,17 @@
                         (intention, context))
                 else:
                     for instantiation in self.config['intentions'][intention][context]:
                         if instantiation not in self.config['contexts'][context]:
                             context_instantiations_to_remove_from_intentions.append(
                                 (intention, context, instantiation))
         for intention, context in contexts_to_remove_from_intentions:
-            del (self.config['intentions'][intention][context])
+            del self.config['intentions'][intention][context]
         for intention, context, instantiation in context_instantiations_to_remove_from_intentions:
-            del (self.config['intentions'][intention][context][instantiation])
+            del self.config['intentions'][intention][context][instantiation]
 
     def change_decision_threshold(self, decision_threshold):
         """
         Changes the decision threshold in the config.
         Args:
             decision_threshold: The new decision threshold.
         Raises:
@@ -799,28 +839,29 @@
         defaultdict:
             a defaultdict containing the config
     """
 
     # if os.path.splitext(path)[-1] != ".yml":
     #     raise TypeError(
     #         'Invalid format file - only supporting yml files')
-    with open(path) as stream:
+    with open(path, encoding='utf-8') as stream:
         return config_to_default_dict(yaml.load(stream, Loader=PrettySafeLoader))
 
-# https://stackoverflow.com/questions/26496831/how-to-convert-defaultdict-of-defaultdicts-of-defaultdicts-to-dict-of-dicts-o
 
+# https://stackoverflow.com/questions/26496831/how-to-convert-defaultdict-of-defaultdicts-of-defaultdicts-to-dict-of-dicts-o
 
 def default_to_regular(d):
     """
     This casts a defaultdict to a regular dict which is needed for saving as yml file.
 
     Args:
         d: the dict which should be casted
     Returns:
         dict:
             a regular dict casted from the defaultdict
     """
-    # casts dicts or default dicts because otherwise it will stop at the first dict and if that has another defaultdict in it - that won't cast
+    # casts dicts or default dicts because otherwise it will stop at the first dict and
+    # if that has another defaultdict in it - that won't cast
     if isinstance(d, defaultdict) or isinstance(d, dict):
         d = {k: default_to_regular(
             v) for k, v in d.items() if not isinstance(v, dict) or v}
     return d
```

### Comparing `CoBaIR-2.1.0/CoBaIR/configurator.py` & `CoBaIR-3.0.0/CoBaIR/configurator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 '''
 This module is a GUI configurator to create configurations for context based intention recognition - it can as well be used in a live mode to test the configuration
 '''
 
 # System imports
 import sys
 from collections import defaultdict
-import tkinter as tk
-from tkinter import filedialog as fd
-from tkinter.simpledialog import Dialog
-from tkinter import ttk
 from copy import deepcopy
 from types import FunctionType as function
 from pathlib import Path
 import itertools
 
 # 3rd party imports
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
 import pyqtgraph as pg
 from PyQt5 import QtWidgets, uic
-from PyQt5.QtWidgets import *
+from PyQt5.QtWidgets import QDialog, QLabel, QLineEdit, QComboBox, QPushButton,\
+    QFrame, QGridLayout, QSizePolicy, QSlider, QFileDialog
+
 from PyQt5.QtCore import Qt, QStringListModel
-from PyQt5.QtGui import QFont, QFontMetrics
+from PyQt5.QtGui import QFont, QFontMetrics, QLinearGradient, QColor
+
 import yaml
 import numpy as np
 
-
 # local imports
 from .bayes_net import BayesNet, load_config
 
 
 # end file header
 __author__ = 'Adrian Lubitz'
 
@@ -61,16 +59,14 @@
         Args:
             master: the master window this dialog belongs to
         Returns:
             tk.Entry:
                 the initial focus
         """
         uic.loadUi(Path(Path(__file__).parent, 'NewIntention.ui'), self)
-        self.intention_entry = self.findChild(QLineEdit, 'lineEdit')
-        self.error_label = self.findChild(QLabel, 'label_2')
         self.error_label.setAlignment(Qt.AlignCenter)
         self.error_label.setStyleSheet("color: red")
         if self.intention:
             self.intention_entry.setText(self.intention)
         return self.intention_entry  # initial focus
 
     def get_result(self):
@@ -137,38 +133,32 @@
             master: the master window this dialog belongs to
         """
         uic.loadUi(Path(Path(__file__).parent,
                    'NewCombinedContextInfluence.ui'), self)
 
         values = list(self.intentions.keys())
 
-        self.intention_selection = self.findChild(QComboBox, 'comboBox')
         self.intention_selection.addItems(values)
         self.intention_selection.setCurrentIndex(0)
-        # Value
-        self.value_selection = self.findChild(QComboBox, 'comboBox_2')
         # Button
-        self.additional_context = self.findChild(QPushButton, 'pushButton')
         self.additional_context.clicked.connect(self.new_instantiation)
-        self.error_label = self.findChild(QLabel, 'label_5')
         self.error_label.setAlignment(Qt.AlignCenter)
         self.error_label.setStyleSheet("color: red")
         # contexts
         self.contexts = {}
-        self.context_frame = self.findChild(QFrame, 'frame')
         self.grid_layout = QGridLayout()
         self.context_frame.setLayout(self.grid_layout)
         for context, instantiations in list(self.intentions.values())[0].items():
             if not isinstance(context, tuple):
                 self.contexts[context] = instantiations
         self.context_selections = []
         self.context_menus = []
         self.instantiation_selections = []
         self.instantiation_menus = []
-        for i in range(2):
+        for _ in range(2):
             self.new_instantiation()
 
     def context_selected(self, context: str, i: int):
         """
         Callback for context selection in dropdown
 
         Args:
@@ -257,30 +247,36 @@
         intention = self.intention_selection.currentText()
         value = self.value_selection.currentText()
         contexts = []
         instantiations = []
         for i, context_selection in enumerate(self.context_selections):
             contexts.append(context_selection.currentText())
             instantiations.append(
-                self.original_instantiations[context_selection.currentText()][self.instantiation_selections[i].currentText()])
+                self.original_instantiations[
+                    context_selection.currentText()
+                ][
+                    self.instantiation_selections[i].currentText()
+                ])
         # intention: str, contexts: tuple, instantiations: tuple, value: int
         result = {'intention': intention, 'value': int(value), 'contexts': tuple(
             contexts), 'instantiations': tuple(instantiations)}
         self.accept()
         return result
 
 
 class NewContextDialog(QDialog):
     """Dialog Window for new Context"""
 
     def __init__(self, parent=None, predefined_context: dict = None) -> None:
         """
-        Extends the Constructor of Dialog to use already existing context and the corresponding instantiations and values.
+        Extends the Constructor of Dialog to use already existing context and 
+            the corresponding instantiations and values.
 
-        If context and their corresponding instantiations and values are given it will be filled in the corresponding text fields.
+        If context and their corresponding instantiations and values are given 
+            it will be filled in the corresponding text fields.
 
         Args:
             predefined_context:
                 Context with the corresponding instantiations.
                 Example: {'speech commands': {
                     'pickup': 0.2, 'handover': 0.2, 'other': 0.6}}
         """
@@ -300,19 +296,14 @@
         Args:
             master: the master window this dialog belongs to
         Returns:
             tk.Entry:
                 the initial focus
         """
         uic.loadUi(Path(Path(__file__).parent, 'NewContext.ui'), self)
-        self.grid_layout_2 = self.findChild(QGridLayout, 'gridLayout_2')
-        self.context_entry = self.findChild(QLineEdit, 'context_entry')
-        self.instantiations_frame = self.findChild(
-            QFrame, 'instantiations_frame')
-        self.error_label = self.findChild(QLabel, 'label_5')
         self.error_label.setAlignment(Qt.AlignCenter)
         self.error_label.setStyleSheet("color: red")
         self.instantiations = []
         self.shown_instantiations = 0
         self.grid_layout = QGridLayout()
         self.instantiations_frame.setLayout(self.grid_layout)
         self.instantiations_frame.setSizePolicy(
@@ -337,25 +328,24 @@
                 name = list(instantiations.keys())[0]
                 # get value
                 value = instantiations[name]
                 # set entries
                 name_entry.setText(str(name))
                 probability_entry.setText(str(value))
                 # del entry
-                del(instantiations[name])
+                del instantiations[name]
             self.grid_layout.addWidget(
                 name_entry, self.shown_instantiations+1, 0)
             self.grid_layout.addWidget(
                 probability_entry, self.shown_instantiations+1, 1)
             self.grid_layout.addWidget(
                 remove_button, self.shown_instantiations+1, 2)
             self.instantiations.append(
                 (name_entry, probability_entry, remove_button))
             self.shown_instantiations += 1
-        self.more = self.findChild(QPushButton, 'pushButton')
         self.more.clicked.connect(self.new_instantiation)
         return self.context_entry
 
     def remove_instantiation(self, remove_button):
         """
         Callback for the remove_button
         Args:
@@ -403,14 +393,17 @@
                 "Both name and probability cannot be empty.")
         elif not name_entry.text():
             self.error_label.setText("Name cannot be empty.")
         elif not probability_entry.text():
             self.error_label.setText("Probability cannot be empty.")
 
     def get_result(self):
+        """
+        Get the result of the New Context dialog.
+        """
         result = defaultdict(lambda: defaultdict(dict))
         errors = []
         context_entry = self.context_entry.text().strip()
         if not context_entry:
             errors.append("Context cannot be empty.")
         else:
             for i, instantiation in enumerate(self.instantiations):
@@ -440,15 +433,15 @@
 
 class Configurator(QtWidgets.QMainWindow):
     '''
     GUI configurator to create configurations for context based intention recognition.
     It can as well be used in a live mode to test the configuration
     '''
 
-    def __init__(self, config: dict = None, *args, **kwargs):
+    def __init__(self, *args, config: dict = None, **kwargs):
         '''
         Setting up the GUI
 
         Args:
             config: A dict with a config following the config format.
         '''
         self.app = QtWidgets.QApplication(sys.argv)
@@ -463,23 +456,15 @@
         # adding view box to the graphic layout widget
         self.view = self.win.addViewBox()
         self.graph_item = TwoLayerGraph()
         self.view.addItem(self.graph_item)
         self.setup_layout()
         self.bayesNet = BayesNet(config)
         self.create_fields()
-        self.show()  # Show the GUI
-
-    def set_error_label_red(self):
-        """
-        setting the alignment and color of the error label
-        """
-        self.error_label.setAlignment(
-            Qt.AlignCenter)  # TODO: no changes of style in functional code!
-        self.error_label.setStyleSheet("color: red")
+        self.show()  # Show the GU
 
     def create_fields(self):
         """
         Creates all necessary fields in the GUI.
 
         This should be used whenever the config is changed.
         It reads all values from the config and adjusts the GUI accordingly.
@@ -510,15 +495,16 @@
         self.decision_threshold_entry.setText(
             str(self.bayesNet.config['decision_threshold']))
 
     def adjust_button_visibility(self):
         """
         Adjusts if buttons are visible or not.
 
-        Buttons for edit and delete will only be visible if there is a corresponding intention or context already created.
+        Buttons for edit and delete will only be visible 
+            if there is a corresponding intention or context already created.
         """
         if self.bayesNet.config['contexts']:
             # set visible
             self.edit_context_button.show()
             self.delete_context_button.show()
             self.grid_layout.addWidget(self.new_context_button, 0, 4)
         else:
@@ -551,39 +537,39 @@
                 return
             try:
                 old_context_name = list(result.keys())[0]
                 new_instantiations = result[old_context_name]
                 if new_instantiations:
                     self.bayesNet.add_context(
                         old_context_name, new_instantiations)
-            except AssertionError as e:
-                self.error_label.setText(str(e))
+            except AssertionError as error_message:
+                self.error_label.setText(str(error_message))
             # update view!
             self.create_fields()
             self.context_selection.setCurrentText(old_context_name)
             # Explicit call is necessary because setCurrentText seems not to trigger the callback
             self.context_selected(old_context_name)
             dialog.accept()
 
-        ok_button = dialog.findChild(QPushButton, "pushButton_2")
-        ok_button.setDefault(True)
-        ok_button.clicked.connect(update_and_close)
-        cancel_button = dialog.findChild(QPushButton, "pushButton_3")
-        cancel_button.clicked.connect(dialog.reject)
+        dialog.ok_button.setDefault(True)
+        dialog.ok_button.clicked.connect(update_and_close)
+        dialog.cancel_button.clicked.connect(dialog.reject)
         dialog.exec_()
 
     def edit_context(self):
         """
         Edit the currently selected context.
 
         !!! note
-        Changing the name of an instantiation will always set the influence value of this instantiation to zero for all intentions!
+        Changing the name of an instantiation will always set the influence value 
+            of this instantiation to zero for all intentions!
 
         !!! note
-        The GUI can only handle strings for now. This means every instantiation name will be casted to a string upon editing.
+        The GUI can only handle strings for now. 
+        This means every instantiation name will be casted to a string upon editing.
         """
         # TODO: renaming instantiations should not neccesarily put influence values to zero - check cases
         # TODO: this will always set the instantiations as Strings
         # Open the new Context dialog with prefilled values
         # open small dialog to create context
 
         context = self.context_selection.currentText()
@@ -600,37 +586,35 @@
                 return
             try:
                 old_context_name = list(result.keys())[0]
                 new_instantiations = result[old_context_name]
                 if new_instantiations:
                     self.bayesNet.edit_context(
                         context, new_instantiations, old_context_name)
-            except (ValueError, AssertionError) as e:
-                self.error_label.setText(str(e))
+            except (ValueError, AssertionError) as error_message:
+                self.error_label.setText(str(error_message))
             self.create_fields()
             self.context_selection.setCurrentText(old_context_name)
             self.context_selected(old_context_name)
             dialog.accept()
-        ok_button = dialog.findChild(QPushButton, "pushButton_2")
-        ok_button.setDefault(True)
-        ok_button.clicked.connect(update_and_close)
-        cancel_button = dialog.findChild(QPushButton, "pushButton_3")
-        cancel_button.clicked.connect(dialog.reject)
+        dialog.ok_button.setDefault(True)
+        dialog.ok_button.clicked.connect(update_and_close)
+        dialog.cancel_button.clicked.connect(dialog.reject)
         dialog.exec_()
 
     def delete_context(self):
         """"
         Deletes the currently selected context.
         """
         self.error_label.setText("")
         context = self.context_dropdown.currentText()
         try:
             self.bayesNet.del_context(context)
-        except AssertionError as e:
-            self.error_label.setText(str(e))
+        except AssertionError as error_message:
+            self.error_label.setText(str(error_message))
         self.create_fields()
 
     def new_intention(self):
         """
         Open a new Dialog to create new intentions.
         """
         dialog = NewIntentionDialog(self)
@@ -639,25 +623,23 @@
             self.error_label.setText("")
             result = dialog.get_result()
             if not result:
                 return
             if result:
                 try:
                     self.bayesNet.add_intention(result)
-                except AssertionError as e:
-                    self.error_label.setText(str(e))
+                except AssertionError as error_message:
+                    self.error_label.setText(str(error_message))
             # update view!
             self.create_fields()
             self.intention_dropdown.setCurrentText(result)
             # Explicit call is neccessary because set seems not to trigger the callback
             self.influencing_context_selected(result)
-        ok_button = dialog.findChild(QPushButton, 'ok')
-        ok_button.clicked.connect(update_and_close)
-        cancel_button = dialog.findChild(QPushButton, "cancel")
-        cancel_button.clicked.connect(dialog.reject)
+        dialog.ok_button.clicked.connect(update_and_close)
+        dialog.cancel_button.clicked.connect(dialog.reject)
         dialog.exec_()
 
     def edit_intention(self):
         """
         Edit the name of the currently selected intention
         """
         # open small dialog to create context
@@ -668,39 +650,37 @@
             self.error_label.setText("")
             result = dialog.get_result()
             if not result:
                 return
             if result:
                 try:
                     self.bayesNet.edit_intention(intention, result)
-                except ValueError as e:
-                    self.error_label.setText(str(e))
+                except ValueError as error_message:
+                    self.error_label.setText(str(error_message))
             self.create_fields()
             self.intention_dropdown.setCurrentText(result)
             # Explicit call is necessary because set seems not to trigger the callback
             self.influencing_context_selected(result)
             dialog.accept()
 
-        ok_button = dialog.findChild(QPushButton, "ok")
-        ok_button.setDefault(True)
-        ok_button.clicked.connect(update_and_close)
-        cancel_button = dialog.findChild(QPushButton, "cancel")
-        cancel_button.clicked.connect(dialog.reject)
+        dialog.ok_button.setDefault(True)
+        dialog.ok_button.clicked.connect(update_and_close)
+        dialog.cancel_button.clicked.connect(dialog.reject)
         dialog.exec_()
 
     def delete_intention(self):
         """
         Delete the currently selected intention
         """
         self.error_label.setText("")
         intention = self.intention_dropdown.currentText()
         try:
             self.bayesNet.del_intention(intention)
-        except AssertionError as e:
-            self.error_label.setText(str(e))
+        except AssertionError as error_message:
+            self.error_label.setText(str(error_message))
         self.create_fields()
 
     def on_clicked_advanced(self):
         """
         Un/folds the advanced section
         """
         if self.advanced_folded:
@@ -717,39 +697,44 @@
             self.new_combined_influence_button.hide()
 
     def new_combined_influence(self):
         """
         Callback for the button
         """
         self.error_label.setText("")
-        dialog = NewCombinedContextDialog(
-            self, intentions=self.bayesNet.config['intentions'])
+        try:
+            dialog = NewCombinedContextDialog(
+                self, intentions=self.bayesNet.config['intentions'])
+        except IndexError:
+            self.error_label.setText(
+                "Intentions and Contexts need to be defined before combining them")
+            return
+        except Exception as e:
+            self.error_label.setText(str(e))
+            return
 
         def update_and_close():
             result = dialog.get_result()
             try:
                 self.bayesNet.add_combined_influence(
                     intention=result['intention'], contexts=result['contexts'], instantiations=result['instantiations'], value=result['value'])
-            except ValueError as e:
-                self.error_label.setText(str(e))
+            except ValueError as error_message:
+                self.error_label.setText(str(error_message))
             self.create_fields()
 
-        ok_button = dialog.findChild(QPushButton, "pushButton_2")
-        ok_button.clicked.connect(update_and_close)
-        cancel_button = dialog.findChild(QPushButton, "pushButton_3")
-        cancel_button.clicked.connect(dialog.reject)
+        dialog.ok_button.clicked.connect(update_and_close)
+        dialog.cancel_button.clicked.connect(dialog.reject)
         dialog.exec_()
 
     def fill_advanced_table(self):
         '''
         Fill the content of the table containing combined influence values
         '''
 
-        font = QFont()
-        font.setPointSize(13)
+        font = QFont("Times New Roman", 13)
         self.advanced_table.setParent(None)
         self.advanced_table.deleteLater()
         self.advanced_table = QFrame(self.advanced_hidden_frame)
         self.advanced_table.setLayout(QGridLayout())
         self.advanced_hidden_frame.layout().addWidget(self.advanced_table, 0, 0)
         self.advanced_table.layout().addWidget(QLabel('Intention'), 0, 0)
         self.advanced_table.layout().addWidget(QLabel('|'), 0, 1)
@@ -758,218 +743,170 @@
         self.advanced_table.layout().addWidget(QLabel('Influence Value'), 0, 4)
         self.advanced_table.setFont(font)
         row = 1
         for intention, context_influence in self.bayesNet.config['intentions'].items():
             for context in context_influence:
                 if isinstance(context, tuple):
                     for j in range(len(list(context_influence[context]))):
-                        key = (list(context_influence[context])[j])
+                        key = list(context_influence[context])[j]
                         # For every combined case make a label and a button
                         self.advanced_table.layout().addWidget(
                             QLabel(f'{intention}'), row, 0)
                         self.advanced_table.layout().addWidget(QLabel('|'), row, 1)
                         # build context String
                         context_string = ""
                         for i, _context in enumerate(context):
                             context_string += f'{_context}={str(key[i])}, '
                         context_string = context_string[:-2]
                         self.advanced_table.layout().addWidget(QLabel(context_string), row, 2)
                         self.advanced_table.layout().addWidget(QLabel('|'), row, 3)
                         self.advanced_table.layout().addWidget(
                             QLabel(f'{list(context_influence[context].values())[0]}'), row, 4)
                         remove_button = QPushButton('remove')
-                        remove_button.clicked.connect(lambda _, intention=intention, contexts=context, instantiations=list(
-                            context_influence[context].keys())[0]: self.remove_combined_influence(intention, contexts, instantiations))
+                        instantiations = list(
+                            context_influence[context].keys())[0]
+                        remove_button.clicked.connect(
+                            lambda _, intention=intention, contexts=context, instantiations=instantiations:
+                            self.remove_combined_influence(intention, contexts, instantiations))
                         self.advanced_table.layout().addWidget(remove_button, row, 5)
                         row += 1
 
     def remove_combined_influence(self, intention: str, contexts: tuple, instantiations: tuple):
+        """
+        Remove a combined influence from the BayesNet and update the advanced table.
+        """
         self.bayesNet.del_combined_influence(
             intention, contexts, instantiations)
         self.fill_advanced_table()
 
     def setup_layout(self):
         """
         Setting up the layout of the GUI.
         """
 
         uic.loadUi(Path(Path(__file__).parent, 'configurator.ui'), self)
-        self.grid_layout = self.findChild(QGridLayout, 'gridLayout')
         self.grid_layout.setVerticalSpacing(5)
 
         self.load_button.clicked.connect(self.load)
         self.save_button.clicked.connect(self.save)
         self.decision_threshold_entry.textChanged.connect(
             self.decision_threshold_changed)
 
-        self.error_label = self.findChild(QLabel, 'error_label')
-        self.set_error_label_red()
         self.error_label.setText("")
 
-        self.context_label = self.findChild(QLabel, 'intention_label_frame_2')
-        self.intention_label_frame = self.findChild(
-            QLabel, 'intention_label_frame')
-        self.on_label = self.findChild(QLabel, 'label_3')
-
-        self.context_dropdown = self.findChild(QComboBox, 'context_selection')
-        self.context_selection = self.context_dropdown
-
-        self.influencing_context_dropdown = self.findChild(
-            QComboBox, 'influencing_context_selection')
-        self.influencing_context_selection = self.influencing_context_dropdown
-
-        self.intention_dropdown = self.findChild(
-            QComboBox, 'intention_selection')
-
         self.context_instantiations = defaultdict(dict)
-
-        self.context_selected_frame = self.findChild(QFrame, 'frame_2')
-        self.influencing_context_frame = self.findChild(QFrame, 'frame')
-
         self.intention_instantiations = defaultdict(lambda: defaultdict(dict))
 
-        self.new_context_button = self.findChild(
-            QPushButton, 'new_context_button')
         self.new_context_button.clicked.connect(self.new_context)
-
-        self.edit_context_button = self.findChild(
-            QPushButton, 'edit_context_button')
         self.edit_context_button.clicked.connect(self.edit_context)
-        self.delete_context_button = self.findChild(
-            QPushButton, 'delete_context_button')
         self.delete_context_button.clicked.connect(self.delete_context)
 
-        self.new_intention_button = self.findChild(
-            QPushButton, 'new_intention_button')
         self.new_intention_button.clicked.connect(self.new_intention)
-        self.edit_intention_button = self.findChild(
-            QPushButton, 'edit_intention_button')
         self.edit_intention_button.clicked.connect(self.edit_intention)
-        self.delete_intention_button = self.findChild(
-            QPushButton, 'delete_intention_button')
+        self.delete_intention_button.clicked.connect(self.delete_intention)
 
-        self.new_combined_influence_button = self.findChild(
-            QPushButton, 'advanced_new_button')
         self.new_combined_influence_button.clicked.connect(
             self.new_combined_influence)
 
-        self.advanced_hidden_frame = self.findChild(QFrame, 'frame_3')
         self.advanced_label.setText("advanced \u25BC")
         self.advanced_label.setParent(self.advanced_hidden_frame)
         self.advanced_folded = False
         self.advanced_label.clicked.connect(self.on_clicked_advanced)
 
-        self.advanced_table = QFrame(self.advanced_hidden_frame)
-        self.advanced_hidden_frame.setLayout(QGridLayout())
-        self.advanced_hidden_frame.layout().addWidget(self.advanced_table, 0, 0)
-        self.on_clicked_advanced()
-
-        # add widgets to layout
-        self.grid_layout.addWidget(self.context_label, 0, 0)
-        self.grid_layout.addWidget(self.context_dropdown, 0, 1)
-        self.grid_layout.addWidget(self.edit_context_button, 0, 2)
-        self.grid_layout.addWidget(self.delete_context_button, 0, 3)
-
-        self.grid_layout.addWidget(self.context_selected_frame, 1, 1)
-
-        self.grid_layout.addWidget(self.intention_label_frame, 2, 0)
-        self.grid_layout.addWidget(self.influencing_context_dropdown, 2, 1)
-        self.grid_layout.addWidget(self.on_label, 2, 2)
-        self.grid_layout.addWidget(self.intention_dropdown, 2, 3)
-        self.grid_layout.addWidget(self.edit_intention_button, 2, 4)
-        self.grid_layout.addWidget(self.delete_intention_button, 2, 5)
-
-        self.grid_layout.addWidget(self.context_instantiations_3, 4, 1)
-        self.grid_layout.addWidget(self.decision_threshold_entry, 4, 2)
+        self.COLORS = {0: 'White', 1: 'Red', 2: 'Orange',
+                       3: 'Yellow', 4: 'darkCyan', 5: 'Green'}
+        # Adding the canvas
+        layout = QGridLayout()
+        self.canvas_frame.setLayout(layout)
+        self.canvas_frame.layout().addWidget(self.win, 0, 0)
 
         self.grid_layout.addWidget(self.advanced_label, 5, 1)
 
-        self.grid_layout.addWidget(self.advanced_new_button, 7, 1)
-
-        self.grid_layout.addWidget(self.load_button, 9, 1)
-        self.grid_layout.addWidget(self.save_button, 9, 2)
-
         # Adding the canvas
         layout = QGridLayout()
         self.canvas_frame.setLayout(layout)
         self.canvas_frame.layout().addWidget(self.win, 0, 0)
 
     def decision_threshold_changed(self, value):
         """
         Callback for change of the decision threshold.
         """
         self.error_label.setText("")
         try:
             self.bayesNet.change_decision_threshold(
                 float(value))
-        except AssertionError as e:
-            self.error_label.setText(f"{e}")
-        except ValueError as e:
+        except AssertionError as error_message:
+            self.error_label.setText(f"{error_message}")
+        except ValueError:
             self.error_label.setText(f'Decision Threshold must be a number')
 
     def set_context_dropdown(self, options: list, command: function = None):
         '''
-        This sets the options for a context optionMenu with the options and the corresponding command.
+        This sets the options for a context optionMenu with the options and corresponding command.
 
         Args:
             options: A list containing the options in the context dropdown
             command: a function which will be triggered when clicked on the dropdown option
         '''
         if not command:
             command = self.context_selected
-        self.context_dropdown.clear()
+        self.context_selection.clear()
 
         if options:
-            self.context_dropdown.addItems(list(options))
-            max_width = max([QFontMetrics(self.context_dropdown.font()).boundingRect(
+            self.context_selection.addItems(list(options))
+            max_width = max([QFontMetrics(self.context_selection.font()).boundingRect(
                 option).width() for option in options])
-            self.context_dropdown.setMinimumWidth(
+            self.context_selection.setMinimumWidth(
                 max_width + 25)
-            self.context_dropdown.setCurrentIndex(0)
-            self.context_dropdown.currentTextChanged.connect(command)
+            self.context_selection.setCurrentIndex(0)
+            self.context_selection.currentTextChanged.connect(command)
         else:
-            self.context_dropdown.addItem('Context')
-            self.context_dropdown.currentTextChanged.connect(command)
-        command(self.context_dropdown.currentText())
+            self.context_selection.addItem('Context')
+            self.context_selection.currentTextChanged.connect(command)
+        command(self.context_selection.currentText())
 
     def draw_graph(self):
         '''
         This draws the graph from the current config.
         '''
-        self.graph_item.set_config(self.bayesNet.config)
+        # only if config is valid
+        if self.bayesNet.valid:
+            self.graph_item.set_config(self.bayesNet.config)
 
     def set_influencing_context_dropdown(self, options: list, command: function = None):
         '''
-        This sets the options for the influencing context optionMenu with the options and the corresponding command.
+        This sets the options for the influencing context optionMenu 
+            with the options and the corresponding command.
 
         Args:
             options: A list containing the options in the influencing context dropdown
             command: a function which will be triggered when clicked on the dropdown option
         '''
         if not command:
             command = self.influencing_context_selected
-        self.influencing_context_dropdown.clear()
+        self.influencing_context_selection.clear()
         if options:
-            self.influencing_context_dropdown.addItems(list(options))
-            max_width = max([QFontMetrics(self.influencing_context_dropdown.font(
+            self.influencing_context_selection.addItems(list(options))
+            max_width = max([QFontMetrics(self.influencing_context_selection.font(
             )).boundingRect(option).width() for option in options])
-            self.influencing_context_dropdown.setMinimumWidth(
+            self.influencing_context_selection.setMinimumWidth(
                 max_width + 25)  # add some padding
-            self.influencing_context_dropdown.setCurrentIndex(0)
-            self.influencing_context_dropdown.currentTextChanged.connect(
+            self.influencing_context_selection.setCurrentIndex(0)
+            self.influencing_context_selection.currentTextChanged.connect(
                 command)
         else:
-            self.influencing_context_dropdown.addItem('Context')
-            self.influencing_context_dropdown.currentIndexChanged.connect(
+            self.influencing_context_selection.addItem('Context')
+            self.influencing_context_selection.currentIndexChanged.connect(
                 command)
-        command(self.influencing_context_dropdown.currentText())
+        command(self.influencing_context_selection.currentText())
 
     def set_intention_dropdown(self, options: list, command: function = None):
         '''
-        This sets the options for a intention optionMenu with the options and the corresponding command
+        This sets the options for a intention optionMenu 
+            with the options and the corresponding command
 
         Args:
             options: A list containing the options in the intention dropdown
             command: a function which will be triggered when clicked on the dropdown option
         '''
         if not command:
             command = self.influencing_context_selected
@@ -992,15 +929,14 @@
     def context_selected(self, context: str):
         """
         Callback for click on context in context dropdown.
 
         Args:
             context: name of the clicked context
         """
-
         for active_context, instantiations in self.context_instantiations.items():
             for instantiation, widgets in instantiations.items():
                 for widget in widgets:
                     try:
                         widget.deleteLater()
                     except AttributeError:
                         pass  # can not destroy StringVars
@@ -1024,15 +960,17 @@
         for instantiation, value in config['contexts'][context].items():
             instantiation_str = str(instantiation) if isinstance(
                 instantiation, bool) else instantiation
             label = QLabel(instantiation_str, self.context_selected_frame)
             label.setFont(QFont('Times New Roman', 13))
             line_edit = QLineEdit(str(value), self.context_selected_frame)
             line_edit.setFont(QFont('Times New Roman', 13))
-            line_edit.textChanged.connect(lambda text, context=context, instantiation=instantiation: self.apriori_values_changed(text, context=context, instantiation=instantiation)
+            line_edit.textChanged.connect(lambda text, context=context, instantiation=instantiation:
+                                          self.apriori_values_changed(
+                                              text, context=context, instantiation=instantiation)
                                           )
 
             layout.addWidget(label, row_count, 0)
             layout.addWidget(line_edit, row_count, 1)
 
             self.context_instantiations[context][instantiation] = (
                 label,
@@ -1056,45 +994,53 @@
                         except AttributeError:
                             pass  # can not destroy StringVars
                         except Exception as e:
                             # TODO: better logging
                             print(f"couldn't destroy: {e}")
         intention = self.intention_dropdown.currentText()
         context = self.influencing_context_selection.currentText()
-        if context not in self.bayesNet.config['contexts'] or intention not in self.bayesNet.config['intentions']:
+        if context not in self.bayesNet.config['contexts'] or \
+                intention not in self.bayesNet.config['intentions']:
             return
 
         self.intention_instantiations = defaultdict(lambda: defaultdict(dict))
 
         layout = QGridLayout()
         self.influencing_context_frame.setLayout(layout)
         layout = self.influencing_context_frame.layout()
 
         layout.setVerticalSpacing(10)
         row_count = layout.rowCount()
 
         for instantiation, value in self.bayesNet.config['intentions'][intention][context].items():
+            influence_text = f'Influence of {context}:{instantiation} on {intention}: LOW'
             instantiation_label = QLabel(
-                f'Influence of {context}:{instantiation} on {intention}: LOW', self.influencing_context_frame)
+                influence_text, self.influencing_context_frame)
+
             instantiation_label.setFont(QFont('Times New Roman', 13))
             slider = QSlider(Qt.Horizontal, self.influencing_context_frame)
             slider.setFixedSize(100, 20)
+
             high_label = QLabel('HIGH', self.influencing_context_frame)
             high_label.setFont(QFont('Times New Roman', 13))
 
             layout.addWidget(instantiation_label, row_count, 0)
             layout.addWidget(slider, row_count, 1)
             layout.addWidget(high_label, row_count, 2)
 
             slider.setMinimum(0)
             slider.setMaximum(5)
             slider.setTickInterval(1)
+            slider.setStyleSheet(
+                f"QSlider::handle:horizontal {{background-color: {self.COLORS[value]}}}")
             slider.setValue(value)
+
             slider.valueChanged.connect(lambda value, context=context, intention=intention,
-                                        instantiation=instantiation: self.influence_values_changed(value, context, intention, instantiation))
+                                        instantiation=instantiation, slider=slider:
+                                        self.influence_values_changed(value, context, intention, instantiation, slider))
 
             self.intention_instantiations[intention][context][instantiation] = (
                 instantiation_label,
                 slider,
                 high_label,
             )
 
@@ -1109,18 +1055,18 @@
         fileName, _ = QFileDialog.getOpenFileName(
             None, "Choose Config", "", "Yaml files (*.yml);;All Files (*)", options=options)
         if fileName:
             try:
                 self.error_label.setText("loading BayesNet...")
                 self.bayesNet.load(fileName)
                 self.error_label.setText("")
-            except AssertionError as e:
-                self.error_label.setText(str(e))
-            except Exception as e:
-                self.error_label.setText(str(e))
+            except AssertionError as error_message:
+                self.error_label.setText(str(error_message))
+            except Exception as error_message:
+                self.error_label.setText(str(error_message))
         self.create_fields()
 
     def save(self):
         """
         opens a asksaveasfilename dialog to save a config
         """
         filetypes = "Yaml files (*.yml);;All Files (*)"
@@ -1138,34 +1084,37 @@
             instantiation: name of the corresponding instantiation
         """
         # update config
         self.error_label.setText("")
         try:
             self.bayesNet.change_context_apriori_value(context=context, instantiation=instantiation, value=float(
                 self.context_instantiations[context][instantiation][1].text()))
-        except AssertionError as e:
-            self.error_label.setText(str(e))
-        except ValueError as e:
+        except AssertionError as error_message:
+            self.error_label.setText(str(error_message))
+        except ValueError:
             self.error_label.setText(
                 f'Apriori probability of context "{context}.{instantiation}" is not a number')
 
-    def influence_values_changed(self, value, context, intention, instantiation):
+    def influence_values_changed(self, value, context, intention, instantiation, slider):
         """
         Callback for change of the influence values.
 
         Args:
             value: new influence value
             context: name of the context
             intention: name of the intention
             instantiation: name of the corresponding instantiation
+            slider: handle to the slider which should change its color
         """
         self.error_label.setText("")
         try:
             self.bayesNet.change_influence_value(
                 intention=intention, context=context, instantiation=instantiation, value=int(value))
+            slider.setStyleSheet(
+                f"QSlider::handle:horizontal {{background-color: {self.COLORS[value]}}}")
         except AssertionError as e:
             self.error_label.setText(str(e))
 
         return value
 
 
 class TwoLayerGraph(pg.GraphItem):
```

### Comparing `CoBaIR-2.1.0/CoBaIR/default_discretizer.py` & `CoBaIR-3.0.0/CoBaIR/default_discretizer.py`

 * *Files identical despite different names*

### Comparing `CoBaIR-2.1.0/CoBaIR/random_base_count.py` & `CoBaIR-3.0.0/CoBaIR/random_base_count.py`

 * *Files identical despite different names*

### Comparing `CoBaIR-2.1.0/CoBaIR.egg-info/PKG-INFO` & `CoBaIR-3.0.0/CoBaIR.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: CoBaIR
-Version: 2.1.0
-Summary: CoBaIR is a python lib for Context Based Intention Recognition
+Version: 3.0.0
+Summary: CoBaIR is a Python library for Context Based Intention Recognition
 Home-page: https://github.com/dfki-ric/CoBaIR
 Author: Adrian Lubitz
 Author-email: Adrian.Lubitz@dfki.de
 License: BSD 3-Clause
 Keywords: intention recognition context human machine interaction robot bayesian
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `CoBaIR-2.1.0/CoBaIR.egg-info/SOURCES.txt` & `CoBaIR-3.0.0/CoBaIR.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CoBaIR-2.1.0/LICENSE` & `CoBaIR-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CoBaIR-2.1.0/PKG-INFO` & `CoBaIR-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: CoBaIR
-Version: 2.1.0
-Summary: CoBaIR is a python lib for Context Based Intention Recognition
+Version: 3.0.0
+Summary: CoBaIR is a Python library for Context Based Intention Recognition
 Home-page: https://github.com/dfki-ric/CoBaIR
 Author: Adrian Lubitz
 Author-email: Adrian.Lubitz@dfki.de
 License: BSD 3-Clause
 Keywords: intention recognition context human machine interaction robot bayesian
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `CoBaIR-2.1.0/README.md` & `CoBaIR-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `CoBaIR-2.1.0/setup.py` & `CoBaIR-3.0.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,43 @@
-from setuptools import setup
-from setuptools import find_packages
-import CoBaIR
 import os
+from setuptools import setup, find_packages
 
-with open('requirements/requirements.txt') as f:
-    requirements = f.read().splitlines()
 
 # TODO: if TAG in pipeline given use tag
 if 'CI_COMMIT_TAG' in os.environ:
     VERSION = os.environ['CI_COMMIT_TAG']
 else:
     VERSION = '0.0.0'
 
-
-def read(fname):
-    return open(os.path.join(os.path.dirname(__file__), fname)).read()
+with open('requirements/requirements.txt', encoding='utf-8') as f:
+    requirements = f.read().splitlines()
 
 
-setup(name='CoBaIR',
-      version=VERSION,
-      description='CoBaIR is a python lib for Context Based Intention Recognition',
-      author='Adrian Lubitz',
-      author_email='Adrian.Lubitz@dfki.de',
-      license='BSD 3-Clause',
-      keywords="intention recognition context human machine interaction robot bayesian",
-      url="https://github.com/dfki-ric/CoBaIR",
-      install_requires=requirements,
-      packages=find_packages(),
-      long_description=read('README.md'),
-      long_description_content_type="text/markdown",
-      classifiers=[
-          "Development Status :: 3 - Alpha",
-          "Environment :: X11 Applications :: Qt",
-          "Intended Audience :: Science/Research",
-          "Programming Language :: Python :: 3.8",
-          "Topic :: Scientific/Engineering :: Artificial Intelligence",
-          "Topic :: Utilities",
-          "License :: OSI Approved :: BSD License",
-      ],
-      python_requires='>=3.8')
+def read(fname: str) -> str:
+    """Read the contents of a file and return it as a string."""
+    return open(os.path.join(os.path.dirname(__file__), fname), encoding='utf-8').read()
+
+
+setup(
+    name='CoBaIR',
+    version=VERSION,
+    description='CoBaIR is a Python library for Context Based Intention Recognition',
+    author='Adrian Lubitz',
+    author_email='Adrian.Lubitz@dfki.de',
+    license='BSD 3-Clause',
+    keywords="intention recognition context human machine interaction robot bayesian",
+    url="https://github.com/dfki-ric/CoBaIR",
+    install_requires=requirements,
+    packages=find_packages(),
+    long_description=read('README.md'),
+    long_description_content_type="text/markdown",
+    classifiers=[
+        "Development Status :: 3 - Alpha",
+        "Environment :: X11 Applications :: Qt",
+        "Intended Audience :: Science/Research",
+        "Programming Language :: Python :: 3.8",
+        "Topic :: Scientific/Engineering :: Artificial Intelligence",
+        "Topic :: Utilities",
+        "License :: OSI Approved :: BSD License",
+    ],
+    python_requires='>=3.8',
+)
```

### Comparing `CoBaIR-2.1.0/tests/test_add_context.py` & `CoBaIR-3.0.0/tests/test_add_context.py`

 * *Files identical despite different names*

### Comparing `CoBaIR-2.1.0/tests/test_add_intention.py` & `CoBaIR-3.0.0/tests/test_add_intention.py`

 * *Files identical despite different names*

### Comparing `CoBaIR-2.1.0/tests/test_create_bayesNet.py` & `CoBaIR-3.0.0/tests/test_create_bayesNet.py`

 * *Files identical despite different names*

### Comparing `CoBaIR-2.1.0/tests/test_delete_context.py` & `CoBaIR-3.0.0/tests/test_delete_context.py`

 * *Files identical despite different names*

### Comparing `CoBaIR-2.1.0/tests/test_delete_intention.py` & `CoBaIR-3.0.0/tests/test_delete_intention.py`

 * *Files identical despite different names*

### Comparing `CoBaIR-2.1.0/tests/test_edit_context.py` & `CoBaIR-3.0.0/tests/test_edit_context.py`

 * *Files identical despite different names*

### Comparing `CoBaIR-2.1.0/tests/test_edit_intention.py` & `CoBaIR-3.0.0/tests/test_edit_intention.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,32 +15,28 @@
 # end file header
 __author__ = 'Arunima Gopikrishnan'
 
 def test_edit_intention_from_empty():
     """
     Test editing on a non existing config
     """
-    bn = BayesNet()
-    old_config1 = deepcopy(bn.config)
+    bayes_net = BayesNet()
+    old_config1 = deepcopy(bayes_net.config)
     intention = 'hand over tool'
     new_name = 'entregar la herramienta'
     # I assume this will throw an Error!
     with pytest.raises(ValueError):
-        bn.edit_intention(intention, new_name=new_name)
-    assert old_config1 == bn.config
+        bayes_net.edit_intention(intention, new_name=new_name)
+    assert old_config1 == bayes_net.config
 
 def test_edit_intention_from_existing_new_name():
     """
     Test editing on an existing config - only changing the name of the intention
     """
-    bn = BayesNet()
-    bn.load('small_example.yml')
+    bayes_net = BayesNet()
+    bayes_net.load('small_example.yml')
     new_name = 'entregar la herramienta'
     old_intention = 'hand over tool'
-    old_config = deepcopy(bn.config)
-    # I assume this will throw an Error! 
-    bn.edit_intention(old_intention, new_name=new_name)
-    assert new_name in bn.config['intentions']
-    assert old_intention not in bn.config['intentions']
-
-
-
+    # I assume this will throw an Error!
+    bayes_net.edit_intention(old_intention, new_name=new_name)
+    assert new_name in bayes_net.config['intentions']
+    assert old_intention not in bayes_net.config['intentions']
```

### Comparing `CoBaIR-2.1.0/tests/test_infer.py` & `CoBaIR-3.0.0/tests/test_infer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 '''
 Tests for adding intention variables
 '''
 
 # System imports
-from copy import deepcopy
 import pytest
 
-# 3rd party imports
-
 # local imports
 from tests import N
 from CoBaIR.bayes_net import BayesNet, default_to_regular, load_config
 
 # end file header
 __author__ = 'Adrian Lubitz'
 bn = BayesNet()
@@ -21,80 +18,96 @@
 def test_infer_no_evidence():
     """
     Test inference without evidence
     """
     probabilities = {'pick up tool': 0.602803738317757,
                      'hand over tool': 0.397196261682243}
 
-    max_intention, inference = bn.infer({})
-    for intention, probability in inference.items():
-        assert round(abs(probability-probabilities[intention]), 7) == 0
+    max_intention, decision_threshold, inference = bn.infer({})
+    assert inference is not None, "No intention was inferred"
+    if max_intention is not None:
+        assert decision_threshold > 0
+        assert round(abs(inference - probabilities[max_intention]), 7) == 0
 
 
 def test_infer_unrelated_evidence():
     """
     Test inference with unrelated evidence of different types
     """
     probabilities = {'pick up tool': 0.602803738317757,
                      'hand over tool': 0.397196261682243}
 
-    max_intention, inference = bn.infer({'some context': 'is not important', 'another context': '',
-                                         'unhashable context': {}, 'int context': 1, 'obj context': bn})
-    for intention, probability in inference.items():
-        assert round(abs(probability-probabilities[intention]), 7) == 0
+    max_intention, decision_threshold, inference = bn.infer({'some context': 'is not important',
+                                                             'another context': '',
+                                                             'unhashable context': {},
+                                                             'int context': 1,
+                                                             'obj context': bn})
+
+    if max_intention is not None:
+        assert decision_threshold > 0
+        assert round(abs(inference - probabilities[max_intention]), 7) == 0
 
 
 def test_infer_single_evidence():
     """
     Test inference with single evidence context present
     """
     probabilities = {'pick up tool': 0.7821782178217822,
                      'hand over tool': 0.21782178217821785}
 
-    max_intention, inference = bn.infer(
+    max_intention, decision_threshold, inference = bn.infer(
         {'speech commands': 'pickup', 'unhashable context': {}})
     for intention, probability in inference.items():
         assert round(abs(probability-probabilities[intention]), 7) == 0
 
 
 def test_infer_multiple_evidence():
     """
     Test inference with multiple evidence context present
     """
     probabilities = {'hand over tool': 0.3797468354430379,
                      'pick up tool': 0.620253164556962}
 
-    max_intention, inference = bn.infer(
-        {'speech commands': 'pickup', 'human holding object': False, 'human activity': 'idle', 'unhashable context': {}})
+    max_intention, decision_threshold, inference = bn.infer({
+        'speech commands': 'pickup',
+        'human holding object': False,
+        'human activity': 'idle',
+        'unhashable context': {}
+    })
     for intention, probability in inference.items():
         assert round(abs(probability-probabilities[intention]), 7) == 0
 
 
 def test_infer_combined_evidence():
     """
     Test inference for the combined case
     """
     probabilities = {'hand over tool': 0.26229508196721313,
                      'pick up tool': 0.7377049180327869}
 
-    max_intention, inference = bn.infer(
-        {'speech commands': 'pickup', 'human holding object': True, 'human activity': 'idle', 'unhashable context': {}})
+    max_intention, decision_threshold, inference = bn.infer({
+        'speech commands': 'pickup',
+        'human holding object': True,
+        'human activity': 'idle',
+        'unhashable context': {}
+    })
     for intention, probability in inference.items():
         assert round(abs(probability-probabilities[intention]), 7) == 0
 
 
 def test_infer_overlapping_combined_evidence():
     """
     Test inference for combined case if two combinations are overlapping - not implemented yet!
     """
     # probabilities = {'hand over tool': 0.26229508196721313,
     #                  'pick up tool': 0.7377049180327869}
 
     # inference = self.bn.infer(
-    #     {'speech commands': 'pickup', 'human holding object': True, 'human activity': 'idle', 'unhashable context': {}})
+    #     {'speech commands': 'pickup',
+    # 'human holding object': True, 'human activity': 'idle', 'unhashable context': {}})
     # print(inference)
     # for intention, probability in inference.items():
     #     self.assertAlmostEqual(probability, probabilities[intention])
     pass
 
 
 def test_infer_invalid_evidence():
```

### Comparing `CoBaIR-2.1.0/tests/test_load.py` & `CoBaIR-3.0.0/tests/test_load.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 '''
 Tests for Loading yaml format config file
 '''
 
 # System imports
-import pytest
 from collections import defaultdict
+import pytest
+
 # 3rd party imports
 from yaml.parser import ParserError
 
 # local imports
 from tests import N
 from CoBaIR.bayes_net import BayesNet, load_config
 
@@ -51,22 +52,25 @@
 def test_loading_invalid_yml_file():
     """
     Test loading invalid file name
     """
 
     config = load_config('small_example_invalid.yml')
 
-    # I assume this will throw an Error!- AssertionError: Influence Value for pick up tool.speech commands.handover must be an integer between 0 and 5! Is 10
+    # I assume this will throw an Error!- 
+    # AssertionError: Influence Value for pick up tool.speech commands.
+    # handover must be an integer between 0 and 5! Is 10
     with pytest.raises(AssertionError):
         BayesNet(config)
-        assert BayesNet(config).valid == False
+        assert BayesNet(config).valid is False
 
 
 def test_loading_valid_yml_file():
     """
-    Test loading valid file name - validata_config() function will validate that the current config follows the correct format.
+    Test loading valid file name - validata_config() function will validate 
+        that the current config follows the correct format.
     """
 
     config = load_config('small_example.yml')
-    bn = BayesNet(config)
+    bayes_net = BayesNet(config)
     # valid config
-    assert bn.valid == True
+    assert bayes_net.valid is True
```

### Comparing `CoBaIR-2.1.0/tests/test_remove_combined_influence.py` & `CoBaIR-3.0.0/tests/test_remove_combined_influence.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,16 +29,17 @@
     with pytest.raises(ValueError):
         bn.del_combined_influence(intention, contexts, instantiations)
 
 
 
 def test_remove_existing_add_new_combined_context_influence():
     """
-    Test removing combined context influence from the loaded config's existing combined context influence
-    and adding combined context influence into the loaded config's existing combined context influence
+    Test removing combined context influence from the loaded config's 
+        existing combined context influence.
+    Adding combined context influence into the loaded config's existing combined context influence
     """
     
     bn = BayesNet()
     bn.load('small_example.yml')
     original_config = deepcopy(bn.config)
  #   for intention, context_influence in bn.config['intentions'].items():
 #            bn._create_combined_context(context_influence)
```


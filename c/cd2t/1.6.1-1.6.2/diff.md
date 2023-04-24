# Comparing `tmp/cd2t-1.6.1.tar.gz` & `tmp/cd2t-1.6.2.tar.gz`

## Comparing `cd2t-1.6.1.tar` & `cd2t-1.6.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     5897 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/DataParser.py
--rw-r--r--   0        0        0     9345 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/References.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/RunTimeEnv.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/__init__.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/results.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/schema.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/utils.py
--rw-r--r--   0        0        0     3215 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/types/List.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/types/NoneDataType.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/types/__init__.py
--rw-r--r--   0        0        0     7874 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/types/base.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/types/bool.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/types/datatype.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/types/enum.py
--rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/types/float.py
--rw-r--r--   0        0        0     7198 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/types/idlist.py
--rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/types/integer.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/types/multitype.py
--rw-r--r--   0        0        0    10171 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/types/object.py
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/types/schema.py
--rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/types/string.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cd2t-1.6.1/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 cd2t-1.6.1/LICENSE
--rw-r--r--   0        0        0    18056 2020-02-02 00:00:00.000000 cd2t-1.6.1/README.md
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 cd2t-1.6.1/pyproject.toml
--rw-r--r--   0        0        0    18703 2020-02-02 00:00:00.000000 cd2t-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0     8420 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/DataParser.py
+-rw-r--r--   0        0        0    14362 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/References.py
+-rw-r--r--   0        0        0     3468 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/RunTimeEnv.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/__init__.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/results.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/schema.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/utils.py
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/types/List.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/types/NoneDataType.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/types/__init__.py
+-rw-r--r--   0        0        0     7819 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/types/base.py
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/types/bool.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/types/datatype.py
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/types/enum.py
+-rw-r--r--   0        0        0     8600 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/types/float.py
+-rw-r--r--   0        0        0     7299 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/types/idlist.py
+-rw-r--r--   0        0        0     6899 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/types/integer.py
+-rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/types/multitype.py
+-rw-r--r--   0        0        0    10586 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/types/object.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/types/schema.py
+-rw-r--r--   0        0        0     5266 2020-02-02 00:00:00.000000 cd2t-1.6.2/cd2t/types/string.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cd2t-1.6.2/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 cd2t-1.6.2/LICENSE
+-rw-r--r--   0        0        0    18238 2020-02-02 00:00:00.000000 cd2t-1.6.2/README.md
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 cd2t-1.6.2/pyproject.toml
+-rw-r--r--   0        0        0    18885 2020-02-02 00:00:00.000000 cd2t-1.6.2/PKG-INFO
```

### Comparing `cd2t-1.6.1/cd2t/References.py` & `cd2t-1.6.2/cd2t/References.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,18 +9,98 @@
     PRODUCER_GLOBAL = 16
     CONSUMER = 32
     CONSUMER_GLOBAL = 64
     ALLOW_ORPHAN_PRODUCER = 128
 
 
 INIT_OPTIONS = OPT.UNIQUE | OPT.UNIQUE_GLOBAL | OPT.PRODUCER | OPT.PRODUCER_GLOBAL
+    
+
+class ReferenceError(Exception):
+    pass
+
+
+class ReferenceElement():
+    """ ReferenceElement stores all information regarding a reference value analyzed in data
+    """
+    def __init__(self,
+                 reference_key: str='',
+                 path: str='',
+                 value: any=None,
+                 options: OPT=INIT_OPTIONS,
+                 namespace: str='') -> None:
+        """
+        Args:
+            reference_key: string - Reference key from schema definition
+
+            path: string - Value's path in data structure
+
+            value: any - Value data
+
+            options: OPT object - indicator for reference options (mode, scope, ...)
+
+            namespace: string - active namepsace during reference creation
+        
+        Raises:
+            ValueError: If arg's data type is wrong.
+        """
+        if not isinstance(namespace, str): raise ValueError("'namespace' not a string")
+        self.namespace = namespace
+        if not isinstance(reference_key, str): raise ValueError("'reference' not a string")
+        self.reference_key = reference_key
+        if not isinstance(path, str): raise ValueError("'path' not a string")
+        self.path = path
+        if not isinstance(options, OPT): raise ValueError("'options' not a OPT object")
+        self.options = options
+        self.value = value
+        self.consumes_from = list()
+        self.provides_to = list()
+
+
+class ConsumerElement(ReferenceElement):
+    """
+    Sub-class to ReferenceElement
+    Specialized for Condumer References
+    """
+    def __init__(self,
+                 reference_key: str='',
+                 path: str='',
+                 value: any=None,
+                 options: OPT=INIT_OPTIONS,
+                 namespace: str='',
+                 provider_namespace: str='') -> None:
+        """
+        Args:
+            < ReferenceElement's arguements >
+
+            provider_namespace: string - namespace where to search for providers (namespace lookup feature)
+        
+        Raises:
+            ValueError: If arg's data type is wrong.
+        """
+        super().__init__(
+            reference_key=reference_key,
+            path=path,
+            value=value,
+            options=options,
+            namespace=namespace)
+        if not isinstance(provider_namespace, str): raise ValueError("'provider_namespace' not a string")
+        self.provider_namespace = provider_namespace
 
 
 class ReferenceFinding(Finding):
-    def __init__(self, message: str, path='', reference=None) -> None:
+    """
+    Sub-class to Finding
+    ReferenceFinding stores all information to a reference issue and 
+    provides a method to present all information as a string (makes it easy for user interfaces)
+    """
+    def __init__(self,
+                 message: str,
+                 path: str='',
+                 reference: ReferenceElement=None) -> None:
         super().__init__(message=message, path=path)
         self.reference = reference
     
     def __str__(self):
         ns_lookup = False
         if self.reference and isinstance(self.reference, ConsumerElement) \
                 and self.reference.provider_namespace:
@@ -34,39 +114,20 @@
             namespace = ''
         path = self.path + ': ' if self.path else ''
         message = f"{self.message} in '{self.reference.provider_namespace}'" \
                      if ns_lookup else self.message
         return namespace + path + message
     
 
-class ReferenceError(Exception):
-    pass
-
-
-class ReferenceElement():
-    def __init__(self, reference='', path='', value=None, options=INIT_OPTIONS, namespace='') -> None:
-        if not isinstance(namespace, str): raise ValueError("'namespace' not a string")
-        self.namespace = namespace
-        if not isinstance(reference, str): raise ValueError("'reference' not a string")
-        self.reference = reference
-        if not isinstance(path, str): raise ValueError("'path' not a string")
-        self.path = path
-        if not isinstance(options, OPT): raise ValueError("'options' not a OPT object")
-        self.options = options
-        self.value = value
-        self.consumes_from = list()
-        self.provides_to = list()
-
-class ConsumerElement(ReferenceElement):
-    def __init__(self, reference='', path='', value=None, options=INIT_OPTIONS, namespace='', provider_namespace='') -> None:
-        super().__init__(reference, path, value, options, namespace)
-        self.provider_namespace = provider_namespace
-    
-
 class GlobalSpace():
+    """
+    GlobalSpace is a space where to register references in global scope.
+    Adding References will stored according to the mode and
+    links (consumer<>producer) to other refererences will be created.
+    """
     uOPT = OPT.UNIQUE_GLOBAL
     pOPT = OPT.PRODUCER_GLOBAL
     cOPT = OPT.CONSUMER_GLOBAL
 
     def __init__(self) -> None:
         self.references = dict()
 
@@ -89,67 +150,101 @@
 
     def get_producers_by_ref_key(self, ref_key :str) -> list[ReferenceElement]:
         return self.references.get(ref_key, dict()).get('producers', list())
 
     def get_consumers_by_ref_key(self, ref_key :str) -> list[ReferenceElement]:
         return self.references.get(ref_key, dict()).get('consumers', list())
 
-    def get_unique_values_by_ref_key(self, ref_key :str) -> set:
+    def get_unique_values_by_ref_key(self, reference_key :str) -> set:
+        """
+        Returns:
+            list - with all 'unique' values with the same reference key
+        """
         unique_values = set()
-        for e in self.get_uniques_by_ref_key(ref_key):
+        for e in self.get_uniques_by_ref_key(reference_key):
             unique_values.add(e.value)
         return unique_values
 
-    def _add_ref_key(self, ref_key :str):
-        if ref_key in self.references.keys():
+    def _add_ref_key(self, reference_key :str):
+        """
+        If reference key is new to this space,
+        creates all required lists (unique,producers and consumers) for key 'ref_key' in references.
+
+        Args:
+            ref_key: string - reference key from schema definition
+        """
+        if reference_key in self.references.keys():
             return
-        self.references[ref_key] = dict(
+        self.references[reference_key] = dict(
             uniques=list(),
             producers=list(),
             consumers=list()
         )
     
-    def add_element(self, new_RE :ReferenceElement) -> list:
+    def add_element(self, new_RE :ReferenceElement) -> list[ReferenceElement]:
+        """
+        Add a new reference to the space, if reference options matches the class scope:
+        - stores reference according to mode in corresponding lists under the reference key
+        - create all links (consumer<>producer) to other references in this space
+
+        Args:
+            new_RE: ReferenceElement object - New reference for this space
+
+        Returns:
+            list of ReferenceElements - which were linked to the new reference
+        
+        Raises:
+            ReferenceError: If reference already in this space
+        """
         linked_elements = list()
-        self._add_ref_key(new_RE.reference)
+        self._add_ref_key(new_RE.reference_key)
         if self.uOPT in new_RE.options:
-            if self.get_uniques_by_value(new_RE.value, new_RE.reference):
+            if self.get_uniques_by_value(new_RE.value, new_RE.reference_key):
                 raise ReferenceError("Reference already defined")
-            self.references[new_RE.reference]['uniques'].append(new_RE)
+            self.references[new_RE.reference_key]['uniques'].append(new_RE)
         if self.pOPT in new_RE.options:
-            self.references[new_RE.reference]['producers'].append(new_RE)
+            self.references[new_RE.reference_key]['producers'].append(new_RE)
             linked_elements = self._link_to_consumers(new_RE)
         if self.cOPT in new_RE.options:
-            self.references[new_RE.reference]['consumers'].append(new_RE)
+            self.references[new_RE.reference_key]['consumers'].append(new_RE)
             linked_elements = self._link_to_producers(new_RE)
         return linked_elements
     
     def _link_to_producers(self, consumer :ReferenceElement) -> list[ReferenceElement]:
         producer_list = list()
-        for producer in self.references[consumer.reference]['producers']:
+        for producer in self.references[consumer.reference_key]['producers']:
             if consumer.value == producer.value and producer not in consumer.consumes_from:
                 # Maybe linking already from another NS or in Global
                 consumer.consumes_from.append(producer)
                 producer.provides_to.append(consumer)
                 producer_list.append(producer)
         return producer_list
     
     def _link_to_consumers(self, producer :ReferenceElement) -> list[ReferenceElement]:
         consumer_list = list()
-        for consumer in self.references[producer.reference]['consumers']:
+        for consumer in self.references[producer.reference_key]['consumers']:
             if producer.value == consumer.value and consumer not in producer.provides_to:
                 # Maybe linking already from another NS or in Global
                 producer.provides_to.append(consumer)
                 consumer.consumes_from.append(producer)
                 consumer_list.append(consumer)
         return consumer_list
     
-    def get_producer_consumer_issues(self):
+    def get_producer_consumer_issues(self) -> list[ReferenceFinding]:
+        """
+        Collects and returns
+        - all consumer references without a linked provider and
+        - all provider references without a linked consumer, if orphan procuders are not allowed,
+        as a list of ReferenceFindings
+
+        Returns:
+            list of ReferenceFindings
+        """
         results = list()
-        for ref_key, ref_lists in self.references.items():
+        for ref_lists in self.references.values():
             for consumer in ref_lists['consumers']:
                 if len(consumer.consumes_from) == 0:
                     # No producer found during analysis!
                     results.append(ReferenceFinding(path=consumer.path,
                                                     message="No producer found",
                                                     reference=consumer))
             for producer in ref_lists['producers']:
@@ -158,21 +253,29 @@
                     results.append(ReferenceFinding(path=producer.path,
                                                     message="Producer has no consumer",
                                                     reference=producer))
         return results
 
 
 class NameSpace(GlobalSpace):
+    """
+    Sub-class to GlobalSpace
+    Namespace is a space in namespace scope
+    """
     uOPT = OPT.UNIQUE
     pOPT = OPT.PRODUCER
     cOPT = OPT.CONSUMER
 
 
 class References():
-    def __init__(self, namespace=str()) -> None:
+    """
+    References stores all references according to the current active namespace and
+    according to the reference options (mode, scope, ...)
+    """
+    def __init__(self, namespace: str='') -> None:
         self.namespace = namespace
         self.globalspace_obj = GlobalSpace()
         self.ns_obj_store = dict()
         self._create_namespace(namespace)
         self.namespace_obj = self.ns_obj_store[namespace]
     
     def change_namespace(self, namespace :str) -> None:
@@ -180,41 +283,85 @@
         self.namespace_obj = self.ns_obj_store[namespace]
         self.namespace = namespace
 
     def _create_namespace(self, namespace :str) -> None:
         if namespace not in self.ns_obj_store.keys():
             self.ns_obj_store[namespace] = NameSpace()
     
-    def add_element(self, reference :ReferenceElement) -> list:
+    def add_element(self, reference :ReferenceElement) -> list[ReferenceElement]:
+        """
+        Add a new reference to the reference store, if reference options matches the class scope:
+        - add the reference to global space and
+        - if mode is consumer and provider namespace is given (namespace lookup),
+          add the reference to provider namespace,
+          else add the reference to the current active namespace
+
+        Args:
+            reference: ReferenceElement object - New reference for this store
+
+        Returns:
+            list of ReferenceElements - which were linked to the new reference
+        
+        Raises:
+            ReferenceError: If reference already in this store
+        """
         reference.namespace = self.namespace
         linked_elements = self.globalspace_obj.add_element(reference)
 
         if isinstance(reference, ConsumerElement) and reference.provider_namespace:
             self._create_namespace(reference.provider_namespace)
             linked_elements += self.ns_obj_store[reference.provider_namespace].add_element(reference)
         else:
             linked_elements += self.namespace_obj.add_element(reference)
         return linked_elements
     
     def get_producer_consumer_issues(self):
+        """
+        Collects and returns
+        - all consumer references without a linked provider and
+        - all provider references without a linked consumer, if orphan procuders are not allowed,
+        from all namespaces as a list of ReferenceFindings.
+        Note: As each reference in global space is also in a namespace, globalspace is skipped.
+
+        Returns:
+            list of ReferenceFindings
+        """
         results = list()
-        for namespace, ns_obj in self.ns_obj_store.items():
+        for ns_obj in self.ns_obj_store.values():
             results += ns_obj.get_producer_consumer_issues()
             # for r in _results:
             #     r.path = namespace+" > "+r.path
             #     results.append(r)
         return results
         
-    def same_unique(self, reference :str) -> list[ReferenceElement]:
+    def same_unique(self, reference :ReferenceElement) -> list[ReferenceElement]:
+        """
+        Returns first found 'unique' references with the same reference key and value as given reference.
+
+        Args:
+            reference: ReferenceElement
+
+        Returns:
+            list of ReferenceElements
+        """
         others = self.namespace_obj.get_uniques_by_value(
-            reference.value, reference.reference)
+            reference.value, reference.reference_key)
         if OPT.UNIQUE_GLOBAL in reference.options:
             others += self.globalspace_obj.get_uniques_by_value(
-                reference.value, reference.reference)
+                reference.value, reference.reference_key)
         if others:
             return others[0]
         return None
 
-    def get_unique_values_by_ref_key(self, ref_key :str) -> set:
-        ns_uniques = set(self.namespace_obj.get_unique_values_by_ref_key(ref_key))
-        global_unique = set(self.globalspace_obj.get_unique_values_by_ref_key(ref_key))
+    def get_unique_values_by_ref_key(self, reference_key :str) -> set:
+        """
+        Returns all found 'unique' values with the same reference key.
+
+        Args:
+            reference_key: string
+
+        Returns:
+            list of values
+        """
+        ns_uniques = set(self.namespace_obj.get_unique_values_by_ref_key(reference_key))
+        global_unique = set(self.globalspace_obj.get_unique_values_by_ref_key(reference_key))
         return ns_uniques.union(global_unique)
```

### Comparing `cd2t-1.6.1/cd2t/results.py` & `cd2t-1.6.2/cd2t/results.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,23 +11,32 @@
         _str = self.message
         if self.path:
             _str = self.path + ': ' + _str
         if self.namespace:
             _str = self.namespace + ' > ' + _str
         return _str
     
-    def __eg__(self, other):
+    def __eq__(self, other):
         return str(self) == str(other)
     
+    def __ne__(self, other):
+        return not self == other
+    
     def __gt__(self, other):
-        return str(self > str(other))
+        return str(self) > str(other)
+    
+    def __ge__(self, other):
+        return self > other or self == other
     
     def __lt__(self, other):
         return str(self) < str(other)
     
+    def __le__(self, other):
+        return self < other or self == other
+    
 
 class ValidationFinding(Finding):
     pass
 
     
 class DataTypeMismatch(ValidationFinding):
     pass
```

### Comparing `cd2t-1.6.1/cd2t/schema.py` & `cd2t-1.6.2/cd2t/schema.py`

 * *Files identical despite different names*

### Comparing `cd2t-1.6.1/cd2t/utils.py` & `cd2t-1.6.2/cd2t/utils.py`

 * *Files identical despite different names*

### Comparing `cd2t-1.6.1/cd2t/types/List.py` & `cd2t-1.6.2/cd2t/types/List.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,66 +12,64 @@
         # option_name, required, class
         ('minimum', False, int, None),
         ('maximum', False, int, None),
         ('allow_duplicates', False, bool, True),
         ('elements', True, [dict, str], dict()),
     ]
 
-    def __init__(self, RTE :RunTimeEnv) -> None:
-        super().__init__(RTE=RTE)
+    def __init__(self) -> None:
+        super().__init__()
         self.minimum = None
         self.maximum = None
         self.allow_duplicates = True
         self.elements = dict()
         self.element_data_type = None
     
-    def build_schema(self, schema :dict, path :str, subschemas :dict, subpath :list):
-        self.__init__(RTE=self.RTE)
+    def build_schema(self, schema :dict, path :str, subschemas :dict, subpath :list, RTE :RunTimeEnv):
+        self.__init__()
         path = path + self.path_symbol
         self.load_schema_options(schema, path)
 
-        self.element_data_type = self._get_data_type('elements', path + 'elements')
+        self.element_data_type = self._get_data_type('elements', path + 'elements', RTE)
         # Save recursively detected data type (i.e. from 'schema' --> subschema)
         self.element_data_type = self.element_data_type.build_schema(
             schema=self.elements, path=path,
-            subschemas=subschemas, subpath=subpath)
+            subschemas=subschemas, subpath=subpath,
+            RTE=RTE)
         return self
     
-    def build_sub_references(self, data :any, path :str):
+    def build_sub_references(self, data :any, path :str, RTE :RunTimeEnv):
         i = 0
         for element in data:
-            self.element_data_type.build_references(element, "%s[%d]" % (path, i))
+            self.element_data_type.build_references(element, "%s[%d]" % (path, i), RTE)
             i += 1
     
-    def autogenerate_data(self, data :any, path :str):
+    def autogenerate_data(self, data :any, path :str, RTE :RunTimeEnv):
         FL = FindingsList()
         if not self.data_matches_type(data):
             return data, FL
-        new_list = list()
-        i = 0
-        for element in data:
-            _data, _FL = self.element_data_type.autogenerate_data(element, "%s[%d]" % (path, i))
-            new_list.append(_data)
+        for i in range(len(data)):
+            _data, _FL = self.element_data_type.autogenerate_data(data[i], "%s[%d]" % (path, i), RTE)
+            data[i] = _data
             FL += _FL
-            i += 1
-        return new_list, FL
+        return data, FL
 
-    def verify_data(self, data :any, path :str) -> FindingsList:
+    def verify_data(self, data :any, path :str, RTE :RunTimeEnv) -> FindingsList:
         FL = FindingsList()
         if self.minimum and len(data) < self.minimum:
             FL.append(WrongValueFinding(
                         path=path,
                         message='Length of list is lower than %d' % self.minimum))
         elif self.maximum and len(data) > self.maximum:
             FL.append(WrongValueFinding(
                         path=path,
                         message='Length of list is greater than %d' % self.maximum))
         i = 0
         for element in data:
-            FL += self.element_data_type.validate_data(element, "%s[%d]" % (path, i))
+            FL += self.element_data_type.validate_data(element, "%s[%d]" % (path, i), RTE)
             i += 1
         
         if not self.allow_duplicates:
             remaining_data = copy.copy(data)
             i = 0 
             for element in data:
                 remaining_data = remaining_data[1:]
```

### Comparing `cd2t-1.6.1/cd2t/types/base.py` & `cd2t-1.6.2/cd2t/types/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,55 +11,52 @@
     path_symbol = '*'
     matching_classes = []
     options = [
         # option_name, required?, class, init_value
     ]
     support_reference = False
 
-    def __init__(self, RTE :RunTimeEnv) -> None:
-        if not isinstance(RTE, RunTimeEnv):
-            raise ValueError("'RTE' must be an object of class 'RunTimeEnv'")
-        self.RTE = RTE
+    def __init__(self) -> None:
         self.ref_OPT = OPT.NONE
         self.ref_key = ''
         self.data_type_mismatch_message = "Value is not '%s'" % self.type
         return
     
     def data_matches_type(self, data :any) -> bool:
         if self.type == 'any':
             return True
         for cls in self.matching_classes:
             if isinstance(data, cls):
                 return True
         return False
     
-    def build_schema(self, schema :dict, path :str, subschemas :dict, subpath :list):
-        self.__init__(self.RTE)
+    def build_schema(self, schema :dict, path :str, subschemas :dict, subpath :list, RTE :RunTimeEnv):
+        self.__init__()
         path = path + self.path_symbol
         self.load_reference_option(schema, path)
         self.load_schema_options(schema, path)
         self.verify_options(path=path)
         return self
     
-    def _get_data_type(self, option :str, path :str) -> DataType:
+    def _get_data_type(self, option :str, path :str, RTE :RunTimeEnv) -> DataType:
         schema = self.__dict__[option]
         if isinstance(schema, dict):
             if len(schema) == 0:
-                return BaseDataType(RTE=self.RTE)
+                return BaseDataType()
             if not 'type' in schema.keys():
                 raise SchemaError("Needs to have a key 'type'", path)
             data_type_name = schema['type']
-        elif self.RTE.allow_shortcuts and isinstance(schema, str):
+        elif RTE.allow_shortcuts and isinstance(schema, str):
             data_type_name = schema
             self.__dict__[option] = dict()
         else:
             raise SchemaError("Wrong value type", path)
         
         try:
-            data_type = self.RTE.get_data_type_class(data_type_name)(RTE=self.RTE)
+            data_type = RTE.get_data_type_class(data_type_name)()
         except SchemaError:
             raise SchemaError("Data type '%s' not found" % data_type_name, path)
         return data_type
 
     
     def load_reference_option(self, schema :dict, path :str):
         if not self.support_reference or 'reference' not in schema.keys():
@@ -131,57 +128,57 @@
                 schema.pop(option, None)
             elif required:
                 raise SchemaError("Key missing", path + option)
         if len(schema):
             raise SchemaError("Unknown option keys '%s'" % ', '.join(schema.keys()), path)
         return
 
-    def validate_data(self, data :any, path :str) -> FindingsList:
+    def validate_data(self, data :any, path :str, RTE :RunTimeEnv) -> FindingsList:
         FL = FindingsList()
         if not self.data_matches_type(data):
             FL.append(DataTypeMismatch(path=path, message=self.data_type_mismatch_message))
             return FL
-        FL += self.verify_reference(data, path)
-        FL += self.verify_data(data, path)
+        FL += self.verify_reference(data, path, RTE)
+        FL += self.verify_data(data, path, RTE)
         return FL
 
-    def verify_data(self, data :any, path :str) -> FindingsList:
+    def verify_data(self, data :any, path :str, RTE :RunTimeEnv) -> FindingsList:
         return FindingsList()
     
-    def build_sub_references(self, data :any, path :str) -> None:
+    def build_sub_references(self, data :any, path :str, RTE :RunTimeEnv) -> None:
         return
     
-    def build_references(self, data :any, path :str) -> None:
+    def build_references(self, data :any, path :str, RTE :RunTimeEnv) -> None:
         if self.data_matches_type(data):
-            self.verify_reference(data=data, path=path)
-            self.build_sub_references(data=data, path=path)
+            self.verify_reference(data=data, path=path, RTE=RTE)
+            self.build_sub_references(data=data, path=path, RTE=RTE)
     
-    def autogenerate_data(self, data :any, path :str):
+    def autogenerate_data(self, data :any, path :str, RTE :RunTimeEnv):
         return data, FindingsList()
     
     def get_reference_data(self, data :any, path :str) -> any:
         return data, FindingsList()
     
     def get_reference_element(self, path :str, ref_data :any) -> any:
         return ReferenceElement(self.ref_key, path, ref_data, self.ref_OPT)
     
-    def verify_reference(self, data :any, path :str) -> FindingsList:
+    def verify_reference(self, data :any, path :str, RTE :RunTimeEnv) -> FindingsList:
         FL = FindingsList()
         if not self.support_reference or OPT.NONE in self.ref_OPT:
             return FL
         ref_data, _FL = self.get_reference_data(data, path)
         FL += _FL
         ref_element = self.get_reference_element(path, ref_data)
         if OPT.UNIQUE in self.ref_OPT:
-            other = self.RTE.references.same_unique(ref_element)
+            other = RTE.references.same_unique(ref_element)
             if other is not None:
-                if other.namespace != self.RTE.references.namespace:
+                if other.namespace != RTE.references.namespace:
                     _path = "%s > %s" % (other.namespace, other.path)
                 else:
                     _path = other.path
                 FL.append(ReferenceFinding(
                     path=path,message="Unique value already used at '%s'" % _path,
                     reference=ref_element))
                 return FL
         # If unique or just for producer/consumer mapping, add element to references
-        self.RTE.references.add_element(ref_element)
+        RTE.references.add_element(ref_element)
         return FL
```

### Comparing `cd2t-1.6.1/cd2t/types/bool.py` & `cd2t-1.6.2/cd2t/types/bool.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,36 +12,34 @@
     options = [
         # option_name, required, class
         ('autogenerate', False, bool, False),
         ('autogenerate_default', False, bool, None),
         ('allowed_value', False, bool, None)
     ]
 
-    def __init__(self, RTE :RunTimeEnv) -> None:
-        super().__init__(RTE=RTE)
+    def __init__(self) -> None:
+        super().__init__()
         self.autogenerate = False
         self.autogenerate_default = None
         self.allowed_value = None
     
     def verify_options(self, path: str):
         if self.autogenerate:
             if self.autogenerate_default is None:
                 raise SchemaError("'autogenerate_default' is required, if autogenerate is enabled", path)
             elif self.allowed_value is not None and self.autogenerate_default != self.allowed_value:
                 raise SchemaError("'allowed_value' and 'autogenerate_default' must be equal", path)
-
-
  
-    def verify_data(self, data :any, path :str) -> FindingsList:
+    def verify_data(self, data :any, path :str, RTE :RunTimeEnv) -> FindingsList:
         FL = FindingsList()
         if self.allowed_value is not None and data != self.allowed_value:
             FL.append(ValidationFinding(path=path, message='Value is not allowed'))
         return FL
     
-    def autogenerate_data(self, data :any, path :str):
+    def autogenerate_data(self, data :any, path :str, RTE :RunTimeEnv):
         FL = FindingsList()
         if data is not None or not self.autogenerate:
             return data, FL
         new_value = self.autogenerate_default
         FL.append(AutogenerationInfo(
                     path=path,
                     message='Autogenerated value is %s' % str(new_value)))
```

### Comparing `cd2t-1.6.1/cd2t/types/enum.py` & `cd2t-1.6.2/cd2t/types/enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,28 +9,28 @@
     path_symbol = '<<'
     options = [
         # option_name, required, class
         ('allowed_values', True, list, None),
     ]
     supported_data_types = [int, float, dict, list, str]
 
-    def __init__(self, RTE :RunTimeEnv) -> None:
-        super().__init__(RTE=RTE)
+    def __init__(self) -> None:
+        super().__init__()
         self.matching_classes = []
         self.allowed_values = None
         self.data_type_mismatch_message = "None of the allowed value data types matches"
     
     def verify_options(self, path: str):
         if not len(self.allowed_values):
             raise SchemaError("'allowed_values' must have at least one element", path)
         for value in self.allowed_values:
             value_type = type(value)
             if value_type not in self.supported_data_types:
                 raise SchemaError("'allowed_values' contains unsupported data types", path)
             if value_type not in self.matching_classes:
                 self.matching_classes.append(value_type)
 
-    def verify_data(self, data :any, path :str) -> FindingsList:
+    def verify_data(self, data :any, path :str, RTE :RunTimeEnv) -> FindingsList:
         FL = FindingsList()
         if data not in self.allowed_values:
             FL.append(WrongValueFinding(path=path, message='Value not allowed'))
         return FL
```

### Comparing `cd2t-1.6.1/cd2t/types/float.py` & `cd2t-1.6.2/cd2t/types/float.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,16 @@
         ('autogenerate', False, bool, False),
         ('autogenerate_default', False, float, None),
         ('autogenerate_ranges', False, list, list()),
         ('autogenerate_random_tries', False, int, 10),
         ('autogenerate_random_decimals', False, int, 2),
     ]
 
-    def __init__(self, RTE :RunTimeEnv) -> None:
-        super().__init__(RTE=RTE)
+    def __init__(self) -> None:
+        super().__init__()
         self.minimum = None
         self.maximum = None
         self.maximum_decimals = None
         self.allowed_values = list()
         self.allowed_dic = dict(
             discrete=list(),  # of floats
             round=list(),     # of tuples (decimals :int, matches :float)
@@ -108,15 +108,15 @@
                     and e[min] <= e[max]:
                 self.autogen_ranges.append((e[min], e[max]))
             else:
                 raise SchemaError(
                     "'autogenerate_ranges' contains unsupported directive at position %d" % i, path)
             i += 1
  
-    def verify_data(self, data :any, path :str) -> FindingsList:
+    def verify_data(self, data :any, path :str, RTE :RunTimeEnv) -> FindingsList:
         def matches_values(value :float, value_dic :dict):
             if value in value_dic['discrete']:
                 return True
             for _round, _match in value_dic['round']:
                 if round(value, _round) == _match:
                     return True
             for _min, _max in value_dic['ranges']:
@@ -137,15 +137,15 @@
                 % (data, self.maximum_decimals), path))
         if matches_values(data, self.not_allowed_dic) \
                 or (self.allowed_values and not matches_values(data, self.allowed_dic)):
             FL.append(WrongValueFinding(
                 path=path, message='%s is not allowed' % data))
         return FL
     
-    def autogenerate_data(self, data :any, path :str):
+    def autogenerate_data(self, data :any, path :str, RTE :RunTimeEnv):
         FL = FindingsList()
         if data is not None or not self.autogenerate:
             return data, FL
         # We need to autogenerate
         new_value = None
         new_element = None
         if self.autogenerate_default:
@@ -156,22 +156,22 @@
                 if not self.autogenerate_ranges:
                     min = self.minimum
                     max = self.maximum
                 else:
                     random_list_key = round(random.uniform(1, len(self.autogen_ranges)))
                     min, max = self.autogen_ranges[random_list_key - 1]
                 random_float = round(random.uniform(min, max), self.autogenerate_random_decimals)
-                results = self.verify_data(random_float, path)
+                results = self.verify_data(random_float, path, RTE)
                 if not len(results):
                     if not OPT.NONE in self.ref_OPT:
                         new_element = ReferenceElement(self.ref_key, path, random_float, self.ref_OPT)
                         if OPT.UNIQUE in self.ref_OPT and \
-                                self.RTE.references.same_unique(new_element) is not None:
+                                RTE.references.same_unique(new_element) is not None:
                             continue
-                        self.RTE.references.add_element(new_element)
+                        RTE.references.add_element(new_element)
                     new_value = random_float
                     break
         if new_value is None:
             FL.append(AutogenerationError(
                 path=path,
                 message='Failed to find a valid random value after %d tries.' % self.autogenerate_random_tries))
         else:
```

### Comparing `cd2t-1.6.1/cd2t/types/idlist.py` & `cd2t-1.6.2/cd2t/types/idlist.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,58 +19,58 @@
         ('id_type', False, str, 'string'),
         ('id_minimum', False, int, None),
         ('id_maximum', False, int, None),
         ('allowed_ids', False, list, None),
         ('not_allowed_ids', False, list, list()),
     ]
 
-    def __init__(self, RTE :RunTimeEnv) -> None:
-        super().__init__(RTE=RTE)
+    def __init__(self) -> None:
+        super().__init__()
         self.minimum = None
         self.maximum = None
         self.elements = None
         self.element_type = None
         self.id_type = 'string'
         self.id_minimum = None
         self.id_maximum = None
         self.allowed_ids = None
         self.not_allowed_ids = list()
     
-    def build_schema(self, schema :dict, path :str, subschemas :dict, subpath :list):
-        self.__init__(RTE=self.RTE)
+    def build_schema(self, schema :dict, path :str, subschemas :dict, subpath :list, RTE :RunTimeEnv):
+        self.__init__()
         path = path + self.path_symbol
         self.load_reference_option(schema, path)
         self.load_schema_options(schema, path)
 
         if self.id_type not in ['string', 'integer']:
             raise SchemaError("id_type '%s' is not valid" % self.id_type, path)
-        self.element_type = self._get_data_type('elements', path + 'elements')
+        self.element_type = self._get_data_type('elements', path + 'elements', RTE)
         # Save recursively detected data type (i.e. from 'schema' --> subschema)
         self.element_type = self.element_type.build_schema(
-            schema=self.elements, path=path, subschemas=subschemas, subpath=subpath)
+            schema=self.elements, path=path, subschemas=subschemas, subpath=subpath, RTE=RTE)
         return self
     
-    def build_sub_references(self, data :any, path :str):
+    def build_sub_references(self, data :any, path :str, RTE :RunTimeEnv):
         for id, element in data.items():
-            self.element_type.build_references(data=element, path=path + self.path_symbol)
+            self.element_type.build_references(data=element, path=path + self.path_symbol, RTE=RTE)
     
-    def autogenerate_data(self, data :any, path :str):
+    def autogenerate_data(self, data :any, path :str, RTE :RunTimeEnv):
         FL = FindingsList()
         if not self.data_matches_type(data):
             return data, FL
-        new_dict = dict()
         for id, element in data.items():
             new_path = path + '{}' + str(id)
             _data, _FL = self.element_type.autogenerate_data(data=element,
-                                                            path=new_path)
-            new_dict[id] = _data
+                                                            path=new_path,
+                                                            RTE=RTE)
+            data[id] = _data
             FL += _FL
-        return new_dict, FL
+        return data, FL
 
-    def verify_data(self, data :any, path :str) -> FindingsList:
+    def verify_data(self, data :any, path :str, RTE :RunTimeEnv) -> FindingsList:
         FL = FindingsList()
         path = path + '{}'
         if self.minimum and len(data) < self.minimum:
             FL.append(WrongValueFinding(
                         path=path,
                         message='Attribute count is lower than minimum %d' % self.minimum))
         elif self.maximum is not None and len(data) > self.maximum:
@@ -132,30 +132,30 @@
                         message="Attribute is not allowed"))
                 elif self.allowed_ids and id not in self.allowed_ids:
                     _FL.append(WrongValueFinding(
                         path=id_path,
                         message="Attribute is not an allowed value"))
 
             if not _FL:
-                FL += (self.element_type.validate_data(data=element, path=id_path))
+                FL += (self.element_type.validate_data(data=element, path=id_path, RTE=RTE))
             else:
                 FL += _FL
         return FL
 
-    def verify_reference(self, data :any, path :str) -> FindingsList:
+    def verify_reference(self, data :any, path :str, RTE :RunTimeEnv) -> FindingsList:
         if not self.data_matches_type(data) or OPT.NONE in self.ref_OPT:
             return []
         results = list()
         for id in data.keys():
             id_path = path + '{}' + id
             element = ReferenceElement(self.ref_key, id_path, id, self.ref_OPT)
-            other = self.RTE.references.same_unique(element)
+            other = RTE.references.same_unique(element)
             if other is not None:
-                if self.RTE.namespace != other.namespace:
+                if RTE.namespace != other.namespace:
                     _path = "%s > %s" % (other.namespace, other.path)
                 else:
                     _path = other.path
                 results.append(UniqueErrorFinding(
                     path=id_path, message="ID '%s' already used at '%s'" % (str(id), _path)))
             else:
-                self.RTE.references.add_element(element)
+                RTE.references.add_element(element)
         return results
```

### Comparing `cd2t-1.6.1/cd2t/types/integer.py` & `cd2t-1.6.2/cd2t/types/integer.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,16 +20,16 @@
         ('autogenerate', False, bool, False),
         ('autogenerate_default', False, int, None),
         ('autogenerate_maximum', False, int, None),
         ('autogenerate_minimum', False, int, None),
         ('autogenerate_find', False, str, 'next_higher'),
     ]
 
-    def __init__(self, RTE :RunTimeEnv) -> None:
-        super().__init__(RTE=RTE)
+    def __init__(self) -> None:
+        super().__init__()
         self.minimum = None
         self.maximum = None
         self.not_allowed_values = list()
         self.autogenerate = False
         self.autogenerate_default = None
         self.autogenerate_find = 'next_higher'
         self.autogenerate_minimum = None
@@ -53,76 +53,76 @@
             elif self.autogenerate_find == 'random' \
                     and (not (self.autogenerate_minimum or self.minimum) \
                               or not (self.autogenerate_maximum or self.maximum)):
                 raise SchemaError("Option 'autogenerate_find' as 'random' needs " +\
                                   "'minimum' or 'autogenerate_minimum' and " +\
                                   "'maximum' or 'autogenerate_maximum' to be set", path)
     
-    def autogenerate_data(self, data :any, path :str):
+    def autogenerate_data(self, data :any, path :str, RTE :RunTimeEnv):
         FL = FindingsList()
         if data is not None or not self.autogenerate:
             return data, FL
         # We need to autogenerate
         if self.autogenerate_default is not None:
             data = self.autogenerate_default
         
         elif self.autogenerate_find == 'next_lower':
             start = self.autogenerate_maximum if self.autogenerate_maximum is not None else self.maximum
             end = self.autogenerate_minimum if self.autogenerate_minimum is not None else self.minimum
             if OPT.UNIQUE not in self.ref_OPT:
                 data = start
             else:
-                all_uniques = self.RTE.references.get_unique_values_by_ref_key(self.ref_key)
+                all_uniques = RTE.references.get_unique_values_by_ref_key(self.ref_key)
                 blocked = all_uniques.union(set(self.not_allowed_values))
                 _iter = itertools.filterfalse(blocked.__contains__, itertools.count(start=start, step=-1))
                 data = next(_iter)
                 if end is not None and data < end:
                     data = None
                 else:
                     new_element = ReferenceElement(self.ref_key, path, data, self.ref_OPT)
-                    self.RTE.references.add_element(new_element)
+                    RTE.references.add_element(new_element)
                 
         elif self.autogenerate_find == 'next_higher':
             start = self.autogenerate_minimum if self.autogenerate_minimum is not None else self.minimum
             end = self.autogenerate_maximum if self.autogenerate_maximum is not None else self.maximum
             if OPT.UNIQUE not in self.ref_OPT:
                 data = start
             else:
-                all_uniques = self.RTE.references.get_unique_values_by_ref_key(self.ref_key)
+                all_uniques = RTE.references.get_unique_values_by_ref_key(self.ref_key)
                 blocked = all_uniques.union(set(self.not_allowed_values))
                 _iter = itertools.filterfalse(blocked.__contains__, itertools.count(start=start, step=1))
                 data = next(_iter)
                 if end is not None and data > end:
                     data = None
                 else:
                     new_element = ReferenceElement(self.ref_key, path, data, self.ref_OPT)
-                    self.RTE.references.add_element(new_element)
+                    RTE.references.add_element(new_element)
         
         elif self.autogenerate_find == 'random':
             start = self.autogenerate_minimum if self.autogenerate_minimum is not None else self.minimum
             end = self.autogenerate_maximum if self.autogenerate_maximum is not None else self.maximum
             min_max_values = set(range(start, end + 1))
             allowed_values = min_max_values - set(self.not_allowed_values)
             if allowed_values and OPT.UNIQUE in self.ref_OPT:
-                available_values = allowed_values - self.RTE.references.get_unique_values_by_ref_key(self.ref_key)
+                available_values = allowed_values - RTE.references.get_unique_values_by_ref_key(self.ref_key)
                 if available_values:
                     data = list(available_values)[random.randint(0, len(available_values)-1)]
                     new_element = ReferenceElement(self.ref_key, path, data, self.ref_OPT)
-                    self.RTE.references.add_element(new_element)
+                    RTE.references.add_element(new_element)
             elif allowed_values:
                 data = list(allowed_values)[random.randint(0, len(allowed_values)-1)]
         
         if data is None:
             FL.append(AutogenerationError(path=path, message='All values in use!'))
         else:
             FL.append(AutogenerationInfo(
                 path=path, message='Autogenerated value is %d' % data))
         return data, FL
  
-    def verify_data(self, data :any, path :str) -> FindingsList:
+    def verify_data(self, data :any, path :str, RTE :RunTimeEnv) -> FindingsList:
         FL = FindingsList()
         if self.minimum is not None and self.minimum > data:
             FL.append(WrongValueFinding(
                 path=path, message='%d is lower than minimum %d' % (data, self.minimum)))
         elif self.maximum is not None and self.maximum < data:
             FL.append(WrongValueFinding(
                 path=path, message='%d is higher than maximum %d' % (data, self.maximum)))
```

### Comparing `cd2t-1.6.1/cd2t/types/multitype.py` & `cd2t-1.6.2/cd2t/types/multitype.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,63 +8,64 @@
     type = 'multitype'
     path_symbol = '?'
     options = [
         # option_name, required, class
         ('types', True, list, None),
     ]
 
-    def __init__(self, RTE :RunTimeEnv) -> None:
-        super().__init__(RTE=RTE)
+    def __init__(self) -> None:
+        super().__init__()
         self.types = None
         self.type_objects = list()
         self.tmp_type = None
         self.matching_classes = []
         self.data_type_mismatch_message = "None of the data types matches"
     
-    def build_schema(self, schema :dict, path :str, subschemas :dict, subpath :list):
-        self.__init__(RTE=self.RTE)
+    def build_schema(self, schema :dict, path :str, subschemas :dict, subpath :list, RTE :RunTimeEnv):
+        self.__init__()
         path = path + self.path_symbol
         self.load_schema_options(schema, path)
         i = 0
         for _type in self.types:
             _path = "%stypes[%d]" % (path, i)
             if isinstance(_type, dict) and not len(_type):
                 raise SchemaError('Empty dictionary is not allowed', _path)
             self.tmp_type = _type
-            data_type = self._get_data_type('tmp_type', _path)
+            data_type = self._get_data_type('tmp_type', _path, RTE)
             if data_type.type == self.type:
                 raise SchemaError("Multitype in Multitype not supported", _path)
             data_type = data_type.build_schema(
                 schema=self.tmp_type, path=path,
-                subschemas=subschemas, subpath=subpath)
+                subschemas=subschemas, subpath=subpath,
+                RTE=RTE)
             self.type_objects.append(data_type)
             self.matching_classes.extend(data_type.matching_classes)
             i += 1
         return self
 
-    def build_sub_references(self, data :any, path :str) -> list:
+    def build_sub_references(self, data :any, path :str, RTE :RunTimeEnv) -> list:
         for type_object in self.type_objects:
             if type_object.data_matches_type(data):
-                type_object.build_references(data=data, path=path)
+                type_object.build_references(data=data, path=path, RTE=RTE)
     
-    def autogenerate_data(self, data :any, path :str):
+    def autogenerate_data(self, data :any, path :str, RTE :RunTimeEnv):
         FL = FindingsList()
         if data is None:
             return data, FL
         # Try to find ...
         for type_object in self.type_objects:
             if type_object.data_matches_type:
-                FL += type_object.autogenerate_data(data=data, path=path)
+                FL += type_object.autogenerate_data(data=data, path=path, RTE=RTE)
         return data, FL
 
-    def validate_data(self, data :any, path :str) -> list:
+    def validate_data(self, data :any, path :str, RTE=RunTimeEnv) -> list:
         FL = FindingsList()
         FL_without_direct_findings = False
         for type_object in self.type_objects:
-            _FL = type_object.validate_data(data=data, path=path)
+            _FL = type_object.validate_data(data=data, path=path, RTE=RTE)
             if _FL:
                 if not FL_without_direct_findings and \
                         len(_FL[0].path) > len(path) + 2:
                     # Path in first finding is not from direct specified data type
                     # -> is comming from sub data types. So first level is 100% fine.
                     FL = _FL
                     FL_without_direct_findings = True
```

### Comparing `cd2t-1.6.1/cd2t/types/object.py` & `cd2t-1.6.2/cd2t/types/object.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,29 +17,29 @@
         ('dependencies', False, dict, dict()),
         ('reference_attributes', False, list, None),
         ('ignore_undefined_attributes', False, bool, False),
         ('allow_regex_attributes', False, bool, False),
         ('autogenerate', False, bool, True)
     ]
 
-    def __init__(self, RTE :RunTimeEnv) -> None:
-        super().__init__(RTE=RTE)
+    def __init__(self) -> None:
+        super().__init__()
         self.attributes = None
         self.attributes_objects = dict()
         self.tmp_a_schema = None
         self.required_attributes = list()
         self.dependencies = dict()
         self.reference_attributes = None
         self.ignore_undefined_attributes = False
         self.allow_regex_attributes = False
         self.autogenerate = True
         return
     
-    def build_schema(self, schema :dict, path :str, subschemas :dict, subpath :list):
-        self.__init__(RTE=self.RTE)
+    def build_schema(self, schema :dict, path :str, subschemas :dict, subpath :list, RTE :RunTimeEnv):
+        self.__init__()
         path = path + self.path_symbol
         self.load_reference_option(schema, path)
         self.load_schema_options(schema, path)
         if self.attributes is None:
             # No other options should be set:
             for option, required, cls, init_value in self.options:
                 if exec("self." + option + " != init_value"):
@@ -68,58 +68,67 @@
                 if not self._attribute_in_list(ex_attr, list(self.attributes.keys()), self.allow_regex_attributes):
                     raise SchemaError("Excluded attribute '%s' " % ex_attr +\
                                       "for dependency '%s' not in attributes" % dep_attr, path)
         #
         for a_name, a_schema in self.attributes.items():
             a_path = path + a_name
             self.tmp_a_schema = a_schema
-            data_type = self._get_data_type('tmp_a_schema', a_path)
+            data_type = self._get_data_type('tmp_a_schema', a_path, RTE)
             # Save recursively detected data type (i.e. from 'schema' --> subschema)
-            self.attributes_objects[a_name] = data_type.build_schema(self.tmp_a_schema, a_path, subschemas, subpath)
+            self.attributes_objects[a_name] = data_type.build_schema(self.tmp_a_schema, a_path, subschemas, subpath, RTE)
         return self
     
-    def build_references(self, data :any, path :str):
+    def build_references(self, data :any, path :str, RTE :RunTimeEnv):
         for a_name, a_data in data.items():
             data_type = self._get_attribute_object(a_name, self.allow_regex_attributes)
             if data_type is None:
                 continue
             a_path = path + self.path_symbol + a_name
-            data_type.build_references(a_data, a_path)
+            data_type.build_references(a_data, a_path, RTE)
     
-    def autogenerate_data(self, data :any, path :str):
+    def autogenerate_data(self, data :any, path :str, RTE :RunTimeEnv):
         FL = FindingsList()
         if data is None or not self.data_matches_type(data):
             return data, FL
-        new_data = dict()
-        processed_attributes = list()
         if not self.allow_regex_attributes and self.autogenerate:
+            if RTE.ruamel_yaml_available and isinstance(data, RTE.CommentedMap):
+                new_data = data
+                insert = True
+            else:
+                new_data = dict()
+                insert = False
+            i = 0
             for a_name, data_type in self.attributes_objects.items():
-                processed_attributes.append(a_name)
                 a_path = path + self.path_symbol + a_name
                 _FL = FindingsList()
                 if a_name not in data.keys():
-                    _data, _FL = data_type.autogenerate_data(data=None, path=a_path)
+                    _data, _FL = data_type.autogenerate_data(data=None, path=a_path, RTE=RTE)
                     if _FL:
-                        new_data[a_name] = _data
+                        if insert:
+                            new_data.insert(pos=i, key=a_name, value=_data, comment='autogenerated')
+                        else:
+                            new_data[a_name] = _data
+                        i += 1
                 else:
-                    _data, _FL = data_type.autogenerate_data(data[a_name], a_path)
+                    _data, _FL = data_type.autogenerate_data(data[a_name], a_path, RTE)
                     new_data[a_name] = _data
+                    i += 1
                 FL += _FL
-        for a_name, a_data in data.items():
-            if a_name in processed_attributes:
-                continue
-            data_type = self._get_attribute_object(a_name, self.allow_regex_attributes)
-            if data_type is None:
-                new_data[a_name] = a_data
-                continue
-            a_path = path + self.path_symbol + a_name
-            _data, _FL = data_type.autogenerate_data(a_data, a_path)
-            new_data[a_name] = _data
-            FL += _FL
-        return new_data, FL
+            data = new_data
+        else:
+            for a_name, a_data in data.items():
+                data_type = self._get_attribute_object(a_name, self.allow_regex_attributes)
+                if data_type is None:
+                    continue
+                a_path = path + self.path_symbol + a_name
+                _data, _FL = data_type.autogenerate_data(a_data, a_path, RTE)
+                if _FL:
+                    data[a_name] = _data
+                    FL += _FL
+        return data, FL
     
     @staticmethod
     def _attribute_in_list(attribute :str, attributes :list, regex_allowed=False) -> bool:
         if regex_allowed:
             return  regex_matches_in_string_list(attribute, attributes)
         elif attribute in attributes:
             return attribute
@@ -128,28 +137,28 @@
     def _get_attribute_object(self, name :str, regex_allowed=False) -> bool:
         if regex_allowed:
             name = string_matches_regex_list(string=name,
                                                    regex_list=list(self.attributes_objects.keys()),
                                                    full_match=True)
         return self.attributes_objects.get(name, None)
 
-    def verify_data(self, data :any, path :str) -> FindingsList:
+    def verify_data(self, data :any, path :str, RTE :RunTimeEnv) -> FindingsList:
         FL = FindingsList()
         if self.attributes is None:
             return FL
         path = path + self.path_symbol
         for a_name, a_data in data.items():
             data_type = self._get_attribute_object(a_name, self.allow_regex_attributes)
             if data_type is None:
                 if self.ignore_undefined_attributes:
                     continue
                 FL.append(ValidationFinding(path=path, message="Invalid attribute '%s'" % a_name))
                 continue
             a_path = path + a_name
-            FL += data_type.validate_data(data=a_data, path=a_path)
+            FL += data_type.validate_data(data=a_data, path=a_path, RTE=RTE)
         for req_attr in self.required_attributes:
             found_in_data_keys = False
             if self.allow_regex_attributes:
                 if regex_matches_in_string_list(
                                                 regex=req_attr,
                                                 strings=list(data.keys()),
                                                 full_match=True):
```

### Comparing `cd2t-1.6.1/cd2t/types/schema.py` & `cd2t-1.6.2/cd2t/types/schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,21 +7,21 @@
     type = 'schema'
     path_symbol = '<>'
     options = [
         # option_name, required, class
         ('subschema', True, str, ''),
     ]
 
-    def __init__(self, RTE :RunTimeEnv) -> None:
-        super().__init__(RTE=RTE)
+    def __init__(self) -> None:
+        super().__init__()
         self.subschema = ''
         self.sub_root_schema = None
     
-    def build_schema(self, schema :dict, path :str, subschemas :dict, subpath :list):
-        self.__init__(RTE=self.RTE)
+    def build_schema(self, schema :dict, path :str, subschemas :dict, subpath :list, RTE :RunTimeEnv):
+        self.__init__()
         _path = path
         path = path + self.path_symbol
         self.load_schema_options(schema, path)
         _sub_schema = subschemas.get(self.subschema, None)
         if _sub_schema is None:
             raise SchemaError("Could not found subschema '%s'" % self.subschema, path)
         new_path = _path + '<' + self.subschema + '>'
@@ -33,16 +33,17 @@
         if isinstance(_sub_schema, Schema):
             # Subschema was already build.
             return _sub_schema.root_data_type
         sub_root_schema = _sub_schema.get('root', None)
         if sub_root_schema is None:
             raise SchemaError("Key missing", new_path + 'root')
         self.sub_root_schema = sub_root_schema
-        sub_data_obj = self._get_data_type('sub_root_schema', new_path + 'root')
+        sub_data_obj = self._get_data_type('sub_root_schema', new_path + 'root', RTE)
         sub_data_obj = sub_data_obj.build_schema(
                                 schema=self.sub_root_schema, path=new_path,
-                                subschemas=subschemas, subpath=new_subpath)
+                                subschemas=subschemas, subpath=new_subpath,
+                                RTE=RTE)
         sub_schema_obj = Schema()
         sub_schema_obj.set_root_data_type(sub_data_obj)
         subschemas[self.subschema] = sub_schema_obj
         return sub_data_obj
```

### Comparing `cd2t-1.6.1/cd2t/types/string.py` & `cd2t-1.6.2/cd2t/types/string.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
         ('allowed_values', False, list, None),
         ('not_allowed_values', False, list, list()),
         ('regex_mode', False, bool, False),
         ('regex_multiline', False, bool, False),
         ('regex_fullmatch', False, bool, True),
     ]
 
-    def __init__(self, RTE :RunTimeEnv) -> None:
-        super().__init__(RTE=RTE)
+    def __init__(self) -> None:
+        super().__init__()
         self.minimum = None
         self.maximum = None
         self.allowed_values = None
         self.not_allowed_values = list()
         self.regex_mode = False
         self.regex_multiline = False
         self.regex_fullmatch = True
@@ -58,15 +58,15 @@
             if OPT.CONSUMER not in self.ref_OPT:
                 raise SchemaError("Namespace lookup needs 'mode' == 'consumer'", path)
             if self.namespace_separator_char is None:
                 raise SchemaError("Namespace lookup requires 'namespace_separator_char' to be set", path)
             if not self.namespace_separator_char:
                 raise SchemaError("'namespace_separator_char' mustn't be '' (empty)", path)
         
-    def verify_data(self, data :any, path :str) -> FindingsList:
+    def verify_data(self, data :any, path :str, RTE :RunTimeEnv) -> FindingsList:
         FL = FindingsList()
         if self.minimum is not None and self.minimum > len(data):
             FL.append(WrongValueFinding(
                 path=path, message='String length is lower than minimum %d' % self.minimum))
         elif self.maximum is not None and self.maximum < len(data):
             FL.append(WrongValueFinding(
                 path=path, message='String length is greater than maximum %d' % self.maximum))
@@ -90,13 +90,13 @@
                     path=path, message="String is not allowed"))
         return FL
     
     def get_reference_element(self, path :str, ref_data :any) -> any:
         if OPT.CONSUMER in self.ref_OPT and self.allow_namespace_lookups:
             if self.namespace_separator_char in ref_data:
                 provider_ns, value = ref_data.split(self.namespace_separator_char, 1)
-                return ConsumerElement(reference=self.ref_key,
+                return ConsumerElement(reference_key=self.ref_key,
                                        path=path,
                                        value=value,
                                        options=self.ref_OPT,
                                        provider_namespace=provider_ns)
         return ReferenceElement(self.ref_key, path, ref_data, self.ref_OPT)
```

### Comparing `cd2t-1.6.1/LICENSE` & `cd2t-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cd2t-1.6.1/README.md` & `cd2t-1.6.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,18 @@
 - **Referencing**: Referencing can check the **uniqueness** of values at different positions in the data structure (i.e. lists of objects with ID attribute). It also can enforce a **consumer/producer modell**. In example, strings at some positions can be collected as *producers*. Strings at other positions must match one of those *produced* string. Scope of references can be limited to namespace.
 - **Value Autogeneration**: Some data types support creation of non-existing values. I.e. unique IDs can be added to the data structure.
 Uniqueness can be limited to namespaces.
 - **Multi Data Support**: Multiple data sources can be check with one schema or many schemas. You can switch schemas during iterating over data sources. Referencing or Autogeneration works across schemas and data sources - but can also be limited to current data.
 - **Schema Validation**: Typos, syntax mistakes or missing required options are reported as SchemaErrors (Exception) during schema loading. Reason and path through schema structured are provided.
 
 ## Change Log
+**Version 1.6.2**:
+- *Fix*: Reference false positives, if Validator object changes
+- *Fix*: Sorting of Validation or Autogeneration findings
+
 **Version 1.6.1**:
 - *Fix*: Data Type shortcut mode with classic dictionary schema
 
 **Version 1.6.0**:
 - *Changed*: Python 3.9 or higher required
 - *New*: Data Type Shortcuts - Specify data type with defaults as string only
 - *Add*: Validator API - Method to get reference findings
@@ -426,15 +430,16 @@
 # 'required_attributes': Each element must have a at least one matching attribute name.
 # 'dependencies.<>.requires': Successful if any object attribute name matches each list entry.
 # 'dependencies.<>.excludes': Error if any object attribute name matches any list entry.
 # !!! Disables autogeneration of missing keys !!!
 
 autogenerate: < bool | default -> True >
 # Enable/Disable autogeneration of missing attributes,
-# if attribute's data type supports autogeneration and is defined within.
+# if 'allow_regex_attributes' == false and
+# attribute's data type supports autogeneration and is defined within.
 
 reference: { reference options }
 # The validator checks, if the same combination of attribute values is specified at
 # another data type with the same reference.key.
 # Requires 'reference_attributes' to be defined.
     
 reference_attributes:
```

### Comparing `cd2t-1.6.1/pyproject.toml` & `cd2t-1.6.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.hatch.build]
 include = [
   "/cd2t",
 ]
 
 [project]
 name = "cd2t"
-version = "1.6.1"
+version = "1.6.2"
 authors = [
   { name="Korte Noack", email="korte@8lacht.de" },
 ]
 description = "cd2t validates data structure, data types and values with templates"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `cd2t-1.6.1/PKG-INFO` & `cd2t-1.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cd2t
-Version: 1.6.1
+Version: 1.6.2
 Summary: cd2t validates data structure, data types and values with templates
 Project-URL: Homepage, https://gitlab.com/ko.no/cd2t
 Project-URL: Bug Tracker, https://gitlab.com/ko.no/cd2t/-/issues
 Author-email: Korte Noack <korte@8lacht.de>
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -33,14 +33,18 @@
 - **Referencing**: Referencing can check the **uniqueness** of values at different positions in the data structure (i.e. lists of objects with ID attribute). It also can enforce a **consumer/producer modell**. In example, strings at some positions can be collected as *producers*. Strings at other positions must match one of those *produced* string. Scope of references can be limited to namespace.
 - **Value Autogeneration**: Some data types support creation of non-existing values. I.e. unique IDs can be added to the data structure.
 Uniqueness can be limited to namespaces.
 - **Multi Data Support**: Multiple data sources can be check with one schema or many schemas. You can switch schemas during iterating over data sources. Referencing or Autogeneration works across schemas and data sources - but can also be limited to current data.
 - **Schema Validation**: Typos, syntax mistakes or missing required options are reported as SchemaErrors (Exception) during schema loading. Reason and path through schema structured are provided.
 
 ## Change Log
+**Version 1.6.2**:
+- *Fix*: Reference false positives, if Validator object changes
+- *Fix*: Sorting of Validation or Autogeneration findings
+
 **Version 1.6.1**:
 - *Fix*: Data Type shortcut mode with classic dictionary schema
 
 **Version 1.6.0**:
 - *Changed*: Python 3.9 or higher required
 - *New*: Data Type Shortcuts - Specify data type with defaults as string only
 - *Add*: Validator API - Method to get reference findings
@@ -442,15 +446,16 @@
 # 'required_attributes': Each element must have a at least one matching attribute name.
 # 'dependencies.<>.requires': Successful if any object attribute name matches each list entry.
 # 'dependencies.<>.excludes': Error if any object attribute name matches any list entry.
 # !!! Disables autogeneration of missing keys !!!
 
 autogenerate: < bool | default -> True >
 # Enable/Disable autogeneration of missing attributes,
-# if attribute's data type supports autogeneration and is defined within.
+# if 'allow_regex_attributes' == false and
+# attribute's data type supports autogeneration and is defined within.
 
 reference: { reference options }
 # The validator checks, if the same combination of attribute values is specified at
 # another data type with the same reference.key.
 # Requires 'reference_attributes' to be defined.
     
 reference_attributes:
```


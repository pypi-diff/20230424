# Comparing `tmp/semantic-field-definition-generator-1.2.0.tar.gz` & `tmp/semantic-field-definition-generator-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic-field-definition-generator-1.2.0.tar", last modified: Thu Mar  2 18:41:19 2023, max compression
+gzip compressed data, was "semantic-field-definition-generator-1.2.1.tar", last modified: Mon Apr 24 15:45:36 2023, max compression
```

## Comparing `semantic-field-definition-generator-1.2.0.tar` & `semantic-field-definition-generator-1.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 casties    (501) staff       (20)        0 2023-03-02 18:41:19.627274 semantic-field-definition-generator-1.2.0/
--rw-r--r--   0 casties    (501) staff       (20)     1073 2023-02-20 08:35:34.000000 semantic-field-definition-generator-1.2.0/LICENSE
--rw-r--r--   0 casties    (501) staff       (20)     7131 2023-03-02 18:41:19.627139 semantic-field-definition-generator-1.2.0/PKG-INFO
--rw-r--r--   0 casties    (501) staff       (20)     5328 2023-03-02 18:35:59.000000 semantic-field-definition-generator-1.2.0/README.md
--rw-r--r--   0 casties    (501) staff       (20)     1024 2023-03-02 18:36:53.000000 semantic-field-definition-generator-1.2.0/pyproject.toml
--rw-r--r--   0 casties    (501) staff       (20)       38 2023-03-02 18:41:19.627309 semantic-field-definition-generator-1.2.0/setup.cfg
-drwxr-xr-x   0 casties    (501) staff       (20)        0 2023-03-02 18:41:19.623583 semantic-field-definition-generator-1.2.0/src/
-drwxr-xr-x   0 casties    (501) staff       (20)        0 2023-03-02 18:41:19.624798 semantic-field-definition-generator-1.2.0/src/SemanticFieldDefinitionGenerator/
--rw-r--r--   0 casties    (501) staff       (20)        0 2023-02-25 16:29:53.000000 semantic-field-definition-generator-1.2.0/src/SemanticFieldDefinitionGenerator/__init__.py
--rw-r--r--   0 casties    (501) staff       (20)     3050 2023-03-02 18:37:44.000000 semantic-field-definition-generator-1.2.0/src/SemanticFieldDefinitionGenerator/generator.py
--rw-r--r--   0 casties    (501) staff       (20)    10296 2023-03-02 18:38:24.000000 semantic-field-definition-generator-1.2.0/src/SemanticFieldDefinitionGenerator/parser.py
--rwxr-xr-x   0 casties    (501) staff       (20)     5185 2023-03-02 18:36:44.000000 semantic-field-definition-generator-1.2.0/src/SemanticFieldDefinitionGenerator/semantic_field_util.py
-drwxr-xr-x   0 casties    (501) staff       (20)        0 2023-03-02 18:41:19.626065 semantic-field-definition-generator-1.2.0/src/SemanticFieldDefinitionGenerator/templates/
--rw-r--r--   0 casties    (501) staff       (20)     2799 2023-03-02 18:26:32.000000 semantic-field-definition-generator-1.2.0/src/SemanticFieldDefinitionGenerator/templates/inline.handlebars
--rw-r--r--   0 casties    (501) staff       (20)     2853 2023-03-02 18:26:16.000000 semantic-field-definition-generator-1.2.0/src/SemanticFieldDefinitionGenerator/templates/json.handlebars
--rw-r--r--   0 casties    (501) staff       (20)     5114 2023-03-02 18:25:13.000000 semantic-field-definition-generator-1.2.0/src/SemanticFieldDefinitionGenerator/templates/metaphacts.handlebars
--rw-r--r--   0 casties    (501) staff       (20)     3963 2023-03-02 18:24:55.000000 semantic-field-definition-generator-1.2.0/src/SemanticFieldDefinitionGenerator/templates/researchspace.handlebars
--rw-r--r--   0 casties    (501) staff       (20)     5384 2023-03-02 18:25:37.000000 semantic-field-definition-generator-1.2.0/src/SemanticFieldDefinitionGenerator/templates/universal.handlebars
-drwxr-xr-x   0 casties    (501) staff       (20)        0 2023-03-02 18:41:19.626950 semantic-field-definition-generator-1.2.0/src/semantic_field_definition_generator.egg-info/
--rw-r--r--   0 casties    (501) staff       (20)     7131 2023-03-02 18:41:19.000000 semantic-field-definition-generator-1.2.0/src/semantic_field_definition_generator.egg-info/PKG-INFO
--rw-r--r--   0 casties    (501) staff       (20)      955 2023-03-02 18:41:19.000000 semantic-field-definition-generator-1.2.0/src/semantic_field_definition_generator.egg-info/SOURCES.txt
--rw-r--r--   0 casties    (501) staff       (20)        1 2023-03-02 18:41:19.000000 semantic-field-definition-generator-1.2.0/src/semantic_field_definition_generator.egg-info/dependency_links.txt
--rw-r--r--   0 casties    (501) staff       (20)       98 2023-03-02 18:41:19.000000 semantic-field-definition-generator-1.2.0/src/semantic_field_definition_generator.egg-info/entry_points.txt
--rw-r--r--   0 casties    (501) staff       (20)       22 2023-03-02 18:41:19.000000 semantic-field-definition-generator-1.2.0/src/semantic_field_definition_generator.egg-info/requires.txt
--rw-r--r--   0 casties    (501) staff       (20)       33 2023-03-02 18:41:19.000000 semantic-field-definition-generator-1.2.0/src/semantic_field_definition_generator.egg-info/top_level.txt
+drwxr-xr-x   0 casties    (501) staff       (20)        0 2023-04-24 15:45:36.696265 semantic-field-definition-generator-1.2.1/
+-rw-r--r--   0 casties    (501) staff       (20)     1073 2023-02-20 08:35:34.000000 semantic-field-definition-generator-1.2.1/LICENSE
+-rw-r--r--   0 casties    (501) staff       (20)     7381 2023-04-24 15:45:36.696128 semantic-field-definition-generator-1.2.1/PKG-INFO
+-rw-r--r--   0 casties    (501) staff       (20)     5578 2023-03-04 15:21:10.000000 semantic-field-definition-generator-1.2.1/README.md
+-rw-r--r--   0 casties    (501) staff       (20)     1024 2023-04-24 15:43:35.000000 semantic-field-definition-generator-1.2.1/pyproject.toml
+-rw-r--r--   0 casties    (501) staff       (20)       38 2023-04-24 15:45:36.696301 semantic-field-definition-generator-1.2.1/setup.cfg
+drwxr-xr-x   0 casties    (501) staff       (20)        0 2023-04-24 15:45:36.692381 semantic-field-definition-generator-1.2.1/src/
+drwxr-xr-x   0 casties    (501) staff       (20)        0 2023-04-24 15:45:36.693575 semantic-field-definition-generator-1.2.1/src/SemanticFieldDefinitionGenerator/
+-rw-r--r--   0 casties    (501) staff       (20)        0 2023-02-25 16:29:53.000000 semantic-field-definition-generator-1.2.1/src/SemanticFieldDefinitionGenerator/__init__.py
+-rw-r--r--   0 casties    (501) staff       (20)     3050 2023-03-02 18:37:44.000000 semantic-field-definition-generator-1.2.1/src/SemanticFieldDefinitionGenerator/generator.py
+-rw-r--r--   0 casties    (501) staff       (20)    10346 2023-03-03 10:06:35.000000 semantic-field-definition-generator-1.2.1/src/SemanticFieldDefinitionGenerator/parser.py
+-rwxr-xr-x   0 casties    (501) staff       (20)     5185 2023-04-24 15:28:47.000000 semantic-field-definition-generator-1.2.1/src/SemanticFieldDefinitionGenerator/semantic_field_util.py
+drwxr-xr-x   0 casties    (501) staff       (20)        0 2023-04-24 15:45:36.694911 semantic-field-definition-generator-1.2.1/src/SemanticFieldDefinitionGenerator/templates/
+-rw-r--r--   0 casties    (501) staff       (20)     2799 2023-03-02 18:26:32.000000 semantic-field-definition-generator-1.2.1/src/SemanticFieldDefinitionGenerator/templates/inline.handlebars
+-rw-r--r--   0 casties    (501) staff       (20)     2853 2023-03-02 18:26:16.000000 semantic-field-definition-generator-1.2.1/src/SemanticFieldDefinitionGenerator/templates/json.handlebars
+-rw-r--r--   0 casties    (501) staff       (20)     5200 2023-04-24 15:39:53.000000 semantic-field-definition-generator-1.2.1/src/SemanticFieldDefinitionGenerator/templates/metaphacts.handlebars
+-rw-r--r--   0 casties    (501) staff       (20)     4049 2023-04-24 15:39:40.000000 semantic-field-definition-generator-1.2.1/src/SemanticFieldDefinitionGenerator/templates/researchspace.handlebars
+-rw-r--r--   0 casties    (501) staff       (20)     5470 2023-04-24 15:39:59.000000 semantic-field-definition-generator-1.2.1/src/SemanticFieldDefinitionGenerator/templates/universal.handlebars
+drwxr-xr-x   0 casties    (501) staff       (20)        0 2023-04-24 15:45:36.695913 semantic-field-definition-generator-1.2.1/src/semantic_field_definition_generator.egg-info/
+-rw-r--r--   0 casties    (501) staff       (20)     7381 2023-04-24 15:45:36.000000 semantic-field-definition-generator-1.2.1/src/semantic_field_definition_generator.egg-info/PKG-INFO
+-rw-r--r--   0 casties    (501) staff       (20)      955 2023-04-24 15:45:36.000000 semantic-field-definition-generator-1.2.1/src/semantic_field_definition_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 casties    (501) staff       (20)        1 2023-04-24 15:45:36.000000 semantic-field-definition-generator-1.2.1/src/semantic_field_definition_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 casties    (501) staff       (20)       98 2023-04-24 15:45:36.000000 semantic-field-definition-generator-1.2.1/src/semantic_field_definition_generator.egg-info/entry_points.txt
+-rw-r--r--   0 casties    (501) staff       (20)       22 2023-04-24 15:45:36.000000 semantic-field-definition-generator-1.2.1/src/semantic_field_definition_generator.egg-info/requires.txt
+-rw-r--r--   0 casties    (501) staff       (20)       33 2023-04-24 15:45:36.000000 semantic-field-definition-generator-1.2.1/src/semantic_field_definition_generator.egg-info/top_level.txt
```

### Comparing `semantic-field-definition-generator-1.2.0/LICENSE` & `semantic-field-definition-generator-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `semantic-field-definition-generator-1.2.0/PKG-INFO` & `semantic-field-definition-generator-1.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-field-definition-generator
-Version: 1.2.0
+Version: 1.2.1
 Summary: A generator for Field Definitions for ResearchSpace and Metaphacts
 Author-email: Robert Casties <casties@mpiwg-berlin.mpg.de>, Florian Kräutli <florian.kraeutli@uzh.ch>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -28,15 +28,21 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Semantic Field Definition Generator
 
-A generator for Metaphacts/ResearchSpace semantic field definitions. Based on https://github.com/swiss-art-research-net/sari-field-definitions-generator
+A generator for [Metaphacts](https://metaphacts.com/) / [ResearchSpace](https://researchspace.org/) semantic field definitions. 
+
+For background information see:
+- ResearchSpace: https://documentation.researchspace.org/resource/Help:SemanticForm
+- Metaphacts: https://help.metaphacts.com/resource/Help:SemanticForm
+
+Based on https://github.com/swiss-art-research-net/sari-field-definitions-generator
 
 ## Installation
 
 install using pip
 
 ```sh
 pip install semantic-field-definition-generator
@@ -121,15 +127,15 @@
 ```
 
 This will read the YAML file `fieldDefinitions.yml` and create ResearchSpace-flavor (`-f RS`) field definitions in the TriG file `../ldp/assets/fieldDefinitions.trig`.
 
 You can also use the generator library in your Python program
 
 ```python
-from sariFieldDefinitionsGenerator import generator
+from SemanticFieldDefinitionGenerator import generator
 
 inputFile = './fieldDefinitions.yml'
 outputFile = '../ldp/assets/fieldDefinitions.trig'
 
 model = generator.loadSourceFromFile(inputFile)
 
 output = generator.generate(model, generator.METAPHACTS)
```

### Comparing `semantic-field-definition-generator-1.2.0/README.md` & `semantic-field-definition-generator-1.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 # Semantic Field Definition Generator
 
-A generator for Metaphacts/ResearchSpace semantic field definitions. Based on https://github.com/swiss-art-research-net/sari-field-definitions-generator
+A generator for [Metaphacts](https://metaphacts.com/) / [ResearchSpace](https://researchspace.org/) semantic field definitions. 
+
+For background information see:
+- ResearchSpace: https://documentation.researchspace.org/resource/Help:SemanticForm
+- Metaphacts: https://help.metaphacts.com/resource/Help:SemanticForm
+
+Based on https://github.com/swiss-art-research-net/sari-field-definitions-generator
 
 ## Installation
 
 install using pip
 
 ```sh
 pip install semantic-field-definition-generator
@@ -89,15 +95,15 @@
 ```
 
 This will read the YAML file `fieldDefinitions.yml` and create ResearchSpace-flavor (`-f RS`) field definitions in the TriG file `../ldp/assets/fieldDefinitions.trig`.
 
 You can also use the generator library in your Python program
 
 ```python
-from sariFieldDefinitionsGenerator import generator
+from SemanticFieldDefinitionGenerator import generator
 
 inputFile = './fieldDefinitions.yml'
 outputFile = '../ldp/assets/fieldDefinitions.trig'
 
 model = generator.loadSourceFromFile(inputFile)
 
 output = generator.generate(model, generator.METAPHACTS)
```

### Comparing `semantic-field-definition-generator-1.2.0/pyproject.toml` & `semantic-field-definition-generator-1.2.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "semantic-field-definition-generator"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
   { name="Robert Casties", email="casties@mpiwg-berlin.mpg.de" },
   { name="Florian Kräutli", email="florian.kraeutli@uzh.ch" },
 ]
 description = "A generator for Field Definitions for ResearchSpace and Metaphacts"
 readme = "README.md"
 license = {file = "LICENSE"}
```

### Comparing `semantic-field-definition-generator-1.2.0/src/SemanticFieldDefinitionGenerator/generator.py` & `semantic-field-definition-generator-1.2.1/src/SemanticFieldDefinitionGenerator/generator.py`

 * *Files identical despite different names*

### Comparing `semantic-field-definition-generator-1.2.0/src/SemanticFieldDefinitionGenerator/parser.py` & `semantic-field-definition-generator-1.2.1/src/SemanticFieldDefinitionGenerator/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,22 +31,52 @@
 # separate NamespaceManager for normalizations
 # rdflib BUG: queries may break when you use the store's manager :-(
 nsManager = NamespaceManager(Dataset())
 for pref, ns in nsPrefixes.items():
     nsManager.bind(pref, ns)
 
 
-def uristr(node):
+def _uristr(node):
     """return string form of node, normalizing URIs.""" 
     if isinstance(node, URIRef):
         # normalize to N3 form including namespaces
         return node.n3(nsManager)
         
     return str(node)
 
+def _set_once(items, key, value):
+    """set items[key] to value if it doesn't exist, warn if value is different."""
+    if key in items:
+        if items[key] != value:
+            logging.warning(f"Ignoring different value to set! key={key} value={value}")
+        
+    else:
+        items[key] = value
+        
+    return items
+
+def _set_append(items, key, value):
+    """set items[key] to value if it doesn't exist, append to list if value is different."""
+    if key in items:
+        oldval = items[key]
+        if oldval != value:
+            # existing value is different
+            if isinstance(oldval, list):
+                # append to existing list
+                oldval.append(value)
+            else:
+                # create new list
+                items[key] = [oldval, value]
+        
+    else:
+        items[key] = value
+        
+    return items
+
+
 def open_sparql_store(endpoint, repository='assets', auth_user='admin', auth_pass='admin'):
     """open connection to SPARQL store.
     endpoint: SPARQL endpoint URI
     repository: RS/MP repository parameter
     auth: (username, password) tuple
     returns rdflib Dataset.
     """
@@ -64,15 +94,15 @@
         
     _store = SPARQLStore(query_endpoint=endpoint, params=params, auth=auth)
     # instantiate Dataset
     store = Dataset(_store)
     return store
 
 def read_trig_store(pathname):
-    """create store from trig file(s).
+    """create store by loading trig file(s) from pathname.
     """
     logging.info(f"creating trig file store from {pathname}")
     store = Dataset()
     p = Path(pathname)
     if p.is_dir():
         for f in p.glob('*.trig'):
             logging.debug(f"reading trig file {f}")
@@ -99,60 +129,33 @@
 
     query = '''select ?graph ?field
     where {
         graph ?graph {
             fieldcon:fieldDefinitionContainer ldp:contains ?field .
             ?field a fielddef:Field .
         }
-    }'''
+    }
+    ORDER BY ?field'''
     logging.debug(f"fields query='{query}'")
     res = store.query(query, initNs=prefixes)
+    
     logging.info(f"found {len(res)} fields (flavor={flavor})")
     for r in res:
         logging.debug(f"field uri={r.field} in graph={r.graph}")
         field_id = str(r.field)
         if field_id_prefix and field_id.startswith(field_id_prefix):
             field_id = field_id[len(field_id_prefix):]
             
         field = read_field(store, r.field, r.graph, field_id, prefixes)
         if field is not None:
             fields.append(field)
 
         #break # debug
     return fields
 
-def _set_once(items, key, value):
-    """set items[key] to value if it doesn't exist, warn if value is different."""
-    if key in items:
-        if items[key] != value:
-            logging.warning(f"Ignoring different value to set! key={key} value={value}")
-        
-    else:
-        items[key] = value
-        
-    return items
-
-def _set_append(items, key, value):
-    """set items[key] to value if it doesn't exist, append to list if value is different."""
-    if key in items:
-        oldval = items[key]
-        if oldval != value:
-            # existing value is different
-            if isinstance(oldval, list):
-                # append to existing list
-                oldval.append(value)
-            else:
-                # create new list
-                items[key] = [oldval, value]
-        
-    else:
-        items[key] = value
-        
-    return items
-
 def read_field(store, field_uri, graph_uri, field_id, prefixes):
     """read the semantic field with URI field_uri in named graph graph_uri from store.
     returns dict of field attributes.
     
     field attributes (see https://documentation.researchspace.org/resource/Help:SemanticForm)
     - id*: Unique identifier of the field definition, in most cases it will be the URI of the field definition
     - label*: A human readable label for the field. Will be used as default label for the input elements within the form.
@@ -218,19 +221,19 @@
     }
     # loop through possibly multiple attribute values
     for f in res:
         _set_once(field, 'label', str(f.label))
         if f.description:
             _set_once(field, 'description', str(f.description))
         if f.domain:
-            _set_append(field, 'domain', uristr(f.domain))
+            _set_append(field, 'domain', _uristr(f.domain))
         if f.range:
-            _set_append(field, 'range', uristr(f.range))
+            _set_append(field, 'range', _uristr(f.range))
         if f.datatype:
-            _set_once(field, 'datatype', uristr(f.datatype))
+            _set_once(field, 'datatype', _uristr(f.datatype))
         if f.minOccurs:
             _set_once(field, 'minOccurs', str(f.minOccurs))
         if f.maxOccurs:
             _set_once(field, 'maxOccurs', str(f.maxOccurs))
         if f.order:
             _set_once(field, 'order', str(f.order))
         if f.defaultValue:
```

### Comparing `semantic-field-definition-generator-1.2.0/src/SemanticFieldDefinitionGenerator/semantic_field_util.py` & `semantic-field-definition-generator-1.2.1/src/SemanticFieldDefinitionGenerator/semantic_field_util.py`

 * *Files identical despite different names*

### Comparing `semantic-field-definition-generator-1.2.0/src/SemanticFieldDefinitionGenerator/templates/inline.handlebars` & `semantic-field-definition-generator-1.2.1/src/SemanticFieldDefinitionGenerator/templates/inline.handlebars`

 * *Files identical despite different names*

### Comparing `semantic-field-definition-generator-1.2.0/src/SemanticFieldDefinitionGenerator/templates/json.handlebars` & `semantic-field-definition-generator-1.2.1/src/SemanticFieldDefinitionGenerator/templates/json.handlebars`

 * *Files identical despite different names*

### Comparing `semantic-field-definition-generator-1.2.0/src/SemanticFieldDefinitionGenerator/templates/metaphacts.handlebars` & `semantic-field-definition-generator-1.2.1/src/SemanticFieldDefinitionGenerator/templates/metaphacts.handlebars`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 @prefix ldp: <http://www.w3.org/ns/ldp#> .
 @prefix mpfield: <http://www.metaphacts.com/ontology/fields#> .
 @prefix prov: <http://www.w3.org/ns/prov#> .
 @prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 @prefix sp: <http://spinrdf.org/sp#> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
 @prefix mpuser: <http://www.metaphacts.com/resource/user/> .
+{{#each fields}}
+    {{#if extraNs }}
+@prefix {{{ extraNs }}} .
+    {{/if}}
+{{/each}}
 
 <http://www.metaphacts.com/ontologies/platform#fieldDefinitionContainer/context> {
   <http://www.metaphacts.com/ontologies/platform#fieldDefinitionContainer> rdfs:comment "Container to store field definitions.";
     a ldp:Container, ldp:Resource, prov:Entity ;
     rdfs:label "Form Container";
     prov:wasAttributedTo mpuser:admin;
     prov:generatedAtTime "2020-04-06T13:49:19.238+03:00"^^xsd:dateTime .
```

### Comparing `semantic-field-definition-generator-1.2.0/src/SemanticFieldDefinitionGenerator/templates/researchspace.handlebars` & `semantic-field-definition-generator-1.2.1/src/SemanticFieldDefinitionGenerator/templates/researchspace.handlebars`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 @prefix ldp: <http://www.w3.org/ns/ldp#> .
 @prefix rsfield: <http://www.researchspace.org/resource/system/fields/> .
 @prefix prov: <http://www.w3.org/ns/prov#> .
 @prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 @prefix sp: <http://spinrdf.org/sp#> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
 @prefix rsuser: <http://www.researchspace.org/resource/user/> .
+{{#each fields}}
+    {{#if extraNs }}
+@prefix {{{ extraNs }}} .
+    {{/if}}
+{{/each}}
 
 <http://www.researchspace.org/resource/system/fieldDefinitionContainer/context> {
   <http://www.researchspace.org/resource/system/fieldDefinitionContainer> rdfs:comment "Container to store field definitions.";
     a ldp:Container, ldp:Resource, prov:Entity ;
     rdfs:label "Form Container";
     prov:wasAttributedTo rsuser:admin ;
     prov:generatedAtTime "2020-04-06T13:49:19.238+03:00"^^xsd:dateTime .
```

### Comparing `semantic-field-definition-generator-1.2.0/src/SemanticFieldDefinitionGenerator/templates/universal.handlebars` & `semantic-field-definition-generator-1.2.1/src/SemanticFieldDefinitionGenerator/templates/universal.handlebars`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 @prefix mpfield: <http://www.metaphacts.com/ontology/fields#> .
 @prefix prov: <http://www.w3.org/ns/prov#> .
 @prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 @prefix sp: <http://spinrdf.org/sp#> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
 @prefix rsuser: <http://www.researchspace.org/resource/user/> .
 @prefix mpuser: <http://www.metaphacts.com/resource/user/> .
+{{#each fields}}
+    {{#if extraNs }}
+@prefix {{{ extraNs }}} .
+    {{/if}}
+{{/each}}
 
 <http://www.researchspace.org/resource/system/fieldDefinitionContainer/context> {
   <http://www.researchspace.org/resource/system/fieldDefinitionContainer> rdfs:comment "Container to store field definitions.";
     a ldp:Container, ldp:Resource, prov:Entity ;
     rdfs:label "Form Container";
     prov:wasAttributedTo rsuser:admin ;
     prov:generatedAtTime "2020-04-06T13:49:19.238+03:00"^^xsd:dateTime .
```

### Comparing `semantic-field-definition-generator-1.2.0/src/semantic_field_definition_generator.egg-info/PKG-INFO` & `semantic-field-definition-generator-1.2.1/src/semantic_field_definition_generator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-field-definition-generator
-Version: 1.2.0
+Version: 1.2.1
 Summary: A generator for Field Definitions for ResearchSpace and Metaphacts
 Author-email: Robert Casties <casties@mpiwg-berlin.mpg.de>, Florian Kräutli <florian.kraeutli@uzh.ch>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -28,15 +28,21 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Semantic Field Definition Generator
 
-A generator for Metaphacts/ResearchSpace semantic field definitions. Based on https://github.com/swiss-art-research-net/sari-field-definitions-generator
+A generator for [Metaphacts](https://metaphacts.com/) / [ResearchSpace](https://researchspace.org/) semantic field definitions. 
+
+For background information see:
+- ResearchSpace: https://documentation.researchspace.org/resource/Help:SemanticForm
+- Metaphacts: https://help.metaphacts.com/resource/Help:SemanticForm
+
+Based on https://github.com/swiss-art-research-net/sari-field-definitions-generator
 
 ## Installation
 
 install using pip
 
 ```sh
 pip install semantic-field-definition-generator
@@ -121,15 +127,15 @@
 ```
 
 This will read the YAML file `fieldDefinitions.yml` and create ResearchSpace-flavor (`-f RS`) field definitions in the TriG file `../ldp/assets/fieldDefinitions.trig`.
 
 You can also use the generator library in your Python program
 
 ```python
-from sariFieldDefinitionsGenerator import generator
+from SemanticFieldDefinitionGenerator import generator
 
 inputFile = './fieldDefinitions.yml'
 outputFile = '../ldp/assets/fieldDefinitions.trig'
 
 model = generator.loadSourceFromFile(inputFile)
 
 output = generator.generate(model, generator.METAPHACTS)
```

### Comparing `semantic-field-definition-generator-1.2.0/src/semantic_field_definition_generator.egg-info/SOURCES.txt` & `semantic-field-definition-generator-1.2.1/src/semantic_field_definition_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*


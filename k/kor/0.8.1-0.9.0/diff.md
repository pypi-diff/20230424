# Comparing `tmp/kor-0.8.1.tar.gz` & `tmp/kor-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kor-0.8.1.tar", max compression
+gzip compressed data, was "kor-0.9.0.tar", max compression
```

## Comparing `kor-0.8.1.tar` & `kor-0.9.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1071 2023-04-20 02:25:23.756379 kor-0.8.1/LICENSE
--rw-r--r--   0        0        0     4273 2023-04-20 02:25:23.756379 kor-0.8.1/README.md
--rw-r--r--   0        0        0      783 2023-04-20 02:25:23.756379 kor-0.8.1/kor/__init__.py
--rw-r--r--   0        0        0     5123 2023-04-20 02:25:23.756379 kor-0.8.1/kor/adapters.py
--rw-r--r--   0        0        0        0 2023-04-20 02:25:23.756379 kor-0.8.1/kor/documents/__init__.py
--rw-r--r--   0        0        0     2191 2023-04-20 02:25:23.760379 kor-0.8.1/kor/documents/html.py
--rw-r--r--   0        0        0      292 2023-04-20 02:25:23.760379 kor-0.8.1/kor/documents/typedefs.py
--rw-r--r--   0        0        0      578 2023-04-20 02:25:23.760379 kor-0.8.1/kor/encoders/__init__.py
--rw-r--r--   0        0        0     4744 2023-04-20 02:25:23.760379 kor-0.8.1/kor/encoders/csv_data.py
--rw-r--r--   0        0        0     3513 2023-04-20 02:25:23.760379 kor-0.8.1/kor/encoders/encode.py
--rw-r--r--   0        0        0     2815 2023-04-20 02:25:23.760379 kor-0.8.1/kor/encoders/json_data.py
--rw-r--r--   0        0        0     1515 2023-04-20 02:25:23.760379 kor-0.8.1/kor/encoders/typedefs.py
--rw-r--r--   0        0        0      514 2023-04-20 02:25:23.760379 kor-0.8.1/kor/encoders/utils.py
--rw-r--r--   0        0        0     6093 2023-04-20 02:25:23.760379 kor-0.8.1/kor/encoders/xml.py
--rw-r--r--   0        0        0     4103 2023-04-20 02:25:23.760379 kor-0.8.1/kor/examples.py
--rw-r--r--   0        0        0      225 2023-04-20 02:25:23.760379 kor-0.8.1/kor/exceptions.py
--rw-r--r--   0        0        0      327 2023-04-20 02:25:23.760379 kor-0.8.1/kor/extraction/__init__.py
--rw-r--r--   0        0        0     6678 2023-04-20 02:25:23.760379 kor-0.8.1/kor/extraction/api.py
--rw-r--r--   0        0        0     2192 2023-04-20 02:25:23.760379 kor-0.8.1/kor/extraction/parser.py
--rw-r--r--   0        0        0     1022 2023-04-20 02:25:23.760379 kor-0.8.1/kor/extraction/typedefs.py
--rw-r--r--   0        0        0     6884 2023-04-20 02:25:23.760379 kor-0.8.1/kor/nodes.py
--rw-r--r--   0        0        0     5758 2023-04-20 02:25:23.760379 kor-0.8.1/kor/prompts.py
--rw-r--r--   0        0        0        0 2023-04-20 02:25:23.760379 kor-0.8.1/kor/py.typed
--rw-r--r--   0        0        0     4493 2023-04-20 02:25:23.760379 kor-0.8.1/kor/type_descriptors.py
--rw-r--r--   0        0        0     2055 2023-04-20 02:25:23.760379 kor-0.8.1/kor/validators.py
--rw-r--r--   0        0        0      181 2023-04-20 02:25:23.760379 kor-0.8.1/kor/version.py
--rw-r--r--   0        0        0     2072 2023-04-20 02:25:23.760379 kor-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     5283 1970-01-01 00:00:00.000000 kor-0.8.1/setup.py
--rw-r--r--   0        0        0     5069 1970-01-01 00:00:00.000000 kor-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-24 14:32:41.085269 kor-0.9.0/LICENSE
+-rw-r--r--   0        0        0     4273 2023-04-24 14:32:41.085269 kor-0.9.0/README.md
+-rw-r--r--   0        0        0      783 2023-04-24 14:32:41.089269 kor-0.9.0/kor/__init__.py
+-rw-r--r--   0        0        0     5123 2023-04-24 14:32:41.089269 kor-0.9.0/kor/adapters.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:32:41.089269 kor-0.9.0/kor/documents/__init__.py
+-rw-r--r--   0        0        0     2191 2023-04-24 14:32:41.089269 kor-0.9.0/kor/documents/html.py
+-rw-r--r--   0        0        0      292 2023-04-24 14:32:41.089269 kor-0.9.0/kor/documents/typedefs.py
+-rw-r--r--   0        0        0      578 2023-04-24 14:32:41.089269 kor-0.9.0/kor/encoders/__init__.py
+-rw-r--r--   0        0        0     4744 2023-04-24 14:32:41.089269 kor-0.9.0/kor/encoders/csv_data.py
+-rw-r--r--   0        0        0     3513 2023-04-24 14:32:41.089269 kor-0.9.0/kor/encoders/encode.py
+-rw-r--r--   0        0        0     2815 2023-04-24 14:32:41.089269 kor-0.9.0/kor/encoders/json_data.py
+-rw-r--r--   0        0        0     1515 2023-04-24 14:32:41.089269 kor-0.9.0/kor/encoders/typedefs.py
+-rw-r--r--   0        0        0      514 2023-04-24 14:32:41.089269 kor-0.9.0/kor/encoders/utils.py
+-rw-r--r--   0        0        0     6093 2023-04-24 14:32:41.089269 kor-0.9.0/kor/encoders/xml.py
+-rw-r--r--   0        0        0     4103 2023-04-24 14:32:41.089269 kor-0.9.0/kor/examples.py
+-rw-r--r--   0        0        0      225 2023-04-24 14:32:41.089269 kor-0.9.0/kor/exceptions.py
+-rw-r--r--   0        0        0      327 2023-04-24 14:32:41.089269 kor-0.9.0/kor/extraction/__init__.py
+-rw-r--r--   0        0        0     6957 2023-04-24 14:32:41.089269 kor-0.9.0/kor/extraction/api.py
+-rw-r--r--   0        0        0     2192 2023-04-24 14:32:41.089269 kor-0.9.0/kor/extraction/parser.py
+-rw-r--r--   0        0        0     1022 2023-04-24 14:32:41.089269 kor-0.9.0/kor/extraction/typedefs.py
+-rw-r--r--   0        0        0     6884 2023-04-24 14:32:41.089269 kor-0.9.0/kor/nodes.py
+-rw-r--r--   0        0        0     5758 2023-04-24 14:32:41.089269 kor-0.9.0/kor/prompts.py
+-rw-r--r--   0        0        0        0 2023-04-24 14:32:41.089269 kor-0.9.0/kor/py.typed
+-rw-r--r--   0        0        0     4493 2023-04-24 14:32:41.089269 kor-0.9.0/kor/type_descriptors.py
+-rw-r--r--   0        0        0     2055 2023-04-24 14:32:41.089269 kor-0.9.0/kor/validators.py
+-rw-r--r--   0        0        0      181 2023-04-24 14:32:41.089269 kor-0.9.0/kor/version.py
+-rw-r--r--   0        0        0     2072 2023-04-24 14:32:41.089269 kor-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     5283 1970-01-01 00:00:00.000000 kor-0.9.0/setup.py
+-rw-r--r--   0        0        0     5069 1970-01-01 00:00:00.000000 kor-0.9.0/PKG-INFO
```

### Comparing `kor-0.8.1/LICENSE` & `kor-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kor-0.8.1/README.md` & `kor-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `kor-0.8.1/kor/__init__.py` & `kor-0.9.0/kor/__init__.py`

 * *Files identical despite different names*

### Comparing `kor-0.8.1/kor/adapters.py` & `kor-0.9.0/kor/adapters.py`

 * *Files identical despite different names*

### Comparing `kor-0.8.1/kor/documents/html.py` & `kor-0.9.0/kor/documents/html.py`

 * *Files identical despite different names*

### Comparing `kor-0.8.1/kor/encoders/__init__.py` & `kor-0.9.0/kor/encoders/__init__.py`

 * *Files identical despite different names*

### Comparing `kor-0.8.1/kor/encoders/csv_data.py` & `kor-0.9.0/kor/encoders/csv_data.py`

 * *Files identical despite different names*

### Comparing `kor-0.8.1/kor/encoders/encode.py` & `kor-0.9.0/kor/encoders/encode.py`

 * *Files identical despite different names*

### Comparing `kor-0.8.1/kor/encoders/json_data.py` & `kor-0.9.0/kor/encoders/json_data.py`

 * *Files identical despite different names*

### Comparing `kor-0.8.1/kor/encoders/typedefs.py` & `kor-0.9.0/kor/encoders/typedefs.py`

 * *Files identical despite different names*

### Comparing `kor-0.8.1/kor/encoders/utils.py` & `kor-0.9.0/kor/encoders/utils.py`

 * *Files identical despite different names*

### Comparing `kor-0.8.1/kor/encoders/xml.py` & `kor-0.9.0/kor/encoders/xml.py`

 * *Files identical despite different names*

### Comparing `kor-0.8.1/kor/examples.py` & `kor-0.9.0/kor/examples.py`

 * *Files identical despite different names*

### Comparing `kor-0.8.1/kor/extraction/api.py` & `kor-0.9.0/kor/extraction/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     node: Object,
     *,
     encoder_or_encoder_class: Union[Type[Encoder], Encoder, str] = "csv",
     type_descriptor: Union[TypeDescriptor, str] = "typescript",
     validator: Optional[Validator] = None,
     input_formatter: InputFormatter = None,
     instruction_template: Optional[PromptTemplate] = None,
+    verbose: Optional[bool] = None,
     **encoder_kwargs: Any,
 ) -> LLMChain:
     """Create an extraction chain.
     
     Args:
         llm: the language model used for extraction
         node: the schematic description of what to extract from text
@@ -69,20 +70,21 @@
             * `Callable`: user provided function
         instruction_template: optional prompt template to use, use to over-ride prompt
              used for generating the instruction section of the prompt.
              It accepts 2 optional input variables:
              * "type_description": type description of the node (from TypeDescriptor)
              * "format_instructions": information on how to format the output
                (from Encoder)
+        verbose: if provided, sets the verbosity on the chain, otherwise default
+                 verbosity of the chain will be used
         encoder_kwargs: Keyword arguments to pass to the encoder class
 
     Returns:
         A langchain chain
         
-        
     Examples:
     
     .. code-block:: python
   
         # For CSV encoding
         chain = create_extraction_chain(llm, node, encoder_or_encoder_class="csv")
     
@@ -90,24 +92,30 @@
         chain = create_extraction_chain(llm, node, encoder_or_encoder_class="JSON",
                                         input_formatter="triple_quotes")
     """
     if not isinstance(node, Object):
         raise ValueError(f"node must be an Object got {type(node)}")
     encoder = initialize_encoder(encoder_or_encoder_class, node, **encoder_kwargs)
     type_descriptor_to_use = initialize_type_descriptors(type_descriptor)
+
+    chain_kwargs = {}
+    if verbose is not None:
+        chain_kwargs["verbose"] = verbose
+
     return LLMChain(
         llm=llm,
         prompt=create_langchain_prompt(
             node,
             encoder,
             type_descriptor_to_use,
             validator=validator,
             instruction_template=instruction_template,
             input_formatter=input_formatter,
         ),
+        **chain_kwargs,
     )
 
 
 async def extract_from_documents(
     chain: LLMChain,
     documents: Sequence[Document],
     *,
```

### Comparing `kor-0.8.1/kor/extraction/parser.py` & `kor-0.9.0/kor/extraction/parser.py`

 * *Files identical despite different names*

### Comparing `kor-0.8.1/kor/extraction/typedefs.py` & `kor-0.9.0/kor/extraction/typedefs.py`

 * *Files identical despite different names*

### Comparing `kor-0.8.1/kor/nodes.py` & `kor-0.9.0/kor/nodes.py`

 * *Files identical despite different names*

### Comparing `kor-0.8.1/kor/prompts.py` & `kor-0.9.0/kor/prompts.py`

 * *Files identical despite different names*

### Comparing `kor-0.8.1/kor/type_descriptors.py` & `kor-0.9.0/kor/type_descriptors.py`

 * *Files identical despite different names*

### Comparing `kor-0.8.1/kor/validators.py` & `kor-0.9.0/kor/validators.py`

 * *Files identical despite different names*

### Comparing `kor-0.8.1/pyproject.toml` & `kor-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kor"
-version = "0.8.1"
+version = "0.9.0"
 description = "Extract information with LLMs from text"
 authors = ["Eugene Yurtsev <eyurtsev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://www.github.com/eyurtsev/kor"
 
 [tool.poetry.dependencies]
```

### Comparing `kor-0.8.1/setup.py` & `kor-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['langchain>=0.0.110', 'openai>=0.27,<0.28', 'pandas>=1.5.3,<2.0.0']
 
 extras_require = \
 {'html': ['markdownify>=0.11.6,<0.12.0']}
 
 setup_kwargs = {
     'name': 'kor',
-    'version': '0.8.1',
+    'version': '0.9.0',
     'description': 'Extract information with LLMs from text',
     'long_description': '**⚠ WARNING: Prototype with unstable API. 🚧**  \n\n[![Unit Tests](https://github.com/eyurtsev/kor/actions/workflows/test.yml/badge.svg?branch=main&event=push)](https://github.com/eyurtsev/kor/actions/workflows/test.yml)\n[![Test Docs](https://github.com/eyurtsev/kor/actions/workflows/doc_test.yaml/badge.svg?branch=main&event=push)](https://github.com/eyurtsev/kor/actions/workflows/doc_test.yaml)\n\n# Kor\n\n\nThis is a half-baked prototype that "helps" you extract structured data from text using LLMs 🧩.\n\nSpecify the schema of what should be extracted and provide some examples.\n\nKor will generate a prompt, send it to the specified LLM and parse out the\noutput. \n\nYou might even get results back.\n\nSee [documentation](https://eyurtsev.github.io/kor/).\n\n## Version >=0.4.0\n\n* Integrated with langchain framework.\n* The code below uses Kor style schema, but you can also use [pydantic](https://eyurtsev.github.io/kor/validation.html).\n\n\n```python\n\n  from langchain.chat_models import ChatOpenAI\n  from kor import create_extraction_chain, Object, Text, Number\n\n  llm = ChatOpenAI(\n      model_name="gpt-3.5-turbo",\n      temperature=0,\n      max_tokens=2000,\n      frequency_penalty=0,\n      presence_penalty=0,\n      top_p=1.0,\n  )\n\n  schema = Object(\n    id="player",\n    description=(\n        "User is controling a music player to select songs, pause or start them or play"\n        " music by a particular artist."\n    ),\n    attributes=[\n        Text(\n            id="song",\n            description="User wants to play this song",\n            examples=[],\n            many=True,\n        ),\n        Text(\n            id="album",\n            description="User wants to play this album",\n            examples=[],\n            many=True,\n        ),\n        Text(\n            id="artist",\n            description="Music by the given artist",\n            examples=[("Songs by paul simon", "paul simon")],\n            many=True,\n        ),\n        Text(\n            id="action",\n            description="Action to take one of: `play`, `stop`, `next`, `previous`.",\n            examples=[\n                ("Please stop the music", "stop"),\n                ("play something", "play"),\n                ("play a song", "play"),\n                ("next song", "next"),\n            ],\n        ),\n    ],\n    many=False,\n)\n\n  chain = create_extraction_chain(llm, schema, encoder_or_encoder_class=\'json\')\n  chain.predict_and_parse(text="play songs by paul simon and led zeppelin and the doors")[\'data\']\n```\n\n```python\n  {\'player\': {\'artist\': [\'paul simon\', \'led zeppelin\', \'the doors\']}}\n```\n\n## Compatibility\n\n`Kor` is tested against python 3.8, 3.9, 3.10, 3.11.\n\n## Installaton \n\n```sh\npip install kor\n```\n\n## 💡 Ideas\n\nIdeas of some things that could be done with Kor.\n\n* Extract data from text that matches an extraction schema.\n* Power an AI assistant with skills by precisely understanding a user request.\n* Provide natural language access to an existing API.\n\n## 🚧 Prototype\n\nPrototype! So the API is not expected to be stable!\n\n##  ✨ What does Kor excel at?  🌟 \n\n* Making mistakes! Plenty of them!\n* Slow! It uses large prompts with examples, and works best with the larger slower LLMs.\n* Crashing for long enough pieces of text! Context length window could become\n  limiting when working with large forms or long text inputs.\n\nThe expectation is that as LLMs improve some of these issues will be mitigated.\n\n## Limtations\n\nNo limitations whatsoever. Do take a look at the section directly above as well\nas at the section about compatibility.\n\n## Potential Changes\n\n* Adding validators\n* Built-in components to quickly assemble schema with examples\n* Add routing layer to select appropriate extraction schema for a use case when\n  many schema exist\n\n## 🎶 Why the name?\n\nFast to type and sufficiently unique.\n\n## Contributing\n\nIf you have any ideas or feature requests, please open an issue and share!\n\nSee [CONTRIBUTING.md](https://github.com/eyurtsev/kor/blob/main/CONTRIBUTING.md) for more information.\n\n## Other packages\n\nProbabilistically speaking this package is unlikely to work for your use case.\n\nSo here are some great alternatives:\n\n* [Promptify](https://github.com/promptslab/Promptify)\n* [MiniChain](https://srush.github.io/MiniChain/examples/stats/)\n',
     'author': 'Eugene Yurtsev',
     'author_email': 'eyurtsev@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://www.github.com/eyurtsev/kor',
```

### Comparing `kor-0.8.1/PKG-INFO` & `kor-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kor
-Version: 0.8.1
+Version: 0.9.0
 Summary: Extract information with LLMs from text
 Home-page: https://www.github.com/eyurtsev/kor
 License: MIT
 Author: Eugene Yurtsev
 Author-email: eyurtsev@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```


# Comparing `tmp/guardrails-ai-0.1.5.tar.gz` & `tmp/guardrails-ai-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guardrails-ai-0.1.5.tar", last modified: Thu Mar 30 10:52:40 2023, max compression
+gzip compressed data, was "guardrails-ai-0.1.6.tar", last modified: Mon Apr 24 16:26:36 2023, max compression
```

## Comparing `guardrails-ai-0.1.5.tar` & `guardrails-ai-0.1.6.tar`

### file list

```diff
@@ -1,33 +1,50 @@
-drwxr-xr-x   0 shreyarajpal   (501) staff       (20)        0 2023-03-30 10:52:40.343996 guardrails-ai-0.1.5/
--rw-r--r--   0 shreyarajpal   (501) staff       (20)    11357 2023-03-13 06:08:31.000000 guardrails-ai-0.1.5/LICENSE
--rw-r--r--   0 shreyarajpal   (501) staff       (20)      165 2023-03-13 07:06:00.000000 guardrails-ai-0.1.5/MANIFEST.in
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     7654 2023-03-30 10:52:40.343712 guardrails-ai-0.1.5/PKG-INFO
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     7023 2023-03-30 10:48:40.000000 guardrails-ai-0.1.5/README.md
-drwxr-xr-x   0 shreyarajpal   (501) staff       (20)        0 2023-03-30 10:52:40.339856 guardrails-ai-0.1.5/guardrails/
--rw-r--r--   0 shreyarajpal   (501) staff       (20)      464 2023-03-30 10:26:26.000000 guardrails-ai-0.1.5/guardrails/__init__.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     3705 2023-03-30 10:48:40.000000 guardrails-ai-0.1.5/guardrails/constants.xml
--rw-r--r--   0 shreyarajpal   (501) staff       (20)    15523 2023-03-30 10:36:18.000000 guardrails-ai-0.1.5/guardrails/datatypes.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     5560 2023-03-30 10:26:26.000000 guardrails-ai-0.1.5/guardrails/guard.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     2755 2023-03-30 10:48:40.000000 guardrails-ai-0.1.5/guardrails/llm_providers.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     2779 2023-03-30 10:45:06.000000 guardrails-ai-0.1.5/guardrails/prompt.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     6587 2023-03-30 10:26:26.000000 guardrails-ai-0.1.5/guardrails/rail.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     9050 2023-03-30 10:45:06.000000 guardrails-ai-0.1.5/guardrails/run.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)    18723 2023-03-30 10:45:06.000000 guardrails-ai-0.1.5/guardrails/schema.py
-drwxr-xr-x   0 shreyarajpal   (501) staff       (20)        0 2023-03-30 10:52:40.341754 guardrails-ai-0.1.5/guardrails/utils/
--rw-r--r--   0 shreyarajpal   (501) staff       (20)        0 2023-03-13 06:08:31.000000 guardrails-ai-0.1.5/guardrails/utils/__init__.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     1555 2023-03-15 07:40:10.000000 guardrails-ai-0.1.5/guardrails/utils/constants.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     2187 2023-03-30 10:26:26.000000 guardrails-ai-0.1.5/guardrails/utils/docs_utils.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     5293 2023-03-30 10:45:06.000000 guardrails-ai-0.1.5/guardrails/utils/logs_utils.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     2566 2023-03-30 10:26:26.000000 guardrails-ai-0.1.5/guardrails/utils/misc.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     3349 2023-03-30 10:26:26.000000 guardrails-ai-0.1.5/guardrails/utils/pydantic_utils.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     8731 2023-03-30 10:26:26.000000 guardrails-ai-0.1.5/guardrails/utils/reask_utils.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)    29301 2023-03-30 10:45:06.000000 guardrails-ai-0.1.5/guardrails/validators.py
--rw-r--r--   0 shreyarajpal   (501) staff       (20)       22 2023-03-30 10:52:02.000000 guardrails-ai-0.1.5/guardrails/version.py
-drwxr-xr-x   0 shreyarajpal   (501) staff       (20)        0 2023-03-30 10:52:40.343270 guardrails-ai-0.1.5/guardrails_ai.egg-info/
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     7654 2023-03-30 10:52:40.000000 guardrails-ai-0.1.5/guardrails_ai.egg-info/PKG-INFO
--rw-r--r--   0 shreyarajpal   (501) staff       (20)      681 2023-03-30 10:52:40.000000 guardrails-ai-0.1.5/guardrails_ai.egg-info/SOURCES.txt
--rw-r--r--   0 shreyarajpal   (501) staff       (20)        1 2023-03-30 10:52:40.000000 guardrails-ai-0.1.5/guardrails_ai.egg-info/dependency_links.txt
--rw-r--r--   0 shreyarajpal   (501) staff       (20)      323 2023-03-30 10:52:40.000000 guardrails-ai-0.1.5/guardrails_ai.egg-info/requires.txt
--rw-r--r--   0 shreyarajpal   (501) staff       (20)       11 2023-03-30 10:52:40.000000 guardrails-ai-0.1.5/guardrails_ai.egg-info/top_level.txt
--rw-r--r--   0 shreyarajpal   (501) staff       (20)       38 2023-03-30 10:52:40.344083 guardrails-ai-0.1.5/setup.cfg
--rw-r--r--   0 shreyarajpal   (501) staff       (20)     4160 2023-03-30 10:26:26.000000 guardrails-ai-0.1.5/setup.py
+drwxr-xr-x   0 shreyarajpal   (501) staff       (20)        0 2023-04-24 16:26:36.575432 guardrails-ai-0.1.6/
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)    11357 2023-03-13 06:08:31.000000 guardrails-ai-0.1.6/LICENSE
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)      165 2023-03-13 07:06:00.000000 guardrails-ai-0.1.6/MANIFEST.in
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     8011 2023-04-24 16:26:36.574864 guardrails-ai-0.1.6/PKG-INFO
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     7330 2023-04-02 04:41:18.000000 guardrails-ai-0.1.6/README.md
+drwxr-xr-x   0 shreyarajpal   (501) staff       (20)        0 2023-04-24 16:26:36.559978 guardrails-ai-0.1.6/guardrails/
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)      549 2023-04-21 21:02:59.000000 guardrails-ai-0.1.6/guardrails/__init__.py
+drwxr-xr-x   0 shreyarajpal   (501) staff       (20)        0 2023-04-24 16:26:36.561770 guardrails-ai-0.1.6/guardrails/applications/
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)        0 2023-04-21 21:02:59.000000 guardrails-ai-0.1.6/guardrails/applications/__init__.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     6379 2023-04-24 16:25:52.000000 guardrails-ai-0.1.6/guardrails/applications/text2sql.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)      702 2023-04-24 16:25:52.000000 guardrails-ai-0.1.6/guardrails/applications/text2sql.rail
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     1613 2023-04-03 06:56:37.000000 guardrails-ai-0.1.6/guardrails/cli.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     4694 2023-04-21 08:15:57.000000 guardrails-ai-0.1.6/guardrails/constants.xml
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)    16775 2023-04-24 00:55:28.000000 guardrails-ai-0.1.6/guardrails/datatypes.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     7361 2023-04-24 00:55:28.000000 guardrails-ai-0.1.6/guardrails/document_store.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     4241 2023-04-24 00:55:28.000000 guardrails-ai-0.1.6/guardrails/embedding.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     6886 2023-04-21 21:02:59.000000 guardrails-ai-0.1.6/guardrails/guard.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     4627 2023-04-24 16:25:52.000000 guardrails-ai-0.1.6/guardrails/llm_providers.py
+drwxr-xr-x   0 shreyarajpal   (501) staff       (20)        0 2023-04-24 16:26:36.564125 guardrails-ai-0.1.6/guardrails/prompt/
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)      115 2023-04-21 08:15:57.000000 guardrails-ai-0.1.6/guardrails/prompt/__init__.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     3004 2023-04-21 21:02:59.000000 guardrails-ai-0.1.6/guardrails/prompt/base_prompt.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     1279 2023-04-21 21:02:59.000000 guardrails-ai-0.1.6/guardrails/prompt/instructions.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)      796 2023-04-21 21:02:59.000000 guardrails-ai-0.1.6/guardrails/prompt/prompt.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     7373 2023-04-21 08:58:33.000000 guardrails-ai-0.1.6/guardrails/rail.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)    10977 2023-04-21 21:02:59.000000 guardrails-ai-0.1.6/guardrails/run.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)    18951 2023-04-21 21:02:59.000000 guardrails-ai-0.1.6/guardrails/schema.py
+drwxr-xr-x   0 shreyarajpal   (501) staff       (20)        0 2023-04-24 16:26:36.569217 guardrails-ai-0.1.6/guardrails/utils/
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)        0 2023-03-13 06:08:31.000000 guardrails-ai-0.1.6/guardrails/utils/__init__.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     1555 2023-03-15 07:40:10.000000 guardrails-ai-0.1.6/guardrails/utils/constants.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     2187 2023-04-21 08:58:53.000000 guardrails-ai-0.1.6/guardrails/utils/docs_utils.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     6100 2023-04-21 21:02:59.000000 guardrails-ai-0.1.6/guardrails/utils/logs_utils.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     2567 2023-04-21 21:02:59.000000 guardrails-ai-0.1.6/guardrails/utils/misc.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     3349 2023-03-30 10:26:26.000000 guardrails-ai-0.1.6/guardrails/utils/pydantic_utils.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     8944 2023-04-21 21:02:59.000000 guardrails-ai-0.1.6/guardrails/utils/reask_utils.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     4030 2023-04-21 21:02:59.000000 guardrails-ai-0.1.6/guardrails/utils/sql_utils.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)    35273 2023-04-24 00:55:28.000000 guardrails-ai-0.1.6/guardrails/validators.py
+drwxr-xr-x   0 shreyarajpal   (501) staff       (20)        0 2023-04-24 16:26:36.570937 guardrails-ai-0.1.6/guardrails/vectordb/
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)       93 2023-04-24 00:55:28.000000 guardrails-ai-0.1.6/guardrails/vectordb/__init__.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     2953 2023-04-24 00:55:28.000000 guardrails-ai-0.1.6/guardrails/vectordb/base.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     3244 2023-04-24 00:55:28.000000 guardrails-ai-0.1.6/guardrails/vectordb/faiss.py
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)       22 2023-04-24 00:55:28.000000 guardrails-ai-0.1.6/guardrails/version.py
+drwxr-xr-x   0 shreyarajpal   (501) staff       (20)        0 2023-04-24 16:26:36.574168 guardrails-ai-0.1.6/guardrails_ai.egg-info/
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     8011 2023-04-24 16:26:36.000000 guardrails-ai-0.1.6/guardrails_ai.egg-info/PKG-INFO
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     1125 2023-04-24 16:26:36.000000 guardrails-ai-0.1.6/guardrails_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)        1 2023-04-24 16:26:36.000000 guardrails-ai-0.1.6/guardrails_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)       50 2023-04-24 16:26:36.000000 guardrails-ai-0.1.6/guardrails_ai.egg-info/entry_points.txt
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)      519 2023-04-24 16:26:36.000000 guardrails-ai-0.1.6/guardrails_ai.egg-info/requires.txt
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)       11 2023-04-24 16:26:36.000000 guardrails-ai-0.1.6/guardrails_ai.egg-info/top_level.txt
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)       38 2023-04-24 16:26:36.575691 guardrails-ai-0.1.6/setup.cfg
+-rw-r--r--   0 shreyarajpal   (501) staff       (20)     4616 2023-04-21 21:02:59.000000 guardrails-ai-0.1.6/setup.py
```

### Comparing `guardrails-ai-0.1.5/LICENSE` & `guardrails-ai-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `guardrails-ai-0.1.5/PKG-INFO` & `guardrails-ai-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: guardrails-ai
-Version: 0.1.5
+Version: 0.1.6
 Summary: Adding guardrails to large language models.
 Home-page: https://github.com/shreyar/guardrails
 Author: Shreya Rajpal
 Author-email: shreya.rajpal@gmail.com
 License: Apache 2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: sql
+Provides-Extra: manifest
+Provides-Extra: vectordb
 Provides-Extra: profanity
 Provides-Extra: critique
 License-File: LICENSE
 
 
 # 🛤️ Guardrails
 
@@ -39,15 +41,15 @@
 - does pydantic-style validation of LLM outputs (including semantic validation such as checking for bias in generated text, checking for bugs in generated code, etc.)
 - takes corrective actions (e.g. reasking LLM) when validation fails,
 - enforces structure and type guarantees (e.g. JSON).
 
 
 ## 🚒 Under the hood
 
-Guardrails provides a format (`.rail`) for enforcing a specification on an LLM output, and a lightweight wrapper around LLM API calls to implement this spec.
+Guardrails provides a file format (`.rail`) for enforcing a specification on an LLM output, and a lightweight wrapper around LLM API calls to implement this spec.
 
 1. `rail` (**R**eliable **AI** markup **L**anguage) files for specifying structure and type information, validators and corrective actions over LLM outputs.
 2. `gd.Guard` wraps around LLM API calls to structure, validate and correct the outputs.
 
 ``` mermaid
 graph LR
     A[Create `RAIL` spec] --> B["Initialize `guard` from spec"];
@@ -86,21 +88,21 @@
 - [ ] Improving reasking logic
 - [ ] A guardrails.js implementation
 - [ ] VSCode extension for `.rail` files
 - [ ] Next version of `.rail` format
 - [ ] Add more LLM providers
 
 ## 🚀 Getting Started
-Let's go through an example where we ask an LLM to explain what a "bank run" is in a tweet, and generate URL links to relevant news articles. We'll generate a `.rail` spec for this and then use Guardrails to enforce it. You can see more examples in the docs.
+Let's go through an example where we ask an LLM to explain what a "bank run" is in a tweet, and generate URLs to relevant news articles. We'll generate a `.rail` spec for this and then use Guardrails to enforce it. You can see more examples in the docs.
 
 ### 📝 Creating a `RAIL` spec
 
 We create a `RAIL` spec to describe the expected structure and types of the LLM output, the quality criteria for the output to be considered valid, and corrective actions to be taken if the output is invalid.
 
-Specifically, we use `RAIL` to
+Using `RAIL`, we:
 - Request the LLM to generate an object with two fields: `explanation` and `follow_up_url`.
 - For the `explanation` field, ensure the max length of the generated string should be between 200 and 280 characters.
   - If the explanation is not of valid length, `reask` the LLM.
 - For the `follow_up_url` field, the URL should be reachable.
   - If the URL is not reachable, we will `filter` it out of the response.
 
 
@@ -160,14 +162,16 @@
     <object name="bank_run" format="length: 2">
         <string name="explanation" description="A paragraph about what a bank run is." format="length: 200 280" on-fail-length="reask" />
         <url name="follow_up_url" description="A web URL where I can read more about bank runs." required="true" format="valid-url" on-fail-valid-url="filter" />
     </object>
 </output>
 
 ONLY return a valid JSON object (no other text is necessary). The JSON MUST conform to the XML format, including any types and format requests e.g. requests for lists, objects and specific types. Be correct and concise.
+
+JSON Output:
 ```
 
 Call the `Guard` object with the LLM API call as the first argument and add any additional arguments to the LLM API call as the remaining arguments.
 
 
 ```python
 import openai
@@ -187,7 +191,11 @@
     'bank_run': {
         'explanation': 'A bank run is when a large number of people withdraw their deposits from a bank due to concerns about its solvency. This can cause a financial crisis if the bank is unable to meet the demand for withdrawals.',
         'follow_up_url': 'https://www.investopedia.com/terms/b/bankrun.asp'
     }
 }
 
 ```
+
+## 🛠️ Contributing
+
+Get started by checking out Github issues and of course using Guardrails to familiarize yourself with the project. Guardrails is still actively under development and any support is gladly welcomed. Feel free to open an issue, or reach out if you would like to add to the project!
```

### Comparing `guardrails-ai-0.1.5/README.md` & `guardrails-ai-0.1.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 - does pydantic-style validation of LLM outputs (including semantic validation such as checking for bias in generated text, checking for bugs in generated code, etc.)
 - takes corrective actions (e.g. reasking LLM) when validation fails,
 - enforces structure and type guarantees (e.g. JSON).
 
 
 ## 🚒 Under the hood
 
-Guardrails provides a format (`.rail`) for enforcing a specification on an LLM output, and a lightweight wrapper around LLM API calls to implement this spec.
+Guardrails provides a file format (`.rail`) for enforcing a specification on an LLM output, and a lightweight wrapper around LLM API calls to implement this spec.
 
 1. `rail` (**R**eliable **AI** markup **L**anguage) files for specifying structure and type information, validators and corrective actions over LLM outputs.
 2. `gd.Guard` wraps around LLM API calls to structure, validate and correct the outputs.
 
 ``` mermaid
 graph LR
     A[Create `RAIL` spec] --> B["Initialize `guard` from spec"];
@@ -65,21 +65,21 @@
 - [ ] Improving reasking logic
 - [ ] A guardrails.js implementation
 - [ ] VSCode extension for `.rail` files
 - [ ] Next version of `.rail` format
 - [ ] Add more LLM providers
 
 ## 🚀 Getting Started
-Let's go through an example where we ask an LLM to explain what a "bank run" is in a tweet, and generate URL links to relevant news articles. We'll generate a `.rail` spec for this and then use Guardrails to enforce it. You can see more examples in the docs.
+Let's go through an example where we ask an LLM to explain what a "bank run" is in a tweet, and generate URLs to relevant news articles. We'll generate a `.rail` spec for this and then use Guardrails to enforce it. You can see more examples in the docs.
 
 ### 📝 Creating a `RAIL` spec
 
 We create a `RAIL` spec to describe the expected structure and types of the LLM output, the quality criteria for the output to be considered valid, and corrective actions to be taken if the output is invalid.
 
-Specifically, we use `RAIL` to
+Using `RAIL`, we:
 - Request the LLM to generate an object with two fields: `explanation` and `follow_up_url`.
 - For the `explanation` field, ensure the max length of the generated string should be between 200 and 280 characters.
   - If the explanation is not of valid length, `reask` the LLM.
 - For the `follow_up_url` field, the URL should be reachable.
   - If the URL is not reachable, we will `filter` it out of the response.
 
 
@@ -139,14 +139,16 @@
     <object name="bank_run" format="length: 2">
         <string name="explanation" description="A paragraph about what a bank run is." format="length: 200 280" on-fail-length="reask" />
         <url name="follow_up_url" description="A web URL where I can read more about bank runs." required="true" format="valid-url" on-fail-valid-url="filter" />
     </object>
 </output>
 
 ONLY return a valid JSON object (no other text is necessary). The JSON MUST conform to the XML format, including any types and format requests e.g. requests for lists, objects and specific types. Be correct and concise.
+
+JSON Output:
 ```
 
 Call the `Guard` object with the LLM API call as the first argument and add any additional arguments to the LLM API call as the remaining arguments.
 
 
 ```python
 import openai
@@ -166,7 +168,11 @@
     'bank_run': {
         'explanation': 'A bank run is when a large number of people withdraw their deposits from a bank due to concerns about its solvency. This can cause a financial crisis if the bank is unable to meet the demand for withdrawals.',
         'follow_up_url': 'https://www.investopedia.com/terms/b/bankrun.asp'
     }
 }
 
 ```
+
+## 🛠️ Contributing
+
+Get started by checking out Github issues and of course using Guardrails to familiarize yourself with the project. Guardrails is still actively under development and any support is gladly welcomed. Feel free to open an issue, or reach out if you would like to add to the project!
```

### Comparing `guardrails-ai-0.1.5/guardrails/constants.xml` & `guardrails-ai-0.1.6/guardrails/constants.xml`

 * *Files 14% similar despite different names*

#### Comparing `guardrails-ai-0.1.5/guardrails/constants.xml` & `guardrails-ai-0.1.6/guardrails/constants.xml`

```diff
@@ -35,8 +35,19 @@
 - `
 <![CDATA[<string name='foo' format='two-words lower-case' />`]]>    =&gt; `{{{{'foo': 'example one'}}}}`
 - `
 <![CDATA[<list name='bar'><string format='upper-case' /></list>]]>    ` =&gt; `{{{{&quot;bar&quot;: ['STRING ONE', 'STRING TWO', etc.]}}}}`
 - `
 <![CDATA[<object name='baz'><string name="foo" format="capitalize two-words" /><integer name="index" format="1-indexed" /></object>]]>    ` =&gt; `{{{{'baz': {{{{'foo': 'Some String', 'index': 1}}}}}}}}`
   </complete_json_suffix_v2>
+  <json_suffix_prompt_examples>
+    ONLY return a valid JSON object (no other text is necessary), where the key of the field in JSON is the `name` attribute of the corresponding XML, and the value is of the type specified by the corresponding XML's tag. The JSON MUST conform to the XML format, including any types and format requests e.g. requests for lists, objects and specific types. Be correct and concise. If you are unsure anywhere, enter `None`.
+
+Here are examples of simple (XML, JSON) pairs that show the expected behavior:
+- `
+<![CDATA[<string name='foo' format='two-words lower-case' />`]]>    =&gt; `{{{{'foo': 'example one'}}}}`
+- `
+<![CDATA[<list name='bar'><string format='upper-case' /></list>]]>    ` =&gt; `{{{{&quot;bar&quot;: ['STRING ONE', 'STRING TWO', etc.]}}}}`
+- `
+<![CDATA[<object name='baz'><string name="foo" format="capitalize two-words" /><integer name="index" format="1-indexed" /></object>]]>    ` =&gt; `{{{{'baz': {{{{'foo': 'Some String', 'index': 1}}}}}}}}`
+  </json_suffix_prompt_examples>
 </constants>
```

### Comparing `guardrails-ai-0.1.5/guardrails/datatypes.py` & `guardrails-ai-0.1.6/guardrails/datatypes.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,37 +38,38 @@
             else:
                 assert len(self._children) == 1, "Must have exactly one child."
                 yield None, list(self._children.values())[0], el_child
 
     def iter(
         self, element: ET._Element
     ) -> Generator[Tuple[str, "DataType", ET._Element], None, None]:
-        """Return a tuple of (name, child_data_type, child_element) for each
-        child."""
+        """
+        Iterate over the children of an element.
+
+        Yields tuples of (name, child_data_type, child_element) for each child.
+        """
         for el_child in element:
-            if "name" in el_child.attrib:
+            if element.tag == "list":
+                assert len(self._children) == 1, "Must have exactly one child."
+                yield None, list(self._children.values())[0], el_child
+            else:
                 name: str = el_child.attrib["name"]
                 child_data_type: DataType = self._children[name]
                 yield name, child_data_type, el_child
-            else:
-                assert len(self._children) == 1, "Must have exactly one child."
-                yield None, list(self._children.values())[0], el_child
 
-    @classmethod
-    def from_str(cls, s: str) -> "DataType":
+    def from_str(self, s: str) -> "DataType":
         """Create a DataType from a string.
 
         Note: ScalarTypes like int, float, bool, etc. will override this method.
         Other ScalarTypes like string, email, url, etc. will not override this
         """
         return s
 
     def validate(self, key: str, value: Any, schema: Dict) -> Dict:
         """Validate a value."""
-
         value = self.from_str(value)
 
         for validator in self.validators:
             schema = validator.validate_with_correction(key, value, schema)
 
         return schema
 
@@ -117,52 +118,48 @@
     pass
 
 
 @register_type("string")
 class String(ScalarType):
     """Element tag: `<string>`"""
 
-    @classmethod
-    def from_str(cls, s: str) -> "String":
+    def from_str(self, s: str) -> "String":
         """Create a String from a string."""
         return s
 
 
 @register_type("integer")
 class Integer(ScalarType):
     """Element tag: `<integer>`"""
 
-    @classmethod
-    def from_str(cls, s: str) -> "Integer":
+    def from_str(self, s: str) -> "Integer":
         """Create an Integer from a string."""
         if s is None:
             return None
 
         return int(s)
 
 
 @register_type("float")
 class Float(ScalarType):
     """Element tag: `<float>`"""
 
-    @classmethod
-    def from_str(cls, s: str) -> "Float":
+    def from_str(self, s: str) -> "Float":
         """Create a Float from a string."""
         if s is None:
             return None
 
         return float(s)
 
 
 @register_type("bool")
 class Boolean(ScalarType):
     """Element tag: `<bool>`"""
 
-    @classmethod
-    def from_str(cls, s: Union[str, bool]) -> "Boolean":
+    def from_str(self, s: Union[str, bool]) -> "Boolean":
         """Create a Boolean from a string."""
         if s is None:
             return None
 
         if isinstance(s, bool):
             return s
 
@@ -172,36 +169,72 @@
             return False
         else:
             raise ValueError(f"Invalid boolean value: {s}")
 
 
 @register_type("date")
 class Date(ScalarType):
-    """Element tag: `<date>`"""
+    """Element tag: `<date>`
 
-    @classmethod
-    def from_str(cls, s: str) -> "Date":
+    To configure the date format, create a date-format attribute on the element.
+    E.g. `<date name="..." ... date-format="%Y-%m-%d" />`
+    """
+
+    def __init__(
+        self, children: Dict[str, Any], format_attr: "FormatAttr", element: ET._Element
+    ) -> None:
+        self.date_format = "%Y-%m-%d"
+        super().__init__(children, format_attr, element)
+
+    def from_str(self, s: str) -> "Date":
         """Create a Date from a string."""
         if s is None:
             return None
 
-        return datetime.datetime.strptime(s, "%Y-%m-%d").date()
+        return datetime.datetime.strptime(s, self.date_format).date()
+
+    @classmethod
+    def from_xml(cls, element: ET._Element, strict: bool = False) -> "DataType":
+        datatype = super().from_xml(element, strict)
+
+        if "date-format" in element.attrib:
+            datatype.date_format = element.attrib["date-format"]
+
+        return datatype
 
 
 @register_type("time")
 class Time(ScalarType):
-    """Element tag: `<time>`"""
+    """Element tag: `<time>`
 
-    @classmethod
-    def from_str(cls, s: str) -> "Time":
+    To configure the date format, create a date-format attribute on the element.
+    E.g. `<time name="..." ... time-format="%H:%M:%S" />`
+    """
+
+    def __init__(
+        self, children: Dict[str, Any], format_attr: "FormatAttr", element: ET._Element
+    ) -> None:
+        self.time_format = "%H:%M:%S"
+        super().__init__(children, format_attr, element)
+
+    def from_str(self, s: str) -> "Time":
         """Create a Time from a string."""
         if s is None:
             return None
 
-        return datetime.datetime.strptime(s, "%H:%M:%S").time()
+        return datetime.datetime.strptime(s, self.time_format).time()
+
+    @classmethod
+    def from_xml(cls, element: ET._Element, strict: bool = False) -> "DataType":
+        datatype = super().from_xml(element, strict)
+
+        if "time-format" in element.attrib:
+            datatype.date_format = element.attrib["time-format"]
+
+        return datatype
 
 
 @register_type("email")
 class Email(ScalarType):
     """Element tag: `<email>`"""
```

### Comparing `guardrails-ai-0.1.5/guardrails/guard.py` & `guardrails-ai-0.1.6/guardrails/guard.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
-from typing import Callable, Dict, Optional, Tuple
+from string import Formatter
+from typing import Callable, Dict, Optional, Tuple, Union
 
 from eliot import start_action, to_file
 
 from guardrails.llm_providers import PromptCallable, get_llm_ask
-from guardrails.prompt import Prompt
+from guardrails.prompt import Instructions, Prompt
 from guardrails.rail import Rail
 from guardrails.run import Runner
 from guardrails.schema import InputSchema, OutputSchema
 from guardrails.utils.logs_utils import GuardState
 from guardrails.utils.reask_utils import sub_reasks_with_fixed_values
 
 logger = logging.getLogger(__name__)
@@ -31,26 +32,32 @@
         rail: Rail,
         num_reasks: int = 1,
     ):
         """Initialize the Guard."""
         self.rail = rail
         self.num_reasks = num_reasks
         self.guard_state = GuardState([])
+        self._reask_prompt = None
 
     @property
     def input_schema(self) -> InputSchema:
         """Return the input schema."""
         return self.rail.input_schema
 
     @property
     def output_schema(self) -> OutputSchema:
         """Return the output schema."""
         return self.rail.output_schema
 
     @property
+    def instructions(self) -> Instructions:
+        """Return the instruction-prompt."""
+        return self.rail.instructions
+
+    @property
     def prompt(self) -> Prompt:
         """Return the prompt."""
         return self.rail.prompt
 
     @property
     def raw_prompt(self) -> Prompt:
         """Return the prompt, alias for `prompt`."""
@@ -67,14 +74,33 @@
         return self.rail.script
 
     @property
     def state(self) -> GuardState:
         """Return the state."""
         return self.guard_state
 
+    @property
+    def reask_prompt(self) -> Prompt:
+        """Return the reask prompt."""
+        return self._reask_prompt
+
+    @reask_prompt.setter
+    def reask_prompt(self, reask_prompt: Union[str, Prompt]):
+        """Set the reask prompt."""
+
+        if isinstance(reask_prompt, str):
+            reask_prompt = Prompt(reask_prompt)
+
+        # Check that the reask prompt has the correct variables
+        variables = [
+            t[1] for t in Formatter().parse(reask_prompt.source) if t[1] is not None
+        ]
+        assert set(variables) == {"previous_response", "output_schema"}
+        self._reask_prompt = reask_prompt
+
     def configure(
         self,
         num_reasks: int = 1,
     ):
         """Configure the Guard."""
         self.num_reasks = num_reasks
 
@@ -121,20 +147,25 @@
             *args: Additional arguments to pass to the LLM API.
             **kwargs: Additional keyword arguments to pass to the LLM API.
 
         Returns:
             The raw text output from the LLM and the validated output.
         """
         with start_action(action_type="guard_call", prompt_params=prompt_params):
+            if "instructions" in kwargs:
+                logger.info("Instructions overridden at call time")
+                # TODO(shreya): should we overwrite self.instructions for this run?
             runner = Runner(
+                instructions=kwargs.get("instructions", self.instructions),
                 prompt=self.prompt,
                 api=get_llm_ask(llm_api, *args, **kwargs),
                 input_schema=self.input_schema,
                 output_schema=self.output_schema,
                 num_reasks=num_reasks,
+                reask_prompt=self.reask_prompt,
             )
             guard_history = runner(prompt_params=prompt_params)
             self.guard_state = self.guard_state.push(guard_history)
             return guard_history.output, guard_history.validated_output
 
     def __repr__(self):
         return f"Guard(RAIL={self.rail})"
@@ -143,14 +174,15 @@
         yield "RAIL", self.rail
 
     def parse(
         self,
         llm_output: str,
         llm_api: PromptCallable = None,
         num_reasks: int = 1,
+        prompt_params: Dict = None,
         *args,
         **kwargs,
     ) -> Dict:
         """Alternate flow to using Guard where the llm_output is known.
 
         Args:
             llm_output: The output from the LLM.
@@ -158,17 +190,19 @@
             num_reasks: The max times to re-ask the LLM for invalid output.
 
         Returns:
             The validated response.
         """
         with start_action(action_type="guard_parse"):
             runner = Runner(
+                instructions=None,
                 prompt=None,
                 api=get_llm_ask(llm_api, *args, **kwargs) if llm_api else None,
                 input_schema=None,
                 output_schema=self.output_schema,
                 num_reasks=num_reasks,
                 output=llm_output,
+                reask_prompt=self.reask_prompt,
             )
-            guard_history = runner()
+            guard_history = runner(prompt_params=prompt_params)
             self.guard_state = self.guard_state.push(guard_history)
             return sub_reasks_with_fixed_values(guard_history.validated_output)
```

### Comparing `guardrails-ai-0.1.5/guardrails/prompt.py` & `guardrails-ai-0.1.6/guardrails/prompt/base_prompt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,37 @@
+"""Class for representing a prompt entry."""
 import re
+from string import Formatter
 from typing import Optional
 
 from guardrails.utils.constants import constants
 
 
-class Prompt:
+class BasePrompt:
+    """Base class for representing an LLM prompt."""
+
     def __init__(self, source: str, output_schema: Optional[str] = None):
         output_schema = output_schema or {}
 
         # Get variable names in the source string (surronded by 2 curly braces)
-        self.variable_names = re.findall(r"{{(.*?)}}", source)
+        self.variable_names = [
+            x[1] for x in Formatter().parse(source) if x[1] is not None
+        ]
 
         format_instructions_start_idx = self.get_format_instructions_idx(source)
 
         # Substitute constants in the prompt.
         source = self.substitute_constants(source)
         # Format instructions contain info for how to format LLM output.
         self.format_instructions = source[format_instructions_start_idx:]
 
-        self.source = source.format(output_schema=output_schema)
+        if output_schema:
+            self.source = source.format(output_schema=output_schema)
+        else:
+            self.source = source
 
     def __repr__(self) -> str:
         # Truncate the prompt to 50 characters and add ellipsis if it's longer.
         truncated_prompt = self.source[:50]
         if len(self.source) > 50:
             truncated_prompt += "..."
         return f"Prompt({truncated_prompt})"
@@ -42,16 +51,15 @@
     def __str__(self) -> str:
         return self.source
 
     def get_prompt_variables(self):
         return self.variable_names
 
     def format(self, **kwargs):
-        """Format the prompt using the given keyword arguments."""
-        return self.source.format(**kwargs)
+        raise NotImplementedError("Subclasses must implement this method.")
 
     def make_vars_optional(self):
         """Make all variables in the prompt optional."""
         for var in self.variable_names:
             self.source = self.source.replace(f"{{{var}}}", f"{{{var}:}}")
 
     def get_format_instructions_idx(self, text: str) -> Optional[int]:
```

### Comparing `guardrails-ai-0.1.5/guardrails/rail.py` & `guardrails-ai-0.1.6/guardrails/rail.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Rail class."""
 from dataclasses import dataclass, field
 from typing import List, Optional
 
 from lxml import etree as ET
 
-from guardrails.prompt import Prompt
+from guardrails.prompt import Instructions, Prompt
 from guardrails.schema import InputSchema, OutputSchema, Schema
 
+# TODO: Logging
 XMLPARSER = ET.XMLParser(encoding="utf-8")
 
 
 @dataclass
 class Script:
     variables: dict = field(default_factory=dict)
     language: str = "python"
@@ -87,14 +88,15 @@
         2. `<input strict=True/False>`, which contains the input schema
         3. `<output strict=True/False>`, which contains the output schema
         4. `<prompt>`, which contains the prompt to be passed to the LLM
     """
 
     input_schema: Optional[InputSchema] = (None,)
     output_schema: Optional[OutputSchema] = (None,)
+    instructions: Optional[Instructions] = (None,)
     prompt: Optional[Prompt] = (None,)
     script: Optional[Script] = (None,)
     version: Optional[str] = ("0.1",)
 
     @classmethod
     def from_file(cls, file_path: str) -> "Rail":
         with open(file_path, "r") as f:
@@ -133,23 +135,31 @@
         if raw_output_schema is None:
             raise ValueError("RAIL file must contain a output-schema element.")
         # Replace all expressions in the <output /> schema.
         raw_output_schema = script.replace_expressions(ET.tostring(raw_output_schema))
         raw_output_schema = ET.fromstring(raw_output_schema, parser=XMLPARSER)
         output_schema = cls.load_output_schema(raw_output_schema)
 
+        # Parse instructions for the LLM. These are optional but if given,
+        # LLMs can use them to improve their output. Commonly these are
+        # prepended to the prompt.
+        instructions = xml.find("instructions")
+        if instructions is not None:
+            instructions = cls.load_instructions(instructions, output_schema)
+
         # Load <prompt />
         prompt = xml.find("prompt")
         if prompt is None:
             raise ValueError("RAIL file must contain a prompt element.")
         prompt = cls.load_prompt(prompt, output_schema)
 
         return cls(
             input_schema=input_schema,
             output_schema=output_schema,
+            instructions=instructions,
             prompt=prompt,
             script=script,
             version=xml.attrib["version"],
         )
 
     @staticmethod
     def load_schema(root: ET._Element) -> Schema:
@@ -166,14 +176,24 @@
     @staticmethod
     def load_output_schema(root: ET._Element) -> OutputSchema:
         """Given the RAIL <output> element, create a Schema object."""
         # Recast the schema as an OutputSchema.
         return OutputSchema(root)
 
     @staticmethod
+    def load_instructions(
+        root: ET._Element, output_schema: OutputSchema
+    ) -> Instructions:
+        """Given the RAIL <instructions> element, create Instructions."""
+        return Instructions(
+            source=root.text,
+            output_schema=output_schema.transpile(),
+        )
+
+    @staticmethod
     def load_prompt(root: ET._Element, output_schema: OutputSchema) -> Prompt:
         """Given the RAIL <prompt> element, create a Prompt object."""
         return Prompt(
             source=root.text,
             output_schema=output_schema.transpile(),
         )
```

### Comparing `guardrails-ai-0.1.5/guardrails/run.py` & `guardrails-ai-0.1.6/guardrails/run.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import Callable, Dict, List, Optional, Tuple
 
 from eliot import start_action
 
 from guardrails.llm_providers import PromptCallable
-from guardrails.prompt import Prompt
+from guardrails.prompt import Instructions, Prompt
 from guardrails.schema import InputSchema, OutputSchema
 from guardrails.utils.logs_utils import GuardHistory, GuardLogs
 from guardrails.utils.reask_utils import (
     ReAsk,
     gather_reasks,
     get_reask_prompt,
     prune_json_for_reasking,
@@ -34,21 +34,23 @@
         num_reasks: The maximum number of times to reask the LLM in case of
             validation failure, defaults to 0.
         output: The output to use instead of calling the API, used in cases
             where the output is already known.
         guard_history: The guard history to use, defaults to an empty history.
     """
 
+    instructions: Optional[Instructions]
     prompt: Prompt
     api: PromptCallable
     input_schema: InputSchema
     output_schema: OutputSchema
     num_reasks: int = 0
     output: str = None
-    guard_history: GuardHistory = GuardHistory([])
+    reask_prompt: Optional[Prompt] = None
+    guard_history: GuardHistory = field(default_factory=lambda: GuardHistory([]))
 
     def _reset_guard_history(self):
         """Reset the guard history."""
         self.guard_history = GuardHistory([])
 
     def __post_init__(self):
         assert (self.prompt and self.api and not self.output) or (
@@ -62,141 +64,183 @@
         Args:
             prompt_params: Parameters to pass to the prompt in order to
                 generate the prompt string.
 
         Returns:
             The guard history.
         """
-
         self._reset_guard_history()
 
         with start_action(
             action_type="run",
+            instructions=self.instructions,
             prompt=self.prompt,
             api=self.api,
             input_schema=self.input_schema,
             output_schema=self.output_schema,
             num_reasks=self.num_reasks,
         ):
-            prompt, input_schema, output_schema = (
+            instructions, prompt, input_schema, output_schema = (
+                self.instructions,
                 self.prompt,
                 self.input_schema,
                 self.output_schema,
             )
             for index in range(self.num_reasks + 1):
                 # Run a single step.
                 validated_output, reasks = self.step(
                     index=index,
                     api=self.api,
+                    instructions=instructions,
                     prompt=prompt,
                     prompt_params=prompt_params,
                     input_schema=input_schema,
                     output_schema=output_schema,
                     output=self.output if index == 0 else None,
                 )
 
                 # Loop again?
                 if not self.do_loop(index, reasks):
                     break
                 # Get new prompt and output schema.
                 prompt, output_schema = self.prepare_to_loop(
-                    reasks, validated_output, output_schema
+                    reasks,
+                    validated_output,
+                    output_schema,
                 )
-                prompt_params = {}
 
             return self.guard_history
 
     def step(
         self,
         index: int,
         api: Callable,
+        instructions: Optional[Instructions],
         prompt: Prompt,
         prompt_params: Dict,
         input_schema: InputSchema,
         output_schema: OutputSchema,
         output: str = None,
     ):
         """Run a full step."""
         with start_action(
             action_type="step",
             index=index,
+            instructions=instructions,
             prompt=prompt,
             prompt_params=prompt_params,
             input_schema=input_schema,
             output_schema=output_schema,
         ):
             # Prepare: run pre-processing, and input validation.
             if not output:
-                prompt = self.prepare(index, prompt, prompt_params, input_schema)
+                instructions, prompt = self.prepare(
+                    index, instructions, prompt, prompt_params, input_schema
+                )
             else:
+                instructions = None
                 prompt = None
 
             # Call: run the API, and convert to dict.
-            output, output_as_dict = self.call(index, prompt, api, output)
+            output, output_as_dict = self.call(index, instructions, prompt, api, output)
 
             # Validate: run output validation.
             validated_output = self.validate(index, output_as_dict, output_schema)
 
             # Introspect: inspect validated output for reasks.
             reasks = self.introspect(index, validated_output)
 
             # Replace reask values with fixed values if terminal step.
             if not self.do_loop(index, reasks):
                 validated_output = sub_reasks_with_fixed_values(validated_output)
 
             # Log: step information.
-            self.log(prompt, output, output_as_dict, validated_output, reasks)
+            self.log(
+                prompt=prompt,
+                instructions=instructions,
+                output=output,
+                output_as_dict=output_as_dict,
+                validated_output=validated_output,
+                reasks=reasks,
+            )
 
             return validated_output, reasks
 
     def prepare(
         self,
         index: int,
+        instructions: Optional[Instructions],
         prompt: Prompt,
         prompt_params: Dict,
         input_schema: InputSchema,
-    ) -> str:
+    ) -> Prompt:
         """Prepare by running pre-processing and input validation."""
         with start_action(action_type="prepare", index=index) as action:
             if prompt_params is None:
                 prompt_params = {}
 
             if input_schema:
                 validated_prompt_params = input_schema.validate(prompt_params)
             else:
                 validated_prompt_params = prompt_params
 
-            if isinstance(prompt, Prompt):
-                prompt = prompt.format(**validated_prompt_params)
+            if isinstance(prompt, str):
+                prompt = Prompt(prompt)
+
+            prompt = prompt.format(**validated_prompt_params)
+
+            # TODO(shreya): should there be any difference to parsing params for prompt?
+            if instructions is not None and isinstance(instructions, Instructions):
+                instructions = instructions.format(**validated_prompt_params)
 
             action.log(
                 message_type="info",
+                instructions=instructions,
                 prompt=prompt,
                 prompt_params=prompt_params,
                 validated_prompt_params=validated_prompt_params,
             )
 
-        return prompt
+        return instructions, prompt
+
+    def post_process(self, output: str) -> str:
+        """Post-process the raw output before parsing it.
+
+        If the output is surrounded by triple backticks, remove them."""
+        output = output.strip()
+        if output.startswith("```"):
+            output = output[3:]
+            if output.startswith("json"):
+                output = output[4:]
+        if output.endswith("```"):
+            output = output[:-3]
+        return output
 
     def call(
         self,
         index: int,
-        prompt: str,
+        instructions: Optional[str],
+        prompt: Prompt,
         api: Callable,
         output: str = None,
     ) -> Tuple[str, Optional[Dict]]:
         """Run a step.
 
         1. Query the LLM API,
         2. Convert the response string to a dict,
         3. Log the output
         """
         with start_action(action_type="call", index=index, prompt=prompt) as action:
-            if prompt:
-                output = api(prompt)
+            if prompt and instructions:
+                output = api(prompt.source, instructions=instructions.source)
+            elif prompt:
+                output = api(prompt.source)
+
+            # Post-process the output before loading it as JSON.
+            output = self.post_process(output)
 
             error = None
             # Treat the output as a JSON string, and load it into a dict.
             try:
                 output_as_dict = json.loads(output, strict=False)
             except json.decoder.JSONDecodeError as e:
                 output_as_dict = None
@@ -241,23 +285,25 @@
                 reasks=[r.__dict__ for r in reasks],
             )
             return reasks
 
     def log(
         self,
         prompt: str,
+        instructions: Optional[str],
         output: str,
         output_as_dict: Dict,
         validated_output: Dict,
         reasks: list,
     ) -> None:
         """Log the step."""
         self.guard_history = self.guard_history.push(
             GuardLogs(
                 prompt=prompt,
+                instructions=instructions,
                 output=output,
                 output_as_dict=output_as_dict,
                 validated_output=validated_output,
                 reasks=reasks,
             )
         )
 
@@ -274,9 +320,10 @@
         output_schema: OutputSchema,
     ) -> Tuple[str, OutputSchema]:
         """Prepare to loop again."""
         prompt, output_schema = get_reask_prompt(
             parsed_rail=output_schema.root,
             reasks=reasks,
             reask_json=prune_json_for_reasking(validated_output),
+            reask_prompt_template=self.reask_prompt,
         )
         return prompt, OutputSchema(output_schema)
```

### Comparing `guardrails-ai-0.1.5/guardrails/schema.py` & `guardrails-ai-0.1.6/guardrails/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,16 +151,15 @@
             return getattr(self, "_validators")
         except AttributeError:
             raise AttributeError("Must call `get_validators` first.")
 
     @property
     def unregistered_validators(self) -> List[str]:
         """Get the list of validators from the format attribute that are not
-        registered for this element.
-        """
+        registered for this element."""
         try:
             return getattr(self, "_unregistered_validators")
         except AttributeError:
             raise AttributeError("Must call `get_validators` first.")
 
     def get_validators(self, strict: bool = False) -> List[Validator]:
         """Get the list of validators from the format attribute. Only the
@@ -291,14 +290,18 @@
     def __setstate__(self, state: Dict[str, Any]) -> None:
         self._schema = state["_schema"]
         self.root = state["root"]
 
     def items(self) -> Dict[str, DataType]:
         return vars(self._schema).items()
 
+    def to_dict(self) -> Dict[str, Any]:
+        """Convert the schema to a dictionary."""
+        return vars(self._schema)
+
     @property
     def parsed_rail(self) -> Optional[ET._Element]:
         return self.root
 
     def validate(
         self,
         data: Optional[Dict[str, Any]],
@@ -386,48 +389,48 @@
         for child in element:
             if isinstance(child, ET._Comment):
                 element.remove(child)
             else:
                 Schema2Prompt.remove_comments(child)
 
     @staticmethod
-    def validator_to_prompt(schema: Schema) -> None:
+    def validator_to_prompt(root: ET.Element, schema_dict: Dict[str, DataType]) -> None:
         """Recursively remove all validator arguments in the `format`
         attribute."""
 
         def _inner(dt: DataType, el: ET._Element):
             if "format" in el.attrib:
                 format = dt.format_attr.to_prompt()
                 if len(format):
                     el.attrib["format"] = format
                 else:
                     del el.attrib["format"]
 
             for _, dt_child, el_child in dt.iter(el):
                 _inner(dt_child, el_child)
 
-        for el_child in schema.root:
-            dt_child = schema[el_child.attrib["name"]]
+        for el_child in root:
+            dt_child = schema_dict[el_child.attrib["name"]]
             _inner(dt_child, el_child)
 
     @staticmethod
-    def pydantic_to_object(schema: Schema) -> None:
+    def pydantic_to_object(root: ET.Element, schema_dict: Dict[str, DataType]) -> None:
         """Recursively replace all pydantic elements with object elements."""
         from guardrails.datatypes import Pydantic
 
         def _inner(dt: DataType, el: ET._Element):
             if isinstance(dt, Pydantic):
                 new_el = dt.to_object_element()
                 el.getparent().replace(el, new_el)
 
             for _, dt_child, el_child in dt.iter(el):
                 _inner(dt_child, el_child)
 
-        for el_child in schema.root:
-            dt_child = schema[el_child.attrib["name"]]
+        for el_child in root:
+            dt_child = schema_dict[el_child.attrib["name"]]
             _inner(dt_child, el_child)
 
     @staticmethod
     def deconstruct_choice(root: ET._Element) -> ET._Element:
         """Deconstruct a choice element into a string and cases."""
 
         def _inner(el: str) -> ET._Element:
@@ -491,26 +494,27 @@
         Args:
             schema: The schema to transpile.
 
         Returns:
             The prompt.
         """
         # Construct another XML tree from the schema.
-        schema = deepcopy(schema)
+        root = deepcopy(schema.root)
+        schema_dict = schema.to_dict()
 
         # Remove comments.
-        cls.remove_comments(schema.root)
+        cls.remove_comments(root)
         # Remove action attributes.
-        cls.remove_on_fail_attributes(schema.root)
+        cls.remove_on_fail_attributes(root)
         # Remove validators with arguments.
-        cls.validator_to_prompt(schema)
+        cls.validator_to_prompt(root, schema_dict)
         # Replace pydantic elements with object elements.
-        cls.pydantic_to_object(schema)
+        cls.pydantic_to_object(root, schema_dict)
         # Deconstruct choice elements into string and cases.
-        updated_root = cls.deconstruct_choice(schema.root)
+        updated_root = cls.deconstruct_choice(root)
 
         # Return the XML as a string that is
         ET.indent(updated_root, space="    ")
         return ET.tostring(
             updated_root,
             encoding="unicode",
             method="xml",
```

### Comparing `guardrails-ai-0.1.5/guardrails/utils/constants.py` & `guardrails-ai-0.1.6/guardrails/utils/constants.py`

 * *Files identical despite different names*

### Comparing `guardrails-ai-0.1.5/guardrails/utils/docs_utils.py` & `guardrails-ai-0.1.6/guardrails/utils/docs_utils.py`

 * *Files identical despite different names*

### Comparing `guardrails-ai-0.1.5/guardrails/utils/logs_utils.py` & `guardrails-ai-0.1.6/guardrails/utils/logs_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,65 @@
 from copy import deepcopy
 from dataclasses import dataclass
-from typing import Any, Dict, List
+from typing import Any, Dict, List, Optional
 
 from rich.console import Group
 from rich.panel import Panel
 from rich.pretty import pretty_repr
 from rich.tree import Tree
 
+from guardrails.prompt import Prompt
 from guardrails.utils.reask_utils import ReAsk, gather_reasks, prune_json_for_reasking
 
 
 @dataclass
 class GuardLogs:
-    prompt: str
+    prompt: Prompt
+    instructions: Optional[str]
     output: str
     output_as_dict: dict
     validated_output: dict
     reasks: List[ReAsk]
 
     @property
     def failed_validations(self) -> List[ReAsk]:
         """Returns the failed validations."""
         return gather_reasks(self.validated_output)
 
     @property
     def rich_group(self) -> Group:
-        return Group(
-            Panel(
-                self.prompt,
-                title="Prompt",
-                style="on #F0F8FF",
-            ),
-            Panel(self.output, title="Raw LLM Output", style="on #F5F5DC"),
-            Panel(
-                pretty_repr(self.validated_output),
-                title="Validated Output",
-                style="on #F0FFF0",
-            ),
-        )
+        if self.instructions is not None:
+            return Group(
+                Panel(
+                    self.prompt.source if self.prompt else "No prompt",
+                    title="Prompt",
+                    style="on #F0F8FF",
+                ),
+                Panel(self.instructions, title="Instructions", style="on #FFF0F2"),
+                Panel(self.output, title="Raw LLM Output", style="on #F5F5DC"),
+                Panel(
+                    pretty_repr(self.validated_output),
+                    title="Validated Output",
+                    style="on #F0FFF0",
+                ),
+            )
+        else:
+            return Group(
+                Panel(
+                    self.prompt.source if self.prompt else "No prompt",
+                    title="Prompt",
+                    style="on #F0F8FF",
+                ),
+                Panel(self.output, title="Raw LLM Output", style="on #F5F5DC"),
+                Panel(
+                    pretty_repr(self.validated_output),
+                    title="Validated Output",
+                    style="on #F0FFF0",
+                ),
+            )
 
 
 @dataclass
 class GuardHistory:
     history: List[GuardLogs]
 
     def push(self, guard_log: GuardLogs) -> "GuardHistory":
```

### Comparing `guardrails-ai-0.1.5/guardrails/utils/misc.py` & `guardrails-ai-0.1.6/guardrails/utils/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def generate_test_artifacts(
     rail_spec: str, guard_history: GuardHistory, on_fail_type: str, artifact_dir: str
 ) -> None:
     """Generate artifacts for testing.
 
     Artifacts include: rail_spec, compiled_prompt, llm_output, validated_response.
     The artifacts are saved by on_fail_type. Check out
-    tests/integration_tests/test_cases/entity_extraction/ for examples.
+    tests/integration_tests/test_assets/entity_extraction/ for examples.
 
     This function is only intended to be used to create artifacts for integration tests
     once the GuardHistory object has been manually checked to be correct.
 
     Args:
         rail_spec: This should be a string representation of the rail.
         guard_history: The guard history object.
```

### Comparing `guardrails-ai-0.1.5/guardrails/utils/pydantic_utils.py` & `guardrails-ai-0.1.6/guardrails/utils/pydantic_utils.py`

 * *Files identical despite different names*

### Comparing `guardrails-ai-0.1.5/guardrails/utils/reask_utils.py` & `guardrails-ai-0.1.6/guardrails/utils/reask_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import json
 from collections import defaultdict
 from copy import deepcopy
 from dataclasses import dataclass
-from typing import Any, Dict, List, Tuple, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 from lxml import etree as ET
 
+from guardrails.prompt import Prompt
 from guardrails.utils.constants import constants
 
 
 @dataclass
 class ReAsk:
     incorrect_value: Any
     error_message: str
@@ -188,15 +189,16 @@
         return None
 
 
 def get_reask_prompt(
     parsed_rail: ET._Element,
     reasks: List[ReAsk],
     reask_json: Dict,
-) -> Tuple[str, ET._Element]:
+    reask_prompt_template: Optional[Prompt] = None,
+) -> Tuple[Prompt, ET._Element]:
     """Construct a prompt for reasking.
 
     Args:
         parsed_rail: The parsed RAIL.
         reasks: List of tuples, where each tuple contains the path to the
             reasked element, and the ReAsk object (which contains the error
             message describing why the reask is necessary).
@@ -213,23 +215,26 @@
     reask_elements = get_reasks_by_element(reasks, parsed_rail_copy)
 
     # Get the pruned JSON so that it only contains ReAsk objects
     # Get the pruned tree
     pruned_tree = get_pruned_tree(parsed_rail_copy, list(reask_elements.keys()))
     pruned_tree_string = OutputSchema(pruned_tree).transpile()
 
-    reask_prompt_template = (
-        constants["high_level_reask_prompt"] + constants["complete_json_suffix"]
-    )
+    if reask_prompt_template is None:
+        reask_prompt_template = Prompt(
+            constants["high_level_reask_prompt"] + constants["complete_json_suffix"]
+        )
 
     def reask_decoder(obj):
         return {k: v for k, v in obj.__dict__.items() if k not in ["path", "fix_value"]}
 
     reask_prompt = reask_prompt_template.format(
-        previous_response=json.dumps(reask_json, indent=2, default=reask_decoder),
+        previous_response=json.dumps(reask_json, indent=2, default=reask_decoder)
+        .replace("{", "{{")
+        .replace("}", "}}"),
         output_schema=pruned_tree_string,
     )
 
     return reask_prompt, pruned_tree
 
 
 def reask_json_as_dict(json: Dict) -> Dict:
@@ -255,15 +260,14 @@
 
     Args:
         value: Either a list, a dictionary, a ReAsk object or a scalar value.
 
     Returns:
         The value with ReAsk objects replaced with their fixed values.
     """
-
     if isinstance(value, list):
         for index, item in enumerate(value):
             value[index] = sub_reasks_with_fixed_values(item)
     elif isinstance(value, dict):
         for dict_key, dict_value in value.items():
             value[dict_key] = sub_reasks_with_fixed_values(dict_value)
     elif isinstance(value, ReAsk):
```

### Comparing `guardrails-ai-0.1.5/guardrails/validators.py` & `guardrails-ai-0.1.6/guardrails/validators.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 
 The name with which a validator is registered is the name that is used
 in the `RAIL` spec to specify formatters.
 """
 import ast
 import logging
 import os
+import re
 from collections import defaultdict
 from copy import deepcopy
 from dataclasses import dataclass
 from typing import Any, Callable, Dict, List, Optional, Type, Union
 
 import openai
 from pydantic import BaseModel, ValidationError
 
 from guardrails.datatypes import registry as types_registry
 from guardrails.utils.reask_utils import ReAsk
+from guardrails.utils.sql_utils import SQLDriver, create_sql_driver
 
 try:
     import numpy as np
 except ImportError:
     _HAS_NUMPY = False
 else:
     _HAS_NUMPY = True
@@ -71,15 +73,14 @@
 
     Args:
         schema: A dict that can contain lists, dicts or scalars.
 
     Returns:
         True if a Refrain object exists in the dict.
     """
-
     for key, value in schema.items():
         if isinstance(value, Refrain):
             return True
         elif isinstance(value, list):
             if check_refrain_in_list(value):
                 return True
         elif isinstance(value, dict):
@@ -94,15 +95,14 @@
 
     Args:
         schema: A list that can contain lists, dicts or scalars.
 
     Returns:
         A list with all Filter objects removed.
     """
-
     filtered_list = []
 
     for item in schema:
         if isinstance(item, Filter):
             pass
         elif isinstance(item, PydanticReAsk):
             filtered_list.append(item)
@@ -125,15 +125,14 @@
 
     Args:
         schema: A dictionary that can contain lists, dicts or scalars.
 
     Returns:
         A dictionary with all Filter objects removed.
     """
-
     filtered_dict = {}
 
     for key, value in schema.items():
         if isinstance(value, Filter):
             pass
         elif isinstance(value, PydanticReAsk):
             filtered_dict[key] = value
@@ -150,15 +149,14 @@
 
 
 def register_validator(name: str, data_type: Union[str, List[str]]):
     """Register a validator for a data type."""
 
     def decorator(cls: type):
         """Register a validator for a data type."""
-
         nonlocal data_type
         if isinstance(data_type, str):
             data_type = (
                 list(types_registry.keys()) if data_type == "all" else [data_type]
             )
         # Make sure that the data type string exists in the data types registry.
         for dt in data_type:
@@ -208,20 +206,18 @@
             logger.debug(
                 f"Validator {self.__class__.__name__} failed for {key} with error {e}."
             )
             return self.on_fail(e)
 
     def validate(self, key: str, value: Any, schema: Union[Dict, List]) -> Dict:
         """Validate a value."""
-
         raise NotImplementedError
 
     def fix(self, error: EventDetail) -> Dict:
         """Debug the incorrect value."""
-
         error.schema[error.key] = error.fix_value
         return error.schema
 
     def reask(self, error: EventDetail) -> Dict:
         """Reask disambiguates the validation failure into a helpful error
         message."""
 
@@ -230,47 +226,42 @@
             error_message=error.error_message,
             fix_value=error.fix_value,
         )
         return error.schema
 
     def filter(self, error: EventDetail) -> Dict:
         """If validation fails, filter the offending key from the schema."""
-
         logger.debug(f"Filtering {error.key} from schema...")
 
         error.schema[error.key] = Filter()
 
         return error.schema
 
     def refrain(self, error: EventDetail) -> Optional[Dict]:
         """If validation fails, refrain from answering."""
-
         logger.debug(f"Refusing to answer {error.key}...")
 
         error.schema[error.key] = Refrain()
         return error.schema
 
     def noop(self, error: EventDetail) -> Dict:
         """If validation fails, do nothing."""
-
         logger.debug(
             f"Validator {self.__class__.__name__} failed for {error.key}, "
             "but doing nothing..."
         )
 
         return error.schema
 
     def exception(self, error: EventDetail) -> None:
         """Raise an exception."""
-
         raise ValidatorError(error.error_message)
 
     def fix_reask(self, error: EventDetail) -> Dict:
         """If validation fails, fix the value and reask."""
-
         schema = self.fix(error)
 
         try:
             self.validate(error.key, error.fix_value, schema)
         except EventDetail as e:
             return self.reask(e)
 
@@ -282,15 +273,14 @@
 
         Args:
             with_keywords: Whether to include the keyword arguments in the prompt.
 
         Returns:
             A string representation of the validator.
         """
-
         if not len(self._kwargs):
             return self.rail_alias
 
         kwargs = self._kwargs.copy()
         for k, v in kwargs.items():
             if not isinstance(v, str):
                 kwargs[k] = str(v)
@@ -421,15 +411,14 @@
     ):
         super().__init__(on_fail=on_fail, choices=choices)
 
         self._choices = choices
 
     def validate(self, key: str, value: Any, schema: Union[Dict, List]) -> Dict:
         """Validate that a value is one of a set of choices."""
-
         logger.debug(f"Validating {value} is in {self._choices}...")
 
         if value not in self._choices:
             raise EventDetail(
                 key=key,
                 value=value,
                 schema=schema,
@@ -481,15 +470,14 @@
         super().__init__(on_fail=on_fail, min=min, max=max)
 
         self._min = min
         self._max = max
 
     def validate(self, key: str, value: Any, schema: Union[Dict, List]) -> Dict:
         """Validate that a value is within a range."""
-
         logger.debug(f"Validating {value} is in range {self._min} - {self._max}...")
 
         val_type = type(value)
 
         if self._min is not None and value < val_type(self._min):
             raise EventDetail(
                 key,
@@ -522,15 +510,14 @@
 
     def __init__(self, choices: List[Any], on_fail: Optional[Callable] = None):
         super().__init__(on_fail=on_fail, choices=choices)
         self._choices = choices
 
     def validate(self, key: str, value: Any, schema: Union[Dict, List]) -> Dict:
         """Validate that a value is within a range."""
-
         logger.debug(f"Validating {value} is in choices {self._choices}...")
 
         if value not in self._choices:
             raise EventDetail(
                 key,
                 value,
                 schema,
@@ -604,15 +591,14 @@
     ):
         super().__init__(on_fail=on_fail, min=min, max=max)
         self._min = int(min) if min is not None else None
         self._max = int(max) if max is not None else None
 
     def validate(self, key: str, value: Any, schema: Union[Dict, List]) -> Dict:
         """Validate that a value is within a range."""
-
         logger.debug(
             f"Validating {value} is in length range {self._min} - {self._max}..."
         )
 
         if self._min is not None and len(value) < self._min:
             logger.debug(f"Value {value} is less than {self._min}.")
 
@@ -773,25 +759,65 @@
     that uses a database connection to check if the query is valid.
 
     - Name for `format` attribute: `bug-free-sql`
     - Supported data types: `sql`
     - Programmatic fix: None
     """
 
+    def __init__(
+        self,
+        conn: Optional[str] = None,
+        schema_file: Optional[str] = None,
+        on_fail: Optional[Callable] = None,
+    ):
+        super().__init__(on_fail=on_fail)
+        self._driver: SQLDriver = create_sql_driver(schema_file=schema_file, conn=conn)
+
     def validate(self, key: str, value: Any, schema: Union[Dict, List]) -> Dict:
-        import sqlvalidator
+        errors = self._driver.validate_sql(value)
+        if len(errors) > 0:
+            raise EventDetail(
+                key,
+                value,
+                schema,
+                ". ".join(errors),
+                None,
+            )
+
+        return schema
+
+
+@register_validator(name="sql-column-presence", data_type="sql")
+class SqlColumnPresence(Validator):
+    """Validate that all columns in the SQL query are present in the schema.
+
+    - Name for `format` attribute: `sql-column-presence`
+    - Supported data types: `string`
+    """
+
+    def __init__(self, cols: List[str], on_fail: Optional[Callable] = None):
+        super().__init__(on_fail=on_fail, cols=cols)
+        self._cols = set(cols)
+
+    def validate(self, key: str, value: Any, schema: Union[Dict, List]) -> Dict:
+        from sqlglot import exp, parse
 
-        sql_query = sqlvalidator.parse(value)
+        expressions = parse(value)
+        cols = set()
+        for expression in expressions:
+            for col in expression.find_all(exp.Column):
+                cols.add(col.alias_or_name)
 
-        if not sql_query.is_valid():
+        diff = cols.difference(self._cols)
+        if len(diff) > 0:
             raise EventDetail(
                 key,
                 value,
                 schema,
-                ". ".join(sql_query.errors),
+                f"Columns [{', '.join(diff)}] not in [{', '.join(self._cols)}]",
                 None,
             )
 
         return schema
 
 
 @register_validator(name="similar-to-document", data_type="string")
@@ -966,7 +992,154 @@
                 value,
                 schema,
                 f"{value} must end with {self._end}",
                 value + [self._end],
             )
 
         return schema
+
+
+@register_validator(name="extracted-summary-sentences-match", data_type="string")
+class ExtractedSummarySentencesMatch(Validator):
+    def __init__(
+        self,
+        documents_dir: str,
+        threshold: float = 0.7,
+        embedding_model: Optional["EmbeddingBase"] = None,  # noqa: F821
+        vector_db: Optional["VectorDBBase"] = None,  # noqa: F821
+        document_store: Optional["DocumentStoreBase"] = None,  # noqa: F821
+        on_fail: Optional[Callable] = None,
+        **kwargs,
+    ):
+        super().__init__(on_fail, **kwargs)
+        # TODO(shreya): Pass embedding_model, vector_db, document_store from spec
+
+        if document_store is None:
+            from guardrails.document_store import EphemeralDocumentStore
+
+            if vector_db is None:
+                from guardrails.vectordb import Faiss
+
+                if embedding_model is None:
+                    from guardrails.embedding import OpenAIEmbedding
+
+                    embedding_model = OpenAIEmbedding()
+
+                vector_db = Faiss.new_flat_ip_index(
+                    embedding_model.output_dim, embedder=embedding_model
+                )
+            self.store = EphemeralDocumentStore(vector_db)
+        else:
+            self.store = document_store
+
+        for doc_path in os.listdir(documents_dir):
+            with open(os.path.join(documents_dir, doc_path)) as f:
+                doc = f.read()
+                self.store.add_text(
+                    doc, {"path": os.path.join(documents_dir, doc_path)}
+                )
+
+        self._threshold = float(threshold)
+
+    def validate(self, key, value, schema) -> Dict:
+        # Split the value into sentences.
+        sentences = re.split(r"(?<=[.!?]) +", value)
+
+        # Check if any of the sentences in the value match any of the sentences
+        # in the documents.
+        unverified = []
+        count = 0
+        new_value = ""
+        citations = ""
+        for i, sentence in enumerate(sentences):
+            page = self.store.search_with_threshold(sentence, self._threshold)
+            if not page:
+                unverified.append(i)
+            else:
+                citations += f"\n[{count+1}] {page[0].metadata['path']}"
+                new_value += sentence + f" [{count+1}] "
+                count += 1
+
+        fixed_summary = new_value + citations
+
+        if unverified:
+            unverified_sentences = "\n".join(
+                "- " + s for i, s in enumerate(sentences) if i in unverified
+            )
+            raise EventDetail(
+                key,
+                value,
+                schema,
+                (
+                    f"The summary \nSummary: {value}\n has sentences\n"
+                    f"{unverified_sentences}\n that are not similar to any document."
+                ),
+                fixed_summary,
+            )
+
+        schema[key] = fixed_summary
+        return schema
+
+    def to_prompt(self, with_keywords: bool = True) -> str:
+        return ""
+
+
+@register_validator(name="qa-relevance-llm-eval", data_type="string")
+class QARelevanceLLMEval(Validator):
+    def __init__(
+        self,
+        llm_callable: Callable = None,
+        on_fail: Optional[Callable] = None,
+        **kwargs,
+    ):
+        super().__init__(on_fail, **kwargs)
+        self.llm_callable = (
+            llm_callable if llm_callable else openai.ChatCompletion.create
+        )
+
+    def selfeval(self, question: str, answer: str):
+        from guardrails import Guard
+
+        spec = """
+<rail version="0.1">
+<output>
+    <bool name="relevant" />
+</output>
+
+<prompt>
+Is the answer below relevant to the question asked?
+Question: {question}
+Answer: {answer}
+
+Relevant (as a JSON with a single boolean key, "relevant"):\
+</prompt>
+</rail>
+    """.format(
+            question=question,
+            answer=answer,
+        )
+        guard = Guard.from_rail_string(spec)
+
+        return guard(
+            self.llm_callable,
+            max_tokens=10,
+            temperature=0.1,
+        )[1]
+
+    def validate(self, key, value, schema) -> Dict:
+        assert "question" in schema, "The schema must contain a `question` key."
+
+        relevant = self.selfeval(schema["question"], value)["relevant"]
+        if relevant:
+            return schema
+
+        fixed_answer = "No relevant answer found."
+        raise EventDetail(
+            key,
+            value,
+            schema,
+            f"The answer {value} is not relevant to the question {schema['question']}.",
+            fixed_answer,
+        )
+
+    def to_prompt(self, with_keywords: bool = True) -> str:
+        return ""
```

### Comparing `guardrails-ai-0.1.5/guardrails_ai.egg-info/PKG-INFO` & `guardrails-ai-0.1.6/guardrails_ai.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: guardrails-ai
-Version: 0.1.5
+Version: 0.1.6
 Summary: Adding guardrails to large language models.
 Home-page: https://github.com/shreyar/guardrails
 Author: Shreya Rajpal
 Author-email: shreya.rajpal@gmail.com
 License: Apache 2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: sql
+Provides-Extra: manifest
+Provides-Extra: vectordb
 Provides-Extra: profanity
 Provides-Extra: critique
 License-File: LICENSE
 
 
 # 🛤️ Guardrails
 
@@ -39,15 +41,15 @@
 - does pydantic-style validation of LLM outputs (including semantic validation such as checking for bias in generated text, checking for bugs in generated code, etc.)
 - takes corrective actions (e.g. reasking LLM) when validation fails,
 - enforces structure and type guarantees (e.g. JSON).
 
 
 ## 🚒 Under the hood
 
-Guardrails provides a format (`.rail`) for enforcing a specification on an LLM output, and a lightweight wrapper around LLM API calls to implement this spec.
+Guardrails provides a file format (`.rail`) for enforcing a specification on an LLM output, and a lightweight wrapper around LLM API calls to implement this spec.
 
 1. `rail` (**R**eliable **AI** markup **L**anguage) files for specifying structure and type information, validators and corrective actions over LLM outputs.
 2. `gd.Guard` wraps around LLM API calls to structure, validate and correct the outputs.
 
 ``` mermaid
 graph LR
     A[Create `RAIL` spec] --> B["Initialize `guard` from spec"];
@@ -86,21 +88,21 @@
 - [ ] Improving reasking logic
 - [ ] A guardrails.js implementation
 - [ ] VSCode extension for `.rail` files
 - [ ] Next version of `.rail` format
 - [ ] Add more LLM providers
 
 ## 🚀 Getting Started
-Let's go through an example where we ask an LLM to explain what a "bank run" is in a tweet, and generate URL links to relevant news articles. We'll generate a `.rail` spec for this and then use Guardrails to enforce it. You can see more examples in the docs.
+Let's go through an example where we ask an LLM to explain what a "bank run" is in a tweet, and generate URLs to relevant news articles. We'll generate a `.rail` spec for this and then use Guardrails to enforce it. You can see more examples in the docs.
 
 ### 📝 Creating a `RAIL` spec
 
 We create a `RAIL` spec to describe the expected structure and types of the LLM output, the quality criteria for the output to be considered valid, and corrective actions to be taken if the output is invalid.
 
-Specifically, we use `RAIL` to
+Using `RAIL`, we:
 - Request the LLM to generate an object with two fields: `explanation` and `follow_up_url`.
 - For the `explanation` field, ensure the max length of the generated string should be between 200 and 280 characters.
   - If the explanation is not of valid length, `reask` the LLM.
 - For the `follow_up_url` field, the URL should be reachable.
   - If the URL is not reachable, we will `filter` it out of the response.
 
 
@@ -160,14 +162,16 @@
     <object name="bank_run" format="length: 2">
         <string name="explanation" description="A paragraph about what a bank run is." format="length: 200 280" on-fail-length="reask" />
         <url name="follow_up_url" description="A web URL where I can read more about bank runs." required="true" format="valid-url" on-fail-valid-url="filter" />
     </object>
 </output>
 
 ONLY return a valid JSON object (no other text is necessary). The JSON MUST conform to the XML format, including any types and format requests e.g. requests for lists, objects and specific types. Be correct and concise.
+
+JSON Output:
 ```
 
 Call the `Guard` object with the LLM API call as the first argument and add any additional arguments to the LLM API call as the remaining arguments.
 
 
 ```python
 import openai
@@ -187,7 +191,11 @@
     'bank_run': {
         'explanation': 'A bank run is when a large number of people withdraw their deposits from a bank due to concerns about its solvency. This can cause a financial crisis if the bank is unable to meet the demand for withdrawals.',
         'follow_up_url': 'https://www.investopedia.com/terms/b/bankrun.asp'
     }
 }
 
 ```
+
+## 🛠️ Contributing
+
+Get started by checking out Github issues and of course using Guardrails to familiarize yourself with the project. Guardrails is still actively under development and any support is gladly welcomed. Feel free to open an issue, or reach out if you would like to add to the project!
```

### Comparing `guardrails-ai-0.1.5/setup.py` & `guardrails-ai-0.1.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,36 +30,46 @@
 REQUIRED = [
     "lxml",
     "openai",
     "rich",
     "eliot",
     "eliot-tree",
     "pydantic",
+    "typer",
+    "griffe",
+    "tenacity",
 ]
 
 # Read in docs/requirements.txt
 with open("docs/requirements.txt") as f:
     DOCS_REQUIREMENTS = f.read().splitlines()
 
+SQL_REQUIREMENTS = ["sqlvalidator", "sqlalchemy>=2.0.9", "sqlglot"]
+
+VECTORDB_REQUIREMENTS = ["faiss-cpu", "numpy", "tiktoken"]
 
 # What packages are optional?
 EXTRAS = {
     "dev": [
         "black==22.12.0",
         "isort>=5.12.0",
         "flake8>=3.8.4",
         "docformatter>=1.4",
         "pytest-cov>=2.10.1",
         "pre-commit>=2.9.3",
         "twine",
         "pytest-mock",
         "pypdfium2",
+        *SQL_REQUIREMENTS,
+        *VECTORDB_REQUIREMENTS,
     ]
     + DOCS_REQUIREMENTS,
-    "sql": ["sqlvalidator"],
+    "sql": SQL_REQUIREMENTS,
+    "manifest": "manifest-ml",
+    "vectordb": VECTORDB_REQUIREMENTS,
     "profanity": ["alt-profanity-check"],
     "critique": ["inspiredco"],
 }
 
 # The rest you shouldn't have to touch too much :)
 # ------------------------------------------------
 # Except, perhaps the License and Trove Classifiers!
@@ -127,14 +137,18 @@
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
     packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
     # If your package is a single module, use this instead of 'packages':
     # py_modules=['mypackage'],
+    # Add CLI for "guardrails" command, point to guardrails.cli:cli
+    entry_points={
+        "console_scripts": ["guardrails=guardrails.cli:cli"],
+    },
     install_requires=REQUIRED,
     include_package_data=True,
     extras_require=EXTRAS,
     license="Apache 2.0",
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
```


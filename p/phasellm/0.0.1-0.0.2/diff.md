# Comparing `tmp/phasellm-0.0.1.tar.gz` & `tmp/phasellm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phasellm-0.0.1.tar", last modified: Sat Apr 15 22:03:29 2023, max compression
+gzip compressed data, was "phasellm-0.0.2.tar", last modified: Mon Apr 24 16:34:50 2023, max compression
```

## Comparing `phasellm-0.0.1.tar` & `phasellm-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-04-15 22:03:29.894817 phasellm-0.0.1/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1083 2023-04-15 22:03:12.000000 phasellm-0.0.1/LICENSE
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      716 2023-04-15 22:03:29.894817 phasellm-0.0.1/PKG-INFO
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-04-15 22:03:29.894817 phasellm-0.0.1/phasellm/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2023-04-15 22:03:12.000000 phasellm-0.0.1/phasellm/__init__.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-04-15 22:03:29.894817 phasellm-0.0.1/phasellm/eval/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       19 2023-04-15 22:03:12.000000 phasellm-0.0.1/phasellm/eval/__init__.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     3500 2023-04-15 22:03:12.000000 phasellm-0.0.1/phasellm/eval/eval.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-04-15 22:03:29.894817 phasellm-0.0.1/phasellm/llms/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       21 2023-04-15 22:03:12.000000 phasellm-0.0.1/phasellm/llms/__init__.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    12046 2023-04-15 22:03:12.000000 phasellm-0.0.1/phasellm/llms/llms.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-04-15 22:03:29.894817 phasellm-0.0.1/phasellm.egg-info/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      716 2023-04-15 22:03:29.000000 phasellm-0.0.1/phasellm.egg-info/PKG-INFO
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      261 2023-04-15 22:03:29.000000 phasellm-0.0.1/phasellm.egg-info/SOURCES.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2023-04-15 22:03:29.000000 phasellm-0.0.1/phasellm.egg-info/dependency_links.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        9 2023-04-15 22:03:29.000000 phasellm-0.0.1/phasellm.egg-info/top_level.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       38 2023-04-15 22:03:29.894817 phasellm-0.0.1/setup.cfg
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1109 2023-04-15 22:03:12.000000 phasellm-0.0.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-24 16:34:50.928490 phasellm-0.0.2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1083 2023-04-24 16:33:56.000000 phasellm-0.0.2/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      739 2023-04-24 16:34:50.928490 phasellm-0.0.2/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4632 2023-04-24 16:33:56.000000 phasellm-0.0.2/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-24 16:34:50.928490 phasellm-0.0.2/phasellm/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-24 16:33:56.000000 phasellm-0.0.2/phasellm/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-24 16:34:50.928490 phasellm-0.0.2/phasellm/eval/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       19 2023-04-24 16:33:56.000000 phasellm-0.0.2/phasellm/eval/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3500 2023-04-24 16:33:56.000000 phasellm-0.0.2/phasellm/eval/eval.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-24 16:34:50.928490 phasellm-0.0.2/phasellm/llms/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-04-24 16:33:56.000000 phasellm-0.0.2/phasellm/llms/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13783 2023-04-24 16:33:56.000000 phasellm-0.0.2/phasellm/llms/llms.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-24 16:34:50.928490 phasellm-0.0.2/phasellm.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      739 2023-04-24 16:34:50.000000 phasellm-0.0.2/phasellm.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-04-24 16:34:50.000000 phasellm-0.0.2/phasellm.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-24 16:34:50.000000 phasellm-0.0.2/phasellm.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      112 2023-04-24 16:34:50.000000 phasellm-0.0.2/phasellm.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-04-24 16:34:50.000000 phasellm-0.0.2/phasellm.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-24 16:34:50.928490 phasellm-0.0.2/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1142 2023-04-24 16:34:41.000000 phasellm-0.0.2/setup.py
```

### Comparing `phasellm-0.0.1/LICENSE` & `phasellm-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `phasellm-0.0.1/PKG-INFO` & `phasellm-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: phasellm
-Version: 0.0.1
+Version: 0.0.2
 Summary: Wrappers for common large langugae models (LLMs) with support for evaluation.
 Home-page: UNKNOWN
 Author: Wojciech Gryc
 Author-email: hello@phaseai.com
 License: MIT
 Keywords: llm,nlp,evaluation,ai
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
 License-File: LICENSE
 
 PhaseLLM provides wrappers for common large language models and use cases. This makes it easy to swap models in and out as needed. We also provide support for evaluation of models so you can choose which models are better to use.
```

### Comparing `phasellm-0.0.1/phasellm/eval/eval.py` & `phasellm-0.0.2/phasellm/eval/eval.py`

 * *Files identical despite different names*

### Comparing `phasellm-0.0.1/phasellm/llms/llms.py` & `phasellm-0.0.2/phasellm/llms/llms.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,29 +89,76 @@
         new_prompt = self.prompt
         for m in matches:
             keyword = m.replace("{", "").replace("}", "").strip()
             if keyword in kwargs:
                 new_prompt = new_prompt.replace(m, kwargs[keyword])
         return new_prompt
 
+class BloomWrapper():
+    """
+    Wrapper for Hugging Face's BLOOM model. Requires access to Hugging Face's inference API.
+    """
+    def __init__(self, apikey):
+        self.apikey = apikey
+
+    def __repr__(self):
+        return f"BloomWrapper()"
+
+    def complete_chat(self, messages, append_role=None):
+        """
+        Mimicks a chat scenario with BLOOM, via a list of {"role": <str>, "content":<str>} objects.
+        """
+
+        prompt_preamble = "You are a friendly chat assistant. You are speaking to the 'user' below and will respond at the end, where it says 'assistant'.\n"
+        prompt_text = prompt_preamble + _clean_messages_to_prompt(messages)
+        if append_role is not None and len(append_role) > 0:
+            prompt_text += f"\n{append_role}:"
+
+        API_URL = "https://api-inference.huggingface.co/models/bigscience/bloom"
+        headers = {"Authorization": f"Bearer {self.apikey}"}
+
+        response = requests.post(API_URL, headers=headers, json={"inputs": prompt_text}).json()
+
+        all_text = response[0]['generated_text']
+        new_text = all_text[len(prompt_text):]
+
+        # We only return the first line of text.
+        newline_location = new_text.find("\n") 
+        if newline_location > 0:
+            new_text = new_text[:newline_location]
+
+        return new_text
+
+    def text_completion(self, prompt):
+        """
+        Completes text via BLOOM (Hugging Face).
+        """
+        API_URL = "https://api-inference.huggingface.co/models/bigscience/bloom"
+        headers = {"Authorization": f"Bearer {self.apikey}"}
+
+        response = requests.post(API_URL, headers=headers, json={"inputs": prompt}).json()
+        all_text = response[0]['generated_text']
+        new_text = all_text[len(prompt):]
+        return new_text
+
 class OpenAIGPTWrapper():
     """
     Wrapper for the OpenAI API. Supports all major text and chat completion models by OpenAI.
     """
 
     def __init__(self, apikey, model="gpt-3.5-turbo"):
         openai.api_key = apikey
         self.model = model
 
     def __repr__(self):
         return f"OpenAIGPTWrapper(model={self.model})"
     
     def complete_chat(self, messages, append_role=None):
         """
-        Completes chat with OpenAI. If using GPT 3.5 or 4, will simply send the list of {"role": <str>, "content":<str>} objects ot the API.
+        Completes chat with OpenAI. If using GPT 3.5 or 4, will simply send the list of {"role": <str>, "content":<str>} objects to the API.
 
         If using an older model, it will structure the messages list into a prompt first.
         """
 
         if self.model.find('gpt-4') >= 0 or self.model.find('gpt-3.5') >= 0:
 
             response = openai.ChatCompletion.create(
@@ -198,15 +245,14 @@
         """
         Completes text based on provided prompt.
         """
 
         r_headers = {"X-API-Key":self.apikey, "Accept":"application/json"}
         r_data = {"prompt": prompt,
                   "model": self.model,
-                  "max_tokens_to_sample": 300, 
                   "stop_sequences": stop_sequences
                 }
 
         resp = requests.post("https://api.anthropic.com/v1/complete", headers=r_headers, json=r_data)
         completion = json.loads(resp.text)["completion"].strip()
         return completion
 
@@ -353,12 +399,12 @@
         """
         self.messages.append({"role":role, "content":message})
 
     def chat(self, message):
         """
         Chats with the chatbot.
         """
-        self.append_message('user', message)
+        self._append_message('user', message)
         response = self.llm.complete_chat(self.messages, "assistant")
-        self.append_message('assistant', response)
+        self._append_message('assistant', response)
         return response
-    
+
```

### Comparing `phasellm-0.0.1/phasellm.egg-info/PKG-INFO` & `phasellm-0.0.2/phasellm.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: phasellm
-Version: 0.0.1
+Version: 0.0.2
 Summary: Wrappers for common large langugae models (LLMs) with support for evaluation.
 Home-page: UNKNOWN
 Author: Wojciech Gryc
 Author-email: hello@phaseai.com
 License: MIT
 Keywords: llm,nlp,evaluation,ai
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
 License-File: LICENSE
 
 PhaseLLM provides wrappers for common large language models and use cases. This makes it easy to swap models in and out as needed. We also provide support for evaluation of models so you can choose which models are better to use.
```


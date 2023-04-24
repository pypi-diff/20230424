# Comparing `tmp/thinkgpt-0.0.3.tar.gz` & `tmp/thinkgpt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thinkgpt-0.0.3.tar", max compression
+gzip compressed data, was "thinkgpt-0.0.4.tar", max compression
```

## Comparing `thinkgpt-0.0.3.tar` & `thinkgpt-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-04-14 15:21:33.490604 thinkgpt-0.0.3/LICENSE
--rw-r--r--   0        0        0     6871 2023-04-20 23:12:15.079797 thinkgpt-0.0.3/README.md
--rw-r--r--   0        0        0      562 2023-04-23 02:11:49.925649 thinkgpt-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-14 15:28:05.934649 thinkgpt-0.0.3/thinkgpt/__init__.py
--rw-r--r--   0        0        0     4157 2023-04-16 20:58:23.227617 thinkgpt-0.0.3/thinkgpt/abstract.py
--rw-r--r--   0        0        0     2223 2023-04-15 22:14:39.262945 thinkgpt-0.0.3/thinkgpt/condition.py
--rw-r--r--   0        0        0     3061 2023-04-20 23:52:42.818016 thinkgpt-0.0.3/thinkgpt/gpt_select.py
--rw-r--r--   0        0        0     1165 2023-04-16 03:45:24.127522 thinkgpt-0.0.3/thinkgpt/helper.py
--rw-r--r--   0        0        0     2812 2023-04-16 20:58:23.231671 thinkgpt-0.0.3/thinkgpt/infer.py
--rw-r--r--   0        0        0     4410 2023-04-21 00:39:21.276973 thinkgpt-0.0.3/thinkgpt/llm.py
--rw-r--r--   0        0        0     2509 2023-04-21 00:50:43.413297 thinkgpt-0.0.3/thinkgpt/memory.py
--rw-r--r--   0        0        0     1854 2023-04-15 15:38:08.801502 thinkgpt-0.0.3/thinkgpt/refine.py
--rw-r--r--   0        0        0     3037 2023-04-23 02:20:34.442965 thinkgpt-0.0.3/thinkgpt/summarize.py
--rw-r--r--   0        0        0     7772 1970-01-01 00:00:00.000000 thinkgpt-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-14 15:21:33.490604 thinkgpt-0.0.4/LICENSE
+-rw-r--r--   0        0        0     6871 2023-04-20 23:12:15.079797 thinkgpt-0.0.4/README.md
+-rw-r--r--   0        0        0      562 2023-04-24 01:10:43.645079 thinkgpt-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-14 15:28:05.934649 thinkgpt-0.0.4/thinkgpt/__init__.py
+-rw-r--r--   0        0        0     4067 2023-04-24 00:39:46.959405 thinkgpt-0.0.4/thinkgpt/abstract.py
+-rw-r--r--   0        0        0     2349 2023-04-24 00:39:46.956963 thinkgpt-0.0.4/thinkgpt/condition.py
+-rw-r--r--   0        0        0     3668 2023-04-24 00:41:27.830853 thinkgpt-0.0.4/thinkgpt/gpt_select.py
+-rw-r--r--   0        0        0     1165 2023-04-16 03:45:24.127522 thinkgpt-0.0.4/thinkgpt/helper.py
+-rw-r--r--   0        0        0     2938 2023-04-24 00:43:29.599263 thinkgpt-0.0.4/thinkgpt/infer.py
+-rw-r--r--   0        0        0     4453 2023-04-24 01:05:55.882845 thinkgpt-0.0.4/thinkgpt/llm.py
+-rw-r--r--   0        0        0     2602 2023-04-24 00:49:11.780601 thinkgpt-0.0.4/thinkgpt/memory.py
+-rw-r--r--   0        0        0     1742 2023-04-24 00:46:00.737818 thinkgpt-0.0.4/thinkgpt/refine.py
+-rw-r--r--   0        0        0     3049 2023-04-24 00:46:00.734818 thinkgpt-0.0.4/thinkgpt/summarize.py
+-rw-r--r--   0        0        0     7772 1970-01-01 00:00:00.000000 thinkgpt-0.0.4/PKG-INFO
```

### Comparing `thinkgpt-0.0.3/LICENSE` & `thinkgpt-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `thinkgpt-0.0.3/README.md` & `thinkgpt-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `thinkgpt-0.0.3/pyproject.toml` & `thinkgpt-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "thinkgpt"
-version = "0.0.3"
+version = "0.0.4"
 description = "ThinkGPT is a Python library aimed at implementing Chain of Thoughts for Large Language Models (LLMs), prompting the model to think, reason, and to create generative agents."
 authors = ["Alaeddine Abdessalem <alaeddine-13@live.fr>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
```

### Comparing `thinkgpt-0.0.3/thinkgpt/abstract.py` & `thinkgpt-0.0.4/thinkgpt/abstract.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import re
 import warnings
 from typing import Dict, List, Any
 
 import numpy as np
 from langchain import PromptTemplate, LLMChain
 from langchain.schema import LLMResult, BaseOutputParser, Generation
-from langchain.llms import OpenAI, BaseLLM, OpenAIChat
+from langchain.llms import BaseLLM, OpenAI
+from langchain.chat_models import ChatOpenAI
 from langchain.embeddings import OpenAIEmbeddings
 from langchain.prompts.few_shot import FewShotPromptTemplate
 from docarray import Document, DocumentArray
 
 from thinkgpt.helper import LineSeparatorOutputParser
 
 examples = [
@@ -78,21 +79,19 @@
         if match:
             return {'action': 'REMEMBER', 'value': match.group(1)}
         else:
             return {'action': 'FINISH', 'value': text.strip()}
 
 class AbstractChain(LLMChain):
     """Prompts the LLM to request to remember memory as needed"""
+    def __init__(self, **kwargs):
+        super().__init__(prompt=ABSTRACTION_PROMPT, **kwargs)
 
     @classmethod
     def from_llm(cls, llm: BaseLLM, verbose: bool = True) -> LLMChain:
-        if not (hasattr(llm, 'model_name') and llm.model_name == 'gpt-4'):
-            warnings.warn(
-                "Keep in mind that LLMs except 'gpt-4' do not exhibit as good abstraction abilities as gpt-4"
-            )
         return cls(prompt=ABSTRACTION_PROMPT, llm=llm, verbose=verbose)
 
     def predict(self, instruction_hint: str = '', **kwargs: Any) -> str:
         return super().predict(instruction_hint=instruction_hint, **kwargs)
 
 
 class AbstractMixin:
@@ -102,13 +101,13 @@
         result = self.abstract_chain.predict(
             observations="\n".join(observations), instruction_hint=instruction_hint
         )
         return LineSeparatorOutputParser().parse(result)
 
 
 if __name__ == '__main__':
-    chain = AbstractChain.from_llm(OpenAI(model_name="gpt-4"))
+    chain = AbstractChain(llm=ChatOpenAI(model_name="gpt-3.5-turbo"))
     print(chain.predict(observations="\n".join([
         "in tunisian, I did not eat is \"ma khditech\"",
         "I did not work is \"ma khdemtech\"",
         "I did not go is \"ma mchitech\"",
     ]), instruction_hint="output the rule in french"))
```

### Comparing `thinkgpt-0.0.3/thinkgpt/condition.py` & `thinkgpt-0.0.4/thinkgpt/condition.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Dict, List, Any, Union
 
 from langchain import PromptTemplate, LLMChain
 from langchain.schema import LLMResult, BaseOutputParser, Generation
-from langchain.llms import OpenAI, BaseLLM, OpenAIChat
+from langchain.llms import OpenAI, BaseLLM
 from langchain.prompts.few_shot import FewShotPromptTemplate
+from langchain.chat_models import ChatOpenAI
 
 CONDITION_EXAMPLES = [
     {
         "question": "Is the sky blue?",
         "answer": "True"
     },
     {
@@ -47,14 +48,16 @@
         elif text == "false":
             return False
         else:
             return "Wrong format of the answer"
 
 
 class ConditionChain(LLMChain):
+    def __init__(self, **kwargs):
+        super().__init__(prompt=CONDITION_PROMPT, **kwargs)
 
     @classmethod
     def from_llm(cls, llm: BaseLLM, verbose: bool = True) -> LLMChain:
         return cls(prompt=CONDITION_PROMPT, llm=llm, verbose=verbose)
 
     def predict(self, question: str, instruction_hint: str = '', **kwargs: Any) -> bool:
         result = super().predict(question=question, instruction_hint=instruction_hint, **kwargs)
@@ -65,9 +68,9 @@
     condition_chain: ConditionChain
 
     def condition(self, question: str, instruction_hint: str = '') -> bool:
         return self.condition_chain.predict(question=question, instruction_hint=instruction_hint)
 
 
 if __name__ == '__main__':
-    chain = ConditionChain.from_llm(OpenAI(model_name="gpt-3.5-turbo"))
+    chain = ConditionChain(llm=ChatOpenAI(model_name="gpt-3.5-turbo"))
     print(chain.predict(question="Is 2+2 equal to 4?", instruction_hint=""))
```

### Comparing `thinkgpt-0.0.3/thinkgpt/gpt_select.py` & `thinkgpt-0.0.4/thinkgpt/gpt_select.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Dict, List, Any, Union, Optional
 
 from langchain import PromptTemplate, LLMChain
 from langchain.schema import LLMResult, BaseOutputParser, Generation
-from langchain.llms import OpenAI, BaseLLM, OpenAIChat
+from langchain.llms import OpenAI, BaseLLM
 from langchain.prompts.few_shot import FewShotPromptTemplate
+from langchain.chat_models import ChatOpenAI
 
 SELECT_EXAMPLES = [
     {
         "question": "Which animal is known as the king of the jungle?",
         "options_text": '\n'.join(["Lion", "Elephant", "Tiger", "Giraffe"]),
         "answer": "Lion"
     },
@@ -48,14 +49,23 @@
     def parse(self, text: str) -> Optional[str]:
         if text.strip().lower() not in [option.lower() for option in self.options]:
             return None
         return text.strip()
 
 
 class SelectChain(LLMChain):
+    def __init__(self, select_examples: Optional[List] = None, **kwargs):
+        SELECT_PROMPT = FewShotPromptTemplate(
+            prefix="Choose the correct answer for the following question from the provided options.",
+            examples=select_examples or SELECT_EXAMPLES,
+            example_prompt=SELECT_EXAMPLE_PROMPT,
+            suffix="{instruction_hint}\nQuestion:\n{question}\nOptions:\n{options_text}\nAnswer:\n",
+            input_variables=["instruction_hint", "question", "options_text"]
+        )
+        super().__init__(prompt=SELECT_PROMPT, **kwargs)
 
     @classmethod
     def from_llm(cls, llm: BaseLLM, select_examples: Optional[List] = None, verbose: bool = True) -> LLMChain:
         SELECT_PROMPT = FewShotPromptTemplate(
             prefix="Choose the correct answer for the following question from the provided options.",
             examples=select_examples or SELECT_EXAMPLES,
             example_prompt=SELECT_EXAMPLE_PROMPT,
@@ -76,10 +86,10 @@
 
     def select(self, question: str, options: List[str], instruction_hint: str = '', select_chain: Optional[SelectChain] = None) -> str:
        chain = select_chain or self.select_chain
        return chain.predict(question=question, options=options, instruction_hint=instruction_hint)
 
 
 if __name__ == '__main__':
-    chain = SelectChain.from_llm(OpenAI(model_name="gpt-3.5-turbo"))
+    chain = SelectChain(llm=ChatOpenAI(model_name="gpt-3.5-turbo"))
     print(chain.predict(question="Which animal is known as the king of the jungle?",
                         options=["Lion", "Elephant", "Tiger", "Giraffe"], instruction_hint=""))
```

### Comparing `thinkgpt-0.0.3/thinkgpt/helper.py` & `thinkgpt-0.0.4/thinkgpt/helper.py`

 * *Files identical despite different names*

### Comparing `thinkgpt-0.0.3/thinkgpt/infer.py` & `thinkgpt-0.0.4/thinkgpt/infer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import warnings
 from typing import Dict, List, Any
 
 from langchain import PromptTemplate, LLMChain
-from langchain.llms import OpenAI, BaseLLM, OpenAIChat
+from langchain.llms import OpenAI, BaseLLM
 from langchain.prompts.few_shot import FewShotPromptTemplate
+from langchain.chat_models import ChatOpenAI
 
 from thinkgpt.helper import LineSeparatorOutputParser
 
 INFERENCE_EXAMPLE_PROMPT = PromptTemplate(template="""
 Facts:
 {facts}
 
@@ -46,14 +47,16 @@
     suffix="Facts:\n{facts}\nNew Observations:",
     input_variables=["instruction_hint", "facts"]
 )
 
 
 class InferChain(LLMChain):
     """Prompts the LLM to generate new observations based on the given facts"""
+    def __init__(self, **kwargs):
+        super().__init__(prompt=INFERENCE_PROMPT, **kwargs)
 
     @classmethod
     def from_llm(cls, llm: BaseLLM, verbose: bool = True) -> LLMChain:
         return cls(prompt=INFERENCE_PROMPT, llm=llm, verbose=verbose)
 
     def predict(self, instruction_hint: str = '', **kwargs: Any) -> str:
         return super().predict(instruction_hint=instruction_hint, **kwargs)
@@ -66,14 +69,14 @@
         result = self.infer_chain.predict(
             facts="\n".join(facts), instruction_hint=instruction_hint
         )
         return LineSeparatorOutputParser().parse(result)
 
 
 if __name__ == '__main__':
-    chain = InferChain.from_llm(OpenAI(model_name="gpt-3.5-turbo"))
+    chain = InferChain(llm=ChatOpenAI(model_name="gpt-3.5-turbo"))
     # examples from the paper https://arxiv.org/abs/2304.03442
     print(chain.predict(facts="\n".join([
         "Klaus Mueller is writing a research paper",
         "Klaus Mueller enjoys reading a book on gentrification",
         "Klaus Mueller is conversing with Ayesha Khan about exercising"
     ])))
```

### Comparing `thinkgpt-0.0.3/thinkgpt/llm.py` & `thinkgpt-0.0.4/thinkgpt/llm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
 from typing import List, Optional, Type, Dict, Any, Union, Iterable
 
-from langchain.llms import OpenAI, BaseLLM, OpenAIChat
+from langchain.llms import OpenAI
+from langchain.chat_models import ChatOpenAI
 from langchain.schema import LLMResult, BaseOutputParser, Generation
 from langchain.embeddings import OpenAIEmbeddings
 from docarray import DocumentArray, Document
 from pydantic.config import Extra
 from thinkgpt.helper import PythonREPL
 
 from thinkgpt.abstract import AbstractMixin, AbstractChain
@@ -15,15 +16,15 @@
 from thinkgpt.refine import RefineMixin, RefineChain
 from thinkgpt.gpt_select import SelectChain, SelectMixin
 
 from thinkgpt.summarize import SummarizeMixin, SummarizeChain
 
 
 
-class ThinkGPT(OpenAIChat, MemoryMixin, AbstractMixin, RefineMixin, ConditionMixin, SelectMixin, InferMixin, SummarizeMixin, extra=Extra.allow):
+class ThinkGPT(ChatOpenAI, MemoryMixin, AbstractMixin, RefineMixin, ConditionMixin, SelectMixin, InferMixin, SummarizeMixin, extra=Extra.allow):
     """Wrapper around OpenAI large language models to augment it with memory
 
     To use, you should have the ``openai`` python package installed, and the
     environment variable ``OPENAI_API_KEY`` set with your API key.
     """
 
     def __init__(self,
@@ -39,50 +40,50 @@
                  # TODO: model name can be specified per mixin
                  **kwargs
                  ):
         super().__init__(**kwargs)
         # TODO: offer more docarray backends
         self.memory = memory or DocumentArray()
         self.embeddings_model = OpenAIEmbeddings()
-        self.openai = OpenAI(model_name=kwargs.get('model_name'))
-        self.execute_with_context_chain = execute_with_context_chain or ExecuteWithContextChain.from_llm(
-            self.openai, verbose=verbose)
-        self.abstract_chain = abstract_chain or AbstractChain.from_llm(
-            self.openai, verbose=verbose)
-        self.refine_chain = refine_chain or RefineChain.from_llm(
-            self.openai, verbose=verbose)
-        self.condition_chain = condition_chain or ConditionChain.from_llm(
-            self.openai, verbose=verbose)
-        self.select_chain = select_chain or SelectChain.from_llm(self.openai, verbose=verbose)
-        self.infer_chain = infer_chain or InferChain.from_llm(self.openai, verbose=verbose)
-        self.summarize_chain = summarize_chain or SummarizeChain.from_llm(self.openai, verbose=verbose)  # Add this line
+        self.openai = ChatOpenAI(model_name=kwargs.get('model_name'))
+        self.execute_with_context_chain = execute_with_context_chain or ExecuteWithContextChain(
+            llm=self.openai, verbose=verbose)
+        self.abstract_chain = abstract_chain or AbstractChain(
+            llm=self.openai, verbose=verbose)
+        self.refine_chain = refine_chain or RefineChain(
+            llm=self.openai, verbose=verbose)
+        self.condition_chain = condition_chain or ConditionChain(
+            llm=self.openai, verbose=verbose)
+        self.select_chain = select_chain or SelectChain(llm=self.openai, verbose=verbose)
+        self.infer_chain = infer_chain or InferChain(llm=self.openai, verbose=verbose)
+        self.summarize_chain = summarize_chain or SummarizeChain(llm=self.openai, verbose=verbose)  # Add this line
         self.mem_cnt = 0
 
 
     def generate(
-            self, prompts: List[str], stop: Optional[List[str]] = None, remember: Union[int, List[str]] = 0
+            self, prompts: List[List[str]], stop: Optional[List[str]] = None, remember: Union[int, List[str]] = 0
     ) -> LLMResult:
         # only works for single prompt
         if len(prompts) > 1:
             raise Exception('only works for a single prompt')
-        prompt = prompts[0]
+        prompt = prompts[0][0]
         if isinstance(remember, int) and remember > 0:
             remembered_elements = self.remember(prompt, limit=5)
             result = self.execute_with_context_chain.predict(prompt=prompt, context='\n'.join(remembered_elements) if remembered_elements else 'Nothing')
         elif isinstance(remember, list):
             result = self.execute_with_context_chain.predict(prompt=prompt, context='\n'.join(remember))
         else:
-            return super().generate(prompts, stop=stop)
+            result = self.execute_with_context_chain.predict(prompt=prompt, context='Nothing')
 
         return LLMResult(generations=[[Generation(text=result)]])
 
     def predict(
             self, prompt: str, stop: Optional[List[str]] = None, remember: Union[int, List[str]] = 0
     ) -> str:
-        return self.generate([prompt], remember=remember).generations[0][0].text
+        return self.generate([[prompt]], remember=remember).generations[0][0].text
 
 
 if __name__ == '__main__':
     llm = ThinkGPT(model_name="gpt-3.5-turbo")
 
     rules = llm.abstract(observations=[
         "in tunisian, I did not eat is \"ma khditech\"",
```

### Comparing `thinkgpt-0.0.3/thinkgpt/memory.py` & `thinkgpt-0.0.4/thinkgpt/memory.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import re
 from typing import Dict, List, Union
 
 import numpy as np
 from langchain import PromptTemplate, LLMChain
 from langchain.embeddings import OpenAIEmbeddings
-from langchain.llms import OpenAI, BaseLLM, OpenAIChat
+from langchain.llms import OpenAI, BaseLLM
 from docarray import Document, DocumentArray
 
 
 EXECUTE_WITH_CONTEXT_PROMPT = PromptTemplate(template="""
 Given a context information, reply to the provided request
 Context: {context}
 User request: {prompt}
 """, input_variables=["prompt", "context"], )
 
 
 
 class ExecuteWithContextChain(LLMChain):
     """Prompts the LLM to execute a request with potential context"""
+    def __init__(self, **kwargs):
+        super().__init__(prompt=EXECUTE_WITH_CONTEXT_PROMPT, **kwargs)
 
     @classmethod
     def from_llm(cls, llm: BaseLLM, verbose: bool = True) -> LLMChain:
         """Get the response parser."""
         return cls(prompt=EXECUTE_WITH_CONTEXT_PROMPT, llm=llm, verbose=verbose)
```

### Comparing `thinkgpt-0.0.3/thinkgpt/refine.py` & `thinkgpt-0.0.4/thinkgpt/refine.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import warnings
 from typing import Dict, List, Any
 
 from langchain import PromptTemplate, LLMChain
-from langchain.llms import OpenAI, BaseLLM, OpenAIChat
+from langchain.llms import OpenAI, BaseLLM
+from langchain.chat_models import ChatOpenAI
 
 
 REFINE_PROMPT = PromptTemplate(template="""
 Based on the critics, fix the content provided to you. {instruction_hint}:
 content:
 {content}
 ---------
@@ -14,21 +15,19 @@
 {critics}
 ---------
 """, input_variables=["critics", "content", "instruction_hint"])
 
 
 class RefineChain(LLMChain):
     """Prompts the LLM to request to remember memory as needed"""
+    def __init__(self, **kwargs):
+        super().__init__(prompt=REFINE_PROMPT, **kwargs)
 
     @classmethod
     def from_llm(cls, llm: BaseLLM, verbose: bool = True) -> LLMChain:
-        if not (hasattr(llm, 'model_name') and llm.model_name == 'gpt-4'):
-            warnings.warn(
-                "Keep in mind that LLMs except 'gpt-4' do not exhibit as good criticizing and self-healing abilities as gpt-4"
-            )
         return cls(prompt=REFINE_PROMPT, llm=llm, verbose=verbose)
 
     def predict(self, instruction_hint: str = '', **kwargs: Any) -> str:
         return super().predict(instruction_hint=instruction_hint, **kwargs)
 
 
 class RefineMixin:
@@ -37,15 +36,15 @@
     def refine(self, content: str, critics: List[str], instruction_hint: str = '') -> str:
         return self.refine_chain.predict(
             content=content, critics="\n".join(critics), instruction_hint=instruction_hint
         )
 
 
 if __name__ == '__main__':
-    chain = RefineChain.from_llm(OpenAI(model_name="gpt-4"))
+    chain = RefineChain(llm=ChatOpenAI(model_name='gpt-3.5-turbo'))
     print(chain.predict(
         content="""
 import re
     print('hello world')
         """,
         critics="""
   File "/Users/alaeddine/Library/Application Support/JetBrains/PyCharm2022.3/scratches/scratch_166.py", line 2
```

### Comparing `thinkgpt-0.0.3/thinkgpt/summarize.py` & `thinkgpt-0.0.4/thinkgpt/summarize.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import textwrap
 
 from pydantic.config import Extra
 import warnings
 from typing import Dict, List, Any
 
 from langchain import PromptTemplate, LLMChain
-from langchain.llms import OpenAI, BaseLLM, OpenAIChat
+from langchain.llms import OpenAI, BaseLLM
+from langchain.chat_models import ChatOpenAI
 
 SUMMARIZE_PROMPT = PromptTemplate(template="""
 Shorten the following memory chunk of an autonomous agent from a first person perspective, using at most {max_tokens} tokens. {instruction_hint}:
 content:
 {content}
 ---------
 """, input_variables=["content", "instruction_hint", "max_tokens"])
@@ -17,16 +18,15 @@
 
 class SummarizeChain(LLMChain, extra=Extra.allow):
     """Prompts the LLM to summarize content as needed"""
     def __init__(self,
                  summarizer_chunk_size: int = 3000,
                  **kwargs
                  ):
-        super().__init__(**kwargs)
-        # TODO: offer more docarray backends
+        super().__init__(prompt=SUMMARIZE_PROMPT, **kwargs)
         self.summarizer_chunk_size = summarizer_chunk_size
 
     @classmethod
     def from_llm(cls, llm: BaseLLM, verbose: bool = True) -> LLMChain:
         return cls(prompt=SUMMARIZE_PROMPT, llm=llm, verbose=verbose)
 
     def predict(self, content, **kwargs: Any) -> str:
@@ -60,15 +60,15 @@
                 result += self.summarize(content=chunk, max_tokens=summary_size, instruction_hint=instruction_hint)
         else:
             return content
         return result
 
 
 if __name__ == '__main__':
-    chain = SummarizeChain.from_llm(OpenAI(model_name="gpt-3.5-turbo"))
+    chain = SummarizeChain(llm=ChatOpenAI(model_name="gpt-3.5-turbo"))
     print(chain.predict(
         content="""Artificial intelligence (AI) is intelligence demonstrated by machines, 
         unlike the natural intelligence displayed by humans and animals, which involves 
         consciousness and emotionality. The distinction between the former and the latter 
         categories is often revealed by the acronym chosen. 'Strong' AI is usually labelled 
         as AGI (Artificial General Intelligence) while attempts to emulate 'natural' 
         intelligence have been called ABI (Artificial Biological Intelligence).""",
```

### Comparing `thinkgpt-0.0.3/PKG-INFO` & `thinkgpt-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thinkgpt
-Version: 0.0.3
+Version: 0.0.4
 Summary: ThinkGPT is a Python library aimed at implementing Chain of Thoughts for Large Language Models (LLMs), prompting the model to think, reason, and to create generative agents.
 License: Apache 2.0
 Author: Alaeddine Abdessalem
 Author-email: alaeddine-13@live.fr
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```


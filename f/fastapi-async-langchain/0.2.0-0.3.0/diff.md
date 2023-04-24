# Comparing `tmp/fastapi_async_langchain-0.2.0.tar.gz` & `tmp/fastapi_async_langchain-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_async_langchain-0.2.0.tar", max compression
+gzip compressed data, was "fastapi_async_langchain-0.3.0.tar", max compression
```

## Comparing `fastapi_async_langchain-0.2.0.tar` & `fastapi_async_langchain-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,10 @@
--rw-r--r--   0        0        0     1073 2023-04-22 19:56:23.738974 fastapi_async_langchain-0.2.0/LICENSE
--rw-r--r--   0        0        0     1574 2023-04-22 19:56:23.738974 fastapi_async_langchain-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-04-22 19:56:23.742974 fastapi_async_langchain-0.2.0/fastapi_async_langchain/__init__.py
--rw-r--r--   0        0        0      648 2023-04-22 19:56:23.742974 fastapi_async_langchain-0.2.0/fastapi_async_langchain/callback.py
--rw-r--r--   0        0        0     2511 2023-04-22 19:56:23.742974 fastapi_async_langchain-0.2.0/fastapi_async_langchain/response.py
--rw-r--r--   0        0        0      481 2023-04-22 19:56:23.742974 fastapi_async_langchain-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2139 1970-01-01 00:00:00.000000 fastapi_async_langchain-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-24 13:16:17.460813 fastapi_async_langchain-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1574 2023-04-24 13:16:17.460813 fastapi_async_langchain-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-24 13:16:17.464813 fastapi_async_langchain-0.3.0/fastapi_async_langchain/__init__.py
+-rw-r--r--   0        0        0      648 2023-04-24 13:16:17.468813 fastapi_async_langchain-0.3.0/fastapi_async_langchain/callback.py
+-rw-r--r--   0        0        0      171 2023-04-24 13:16:17.468813 fastapi_async_langchain-0.3.0/fastapi_async_langchain/responses/__init__.py
+-rw-r--r--   0        0        0     1743 2023-04-24 13:16:17.468813 fastapi_async_langchain-0.3.0/fastapi_async_langchain/responses/base.py
+-rw-r--r--   0        0        0     1182 2023-04-24 13:16:17.468813 fastapi_async_langchain-0.3.0/fastapi_async_langchain/responses/llm.py
+-rw-r--r--   0        0        0     1493 2023-04-24 13:16:17.468813 fastapi_async_langchain-0.3.0/fastapi_async_langchain/responses/retrieval_qa.py
+-rw-r--r--   0        0        0      481 2023-04-24 13:16:17.468813 fastapi_async_langchain-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2139 1970-01-01 00:00:00.000000 fastapi_async_langchain-0.3.0/PKG-INFO
```

### Comparing `fastapi_async_langchain-0.2.0/LICENSE` & `fastapi_async_langchain-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.2.0/README.md` & `fastapi_async_langchain-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.2.0/fastapi_async_langchain/callback.py` & `fastapi_async_langchain-0.3.0/fastapi_async_langchain/callback.py`

 * *Files identical despite different names*

### Comparing `fastapi_async_langchain-0.2.0/fastapi_async_langchain/response.py` & `fastapi_async_langchain-0.3.0/fastapi_async_langchain/responses/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,27 @@
 from functools import partial
 from typing import Any, Dict, Union
 
 from fastapi.responses import StreamingResponse
-from langchain import LLMChain
-from langchain.callbacks import AsyncCallbackManager
+from langchain.chains.base import Chain
 from starlette.types import Send
 
-from .callback import AsyncFastApiStreamingCallback
 
-
-class LangchainStreamingResponse(StreamingResponse):
-    """StreamingResponse for langchain LLM chains."""
+class BaseLangchainStreamingResponse(StreamingResponse):
+    """Base StreamingResponse class wrapper for langchain chains."""
 
     def __init__(
         self,
-        chain: LLMChain,
+        chain: Chain,
         inputs: Union[Dict[str, Any], Any],
         **kwargs: Any,
     ) -> None:
         super().__init__(content=iter(()), **kwargs)
 
-        def chain_wrapper_fn(chain: LLMChain, inputs: Union[Dict[str, Any], Any]):
-            async def wrapper(send: Send):
-                if not isinstance(chain.llm.callback_manager, AsyncCallbackManager):
-                    raise TypeError(
-                        "llm.callback_manager must be an instance of AsyncCallbackManager"
-                    )
-                for handler in chain.llm.callback_manager.handlers:
-                    if isinstance(handler, AsyncFastApiStreamingCallback):
-                        chain.llm.callback_manager.remove_handler(handler)
-                        break
-                chain.llm.callback_manager.add_handler(
-                    AsyncFastApiStreamingCallback(send=send)
-                )
-                return await chain.arun(inputs)
-
-            return wrapper
-
-        self.chain_wrapper_fn = chain_wrapper_fn(chain, inputs)
+        self.chain_wrapper_fn = self.chain_wrapper_fn(chain, inputs)
 
     async def stream_response(self, send: Send) -> None:
         await send(
             {
                 "type": "http.response.start",
                 "status": self.status_code,
                 "headers": self.raw_headers,
@@ -64,7 +44,11 @@
                     "body": str(e).encode(self.charset),
                     "more_body": False,
                 }
             )
             return
 
         await send({"type": "http.response.body", "body": b"", "more_body": False})
+
+    @staticmethod
+    def chain_wrapper_fn(chain: Chain, inputs: Union[Dict[str, Any], Any]):
+        raise NotImplementedError
```

### Comparing `fastapi_async_langchain-0.2.0/PKG-INFO` & `fastapi_async_langchain-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-async-langchain
-Version: 0.2.0
+Version: 0.3.0
 Summary: FastAPI async components for streaming LLM chains.
 Author: Ajinkya Indulkar
 Author-email: 26824103+ajndkr@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


# Comparing `tmp/griseo-0.7.2.tar.gz` & `tmp/griseo-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griseo-0.7.2.tar", max compression
+gzip compressed data, was "griseo-0.8.0.tar", max compression
```

## Comparing `griseo-0.7.2.tar` & `griseo-0.8.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-04-07 10:13:05.026502 griseo-0.7.2/LICENSE
--rw-r--r--   0        0        0      280 2023-04-07 10:13:05.026502 griseo-0.7.2/README.md
--rw-r--r--   0        0        0     3191 2023-04-07 10:13:05.026502 griseo-0.7.2/griseo/__init__.py
--rw-r--r--   0        0        0      653 2023-04-07 10:13:05.026502 griseo-0.7.2/griseo/__main__.py
--rw-r--r--   0        0        0     1193 2023-04-07 10:13:05.026502 griseo-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     1115 1970-01-01 00:00:00.000000 griseo-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-24 14:34:40.416451 griseo-0.8.0/LICENSE
+-rw-r--r--   0        0        0      280 2023-04-24 14:34:40.416451 griseo-0.8.0/README.md
+-rw-r--r--   0        0        0     3403 2023-04-24 14:34:40.416451 griseo-0.8.0/griseo/__init__.py
+-rw-r--r--   0        0        0      653 2023-04-24 14:34:40.416451 griseo-0.8.0/griseo/__main__.py
+-rw-r--r--   0        0        0     1193 2023-04-24 14:34:40.416451 griseo-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1115 1970-01-01 00:00:00.000000 griseo-0.8.0/PKG-INFO
```

### Comparing `griseo-0.7.2/LICENSE` & `griseo-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `griseo-0.7.2/griseo/__init__.py` & `griseo-0.8.0/griseo/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import sys
+import textwrap
 from argparse import ArgumentParser, ArgumentDefaultsHelpFormatter, REMAINDER
 from importlib import metadata
 
 import openai
 
 __version__ = metadata.version(__package__)
 del metadata  # avoids polluting the results of dir(__package__)
@@ -69,20 +70,29 @@
     commands = {
         'c': lambda: ctx.clear(),
         'clear': lambda: ctx.clear(),
         'q': lambda: sys.exit(0),
         'quit': lambda: sys.exit(0),
     }
 
+    print(textwrap.dedent(f"""\
+    Welcome to chat with Griseo!
+
+    type :c or :clear to clear context
+    type :q or :quit  to exit
+    """))
+
     while True:
         req = input('user << ').strip()
         if req.startswith(':'):
             commands[req[1:]]()
             continue
-        ctx.tell(req)
+
+        if len(req) > 0:  # skip empty input
+            ctx.tell(req)
 
 
 def main():
     import dotenv
     import os
 
     dotenv.load_dotenv()
```

### Comparing `griseo-0.7.2/griseo/__main__.py` & `griseo-0.8.0/griseo/__main__.py`

 * *Files identical despite different names*

### Comparing `griseo-0.7.2/pyproject.toml` & `griseo-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 [tool.poetry]
 name = "griseo"
-version = "0.7.2"
+version = "0.8.0"
 description = "Chat with OpenAI in the Hacker way."
 authors = ["tison <wander4096@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/korandoru/griseo"
 repository = "https://github.com/korandoru/griseo"
 documentation = "https://github.com/korandoru/griseo"
```

### Comparing `griseo-0.7.2/PKG-INFO` & `griseo-0.8.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: griseo
-Version: 0.7.2
+Version: 0.8.0
 Summary: Chat with OpenAI in the Hacker way.
 Home-page: https://github.com/korandoru/griseo
 License: Apache-2.0
 Keywords: chatgpt,cli,openai
 Author: tison
 Author-email: wander4096@gmail.com
 Requires-Python: >=3.8,<4.0
```


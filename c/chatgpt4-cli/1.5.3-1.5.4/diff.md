# Comparing `tmp/chatgpt4-cli-1.5.3.tar.gz` & `tmp/chatgpt4-cli-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt4-cli-1.5.3.tar", last modified: Mon Apr 24 13:40:47 2023, max compression
+gzip compressed data, was "chatgpt4-cli-1.5.4.tar", last modified: Mon Apr 24 16:05:42 2023, max compression
```

## Comparing `chatgpt4-cli-1.5.3.tar` & `chatgpt4-cli-1.5.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:40:47.943168 chatgpt4-cli-1.5.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:40:47.943168 chatgpt4-cli-1.5.3/GPTCLI/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-24 13:40:22.000000 chatgpt4-cli-1.5.3/GPTCLI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-24 13:40:22.000000 chatgpt4-cli-1.5.3/GPTCLI/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-04-24 13:40:22.000000 chatgpt4-cli-1.5.3/GPTCLI/addons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-24 13:40:22.000000 chatgpt4-cli-1.5.3/GPTCLI/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-04-24 13:40:22.000000 chatgpt4-cli-1.5.3/GPTCLI/emage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    32308 2023-04-24 13:40:22.000000 chatgpt4-cli-1.5.3/GPTCLI/gptcli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-04-24 13:40:22.000000 chatgpt4-cli-1.5.3/GPTCLI/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-04-24 13:40:22.000000 chatgpt4-cli-1.5.3/GPTCLI/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-24 13:40:22.000000 chatgpt4-cli-1.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15275 2023-04-24 13:40:47.943168 chatgpt4-cli-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14204 2023-04-24 13:40:22.000000 chatgpt4-cli-1.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:40:47.943168 chatgpt4-cli-1.5.3/chatgpt4_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15275 2023-04-24 13:40:47.000000 chatgpt4-cli-1.5.3/chatgpt4_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-24 13:40:47.000000 chatgpt4-cli-1.5.3/chatgpt4_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:40:47.000000 chatgpt4-cli-1.5.3/chatgpt4_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 13:40:47.000000 chatgpt4-cli-1.5.3/chatgpt4_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-24 13:40:47.000000 chatgpt4-cli-1.5.3/chatgpt4_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 13:40:47.000000 chatgpt4-cli-1.5.3/chatgpt4_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 13:40:47.943168 chatgpt4-cli-1.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-24 13:40:22.000000 chatgpt4-cli-1.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:05:42.244313 chatgpt4-cli-1.5.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:05:42.240313 chatgpt4-cli-1.5.4/GPTCLI/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-24 16:05:15.000000 chatgpt4-cli-1.5.4/GPTCLI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-24 16:05:15.000000 chatgpt4-cli-1.5.4/GPTCLI/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-04-24 16:05:15.000000 chatgpt4-cli-1.5.4/GPTCLI/addons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-24 16:05:15.000000 chatgpt4-cli-1.5.4/GPTCLI/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-04-24 16:05:15.000000 chatgpt4-cli-1.5.4/GPTCLI/emage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32351 2023-04-24 16:05:15.000000 chatgpt4-cli-1.5.4/GPTCLI/gptcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-04-24 16:05:15.000000 chatgpt4-cli-1.5.4/GPTCLI/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-04-24 16:05:15.000000 chatgpt4-cli-1.5.4/GPTCLI/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-24 16:05:15.000000 chatgpt4-cli-1.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15275 2023-04-24 16:05:42.244313 chatgpt4-cli-1.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14204 2023-04-24 16:05:15.000000 chatgpt4-cli-1.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:05:42.240313 chatgpt4-cli-1.5.4/chatgpt4_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15275 2023-04-24 16:05:42.000000 chatgpt4-cli-1.5.4/chatgpt4_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-24 16:05:42.000000 chatgpt4-cli-1.5.4/chatgpt4_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 16:05:42.000000 chatgpt4-cli-1.5.4/chatgpt4_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 16:05:42.000000 chatgpt4-cli-1.5.4/chatgpt4_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-24 16:05:42.000000 chatgpt4-cli-1.5.4/chatgpt4_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 16:05:42.000000 chatgpt4-cli-1.5.4/chatgpt4_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 16:05:42.244313 chatgpt4-cli-1.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-24 16:05:15.000000 chatgpt4-cli-1.5.4/setup.py
```

### Comparing `chatgpt4-cli-1.5.3/GPTCLI/__init__.py` & `chatgpt4-cli-1.5.4/GPTCLI/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.5.3"
+__version__ = "1.5.4"
 __author__ = "Smartwa Caleb"
 __repo__ = "https://github.com/Simatwa/gpt-cli"
 __info__ = "Interact with ChatGPT and Bard at the terminal."
 
 import logging
 
 logging.basicConfig(
```

### Comparing `chatgpt4-cli-1.5.3/GPTCLI/addons.py` & `chatgpt4-cli-1.5.4/GPTCLI/addons.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import re
 from os import remove, system
 from time import sleep
 from . import logging, getExc
 from threading import Thread as thr
+from sys import exit
 
 
 class file_parser:
     """Handles contents from text file"""
 
     def __init__(self, prompt):
         self.prompt = prompt
@@ -140,12 +141,31 @@
 
     @classmethod
     def stop_spinning(cls):
         """Stop displaying busy-bar"""
         if cls.querying:
             cls.querying = False
             sleep(cls.sleep_time)
-
+    
+    @classmethod
+    def run(cls):
+        """Handles GPT querying functions
+        """
+        def decorator(func):
+            def main(*args,**kwargs):
+                try:
+                    return func(*args,**kwargs)
+                except KeyboardInterrupt:
+                    cls.stop_spinning()
+                    return 
+                except EOFError:
+                    cls.querying = False
+                    exit(logging.info("Stopping program"))
+                except Exception as e:
+                    cls.stop_spinning()
+                    logging.error(getExc(e))
+            return main
+        return decorator
 
 if __name__ == "__main__":
     st = file_parser("I want you to debug this python code {f.test.py}")
     print(st.parse)
```

### Comparing `chatgpt4-cli-1.5.3/GPTCLI/bard.py` & `chatgpt4-cli-1.5.4/GPTCLI/bard.py`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.5.3/GPTCLI/emage.py` & `chatgpt4-cli-1.5.4/GPTCLI/emage.py`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.5.3/GPTCLI/gptcli.py` & `chatgpt4-cli-1.5.4/GPTCLI/gptcli.py`

 * *Files 0% similar despite different names*

```diff
@@ -597,15 +597,16 @@
         if isinstance(prompt, list):
             if len(prompt) >= 2 and prompt[0:2] == ["I'm", "sorry"]:
                 resp = False
         else:
             if prompt.startswith("I'm sorry"):
                 resp = False
         return resp
-
+    
+    @progress.run()
     def default(self, raw, return_fb=False, no_check=False):
         raw = self.parser(raw)
         run_against_system = False
         if not raw:
             self.do__prompt(self.prompt_disp)
             return
         # out = lambda b: print(self.color_dict[args.output_color] + b + Fore.RESET)
@@ -626,23 +627,24 @@
                 if return_fb:
                     return feedback.strip()
                 record_keeper.main(feedback)
                 if run_against_system:
                     system_control(feedback).execute(args.sudo)
 
             else:
-                progress.querying = False
+                progress.stop_spinning()
                 logging.error(str(rp[1]))
             print(Fore.RESET)
         self.do__prompt(self.prompt_disp)
 
     def do_gpt4(self, line):
         """Interact with ChatGPT4"""
         self.default(line, no_check=True)
 
+    @progress.run()
     def do_bard(self, line, return_fb=False, chat=False):
         """Interact with Google's bard"""
         progress.display_bar(args)
         if "--gpt4" in line:
             return self.default(line.replace("--gpt4", ""), no_check=True)
 
         args.message = line
```

### Comparing `chatgpt4-cli-1.5.3/GPTCLI/helper.py` & `chatgpt4-cli-1.5.4/GPTCLI/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,9 +76,11 @@
 * Use `_botchat` to let the 2 GPTs chat to each other
 
 * Use double `./` (fullstop and foward slash) to interact with system commands
       e.g './ifconfig'
       
 * Use {{f.text-filename}} to issue prompt contained in  the 'text-filename'
 
-* _exit or `CTRL+C` : Quits the program.
+* Use `CTRL+C` to cancel a request 
+
+* _exit or `CTRL+C` or `CTRL+Z` : Quits the program.
         """
```

### Comparing `chatgpt4-cli-1.5.3/GPTCLI/image.py` & `chatgpt4-cli-1.5.4/GPTCLI/image.py`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.5.3/LICENSE` & `chatgpt4-cli-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.5.3/PKG-INFO` & `chatgpt4-cli-1.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt4-cli
-Version: 1.5.3
+Version: 1.5.4
 Summary: Interact with ChatGPT and Bard at the terminal.
 Home-page: https://github.com/Simatwa/gpt-cli
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/issues/new
@@ -24,15 +24,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">gpt-cli</h1>
 <p align="center">
 <a href="https://github.com/Simatwa/gpt-cli"><img src="https://img.shields.io/static/v1?logo=Github&label=Github&message=Passing&color=lime" alt="Gihtub"/></a>
-<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.3&color=green&logo=pypi" alt="Pypi"/>
+<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.4&color=green&logo=pypi" alt="Pypi"/>
 <a href="https://wakatime.com/badge/github/Simatwa/gpt-cli"><img src="https://wakatime.com/badge/github/Simatwa/gpt-cli.svg" alt="wakatime"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=License&message=MIT&color=green&logo=MIT" alt="license"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Development&message=Beta&color=Orange&logo=progress" alt="Progress"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Code Style&message=Black&color=black&logo=Black" alt="Code-style"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=green" alt="Coverage"/></a>
 <a href="https://pepy.tech/project/chatgpt4-cli"><img src="https://static.pepy.tech/badge/chatgpt4-cli" alt="Downloads"/></a>
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.5.3 Summary: Interact with
+Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.5.4 Summary: Interact with
 ChatGPT and Bard at the terminal. Home-page: https://github.com/Simatwa/gpt-cli
 Author: Smartwa Caleb Author-email: smartwacaleb@gmail.com Maintainer: Smartwa
 Caleb License: MIT Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/
 issues/new Classifier: License :: OSI Approved :: MIT License Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English Classifier: License :: Free For Home
 Use Classifier: Topic :: Home Automation Classifier: Intended Audience ::
```

### Comparing `chatgpt4-cli-1.5.3/README.md` & `chatgpt4-cli-1.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <h1 align="center">gpt-cli</h1>
 <p align="center">
 <a href="https://github.com/Simatwa/gpt-cli"><img src="https://img.shields.io/static/v1?logo=Github&label=Github&message=Passing&color=lime" alt="Gihtub"/></a>
-<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.3&color=green&logo=pypi" alt="Pypi"/>
+<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.4&color=green&logo=pypi" alt="Pypi"/>
 <a href="https://wakatime.com/badge/github/Simatwa/gpt-cli"><img src="https://wakatime.com/badge/github/Simatwa/gpt-cli.svg" alt="wakatime"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=License&message=MIT&color=green&logo=MIT" alt="license"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Development&message=Beta&color=Orange&logo=progress" alt="Progress"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Code Style&message=Black&color=black&logo=Black" alt="Code-style"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=green" alt="Coverage"/></a>
 <a href="https://pepy.tech/project/chatgpt4-cli"><img src="https://static.pepy.tech/badge/chatgpt4-cli" alt="Downloads"/></a>
 </p>
```

### Comparing `chatgpt4-cli-1.5.3/chatgpt4_cli.egg-info/PKG-INFO` & `chatgpt4-cli-1.5.4/chatgpt4_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt4-cli
-Version: 1.5.3
+Version: 1.5.4
 Summary: Interact with ChatGPT and Bard at the terminal.
 Home-page: https://github.com/Simatwa/gpt-cli
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/issues/new
@@ -24,15 +24,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">gpt-cli</h1>
 <p align="center">
 <a href="https://github.com/Simatwa/gpt-cli"><img src="https://img.shields.io/static/v1?logo=Github&label=Github&message=Passing&color=lime" alt="Gihtub"/></a>
-<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.3&color=green&logo=pypi" alt="Pypi"/>
+<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.4&color=green&logo=pypi" alt="Pypi"/>
 <a href="https://wakatime.com/badge/github/Simatwa/gpt-cli"><img src="https://wakatime.com/badge/github/Simatwa/gpt-cli.svg" alt="wakatime"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=License&message=MIT&color=green&logo=MIT" alt="license"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Development&message=Beta&color=Orange&logo=progress" alt="Progress"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Code Style&message=Black&color=black&logo=Black" alt="Code-style"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=green" alt="Coverage"/></a>
 <a href="https://pepy.tech/project/chatgpt4-cli"><img src="https://static.pepy.tech/badge/chatgpt4-cli" alt="Downloads"/></a>
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.5.3 Summary: Interact with
+Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.5.4 Summary: Interact with
 ChatGPT and Bard at the terminal. Home-page: https://github.com/Simatwa/gpt-cli
 Author: Smartwa Caleb Author-email: smartwacaleb@gmail.com Maintainer: Smartwa
 Caleb License: MIT Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/
 issues/new Classifier: License :: OSI Approved :: MIT License Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English Classifier: License :: Free For Home
 Use Classifier: Topic :: Home Automation Classifier: Intended Audience ::
```

### Comparing `chatgpt4-cli-1.5.3/setup.py` & `chatgpt4-cli-1.5.4/setup.py`

 * *Files identical despite different names*


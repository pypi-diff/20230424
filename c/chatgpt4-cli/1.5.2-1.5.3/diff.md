# Comparing `tmp/chatgpt4-cli-1.5.2.tar.gz` & `tmp/chatgpt4-cli-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt4-cli-1.5.2.tar", last modified: Fri Apr 21 07:05:03 2023, max compression
+gzip compressed data, was "chatgpt4-cli-1.5.3.tar", last modified: Mon Apr 24 13:40:47 2023, max compression
```

## Comparing `chatgpt4-cli-1.5.2.tar` & `chatgpt4-cli-1.5.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:05:03.425552 chatgpt4-cli-1.5.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:05:03.425552 chatgpt4-cli-1.5.2/GPTCLI/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-21 07:04:41.000000 chatgpt4-cli-1.5.2/GPTCLI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-21 07:04:41.000000 chatgpt4-cli-1.5.2/GPTCLI/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-21 07:04:41.000000 chatgpt4-cli-1.5.2/GPTCLI/addons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-21 07:04:41.000000 chatgpt4-cli-1.5.2/GPTCLI/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-04-21 07:04:41.000000 chatgpt4-cli-1.5.2/GPTCLI/emage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31397 2023-04-21 07:04:41.000000 chatgpt4-cli-1.5.2/GPTCLI/gptcli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-04-21 07:04:41.000000 chatgpt4-cli-1.5.2/GPTCLI/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-04-21 07:04:41.000000 chatgpt4-cli-1.5.2/GPTCLI/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-21 07:04:41.000000 chatgpt4-cli-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15170 2023-04-21 07:05:03.425552 chatgpt4-cli-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14099 2023-04-21 07:04:41.000000 chatgpt4-cli-1.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:05:03.425552 chatgpt4-cli-1.5.2/chatgpt4_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15170 2023-04-21 07:05:03.000000 chatgpt4-cli-1.5.2/chatgpt4_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-21 07:05:03.000000 chatgpt4-cli-1.5.2/chatgpt4_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 07:05:03.000000 chatgpt4-cli-1.5.2/chatgpt4_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-21 07:05:03.000000 chatgpt4-cli-1.5.2/chatgpt4_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-21 07:05:03.000000 chatgpt4-cli-1.5.2/chatgpt4_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 07:05:03.000000 chatgpt4-cli-1.5.2/chatgpt4_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 07:05:03.425552 chatgpt4-cli-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-04-21 07:04:41.000000 chatgpt4-cli-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:40:47.943168 chatgpt4-cli-1.5.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:40:47.943168 chatgpt4-cli-1.5.3/GPTCLI/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-24 13:40:22.000000 chatgpt4-cli-1.5.3/GPTCLI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-24 13:40:22.000000 chatgpt4-cli-1.5.3/GPTCLI/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-04-24 13:40:22.000000 chatgpt4-cli-1.5.3/GPTCLI/addons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-24 13:40:22.000000 chatgpt4-cli-1.5.3/GPTCLI/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-04-24 13:40:22.000000 chatgpt4-cli-1.5.3/GPTCLI/emage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32308 2023-04-24 13:40:22.000000 chatgpt4-cli-1.5.3/GPTCLI/gptcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-04-24 13:40:22.000000 chatgpt4-cli-1.5.3/GPTCLI/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-04-24 13:40:22.000000 chatgpt4-cli-1.5.3/GPTCLI/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-24 13:40:22.000000 chatgpt4-cli-1.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15275 2023-04-24 13:40:47.943168 chatgpt4-cli-1.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14204 2023-04-24 13:40:22.000000 chatgpt4-cli-1.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:40:47.943168 chatgpt4-cli-1.5.3/chatgpt4_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15275 2023-04-24 13:40:47.000000 chatgpt4-cli-1.5.3/chatgpt4_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-24 13:40:47.000000 chatgpt4-cli-1.5.3/chatgpt4_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:40:47.000000 chatgpt4-cli-1.5.3/chatgpt4_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 13:40:47.000000 chatgpt4-cli-1.5.3/chatgpt4_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-24 13:40:47.000000 chatgpt4-cli-1.5.3/chatgpt4_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 13:40:47.000000 chatgpt4-cli-1.5.3/chatgpt4_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 13:40:47.943168 chatgpt4-cli-1.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-24 13:40:22.000000 chatgpt4-cli-1.5.3/setup.py
```

### Comparing `chatgpt4-cli-1.5.2/GPTCLI/__init__.py` & `chatgpt4-cli-1.5.3/GPTCLI/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-__version__ = "1.5.2"
+__version__ = "1.5.3"
 __author__ = "Smartwa Caleb"
 __repo__ = "https://github.com/Simatwa/gpt-cli"
+__info__ = "Interact with ChatGPT and Bard at the terminal."
 
 import logging
 
 logging.basicConfig(
     format="%(levelname)s - %(message)s - (%(asctime)s) ",  # [%(module)s,%(lineno)s]",
     datefmt="%d-%b-%Y %H:%M:%S",
     level=logging.INFO,
```

### Comparing `chatgpt4-cli-1.5.2/GPTCLI/addons.py` & `chatgpt4-cli-1.5.3/GPTCLI/addons.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
 from os import remove, system
 from time import sleep
 from . import logging, getExc
+from threading import Thread as thr
 
 
 class file_parser:
     """Handles contents from text file"""
 
     def __init__(self, prompt):
         self.prompt = prompt
@@ -106,10 +107,45 @@
         """Deletes the bash script file"""
         try:
             remove(self.file_name)
         except Exception as e:
             logging.error(getExc(e))
 
 
+class progress:
+    querying = None
+    __spinner = (("-", "\\", "|", "/"), ("█■■■■", "■█■■■", "■■█■■", "■■■█■", "■■■■█"))
+    sleep_time = 0.1
+
+    @classmethod
+    def __action(cls, index):
+        while cls.querying:
+            for spin in cls.__spinner[index]:
+                print(" " + spin, end="\r", flush=True)
+                if not cls.querying:
+                    break
+                sleep(cls.sleep_time)
+
+    @classmethod
+    def display_bar(cls, args):
+        try:
+            cls.querying = True
+            t1 = thr(
+                target=cls.__action,
+                args=(args.spinner - 1,),
+            )
+            t1.start()
+        except Exception as e:
+            cls.querying = False
+            logging.debug(getExc(e))
+
+    @classmethod
+    def stop_spinning(cls):
+        """Stop displaying busy-bar"""
+        if cls.querying:
+            cls.querying = False
+            sleep(cls.sleep_time)
+
+
 if __name__ == "__main__":
     st = file_parser("I want you to debug this python code {f.test.py}")
     print(st.parse)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `chatgpt4-cli-1.5.2/GPTCLI/bard.py` & `chatgpt4-cli-1.5.3/GPTCLI/bard.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from Bard import Chatbot
-from . import logging, error_handler,getExc
+from . import logging, error_handler, getExc
 from sys import exit
 from os import environ
 from json import load
 from time import sleep
 
 
 class Bard:
```

### Comparing `chatgpt4-cli-1.5.2/GPTCLI/emage.py` & `chatgpt4-cli-1.5.3/GPTCLI/emage.py`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.5.2/GPTCLI/gptcli.py` & `chatgpt4-cli-1.5.3/GPTCLI/gptcli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/python
-from . import __version__, __author__, __repo__
+from . import __version__, __author__, __repo__, __info__
 from colorama import Fore, Back
 from os import getlogin, getcwd, path
 from rich.console import Console
 from rich.panel import Panel
 from rich.style import Style
 from rich import print as rich_print
 import argparse
@@ -56,17 +56,15 @@
         disp = f"""
             Repo : {__repo__}
             By   : {__author__}"""
         gstyle = Style(color="cyan", frame="double")
         intro = Panel(disp, title=f"gpt-cli v{__version__}", style=gstyle)
         rich_print(intro)
 
-        parser = argparse.ArgumentParser(
-            description="Interact with ChatGPT at the terminal"
-        )
+        parser = argparse.ArgumentParser(description=__info__)
         parser.add_argument(
             "-v", "--version", action="version", version=f"%(prog)s v{__version__}"
         )
         parser.add_argument("message", help="Message to be send.", nargs="*")
         models = [
             "text-davinci-001",
             "text-davinci-002",
@@ -174,15 +172,15 @@
             default="yellow",
             metavar="[cyan|green|yellow|red]",
             choices=self.colors,
         )
         parser.add_argument(
             "--prompt",
             help="Customizes the prompt display",
-            default=f"┌─[{getlogin().capitalize()}@ChatGPT4]─(%H:%M:%S)",
+            default=f"┌─[{getlogin().capitalize()}@GPTs]─(%H:%M:%S)",
             dest="settings",
             nargs="*",
         )
         parser.add_argument(
             "-tm",
             "--timeout",
             help="Request timeout while making request - (Soon)",
@@ -280,14 +278,23 @@
             "--stream-interval",
             metavar="TIME",
             help="Interval for printing responses in (s)",
             type=float,
             default=0.01,
         )
         parser.add_argument(
+            "-spin",
+            "--spinner",
+            choices=[1, 2],
+            type=int,
+            help="Busy bar indicator",
+            metavar="1|2",
+            default=2,
+        )
+        parser.add_argument(
             "--disable-stream",
             help="Specifies not to stream responses from ChatGPT",
             action="store_true",
         )
         parser.add_argument(
             "--new-record",
             help="Override previous chats under the filepath",
@@ -338,21 +345,21 @@
 from .emage import emager
 from re import sub
 from datetime import datetime
 from os import system, remove, path, environ, makedirs
 from threading import Thread as thr
 from appdirs import AppDirs
 from rich.markdown import Markdown
-from .addons import file_parser, system_control
+from .addons import file_parser, system_control, progress
 from .bard import Bard
 from time import sleep
 
 app_dir = AppDirs(
-    "smartwa",
     "gpt-cli",
+    "smartwa",
 ).user_data_dir
 
 first_time_run = False
 
 date_stamp = lambda text: datetime.today().strftime(text)
 
 if not path.isdir(app_dir):
@@ -373,29 +380,33 @@
 
     def gpt_v1(self, rp: str = None):
         """Utilises GPTv1"""
         if not args.disable_stream:
             for data in chatbot.ask_stream(
                 args.message, args.temperature, user=args.role
             ):
+                progress.stop_spinning()
                 print(data, end="", flush=True)
                 rp = "".join([rp, data])
         else:
             rp = chatbot.ask(args.message, user=args.role)
+            progress.stop_spinning()
             self.out(rp)
         return rp
 
     def gpt_v4(self, rp: str = None):
         """Utilises GPTv4"""
         if not args.disable_stream:
             for data in chatbot.ask_stream(args.message, role=args.role):
+                progress.stop_spinning()
                 print(data, end="", flush=True)
                 rp = "".join([rp, data])
         else:
             rp = chatbot.ask(args.message, role=args.role)
+            progress.stop_spinning()
             self.out(rp)
         return rp
 
     def main(self):
         """Main Method"""
         try:
             if args.gpt in ("4"):
@@ -565,16 +576,20 @@
     )
     prompt = time_now_format(prompt_disp)
     config_handler = config_handler()
     color_dict = config_handler.color_dict
     bcolor_dict = config_handler.bcolor_dict
     interactive = local_interactor()
     parser = lambda self, line: file_parser(line).parse()
-    if not args.update:
+    if any([args.bkey, args.bkey_path, args.bcookie_file, environ.get("BARD_SESSION")]):
         bard = Bard(args)
+    elif args.bard:
+        exit(logging.critical("Bard's cookie file is required"))
+    elif not any([args.dump, args.update]):
+        logging.warning("Cannot use Bard, since cookie file is missing.")
 
     def apply_color(self):
         print(
             self.bcolor_dict[args.background_color] + self.color_dict[args.input_color]
         )
 
     def prompt_is_error_free(self, prompt, resp=True) -> bool:
@@ -593,14 +608,15 @@
         if not raw:
             self.do__prompt(self.prompt_disp)
             return
         # out = lambda b: print(self.color_dict[args.output_color] + b + Fore.RESET)
         if raw[0:2] == "./":
             system((raw[2:]).strip())
         else:
+            progress.display_bar(args)
             if "--system" in raw:
                 run_against_system = True
                 raw = raw.replace("--system", "")
             if any(["--bard" in raw, args.bard]) and not no_check:
                 return self.do_bard(raw.replace("--bard", ""))
             args.message = raw
             print(self.color_dict[args.output_color], end="")
@@ -610,40 +626,44 @@
                 if return_fb:
                     return feedback.strip()
                 record_keeper.main(feedback)
                 if run_against_system:
                     system_control(feedback).execute(args.sudo)
 
             else:
+                progress.querying = False
                 logging.error(str(rp[1]))
             print(Fore.RESET)
         self.do__prompt(self.prompt_disp)
 
     def do_gpt4(self, line):
         """Interact with ChatGPT4"""
         self.default(line, no_check=True)
 
     def do_bard(self, line, return_fb=False, chat=False):
         """Interact with Google's bard"""
+        progress.display_bar(args)
         if "--gpt4" in line:
             return self.default(line.replace("--gpt4", ""), no_check=True)
 
         args.message = line
         if chat:
             print(self.color_dict[args.input_color], end="")
         else:
             print(self.color_dict[args.output_color], end="")
         if args.disable_stream:
             inf, info = self.bard.chat(line, False), ""
             for value in inf:
+                progress.stop_spinning()
                 info = info + value
             gpt3.out(info)
         else:
             info = ""
             for val in self.bard.chat(line):
+                progress.stop_spinning()
                 print(val, end="", flush=True)
                 info = info + val
         if not chat:
             record_keeper.main(info)
         print(self.color_dict[args.input_color])
         self.do__prompt(self.prompt_disp)
         if return_fb:
@@ -752,14 +772,15 @@
                     "Cookie file is required at launch [--cookie-file {path}]"
                 )
         except Exception as e:
             logging.error(getExc(e))
         self.do__prompt(self.prompt_disp)
 
     def do__prompt(self, line):
+        progress.querying = False
         line = self.parser(line)
         if not line:
             return
         """Modify prompts"""
         self.prompt_disp = line
         self.prompt = time_now_format(line)
 
@@ -963,15 +984,17 @@
             )
             if args.bard:
                 run.do_bard(prompt)
             else:
                 run.default(prompt)
         run.cmdloop()
     except (KeyboardInterrupt, EOFError):
+        progress.querying = False
         exit(logging.info("Stopping program"))
     except Exception as e:
+        progress.querying = False
         # logging.exception(e)
         logging.error(getExc(e))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `chatgpt4-cli-1.5.2/GPTCLI/helper.py` & `chatgpt4-cli-1.5.3/GPTCLI/helper.py`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.5.2/GPTCLI/image.py` & `chatgpt4-cli-1.5.3/GPTCLI/image.py`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.5.2/LICENSE` & `chatgpt4-cli-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.5.2/PKG-INFO` & `chatgpt4-cli-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt4-cli
-Version: 1.5.2
+Version: 1.5.3
 Summary: Interact with ChatGPT and Bard at the terminal.
 Home-page: https://github.com/Simatwa/gpt-cli
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/issues/new
@@ -24,25 +24,25 @@
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">gpt-cli</h1>
 <p align="center">
 <a href="https://github.com/Simatwa/gpt-cli"><img src="https://img.shields.io/static/v1?logo=Github&label=Github&message=Passing&color=lime" alt="Gihtub"/></a>
-<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.2&color=green&logo=pypi" alt="Pypi"/>
+<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.3&color=green&logo=pypi" alt="Pypi"/>
 <a href="https://wakatime.com/badge/github/Simatwa/gpt-cli"><img src="https://wakatime.com/badge/github/Simatwa/gpt-cli.svg" alt="wakatime"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=License&message=MIT&color=green&logo=MIT" alt="license"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Development&message=Beta&color=Orange&logo=progress" alt="Progress"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Code Style&message=Black&color=black&logo=Black" alt="Code-style"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=green" alt="Coverage"/></a>
 <a href="https://pepy.tech/project/chatgpt4-cli"><img src="https://static.pepy.tech/badge/chatgpt4-cli" alt="Downloads"/></a>
 </p>
 
 CLI tool for interacting with [ChatGPT](https://openai.com) and [Bard](https://bard.google.com).
-> Generate images with Bing and ChatGPT's DALL-E model.
+> Generate images with BingImageCreator and ChatGPT's DALL-E models.
 
 ![screenshot](https://github.com/Simatwa/gpt-cli/raw/main/assets/Screenshot1.png)
 
 ## [Independencies](requirements.txt)
 
 * [Openai](https://github.com/openai/openai-python)
 * [Numpy](https://github.com/numpy/numpy)
@@ -230,33 +230,33 @@
 <summary>
 
 For more info run `gpt-cli -h`.
 
 </summary>
 
 ```
-╭─────────────────────────────── gpt-cli v1.4.9 ───────────────────────────────╮
+╭─────────────────────────────── gpt-cli v1.5.3 ───────────────────────────────╮
 │                                                                              │
 │             Repo : https://github.com/Simatwa/gpt-cli                        │
 │             By   : Smartwa Caleb                                             │
 ╰──────────────────────────────────────────────────────────────────────────────╯
 usage: gpt-cli [-h] [-v] [-m gpt-3.5-turbo|gpt-4|gpt-4-32k] [-t [0.1-1]]
                [-mt [1-7000]] [-tp [0.1-1]] [-f [0.1-2]] [-p [0.1-2]] [-k KEY]
                [-kp path] [-ic [cyan|green|yellow|red]]
                [-oc [cyan|green|yellow|red]] [-bc [blue,magenta,black,reset]]
                [-pc [cyan|green|yellow|red]] [--prompt [SETTINGS ...]]
                [-tm value] [-pr PROXY] [-rc value] [-g 1,4] [-sp [text ...]]
                [-fp path] [-o path] [-pp prefix] [-rp prefix]
                [-dm keys|values|show|{fnm}] [-dl symbol] [-cf path] [-bk KEY]
-               [-bkp PATH] [-bcf PATH] [-si TIME] [--disable-stream]
-               [--new-record] [--disable-recording] [--zero-show] [--bard]
-               [--markdown] [--update] [--sudo]
+               [-bkp PATH] [-bcf PATH] [-si TIME] [-spin 1|2]
+               [--disable-stream] [--new-record] [--disable-recording]
+               [--zero-show] [--bard] [--markdown] [--update] [--sudo]
                [message ...]
 
-Interact with ChatGPT at the terminal
+Interact with ChatGPT and Bard at the terminal.
 
 positional arguments:
   message               Message to be send.
 
 options:
   -h, --help            show this help message and exit
   -v, --version         show program's version number and exit
@@ -318,14 +318,16 @@
                         Bard's session value
   -bkp PATH, --bard-key-path PATH
                         Path to Bard's key path
   -bcf PATH, --bard-cookie-file PATH
                         Path to Bard's cookie file
   -si TIME, --stream-interval TIME
                         Interval for printing responses in (s)
+  -spin 1|2, --spinner 1|2
+                        Busy bar indicator
   --disable-stream      Specifies not to stream responses from ChatGPT
   --new-record          Override previous chats under the filepath
   --disable-recording   Disable saving prompts and responses
   --zero-show           Specifies not to stdout prompt of the act parsed
   --bard                Make Bard the default GPT
   --markdown            Stdout responses in markdown-format - disables
                         streaming
@@ -359,15 +361,15 @@
 
 - Anyone is free to [fork](https://github.com/Simatwa/gpt-cli/fork), submit an [issue](https://github.com/Simatwa/gpt-cli/issues) without any **guideline** or submitting a [pull request](https://github.com/Simatwa/gpt-cli/pulls).
 
 ### ToDo
 
 - [x] Use dialogue
 - [x] Issue prompt from a file
-- [ ] Busy bar
+- [x] Busy bar
 
   > Review [CHANGELOG](https://github.com/Simatwa/gpt-cli/blob/main/CHANGELOG.md)
 
 ## Acknowledgements
 
 1. [remo7777](https://github.com/remo7777/T-Header)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.5.2 Summary: Interact with
+Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.5.3 Summary: Interact with
 ChatGPT and Bard at the terminal. Home-page: https://github.com/Simatwa/gpt-cli
 Author: Smartwa Caleb Author-email: smartwacaleb@gmail.com Maintainer: Smartwa
 Caleb License: MIT Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/
 issues/new Classifier: License :: OSI Approved :: MIT License Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English Classifier: License :: Free For Home
 Use Classifier: Topic :: Home Automation Classifier: Intended Audience ::
@@ -12,16 +12,16 @@
 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown License-File: LICENSE
                              ****** gpt-cli ******
    [Gihtub] [Pypi]_[wakatime]_[license]_[Progress]_[Code-style]_[Coverage]_
                                   [Downloads]
 CLI tool for interacting with [ChatGPT](https://openai.com) and [Bard](https://
-bard.google.com). > Generate images with Bing and ChatGPT's DALL-E model. !
-[screenshot](https://github.com/Simatwa/gpt-cli/raw/main/assets/
+bard.google.com). > Generate images with BingImageCreator and ChatGPT's DALL-
+E models. ![screenshot](https://github.com/Simatwa/gpt-cli/raw/main/assets/
 Screenshot1.png) ## [Independencies](requirements.txt) * [Openai](https://
 github.com/openai/openai-python) * [Numpy](https://github.com/numpy/numpy) *
 [Colorama](https://github.com/tartley/colorama) * [revChatGPT](https://
 github.com/acheong08/ChatGPT) ### Features - Chat with ChatGPT and Bard
 conversationally. - Let **ChatGPT** and **Bard** chat to each other. - Generate
 Images (DALL-E & BingImageCreator)- Based on your prompt or GPT generated
 description. - Stream or Non-stream responses. - Maintain record of the chats.
@@ -83,74 +83,75 @@
 13._help : Show this help info * Use `./` (fullstop and forward slash) to
 interact with **system commands** - e.g ```./ifconfig``` * Use `_botchat` to
 let the 2 GPTs chat to each other > **Note** You can further specify the GPT to
 be used by appending `--gpt4` or `--bard` in the prompt. * Use *{{f.text-
 filename}}* to issue prompt contained in the 'text-filename'    For more info
 run `gpt-cli -h`.  ```
 â­âââââââââââââââââââââââââââââââ
-gpt-cli v1.4.9
+gpt-cli v1.5.3
 ââââââââââââââââââââââââââââââââ®
 â â â Repo : https://github.com/Simatwa/gpt-cli â â By : Smartwa
 Caleb â
 â°âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
 usage: gpt-cli [-h] [-v] [-m gpt-3.5-turbo|gpt-4|gpt-4-32k] [-t [0.1-1]] [-mt
 [1-7000]] [-tp [0.1-1]] [-f [0.1-2]] [-p [0.1-2]] [-k KEY] [-kp path] [-ic
 [cyan|green|yellow|red]] [-oc [cyan|green|yellow|red]] [-bc
 [blue,magenta,black,reset]] [-pc [cyan|green|yellow|red]] [--prompt [SETTINGS
 ...]] [-tm value] [-pr PROXY] [-rc value] [-g 1,4] [-sp [text ...]] [-fp path]
 [-o path] [-pp prefix] [-rp prefix] [-dm keys|values|show|{fnm}] [-dl symbol]
-[-cf path] [-bk KEY] [-bkp PATH] [-bcf PATH] [-si TIME] [--disable-stream] [--
-new-record] [--disable-recording] [--zero-show] [--bard] [--markdown] [--
-update] [--sudo] [message ...] Interact with ChatGPT at the terminal positional
-arguments: message Message to be send. options: -h, --help show this help
-message and exit -v, --version show program's version number and exit -m gpt-
-3.5-turbo|gpt-4|gpt-4-32k, --model gpt-3.5-turbo|gpt-4|gpt-4-32k ChatGPT model
-to be used -t [0.1-1], --temperature [0.1-1] Charge of the generated text's
-randomness -mt [1-7000], --max-tokens [1-7000] Maximum number of tokens to be
-generated upon completion -tp [0.1-1], --top-p [0.1-1] Sampling threshold
-during inference time -f [0.1-2], --frequency-penalty [0.1-2] Chances of word
-being repeated -p [0.1-2], --presence-frequency [0.1-2] Chances of topic being
-repeated -k KEY, --key KEY OPENAI-API-KEY -kp path, --key-path path Path to
-text-file containing GPT-api key -ic [cyan|green|yellow|red], --input-color
-[cyan|green|yellow|red] Font color for inputs -oc [cyan|green|yellow|red], --
-output-color [cyan|green|yellow|red] Font color for outputs -bc
-[blue,magenta,black,reset], --background-color [blue,magenta,black,reset]
-Console's background-color -pc [cyan|green|yellow|red], --prompt-color
-[cyan|green|yellow|red] Prompt's display color --prompt [SETTINGS ...]
-Customizes the prompt display -tm value, --timeout value Request timeout while
-making request - (Soon) -pr PROXY, --proxy PROXY Pivot request through this
-proxy -rc value, --reply-count value Number of responses to be received -g 1,4,
---gpt 1,4 ChatGPT version to be used -sp [text ...], --system-prompt [text ...]
-Text to train ChatGPT at the start -fp path, --file-path path Path to .csv file
-containing role and prompt - [act,prompt] -o path, --output path Filepath for
-saving the chats - default [/home/smartwa/git/gpt-cli/.chatgpt-history.txt] -pp
-prefix, --prompt-prefix prefix Text to append before saving each prompt -
-default [>>> timestamp] -rp prefix, --response-prefix prefix Text to append
-before saving each response - default [None] -dm keys|values|show|{fnm}, --dump
-keys|values|show|{fnm} Stdout [keys,values]; Save all prompts in json format to
-a file -dl symbol, --delimiter symbol Delimeter for the .CSV file -
-[act,prompt] -cf path, --cookie-file path Path to Bing's cookies - for Edge
-Image Generation -bk KEY, --bard-key KEY Bard's session value -bkp PATH, --
-bard-key-path PATH Path to Bard's key path -bcf PATH, --bard-cookie-file PATH
-Path to Bard's cookie file -si TIME, --stream-interval TIME Interval for
-printing responses in (s) --disable-stream Specifies not to stream responses
-from ChatGPT --new-record Override previous chats under the filepath --disable-
-recording Disable saving prompts and responses --zero-show Specifies not to
-stdout prompt of the act parsed --bard Make Bard the default GPT --markdown
-Stdout responses in markdown-format - disables streaming --update Download
-latest prompts - [awesome-chatgpt-prompts] --sudo Run commands against system
-with sudo privileges ```  > **Note** : **gpt-4** *(model)* supports upto *7000*
-tokens and others *3000*. > **Warning** : **gpt-1** Has issues - *(To be fixed
-later)* Visit [acheong08/Bard](https://github.com/acheong08/Bard) for info on
-how to get the Bard's cookie file and Sessions. ## Motive   Love for `Terminal`
-â¤ï¸  As a `terminal guy` I used to find it uncomfortable to keep shifting
-from one window to next in order to access ChatGPT even after trying out the
-[gpt-login](https://github.com/Simatwa/gpt-login), the rest is [here.](https://
-github.com/Simatwa/gpt-cli)  ## Contributions - Anyone is free to [fork](https:
-//github.com/Simatwa/gpt-cli/fork), submit an [issue](https://github.com/
-Simatwa/gpt-cli/issues) without any **guideline** or submitting a [pull
-request](https://github.com/Simatwa/gpt-cli/pulls). ### ToDo - [x] Use dialogue
-- [x] Issue prompt from a file - [ ] Busy bar > Review [CHANGELOG](https://
-github.com/Simatwa/gpt-cli/blob/main/CHANGELOG.md) ## Acknowledgements 1.
-[remo7777](https://github.com/remo7777/T-Header) 2. [acheong08](https://
+[-cf path] [-bk KEY] [-bkp PATH] [-bcf PATH] [-si TIME] [-spin 1|2] [--disable-
+stream] [--new-record] [--disable-recording] [--zero-show] [--bard] [--
+markdown] [--update] [--sudo] [message ...] Interact with ChatGPT and Bard at
+the terminal. positional arguments: message Message to be send. options: -h, --
+help show this help message and exit -v, --version show program's version
+number and exit -m gpt-3.5-turbo|gpt-4|gpt-4-32k, --model gpt-3.5-turbo|gpt-
+4|gpt-4-32k ChatGPT model to be used -t [0.1-1], --temperature [0.1-1] Charge
+of the generated text's randomness -mt [1-7000], --max-tokens [1-7000] Maximum
+number of tokens to be generated upon completion -tp [0.1-1], --top-p [0.1-1]
+Sampling threshold during inference time -f [0.1-2], --frequency-penalty [0.1-
+2] Chances of word being repeated -p [0.1-2], --presence-frequency [0.1-2]
+Chances of topic being repeated -k KEY, --key KEY OPENAI-API-KEY -kp path, --
+key-path path Path to text-file containing GPT-api key -ic
+[cyan|green|yellow|red], --input-color [cyan|green|yellow|red] Font color for
+inputs -oc [cyan|green|yellow|red], --output-color [cyan|green|yellow|red] Font
+color for outputs -bc [blue,magenta,black,reset], --background-color
+[blue,magenta,black,reset] Console's background-color -pc
+[cyan|green|yellow|red], --prompt-color [cyan|green|yellow|red] Prompt's
+display color --prompt [SETTINGS ...] Customizes the prompt display -tm value,
+--timeout value Request timeout while making request - (Soon) -pr PROXY, --
+proxy PROXY Pivot request through this proxy -rc value, --reply-count value
+Number of responses to be received -g 1,4, --gpt 1,4 ChatGPT version to be used
+-sp [text ...], --system-prompt [text ...] Text to train ChatGPT at the start -
+fp path, --file-path path Path to .csv file containing role and prompt -
+[act,prompt] -o path, --output path Filepath for saving the chats - default [/
+home/smartwa/git/gpt-cli/.chatgpt-history.txt] -pp prefix, --prompt-prefix
+prefix Text to append before saving each prompt - default [>>> timestamp] -rp
+prefix, --response-prefix prefix Text to append before saving each response -
+default [None] -dm keys|values|show|{fnm}, --dump keys|values|show|{fnm} Stdout
+[keys,values]; Save all prompts in json format to a file -dl symbol, --
+delimiter symbol Delimeter for the .CSV file - [act,prompt] -cf path, --cookie-
+file path Path to Bing's cookies - for Edge Image Generation -bk KEY, --bard-
+key KEY Bard's session value -bkp PATH, --bard-key-path PATH Path to Bard's key
+path -bcf PATH, --bard-cookie-file PATH Path to Bard's cookie file -si TIME, --
+stream-interval TIME Interval for printing responses in (s) -spin 1|2, --
+spinner 1|2 Busy bar indicator --disable-stream Specifies not to stream
+responses from ChatGPT --new-record Override previous chats under the filepath
+--disable-recording Disable saving prompts and responses --zero-show Specifies
+not to stdout prompt of the act parsed --bard Make Bard the default GPT --
+markdown Stdout responses in markdown-format - disables streaming --update
+Download latest prompts - [awesome-chatgpt-prompts] --sudo Run commands against
+system with sudo privileges ```  > **Note** : **gpt-4** *(model)* supports upto
+*7000* tokens and others *3000*. > **Warning** : **gpt-1** Has issues - *(To be
+fixed later)* Visit [acheong08/Bard](https://github.com/acheong08/Bard) for
+info on how to get the Bard's cookie file and Sessions. ## Motive   Love for
+`Terminal` â¤ï¸  As a `terminal guy` I used to find it uncomfortable to keep
+shifting from one window to next in order to access ChatGPT even after trying
+out the [gpt-login](https://github.com/Simatwa/gpt-login), the rest is [here.]
+(https://github.com/Simatwa/gpt-cli)  ## Contributions - Anyone is free to
+[fork](https://github.com/Simatwa/gpt-cli/fork), submit an [issue](https://
+github.com/Simatwa/gpt-cli/issues) without any **guideline** or submitting a
+[pull request](https://github.com/Simatwa/gpt-cli/pulls). ### ToDo - [x] Use
+dialogue - [x] Issue prompt from a file - [x] Busy bar > Review [CHANGELOG]
+(https://github.com/Simatwa/gpt-cli/blob/main/CHANGELOG.md) ## Acknowledgements
+1. [remo7777](https://github.com/remo7777/T-Header) 2. [acheong08](https://
 github.com/acheong08/ChatGPT) 3. [f](https://github.com/f/awesome-chatgpt-
 prompts)
```

### Comparing `chatgpt4-cli-1.5.2/README.md` & `chatgpt4-cli-1.5.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <h1 align="center">gpt-cli</h1>
 <p align="center">
 <a href="https://github.com/Simatwa/gpt-cli"><img src="https://img.shields.io/static/v1?logo=Github&label=Github&message=Passing&color=lime" alt="Gihtub"/></a>
-<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.2&color=green&logo=pypi" alt="Pypi"/>
+<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.3&color=green&logo=pypi" alt="Pypi"/>
 <a href="https://wakatime.com/badge/github/Simatwa/gpt-cli"><img src="https://wakatime.com/badge/github/Simatwa/gpt-cli.svg" alt="wakatime"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=License&message=MIT&color=green&logo=MIT" alt="license"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Development&message=Beta&color=Orange&logo=progress" alt="Progress"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Code Style&message=Black&color=black&logo=Black" alt="Code-style"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=green" alt="Coverage"/></a>
 <a href="https://pepy.tech/project/chatgpt4-cli"><img src="https://static.pepy.tech/badge/chatgpt4-cli" alt="Downloads"/></a>
 </p>
 
 CLI tool for interacting with [ChatGPT](https://openai.com) and [Bard](https://bard.google.com).
-> Generate images with Bing and ChatGPT's DALL-E model.
+> Generate images with BingImageCreator and ChatGPT's DALL-E models.
 
 ![screenshot](https://github.com/Simatwa/gpt-cli/raw/main/assets/Screenshot1.png)
 
 ## [Independencies](requirements.txt)
 
 * [Openai](https://github.com/openai/openai-python)
 * [Numpy](https://github.com/numpy/numpy)
@@ -203,33 +203,33 @@
 <summary>
 
 For more info run `gpt-cli -h`.
 
 </summary>
 
 ```
-╭─────────────────────────────── gpt-cli v1.4.9 ───────────────────────────────╮
+╭─────────────────────────────── gpt-cli v1.5.3 ───────────────────────────────╮
 │                                                                              │
 │             Repo : https://github.com/Simatwa/gpt-cli                        │
 │             By   : Smartwa Caleb                                             │
 ╰──────────────────────────────────────────────────────────────────────────────╯
 usage: gpt-cli [-h] [-v] [-m gpt-3.5-turbo|gpt-4|gpt-4-32k] [-t [0.1-1]]
                [-mt [1-7000]] [-tp [0.1-1]] [-f [0.1-2]] [-p [0.1-2]] [-k KEY]
                [-kp path] [-ic [cyan|green|yellow|red]]
                [-oc [cyan|green|yellow|red]] [-bc [blue,magenta,black,reset]]
                [-pc [cyan|green|yellow|red]] [--prompt [SETTINGS ...]]
                [-tm value] [-pr PROXY] [-rc value] [-g 1,4] [-sp [text ...]]
                [-fp path] [-o path] [-pp prefix] [-rp prefix]
                [-dm keys|values|show|{fnm}] [-dl symbol] [-cf path] [-bk KEY]
-               [-bkp PATH] [-bcf PATH] [-si TIME] [--disable-stream]
-               [--new-record] [--disable-recording] [--zero-show] [--bard]
-               [--markdown] [--update] [--sudo]
+               [-bkp PATH] [-bcf PATH] [-si TIME] [-spin 1|2]
+               [--disable-stream] [--new-record] [--disable-recording]
+               [--zero-show] [--bard] [--markdown] [--update] [--sudo]
                [message ...]
 
-Interact with ChatGPT at the terminal
+Interact with ChatGPT and Bard at the terminal.
 
 positional arguments:
   message               Message to be send.
 
 options:
   -h, --help            show this help message and exit
   -v, --version         show program's version number and exit
@@ -291,14 +291,16 @@
                         Bard's session value
   -bkp PATH, --bard-key-path PATH
                         Path to Bard's key path
   -bcf PATH, --bard-cookie-file PATH
                         Path to Bard's cookie file
   -si TIME, --stream-interval TIME
                         Interval for printing responses in (s)
+  -spin 1|2, --spinner 1|2
+                        Busy bar indicator
   --disable-stream      Specifies not to stream responses from ChatGPT
   --new-record          Override previous chats under the filepath
   --disable-recording   Disable saving prompts and responses
   --zero-show           Specifies not to stdout prompt of the act parsed
   --bard                Make Bard the default GPT
   --markdown            Stdout responses in markdown-format - disables
                         streaming
@@ -332,15 +334,15 @@
 
 - Anyone is free to [fork](https://github.com/Simatwa/gpt-cli/fork), submit an [issue](https://github.com/Simatwa/gpt-cli/issues) without any **guideline** or submitting a [pull request](https://github.com/Simatwa/gpt-cli/pulls).
 
 ### ToDo
 
 - [x] Use dialogue
 - [x] Issue prompt from a file
-- [ ] Busy bar
+- [x] Busy bar
 
   > Review [CHANGELOG](https://github.com/Simatwa/gpt-cli/blob/main/CHANGELOG.md)
 
 ## Acknowledgements
 
 1. [remo7777](https://github.com/remo7777/T-Header)
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
                              ****** gpt-cli ******
    [Gihtub] [Pypi]_[wakatime]_[license]_[Progress]_[Code-style]_[Coverage]_
                                   [Downloads]
 CLI tool for interacting with [ChatGPT](https://openai.com) and [Bard](https://
-bard.google.com). > Generate images with Bing and ChatGPT's DALL-E model. !
-[screenshot](https://github.com/Simatwa/gpt-cli/raw/main/assets/
+bard.google.com). > Generate images with BingImageCreator and ChatGPT's DALL-
+E models. ![screenshot](https://github.com/Simatwa/gpt-cli/raw/main/assets/
 Screenshot1.png) ## [Independencies](requirements.txt) * [Openai](https://
 github.com/openai/openai-python) * [Numpy](https://github.com/numpy/numpy) *
 [Colorama](https://github.com/tartley/colorama) * [revChatGPT](https://
 github.com/acheong08/ChatGPT) ### Features - Chat with ChatGPT and Bard
 conversationally. - Let **ChatGPT** and **Bard** chat to each other. - Generate
 Images (DALL-E & BingImageCreator)- Based on your prompt or GPT generated
 description. - Stream or Non-stream responses. - Maintain record of the chats.
@@ -69,74 +69,75 @@
 13._help : Show this help info * Use `./` (fullstop and forward slash) to
 interact with **system commands** - e.g ```./ifconfig``` * Use `_botchat` to
 let the 2 GPTs chat to each other > **Note** You can further specify the GPT to
 be used by appending `--gpt4` or `--bard` in the prompt. * Use *{{f.text-
 filename}}* to issue prompt contained in the 'text-filename'    For more info
 run `gpt-cli -h`.  ```
 â­âââââââââââââââââââââââââââââââ
-gpt-cli v1.4.9
+gpt-cli v1.5.3
 ââââââââââââââââââââââââââââââââ®
 â â â Repo : https://github.com/Simatwa/gpt-cli â â By : Smartwa
 Caleb â
 â°âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
 usage: gpt-cli [-h] [-v] [-m gpt-3.5-turbo|gpt-4|gpt-4-32k] [-t [0.1-1]] [-mt
 [1-7000]] [-tp [0.1-1]] [-f [0.1-2]] [-p [0.1-2]] [-k KEY] [-kp path] [-ic
 [cyan|green|yellow|red]] [-oc [cyan|green|yellow|red]] [-bc
 [blue,magenta,black,reset]] [-pc [cyan|green|yellow|red]] [--prompt [SETTINGS
 ...]] [-tm value] [-pr PROXY] [-rc value] [-g 1,4] [-sp [text ...]] [-fp path]
 [-o path] [-pp prefix] [-rp prefix] [-dm keys|values|show|{fnm}] [-dl symbol]
-[-cf path] [-bk KEY] [-bkp PATH] [-bcf PATH] [-si TIME] [--disable-stream] [--
-new-record] [--disable-recording] [--zero-show] [--bard] [--markdown] [--
-update] [--sudo] [message ...] Interact with ChatGPT at the terminal positional
-arguments: message Message to be send. options: -h, --help show this help
-message and exit -v, --version show program's version number and exit -m gpt-
-3.5-turbo|gpt-4|gpt-4-32k, --model gpt-3.5-turbo|gpt-4|gpt-4-32k ChatGPT model
-to be used -t [0.1-1], --temperature [0.1-1] Charge of the generated text's
-randomness -mt [1-7000], --max-tokens [1-7000] Maximum number of tokens to be
-generated upon completion -tp [0.1-1], --top-p [0.1-1] Sampling threshold
-during inference time -f [0.1-2], --frequency-penalty [0.1-2] Chances of word
-being repeated -p [0.1-2], --presence-frequency [0.1-2] Chances of topic being
-repeated -k KEY, --key KEY OPENAI-API-KEY -kp path, --key-path path Path to
-text-file containing GPT-api key -ic [cyan|green|yellow|red], --input-color
-[cyan|green|yellow|red] Font color for inputs -oc [cyan|green|yellow|red], --
-output-color [cyan|green|yellow|red] Font color for outputs -bc
-[blue,magenta,black,reset], --background-color [blue,magenta,black,reset]
-Console's background-color -pc [cyan|green|yellow|red], --prompt-color
-[cyan|green|yellow|red] Prompt's display color --prompt [SETTINGS ...]
-Customizes the prompt display -tm value, --timeout value Request timeout while
-making request - (Soon) -pr PROXY, --proxy PROXY Pivot request through this
-proxy -rc value, --reply-count value Number of responses to be received -g 1,4,
---gpt 1,4 ChatGPT version to be used -sp [text ...], --system-prompt [text ...]
-Text to train ChatGPT at the start -fp path, --file-path path Path to .csv file
-containing role and prompt - [act,prompt] -o path, --output path Filepath for
-saving the chats - default [/home/smartwa/git/gpt-cli/.chatgpt-history.txt] -pp
-prefix, --prompt-prefix prefix Text to append before saving each prompt -
-default [>>> timestamp] -rp prefix, --response-prefix prefix Text to append
-before saving each response - default [None] -dm keys|values|show|{fnm}, --dump
-keys|values|show|{fnm} Stdout [keys,values]; Save all prompts in json format to
-a file -dl symbol, --delimiter symbol Delimeter for the .CSV file -
-[act,prompt] -cf path, --cookie-file path Path to Bing's cookies - for Edge
-Image Generation -bk KEY, --bard-key KEY Bard's session value -bkp PATH, --
-bard-key-path PATH Path to Bard's key path -bcf PATH, --bard-cookie-file PATH
-Path to Bard's cookie file -si TIME, --stream-interval TIME Interval for
-printing responses in (s) --disable-stream Specifies not to stream responses
-from ChatGPT --new-record Override previous chats under the filepath --disable-
-recording Disable saving prompts and responses --zero-show Specifies not to
-stdout prompt of the act parsed --bard Make Bard the default GPT --markdown
-Stdout responses in markdown-format - disables streaming --update Download
-latest prompts - [awesome-chatgpt-prompts] --sudo Run commands against system
-with sudo privileges ```  > **Note** : **gpt-4** *(model)* supports upto *7000*
-tokens and others *3000*. > **Warning** : **gpt-1** Has issues - *(To be fixed
-later)* Visit [acheong08/Bard](https://github.com/acheong08/Bard) for info on
-how to get the Bard's cookie file and Sessions. ## Motive   Love for `Terminal`
-â¤ï¸  As a `terminal guy` I used to find it uncomfortable to keep shifting
-from one window to next in order to access ChatGPT even after trying out the
-[gpt-login](https://github.com/Simatwa/gpt-login), the rest is [here.](https://
-github.com/Simatwa/gpt-cli)  ## Contributions - Anyone is free to [fork](https:
-//github.com/Simatwa/gpt-cli/fork), submit an [issue](https://github.com/
-Simatwa/gpt-cli/issues) without any **guideline** or submitting a [pull
-request](https://github.com/Simatwa/gpt-cli/pulls). ### ToDo - [x] Use dialogue
-- [x] Issue prompt from a file - [ ] Busy bar > Review [CHANGELOG](https://
-github.com/Simatwa/gpt-cli/blob/main/CHANGELOG.md) ## Acknowledgements 1.
-[remo7777](https://github.com/remo7777/T-Header) 2. [acheong08](https://
+[-cf path] [-bk KEY] [-bkp PATH] [-bcf PATH] [-si TIME] [-spin 1|2] [--disable-
+stream] [--new-record] [--disable-recording] [--zero-show] [--bard] [--
+markdown] [--update] [--sudo] [message ...] Interact with ChatGPT and Bard at
+the terminal. positional arguments: message Message to be send. options: -h, --
+help show this help message and exit -v, --version show program's version
+number and exit -m gpt-3.5-turbo|gpt-4|gpt-4-32k, --model gpt-3.5-turbo|gpt-
+4|gpt-4-32k ChatGPT model to be used -t [0.1-1], --temperature [0.1-1] Charge
+of the generated text's randomness -mt [1-7000], --max-tokens [1-7000] Maximum
+number of tokens to be generated upon completion -tp [0.1-1], --top-p [0.1-1]
+Sampling threshold during inference time -f [0.1-2], --frequency-penalty [0.1-
+2] Chances of word being repeated -p [0.1-2], --presence-frequency [0.1-2]
+Chances of topic being repeated -k KEY, --key KEY OPENAI-API-KEY -kp path, --
+key-path path Path to text-file containing GPT-api key -ic
+[cyan|green|yellow|red], --input-color [cyan|green|yellow|red] Font color for
+inputs -oc [cyan|green|yellow|red], --output-color [cyan|green|yellow|red] Font
+color for outputs -bc [blue,magenta,black,reset], --background-color
+[blue,magenta,black,reset] Console's background-color -pc
+[cyan|green|yellow|red], --prompt-color [cyan|green|yellow|red] Prompt's
+display color --prompt [SETTINGS ...] Customizes the prompt display -tm value,
+--timeout value Request timeout while making request - (Soon) -pr PROXY, --
+proxy PROXY Pivot request through this proxy -rc value, --reply-count value
+Number of responses to be received -g 1,4, --gpt 1,4 ChatGPT version to be used
+-sp [text ...], --system-prompt [text ...] Text to train ChatGPT at the start -
+fp path, --file-path path Path to .csv file containing role and prompt -
+[act,prompt] -o path, --output path Filepath for saving the chats - default [/
+home/smartwa/git/gpt-cli/.chatgpt-history.txt] -pp prefix, --prompt-prefix
+prefix Text to append before saving each prompt - default [>>> timestamp] -rp
+prefix, --response-prefix prefix Text to append before saving each response -
+default [None] -dm keys|values|show|{fnm}, --dump keys|values|show|{fnm} Stdout
+[keys,values]; Save all prompts in json format to a file -dl symbol, --
+delimiter symbol Delimeter for the .CSV file - [act,prompt] -cf path, --cookie-
+file path Path to Bing's cookies - for Edge Image Generation -bk KEY, --bard-
+key KEY Bard's session value -bkp PATH, --bard-key-path PATH Path to Bard's key
+path -bcf PATH, --bard-cookie-file PATH Path to Bard's cookie file -si TIME, --
+stream-interval TIME Interval for printing responses in (s) -spin 1|2, --
+spinner 1|2 Busy bar indicator --disable-stream Specifies not to stream
+responses from ChatGPT --new-record Override previous chats under the filepath
+--disable-recording Disable saving prompts and responses --zero-show Specifies
+not to stdout prompt of the act parsed --bard Make Bard the default GPT --
+markdown Stdout responses in markdown-format - disables streaming --update
+Download latest prompts - [awesome-chatgpt-prompts] --sudo Run commands against
+system with sudo privileges ```  > **Note** : **gpt-4** *(model)* supports upto
+*7000* tokens and others *3000*. > **Warning** : **gpt-1** Has issues - *(To be
+fixed later)* Visit [acheong08/Bard](https://github.com/acheong08/Bard) for
+info on how to get the Bard's cookie file and Sessions. ## Motive   Love for
+`Terminal` â¤ï¸  As a `terminal guy` I used to find it uncomfortable to keep
+shifting from one window to next in order to access ChatGPT even after trying
+out the [gpt-login](https://github.com/Simatwa/gpt-login), the rest is [here.]
+(https://github.com/Simatwa/gpt-cli)  ## Contributions - Anyone is free to
+[fork](https://github.com/Simatwa/gpt-cli/fork), submit an [issue](https://
+github.com/Simatwa/gpt-cli/issues) without any **guideline** or submitting a
+[pull request](https://github.com/Simatwa/gpt-cli/pulls). ### ToDo - [x] Use
+dialogue - [x] Issue prompt from a file - [x] Busy bar > Review [CHANGELOG]
+(https://github.com/Simatwa/gpt-cli/blob/main/CHANGELOG.md) ## Acknowledgements
+1. [remo7777](https://github.com/remo7777/T-Header) 2. [acheong08](https://
 github.com/acheong08/ChatGPT) 3. [f](https://github.com/f/awesome-chatgpt-
 prompts)
```

### Comparing `chatgpt4-cli-1.5.2/chatgpt4_cli.egg-info/PKG-INFO` & `chatgpt4-cli-1.5.3/chatgpt4_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt4-cli
-Version: 1.5.2
+Version: 1.5.3
 Summary: Interact with ChatGPT and Bard at the terminal.
 Home-page: https://github.com/Simatwa/gpt-cli
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/issues/new
@@ -24,25 +24,25 @@
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">gpt-cli</h1>
 <p align="center">
 <a href="https://github.com/Simatwa/gpt-cli"><img src="https://img.shields.io/static/v1?logo=Github&label=Github&message=Passing&color=lime" alt="Gihtub"/></a>
-<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.2&color=green&logo=pypi" alt="Pypi"/>
+<a href="https://pypi.org/project/chatgpt4-cli/"><img src="https://img.shields.io/static/v1?label=Pypi&message=v1.5.3&color=green&logo=pypi" alt="Pypi"/>
 <a href="https://wakatime.com/badge/github/Simatwa/gpt-cli"><img src="https://wakatime.com/badge/github/Simatwa/gpt-cli.svg" alt="wakatime"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=License&message=MIT&color=green&logo=MIT" alt="license"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Development&message=Beta&color=Orange&logo=progress" alt="Progress"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Code Style&message=Black&color=black&logo=Black" alt="Code-style"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=green" alt="Coverage"/></a>
 <a href="https://pepy.tech/project/chatgpt4-cli"><img src="https://static.pepy.tech/badge/chatgpt4-cli" alt="Downloads"/></a>
 </p>
 
 CLI tool for interacting with [ChatGPT](https://openai.com) and [Bard](https://bard.google.com).
-> Generate images with Bing and ChatGPT's DALL-E model.
+> Generate images with BingImageCreator and ChatGPT's DALL-E models.
 
 ![screenshot](https://github.com/Simatwa/gpt-cli/raw/main/assets/Screenshot1.png)
 
 ## [Independencies](requirements.txt)
 
 * [Openai](https://github.com/openai/openai-python)
 * [Numpy](https://github.com/numpy/numpy)
@@ -230,33 +230,33 @@
 <summary>
 
 For more info run `gpt-cli -h`.
 
 </summary>
 
 ```
-╭─────────────────────────────── gpt-cli v1.4.9 ───────────────────────────────╮
+╭─────────────────────────────── gpt-cli v1.5.3 ───────────────────────────────╮
 │                                                                              │
 │             Repo : https://github.com/Simatwa/gpt-cli                        │
 │             By   : Smartwa Caleb                                             │
 ╰──────────────────────────────────────────────────────────────────────────────╯
 usage: gpt-cli [-h] [-v] [-m gpt-3.5-turbo|gpt-4|gpt-4-32k] [-t [0.1-1]]
                [-mt [1-7000]] [-tp [0.1-1]] [-f [0.1-2]] [-p [0.1-2]] [-k KEY]
                [-kp path] [-ic [cyan|green|yellow|red]]
                [-oc [cyan|green|yellow|red]] [-bc [blue,magenta,black,reset]]
                [-pc [cyan|green|yellow|red]] [--prompt [SETTINGS ...]]
                [-tm value] [-pr PROXY] [-rc value] [-g 1,4] [-sp [text ...]]
                [-fp path] [-o path] [-pp prefix] [-rp prefix]
                [-dm keys|values|show|{fnm}] [-dl symbol] [-cf path] [-bk KEY]
-               [-bkp PATH] [-bcf PATH] [-si TIME] [--disable-stream]
-               [--new-record] [--disable-recording] [--zero-show] [--bard]
-               [--markdown] [--update] [--sudo]
+               [-bkp PATH] [-bcf PATH] [-si TIME] [-spin 1|2]
+               [--disable-stream] [--new-record] [--disable-recording]
+               [--zero-show] [--bard] [--markdown] [--update] [--sudo]
                [message ...]
 
-Interact with ChatGPT at the terminal
+Interact with ChatGPT and Bard at the terminal.
 
 positional arguments:
   message               Message to be send.
 
 options:
   -h, --help            show this help message and exit
   -v, --version         show program's version number and exit
@@ -318,14 +318,16 @@
                         Bard's session value
   -bkp PATH, --bard-key-path PATH
                         Path to Bard's key path
   -bcf PATH, --bard-cookie-file PATH
                         Path to Bard's cookie file
   -si TIME, --stream-interval TIME
                         Interval for printing responses in (s)
+  -spin 1|2, --spinner 1|2
+                        Busy bar indicator
   --disable-stream      Specifies not to stream responses from ChatGPT
   --new-record          Override previous chats under the filepath
   --disable-recording   Disable saving prompts and responses
   --zero-show           Specifies not to stdout prompt of the act parsed
   --bard                Make Bard the default GPT
   --markdown            Stdout responses in markdown-format - disables
                         streaming
@@ -359,15 +361,15 @@
 
 - Anyone is free to [fork](https://github.com/Simatwa/gpt-cli/fork), submit an [issue](https://github.com/Simatwa/gpt-cli/issues) without any **guideline** or submitting a [pull request](https://github.com/Simatwa/gpt-cli/pulls).
 
 ### ToDo
 
 - [x] Use dialogue
 - [x] Issue prompt from a file
-- [ ] Busy bar
+- [x] Busy bar
 
   > Review [CHANGELOG](https://github.com/Simatwa/gpt-cli/blob/main/CHANGELOG.md)
 
 ## Acknowledgements
 
 1. [remo7777](https://github.com/remo7777/T-Header)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.5.2 Summary: Interact with
+Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.5.3 Summary: Interact with
 ChatGPT and Bard at the terminal. Home-page: https://github.com/Simatwa/gpt-cli
 Author: Smartwa Caleb Author-email: smartwacaleb@gmail.com Maintainer: Smartwa
 Caleb License: MIT Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/
 issues/new Classifier: License :: OSI Approved :: MIT License Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English Classifier: License :: Free For Home
 Use Classifier: Topic :: Home Automation Classifier: Intended Audience ::
@@ -12,16 +12,16 @@
 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown License-File: LICENSE
                              ****** gpt-cli ******
    [Gihtub] [Pypi]_[wakatime]_[license]_[Progress]_[Code-style]_[Coverage]_
                                   [Downloads]
 CLI tool for interacting with [ChatGPT](https://openai.com) and [Bard](https://
-bard.google.com). > Generate images with Bing and ChatGPT's DALL-E model. !
-[screenshot](https://github.com/Simatwa/gpt-cli/raw/main/assets/
+bard.google.com). > Generate images with BingImageCreator and ChatGPT's DALL-
+E models. ![screenshot](https://github.com/Simatwa/gpt-cli/raw/main/assets/
 Screenshot1.png) ## [Independencies](requirements.txt) * [Openai](https://
 github.com/openai/openai-python) * [Numpy](https://github.com/numpy/numpy) *
 [Colorama](https://github.com/tartley/colorama) * [revChatGPT](https://
 github.com/acheong08/ChatGPT) ### Features - Chat with ChatGPT and Bard
 conversationally. - Let **ChatGPT** and **Bard** chat to each other. - Generate
 Images (DALL-E & BingImageCreator)- Based on your prompt or GPT generated
 description. - Stream or Non-stream responses. - Maintain record of the chats.
@@ -83,74 +83,75 @@
 13._help : Show this help info * Use `./` (fullstop and forward slash) to
 interact with **system commands** - e.g ```./ifconfig``` * Use `_botchat` to
 let the 2 GPTs chat to each other > **Note** You can further specify the GPT to
 be used by appending `--gpt4` or `--bard` in the prompt. * Use *{{f.text-
 filename}}* to issue prompt contained in the 'text-filename'    For more info
 run `gpt-cli -h`.  ```
 â­âââââââââââââââââââââââââââââââ
-gpt-cli v1.4.9
+gpt-cli v1.5.3
 ââââââââââââââââââââââââââââââââ®
 â â â Repo : https://github.com/Simatwa/gpt-cli â â By : Smartwa
 Caleb â
 â°âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
 usage: gpt-cli [-h] [-v] [-m gpt-3.5-turbo|gpt-4|gpt-4-32k] [-t [0.1-1]] [-mt
 [1-7000]] [-tp [0.1-1]] [-f [0.1-2]] [-p [0.1-2]] [-k KEY] [-kp path] [-ic
 [cyan|green|yellow|red]] [-oc [cyan|green|yellow|red]] [-bc
 [blue,magenta,black,reset]] [-pc [cyan|green|yellow|red]] [--prompt [SETTINGS
 ...]] [-tm value] [-pr PROXY] [-rc value] [-g 1,4] [-sp [text ...]] [-fp path]
 [-o path] [-pp prefix] [-rp prefix] [-dm keys|values|show|{fnm}] [-dl symbol]
-[-cf path] [-bk KEY] [-bkp PATH] [-bcf PATH] [-si TIME] [--disable-stream] [--
-new-record] [--disable-recording] [--zero-show] [--bard] [--markdown] [--
-update] [--sudo] [message ...] Interact with ChatGPT at the terminal positional
-arguments: message Message to be send. options: -h, --help show this help
-message and exit -v, --version show program's version number and exit -m gpt-
-3.5-turbo|gpt-4|gpt-4-32k, --model gpt-3.5-turbo|gpt-4|gpt-4-32k ChatGPT model
-to be used -t [0.1-1], --temperature [0.1-1] Charge of the generated text's
-randomness -mt [1-7000], --max-tokens [1-7000] Maximum number of tokens to be
-generated upon completion -tp [0.1-1], --top-p [0.1-1] Sampling threshold
-during inference time -f [0.1-2], --frequency-penalty [0.1-2] Chances of word
-being repeated -p [0.1-2], --presence-frequency [0.1-2] Chances of topic being
-repeated -k KEY, --key KEY OPENAI-API-KEY -kp path, --key-path path Path to
-text-file containing GPT-api key -ic [cyan|green|yellow|red], --input-color
-[cyan|green|yellow|red] Font color for inputs -oc [cyan|green|yellow|red], --
-output-color [cyan|green|yellow|red] Font color for outputs -bc
-[blue,magenta,black,reset], --background-color [blue,magenta,black,reset]
-Console's background-color -pc [cyan|green|yellow|red], --prompt-color
-[cyan|green|yellow|red] Prompt's display color --prompt [SETTINGS ...]
-Customizes the prompt display -tm value, --timeout value Request timeout while
-making request - (Soon) -pr PROXY, --proxy PROXY Pivot request through this
-proxy -rc value, --reply-count value Number of responses to be received -g 1,4,
---gpt 1,4 ChatGPT version to be used -sp [text ...], --system-prompt [text ...]
-Text to train ChatGPT at the start -fp path, --file-path path Path to .csv file
-containing role and prompt - [act,prompt] -o path, --output path Filepath for
-saving the chats - default [/home/smartwa/git/gpt-cli/.chatgpt-history.txt] -pp
-prefix, --prompt-prefix prefix Text to append before saving each prompt -
-default [>>> timestamp] -rp prefix, --response-prefix prefix Text to append
-before saving each response - default [None] -dm keys|values|show|{fnm}, --dump
-keys|values|show|{fnm} Stdout [keys,values]; Save all prompts in json format to
-a file -dl symbol, --delimiter symbol Delimeter for the .CSV file -
-[act,prompt] -cf path, --cookie-file path Path to Bing's cookies - for Edge
-Image Generation -bk KEY, --bard-key KEY Bard's session value -bkp PATH, --
-bard-key-path PATH Path to Bard's key path -bcf PATH, --bard-cookie-file PATH
-Path to Bard's cookie file -si TIME, --stream-interval TIME Interval for
-printing responses in (s) --disable-stream Specifies not to stream responses
-from ChatGPT --new-record Override previous chats under the filepath --disable-
-recording Disable saving prompts and responses --zero-show Specifies not to
-stdout prompt of the act parsed --bard Make Bard the default GPT --markdown
-Stdout responses in markdown-format - disables streaming --update Download
-latest prompts - [awesome-chatgpt-prompts] --sudo Run commands against system
-with sudo privileges ```  > **Note** : **gpt-4** *(model)* supports upto *7000*
-tokens and others *3000*. > **Warning** : **gpt-1** Has issues - *(To be fixed
-later)* Visit [acheong08/Bard](https://github.com/acheong08/Bard) for info on
-how to get the Bard's cookie file and Sessions. ## Motive   Love for `Terminal`
-â¤ï¸  As a `terminal guy` I used to find it uncomfortable to keep shifting
-from one window to next in order to access ChatGPT even after trying out the
-[gpt-login](https://github.com/Simatwa/gpt-login), the rest is [here.](https://
-github.com/Simatwa/gpt-cli)  ## Contributions - Anyone is free to [fork](https:
-//github.com/Simatwa/gpt-cli/fork), submit an [issue](https://github.com/
-Simatwa/gpt-cli/issues) without any **guideline** or submitting a [pull
-request](https://github.com/Simatwa/gpt-cli/pulls). ### ToDo - [x] Use dialogue
-- [x] Issue prompt from a file - [ ] Busy bar > Review [CHANGELOG](https://
-github.com/Simatwa/gpt-cli/blob/main/CHANGELOG.md) ## Acknowledgements 1.
-[remo7777](https://github.com/remo7777/T-Header) 2. [acheong08](https://
+[-cf path] [-bk KEY] [-bkp PATH] [-bcf PATH] [-si TIME] [-spin 1|2] [--disable-
+stream] [--new-record] [--disable-recording] [--zero-show] [--bard] [--
+markdown] [--update] [--sudo] [message ...] Interact with ChatGPT and Bard at
+the terminal. positional arguments: message Message to be send. options: -h, --
+help show this help message and exit -v, --version show program's version
+number and exit -m gpt-3.5-turbo|gpt-4|gpt-4-32k, --model gpt-3.5-turbo|gpt-
+4|gpt-4-32k ChatGPT model to be used -t [0.1-1], --temperature [0.1-1] Charge
+of the generated text's randomness -mt [1-7000], --max-tokens [1-7000] Maximum
+number of tokens to be generated upon completion -tp [0.1-1], --top-p [0.1-1]
+Sampling threshold during inference time -f [0.1-2], --frequency-penalty [0.1-
+2] Chances of word being repeated -p [0.1-2], --presence-frequency [0.1-2]
+Chances of topic being repeated -k KEY, --key KEY OPENAI-API-KEY -kp path, --
+key-path path Path to text-file containing GPT-api key -ic
+[cyan|green|yellow|red], --input-color [cyan|green|yellow|red] Font color for
+inputs -oc [cyan|green|yellow|red], --output-color [cyan|green|yellow|red] Font
+color for outputs -bc [blue,magenta,black,reset], --background-color
+[blue,magenta,black,reset] Console's background-color -pc
+[cyan|green|yellow|red], --prompt-color [cyan|green|yellow|red] Prompt's
+display color --prompt [SETTINGS ...] Customizes the prompt display -tm value,
+--timeout value Request timeout while making request - (Soon) -pr PROXY, --
+proxy PROXY Pivot request through this proxy -rc value, --reply-count value
+Number of responses to be received -g 1,4, --gpt 1,4 ChatGPT version to be used
+-sp [text ...], --system-prompt [text ...] Text to train ChatGPT at the start -
+fp path, --file-path path Path to .csv file containing role and prompt -
+[act,prompt] -o path, --output path Filepath for saving the chats - default [/
+home/smartwa/git/gpt-cli/.chatgpt-history.txt] -pp prefix, --prompt-prefix
+prefix Text to append before saving each prompt - default [>>> timestamp] -rp
+prefix, --response-prefix prefix Text to append before saving each response -
+default [None] -dm keys|values|show|{fnm}, --dump keys|values|show|{fnm} Stdout
+[keys,values]; Save all prompts in json format to a file -dl symbol, --
+delimiter symbol Delimeter for the .CSV file - [act,prompt] -cf path, --cookie-
+file path Path to Bing's cookies - for Edge Image Generation -bk KEY, --bard-
+key KEY Bard's session value -bkp PATH, --bard-key-path PATH Path to Bard's key
+path -bcf PATH, --bard-cookie-file PATH Path to Bard's cookie file -si TIME, --
+stream-interval TIME Interval for printing responses in (s) -spin 1|2, --
+spinner 1|2 Busy bar indicator --disable-stream Specifies not to stream
+responses from ChatGPT --new-record Override previous chats under the filepath
+--disable-recording Disable saving prompts and responses --zero-show Specifies
+not to stdout prompt of the act parsed --bard Make Bard the default GPT --
+markdown Stdout responses in markdown-format - disables streaming --update
+Download latest prompts - [awesome-chatgpt-prompts] --sudo Run commands against
+system with sudo privileges ```  > **Note** : **gpt-4** *(model)* supports upto
+*7000* tokens and others *3000*. > **Warning** : **gpt-1** Has issues - *(To be
+fixed later)* Visit [acheong08/Bard](https://github.com/acheong08/Bard) for
+info on how to get the Bard's cookie file and Sessions. ## Motive   Love for
+`Terminal` â¤ï¸  As a `terminal guy` I used to find it uncomfortable to keep
+shifting from one window to next in order to access ChatGPT even after trying
+out the [gpt-login](https://github.com/Simatwa/gpt-login), the rest is [here.]
+(https://github.com/Simatwa/gpt-cli)  ## Contributions - Anyone is free to
+[fork](https://github.com/Simatwa/gpt-cli/fork), submit an [issue](https://
+github.com/Simatwa/gpt-cli/issues) without any **guideline** or submitting a
+[pull request](https://github.com/Simatwa/gpt-cli/pulls). ### ToDo - [x] Use
+dialogue - [x] Issue prompt from a file - [x] Busy bar > Review [CHANGELOG]
+(https://github.com/Simatwa/gpt-cli/blob/main/CHANGELOG.md) ## Acknowledgements
+1. [remo7777](https://github.com/remo7777/T-Header) 2. [acheong08](https://
 github.com/acheong08/ChatGPT) 3. [f](https://github.com/f/awesome-chatgpt-
 prompts)
```

### Comparing `chatgpt4-cli-1.5.2/setup.py` & `chatgpt4-cli-1.5.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
-from GPTCLI import __version__, __author__, __repo__
+from GPTCLI import __version__, __author__, __repo__, __info__
 
 setup(
     name="chatgpt4-cli",
     packages=["GPTCLI"],
     version=__version__,
     license="MIT",
     author=__author__,
     maintainer=__author__,
     author_email="smartwacaleb@gmail.com",
-    description="Interact with ChatGPT and Bard at the terminal.",
+    description=__info__,
     url=__repo__,
     project_urls={"Bug Report": f"{__repo__}/issues/new"},
     install_requires=[
         "numpy>=1.23.4",
         "colorama>=0.4.6",
         "openai>=0.26.4",
         "revChatGPT==4.0.6",
```

